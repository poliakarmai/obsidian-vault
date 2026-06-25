---
tags: [hermes, architecture, memory, agent-design]
created: 2026-06-23
status: verified
---

# Архитектура памяти Hermes Agent

> Готовый шаблон для тиражирования на других агентов.

---

## 4 слоя памяти

```
ЗАПУСК СЕССИИ
│
├─ СЛОЙ 1: System Prompt (авто-инжект)
│   ├── Persona (кто я, роль, стиль)
│   ├── MEMORY block ← 2200 chars, из memory tool
│   ├── USER PROFILE block ← 1375 chars
│   ├── Список доступных скиллов (названия + описания)
│   └── Список инструментов (tools)
│
├─ СЛОЙ 2: 6 baseline skills (skill_view)
│   ├── hermes-constitution    — конституция оркестрации
│   ├── communication-protocol — правила общения
│   ├── brand-voice-polyakov   — голосовой профиль
│   ├── obsidian-context       — Obsidian vault loader
│   ├── using-hermes-skills    — роутер скиллов
│   └── memory-preload         — загрузка контекста
│
├─ СЛОЙ 3: memory-preload (восстановление контекста)
│   ├── Определить роль: admin или tenant ($HOME)
│   ├── Загрузить файлы из Obsidian:
│   │   ├── user-profile.md (профиль пользователя)
│   │   ├── memory.md (техническая память)
│   │   └── trading.md (трейдинг-контекст)
│   ├── ВЕРИФИКАЦИЯ свежести:
│   │   ├── git log vs vault → vault устарел?
│   │   └── systemctl status vs vault → сервис живой?
│   └── session_search(limit=3) → последние 3 сессии
│
└─ СЛОЙ 4: Obsidian vault (внешняя безлимитная память)
    ├── BM25/WRL поиск: ~/.hermes/scripts/obsidian_search.py
    ├── Meilisearch: multi-tenant фильтрация по path
    └── Заметки: 00-Index → user-profile → memory → trading → ...
```

## Инструменты памяти

| Инструмент | Назначение | Лимит |
|-----------|-----------|-------|
| `memory()` | Встроенная память (инжект в промпт) | 2,200 chars |
| `skill_view()` | Процедурная память (скиллы) | безлимитно |
| `session_search()` | Поиск прошлых сессий (SQLite FTS5) | все сессии |
| `write_file()` / `patch()` | Запись в Obsidian vault | безлимитно |
| `obsidian_search.py` | Семантический BM25/WRL поиск | безлимитно |

## Принцип эскалации

```
memory() → критические факты (пути, ключи, конфиги)
    ↓ переполнение (95%)
session_search() → «что делали вчера»
    ↓ для долгосрочного
Obsidian vault → безлимитное хранение
    ↓ поиск
BM25/WRL → семантический поиск без LLM
```

## Процедура при переполнении memory

1. memory ≥ 95% → сжатие: replace старых записей короткими
2. Неактуальное → remove
3. Критичное → Obsidian vault (write_file)

## 6 baseline skills (обязательные при старте)

| # | Скилл | Зачем |
|---|-------|-------|
| 1 | `hermes-constitution` | Правила оркестрации, приоритеты |
| 2 | `communication-protocol` | 6 правил общения |
| 3 | `brand-voice-polyakov` | Голосовой профиль |
| 4 | `obsidian-context` | Загрузка Obsidian vault |
| 5 | `using-hermes-skills` | Роутер скиллов |
| 6 | `memory-preload` | Восстановление контекста сессии |

## Минимальный набор для нового агента

```yaml
# 1. System prompt
persona: "кто ты, роль, стиль"
memory_block: "2200 chars критических фактов"
user_profile: "1375 chars профиля пользователя"

# 2. Baseline skills (3-5)
skills:
  - constitution     # правила
  - protocol         # общение
  - voice            # голос
  - memory-preload   # восстановление контекста
  - skill-router     # роутер

# 3. Preload flow
preload:
  1_detect_role: "admin или tenant по $HOME"
  2_load_files: "user-profile.md, memory.md, project.md"
  3_verify_freshness: "git log, systemctl vs vault"
  4_session_history: "последние 3 сессии"

# 4. External storage
storage:
  type: "Obsidian vault или Markdown-файлы"
  search: "BM25 (без LLM) или embeddings"
  index: "00-Index.md"
```

## Статус проверки (23.06.2026)

| Слой | Статус | Детали |
|------|--------|--------|
| System Prompt | ✅ | MEMORY block 2,142/2,200 |
| Baseline skills | ✅ | 6 скиллов загружаются при старте |
| memory-preload | ✅ | Определение роли, загрузка vault |
| Obsidian vault | ✅ | BM25-поиск работает |
| session_search | ✅ | FTS5 по SQLite |
