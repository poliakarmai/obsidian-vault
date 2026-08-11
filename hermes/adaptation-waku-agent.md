# Адаптация waku-agent → multi-tenant Hermes

> Анализ архитектуры [waku-agent](https://github.com/ShenSeanChen/waku-agent) (991⭐) и план адаптации трёх ключевых механизмов под оркестрацию тенантов Hermes.
> Дата: 09.08.2026

---

## Контекст: что есть в Hermes сейчас

| Характеристика | Hermes (текущий) | waku-agent |
|---|---|---|
| Тенанты | 10 (через channel_profiles) | 1 (personal agent) |
| Контекст при старте | 6 baseline-скиллов (~15K токенов) **каждый ход** | Retrieval gate решает |
| Изоляция | disabled_toolsets + Linux users + iptables | SQLite state.db, всё локально |
| Память | Obsidian vault + memory tool | state.db (FTS5) + MEMORY.md mirror |
| Loop | Встроен в gateway | 95 строк Python, observer-паттерн |
| Consolidation | Нет | Батчами (после N чатов), дешёвой моделью |
| Graphs | delegate_task (spawn sub-agents) | Graph engine: параллельные ноды + детерминированные роутеры |

---

## 🎯 1. Retrieval Gate → Tenant Context Gate

### Проблема
Hermes грузит 6 baseline-скиллов (~15K токенов) при КАЖДОМ старте сессии (через SOUL.md). Для тенантов это:
- Лишние токены на простые запросы («привет», «как дела», «сколько времени»)
- Раздувание контекста → деградация на длинных сессиях
- ~$0.003 за каждый skip'абельный ход (при 80% cache hit)

### Решение: Tenant Context Gate

```
tenant_message → [TenantContextGate] → skip (быстрый ответ) / retrieve (полный контекст)
```

**Архитектура:**

```python
# ~/.hermes/scripts/tenant_context_gate.py

GATE_PROMPT = """Ты — retrieval gate персонального ассистента.
Дан запрос пользователя. Реши, нужен ли для ответа доступ к долговременной памяти
(факты о пользователе, проектах, предпочтениях, прошлых событиях).

Ответь ТОЛЬКО JSON:
{"retrieve": true/false, "query": "<поисковый запрос если true>", "reason": "<5 слов>"}

Общие знания, математика, small talk → false.
Всё что касается пользователя, его проектов, планов → true.

Запрос: {message}"""

def should_load_context(message: str) -> tuple[bool, str]:
    """Вызывается ПЕРЕД загрузкой baseline-скиллов."""
    # Дешёвая модель (deepseek-v4-flash, ~100 токенов)
    response = cheap_llm(GATE_PROMPT.format(message=message))
    decision = parse_json(response)
    return decision["retrieve"], decision.get("query", "")
```

**Multi-tenant адаптация:**

| Компонент | Реализация |
|-----------|-----------|
| Гейт на стороне gateway | Перед `_handle_message_with_agent()` → вызов gate |
| Tenant-specific | Каждый tenant имеет свой `retrieval_gate_threshold` в `config.yaml` |
| Fail-open | Если gate упал → грузим полный контекст (безопасность) |
| Кеширование | Если `retrieve=false`, кешируем SOUL.md/system prompt без инжекции скиллов |

**Экономия:**
- ~80% простых запросов → skip (~12K токенов экономии на каждом)
- При 20 сообщениях/день/тенант → ~240K токенов/день → ~$0.06/день экономии на всех тенантах
- Pro-тенанты: бюджет 5M TPM расходуется медленнее

### План внедрения

**Фаза 1 — A/B тест (неделя 1):**
1. `context_gate_enabled: false` по умолчанию
2. Включаем для 2 тестовых тенантов
3. Метрики: skip_rate, false_negative_rate, cost_savings

**Фаза 2 — rollout (неделя 2):**
4. Включаем для всех тенантов
5. Добавляем `context_gate_override` — пользователь может форсировать full context (`/full`)

---

## 🕸️ 2. Graph Workflows → Tenant Triage Router

### Проблема
Сейчас Hermes обрабатывает ВСЕ сообщения через полный пайплайн: загрузка контекста → LLM → tools. Нет дифференциации по сложности запроса.

### Решение: Tenant Triage Graph

```
tenant_message
    ↓
┌───────────────────────────────────────┐
│  [classify]  ← дешёвая модель (flash) │
│  [check_quota] ← локально, параллельно │
│       ↓                               │
│  router(state) → Python-функция       │
│       ↓                               │
│  ┌──────┐  ┌──────┐  ┌──────────┐    │
│  │quick │  │ look │  │full_agent│    │
│  │reply │  │  up  │  │(loop)    │    │
│  └──────┘  └──────┘  └──────────┘    │
│  малая     поиск по   полный агент    │
│  модель    vault      + tools         │
└───────────────────────────────────────┘
```

**Классы запросов:**

| Класс | Пример | Куда | Модель |
|-------|--------|------|--------|
| `small_talk` | «привет», «спасибо», «как дела» | `quick_reply` | flash |
| `lookup` | «какая у меня подписка», «что в календаре» | `lookup` | flash + прямой SQL/vault |
| `agent` | «составь отчёт по трубам», «разверни VPN» | `full_agent` | pro (текущий loop) |

**Multi-tenant роутер:**

```python
# ~/.hermes/scripts/triage_router.py

def route(state: dict) -> str:
    """Детерминированный роутер — код, не LLM."""
    intent = state.get("intent")       # от classify
    quota_ok = state.get("quota_ok")   # от check_quota
    
    if not quota_ok:
        return "quota_exceeded"
    
    if intent in ("small_talk", "greeting"):
        return "quick_reply"
    elif intent in ("lookup", "status"):
        return "lookup"
    elif intent in ("agent", "complex"):
        return "full_agent"
    
    return "full_agent"  # default → безопасность
```

**Tenant-specific classify:**

```python
# classify использует tenant-specific контекст:
# - Тариф (pro/demo/expert) → разные пороги
# - История интентов → кеш для ускорения
# - Tenant-specific keywords (трубы, дроны, трейдинг)
```

### План внедрения

**Фаза 1 — graph engine (неделя 1):**
1. `waku/graph/engine.py` → адаптировать как `~/.hermes/hermes_graph/engine.py`
2. Nodes: fn, llm, agent (три типа)
3. Waves: параллельные ноды через ThreadPoolExecutor
4. Routers: Python-функции, детерминированные
5. Guards: per-node max_visits + global max_steps

**Фаза 2 — triage graph (неделя 2):**
6. Classify + check_quota → параллельно
7. Router → quick/lookup/full_agent
8. Fail-open → любой сбой → full_agent

**Фаза 3 — tenant graphs (неделя 3):**
9. Tenant-specific графы в `profiles/<tenant>/graphs/`
10. Возможность переопределять дефолтный triage

---

## 🧠 3. Consolidation → Tenant Memory Distiller

### Проблема
Сейчас память в Hermes обновляется через `memory` tool — агент должен явно вызвать его. Нет автоматической консолидации истории чатов в durable facts.

### Решение: Tenant Memory Distiller

```
чат-лог тенанта (N сообщений)
    ↓
consolidate_if_due(every_n=10)
    ↓
дешёвая модель (flash) дистиллирует:
    ├── facts → semantic memory (vault/state.db)
    └── episode → episodic memory (vault/state.db)
```

**Multi-tenant адаптация:**

| Параметр | Значение | Комментарий |
|----------|---------|-------------|
| `every_n` | 10 сообщений | После каждых 10 обменов (user+assistant) |
| Модель | deepseek-v4-flash | Дешёвая, ~$0.0001/консолидация |
| Хранилище | Tenant vault + state.db | Двойная запись: SQLite + MEMORY.md |
| Асинхронность | После ответа пользователю | Не блокирует ход |
| Loss-safe | При ошибке — лог остаётся неконсолидированным | Не теряем данные |

**Что дистиллируется:**

```json
{
  "facts": [
    {"subject": "Клиент D.V.", "content": "Заинтересован в трубах 530×8 ст.20"},
    {"subject": "Проект Алхимик", "content": "Дроны, этап тестирования прошивки"}
  ],
  "episode": "09.08.2026: обсудили поставку труб для D.V., согласовали цены"
}
```

### План внедрения

**Фаза 1 — consolidation engine (неделя 1):**
1. `~/.hermes/scripts/memory_distiller.py`
2. SQLite-таблица `chat_log` в каждом tenant vault
3. `consolidate_if_due(every_n)` — проверка и дистилляция

**Фаза 2 — интеграция (неделя 2):**
4. Gateway пишет в `chat_log` после каждого хода
5. Consolidation вызывается асинхронно после ответа
6. Результаты пишутся в tenant vault (`facts.md` + `episodes.md`)
7. Cron для периодической сверки

---

## 📊 Экономический эффект

| Механизм | Экономия токенов/ход | При 200 ходов/день | $/месяц |
|----------|---------------------|--------------------|---------|
| Context Gate | ~12K (при skip) × 80% skip rate | ~1.9M/день | ~$15 |
| Triage Router | ~10K (при quick/lookup) × 60% | ~1.2M/день | ~$10 |
| Memory Distiller | +500/ход (запись в chat_log) | −0.1M/день | +$0.80 |
| **Итого** | | **~3M/день экономии** | **~$24** |

---

## 🏗️ Файлы и скрипты

| Файл | Назначение |
|------|-----------|
| `~/.hermes/scripts/tenant_context_gate.py` | Retrieval Gate: skip vs retrieve |
| `~/.hermes/scripts/triage_router.py` | Graph router: quick/lookup/full_agent |
| `~/.hermes/scripts/memory_distiller.py` | Consolidation engine |
| `~/.hermes/hermes_graph/engine.py` | Graph engine (адаптация waku/graph/engine.py) |
| `~/.hermes/hermes_graph/triage.py` | Triage graph definition |
| `~/.hermes/config.yaml` | + `context_gate_enabled`, `triage_enabled` |
| `profiles/<tenant>/config.yaml` | + `retrieval_gate_threshold`, `consolidation_every_n` |

---

## ⚠️ Риски

| Риск | Mitigation |
|------|-----------|
| Gate false-negative (нужен контекст, а skip) | Fail-open: при сомнении → retrieve |
| Triage misclassification (сложный запрос → quick reply) | Fail-open: default → full_agent |
| Consolidation garbage (плохие факты) | Loss-safe: лог остаётся, можно передистиллировать |
| Увеличение latency (gate + triage → +500ms) | Кеширование решений gate, параллельные ноды в triage |
| Tenant-specific не учтён | У каждого tenant свои пороги в config.yaml |
