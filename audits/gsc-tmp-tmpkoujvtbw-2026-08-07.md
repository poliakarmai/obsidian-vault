---
title: "GSC Audit: /tmp/tmpkoujvtbw"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpkoujvtbw

**Дата:** 07.08.2026 11:16  
**Путь:** `/tmp/tmpkoujvtbw`  
**Всего находок:** 7  
**CRITICAL:** 2 | **HIGH:** 0 | **MEDIUM:** 2 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025-hardcoded_secret | 2 |
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
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-07T11:16:02.774602*