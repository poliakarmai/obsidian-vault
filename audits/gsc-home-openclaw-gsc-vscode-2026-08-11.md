---
title: "GSC Audit: /home/openclaw/gsc-vscode"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc-vscode

**Дата:** 11.08.2026 09:17  
**Путь:** `/home/openclaw/gsc-vscode`  
**Всего находок:** 11  
**CRITICAL:** 0 | **HIGH:** 6 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 5 |
| GS020 | 2 |
| GS032-exfil_env_send | 2 |
| GS025 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
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
| i | GS020 |  | 43 |
| i | GS020 |  | 44 |
| ? | GS032-exfil_env_send | client.ts | 99 |
| ? | GS032-exfil_env_send | client.ts | 103 |
| H | GS025 | package-lock.json | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:17:14.396400*