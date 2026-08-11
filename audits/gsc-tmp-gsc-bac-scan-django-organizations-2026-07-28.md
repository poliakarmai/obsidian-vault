---
title: "GSC Audit: /tmp/gsc-bac-scan/django-organizations"
date: 2026-07-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-bac-scan/django-organizations

**Дата:** 28.07.2026 19:15  
**Путь:** `/tmp/gsc-bac-scan/django-organizations`  
**Всего находок:** 66  
**CRITICAL:** 4 | **HIGH:** 20 | **MEDIUM:** 6 | **LOW:** 31

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 22 |
| Python: File upload without content-type validation | 12 |
| GS012 | 9 |
| CVE-2026-37270: Hardcoded credential | 4 |
| GS015 | 4 |
| Hardcoded encryption key | 4 |
| CVE-2026-56318: Information disclosure | 2 |
| Debug mode enabled | 2 |
| GS011 | 2 |
| JWT: Hardcoded secret <32 chars | 1 |
| Хардкод IP адреса | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | base.py | 64 | Match:                 key = "OrgModel" |
| CRITICAL | ? | base.py | 66 | Match:                 key = "OrgUserModel" |
| CRITICAL | ? | base.py | 68 | Match:                 key = "OrgOwnerModel" |
| CRITICAL | ? | base.py | 73 | Match:                 key = "OrgInviteModel" |
| HIGH | ? | base.py | 357 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | base.py | 382 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 32 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | abstract.py | 200 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | abstract.py | 328 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | modeled.py | 90 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | defaults.py | 107 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | defaults.py | 126 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | defaults.py | 128 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | defaults.py | 240 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | defaults.py | 273 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | defaults.py | 352 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | manage.py | 72 | Hacking APIs (No Starch Press) |
| HIGH | ? | settings.py | 133 | Match: INTERNAL_IPS = ("127.0.0.1",) |
| HIGH | ? | manage.py | 34 | Match:     DEBUG=True, |
| HIGH | ? | settings.py | 8 | Match: DEBUG = True |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS011 | settings.py | 80 | Found JWT secret in code: '7@m$nx@q...'. JWT secrets must be |
| HIGH | GS011 | manage.py | 72 | Found JWT secret in code: 'ThisIsHo...'. JWT secrets must be |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | base.py | 357 |
| H | ? | base.py | 382 |
| H | ? | forms.py | 32 |
| H | ? | abstract.py | 200 |
| H | ? | abstract.py | 328 |
| H | ? | modeled.py | 90 |
| H | ? | defaults.py | 107 |
| H | ? | defaults.py | 126 |
| H | ? | defaults.py | 128 |
| H | ? | defaults.py | 240 |
| H | ? | defaults.py | 273 |
| H | ? | defaults.py | 352 |
| H | ? | manage.py | 72 |
| M | ? | manage.py | 72 |
| M | ? | settings.py | 80 |
| M | ? | base.py | 64 |
| M | ? | base.py | 66 |
| M | ? | base.py | 68 |
| M | ? | base.py | 73 |
| L | GS008 | settings.py | 9 |
| L | GS008 | settings.py | 15 |
| L | GS008 | settings.py | 17 |
| L | GS008 | settings.py | 26 |
| L | GS008 | settings.py | 30 |
| L | GS008 | settings.py | 32 |
| L | GS008 | settings.py | 36 |
| L | GS008 | settings.py | 40 |
| L | GS008 | settings.py | 43 |
| L | GS008 | settings.py | 58 |
| L | GS008 | settings.py | 83 |
| L | GS008 | settings.py | 96 |
| L | GS008 | settings.py | 98 |
| L | GS008 | settings.py | 133 |
| L | GS008 | settings.py | 135 |
| L | GS008 | settings.py | 137 |
| L | GS008 | settings.py | 155 |
| L | GS008 | settings.py | 175 |
| L | GS008 | abstract.py | 19 |
| L | GS008 | app_settings.py | 6 |
| L | GS008 | app_settings.py | 10 |
| L | GS008 | app_settings.py | 16 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 22 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| H | ? | settings.py | 133 |
| C | ? | base.py | 64 |
| C | ? | base.py | 66 |
| C | ? | base.py | 68 |
| C | ? | base.py | 73 |
| H | ? | manage.py | 34 |
| H | ? | settings.py | 8 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| s | GS009 |  | 0 |
| H | GS011 | settings.py | 80 |
| H | GS011 | manage.py | 72 |
| L | GS012 | abstract.py | 200 |
| L | GS012 | defaults.py | 107 |
| L | GS012 | defaults.py | 126 |
| L | GS012 | defaults.py | 128 |
| L | GS012 | defaults.py | 240 |
| L | GS012 | defaults.py | 273 |
| L | GS012 | defaults.py | 352 |
| L | GS012 | modeled.py | 90 |
| L | GS012 | base.py | 382 |

---
*Сгенерировано GSC v0.6 · 2026-07-28T19:15:07.862459*