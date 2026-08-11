---
title: "GSC Audit: /tmp/gsc-hunt-1"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-1

**Дата:** 10.08.2026 07:07  
**Путь:** `/tmp/gsc-hunt-1`  
**Всего находок:** 13  
**CRITICAL:** 1 | **HIGH:** 1 | **MEDIUM:** 2 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025-no_rate_limit_auth | 4 |
| GS025 | 2 |
| GS029 | 1 |
| GS001 | 1 |
| GS015 | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS021 | 1 |
| GS025-wildcard_bind | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | database.py | 5 | Found: DATABASE_URL = "sqlite:///./local_storage.db" |
| HIGH | GS025 | notify.py | 14 |  |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS025 | notify.py | 14 |
| M | GS025 | users_db_crud.py | 22 |
| M | GS029 | users_db_crud.py | 22 |
| C | GS001 | database.py | 5 |
| I | GS015 | main.py | 25 |
| s | GS009 |  | 0 |
| L | GS011 | authentication.py | 48 |
| s | GS021 |  | 50 |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-10T07:07:27.814749*