---
title: "GSC Audit: /tmp/tmp_74aq9mf"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmp_74aq9mf

**Дата:** 08.08.2026 08:57  
**Путь:** `/tmp/tmp_74aq9mf`  
**Всего находок:** 5  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025-eval_usage | 2 |
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

---
*Сгенерировано GSC v0.6 · 2026-08-08T08:57:33.009271*