---
title: "GSC Audit: gsc-vscode"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — gsc-vscode

**Дата:** 07.08.2026 14:48  
**Путь:** `/home/openclaw/gsc/gsc-vscode`  
**Всего находок:** 8  
**CRITICAL:** 1 | **HIGH:** 1 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS021 | 5 |
| GS001 | 1 |
| GS025 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | tsconfig.json | 4 | Found: "ES2022" |
| HIGH | GS025 | package-lock.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | tsconfig.json | 4 |
| H | GS025 | package-lock.json | 0 |
| s | GS009 |  | 0 |
| s | GS021 |  | 43 |
| s | GS021 |  | 45 |
| s | GS021 |  | 46 |
| s | GS021 |  | 47 |
| s | GS021 |  | 10 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T14:48:45.183965*