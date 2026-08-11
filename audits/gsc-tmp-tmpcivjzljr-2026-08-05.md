---
title: "GSC Audit: /tmp/tmpcivjzljr"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpcivjzljr

**Дата:** 05.08.2026 05:09  
**Путь:** `/tmp/tmpcivjzljr`  
**Всего находок:** 3  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| eval() or exec() usage | 1 |
| GS004 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | test.py | 1 | Match: def exec(u): return eval(u) |
| HIGH | GS004 | test.py | 1 | Line 1: def exec(u): return eval(u) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | test.py | 1 |
| H | GS004 | test.py | 1 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T05:09:50.100434*