---
title: "GSC Audit: /tmp/gsc-calibration/iac-demo"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/iac-demo

**Дата:** 07.08.2026 14:48  
**Путь:** `/tmp/gsc-calibration/iac-demo`  
**Всего находок:** 4  
**CRITICAL:** 1 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS031 | 1 |
| GS029 | 1 |
| GS025 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS031 | Dockerfile | 1 | Match: FROM node:latest |
| HIGH | GS029 | Dockerfile | 3 | Match: ENV SECRET=x |
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS031 | Dockerfile | 1 |
| H | GS029 | Dockerfile | 3 |
| H | GS025 | expected.json | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T14:48:41.604095*