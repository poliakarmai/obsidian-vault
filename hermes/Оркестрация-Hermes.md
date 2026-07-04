# Оркестрация Hermes — полная картина

> 04.07.2026 · 5/5 фаз + KG/Reflect · 18 скриптов · продакшен-ready

---

## 🧠 Кто я

**Море** — главный оркестратор multi-tenant Hermes. Профиль `default`.

**Что я делаю:**
- Управляю трейдингом Bybit (bybit-ws)
- Оркестрирую тенантов (Morearbot, Apolai, Ilya + 7 юзеров)
- Слежу за VPN-инфраструктурой
- Веду документооборот Газпрома
- Развиваю платформу (скиллы, cron, автоматизации, биллинг, безопасность, продукт)

**Приоритеты:** Трейдинг → Газпром → VPN → Multi-tenant → Продукт

---

## 🏗️ Архитектура тенантов

```
МОРЕ (default) — полный доступ
 │
 ├── @Morearbot (Hermes Gateway, 200MB)
 │   └── Pro-клиенты: полный Hermes после оплаты Stars
 │
 ├── @Apolaibot (скрипт, 62MB)
 │   └── Demo: каталог / онбординг / 2FA / фидбек / summarize / export / temp / tools
 │
 ├── @miropolbot (скрипт, 10MB)
 │   └── Приём Telegram Stars + активация
 │
 ├── Ilya (profile user_470549555) — песочница terminal+file
 ├── user_5529208670 — Cryptos
 ├── user_1148002325, user_2115597720, user_308591502
 └── poliakarm, apolai, demo
```

| Бот | Тип | RAM | Назначение | Команд |
|---|---|---|---|---|
| **Море** | Hermes Gateway | 200MB | Оркестратор | все |
| @Morearbot | Hermes Gateway | 200MB | Pro-тенанты | базовые |
| @Apolaibot | python-telegram-bot | 62MB | Demo + лидогенерация | 10 |
| @miropolbot | Polling-скрипт | 10MB | Оплата Stars | 3 |

---

## 🔐 Безопасность — 5 слоёв (Фаза 1 ✅)

| Слой | Инструмент | Что делает |
|---|---|---|
| **Терминал** | `safety-guard` | rm -rf, git push --force, chmod 777 |
| **Статика** | `skill-security-scan` | IP, токены, секреты в скиллах |
| **Код** | `security-and-hardening` | OWASP Top 10, pip-audit, HIBP |
| **Рантайм** | `skill_sandbox.py` | Podman: без сети, readonly FS, лимиты |
| **Аудит** | `agent_fs.py` | Версионирование, локинг, rollback, audit trail |
| **2FA** | TOTP (pyotp) | Google Authenticator для админов |
| **Prompt** | `input-guardrails` + `tool-output-guard` | Двойная защита от инъекций |

---

## 💰 Биллинг — 4 тарифа (Фаза 2 ✅)

| Тариф | Цена | Токены/мес | Команда | Фичи |
|-------|------|-----------|---------|-------|
| **Start** | 0₽ | 1M | 1 | чат + скиллы |
| **Basic** | 690₽ | 5M | 1 | + поиск + документы |
| **Pro** | 1990₽ | 20M | 5 | + экспорт + инкогнито |
| **Expert** | 5990₽ | 100M | 50 | + трейдинг + on-prem |

Инструменты: `billing.py` (SQLite), `tenant_features.py` (фидбек, бюджет, каталог)

---

## 🟢 Продукт (Фаза 3 ✅)

| Фича | Инструмент |
|------|-----------|
| Каталог скиллов | `/skills` — 7 профессий × 5 скиллов |
| Онбординг | Кнопки выбора роли в `/start` |
| Пользовательские скиллы | `user_skills.py` — создание/запуск в песочнице |
| Командный vault | `team_vault.py` — BM25-поиск, цитирование |
| Генерация документов | `doc_export.py` — MD→PDF/DOCX/XLSX |

---

## 🔵 Платформа (Фаза 4 ✅)

| Фича | Инструмент |
|------|-----------|
| Облачное зеркало | `cloud_mirror.py` — watchdog, bidirectional sync |
| Очередь агентов | `agent_queue.py` — FIFO, статус, ETA, авто-активация |
| Прозрачность тулов | `/tools` — последние 5 операций из audit trail |
| Реконнект стрима | архитектурно заложен |

---

## ⚪ Масштаб (Фаза 5 ✅)

| Фича | Инструмент |
|------|-----------|
| Health Dashboard | `health_dashboard.py` — 7 сервисов, JSON API |
| Whitelabel | `whitelabel.py` — брендинг для тенантов |

---

## 📊 Скиллы по tiers

| Tier | Кол-во | Кому |
|---|---|---|
| **base** | 55 | Всем тенантам |
| **admin_only** | 53 | Только Море |
| **opt_in** | 25 | По запросу |
| **Новые (04.07)** | 1 | knowledge-graph-reflect |
| **Всего** | ~184 | — |

---

## 🧠 Knowledge Graph + Reflect (04.07.2026)

Две фичи памяти для всех тенантов:

### Knowledge Graph (`kg.py`)
- Граф `[[wikilinks]]` из Obsidian vault → SQLite
- Basename-резолвинг: `[[trading]]` → `hermes/trading.md`
- Инкрементальный (по mtime), `--full` для перестройки
- Запросы: `query`, `backlinks`, `path`, `orphans`, `search`, `stats`
- У каждого тенанта своя БД (`~/.hermes/kg-<tenant>.db`)

### Reflect (`reflect.py`)
- Автономный ночной цикл: KG → свежие заметки → DeepSeek → инсайты
- Сохраняет в `hermes/insights/YYYY-MM-DD.md`
- Категории: паттерны, противоречия, пробелы, действия
- Верификация сохранения (≥200 байт)

### Multi-tenant оркестратор (`reflect-all.py`)
- Один скрипт для всех: админ + 9 тенантов
- Крон `aebfa1645602`, ежедневно 03:00, `no_agent=true`

| Тенант | .md | KG |
|--------|-----|-----|
| admin | 252 | `~/.hermes/kg.db` |
| dv | 40 | `~/.hermes/kg-dv.db` |
| kolesnikov | 15 | `~/.hermes/kg-kolesnikov.db` |
| cryptos, drone_dev, illarionov, ilya | 3 | `~/.hermes/kg-*.db` |
| nikita | 2 | `~/.hermes/kg-nikita.db` |
| d_fffa, marina | 1 | `~/.hermes/kg-*.db` |

---

## ⏱️ Ключевые cron-джобы

### Трейдинг
| Джоб | Когда |
|---|---|
| 📊 Авто-вход по сканам | Каждые 4ч |
| 🔗 Корреляционные алерты | Каждые 2ч |
| 📈 M5/M3 авто-сканер | Каждые 4ч |
| 🌅 Утренний LONG-скан | 05:00 |
| 💹 Dashboard pin | Каждый час |
| 📋 PnL-сводка | 09:00 |
| 🏦 Weekly PnL | Пн 09:00 |

### Инфраструктура
| Джоб | Когда |
|---|---|
| 🔍 VPN watchdog | Каждые 5м |
| 📡 Telegram watchdog | Каждые 5м |
| 🩺 Tenant health | 09:00 |
| 🛡️ Gateway patch watchdog | Каждые 10м |
| 💾 Дисковый мониторинг | 08:00 |
| 🔄 Pipeline trace | Каждые 6ч |
| 🔁 Skill sync | Каждые 3 дня |

### Безопасность
| Джоб | Когда |
|---|---|
| 🔐 HIBP check | 09:00 |
| 🛡️ Skill security scan | Вс 08:00 |
| 📦 Pip audit | Вс 08:00 |

### Бизнес
| Джоб | Когда |
|---|---|
| 💰 DeepSeek баланс | Каждые 2ч |
| ⭐ Stars активатор | Каждые 5м |
| 💎 TON активатор | Каждые 2м |
| 📊 Cost tracking | Каждые 3ч |

### Память (новое 04.07)
| Джоб | Когда |
|---|---|
| 🌙 Reflect All | 03:00 |

### Газпром
| Джоб | Когда |
|---|---|
| 📄 Авто-конвейер PDF | Каждые 15м |
| 📋 Structured extraction | Каждые 10м |
| 🏭 Вахта: дедлайны | 06:00 |

---

## 🛠️ Все инструменты

| Фаза | Инструмент | Назначение |
|------|-----------|-----------|
| 🔴 1 | `agent_fs.py` | Агентская ФС: версионирование + локинг + rollback |
| 🔴 1 | `skill_sandbox.py` | Podman-песочница для пользовательского кода |
| 🔴 1 | 2FA | TOTP Google Authenticator в @Apolaibot |
| 🟡 2 | `billing.py` | 4 тарифа, организации, промокоды |
| 🟡 2 | `tenant_features.py` | Каталог, фидбек, бюджет для тенантов |
| 🟢 3 | `user_skills.py` | Пользовательские скиллы |
| 🟢 3 | `team_vault.py` | Командный vault + BM25 |
| 🟢 3 | `doc_export.py` | MD→PDF/DOCX/XLSX |
| 🔵 4 | `agent_queue.py` | Очередь агентов FIFO |
| 🔵 4 | `cloud_mirror.py` | Облачное зеркало папки |
| 🔵 4 | `/tools` | Прозрачность тулов |
| ⚪ 5 | `health_dashboard.py` | Мониторинг сервисов |
| ⚪ 5 | `whitelabel.py` | Брендинг тенантов |
| 🧠 6 | `kg.py` | Knowledge Graph [[wikilinks]] → SQLite |
| 🧠 6 | `reflect.py` | Ночной цикл осмысления vault |
| 🧠 6 | `reflect-all.py` | Multi-tenant оркестратор Reflect |

---

## 📦 Проекты

| Проект | Статус |
|---|---|
| bybit-ws (трейдинг) | 🟢 12 позиций |
| VPN-инфра | 🟢 6 клиентов |
| @Apolaibot (демо) | 🟢 6 пользователей, 10 команд |
| Биллинг | 🟢 1 Pro, 1 организация, 2 промокода |
| Gazprom-документы | 🟢 inbox мониторится |
| Дорожная карта | 🟢 5/5 фаз |

---

## 🔗 Ссылки

- [[roadmap-apolaibot]] — дорожная карта
- [[competitors/iskra]] — анализ конкурента (18 фич)
- [[trading]] — трейдинг и bybit-ws
- [[memory]] — техническая память
- [[user-profile]] — профиль пользователя
- [[hermes/insights/2026-07-04]] — последние инсайты Reflect
