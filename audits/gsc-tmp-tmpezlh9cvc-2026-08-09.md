---
title: "GSC Audit: /tmp/tmpezlh9cvc"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpezlh9cvc

**Дата:** 09.08.2026 09:57  
**Путь:** `/tmp/tmpezlh9cvc`  
**Всего находок:** 7  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025-eval_usage | 2 |
| YAML-36ACF0AD | 2 |
| GS008 | 1 |
| GS004 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS008 | test.py | 1 | Match: def exec(u): return eval(u) |
| HIGH | GS004 | test.py | 1 | Line 1: def exec(u): return eval(u) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS008 | test.py | 1 |
| H | GS004 | test.py | 1 |
| s | GS009 |  | 0 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | test.py | ? |
| ? | YAML-36ACF0AD | test.py | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-09T09:57:35.386690*