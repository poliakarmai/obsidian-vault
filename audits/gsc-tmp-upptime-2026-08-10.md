---
title: "GSC Audit: /tmp/upptime"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/upptime

**Дата:** 10.08.2026 14:22  
**Путь:** `/tmp/upptime`  
**Всего находок:** 3  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025 | 2 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | .templaterc.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .upptimerc.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS025 | .templaterc.json | 0 |
| H | GS025 | .upptimerc.yml | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-10T14:22:45.311797*