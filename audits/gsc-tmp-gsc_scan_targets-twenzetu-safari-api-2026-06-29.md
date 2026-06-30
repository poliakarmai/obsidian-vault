---
title: "GSC Audit: /tmp/gsc_scan_targets/twenzetu-safari-api"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/twenzetu-safari-api

**Дата:** 29.06.2026 14:22  
**Путь:** `/tmp/gsc_scan_targets/twenzetu-safari-api`  
**Всего находок:** 47  
**CRITICAL:** 12 | **HIGH:** 10 | **MEDIUM:** 6 | **LOW:** 18

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 18 |
| Python: File upload without content-type validation | 7 |
| GS001 | 6 |
| Hardcoded encryption key | 6 |
| GS012 | 6 |
| Хардкод IP адреса | 3 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | auth.json | 9 | Found: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBl |
| CRITICAL | GS001 | tests.py | 39 | Found: password='Pass1234!' |
| CRITICAL | GS001 | tests.py | 55 | Found: password='Pass1234!' |
| CRITICAL | GS001 | tests.py | 28 | Found: password='Pass1234!' |
| CRITICAL | GS001 | tests.py | 14 | Found: password='Pass1234!' |
| CRITICAL | GS001 | tests.py | 27 | Found: password='Pass1234!' |
| CRITICAL | ? | tests.py | 14 | Match:         self.user = User.objects.create_user(username |
| CRITICAL | ? | tests.py | 39 | Match:         User.objects.create_user(username='loginuser' |
| CRITICAL | ? | tests.py | 55 | Match:         user = User.objects.create_user(username='pro |
| CRITICAL | ? | tests.py | 28 | Match:         self.user = User.objects.create_user(username |
| CRITICAL | ? | views.py | 89 | Match:     cache_key = 'featured_attractions' |
| CRITICAL | ? | tests.py | 27 | Match:         self.user = User.objects.create_user(username |
| HIGH | ? | views.py | 24 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 48 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 49 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 73 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | services.py | 133 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 22 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 54 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | settings.py | 26 | Match: ALLOWED_HOSTS = config('ALLOWED_HOSTS', default='loca |
| HIGH | ? | settings.py | 172 | Match:     'http://127.0.0.1:8000', |
| HIGH | ? | settings.py | 204 | Match:     ] + [h for h in ALLOWED_HOSTS if h not in ('', 'l |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | views.py | 24 |
| H | ? | views.py | 48 |
| H | ? | views.py | 49 |
| H | ? | views.py | 73 |
| H | ? | services.py | 133 |
| H | ? | views.py | 22 |
| H | ? | views.py | 54 |
| C | GS001 | auth.json | 9 |
| C | GS001 | tests.py | 39 |
| C | GS001 | tests.py | 55 |
| C | GS001 | tests.py | 28 |
| C | GS001 | tests.py | 14 |
| C | GS001 | tests.py | 27 |
| L | GS008 | settings.py | 57 |
| L | GS008 | settings.py | 60 |
| L | GS008 | settings.py | 62 |
| L | GS008 | settings.py | 74 |
| L | GS008 | settings.py | 89 |
| L | GS008 | settings.py | 119 |
| L | GS008 | settings.py | 120 |
| L | GS008 | settings.py | 121 |
| L | GS008 | settings.py | 122 |
| L | GS008 | settings.py | 133 |
| L | GS008 | settings.py | 140 |
| L | GS008 | settings.py | 143 |
| L | GS008 | settings.py | 160 |
| L | GS008 | settings.py | 169 |
| L | GS008 | settings.py | 175 |
| L | GS008 | settings.py | 178 |
| L | GS008 | settings.py | 188 |
| L | GS008 | settings.py | 191 |
| H | ? | settings.py | 26 |
| H | ? | settings.py | 172 |
| H | ? | settings.py | 204 |
| C | ? | tests.py | 14 |
| C | ? | tests.py | 39 |
| C | ? | tests.py | 55 |
| C | ? | tests.py | 28 |
| C | ? | views.py | 89 |
| C | ? | tests.py | 27 |
| s | GS009 |  | 0 |
| M | GS012 | views.py | 0 |
| M | GS012 | views.py | 0 |
| M | GS012 | views.py | 0 |
| M | GS012 | views.py | 0 |
| M | GS012 | views.py | 0 |
| M | GS012 | services.py | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:22:05.891027*