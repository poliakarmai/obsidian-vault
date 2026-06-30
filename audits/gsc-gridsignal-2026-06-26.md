---
title: "GSC Audit: gridsignal"
date: 2026-06-26
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — gridsignal

**Дата:** 26.06.2026 08:42  
**Путь:** `/home/openclaw/.local/bin`  
**Всего находок:** 82  
**CRITICAL:** 3 | **HIGH:** 10 | **MEDIUM:** 69 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Синхронный код в async | 65 |
| Хардкод IP адреса | 10 |
| Bare except: | 4 |
| Hardcoded encryption key | 2 |
| SQL injection risk: f-string in query | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | loop-journal | 258 | OWASP A03: Injection |
| CRITICAL | ? | gridsignal-bot.py.bak.20260619_1722 | 30 | Match:         row = db.execute("SELECT value FROM kv_store  |
| CRITICAL | ? | gridsignal-bot.py.bak.20260619_1722 | 838 | Match:     header_key = 'scan_header_short' if mode == 'shor |
| HIGH | ? | meili-mcp.py | 7 | Match: MEILI_URL = "http://127.0.0.1:7700" |
| HIGH | ? | hermes-tenant.bak | 157 | Match:          "-d", "127.0.0.0/8", "-j", "DROP"], |
| HIGH | ? | hermes-tenant.bak | 168 | Match:         print(f"   👉 Ручками: sudo iptables -A OUTPUT |
| HIGH | ? | hermes-tenant.bak | 176 | Match:          "-d", "127.0.0.0/8", "-j", "DROP"], |
| HIGH | ? | hermes-tenant | 157 | Match:          "-d", "127.0.0.0/8", "-j", "DROP"], |
| HIGH | ? | hermes-tenant | 168 | Match:         print(f"   👉 Ручками: sudo iptables -A OUTPUT |
| HIGH | ? | hermes-tenant | 176 | Match:          "-d", "127.0.0.0/8", "-j", "DROP"], |
| HIGH | ? | hermes-mcp-server.py | 28 | Match: RPC_BASE = f"http://127.0.0.1:{RPC_PORT}" |
| HIGH | ? | search-web.py | 8 | Match: OPENSERP_URL = os.environ.get("OPENSERP_URL", "http:/ |
| HIGH | ? | bybit-mcp-server.py | 28 | Match: RPC_BASE = f"http://127.0.0.1:{RPC_PORT}" |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | loop-journal | 258 |
| M | ? | reconcile-hook | 25 |
| M | ? | newswatch | 19 |
| M | ? | newswatch | 84 |
| M | ? | newswatch | 127 |
| H | ? | meili-mcp.py | 7 |
| H | ? | hermes-tenant.bak | 157 |
| H | ? | hermes-tenant.bak | 168 |
| H | ? | hermes-tenant.bak | 176 |
| H | ? | hermes-tenant | 157 |
| H | ? | hermes-tenant | 168 |
| H | ? | hermes-tenant | 176 |
| H | ? | hermes-mcp-server.py | 28 |
| H | ? | search-web.py | 8 |
| H | ? | bybit-mcp-server.py | 28 |
| C | ? | gridsignal-bot.py.bak.20260619_1722 | 30 |
| C | ? | gridsignal-bot.py.bak.20260619_1722 | 838 |
| M | ? | bybit-grid-m5 | 23 |
| M | ? | bybit-grid-m5 | 54 |
| M | ? | paper-trade | 183 |
| M | ? | hermes-tenant.bak | 138 |
| M | ? | hermes-tenant.bak | 163 |
| M | ? | hermes-tenant.bak | 182 |
| M | ? | hermes-tenant.bak | 198 |
| M | ? | hermes-tenant.bak | 205 |
| M | ? | hermes-tenant.bak | 209 |
| M | ? | hermes-tenant.bak | 365 |
| M | ? | hermes-tenant.bak | 369 |
| M | ? | hermes-tenant.bak | 431 |
| M | ? | hermes-tenant.bak | 455 |
| M | ? | hermes-tenant.bak | 530 |
| M | ? | hermes-tenant.bak | 547 |
| M | ? | hermes-tenant.bak | 665 |
| M | ? | hermes-tenant.bak | 676 |
| M | ? | hermes-tenant.bak | 702 |
| M | ? | bybit-smoke | 11 |
| M | ? | hermes-tenant | 138 |
| M | ? | hermes-tenant | 163 |
| M | ? | hermes-tenant | 182 |
| M | ? | hermes-tenant | 198 |
| M | ? | hermes-tenant | 205 |
| M | ? | hermes-tenant | 209 |
| M | ? | hermes-tenant | 365 |
| M | ? | hermes-tenant | 369 |
| M | ? | hermes-tenant | 431 |
| M | ? | hermes-tenant | 455 |
| M | ? | hermes-tenant | 530 |
| M | ? | hermes-tenant | 547 |
| M | ? | hermes-tenant | 665 |
| M | ? | hermes-tenant | 676 |
| M | ? | hermes-tenant | 702 |
| M | ? | hermes-mcp-server.py | 55 |
| M | ? | hermes-mcp-server.py | 70 |
| M | ? | hermes-white-label | 50 |
| M | ? | hermes-white-label | 136 |
| M | ? | hermes-white-label | 137 |
| M | ? | hermes-white-label | 143 |
| M | ? | gridsignal_scanner.py | 49 |
| M | ? | bybit-mcp-server.py | 55 |
| M | ? | bybit-mcp-server.py | 70 |
| M | ? | bybit-mcp-server.py | 88 |
| M | ? | backtest | 21 |
| M | ? | bybit-scan | 48 |
| M | ? | gridsignal-bot.py | 1342 |
| M | ? | gridsignal-bot.py | 1344 |
| M | ? | gridsignal-bot.py | 1443 |
| M | ? | gridsignal-bot.py | 1445 |
| M | ? | gridsignal-bot.py | 1531 |
| M | ? | gridsignal-bot.py | 2096 |
| M | ? | bybit-deploy | 14 |
| M | ? | hermes-onboard | 19 |
| M | ? | gridsignal-bot.py.bak.20260619_1722 | 1181 |
| M | ? | gridsignal-bot.py.bak.20260619_1722 | 1183 |
| M | ? | gridsignal-bot.py.bak.20260619_1722 | 1282 |
| M | ? | gridsignal-bot.py.bak.20260619_1722 | 1284 |
| M | ? | gridsignal-bot.py.bak.20260619_1722 | 1361 |
| M | ? | gridsignal-bot.py.bak.20260619_1722 | 1921 |
| M | ? | bybit-grid-m3 | 35 |
| M | ? | bybit-grid-m3 | 65 |
| M | ? | bybit-execute-deploy | 14 |
| M | ? | newswatch | 95 |
| M | ? | hermes-admin | 21 |

---
*Сгенерировано GSC v0.6 · 2026-06-26T08:42:33.292298*