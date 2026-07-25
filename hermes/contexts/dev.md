# Dev-контекст

> Загружать при входе в dev-режим (код, архитектура, деплой)

## Codebase-Memory MCP

Проекты в индексе: `list_projects`

| Задача | Инструмент |
|--------|-----------|
| Найти определение | `search_graph(query="...")` |
| Граф вызовов | `trace_path(function_name="...")` |
| Хотспоты/O(n²) | `query_graph` → `transitive_loop_depth >= 3` |
| Фрагмент кода | `get_code_snippet(qualified_name="...")` |
| Что сломал коммит | `detect_changes(since="HEAD~1")` |

## Проекты

| Проект | Путь | AGENTS.md |
|--------|------|-----------|
| bybit-ws | `~/bybit-ws/` | ✅ (98 строк) |
| gsc | `~/gsc/` | ✅ |
| baza | `~/baza/` | shared KB, web UI |
| hermes-infra | `~/hermes-infra/` | openwiki docs |

## Правила

- **Judge** перед изменениями кода/конфигов
- **Credential scanner** маскирует токены в shell → Python-скрипт через write_file + terminal
- **systemctl daemon-reload** после создания drop-in'ов
- **HERMES config**: править только через `hermes config set`, не patch/write_file
- **Gateway**: НЕ рестартить в середине сессии. Промпты/скиллы → /new
