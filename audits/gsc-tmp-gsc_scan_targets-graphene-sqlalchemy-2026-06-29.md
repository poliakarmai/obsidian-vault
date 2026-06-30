---
title: "GSC Audit: /tmp/gsc_scan_targets/graphene-sqlalchemy"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/graphene-sqlalchemy

**Дата:** 29.06.2026 14:21  
**Путь:** `/tmp/gsc_scan_targets/graphene-sqlalchemy`  
**Всего находок:** 16  
**CRITICAL:** 0 | **HIGH:** 1 | **MEDIUM:** 13 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 13 |
| GS003 | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | registry.py | 54 |
| M | ? | filters.py | 82 |
| M | ? | filters.py | 255 |
| M | ? | filters.py | 456 |
| M | ? | types.py | 461 |
| M | ? | types.py | 503 |
| M | ? | types.py | 699 |
| M | ? | batching.py | 70 |
| M | ? | batching.py | 72 |
| M | ? | fields.py | 35 |
| M | ? | fields.py | 38 |
| M | ? | fields.py | 41 |
| M | ? | fields.py | 105 |
| L | GS003 | types.py | 149 |
| H | ? | .pre-commit-config.yaml | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:21:54.799441*