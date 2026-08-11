---
title: "GSC Audit: /tmp/gsc-calibration/flask-jwt-auth"
date: 2026-08-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/flask-jwt-auth

**Дата:** 06.08.2026 06:44  
**Путь:** `/tmp/gsc-calibration/flask-jwt-auth`  
**Всего находок:** 24  
**CRITICAL:** 2 | **HIGH:** 6 | **MEDIUM:** 5 | **LOW:** 5

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| CVE-2026-56318: Information disclosure | 3 |
| GS003 | 3 |
| CVE-2026-37270: Hardcoded credential | 2 |
| Debug mode enabled | 2 |
| GS007 | 2 |
| GS011 | 2 |
| GS025-debug_mode | 2 |
| Python: File upload without content-type validation | 1 |
| JWT: Hardcoded secret <32 chars | 1 |
| GS001 | 1 |
| World-readable file: .travis.yml (664) | 1 |
| GS009 | 1 |
| GS012 | 1 |
| GS019 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | models.py | 42 | Found: 'HS256' |
| CRITICAL | GS019 | config.py | 35 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | ? | manage.py | 48 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | config.py | 35 | Hacking APIs (No Starch Press) |
| HIGH | ? | config.py | 19 | Match:     DEBUG = True |
| HIGH | ? | config.py | 26 | Match:     DEBUG = True |
| HIGH | ? | .travis.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS011 | config.py | 35 | Found JWT secret in code: 'my_preci...'. JWT secrets must be |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | manage.py | 48 |
| H | ? | config.py | 35 |
| M | ? | config.py | 35 |
| M | ? | views.py | 109 |
| M | ? | views.py | 147 |
| M | ? | views.py | 109 |
| M | ? | views.py | 147 |
| C | GS001 | models.py | 42 |
| L | GS003 | manage.py | 49 |
| L | GS003 | manage.py | 54 |
| L | GS003 | views.py | 84 |
| H | ? | config.py | 19 |
| H | ? | config.py | 26 |
| H | ? | .travis.yml | 0 |
| I | GS007 | models.py | 14 |
| I | GS007 | models.py | 88 |
| s | GS009 |  | 0 |
| H | GS011 | config.py | 35 |
| L | GS011 | models.py | 70 |
| L | GS012 | manage.py | 48 |
| C | GS019 | config.py | 35 |
| s | GS021 |  | 5 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-06T06:44:44.109724*