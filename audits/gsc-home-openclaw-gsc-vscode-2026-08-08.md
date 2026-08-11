---
title: "GSC Audit: /home/openclaw/gsc-vscode"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc-vscode

**Дата:** 08.08.2026 04:08  
**Путь:** `/home/openclaw/gsc-vscode`  
**Всего находок:** 11  
**CRITICAL:** 2 | **HIGH:** 6 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 5 |
| GS001 | 2 |
| GS020 | 2 |
| GS025 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | tsconfig.json | 4 | Found: "ES2022" |
| CRITICAL | GS001 | tsconfig.json | 7 | Found: "ES2022" |
| HIGH | GS000-LEGACY | client.ts | 84 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | suite.test.ts | 40 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | suite.test.ts | 44 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | extension.ts | 122 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | extension.ts | 124 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS025 | package-lock.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS000-LEGACY | client.ts | 84 |
| H | GS000-LEGACY | suite.test.ts | 40 |
| H | GS000-LEGACY | suite.test.ts | 44 |
| H | GS000-LEGACY | extension.ts | 122 |
| H | GS000-LEGACY | extension.ts | 124 |
| C | GS001 | tsconfig.json | 4 |
| C | GS001 | tsconfig.json | 7 |
| i | GS020 |  | 43 |
| i | GS020 |  | 44 |
| H | GS025 | package-lock.json | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:08:47.305672*