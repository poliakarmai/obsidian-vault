---
title: "GSC Audit: /tmp/fastapi-users"
date: 2026-07-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/fastapi-users

**Дата:** 06.07.2026 09:10  
**Путь:** `/tmp/fastapi-users`  
**Всего находок:** 9  
**CRITICAL:** 5 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS001 | 5 |
| GS011 | 2 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | common.py | 23 | Found: TOKEN = "RESET_PASSWORD_BAD_TOKEN" |
| CRITICAL | GS001 | common.py | 25 | Found: TOKEN = "VERIFY_USER_BAD_TOKEN" |
| CRITICAL | GS001 | common.py | 16 | Found: PASSWORD = "REGISTER_INVALID_PASSWORD" |
| CRITICAL | GS001 | common.py | 24 | Found: PASSWORD = "RESET_PASSWORD_INVALID_PASSWORD" |
| CRITICAL | GS001 | common.py | 28 | Found: PASSWORD = "UPDATE_USER_INVALID_PASSWORD" |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS011 | oauth.py | 18 | Detected: KEY = "csrftoken" |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | common.py | 23 |
| C | GS001 | common.py | 25 |
| C | GS001 | common.py | 16 |
| C | GS001 | common.py | 24 |
| C | GS001 | common.py | 28 |
| H | ? | mkdocs.yml | 0 |
| s | GS009 |  | 0 |
| L | GS011 | jwt.py | 36 |
| H | GS011 | oauth.py | 18 |

---
*Сгенерировано GSC v0.6 · 2026-07-06T09:10:42.410009*