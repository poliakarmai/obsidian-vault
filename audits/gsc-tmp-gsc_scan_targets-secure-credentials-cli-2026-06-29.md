---
title: "GSC Audit: /tmp/gsc_scan_targets/secure-credentials-cli"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/secure-credentials-cli

**Дата:** 29.06.2026 14:21  
**Путь:** `/tmp/gsc_scan_targets/secure-credentials-cli`  
**Всего находок:** 22  
**CRITICAL:** 1 | **HIGH:** 0 | **MEDIUM:** 0 | **LOW:** 20

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 16 |
| GS008 | 4 |
| GS001 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | main.py | 48 | Found: Password: ").strip()
    
    # Derive key from input |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | main.py | 48 |
| L | GS003 | main.py | 9 |
| L | GS003 | main.py | 15 |
| L | GS003 | main.py | 19 |
| L | GS003 | main.py | 33 |
| L | GS003 | main.py | 45 |
| L | GS003 | main.py | 58 |
| L | GS003 | main.py | 62 |
| L | GS003 | main.py | 73 |
| L | GS003 | main.py | 84 |
| L | GS003 | main.py | 94 |
| L | GS003 | main.py | 95 |
| L | GS003 | main.py | 96 |
| L | GS003 | main.py | 98 |
| L | GS003 | main.py | 100 |
| L | GS003 | main.py | 103 |
| L | GS003 | main.py | 106 |
| L | GS008 | config.py | 7 |
| L | GS008 | config.py | 10 |
| L | GS008 | config.py | 13 |
| L | GS008 | config.py | 16 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:21:55.836330*