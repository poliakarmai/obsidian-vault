---
title: "GSC Audit: /tmp/gsc_scan_targets/flask-jwt-auth"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/flask-jwt-auth

**Дата:** 29.06.2026 14:44  
**Путь:** `/tmp/gsc_scan_targets/flask-jwt-auth`  
**Всего находок:** 11  
**CRITICAL:** 0 | **HIGH:** 5 | **MEDIUM:** 0 | **LOW:** 5

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 3 |
| Debug mode enabled | 2 |
| GS011 | 2 |
| Python: File upload without content-type validation | 1 |
| World-readable file: .travis.yml (664) | 1 |
| GS009 | 1 |
| GS012 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | manage.py | 48 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | config.py | 19 | Match:     DEBUG = True |
| HIGH | ? | config.py | 26 | Match:     DEBUG = True |
| HIGH | ? | .travis.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS011 | config.py | 35 | Found JWT secret in code: 'my_preci...'. JWT secrets must be |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | manage.py | 48 |
| L | GS003 | manage.py | 49 |
| L | GS003 | manage.py | 54 |
| L | GS003 | views.py | 84 |
| H | ? | config.py | 19 |
| H | ? | config.py | 26 |
| H | ? | .travis.yml | 0 |
| s | GS009 |  | 0 |
| H | GS011 | config.py | 35 |
| L | GS011 | models.py | 55 |
| L | GS012 | manage.py | 48 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:44:20.681831*