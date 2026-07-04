---
tags: [hermes, agents, architecture, checkpointing]
source: MiMo Code crash (2h work lost)
created: 2026-07-01
---

# Checkpointing для AI-агентов

## Проблема

Агент @mimopolbot (MiMo Code) работал 2 часа → упал → начал сначала.
Потеря всего прогресса — неприемлемо для долгих задач.

## Решение: checkpointing

▸ Каждые N шагов — snapshot состояния
▸ Crash → resume с последнего checkpoint
▸ Compaction: 10 checkpoint → 1 сжатый

В Claude Code это `/compact`.

## Минимальный checkpoint

```
.session/
├── checkpoint_0001.json    # conversation history + tool state + file mutations
├── checkpoint_0002.json
├── compact_0001.json       # сжатый: объединяет 10 чекпоинтов
└── checkpoint.lock         # блокировка записи
```

Формат — JSON. Сериализуется вся сессия:
- **conversation history** — все сообщения user/assistant/tool
- **tool state** — какие тулы были вызваны, результаты
- **file mutations** — что создано/изменено

## Когда применять

- Любой агент, работающий дольше 5 минут
- Мультишаговые задачи (веб-поиск, код, установка зависимостей)
- Задачи с внешними эффектами (запись файлов, API-вызовы)

## Примечание

Для следующей замены @mimopolbot — checkpointing в базовую архитектуру.
