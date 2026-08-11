---
title: "GSC Audit: /tmp/gsc-learn/click"
date: 2026-07-30
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/click

**Дата:** 30.07.2026 04:10  
**Путь:** `/tmp/gsc-learn/click`  
**Всего находок:** 14  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 9 | **LOW:** 2

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 8 |
| GS003 | 1 |
| GS008 | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | _winconsole.py | 35 |
| M | ? | testing.py | 106 |
| M | ? | parser.py | 197 |
| M | ? | core.py | 799 |
| M | ? | core.py | 1814 |
| M | ? | core.py | 1863 |
| M | ? | core.py | 2020 |
| M | ? | core.py | 2042 |
| L | GS003 | testing.py | 7 |
| L | GS008 | _compat.py | 13 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| s | GS009 |  | 0 |
| M | ? | shell_completion.py | 405 |

---
*Сгенерировано GSC v0.6 · 2026-07-30T04:10:12.889518*