---
title: "GSC Audit: /tmp/gsc_scan_targets/blueprint-api"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/blueprint-api

**Дата:** 29.06.2026 14:21  
**Путь:** `/tmp/gsc_scan_targets/blueprint-api`  
**Всего находок:** 15  
**CRITICAL:** 0 | **HIGH:** 1 | **MEDIUM:** 1 | **LOW:** 12

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 12 |
| Python: File upload without content-type validation | 1 |
| GS009 | 1 |
| GS012 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | views.py | 29 | File upload without MIME-type validation → malicious file up |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | views.py | 29 |
| L | GS008 | settings.py | 32 |
| L | GS008 | settings.py | 37 |
| L | GS008 | settings.py | 59 |
| L | GS008 | settings.py | 65 |
| L | GS008 | settings.py | 77 |
| L | GS008 | settings.py | 92 |
| L | GS008 | settings.py | 98 |
| L | GS008 | settings.py | 128 |
| L | GS008 | settings.py | 130 |
| L | GS008 | settings.py | 132 |
| L | GS008 | settings.py | 134 |
| L | GS008 | settings.py | 142 |
| s | GS009 |  | 0 |
| M | GS012 | views.py | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:21:50.329807*