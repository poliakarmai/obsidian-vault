---
title: "GSC Audit: /tmp/tmp17ll_sig"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmp17ll_sig

**Дата:** 07.08.2026 12:18  
**Путь:** `/tmp/tmp17ll_sig`  
**Всего находок:** 3  
**CRITICAL:** 2 | **HIGH:** 0 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| SQL injection risk: f-string in query | 1 |
| CVE-2026-55721: SQL injection | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | test.py | 1 | OWASP A03: Injection |
| CRITICAL | ? | test.py | 1 |  |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | test.py | 1 |
| C | ? | test.py | 1 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T12:18:13.878057*