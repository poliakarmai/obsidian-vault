---
title: "GSC Audit: /tmp/tmpipvyl_vi"
date: 2026-07-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpipvyl_vi

**Дата:** 29.07.2026 20:10  
**Путь:** `/tmp/tmpipvyl_vi`  
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
*Сгенерировано GSC v0.6 · 2026-07-29T20:10:43.982110*