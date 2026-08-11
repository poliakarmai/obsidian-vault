---
title: "GSC Audit: /tmp/gsc-calibration-real/clean-django-view"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration-real/clean-django-view

**Дата:** 07.08.2026 14:57  
**Путь:** `/tmp/gsc-calibration-real/clean-django-view`  
**Всего находок:** 2  
**CRITICAL:** 0 | **HIGH:** 1 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS025 | expected.json | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T14:57:23.814110*