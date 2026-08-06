# HERMES — Мастер-документ оркестрации

> **Версия:** 2026-08-06 v5 (+Router +Isolation +Cron +Secrets) (+RBAC +Observability +Quota +Alerts +Lifecycle) | **Автор:** Море (admin)
> **Назначение:** Единый источник правды по всей Hermes-инфраструктуре — кодовая база, скиллы, инстинкты, тенанты, архитектура.

---

## 1. Архитектура

```
┌─────────────────────────────────────────────────────────┐
│                    HERMES GATEWAY                        │
│  systemd: hermes-gateway.service | RAM: ~900MB           │
│  telegram + whatsapp + local                             │
├─────────────────────────────────────────────────────────┤
│  ┌──────────┐  ┌──────────┐  ┌──────────┐              │
│  │  МОРЕ    │  │MOREARBOT │  │  APOLAI  │  ... 14 шт   │
│  │ default  │  │morearbot │  │  apolai  │              │
│  │ полный   │  │ урезан   │  │ урезан   │              │
│  │ доступ   │  │ chat+pay │  │ chat+pay │              │
│  └──────────┘  └──────────┘  └──────────┘              │
├─────────────────────────────────────────────────────────┤
│  profiles/<tenant>/                                     │
│  ├── skills/      изолированные скиллы                  │
│  ├── memories/    память (USER.md, MEMORY.md)           │
│  └── cron/        крон-джобы тенанта                    │
├─────────────────────────────────────────────────────────┤
│  skills/          общие скиллы (69 категорий, 294 шт)   │
│  instincts/       инстинкты (19 шт, 5 mandatory)        │
│  scripts/         скрипты (181 шт)                      │
│  config.yaml      провайдеры, MCP, лимиты               │
└─────────────────────────────────────────────────────────┘
```

### Платформы

| Платформа | Канал | Статус |
|-----------|-------|:------:|
| Telegram | DM "Poliakarm" + Home (5529208670) | ✅ primary |
| WhatsApp | Connected | ✅ |
| Local | Файлы на машине | ✅ |

### MCP-серверы

| Сервер | Назначение |
|--------|-----------|
| `bybit-ws` | Трейдинг: позиции, скан, вход/выход |
| `codebase-memory` | Структурный поиск по коду (Cypher, 158 языков) |
| `repowise` | Семантический слой: health, git-история, ADR, мёртвый код |
| `lazyweb` | Быстрый веб-поиск |
| `tutu` | Общий MCP (погода, курсы валют и т.д.) |

### Провайдеры

| Провайдер | Модель | Назначение |
|-----------|--------|-----------|
| deepseek | deepseek-v5 (+Router +Isolation +Cron +Secrets)-pro | Основная модель (Mоре) |
| google | gemini-2.5-flash | Vision (изображения) |

---

## 2. Тенанты — 14 профилей

| Профиль | TG ID | Роль | Скиллов | Память | Cron | Тип |
|---------|-------|------|:-------:|:------:|:----:|-----|
| **default** | — | Море (админ) | 80 | ✅ | ✅ | admin |
| **poliakarm** | — | Поляков (DM) | 159 | — | — | admin |
| **morearbot** | @Morearbot | Pro-бот (gateway) | 84 | — | — | bot |
| **apolai** | @Apolaibot | Demo-бот | 84 | — | — | bot |
| **demo** | — | Тестовый | 83 | — | 1 | test |
| **vietnam-pro** | @Vietlivebot | Вьетнам Pro | 136 | — | — | bot |
| **vietnam-guide** | — | Вьетнам dev | 77 | — | — | dev |
| **user_5529208670** | @Cryptoram | Поляков (второй) | 130 | — | — | user |
| **user_696238708** | крипто-клиент | 130 | 2 | — | user |
| **user_1971012634** | клиент | 123 | — | — | user |
| **user_2115597720** | клиент | 130 | — | — | user |
| **user_308591502** | клиент | 130 | — | — | user |
| **user_470549555** | клиент | 130 | — | — | user |
| **user_7413748866** | клиент | 72 | — | — | user |

### Права доступа

```
admin (default, poliakarm)
  ├── все toolsets
  ├── терминал, файлы, MCP
  ├── cronjob создание/управление
  └── делегирование тенантам

bot (morearbot, apolai, vietnam-pro)
  ├── chat + /upgrade
  ├── delegate_task
  └── БЕЗ терминала, БЕЗ файлов

user (user_*)
  ├── chat + базовые tools
  └── ограничения через channel_profiles
```

---

## 3. Скиллы — 294 шт (69 категорий)

### Топ-категории (по количеству)

| Категория | Скиллов | Назначение |
|-----------|:-------:|-----------|
| **devops** | 55 | Инфраструктура, деплой, мониторинг |
| **productivity** | 42 | Email, Notion, календарь, документы |
| **meta** | 27 | Мета-скиллы: роутер, память, конституция |
| **software-development** | 23 | Кодинг, архитектура, тесты |
| **creative** | 18 | Генерация контента, медиа |
| **engineering** | 13 | Инженерные расчёты |
| **context-eng** | 12 | Контекстная инженерия |
| **mlops** | 9 | ML-операции |
| **media** | 8 | YouTube, изображения, аудио |
| **trading** | 7 | Трейдинг, стратегии |
| **autonomous-ai-agents** | 7 | Автономные агенты |
| **github** | 6 | GitHub-операции |

### Обязательные скиллы (при старте)

| Скилл | Назначение |
|-------|-----------|
| `hermes-constitution` | Правила оркестрации, приоритеты |
| `communication-protocol` | Правила общения, стиль |
| `brand-voice-polyakov` | Голосовой профиль |
| `obsidian-context` | Obsidian vault loader |
| `using-hermes-skills` | Роутер скиллов |
| `memory-preload` | Контекст прошлых сессий |

### Shared-скиллы (для тенантов)

113 скиллов в `/opt/hermes/shared-skills/` — базовая поставка для всех профилей.

---

## 4. Инстинкты — 19 шт

### По доменам

| Домен | Кол-во |
|-------|:------:|
| devops | 7 |
| trading | 2 |
| knowledge | 2 |
| productivity | 2 |
| risk | 1 |
| safety | 1 |
| infrastructure | 1 |
| optimization | 1 |
| data-integrity | 1 |
| communication | 1 |

### Mandatory (авто-загрузка для всех тенантов)

| # | Инстинкт | Суть |
|---|---------|------|
| 11 | `mandatory-judge` | Judge перед кодом/конфигом |
| 12 | `shared-knowledge-base` | Сохранять в shared skills |
| 16 | `vision-gemini-required` | Vision только через Gemini |
| 18 | `live-data-primary-source` | Живые данные только из источника |
| 19 | `telegram-no-tables` | Таблицы → моноширинный `<pre>` |

---

## 5. Скрипты — 181 шт

### Ключевые скрипты

| Скрипт | Назначение |
|--------|-----------|
| `bybit-watchdog.py` | Мониторинг bybit-ws, авто-рестарт |
| `bybit-mcp-server.py` | MCP-сервер для трейдинга |
| `bybit-metrics-exporter.py` | Prometheus-метрики |
| `stars-payment-handler.py` | @miropolbot: приём оплат Stars/TON |
| `stars-activator.py` | Активация Pro по оплате |
| `ton-activator.py` | Активация TON-платежей |
| `deprovision.py` | Авто-офбординг тенантов (30 дней) |
| `apolaibot-demo.py` | Demo-бот @Apolaibot v3.1 |
| `gridsignal-bot.py` | @Gridbolbot — сигналы Bollinger Grid |
| `hermes-tenant` | CLI: onboard/offboard тенантов |
| `skill-sync.py` | Синхронизация скиллов default → тенанты |
| `kg.py` | Knowledge Graph из Obsidian |
| `reflect.py` | Ночной цикл инсайтов |
| `obsidian_search.py` | BM25-поиск по vault |
| `artifacts.py` | Слой артефактов между лупами |
| `verify.py` | Maker-Checker верификатор |
| `goal_loop.py` | Goal-лупы с чекпоинтами |
| `doc2skill.py` | PDF/URL → авто-скилл |
| `plural-ru.py` | Склонение слов |
| `file-id-cache.py` | Кэш file_id Telegram |
| `payment-smart-cart.py` | Умная корзина APScheduler |
| `audit-trail.py` | Аудит-трейл операций |
| `billing.py` | Биллинг и расчёт стоимости |
| `hermes_quota.py` | 📊 Квоты: дневные лимиты токенов/событий/MCP |
| `hermes_alerts.py` | 🚨 Алерты: доставка аномалий админу + авто-действия |
| `hermes_tenant_lifecycle.py` | 🔄 Жизненный цикл: active→grace→frozen→deleted |
| `hermes_skill_router.py` | 🎯 Динамический роутер: intent → нужные скиллы (экономия токенов) |
| `hermes_isolation_test.py` | 🛡️ Ночные тесты: RBAC, изоляция, cron, права (30 проверок) |
| `hermes_gateway_hook.py` | 🔗 Watchdog: RBAC + метрики в реальном времени |
| `hermes_rbac_guard.py` | 🔒 RBAC-шлагбаум: проверка прав до выполнения tool |
| `hermes_tenant_metrics.py` | 📊 Метрики тенантов: токены, вызовы, аномалии |

### Shared-скрипты (для всех)

`~/.hermes/scripts/plural-ru.py` — склонения слов
`~/.hermes/scripts/file-id-cache.py` — кэш Telegram file_id

---

## 6. Боты и сервисы

| Сервис | Бот | Платформа | RAM | Назначение |
|--------|-----|-----------|:---:|-----------|
| `hermes-gateway` | @Morearbot | Telegram | 896MB | Основной gateway |
| `apolaibot-demo` | @Apolaibot | Telegram | 16MB | Demo-бот |
| `gridsignal-bot` | @Gridbolbot | Telegram | 19MB | Торговые сигналы |
| `stars-payment` | @miropolbot | Telegram | 7MB | Приём оплат |
| `vpn-seller-bot` | @poliakarbot | Telegram | 14MB | Продажа VPN |
| `vietnam-guide` | @Vietlivebot | Telegram | 14MB | Гид по Вьетнаму |
| `vietnam-api` | — | REST :8090 | 0.4MB | API гида |
| `vietnam-food` | — | Web :8091 | 2MB | Food Web App |
| `bybit-ws-async` | — | RPC :8766 | 88MB | Трейдинг-движок |
| `vpn-core-xray` | — | VLESS :4443 | — | VPN-сервер |
| `vpn-core-hysteria` | — | Hysteria2 :8445 | — | VPN-сервер |

---

## 7. Проекты

| Проект | Путь | Репозиторий | AGENTS.md |
|--------|------|-------------|:---------:|
| **bybit-ws** | `~/bybit-ws/` | github/poliakarmai | ✅ |
| **GSC** | `~/gsc/` | github/poliakarmai | ✅ |
| **vpn-infra** | `~/vpn-infra/` | github/poliakarmai | ✅ |
| **pci-index** | `~/pci-index/` | github/poliakarmai | ✅ |
| **gridsignal-bot** | `~/.local/bin/` | github/poliakarmai | ✅ |
| **gsc-vscode** | `~/gsc-vscode/` | github/poliakarmai | ✅ (06.08) |
| **hermes-infra** | `~/hermes-infra/` | github/poliakarmai | ✅ (06.08) |
| **hermes-orchestration** | `~/hermes-orchestration/` | github/poliakarmai | ✅ |
| **hermes-agent-orch.** | `~/projects/` | github/poliakarmai | ✅ |
| **vietnam-guide-bot** | `~/vietnam-guide-bot/` | — | — |
| **gazprom-work** | `~/gazprom-work/` | — | — |
| **obsidian-vault** | `~/obsidian-vault/` | github/poliakarmai | ✅ (06.08) |
| **poliakarmai.github.io** | `~/poliakarmai.github.io/` | github/poliakarmai | ✅ (06.08) |
| **freellmapi** | `~/freellmapi/` | — | — |

---

## 8. Ключевые пути

| Что | Где |
|-----|-----|
| Конфиг Hermes | `~/.hermes/config.yaml` |
| Скиллы (свои) | `~/.hermes/skills/` |
| Инстинкты | `~/.hermes/instincts/instincts.jsonl` |
| Конституция | `~/.hermes/HERMES_CONSTITUTION.md` |
| Obsidian vault | `~/obsidian-vault/` |
| Логи bybit-ws | `~/.local/share/bybit-ws/events.log` |
| БД bybit-ws | `~/.local/share/bybit-ws/state.db` |
| Бэкапы vault | `~/.hermes/backups/daily/` |
| Крон-логи | `~/.hermes/cron/output/` |
| Кэш изображений | `~/.hermes/cache/images/` |
| Shared skills | `/opt/hermes/shared-skills/` |

---

## 9. Инварианты (не нарушать)

1. **Изоляция тенантов.** Профили не видят чужих skills/memories/cron.
2. **Конституция первая.** `hermes-constitution` загружается в начале каждой сессии.
3. **Живые данные > кэш.** Позиции/PnL/статус — из RPC/SQLite/systemctl, не из памяти.
4. **3 провала → стоп.** Спросить или сменить подход.
5. **Scope discipline.** Только запрошенное, без бонусных рефакторингов.
6. **Mandatory instinct №18.** 401 ≠ "позиций нет". 401 = "нужен токен".
7. **Telegram ≠ markdown.** Таблицы → моноширинный `<pre>`, не raw pipe-строки.
8. **Один gateway.** Не плодить отдельных гейтвеев для ботов.
9. **AGENTS.md в каждом проекте.** Новый проект → AGENTS.md в корне.
10. **RBAC прежде тула.** Hard-проверка прав на уровне кода. Bot не может terminal, user не может cronjob.
11. **Метрики по тенантам.** Токены, tool calls, MCP, denied — всё в SQLite. Аномалии → алерт.

---

## 10. RBAC — изоляция инструментов

**Политика:** `~/.hermes/rbac_policy.json` (авто-сгенерирована при первом запуске)

Принцип: deny имеет приоритет, нет allow → default deny.

| Роль | Разрешено | Запрещено |
|------|-----------|-----------|
| **admin** | `*` (всё) | — |
| **bot** | chat, answer, pay, upgrade, delegate_task | execute_command, terminal, write_file, read_file, cronjob, mcp:\*, file:\* |
| **user** | chat, answer, web_search | execute_command, terminal, write_file, read_file, cronjob, delegate_task, mcp:\*, file:\* |
| **test** | chat, answer, basic_tools | execute_command, write_file, cronjob, mcp:\* |
| **dev** | chat, basic_tools, code_search, mcp:codebase-memory, mcp:repowise | execute_command, write_file, cronjob, mcp:bybit-ws |

**Проверка:**
```bash
python3 ~/.hermes/scripts/hermes_rbac_guard.py check --tenant user_5529208670 --tool execute_command
# → exit 3 (denied)
```

**Файлы:**
- `~/.hermes/scripts/hermes_rbac_guard.py` (249 строк) — RBAC-шлагбаум
- `~/.hermes/rbac_policy.json` — политика
- `~/.local/share/hermes/rbac_audit.jsonl` — аудит-лог

---

## 11. Tenant Observability — метрики

**Хранилище:** SQLite `~/.local/share/hermes/tenant_usage.db` (WAL-режим)

**Что измеряется:**
- Токены (in/out/total) на тенанта
- Tool calls (allowed + denied)
- MCP calls
- Latency (средняя)
- Ошибки

**CLI:**
```bash
# Запись события
python3 ~/.hermes/scripts/hermes_tenant_metrics.py record --tenant user_X --event llm --tokens-in 1200 --tokens-out 350

# Дневной отчёт
python3 ~/.hermes/scripts/hermes_tenant_metrics.py report

# Поиск аномалий (токены > 200K, events > 800, denied > 5, MCP > 200)
python3 ~/.hermes/scripts/hermes_tenant_metrics.py anomalies --json
```

**Пороги аномалий (по умолчанию):**
- Токены: 200,000/день
- События: 800/день
- Denied: 5/день
- MCP-вызовы: 200/день

**Файлы:**
- `~/.hermes/scripts/hermes_tenant_metrics.py` (248 строк)
- `~/.hermes/scripts/hermes_gateway_hook.py` — watchdog (systemd)

---

## 12. Quota — дневные лимиты

**Политика:** `~/.hermes/quota_policy.json` (авто-сгенерирована)

| Роль | Токены/день | События/день | MCP/день | Denied | При превышении |
|------|:-----------:|:------------:|:--------:|:------:|:-------------:|
| admin | ∞ | ∞ | ∞ | alert>10 | alert |
| bot | 300K | 1000 | 200 | 5 | freeze |
| user | 100K | 300 | 0 | 3 | throttle |
| test | 50K | 100 | 10 | 3 | throttle |
| dev | 200K | 500 | 100 | 5 | throttle |

**Проверка:**
```bash
python3 ~/.hermes/scripts/hermes_quota.py check --tenant user_X --role user --cost-tokens 1200
# exit: 0=ok, 1=warning, 2=throttle, 3=freeze
```

---

## 13. Alerts — доставка админу

**Файл:** `~/.hermes/scripts/hermes_alerts.py`

Собирает аномалии из метрик + квот, форматирует в Telegram-сообщение.

```bash
python3 ~/.hermes/scripts/hermes_alerts.py check           # отчёт
python3 ~/.hermes/scripts/hermes_alerts.py check --auto    # + авто-действия
```

**Авто-действия при --auto:**
- denied burst → throttle
- token spike > 500K → freeze
- mcp flood → warning

Рекомендуемый cron: `0 * * * *` (каждый час)

---

## 15. Tenant Lifecycle — жизненный цикл

**Файл:** `~/.hermes/scripts/hermes_tenant_lifecycle.py`

Связывает `billing.py` + `deprovision.py` + `rbac_policy.json` в автомат:

```
active ──оплата просрочена──▶ grace (3 дня) ──▶ frozen (7 дней) ──▶ deleted (30 дней)
  ✅ всё работает            ⚠️ без MCP/cron      🧊 chat+pay         ❌ deprovision
```

**Проверка:**
```bash
python3 ~/.hermes/scripts/hermes_tenant_lifecycle.py check
python3 ~/.hermes/scripts/hermes_tenant_lifecycle.py apply    # применить переходы
```

**Автоматические действия при transition:**
- grace → RBAC: user-права, убраны MCP/cron/файлы
- frozen → RBAC: chat+pay only
- deleted → вызов deprovision.py

Рекомендуемый cron: `0 2 * * *` (раз в сутки)

---

## 14. Skill Router — динамическая подгрузка

**Файл:** `~/.hermes/scripts/hermes_skill_router.py`

Вместо загрузки 130+ скиллов в контекст — подбирает 3-5 релевантных по intent.

| Компонент | Значение |
|-----------|---------|
| Проиндексировано | 327 скиллов, 15 категорий |
| Обязательные | 6 (всегда) |
| Дополнительные | до 5 по запросу |
| Экономия токенов | ~3-5K на сессию |

**Пример:** запрос «позиции bybit» → trading-data-sources, bybit-ws-maintenance.
Запрос «привет» → только mandatory (без тяжёлых скиллов).

```bash
python3 ~/.hermes/scripts/hermes_skill_router.py index   # построить индекс
python3 ~/.hermes/scripts/hermes_skill_router.py route "запрос"
```

---

## 18. Isolation Tests + Cron + Secrets

**Файл:** `~/.hermes/scripts/hermes_isolation_test.py`

Ночная проверка (30 тестов): RBAC deny/allow, изоляция профилей, cron-лимиты, права файлов.

```bash
python3 ~/.hermes/scripts/hermes_isolation_test.py
# exit 0 = всё чисто, exit 1 = нарушения
```

**Cron-лимиты:** admin=∞, bot=0, user=0, test=1, dev=3.
**Права:** config.yaml, .env, rbac_policy.json → 600.

Рекомендуемый cron: `0 3 * * *` (раз в сутки)

---

## 16. Онбординг нового тенанта

```bash
# Полный онбординг (user + профиль + скиллы + права)
python3 ~/.hermes/scripts/hermes-tenant-full onboard <tg_id> <имя> <тариф>

# Синхронизация скиллов
python3 ~/.hermes/scripts/skill-sync.py

# Проверка
ls ~/.hermes/profiles/<имя>/
```

---

## 17. Конвенции

- **Язык:** русский. Код/команды/API — английский.
- **Стиль:** дружелюбный, краткий, с иронией. Как с коллегой за кофе.
- **Пруф или не было.** `exit_code=0` или не считается.
- **Obsidian vault — persistence.** Факты сохранять через `write_file`/`patch`.
- **После сложных задач → скилл.** 5+ tool calls = кандидат.
- **Формат коммитов:** русский, `feat(scope): описание` / `fix(scope): описание` / `docs: описание`.

---

*Обновлено: 06.08.2026. При изменениях — обновлять этот файл.*
