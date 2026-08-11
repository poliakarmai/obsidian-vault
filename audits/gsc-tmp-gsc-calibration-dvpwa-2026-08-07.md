---
title: "GSC Audit: /tmp/gsc-calibration/dvpwa"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/dvpwa

**Дата:** 07.08.2026 11:48  
**Путь:** `/tmp/gsc-calibration/dvpwa`  
**Всего находок:** 94  
**CRITICAL:** 4 | **HIGH:** 7 | **MEDIUM:** 0 | **LOW:** 29

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 20 |
| GS020 | 20 |
| GS025-eval_usage | 19 |
| GS008 | 5 |
| GS007 | 5 |
| GS012 | 4 |
| Rust: .clone() in hot path | 4 |
| Weak password validation | 3 |
| GS021 | 3 |
| GS022 | 3 |
| SQL injection risk: f-string in query | 1 |
| GS015 | 1 |
| Хардкод IP адреса | 1 |
| World-readable file: docker-compose.yml (664) | 1 |
| World-readable file: Dockerfile.db (664) | 1 |
| GS009 | 1 |
| GS025-debug_mode | 1 |
| GS025-insecure_random | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | materialize.min.js | 6 | OWASP A03: Injection |
| CRITICAL | ? | forms.py | 9 | Match:     T.Key('review_text'): T.String(min_length=1), |
| CRITICAL | ? | forms.py | 13 | Match:     T.Key('name'): T.String(min_length=1), |
| CRITICAL | ? | forms.py | 17 | Match:     T.Key('title'): T.String(min_length=1, max_length |
| HIGH | ? | dev.yaml | 14 | Match:   host: 0.0.0.0 |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | Dockerfile.db | 0 | Permissions 664 — should be 600 |
| HIGH | ? | materialize.js | 8714 | Clone in performance-critical code — consider references |
| HIGH | ? | materialize.js | 8727 | Clone in performance-critical code — consider references |
| HIGH | ? | materialize.js | 8743 | Clone in performance-critical code — consider references |
| HIGH | ? | materialize.min.js | 6 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | materialize.min.js | 6 |
| L | GS003 | materialize.js | 173 |
| L | GS003 | materialize.js | 592 |
| L | GS003 | materialize.js | 601 |
| L | GS003 | materialize.js | 602 |
| L | GS003 | materialize.js | 645 |
| L | GS003 | materialize.js | 657 |
| L | GS003 | materialize.js | 661 |
| L | GS003 | materialize.js | 699 |
| L | GS003 | materialize.js | 700 |
| L | GS003 | materialize.js | 754 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS003 | materialize.min.js | 6 |
| L | GS008 | config.py | 4 |
| L | GS008 | forms.py | 4 |
| L | GS008 | forms.py | 8 |
| L | GS008 | forms.py | 12 |
| L | GS008 | forms.py | 16 |
| I | GS015 | app.py | 23 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 4 |
| i | GS020 |  | 2 |
| i | GS020 |  | 3 |
| i | GS020 |  | 396 |
| i | GS020 |  | 3444 |
| i | GS020 |  | 8589 |
| i | GS020 |  | 8591 |
| i | GS020 |  | 6 |
| i | GS020 |  | 6 |
| i | GS020 |  | 6 |
| i | GS020 |  | 6 |
| i | GS020 |  | 6 |
| H | ? | dev.yaml | 14 |
| C | ? | forms.py | 9 |
| C | ? | forms.py | 13 |
| C | ? | forms.py | 17 |
| H | ? | docker-compose.yml | 0 |
| H | ? | Dockerfile.db | 0 |
| I | GS007 | 000-init-schema.sql | 2 |
| I | GS007 | 000-init-schema.sql | 13 |
| I | GS007 | 000-init-schema.sql | 20 |
| I | GS007 | 000-init-schema.sql | 28 |
| I | GS007 | 000-init-schema.sql | 39 |
| s | GS009 |  | 0 |
| L | GS012 | materialize.js | 1078 |
| L | GS012 | materialize.js | 1179 |
| L | GS012 | materialize.js | 1195 |
| L | GS012 | materialize.js | 1197 |
| c | GS021 |  | 20 |
| s | GS021 |  | 4 |
| s | GS021 |  | 6 |
| r | GS022 |  | 3 |
| r | GS022 |  | 5230 |
| r | GS022 |  | 6 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| H | ? | materialize.js | 8714 |
| H | ? | materialize.js | 8727 |
| H | ? | materialize.js | 8743 |
| H | ? | materialize.min.js | 6 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T11:48:05.784741*