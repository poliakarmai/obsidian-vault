---
title: "GSC Audit: /tmp/gsc-hunt-4"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-4

**Дата:** 11.08.2026 07:06  
**Путь:** `/tmp/gsc-hunt-4`  
**Всего находок:** 39  
**CRITICAL:** 0 | **HIGH:** 3 | **MEDIUM:** 23 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Синхронный код в async | 23 |
| GS032-fake_tool_call_execute | 9 |
| GS037-command_injection_os | 2 |
| GS004 | 2 |
| GS000-LEGACY | 1 |
| GS032-high_density | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS000-LEGACY | bot.py | 439 | File upload without MIME-type validation → malicious file up |
| HIGH | GS004 | bot.py | 395 | Line 395: out = os.popen(f"tasklist | findstr {context.args[ |
| HIGH | GS004 | bot.py | 402 | Line 402: out = os.popen(f"ps -A | grep {context.args[0]}"). |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS000-LEGACY | bot.py | 439 |
| ? | GS032-fake_tool_call_execute | bot.py | 147 |
| ? | GS032-fake_tool_call_execute | bot.py | 151 |
| ? | GS032-fake_tool_call_execute | bot.py | 181 |
| ? | GS032-fake_tool_call_execute | bot.py | 185 |
| ? | GS032-fake_tool_call_execute | bot.py | 215 |
| ? | GS032-fake_tool_call_execute | bot.py | 244 |
| ? | GS032-fake_tool_call_execute | bot.py | 248 |
| ? | GS032-fake_tool_call_execute | bot.py | 286 |
| ? | GS032-fake_tool_call_execute | bot.py | 288 |
| ? | GS032-high_density | bot.py | 1 |
| ? | GS037-command_injection_os | bot.py | 395 |
| ? | GS037-command_injection_os | bot.py | 402 |
| H | GS004 | bot.py | 395 |
| H | GS004 | bot.py | 402 |
| s | GS009 |  | 0 |
| M | ? | bot_setup.py | 78 |
| M | ? | bot_setup.py | 80 |
| M | ? | bot_setup.py | 83 |
| M | ? | bot_setup.py | 85 |
| M | ? | bot.py | 147 |
| M | ? | bot.py | 151 |
| M | ? | bot.py | 161 |
| M | ? | bot.py | 166 |
| M | ? | bot.py | 181 |
| M | ? | bot.py | 185 |
| M | ? | bot.py | 195 |
| M | ? | bot.py | 200 |
| M | ? | bot.py | 215 |
| M | ? | bot.py | 244 |
| M | ? | bot.py | 248 |
| M | ? | bot.py | 286 |
| M | ? | bot.py | 288 |
| M | ? | bot.py | 318 |
| M | ? | bot.py | 323 |
| M | ? | bot.py | 339 |
| M | ? | bot.py | 344 |
| M | ? | bot.py | 418 |
| M | ? | bot.py | 426 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T07:06:18.188687*