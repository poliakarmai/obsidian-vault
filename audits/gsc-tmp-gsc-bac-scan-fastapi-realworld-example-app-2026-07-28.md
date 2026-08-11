---
title: "GSC Audit: /tmp/gsc-bac-scan/fastapi-realworld-example-app"
date: 2026-07-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-bac-scan/fastapi-realworld-example-app

**Дата:** 28.07.2026 19:13  
**Путь:** `/tmp/gsc-bac-scan/fastapi-realworld-example-app`  
**Всего находок:** 102  
**CRITICAL:** 3 | **HIGH:** 11 | **MEDIUM:** 0 | **LOW:** 18

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 69 |
| GS008 | 17 |
| Хардкод IP адреса | 8 |
| Weak password validation | 2 |
| GS011 | 2 |
| GS001 | 1 |
| World-readable file: docker-compose.yml (664) | 1 |
| GS009 | 1 |
| GS014 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | docker-compose.yml | 10 | Found: DATABASE_URL: "postgresql://postgres:postgres@db/post |
| CRITICAL | ? | articles.py | 38 | Match:     slug: str = Path(..., min_length=1), |
| CRITICAL | ? | profiles.py | 16 | Match:     username: str = Path(..., min_length=1), |
| HIGH | ? | Dockerfile | 21 | Match:     poetry run uvicorn --host=0.0.0.0 app.main:app |
| HIGH | ? | poetry.lock | 155 | Match: typing-extensions = {version = ">=3.10.0.0", markers  |
| HIGH | ? | poetry.lock | 803 | Match: typing-extensions = ">=3.7.4.3" |
| HIGH | ? | poetry.lock | 1066 | Match: aiosqlite = ["typing_extensions (!=3.10.0.1)", "green |
| HIGH | ? | poetry.lock | 1142 | Match: version = "3.10.0.2" |
| HIGH | ? | poetry.lock | 2029 | Match:     {file = "typing_extensions-3.10.0.2-py2-none-any. |
| HIGH | ? | poetry.lock | 2030 | Match:     {file = "typing_extensions-3.10.0.2-py3-none-any. |
| HIGH | ? | poetry.lock | 2031 | Match:     {file = "typing_extensions-3.10.0.2.tar.gz", hash |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS011 | authentication.py | 18 | Detected: KEY = "Authorization" |
| HIGH | GS014 | docker-compose.yml | 10 | Database URL contains password in plaintext. Use environment |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | docker-compose.yml | 10 |
| L | GS008 | articles.py | 25 |
| L | GS008 | strings.py | 3 |
| L | GS008 | strings.py | 4 |
| L | GS008 | strings.py | 5 |
| L | GS008 | strings.py | 6 |
| L | GS008 | strings.py | 8 |
| L | GS008 | strings.py | 9 |
| L | GS008 | strings.py | 10 |
| L | GS008 | strings.py | 12 |
| L | GS008 | strings.py | 13 |
| L | GS008 | strings.py | 14 |
| L | GS008 | strings.py | 15 |
| L | GS008 | strings.py | 18 |
| L | GS008 | strings.py | 20 |
| L | GS008 | strings.py | 21 |
| L | GS008 | strings.py | 23 |
| L | GS008 | strings.py | 25 |
| I | GS015 | articles.py | 1 |
| I | GS015 | authentication.py | 1 |
| I | GS015 | comments.py | 1 |
| I | GS015 | database.py | 1 |
| I | GS015 | profiles.py | 1 |
| I | GS015 | http_error.py | 1 |
| I | GS015 | validation_error.py | 1 |
| I | GS015 | api.py | 1 |
| I | GS015 | api.py | 1 |
| I | GS015 | articles_common.py | 22 |
| I | GS015 | articles_common.py | 47 |
| I | GS015 | articles_common.py | 77 |
| I | GS015 | articles_common.py | 22 |
| I | GS015 | articles_common.py | 47 |
| I | GS015 | articles_common.py | 77 |
| I | GS015 | articles_common.py | 22 |
| I | GS015 | articles_common.py | 47 |
| I | GS015 | articles_common.py | 77 |
| I | GS015 | articles_resource.py | 30 |
| I | GS015 | articles_resource.py | 53 |
| I | GS015 | articles_resource.py | 82 |
| I | GS015 | articles_resource.py | 89 |
| I | GS015 | articles_resource.py | 109 |
| I | GS015 | articles_resource.py | 30 |
| I | GS015 | articles_resource.py | 53 |
| I | GS015 | articles_resource.py | 82 |
| I | GS015 | articles_resource.py | 89 |
| I | GS015 | articles_resource.py | 109 |
| I | GS015 | articles_resource.py | 30 |
| I | GS015 | articles_resource.py | 53 |
| I | GS015 | articles_resource.py | 82 |
| I | GS015 | articles_resource.py | 89 |
| I | GS015 | articles_resource.py | 109 |
| I | GS015 | authentication.py | 22 |
| I | GS015 | authentication.py | 56 |
| I | GS015 | authentication.py | 22 |
| I | GS015 | authentication.py | 56 |
| I | GS015 | authentication.py | 22 |
| I | GS015 | authentication.py | 56 |
| I | GS015 | comments.py | 26 |
| I | GS015 | comments.py | 40 |
| I | GS015 | comments.py | 60 |
| I | GS015 | comments.py | 26 |
| I | GS015 | comments.py | 40 |
| I | GS015 | comments.py | 60 |
| I | GS015 | comments.py | 26 |
| I | GS015 | comments.py | 40 |
| I | GS015 | comments.py | 60 |
| I | GS015 | profiles.py | 16 |
| I | GS015 | profiles.py | 27 |
| I | GS015 | profiles.py | 57 |
| I | GS015 | profiles.py | 16 |
| I | GS015 | profiles.py | 27 |
| I | GS015 | profiles.py | 57 |
| I | GS015 | profiles.py | 16 |
| I | GS015 | profiles.py | 27 |
| I | GS015 | profiles.py | 57 |
| I | GS015 | tags.py | 10 |
| I | GS015 | tags.py | 10 |
| I | GS015 | tags.py | 10 |
| I | GS015 | users.py | 18 |
| I | GS015 | users.py | 38 |
| I | GS015 | users.py | 18 |
| I | GS015 | users.py | 38 |
| I | GS015 | users.py | 18 |
| I | GS015 | users.py | 38 |
| I | GS015 | app.py | 1 |
| I | GS015 | main.py | 18 |
| I | GS015 | main.py | 45 |
| H | ? | Dockerfile | 21 |
| H | ? | poetry.lock | 155 |
| H | ? | poetry.lock | 803 |
| H | ? | poetry.lock | 1066 |
| H | ? | poetry.lock | 1142 |
| H | ? | poetry.lock | 2029 |
| H | ? | poetry.lock | 2030 |
| H | ? | poetry.lock | 2031 |
| C | ? | articles.py | 38 |
| C | ? | profiles.py | 16 |
| H | ? | docker-compose.yml | 0 |
| s | GS009 |  | 0 |
| H | GS011 | authentication.py | 18 |
| L | GS011 | jwt.py | 37 |
| H | GS014 | docker-compose.yml | 10 |

---
*Сгенерировано GSC v0.6 · 2026-07-28T19:13:49.135699*