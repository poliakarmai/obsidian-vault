---
title: "GSC Audit: /tmp/gsc-external/openwiki"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/openwiki

**Дата:** 11.08.2026 09:18  
**Путь:** `/tmp/gsc-external/openwiki`  
**Всего находок:** 31  
**CRITICAL:** 0 | **HIGH:** 5 | **MEDIUM:** 0 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS034-token_collector | 16 |
| GS022 | 7 |
| GS025 | 3 |
| GS032-system_prompt_override | 1 |
| GS002 | 1 |
| GS009 | 1 |
| GS014 | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | package.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | pnpm-lock.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | tsconfig.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | credentials.tsx | 0 | File credentials.tsx has permissions -rw-rw-r-- — readable b |
| HIGH | ? | index.ts | 1210 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| ? | GS032-system_prompt_override | prompt.ts | 16 |
| ? | GS034-token_collector | index.ts | 354 |
| ? | GS034-token_collector | index.ts | 367 |
| ? | GS034-token_collector | index.ts | 383 |
| ? | GS034-token_collector | index.ts | 391 |
| ? | GS034-token_collector | index.ts | 403 |
| ? | GS034-token_collector | index.ts | 1274 |
| ? | GS034-token_collector | commands.ts | 168 |
| ? | GS034-token_collector | constants.ts | 148 |
| ? | GS034-token_collector | env.ts | 24 |
| ? | GS034-token_collector | env.ts | 26 |
| ? | GS034-token_collector | env.ts | 60 |
| ? | GS034-token_collector | env.ts | 61 |
| ? | GS034-token_collector | env.ts | 109 |
| ? | GS034-token_collector | env.ts | 117 |
| ? | GS034-token_collector | env.ts | 154 |
| ? | GS034-token_collector | env.ts | 158 |
| H | GS025 | package.json | 0 |
| H | GS025 | pnpm-lock.yaml | 0 |
| H | GS025 | tsconfig.json | 0 |
| H | GS002 | credentials.tsx | 0 |
| s | GS009 |  | 0 |
| L | GS014 | credentials.tsx | 1 |
| r | GS022 |  | 1094 |
| r | GS022 |  | 1103 |
| r | GS022 |  | 1135 |
| r | GS022 |  | 1135 |
| r | GS022 |  | 1244 |
| r | GS022 |  | 1246 |
| r | GS022 |  | 1306 |
| H | ? | index.ts | 1210 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:18:42.884731*