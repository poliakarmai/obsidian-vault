---
title: "GSC Plugin Detector System (CVE Lite-inspired)"
created: 2026-06-26
tags: [gsc, security, architecture, detectors, plugin]
status: done
---

# GSC Plugin Detector System

Внедрена плагинная архитектура детекторов по образцу OWASP CVE Lite CLI.

## До / После

| | Было | Стало |
|---|------|-------|
| Архитектура | Flat grep-список из 135+ паттернов | Плагинные модули + grep-наследие |
| Новый детектор | Вписать regex в `check_source_driven()` | Создать модуль `gsNNN.py` → зарегистрировать |
| Интерфейс | Нет единого | `detect(ctx: AuditContext) → list[Finding]` |
| Контекст | Разбросан по переменным | `AuditContext` (project, path, files, cache, skipped) |
| Авто-фиксы | Нет | `fix_suggestion` + `references` в каждом Finding |

## Результаты первого прогона (bybit-ws)

| Детектор | Находок | Комментарий |
|----------|---------|-------------|
| GS001 (hardcoded secrets) | 0 | ✅ bybit-ws чист |
| GS002 (world-readable) | 0 | ✅ права норм |
| GS003 (debug prints) | 368 | print() во многих модулях |

Всего: 454 находки (368 plugin + 86 legacy grep)

## Структура

```
gsc/gsc_detectors/
├── __init__.py       ← AuditContext, Finding, Detector interface
├── registry.py       ← ALL_DETECTORS, get_detectors(), run_detectors()
├── gs001_hardcoded_secret.py
├── gs002_world_readable.py
└── gs003_debug_prints.py
```

## Интеграция с gsc.py

`check_plugin_detectors()` вызывается параллельно с legacy-проверками:
- Echelon 1: `check_source_driven()` + `check_plugin_detectors(echelon=1)` → GS001, GS003
- Echelon 2: `check_security()` + `check_plugin_detectors(echelon=2)` → GS002

При отсутствии `gsc_detectors/` — деградирует молча (ImportError → `return []`).
