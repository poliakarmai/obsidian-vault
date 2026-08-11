---
title: "GSC Audit: /tmp/tmp5qo86hnj"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmp5qo86hnj

**Дата:** 05.08.2026 12:24  
**Путь:** `/tmp/tmp5qo86hnj`  
**Всего находок:** 5  
**CRITICAL:** 2 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025-eval_exec_usage | 2 |
| eval() or exec() usage | 1 |
| GS004 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS025-eval_exec_usage | test.py | 1 | def exec(u): return eval(u) | ai_provenance: 0% |
| CRITICAL | GS025-eval_exec_usage | test.py | 1 | def exec(u): return eval(u) | ai_provenance: 0% |
| HIGH | ? | test.py | 1 | Match: def exec(u): return eval(u) |
| HIGH | GS004 | test.py | 1 | Line 1: def exec(u): return eval(u) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | test.py | 1 |
| H | GS004 | test.py | 1 |
| s | GS009 |  | 0 |
| C | GS025-eval_exec_usage | test.py | 1 |
| C | GS025-eval_exec_usage | test.py | 1 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T12:24:03.302634*