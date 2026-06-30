# Shared KB — кросс-тенантный кеш знаний

> Спецификация v3.2 — feature flags + метрики 29.06.2026.  
> Проект: `~/baza/` (git), БД: `~/.hermes/shared_kb/solutions.db`  
> **14 коммитов | 146 тестов | ~4000 строк | 100k load test пройден**

## 1. Суть

Каждый раз когда Hermes решает проблему для тенанта — решение сохраняется в общий индекс.  
Когда другой тенант (или тот же) задаёт похожий вопрос — ответ достаётся из кеша, LLM не вызывается.

**Эффект:** экономия токенов от 5 до 60% (Coinbase benchmark), ускорение ответов, накопление опыта.

---

## 2. Где живёт

```
~/baza/                              ← git-репо проекта
├── shared_kb/
│   ├── __init__.py        (28)      ← экспорт публичного API
│   ├── db.py              (823)     ← SQLite+FTS5+WAL, CRUD, конфликты, диалоги
│   ├── search.py          (539)     ← L1/L2/RRF, диалоги, suggestions
│   ├── agent_hook.py      (328)     ← cache-first, multi-turn, confidence, теги
│   ├── cli.py             (305)     ← 12 команд CLI
│   ├── longterm.py        (117)     ← drift, staleness, A/B testing
│   ├── export_obsidian.py (86)      ← экспорт в Obsidian .md + JSONL
│   └── web_ui.py          (234)     ← Flask админ-панель
├── bin/
│   └── shared-kb                     ← symlink → shared_kb/cli.py (chmod +x)
└── tests/                            ← 78 тестов (pytest, sqlite3)

~/.hermes/shared_kb/
├── solutions.db                      ← SQLite + FTS5 (runtime)
└── exports/                          ← Obsidian .md + JSONL экспорты
```

---

## 3. Схема БД (реализована)

```sql
CREATE TABLE IF NOT EXISTS solutions (
    id              TEXT PRIMARY KEY,              -- UUID4
    query_hash      TEXT NOT NULL,                 -- v3.1: NOT UNIQUE — versioned on collision
    query           TEXT NOT NULL,                 -- нормализованный запрос (цены→PRICE, пути→PATH)
    query_original  TEXT,                          -- v3.1: исходный запрос до нормализации
    query_domain    TEXT NOT NULL DEFAULT 'general',
    solution        TEXT NOT NULL,
    solution_type   TEXT NOT NULL DEFAULT 'text',
    tenant_hash     TEXT NOT NULL,                 -- sha256(tenant_id)[:12]
    tokens_saved    INTEGER NOT NULL DEFAULT 0,
    hit_count       INTEGER NOT NULL DEFAULT 0,
    similarity_avg  REAL NOT NULL DEFAULT 0.0,
    downvotes       INTEGER NOT NULL DEFAULT 0,   -- 3 → авто-деактивация
    is_verified     INTEGER NOT NULL DEFAULT 0,   -- ручная верификация админом
    confidence      REAL NOT NULL DEFAULT 0.0,    -- 🆕 0-100, ≥90 → is_verified=1
    feedback_text   TEXT,                          -- текст фидбека
    supersedes      TEXT REFERENCES solutions(id), -- 🆕 версионирование
    version         INTEGER DEFAULT 1,             -- 🆕 версия решения
    created_at      TEXT NOT NULL DEFAULT (datetime('now')),
    last_hit_at     TEXT,
    expires_at      TEXT,                          -- NULL = бессрочно
    is_active       INTEGER NOT NULL DEFAULT 1
);

-- Теги (auto-tagging через дешёвую LLM) 🆕
CREATE TABLE IF NOT EXISTS solution_tags (
    solution_id TEXT REFERENCES solutions(id),
    tag TEXT,
    PRIMARY KEY (solution_id, tag)
);

-- Multi-turn диалоги 🆕
CREATE TABLE IF NOT EXISTS conversations (
    id          TEXT PRIMARY KEY,
    thread_hash TEXT NOT NULL,                    -- sha256 первых 3 сообщений
    messages    TEXT NOT NULL,                     -- JSON: [{role, content}, ...]
    domain      TEXT NOT NULL DEFAULT 'general',
    created_at  TEXT NOT NULL DEFAULT (datetime('now')),
    last_hit_at TEXT
);

-- FTS5 индексы
CREATE VIRTUAL TABLE IF NOT EXISTS solutions_fts USING fts5(
    query, solution, query_domain,
    content='solutions', content_rowid='rowid'
);
CREATE VIRTUAL TABLE IF NOT EXISTS conversations_fts USING fts5(
    messages, domain,
    content='conversations', content_rowid='rowid'
);

-- v3.1: кеш переписанных запросов (экономия токенов на L3)
CREATE TABLE IF NOT EXISTS query_rewrites (
    original_hash   TEXT PRIMARY KEY,              -- sha256(original)
    original        TEXT NOT NULL,
    rewritten       TEXT NOT NULL,
    domain          TEXT NOT NULL DEFAULT 'general',
    hit_count       INTEGER NOT NULL DEFAULT 1,
    created_at      TEXT NOT NULL DEFAULT (datetime('now')),
    last_hit_at     TEXT
);

-- Статистика доменов (материализованная)
CREATE TABLE IF NOT EXISTS domain_stats (
    domain TEXT PRIMARY KEY,
    total_solutions INTEGER, total_hits INTEGER,
    tokens_saved INTEGER, last_updated TEXT
);

-- PRAGMA: journal_mode=WAL, busy_timeout=5000, user_version=2
-- Транзакции: DEFERRED + with conn: (атомарные INSERT+триггеры+domain_stats)
-- Индексы: query_hash+is_active, tenant_hash+is_active, expires_at (partial)
```

---

## 4. Поисковый движок

### 4.1. Трёхуровневый поиск с RRF (гибридный) ✅

```
shared_kb.search(query, domain=None, threshold=0.75)
  │
  ├─ L1: Точное совпадение (query_hash)
  │     └─ normalize_query → sha256 → lookup в solutions
  │        └─ HIT → similarity=1.0, hit_level=L1_HASH → ✅ мгновенно
  │
  ├─ L2: Гибридный поиск — BM25 + Semantic (RRF, k=60)
  │     └─ Параллельно:
  │        ├─ BM25: FTS5 MATCH с term1* OR term2* ... + domain фильтр
  │        └─ Semantic: SentenceTransformer (опционально, если доступен)
  │     └─ RRF-фьюжн: score = Σ 1/(60 + rank) для каждого метода
  │        └─ HIT если score ≥ threshold → hit_level=L2_RRF
  │
  └─ L3: Query Rewriting (дешёвая LLM) 🔄
        └─ GPT-4o-mini переписывает запрос в каноническую форму
           └─ Повторный поиск с переписанным запросом
```

### 4.2. Нормализация запроса

```python
def normalize_query(text: str) -> str:
    text = text.lower().strip()
    text = re.sub(r'[^\w\s\-\>\.\,\#\+/]', ' ', text)      # пунктуация
    text = re.sub(r'\b\d{1,3}\.\d{1,6}\b', 'PRICE', text)  # цены
    text = re.sub(r'\b\d{4}-\d{2}-\d{2}\b', 'DATE', text)   # даты
    text = re.sub(r'-?\b\d{8,15}\b', 'CHAT_ID', text)       # Telegram ID
    text = re.sub(r'/[\w/]+/[\w\.\-]+', 'PATH', text)        # пути
    text = re.sub(r'\b[\w_]+=.+', 'VAR=VAL', text)           # env vars
    text = re.sub(r'@\w+', '@USER', text)                    # юзернеймы
    text = re.sub(r'\s+', ' ', text)
    return text.strip()
```

### 4.3. Ранжирование

```python
def rank_results(hits, target_domain, query_len):
    for h in hits:
        score = 1.0

        # BM25: FTS5 возвращает ОТРИЦАТЕЛЬНЫЕ числа (-15.2 = отлично, -2.1 = слабо)
        bm25 = h.get('bm25_score')
        if bm25 is not None:
            bm25_abs = abs(bm25)
            bm25_mult = min(2.0, 1.0 + (bm25_abs / 20.0))
            score *= bm25_mult

        if domain == target_domain:   score *= 1.5             # domain boost
        decay = max(0.5, 0.95 ** days_since_last_hit)          # recency
        score *= decay
        if hit_count > 5:             score *= 1.2             # proven solution
        if downvotes >= 3:            score *= 0.5             # penalty
        score *= (confidence / 100) if confidence else 1.0     # 🆕 confidence boost
        h['_score'] = min(score, 1.0)
```

### 4.4. Логика HIT/MISS

```
score >= 0.85 → STRONG HIT  → вернуть кеш + Proactive Suggestions + пропустить LLM
score 0.75-0.84 → WEAK HIT  → вернуть кеш + "🤔 похоже на ваш случай?"
score < 0.75 → MISS         → LLM + сохранить в кеш
```

### 4.5. Dangerous command filter

Перед возвратом STRONG HIT — solution проверяется на деструктивные паттерны (`rm -rf /`, `dd if=`, `git push --force master`, `chmod 777`, `shutdown`). Если найдено → форсированный MISS.

---

## 5. Сохранение (agent_hook.save_solution)

### 5.1. Когда сохранять

- После успешного LLM-ответа на вопрос
- Ответ >10 символов, вопрос >20 символов
- Нет опасных команд в ответе
- Нет кредов/токенов в вопросе и ответе

### 5.2. Что НЕ сохранять (фильтры)

```python
BLOCK_PATTERNS = [
    r'\b[0-9a-f]{40}\b',                # SHA — возможные ключи
    r'sk-[A-Za-z0-9]{32,}',             # OpenAI ключи
    r'ghp_[A-Za-z0-9]{36}',             # GitHub токены
    r'Bearer\s+[A-Za-z0-9\-_\.]+=*',    # Bearer токены
    r'api_key\s*=\s*[\'"]\S+[\'"]',     # API ключи в коде
    r'\b\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\b',  # IP адреса
]
```

### 5.3. TTL по доменам

| Домен | TTL | Причина |
|-------|-----|---------|
| trading | 90 дней | API меняются |
| python | 180 дней | Код устаревает |
| infra | 180 дней | Инфра эволюционирует |
| vpn | 90 дней | Конфиги меняются |
| auto | ∞ | Физика не устаревает |
| general | 365 дней | Медленный износ |

---

## 6. Приватность

### 6.1. Обезличивание

- `tenant_hash` = `sha256(str(tenant_id))[:12]` — необратимый
- `normalize_query` удаляет имена, CHAT_ID, пути, цены
- `anonymize_query` заменяет @username → @USER

### 6.2. Доступ

- **Админ (Море):** полный доступ, статистика по тенантам
- **Тенанты:** только через `search()` — не видят tenant_hash
- **Внешние:** доступа нет

---

## 7. CLI

```bash
# Поиск
shared-kb search "шорт стоплосс выбивает" --domain trading
shared-kb search "indentationerror gateway" --domain python -t 0.7

# Сохранение (ручное)
shared-kb store "шорт SL fix" "entry * 1.05 для SHORT" --domain trading

# Статистика
shared-kb stats
shared-kb stats --domain trading

# Дедупликация (по префиксу первых 50 символов)
shared-kb dedup --similarity 0.92 --dry-run
shared-kb dedup --auto

# Конфликты 🆕
shared-kb conflicts                          # найти противоречивые решения
shared-kb conflicts --auto-resolve           # авто-merge безопасных

# Drift Detection 🆕
shared-kb drift                              # найти дрейфующие решения
shared-kb drift --domain trading

# Staleness Detection 🆕
shared-kb staleness                          # найти просроченные решения
shared-kb staleness --domain python

# Очистка
shared-kb vacuum              # FTS5 оптимизация
shared-kb cleanup --ttl 90    # деактивация просроченных

# Экспорт
shared-kb export                            # JSONL в stdout
shared-kb export --format obsidian --output ~/obsidian-vault/kb/
```

### Web UI 🆕

```bash
shared-kb web                    # Flask на http://127.0.0.1:8767
shared-kb web --port 9000        # кастомный порт
```

**Страницы:**
- `/` — Dashboard (статистика, графики)
- `/solutions` — таблица решений с поиском/фильтрами
- `/api/search?q=...` — REST API поиска

---

## 8. Интеграция с Hermes

### 8.1. Конституция (§XV)

```
Перед ЛЮБЫМ LLM-вызовом для ответа на вопрос:
  → shared_kb.check_cache(query)
     → STRONG HIT (≥0.85) → вернуть из кеша + suggestions, LLM не вызывать
     → WEAK HIT (0.75-0.84) → показать кеш + спросить «это ваш случай?»
     → MISS → LLM → shared_kb.save_solution()
```

### 8.2. Код интеграции

```python
import sys; sys.path.insert(0, '/home/openclaw/baza')
from shared_kb import check_cache, save_solution

# Перед LLM:
cached = check_cache(user_message)
if cached and cached['hit_type'] == 'STRONG':
    return f"⚡ Из кеша: {cached['solution']}"

# После успешного LLM-ответа:
save_solution(query=user_message, solution=response, tenant_id=chat_id)
```

### 8.3. Определение домена

```python
DOMAIN_PATTERNS = {
    'trading': ['bybit', 'шорт', 'лонг', 'SL', 'TP', 'Bollinger', 'позици', 'стоплосс'],
    'python':  ['import', 'def ', 'class ', 'ошибк', 'exception', 'python', 'traceback'],
    'auto':    ['двигател', 'тормоз', 'VW', 'T-Roc', 'EPC', 'датчик', 'колес'],
    'infra':   ['gateway', 'systemd', 'рестарт', 'сервер', 'deploy', 'ssh', 'docker'],
    'vpn':     ['vpn', 'xray', 'vless', 'ключ', 'трафик', 'hysteria'],
    'general': [],
}
```

---

## 9. Метрики и мониторинг

| Метрика | Описание | Хранение |
|---------|----------|----------|
| `hit_rate` | % запросов из кеша | domain_stats |
| `tokens_saved` | ~токенов не потрачено | solutions.tokens_saved |
| `cache_size` | активных решений | COUNT(is_active=1) |
| `avg_similarity` | средняя схожесть hit'ов | solutions.similarity_avg |
| `downvotes` | негативных фидбеков | solutions.downvotes |

---

## 10. Фидбек-луп

```
Пользователь поправил кешированный ответ
  → handle_negative_feedback(solution_id, "не подходит потому что...")
     → downvotes += 1
        → если downvotes >= 3 → is_active = 0 (авто-деактивация)
```

---

## 11. Питфоллы (учтены при реализации)

| Риск | Решение |
|------|---------|
| SQLite блокировки при concurrent writes | `PRAGMA journal_mode=WAL` + `busy_timeout=5000`. Все write-операции обёрнуты в `with conn:` |
| Кеш галлюцинаций | 3 downvotes → деактивация, фидбек-текст для аудита |
| Устаревание (API v1→v2) | TTL по доменам: trading 90д, python 180д, auto ∞ |
| Контекстная привязка (пути, цены) | `normalize_query` заменяет PATH/PRICE/DATE/CHAT_ID |
| Деструктивные команды в кеше | Dangerous command filter при search() — форсирует MISS |
| CHAT_ID с минусом (Telegram супергруппы) | Regex `-?\b\d{8,15}\b` вместо `\b\d{8,}\b` |
| FTS5 отрицательные BM25 | `abs(bm25)` с нормализацией в множитель 1.0–2.0 |
| Составные слова (стоп-лосс) | Разбиваются на OR-токены (`стоп*` + `лосс*`) |
| Точки в FTS5 запросах | Экранируются/удаляются (синтаксическая ошибка FTS5) |
| Exact-конфликты невозможны | `UNIQUE query_hash` гарантирует — конфликты только approximate |

---

## 12. Реализованные файлы

| Файл | Строк | Назначение |
|------|-------|-----------|
| `shared_kb/__init__.py` | 28 | Экспорт публичного API |
| `shared_kb/db.py` | 823 | SQLite+FTS5+WAL, CRUD, конфликты, диалоги |
| `shared_kb/search.py` | 539 | L1/L2/RRF, поиск диалогов, suggestions |
| `shared_kb/agent_hook.py` | 328 | cache-first, multi-turn, confidence, теги |
| `shared_kb/cli.py` | 305 | 12 команд CLI |
| `shared_kb/longterm.py` | 117 | drift, staleness, A/B testing |
| `shared_kb/export_obsidian.py` | 86 | экспорт в Obsidian .md + JSONL |
| `shared_kb/web_ui.py` | 234 | Flask админ-панель |
| **Итого** | **2460** | |

---

## 13. Критерии успеха

- [x] `shared-kb search "шорт стоплосс"` находит решение (L1_HASH)
- [x] 3 downvotes → деактивация
- [x] WAL mode, конкурентные запросы не блокируются
- [x] Опасные команды фильтруются
- [x] Тенант не видит чужих tenant_hash
- [x] Креды/токены не сохраняются
- [x] 78 тестов зелёные, покрытие всех модулей
- [x] Git-история чистая (11 коммитов)
- [ ] Hit rate > 20% через 2 недели (cold start — нужен прогрев)

---

## 14. Реализованные фичи v3.0 ✅

### Quick Wins (реализовано)

| Фича | Статус | Коммит | Описание |
|------|--------|--------|----------|
| Hybrid Search (RRF) | ✅ | `48a678e` | Параллельный BM25 + Semantic, Reciprocal Rank Fusion (k=60) |
| Query Rewriting | ✅ | `48a678e` | Дешёвая LLM переписывает запрос в каноническую форму |
| Solution Versioning | ✅ | `48a678e` | `supersedes` + `version`, архив вместо удаления |
| Confidence Scoring | ✅ | `48a678e` | Эвристическая оценка 0-100, ≥90 → is_verified=1 |
| Auto-Tagging | ✅ | `48a678e` | Теги через дешёвую LLM, таблица `solution_tags` |

### v3.0 Core (реализовано)

| Фича | Статус | Коммит | Описание |
|------|--------|--------|----------|
| Multi-turn Context Cache | ✅ | `19263f9` | Кеширование целых диалогов, `conversations` + FTS5 |
| Conflict Detection | ✅ | `ac436f1` | Jaccard similarity, три уровня: merge/review/review |
| Proactive Suggestions | ✅ | `a7b1128` | Связанные решения при STRONG hit по тегам → domain fallback |
| Export в Obsidian | ✅ | `43cd498` | .md с YAML frontmatter + JSONL |

### Long-term Vision (реализовано)

| Фича | Статус | Коммит | Описание |
|------|--------|--------|----------|
| Drift Detection | ✅ | `cece1ae` | BM25-кластеризация, поиск дрейфующих решений |
| Staleness Detection | ✅ | `cece1ae` | TTL-based авто-обнаружение просроченных |
| A/B Testing | ✅ | `cece1ae` | Фреймворк с трекингом метрик (cache vs LLM) |
| Web UI (Flask) | ✅ | `e7b8f99` | Dashboard + Solutions + REST API на :8767 |

---

## 15. Что дальше (v4.0)

| Фича | Effort | Impact | Статус |
|------|--------|--------|--------|
|| Federated KB (P2P sync) | 2 недели | Масштабирование | ⏳ TODO |
|| Learning to Rank (XGBoost) | 1 неделя | Адаптивное ранжирование | ⏳ TODO |
|| L3 Semantic (SentenceTransformer) | 2 дня | +5-10% hit rate | ⏳ Опционально |

---

## 16. v3.1 Changelog (фиксы после рецензии)

### 🔴 Критичное
| # | Что | Как исправлено |
|---|-----|---------------|
| 1 | **Коллизии query_hash** — UNIQUE ломал вставку при одинаковой нормализации | `query_hash NOT NULL` без UNIQUE, при коллизии — версионирование (supersedes + version++), оригинальный запрос в `query_original` |
| 2 | **tenant_hash без соли** — rainbow-атака возможна | `_salted_tenant_hash()`: `sha256(tenant_id:SALT)[:16]`, соль из `$SHARED_KB_SALT` или default |
| 3 | **BLOCK_PATTERNS неполный** — приватные ключи, JWT, AWS, Slack | Добавлено 9 паттернов: RSA/EC/OPENSSH ключи, JWT, AKIA, xox*, GitHub OAuth/PAT, телефоны, email |
| 4 | **DANGEROUS_PATTERNS неполный** — SQL/кубер | Добавлено: DROP TABLE/DATABASE, TRUNCATE, kubectl delete ns, DELETE без WHERE |
| 5 | **Хардкод пути** `/home/openclaw/baza` в спеке | Исправлено: код использует относительные импорты. В спеке — `PYTHONPATH` или `pip install -e` |

### 🟡 Важное
| # | Что | Как исправлено |
|---|-----|---------------|
| 6 | **Цены без копеек** — `\d{1,3}\.\d{1,6}` не ловил `100` | Regex: `\b\d{1,10}[.,]\d{1,6}\b`, даты/chat_id обрабатываются раньше |
| 7 | **confidence — чёрный ящик** | Формула зафиксирована: baseline 50 + длина ответа + код/пути + конкретность |
| 8 | **similarity_avg — среднее арифметическое** | Заменено на EMA: `0.9 × old + 0.1 × new` |
| 9 | **Нет индексов** для tenant/expires | Добавлены: `idx_tenant(tenant_hash, is_active)`, `idx_expires(expires_at) WHERE is_active=1` |
| 10 | **L3 rewrite — платные вызовы LLM** | Кеш `query_rewrites`: `sha256(original) → rewritten`, hit_count |
| 11 | **Dangerous filter без внешнего конфига** | `dangerous_patterns.yaml` — можно редактировать без перекомпиляции |

### 🟢 Инфраструктура
| # | Что | Как исправлено |
|---|-----|---------------|
| 12 | **Миграции БД** | `PRAGMA user_version = 2` в `init_db()` |
| 13 | **Нет бэкапов** | `backup-kb.py` + cron ежедневно в 03:00 (ротация: 7 daily + 4 weekly) |
| 14 | **Тесты** | 78 → 105: +27 тестов на collision, salt, EMA, BLOCK_PATTERNS, rewrite cache, dangerous patterns, query_original, schema version |

### 📊 Итоговые метрики v3.1

| Метрика | v3.0 | v3.1 |
|---------|------|------|
| Коммитов | 11 | 12 |
| Тестов | 78 | **105** |
| Строк кода | ~2460 | **~3100** |
| Таблиц БД | 5 | **6** (+query_rewrites) |
| BLOCK_PATTERNS | 7 | **16** |
| DANGEROUS_PATTERNS | 13 | **19** |

---

## 17. Валидаторы спеки (v3.1)

Два инструмента проверки соответствия кода спеке:

### 17.1. Статический валидатор

```bash
python3 scripts/validate_spec.py
```

**114 проверок** — без запуска БД, за секунды:
- Все файлы на месте, строки в допуске
- Публичный API (17 экспортов)
- CLI-команды (11 шт.)
- Таблицы БД (7 шт.) и колонки (10 шт.)
- BLOCK_PATTERNS ≥ 14, DANGEROUS_PATTERNS ≥ 17
- Домены, TTL, уровни поиска, нормализация
- Все 17 фич v3.0/v3.1
- PRAGMA, индексы, backup cron

### 17.2. Интеграционные тесты

```bash
pytest tests/test_spec_validation.py -v
```

**41 тест** — проверяет поведение против реальной БД:

| Класс | Тестов | Что проверяет |
|-------|--------|---------------|
| `TestSchema` | 6 | Таблицы, колонки, WAL, FTS5-триггеры, NOT UNIQUE, user_version |
| `TestNormalization` | 8 | PRICE/DATE/PATH/CHAT_ID/@USER + детерминизм |
| `TestSecurityFilters` | 6 | BLOCK_PATTERNS ловят секреты, save_solution reject |
| `TestDangerousFilter` | 7 | Опасные команды → blocked |
| `TestHitMissLogic` | 2 | STRONG HIT / MISS |
| `TestFeedbackLoop` | 1 | 3 downvotes → деактивация |
| `TestTTL` | 2 | trading=90д, auto=∞ |
| `TestPrivacy` | 2 | tenant_hash salted, search не светит |
| `TestSuccessCriteria` | 4 | Все 7 критериев из §13 |
| `TestPitfalls` | 3 | Минус-чатид, составные слова, точки в FTS5 |

### 17.3. Полный прогон

```bash
pytest tests/ -q
# 146 passed — все тесты (105 базовых + 41 spec-валидация)
```

---

## 18. Итоговые метрики (v3.0 → v3.1)

| Метрика | v3.0 | v3.1 |
|---------|------|------|
| Коммитов | 11 | **13** |
| Тестов | 78 | **146** |
| Строк кода | ~2460 | **~3500** |
| Таблиц БД | 5 | **6** (+query_rewrites) |
| BLOCK_PATTERNS | 7 | **16** |
| DANGEROUS_PATTERNS | 13 | **19** |
| Статических проверок | 0 | **114** |
| Интеграционных тестов | 0 | **41** |
| CLI команд | 12 | 12 |
| Backup cron | ❌ | ✅ ежедневно 03:00 |

---

## 19. v3.2 — Feature Flags + Метрики

### 19.1. Feature Flags

Конфиг: `~/.hermes/shared_kb/config.yaml`

```yaml
features:
  # Основные (всегда включены)
  l1_exact_match: true
  l2_bm25_search: true
  l2_tag_search: true
  rrf_fusion: true
  proactive_suggestions: true
  dangerous_filter: true
  block_secrets: true

  # Экспериментальные (поэтапное включение)
  semantic_search: false       # SentenceTransformer
  llm_rewrite: false           # GPT-4o-mini
  llm_confidence: false        # LLM confidence
  llm_tagging: false           # LLM auto-tagging
  ab_testing: false            # A/B cache vs LLM
```

**Принцип:** менять без перезапуска — перечитывается каждые 5 секунд. Каждый флаг оборачивает соответствующий участок кода: `if flags.is_on('semantic_search'): ...`

### 19.2. Operational Metrics

Модуль `config.py` — `MetricsCollector` (in-memory, thread-safe):

| Метрика | Описание |
|---------|----------|
| `total_searches` | Всего поисков |
| `hit_rate` | % попаданий в кеш |
| `by_level` | Распределение по L1_HASH / L2_BM25 / MISS |
| `latency p50/p95/p99` | Перцентили задержки (последние 1000 запросов) |
| `secrets_blocked` | Заблокировано попыток сохранить секреты |
| `dangerous_blocked` | Заблокировано опасных команд |

### 19.3. Health Endpoint

```bash
curl http://127.0.0.1:8767/health
```

```json
{
  "status": "healthy",
  "hit_rate": 66.7,
  "latency_p50_ms": 0.63,
  "latency_p95_ms": 0.89,
  "total_searches": 502,
  "secrets_blocked": 1,
  "dangerous_blocked": 0
}
```

### 19.4. Metrics Endpoint

```bash
curl http://127.0.0.1:8767/metrics
# → полный дамп: metrics + feature flags
```

### 19.5. Нагрузочный тест (100k решений)

```bash
python3 tests/load_test_100k.py -n 100000 --search-samples 500
```

| Метрика | 10k | 100k |
|---------|-----|------|
| БД | 7.2 MB | **71.9 MB** |
| Insert speed | — | 589/s |
| L1 hit rate | 100% | 100% |
| L1 p50 | 0.55ms | **0.63ms** |
| L1 p95 | 0.80ms | 0.89ms |
| Cold p50 | 1.34ms | 1.78ms |
| False positives | 0 | **0** |

---

## 20. Итоговые метрики (v3.0 → v3.2)

| Метрика | v3.0 | v3.1 | v3.2 |
|---------|------|------|------|
| Коммитов | 11 | 13 | **14** |
| Тестов | 78 | 146 | 146 |
| Строк кода | ~2460 | ~3500 | **~4000** |
| Feature flags | ❌ | ❌ | **✅ 12 флагов** |
| Operational metrics | ❌ | ❌ | **✅ latency/hit-rate** |
| Health endpoint | ❌ | ❌ | **✅ /health + /metrics** |
| Load test (100k) | ❌ | ❌ | **✅ пройден** |
| Backup cron | ❌ | ✅ | ✅ |
