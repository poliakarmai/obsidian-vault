---
title: Evidence & Feedback Layer — архитектурное решение
created: 2026-06-23
source: Skill Harnessing (arXiv, 2026)
tags: [architecture, evidence, feedback, audit, hermes]
---

# Evidence & Feedback Layer

## Контекст

Согласно эталонной архитектуре Skill Harnessing, четвёртый слой — Evidence & Feedback — обеспечивает: улики для аудита, воспроизводимость действий, обратную связь для улучшения системы.

У нас эти функции размазаны по 5+ механизмам без единой концепции. Формализуем.

## Текущее состояние (as-is)

| Механизм | Что фиксирует | Где хранит |
|----------|--------------|-----------|
| `audit-trail` | Файловые операции (write_file, patch) | `~/.hermes/data/audit_trail.db` |
| `tenant-audit` | Действия тенантов (сообщения, команды) | `~/.hermes/data/tenant_audit.db` |
| `session_search` | История диалогов | `~/.hermes/sessions.db` |
| `trade_history` | Торговые сделки (LONG/SHORT) | `~/.local/share/bybit-ws/state.db` |
| `vault-vs-reality` | Расхождения vault / реальность | cron-отчёт в Telegram |
| `invariant-check` | Состояние при старте | stdout / exit code |

**Проблемы:**
- Разные БД, разные форматы, нет единого query-интерфейса
- Нет связи между событиями (какой диалог привёл к какой файловой операции?)
- Feedback не замкнут — ошибки фиксируются, но не возвращаются в улучшение скиллов

## Целевое состояние (to-be)

### Принципы

1. **Каждое действие агента оставляет улику.** Файловая операция, вызов API, ответ пользователю — всё с timestamp + session_id + agent_id.
2. **Улики связаны.** Файловая операция знает message_id. Трейд знает какой skill его инициировал.
3. **Feedback замкнут.** Ошибки → skill-evolution. Успешные паттерны → base skills.
4. **Аудит читаем.** Единый формат, единый query-интерфейс.

### Компоненты

```
Evidence & Feedback Layer
├── Evidence Collectors (пишут улики)
│   ├── audit-trail.py      ← файловые операции (уже есть)
│   ├── tenant-audit.py     ← действия тенантов (уже есть)
│   ├── trade_history       ← сделки (уже есть)
│   └── agent-telemetry     ← метрики агента (уже есть)
│
├── Evidence Store (единое хранилище)
│   └── evidence.db         ← SQLite, unified schema
│       ├── events (timestamp, session_id, agent, type, detail)
│       ├── file_ops (event_id FK→events)
│       ├── api_calls (event_id FK→events)
│       └── decisions (event_id FK→events)
│
├── Feedback Loop (обратная связь)
│   ├── invariant-check     ← pre-session validation
│   ├── vault-vs-reality    ← daily drift detection
│   ├── skill-evolution     ← DSPy → улучшение скиллов
│   └── error→fix pipeline  ← ошибки → исправления
│
└── Query Interface
    ├── evidence-query CLI  ← единый поиск по всем уликам
    └── audit-report cron   ← еженедельный отчёт
```

### Связи между событиями

```
User message (session_search)
  └→ Agent response
       └→ File write (audit-trail: message_id=X)
            └→ Skill updated (skill-sync)
                 └→ Trade decision (trade_history: triggered_by_skill=Y)
```

## План внедрения

### Фаза 1: Evidence Store (MVP)
- Создать `evidence.db` с unified schema
- Миграция: audit-trail + tenant-audit → evidence.db
- `evidence-query` CLI: поиск по session_id, агенту, типу, диапазону дат

### Фаза 2: Связи
- Добавить `session_id` и `message_id` во все события
- Связать file_ops ↔ trade_history ↔ session_search

### Фаза 3: Feedback Loop
- Авто-анализ ошибок → предложения по улучшению скиллов
- Интеграция с skill-evolution (DSPy)

## Метрики

- Покрытие: % действий агента с уликой (цель: 100%)
- Связность: % событий с session_id (цель: 90%)
- Время до ответа на инцидент: от алерта до фикса (цель: <1ч)
