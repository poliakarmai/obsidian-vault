---
title: "GSC Audit: /tmp/gsc_scan_targets/tock"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/tock

**Дата:** 29.06.2026 14:26  
**Путь:** `/tmp/gsc_scan_targets/tock`  
**Всего находок:** 183  
**CRITICAL:** 2 | **HIGH:** 69 | **MEDIUM:** 0 | **LOW:** 105

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 58 |
| Python: File upload without content-type validation | 54 |
| GS012 | 42 |
| GS015 | 6 |
| GS003 | 5 |
| Хардкод IP адреса | 3 |
| Debug mode enabled | 2 |
| GS014 | 2 |
| SQL injection risk: f-string in query | 1 |
| Python: SSRF via requests without URL validation | 1 |
| GS001 | 1 |
| User-controlled URL in request | 1 |
| World-readable file: package-lock.json (664) | 1 |
| World-readable file: package.json (664) | 1 |
| World-readable file: docker-compose.yml (664) | 1 |
| World-readable file: manifest-staging.yml (664) | 1 |
| World-readable file: manifest-production.yml (664) | 1 |
| GS009 | 1 |
| GS011 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | plotly-basic-2.8.3.min.js | 24 | OWASP A03: Injection |
| CRITICAL | GS001 | dev.py | 25 | Found: postgres://tock:tock@localho |
| HIGH | ? | compliance.py | 15 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | tests.py | 79 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 86 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 98 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 106 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 113 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 121 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 132 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 142 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 152 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 184 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 195 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 221 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 241 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 265 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 288 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 314 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 386 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 396 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 406 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 413 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 421 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 429 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 435 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 498 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 505 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 512 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 523 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 534 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 128 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 295 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 42 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 218 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 290 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 508 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 597 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 335 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 427 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 616 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 621 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 623 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 11 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 403 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | tests.py | 422 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | update_billable_expectations.py | 29 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | update_billable_expectations.py | 35 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | calculate_timecard_utilization.py | 16 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | manage.py | 65 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | remote_user_auth.py | 80 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 77 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 209 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 219 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 221 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 82 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 87 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | docker-compose.yml | 21 | Match:     command: "python manage.py runserver 0.0.0.0:8000 |
| HIGH | ? | plotly-basic-2.8.3.min.js | 24 | Match: var n,a=e("./lib/build-log"),i=e("./lib/epsilon"),o=e |
| HIGH | ? | dev.py | 20 | Match:     '127.0.0.1', |
| HIGH | ? | dev.py | 9 | Match: DEBUG = True |
| HIGH | ? | test.py | 10 | Match: DEBUG = True |
| HIGH | ? | compliance.py | 15 | Match: resp = requests.get(f"{url}/users.json", headers=head |
| HIGH | ? | package-lock.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | package.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | manifest-staging.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | manifest-production.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS011 | dev.py | 11 | Found JWT secret in code: 'developm...'. JWT secrets must be |
| HIGH | GS014 | docker-compose.yml | 13 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | dev.py | 25 | Database URL contains password in plaintext. Use environment |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | plotly-basic-2.8.3.min.js | 24 |
| H | ? | compliance.py | 15 |
| H | ? | tests.py | 79 |
| H | ? | tests.py | 86 |
| H | ? | tests.py | 98 |
| H | ? | tests.py | 106 |
| H | ? | tests.py | 113 |
| H | ? | tests.py | 121 |
| H | ? | tests.py | 132 |
| H | ? | tests.py | 142 |
| H | ? | tests.py | 152 |
| H | ? | tests.py | 184 |
| H | ? | tests.py | 195 |
| H | ? | tests.py | 221 |
| H | ? | tests.py | 241 |
| H | ? | tests.py | 265 |
| H | ? | tests.py | 288 |
| H | ? | tests.py | 314 |
| H | ? | tests.py | 386 |
| H | ? | tests.py | 396 |
| H | ? | tests.py | 406 |
| H | ? | tests.py | 413 |
| H | ? | tests.py | 421 |
| H | ? | tests.py | 429 |
| H | ? | tests.py | 435 |
| H | ? | tests.py | 498 |
| H | ? | tests.py | 505 |
| H | ? | tests.py | 512 |
| H | ? | tests.py | 523 |
| H | ? | tests.py | 534 |
| H | ? | models.py | 128 |
| H | ? | models.py | 295 |
| H | ? | models.py | 42 |
| H | ? | models.py | 218 |
| H | ? | models.py | 290 |
| H | ? | models.py | 508 |
| H | ? | models.py | 597 |
| H | ? | forms.py | 335 |
| H | ? | views.py | 427 |
| H | ? | views.py | 616 |
| H | ? | views.py | 621 |
| H | ? | views.py | 623 |
| H | ? | utils.py | 11 |
| H | ? | tests.py | 403 |
| H | ? | tests.py | 422 |
| H | ? | update_billable_expectations.py | 29 |
| H | ? | update_billable_expectations.py | 35 |
| H | ? | calculate_timecard_utilization.py | 16 |
| H | ? | manage.py | 65 |
| H | ? | remote_user_auth.py | 80 |
| H | ? | models.py | 77 |
| H | ? | models.py | 209 |
| H | ? | models.py | 219 |
| H | ? | models.py | 221 |
| H | ? | views.py | 82 |
| H | ? | views.py | 87 |
| C | GS001 | dev.py | 25 |
| L | GS003 | compliance.py | 30 |
| L | GS003 | compliance.py | 31 |
| L | GS003 | manage.py | 35 |
| L | GS003 | manage.py | 36 |
| L | GS003 | filter_report_table.js | 25 |
| L | GS008 | base.py | 20 |
| L | GS008 | base.py | 22 |
| L | GS008 | base.py | 27 |
| L | GS008 | base.py | 29 |
| L | GS008 | base.py | 47 |
| L | GS008 | base.py | 72 |
| L | GS008 | base.py | 86 |
| L | GS008 | base.py | 90 |
| L | GS008 | base.py | 92 |
| L | GS008 | base.py | 93 |
| L | GS008 | base.py | 94 |
| L | GS008 | base.py | 95 |
| L | GS008 | base.py | 96 |
| L | GS008 | base.py | 98 |
| L | GS008 | base.py | 101 |
| L | GS008 | base.py | 122 |
| L | GS008 | base.py | 131 |
| L | GS008 | base.py | 133 |
| L | GS008 | base.py | 136 |
| L | GS008 | base.py | 137 |
| L | GS008 | base.py | 138 |
| L | GS008 | base.py | 141 |
| L | GS008 | base.py | 142 |
| L | GS008 | base.py | 143 |
| L | GS008 | base.py | 146 |
| L | GS008 | base.py | 147 |
| L | GS008 | base.py | 148 |
| L | GS008 | base.py | 156 |
| L | GS008 | base.py | 159 |
| L | GS008 | dev.py | 17 |
| L | GS008 | dev.py | 19 |
| L | GS008 | dev.py | 44 |
| L | GS008 | dev.py | 54 |
| L | GS008 | dev.py | 58 |
| L | GS008 | dev.py | 65 |
| L | GS008 | dev.py | 70 |
| L | GS008 | production.py | 11 |
| L | GS008 | production.py | 15 |
| L | GS008 | production.py | 20 |
| L | GS008 | production.py | 21 |
| L | GS008 | production.py | 22 |
| L | GS008 | production.py | 23 |
| L | GS008 | production.py | 32 |
| L | GS008 | production.py | 33 |
| L | GS008 | production.py | 34 |
| L | GS008 | production.py | 35 |
| L | GS008 | production.py | 36 |
| L | GS008 | production.py | 37 |
| L | GS008 | production.py | 38 |
| L | GS008 | production.py | 40 |
| L | GS008 | production.py | 46 |
| L | GS008 | production.py | 47 |
| L | GS008 | production.py | 49 |
| L | GS008 | test.py | 10 |
| L | GS008 | test.py | 12 |
| L | GS008 | test.py | 22 |
| L | GS008 | test.py | 24 |
| L | GS008 | test.py | 26 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 29 |
| I | GS015 | urls.py | 1 |
| H | ? | docker-compose.yml | 21 |
| H | ? | plotly-basic-2.8.3.min.js | 24 |
| H | ? | dev.py | 20 |
| H | ? | dev.py | 9 |
| H | ? | test.py | 10 |
| H | ? | compliance.py | 15 |
| H | ? | package-lock.json | 0 |
| H | ? | package.json | 0 |
| H | ? | docker-compose.yml | 0 |
| H | ? | manifest-staging.yml | 0 |
| H | ? | manifest-production.yml | 0 |
| s | GS009 |  | 0 |
| H | GS011 | dev.py | 11 |
| L | GS012 | tests.py | 403 |
| L | GS012 | tests.py | 422 |
| L | GS012 | models.py | 209 |
| L | GS012 | models.py | 219 |
| L | GS012 | views.py | 82 |
| L | GS012 | views.py | 87 |
| L | GS012 | views.py | 427 |
| L | GS012 | views.py | 621 |
| L | GS012 | views.py | 623 |
| L | GS012 | manage.py | 65 |
| L | GS012 | tests.py | 79 |
| L | GS012 | tests.py | 86 |
| L | GS012 | tests.py | 98 |
| L | GS012 | tests.py | 106 |
| L | GS012 | tests.py | 113 |
| L | GS012 | tests.py | 121 |
| L | GS012 | tests.py | 132 |
| L | GS012 | tests.py | 142 |
| L | GS012 | tests.py | 152 |
| L | GS012 | tests.py | 184 |
| L | GS012 | tests.py | 195 |
| L | GS012 | tests.py | 221 |
| L | GS012 | tests.py | 241 |
| L | GS012 | tests.py | 265 |
| L | GS012 | tests.py | 288 |
| L | GS012 | tests.py | 314 |
| L | GS012 | tests.py | 386 |
| L | GS012 | tests.py | 396 |
| L | GS012 | tests.py | 406 |
| L | GS012 | tests.py | 413 |
| L | GS012 | tests.py | 421 |
| L | GS012 | tests.py | 429 |
| L | GS012 | tests.py | 435 |
| L | GS012 | tests.py | 498 |
| L | GS012 | tests.py | 505 |
| L | GS012 | tests.py | 512 |
| L | GS012 | tests.py | 523 |
| L | GS012 | tests.py | 534 |
| L | GS012 | calculate_timecard_utilization.py | 16 |
| L | GS012 | update_billable_expectations.py | 29 |
| L | GS012 | update_billable_expectations.py | 35 |
| L | GS012 | remote_user_auth.py | 80 |
| H | GS014 | docker-compose.yml | 13 |
| H | GS014 | dev.py | 25 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:26:41.332697*