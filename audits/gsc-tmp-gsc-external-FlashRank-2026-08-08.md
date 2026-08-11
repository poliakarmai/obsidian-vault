---
title: "GSC Audit: /tmp/gsc-external/FlashRank"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/FlashRank

**Дата:** 08.08.2026 19:16  
**Путь:** `/tmp/gsc-external/FlashRank`  
**Всего находок:** 2  
**CRITICAL:** 0 | **HIGH:** 1 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS000-LEGACY | Ranker.py | 95 | User-controlled URL in HTTP request → SSRF. From BugHunter h |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS000-LEGACY | Ranker.py | 95 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T19:16:59.186988*