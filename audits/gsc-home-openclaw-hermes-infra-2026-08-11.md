---
title: "GSC Audit: /home/openclaw/hermes-infra"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/hermes-infra

**Дата:** 11.08.2026 09:16  
**Путь:** `/home/openclaw/hermes-infra`  
**Всего находок:** 26  
**CRITICAL:** 2 | **HIGH:** 2 | **MEDIUM:** 14 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Синхронный код в async | 14 |
| GS032-fake_tool_call_execute | 3 |
| GS025 | 2 |
| GS020 | 1 |
| GS037-command_injection_os | 1 |
| GS000-LEGACY | 1 |
| GS004 | 1 |
| GS007 | 1 |
| GS009 | 1 |
| YAML-B39DC08C | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS025 | stars-payment-handler.py | 167 |  |
| CRITICAL | GS025 | bybit-db-backup.py | 100 |  |
| HIGH | GS000-LEGACY | bybit-db-backup.py | 100 | Match:         os.system(f'sqlite3 {DATA_DIR}/state.db .dump |
| HIGH | GS004 | bybit-db-backup.py | 100 | Line 100: os.system(f'sqlite3 {DATA_DIR}/state.db .dump > {s |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS025 | stars-payment-handler.py | 167 |
| C | GS025 | bybit-db-backup.py | 100 |
| i | GS020 |  | 124 |
| ? | GS032-fake_tool_call_execute | deprovision.py | 124 |
| ? | GS032-fake_tool_call_execute | stars-activator.py | 125 |
| ? | GS032-fake_tool_call_execute | stars-payment-handler.py | 167 |
| ? | GS037-command_injection_os | bybit-db-backup.py | 100 |
| H | GS000-LEGACY | bybit-db-backup.py | 100 |
| H | GS004 | bybit-db-backup.py | 100 |
| I | GS007 | stars-payment-handler.py | 123 |
| s | GS009 |  | 0 |
| ? | YAML-B39DC08C | hermes-tenant | ? |
| M | ? | stars-payment-handler.py | 84 |
| M | ? | deprovision.py | 47 |
| M | ? | hermes-tenant | 138 |
| M | ? | hermes-tenant | 163 |
| M | ? | hermes-tenant | 182 |
| M | ? | hermes-tenant | 197 |
| M | ? | hermes-tenant | 204 |
| M | ? | hermes-tenant | 358 |
| M | ? | hermes-tenant | 362 |
| M | ? | hermes-tenant | 424 |
| M | ? | hermes-tenant | 448 |
| M | ? | stars-activator.py | 61 |
| M | ? | ton-activator.py | 108 |
| M | ? | ton-activator.py | 126 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:16:13.615784*