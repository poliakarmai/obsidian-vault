---
title: "GSC Audit: /tmp/tmp1heyelm3"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmp1heyelm3

**Дата:** 05.08.2026 12:23  
**Путь:** `/tmp/tmp1heyelm3`  
**Всего находок:** 4  
**CRITICAL:** 2 | **HIGH:** 0 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| CVE-2026-55223: Insecure deserialization | 1 |
| pickle.load() — unsafe deserialization | 1 |
| GS009 | 1 |
| GS025-unsafe_pickle | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | test.py | 2 | Match: def load(x): return pickle.loads(x) |
| CRITICAL | GS025-unsafe_pickle | test.py | 2 | def load(x): return pickle.loads(x) | ai_provenance: 0% |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | test.py | 2 |
| C | ? | test.py | 2 |
| s | GS009 |  | 0 |
| C | GS025-unsafe_pickle | test.py | 2 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T12:23:54.191776*