---
title: "GSC Audit: /tmp/gsc-calibration/assert-demo"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/assert-demo

**Дата:** 08.08.2026 04:05  
**Путь:** `/tmp/gsc-calibration/assert-demo`  
**Всего находок:** 5  
**CRITICAL:** 1 | **HIGH:** 1 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS018 | 1 |
| GS001 | 1 |
| GS015 | 1 |
| GS025 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | expected.json | 1 | Found: "GS018" |
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS018 | app.py | 2 |
| C | GS001 | expected.json | 1 |
| I | GS015 | app.py | 1 |
| H | GS025 | expected.json | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:05:04.393792*