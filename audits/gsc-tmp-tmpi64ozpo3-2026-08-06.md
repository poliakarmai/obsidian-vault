---
title: "GSC Audit: /tmp/tmpi64ozpo3"
date: 2026-08-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpi64ozpo3

**Дата:** 06.08.2026 09:42  
**Путь:** `/tmp/tmpi64ozpo3`  
**Всего находок:** 3  
**CRITICAL:** 1 | **HIGH:** 0 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| CVE-2026-55223: Insecure deserialization | 1 |
| pickle.load() — unsafe deserialization | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | test.py | 2 | Match: def load(x): return pickle.loads(x) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | test.py | 2 |
| C | ? | test.py | 2 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-06T09:42:07.162853*