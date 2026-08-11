---
title: "GSC Audit: demo/repo"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — demo/repo

**Дата:** 07.08.2026 15:58  
**Путь:** `/home/openclaw/gsc/demo/repo`  
**Всего находок:** 20  
**CRITICAL:** 3 | **HIGH:** 1 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 10 |
| GS005 | 2 |
| GS007 | 2 |
| GS025-eval_usage | 2 |
| GS020 | 1 |
| GS008 | 1 |
| GS009 | 1 |
| GS025-debug_mode | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | app.py | 13 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 13 |  |
| CRITICAL | GS007 | app.py | 33 | Match:     return str(pickle.loads(base64.b64decode(data))) |
| HIGH | GS008 | app.py | 26 | Match:     return str(eval(expr)) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | app.py | 13 |
| M | GS007 | app.py | 33 |
| C | GS005 | app.py | 13 |
| I | GS015 | app.py | 16 |
| I | GS015 | app.py | 22 |
| I | GS015 | app.py | 28 |
| I | GS015 | app.py | 16 |
| I | GS015 | app.py | 22 |
| I | GS015 | app.py | 28 |
| I | GS015 | app.py | 16 |
| I | GS015 | app.py | 22 |
| I | GS015 | app.py | 28 |
| I | GS015 | app.py | 5 |
| i | GS020 |  | 20 |
| H | GS008 | app.py | 26 |
| C | GS007 | app.py | 33 |
| s | GS009 |  | 0 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-07T15:58:37.655692*