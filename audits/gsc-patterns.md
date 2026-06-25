# GSC Active Patterns
Generated: 2026-06-25 06:20
Total: 23 patterns

| Project | Cat | Ech | Pattern | Type | TP/FP |
|---------|-----|-----|---------|------|-------|
| * | HIGH | 1 | Обфускация токенов в f-строках | semantic | 1/0 (100%) |
| * | HIGH | 2 | Хардкод IP адреса | regex | 1/0 (100%) |
| * | MEDIUM | 3 | Синхронный код в async | semantic | 1/0 (100%) |
| apolaibot | LOW | 1 | Код в репо отстаёт | semantic | 1/0 (100%) |
| apolaibot | MEDIUM | 2 | Нет HTTPS pinning | config | 1/0 (100%) |
| apolaibot | HIGH | 2 | Prompt injection открыт | semantic | 1/0 (100%) |
| apolaibot | CRITICAL | 2 | API-ключ в config.yaml | grep | 1/0 (100%) |
| apolaibot | MEDIUM | 3 | In-memory state | structural | 1/0 (100%) |
| bybit-ws | HIGH | 1 | env vars разбросаны по коду | regex | 1/0 (100%) |
| bybit-ws | HIGH | 2 | API-ключи в коде | regex | 1/0 (100%) |
| bybit-ws | MEDIUM | 3 | ML Gate молчаливый пропуск | semantic | 1/0 (100%) |
| bybit-ws | CRITICAL | 3 | SQLite без WAL | grep | 1/0 (100%) |
| gridsignal | MEDIUM | 1 | Хардкод admin ID | regex | 1/0 (100%) |
| gridsignal | LOW | 1 | Dead code / unused variables | regex | 1/0 (100%) |
| gridsignal | HIGH | 2 | Токен в /proc/PID/environ | semantic | 1/0 (100%) |
| gridsignal | MEDIUM | 3 | Интервалы бот↔RPC не совпадают | semantic | 1/0 (100%) |
| gridsignal | HIGH | 3 | Скоры выходят за заявленный диапазон | semantic | 1/0 (100%) |
| vpn-bot | MEDIUM | 1 | __import__ вместо import | grep | 1/0 (100%) |
| vpn-bot | LOW | 1 | bare except: pass | grep | 1/0 (100%) |
| vpn-bot | MEDIUM | 2 | .env права не 600 | grep | 1/0 (100%) |
| vpn-bot | HIGH | 2 | EnvironmentFile утечка | config | 1/0 (100%) |
| vpn-bot | CRITICAL | 2 | Полный sudo | grep | 1/0 (100%) |
| vpn-bot | HIGH | 3 | TOCTOU race condition | semantic | 1/0 (100%) |

---
## Pattern Details

### [HIGH] Обфускация токенов в f-строках
- **Проект:** *
- **Эшелон:** 1
- **Тип:** `semantic`
- **Паттерн:** `TELEGRAM_.*BOT_TOKEN|os\.environ.*\+.*TOKEN`
- **Описание:** Не использовать конкатенацию для обхода маскировки — читать напрямую

### [HIGH] Хардкод IP адреса
- **Проект:** *
- **Эшелон:** 2
- **Тип:** `regex`
- **Паттерн:** `(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)`
- **Описание:** IP адреса кроме 127.x.x.x должны быть в env vars

### [MEDIUM] Синхронный код в async
- **Проект:** *
- **Эшелон:** 3
- **Тип:** `semantic`
- **Паттерн:** `subprocess\.run|requests\.(get|post).*async def`
- **Описание:** Блокирующие вызовы в async-функциях → asyncio.to_thread()

### [LOW] Код в репо отстаёт
- **Проект:** apolaibot
- **Эшелон:** 1
- **Тип:** `semantic`
- **Паттерн:** `repo vs deployed`
- **Описание:** Регулярная синхронизация репо ← прод

### [MEDIUM] Нет HTTPS pinning
- **Проект:** apolaibot
- **Эшелон:** 2
- **Тип:** `config`
- **Паттерн:** `aiohttp\.ClientSession\(\)`
- **Описание:** Явный SSL-контекст с check_hostname=True

### [HIGH] Prompt injection открыт
- **Проект:** apolaibot
- **Эшелон:** 2
- **Тип:** `semantic`
- **Паттерн:** `user_msg.*api.*completion`
- **Описание:** Пользовательский ввод в LLM должен проходить санитизацию

### [CRITICAL] API-ключ в config.yaml
- **Проект:** apolaibot
- **Эшелон:** 2
- **Тип:** `grep`
- **Паттерн:** `api_key:\s*[A-Za-z0-9_\-\.]{8,}`
- **Описание:** Ключи в config.yaml → ${ENV_VAR} из .env

### [MEDIUM] In-memory state
- **Проект:** apolaibot
- **Эшелон:** 3
- **Тип:** `structural`
- **Паттерн:** `conversations\s*=\s*\{\}|history\s*=\s*\{\}`
- **Описание:** Всё что теряется при рестарте — на диск (JSON/SQLite)

### [HIGH] env vars разбросаны по коду
- **Проект:** bybit-ws
- **Эшелон:** 1
- **Тип:** `regex`
- **Паттерн:** `os\.environ\.get\(['\"]BYBIT_`
- **Описание:** Feature flags должны быть в едином модуле feature_flags.py

### [HIGH] API-ключи в коде
- **Проект:** bybit-ws
- **Эшелон:** 2
- **Тип:** `regex`
- **Паттерн:** `(api_key|secret|token)\s*=\s*['\"][A-Za-z0-9_\-]{8,}['\"]`
- **Описание:** Никаких хардкодов API-ключей — только os.environ.get()

### [MEDIUM] ML Gate молчаливый пропуск
- **Проект:** bybit-ws
- **Эшелон:** 3
- **Тип:** `semantic`
- **Паттерн:** `AND voting without logging`
- **Описание:** Комбинированные гейты должны логировать причину блокировки каждого

### [CRITICAL] SQLite без WAL
- **Проект:** bybit-ws
- **Эшелон:** 3
- **Тип:** `grep`
- **Паттерн:** `sqlite3\.connect\([^)]*\)(?!.*check_same_thread)`
- **Описание:** Все sqlite3.connect() должны иметь check_same_thread=False и PRAGMA journal_mode=WAL

### [MEDIUM] Хардкод admin ID
- **Проект:** gridsignal
- **Эшелон:** 1
- **Тип:** `regex`
- **Паттерн:** `== \d{6,12}\b|admin.*id.*\d{6,12}`
- **Описание:** Admin ID и chat ID должны быть в env vars

### [LOW] Dead code / unused variables
- **Проект:** gridsignal
- **Эшелон:** 1
- **Тип:** `regex`
- **Паттерн:** `^[A-Z_]+ = .+\n(?!.*\1)`
- **Описание:** Неиспользуемые переменные и константы

### [HIGH] Токен в /proc/PID/environ
- **Проект:** gridsignal
- **Эшелон:** 2
- **Тип:** `semantic`
- **Паттерн:** `CRYPTOBOT_TOKEN|TELEGRAM_BOT_TOKEN.*os.environ`
- **Описание:** Токены должны удаляться из environ после чтения: os.environ.pop()

### [MEDIUM] Интервалы бот↔RPC не совпадают
- **Проект:** gridsignal
- **Эшелон:** 3
- **Тип:** `semantic`
- **Паттерн:** `interval.*enum.*mismatch`
- **Описание:** Enum'ы интервалов между клиентом и сервером должны совпадать

### [HIGH] Скоры выходят за заявленный диапазон
- **Проект:** gridsignal
- **Эшелон:** 3
- **Тип:** `semantic`
- **Паттерн:** `score.*range.*display`
- **Описание:** Фактические границы вычислений должны совпадать с UI

### [MEDIUM] __import__ вместо import
- **Проект:** vpn-bot
- **Эшелон:** 1
- **Тип:** `grep`
- **Паттерн:** `__import__\([^)]+\)`
- **Описание:** Никаких __import__() — нормальный import наверху файла

### [LOW] bare except: pass
- **Проект:** vpn-bot
- **Эшелон:** 1
- **Тип:** `grep`
- **Паттерн:** `except Exception:\s*\n\s*pass`
- **Описание:** Bare except должен хотя бы log.debug()

### [MEDIUM] .env права не 600
- **Проект:** vpn-bot
- **Эшелон:** 2
- **Тип:** `grep`
- **Паттерн:** `ls -la .*.env`
- **Описание:** .env должен быть chmod 600

### [HIGH] EnvironmentFile утечка
- **Проект:** vpn-bot
- **Эшелон:** 2
- **Тип:** `config`
- **Паттерн:** `EnvironmentFile=.*\.env`
- **Описание:** Токены не должны быть в /proc/PID/environ — прямой парсинг .env в коде

### [CRITICAL] Полный sudo
- **Проект:** vpn-bot
- **Эшелон:** 2
- **Тип:** `grep`
- **Паттерн:** `ALL=\(ALL\)\s+NOPASSWD:\s*ALL`
- **Описание:** Никакого NOPASSWD:ALL — только ограниченные права в sudoers.d/

### [HIGH] TOCTOU race condition
- **Проект:** vpn-bot
- **Эшелон:** 3
- **Тип:** `semantic`
- **Паттерн:** `(can_redeem|can_use|check_)\w+.*\n.*redeem|use_`
- **Описание:** Check-then-act паттерн — использовать атомарные операции (INSERT OR IGNORE, UPDATE WHERE)
