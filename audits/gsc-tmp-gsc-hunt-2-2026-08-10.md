---
title: "GSC Audit: /tmp/gsc-hunt-2"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-2

**Дата:** 10.08.2026 07:07  
**Путь:** `/tmp/gsc-hunt-2`  
**Всего находок:** 22  
**CRITICAL:** 0 | **HIGH:** 1 | **MEDIUM:** 0 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 16 |
| GS022 | 2 |
| GS003 | 1 |
| GS009 | 1 |
| GS019 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS019 | main.py | 31 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS003 | main.py | 62 |
| I | GS015 | main.py | 30 |
| I | GS015 | main.py | 35 |
| I | GS015 | main.py | 41 |
| I | GS015 | main.py | 66 |
| I | GS015 | main.py | 71 |
| I | GS015 | main.py | 30 |
| I | GS015 | main.py | 35 |
| I | GS015 | main.py | 41 |
| I | GS015 | main.py | 66 |
| I | GS015 | main.py | 71 |
| I | GS015 | main.py | 30 |
| I | GS015 | main.py | 35 |
| I | GS015 | main.py | 41 |
| I | GS015 | main.py | 66 |
| I | GS015 | main.py | 71 |
| I | GS015 | main.py | 27 |
| s | GS009 |  | 0 |
| H | GS019 | main.py | 31 |
| s | GS021 |  | 14 |
| r | GS022 |  | 117 |
| r | GS022 |  | 30 |

---
*Сгенерировано GSC v0.6 · 2026-08-10T07:07:32.025554*