---
title: "GSC Audit: /home/openclaw/gsc/tests/test_corpus_gs005.py"
date: 2026-06-30
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc/tests/test_corpus_gs005.py

**Дата:** 30.06.2026 08:35  
**Путь:** `/home/openclaw/gsc/tests/test_corpus_gs005.py`  
**Всего находок:** 17  
**CRITICAL:** 16 | **HIGH:** 0 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| SQL injection risk: f-string in query | 12 |
| Python: raw string concatenation in SQL | 4 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | 8 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 12 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 15 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 19 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 20 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 23 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 28 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 31 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 37 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 39 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 43 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 46 | 0 | OWASP A03: Injection |
| CRITICAL | ? | 11 | 0 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | 16 | 0 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | 24 | 0 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | 25 | 0 | String concatenation with SQL — classic SQL injection vector |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | 8 | 0 |
| C | ? | 12 | 0 |
| C | ? | 15 | 0 |
| C | ? | 19 | 0 |
| C | ? | 20 | 0 |
| C | ? | 23 | 0 |
| C | ? | 28 | 0 |
| C | ? | 31 | 0 |
| C | ? | 37 | 0 |
| C | ? | 39 | 0 |
| C | ? | 43 | 0 |
| C | ? | 46 | 0 |
| C | ? | 11 | 0 |
| C | ? | 16 | 0 |
| C | ? | 24 | 0 |
| C | ? | 25 | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-30T08:35:48.008517*