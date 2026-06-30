---
title: "GSC Audit: /tmp/gsc-learn/click"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/click

**Дата:** 29.06.2026 04:06  
**Путь:** `/tmp/gsc-learn/click`  
**Всего находок:** 12  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 9 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 8 |
| GS003 | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | core.py | 795 |
| M | ? | core.py | 1773 |
| M | ? | core.py | 1822 |
| M | ? | core.py | 1979 |
| M | ? | core.py | 2001 |
| M | ? | parser.py | 197 |
| M | ? | testing.py | 106 |
| M | ? | _winconsole.py | 35 |
| L | GS003 | testing.py | 7 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| M | ? | shell_completion.py | 326 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T04:06:48.879917*