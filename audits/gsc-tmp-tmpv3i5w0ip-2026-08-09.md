---
title: "GSC Audit: /tmp/tmpv3i5w0ip"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpv3i5w0ip

**Дата:** 09.08.2026 06:28  
**Путь:** `/tmp/tmpv3i5w0ip`  
**Всего находок:** 8  
**CRITICAL:** 2 | **HIGH:** 0 | **MEDIUM:** 2 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS029 | 2 |
| GS025-hardcoded_secret | 2 |
| GS025 | 1 |
| GS001 | 1 |
| GS037-hardcoded_password | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | test.py | 1 | Found: password = "my-super-secret-password" |
| CRITICAL | GS029 | test.py | 1 | Match: password = "my-super-secret-password" |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS025 | test.py | 1 |
| M | GS029 | test.py | 1 |
| C | GS001 | test.py | 1 |
| ? | GS037-hardcoded_password | test.py | 1 |
| C | GS029 | test.py | 1 |
| s | GS009 |  | 0 |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-09T06:28:21.288058*