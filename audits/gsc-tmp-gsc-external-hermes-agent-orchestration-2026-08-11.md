---
title: "GSC Audit: /tmp/gsc-external/hermes-agent-orchestration"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/hermes-agent-orchestration

**Дата:** 11.08.2026 09:15  
**Путь:** `/tmp/gsc-external/hermes-agent-orchestration`  
**Всего находок:** 33  
**CRITICAL:** 2 | **HIGH:** 2 | **MEDIUM:** 16 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Синхронный код в async | 15 |
| GS008 | 3 |
| GS007 | 3 |
| GS005 | 2 |
| GS032-fake_tool_call_execute | 2 |
| GS025-eval_usage | 2 |
| YAML-36ACF0AD | 2 |
| YAML-B39DC08C | 2 |
| GS029 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | tenant-audit.py | 63 | OWASP A03: Injection |
| CRITICAL | GS005 | tenant-audit.py | 63 |  |
| HIGH | GS008 | skill-validate.py | 86 | Match:         (r'\beval\s*\(', "eval() call detected"), |
| HIGH | GS008 | skill-validate.py | 87 | Match:         (r'\bexec\s*\(', "exec() call detected"), |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | tenant-audit.py | 63 |
| C | GS005 | tenant-audit.py | 63 |
| M | GS029 | skill-sync.py | 220 |
| L | GS008 | metrics-collector.py | 20 |
| ? | GS032-fake_tool_call_execute | deprovision.py | 126 |
| ? | GS032-fake_tool_call_execute | stars-activator.py | 127 |
| H | GS008 | skill-validate.py | 86 |
| H | GS008 | skill-validate.py | 87 |
| I | GS007 | miropolbot.py | 35 |
| I | GS007 | audit-log-parser.py | 67 |
| I | GS007 | tenant-audit.py | 26 |
| s | GS009 |  | 0 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | skill-validate.py | ? |
| ? | YAML-36ACF0AD | skill-validate.py | ? |
| ? | YAML-B39DC08C | deepseek-balance-monitor.py | ? |
| ? | YAML-B39DC08C | hermes-tenant | ? |
| M | ? | skill-sync.py | 67 |
| M | ? | skill-sync.py | 149 |
| M | ? | skill-sync.py | 172 |
| M | ? | skill-sync.py | 200 |
| M | ? | deprovision.py | 49 |
| M | ? | hermes-tenant | 130 |
| M | ? | hermes-tenant | 155 |
| M | ? | hermes-tenant | 174 |
| M | ? | hermes-tenant | 189 |
| M | ? | hermes-tenant | 196 |
| M | ? | hermes-tenant | 350 |
| M | ? | hermes-tenant | 354 |
| M | ? | hermes-tenant | 408 |
| M | ? | hermes-tenant | 432 |
| M | ? | stars-activator.py | 63 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:15:48.089108*