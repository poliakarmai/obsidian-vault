---
title: "GSC Audit: /tmp/gsc-external/myNetwork"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/myNetwork

**Дата:** 09.08.2026 06:32  
**Путь:** `/tmp/gsc-external/myNetwork`  
**Всего находок:** 47  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS020 | 16 |
| GS025-eval_usage | 11 |
| YAML-36ACF0AD | 11 |
| GS021 | 3 |
| GS025 | 2 |
| GS003 | 1 |
| GS009 | 1 |
| GS022 | 1 |
| Deep analysis requires OpenRouter API key | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | package-lock.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | package.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS025 | package-lock.json | 0 |
| H | GS025 | package.json | 0 |
| L | GS003 | audit-supply-chain.js | 139 |
| i | GS020 |  | 61 |
| i | GS020 |  | 318 |
| i | GS020 |  | 347 |
| i | GS020 |  | 397 |
| i | GS020 |  | 471 |
| i | GS020 |  | 500 |
| i | GS020 |  | 529 |
| i | GS020 |  | 535 |
| i | GS020 |  | 557 |
| i | GS020 |  | 581 |
| i | GS020 |  | 721 |
| i | GS020 |  | 62 |
| i | GS020 |  | 322 |
| i | GS020 |  | 348 |
| i | GS020 |  | 402 |
| i | GS020 |  | 699 |
| s | GS009 |  | 0 |
| s | GS021 |  | 6 |
| s | GS021 |  | 17 |
| s | GS021 |  | 82 |
| r | GS022 |  | 289 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | audit-supply-chain.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | discovery.js | ? |
| ? | YAML-36ACF0AD | net-utils.js | ? |
| I | ? |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T06:32:34.497518*