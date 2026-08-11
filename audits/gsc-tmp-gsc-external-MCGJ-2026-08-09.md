---
title: "GSC Audit: /tmp/gsc-external/MCGJ"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/MCGJ

**Дата:** 09.08.2026 07:22  
**Путь:** `/tmp/gsc-external/MCGJ`  
**Всего находок:** 32  
**CRITICAL:** 2 | **HIGH:** 2 | **MEDIUM:** 1 | **LOW:** 18

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 9 |
| GS012 | 8 |
| GS022 | 4 |
| GS007 | 3 |
| GS005 | 2 |
| GS025 | 1 |
| GS019 | 1 |
| GS010 | 1 |
| GS008 | 1 |
| GS009 | 1 |
| Deep analysis requires OpenRouter API key | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | models.py | 24 | OWASP A03: Injection |
| CRITICAL | GS005 | models.py | 24 |  |
| HIGH | GS025 | services.py | 50 |  |
| HIGH | GS019 | auth.py | 40 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | models.py | 24 |
| C | GS005 | models.py | 24 |
| H | GS025 | services.py | 50 |
| H | GS019 | auth.py | 40 |
| M | GS010 | db.py | 245 |
| L | GS003 | spotify_backfill.py | 63 |
| L | GS003 | spotify_export.py | 80 |
| L | GS003 | db.py | 58 |
| L | GS003 | db.py | 129 |
| L | GS003 | db.py | 134 |
| L | GS003 | db.py | 141 |
| L | GS003 | db.py | 155 |
| L | GS003 | main.js | 22 |
| L | GS003 | main.js | 51 |
| L | GS008 | models.py | 11 |
| I | GS007 | 001-init.sql | 2 |
| I | GS007 | 001-init.sql | 10 |
| I | GS007 | 001-init.sql | 18 |
| s | GS009 |  | 0 |
| L | GS012 | auth.py | 72 |
| L | GS012 | auth.py | 143 |
| L | GS012 | mcgj.py | 166 |
| L | GS012 | mcgj.py | 347 |
| L | GS012 | mcgj.py | 357 |
| L | GS012 | mcgj.py | 412 |
| L | GS012 | mcgj.py | 428 |
| L | GS012 | mcgj.py | 439 |
| r | GS022 |  | 81 |
| r | GS022 |  | 88 |
| r | GS022 |  | 3 |
| r | GS022 |  | 53 |
| I | ? |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T07:22:11.018569*