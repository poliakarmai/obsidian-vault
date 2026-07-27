---
title: "GSC Audit: /tmp/gsc-learn/sqlmodel"
date: 2026-07-26
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/sqlmodel

**Дата:** 26.07.2026 04:00  
**Путь:** `/tmp/gsc-learn/sqlmodel`  
**Всего находок:** 32  
**CRITICAL:** 0 | **HIGH:** 20 | **MEDIUM:** 5 | **LOW:** 5

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| eval() or exec() usage | 8 |
| GS004 | 8 |
| Python: assert in production | 5 |
| GS003 | 4 |
| GS008 | 1 |
| GS015 | 1 |
| World-readable file: sponsors.yml (664) | 1 |
| World-readable file: mkdocs.env.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | session.py | 27 | Match:     def exec( |
| HIGH | ? | session.py | 39 | Match:     def exec( |
| HIGH | ? | session.py | 51 | Match:     def exec( |
| HIGH | ? | session.py | 62 | Match:     def exec( |
| HIGH | ? | session.py | 34 | Match:     async def exec( |
| HIGH | ? | session.py | 46 | Match:     async def exec( |
| HIGH | ? | session.py | 58 | Match:     async def exec( |
| HIGH | ? | session.py | 69 | Match:     async def exec( |
| HIGH | ? | sponsors.yml | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | ? | mkdocs.env.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | session.py | 34 | Line 34: async def exec( |
| HIGH | GS004 | session.py | 46 | Line 46: async def exec( |
| HIGH | GS004 | session.py | 58 | Line 58: async def exec( |
| HIGH | GS004 | session.py | 69 | Line 69: async def exec( |
| HIGH | GS004 | session.py | 27 | Line 27: def exec( |
| HIGH | GS004 | session.py | 39 | Line 39: def exec( |
| HIGH | GS004 | session.py | 51 | Line 51: def exec( |
| HIGH | GS004 | session.py | 62 | Line 62: def exec( |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | deploy_docs_status.py | 60 |
| M | ? | deploy_docs_status.py | 70 |
| M | ? | main.py | 757 |
| M | ? | main.py | 772 |
| M | ? | main.py | 773 |
| L | GS003 | add_latest_release_date.py | 24 |
| L | GS003 | add_latest_release_date.py | 29 |
| L | GS003 | add_latest_release_date.py | 34 |
| L | GS003 | deploy_docs_status.py | 109 |
| L | GS008 | _compat.py | 32 |
| I | GS015 | main.py | 1 |
| H | ? | session.py | 27 |
| H | ? | session.py | 39 |
| H | ? | session.py | 51 |
| H | ? | session.py | 62 |
| H | ? | session.py | 34 |
| H | ? | session.py | 46 |
| H | ? | session.py | 58 |
| H | ? | session.py | 69 |
| H | ? | sponsors.yml | 0 |
| H | ? | mkdocs.env.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | mkdocs.yml | 0 |
| H | GS004 | session.py | 34 |
| H | GS004 | session.py | 46 |
| H | GS004 | session.py | 58 |
| H | GS004 | session.py | 69 |
| H | GS004 | session.py | 27 |
| H | GS004 | session.py | 39 |
| H | GS004 | session.py | 51 |
| H | GS004 | session.py | 62 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-26T04:00:37.685695*