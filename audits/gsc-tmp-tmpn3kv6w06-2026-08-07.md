---
title: "GSC Audit: /tmp/tmpn3kv6w06"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpn3kv6w06

**Дата:** 07.08.2026 15:00  
**Путь:** `/tmp/tmpn3kv6w06`  
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
*Сгенерировано GSC v0.6 · 2026-08-07T15:00:18.029105*