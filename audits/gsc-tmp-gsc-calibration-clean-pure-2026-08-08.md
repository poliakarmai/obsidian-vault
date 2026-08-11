---
title: "GSC Audit: /tmp/gsc-calibration/clean-pure"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/clean-pure

**Дата:** 08.08.2026 04:05  
**Путь:** `/tmp/gsc-calibration/clean-pure`  
**Всего находок:** 3  
**CRITICAL:** 0 | **HIGH:** 1 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 1 |
| GS025 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| I | GS015 | app.py | 1 |
| H | GS025 | expected.json | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:05:09.222042*