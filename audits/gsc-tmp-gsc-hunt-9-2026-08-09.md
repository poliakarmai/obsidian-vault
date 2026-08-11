---
title: "GSC Audit: /tmp/gsc-hunt-9"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-9

**Дата:** 09.08.2026 09:55  
**Путь:** `/tmp/gsc-hunt-9`  
**Всего находок:** 25  
**CRITICAL:** 1 | **HIGH:** 1 | **MEDIUM:** 5 | **LOW:** 14

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 14 |
| Синхронный код в async | 4 |
| GS029 | 1 |
| GS001 | 1 |
| GS020 | 1 |
| GS037-hardcoded_password | 1 |
| GS009 | 1 |
| GS017 | 1 |
| YAML-B39DC08C | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | cli.py | 104 | Found: password: ")
        try:
            return hbk.Arch |
| HIGH | GS017 | cli.py | 176 | Password length = 4 chars. |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS029 | index.py | 68 |
| C | GS001 | cli.py | 104 |
| L | GS003 | mount.py | 87 |
| L | GS003 | mount.py | 91 |
| L | GS003 | mount.py | 92 |
| L | GS003 | mount.py | 98 |
| L | GS003 | mount.py | 107 |
| L | GS003 | mount.py | 109 |
| L | GS003 | mount.py | 110 |
| L | GS003 | mount.py | 113 |
| L | GS003 | mount.py | 151 |
| L | GS003 | mount.py | 158 |
| L | GS003 | mount.py | 161 |
| L | GS003 | mount.py | 169 |
| L | GS003 | mount.py | 173 |
| L | GS003 | mount.py | 175 |
| i | GS020 |  | 21 |
| ? | GS037-hardcoded_password | cli.py | 104 |
| s | GS009 |  | 0 |
| H | GS017 | cli.py | 176 |
| ? | YAML-B39DC08C | cli.py | ? |
| M | ? | mount.py | 55 |
| M | ? | mount.py | 65 |
| M | ? | mount.py | 96 |
| M | ? | mount.py | 172 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T09:55:13.007238*