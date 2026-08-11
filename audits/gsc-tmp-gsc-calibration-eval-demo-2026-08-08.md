---
title: "GSC Audit: /tmp/gsc-calibration/eval-demo"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/eval-demo

**Дата:** 08.08.2026 04:05  
**Путь:** `/tmp/gsc-calibration/eval-demo`  
**Всего находок:** 8  
**CRITICAL:** 1 | **HIGH:** 3 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025-eval_usage | 2 |
| GS001 | 1 |
| GS015 | 1 |
| GS008 | 1 |
| GS025 | 1 |
| GS004 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | expected.json | 1 | Found: "GS008" |
| HIGH | GS008 | app.py | 1 | Match: def exec(u): return eval(u) |
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | app.py | 1 | Line 1: def exec(u): return eval(u) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | expected.json | 1 |
| I | GS015 | app.py | 1 |
| H | GS008 | app.py | 1 |
| H | GS025 | expected.json | 0 |
| H | GS004 | app.py | 1 |
| s | GS009 |  | 0 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:05:11.907751*