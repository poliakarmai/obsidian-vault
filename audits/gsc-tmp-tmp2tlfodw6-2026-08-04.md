---
title: "GSC Audit: /tmp/tmp2tlfodw6"
date: 2026-08-04
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmp2tlfodw6

**Дата:** 04.08.2026 22:28  
**Путь:** `/tmp/tmp2tlfodw6`  
**Всего находок:** 5  
**CRITICAL:** 2 | **HIGH:** 0 | **MEDIUM:** 2 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| CVE-2026-56318: Information disclosure | 1 |
| CVE-2026-37270: Hardcoded credential | 1 |
| GS001 | 1 |
| Hardcoded encryption key | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | test.py | 1 | Found: password = "my-super-secret-password" |
| CRITICAL | ? | test.py | 1 | Match: password = "my-super-secret-password" |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | test.py | 1 |
| M | ? | test.py | 1 |
| C | GS001 | test.py | 1 |
| C | ? | test.py | 1 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-04T22:28:41.326749*