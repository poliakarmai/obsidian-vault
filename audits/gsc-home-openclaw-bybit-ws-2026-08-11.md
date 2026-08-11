---
title: "GSC Audit: /home/openclaw/bybit-ws"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/bybit-ws

**Дата:** 11.08.2026 09:04  
**Путь:** `/home/openclaw/bybit-ws`  
**Всего находок:** 1085  
**CRITICAL:** 2 | **HIGH:** 117 | **MEDIUM:** 34 | **LOW:** 126

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 584 |
| GS003 | 102 |
| GS020 | 91 |
| GS018 | 77 |
| GS021 | 63 |
| GS007 | 42 |
| YAML-B39DC08C | 18 |
| Синхронный код в async | 14 |
| GS008 | 13 |
| GS000-LEGACY | 12 |
| GS025-eval_usage | 11 |
| YAML-36ACF0AD | 10 |
| GS029 | 9 |
| GS025 | 8 |
| GS037-hardcoded_password | 6 |
| GS011 | 4 |
| GS005 | 2 |
| GS015 | 2 |
| Systemd: RestrictSUIDSGID= not set | 2 |
| GS012 | 2 |
| GS025-permissive_cors | 2 |
| Systemd: NoNewPrivileges= not set | 1 |
| Systemd: ProtectSystem= not set | 1 |
| Systemd: ProtectHome= not set | 1 |
| Systemd: PrivateTmp= not set | 1 |
| Systemd: ProtectProc= not set | 1 |
| Systemd: MemoryDenyWriteExecute= not set | 1 |
| Systemd: RestrictRealtime= not set | 1 |
| Systemd: RemoveIPC= not set | 1 |
| Systemd: LockPersonality= not set | 1 |
| GS009 | 1 |
| GS017 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | dspy_optimizer.py | 84 | OWASP A03: Injection |
| CRITICAL | GS005 | dspy_optimizer.py | 84 |  |
| HIGH | GS000-LEGACY | bybit_ws_sdk.py | 38 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | bybit_ws_sdk.py | 43 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | lstm_regime.py | 531 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | rl_agent.py | 139 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | lstm_world_model.py | 417 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | lstm_world_model.py | 439 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | dspy_optimizer.py | 405 | File upload without MIME-type validation → malicious file up |
| HIGH | GS025 | bybit_ws_sdk.py | 38 |  |
| HIGH | GS025 | bybit_ws_sdk.py | 43 |  |
| HIGH | GS000-LEGACY | bybit_ws_sdk.py | 38 | Match:         r = requests.get(f"{self.base_url}{path}", ti |
| HIGH | GS000-LEGACY | bybit_ws_sdk.py | 43 | Match:         r = requests.post(f"{self.base_url}{path}", j |
| HIGH | GS008 | lstm_regime.py | 512 | Match:         model.eval() |
| HIGH | GS008 | lstm_regime.py | 605 | Match:         model.eval() |
| HIGH | GS008 | lstm_world_model.py | 402 | Match:         model.eval() |
| HIGH | GS008 | lstm_world_model.py | 467 | Match:     model.eval() |
| HIGH | GS008 | lstm_world_model.py | 565 | Match:     model.eval() |
| HIGH | GS025 | state.db | 0 | Permissions 644 — should be 600 |
| HIGH | GS025 | openapi.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | config.example.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .mcp.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | bybit-ws.service | 0 | NoNewPrivileges= not set |
| HIGH | GS007 | gridsignal-bot.py | 148 | Line 148: "SELECT 1 FROM pro_users WHERE user_id=? AND activ |
| HIGH | GS007 | gridsignal-bot.py | 249 | Line 249: row = conn.execute('SELECT user_id, username, firs |
| HIGH | GS007 | gridsignal-bot.py | 390 | Line 390: row = conn.execute('SELECT lang FROM users WHERE u |
| HIGH | GS007 | gridsignal-bot.py | 1064 | Line 1064: "SELECT paid_at, expires_at, active FROM pro_user |
| HIGH | GS007 | gridsignal-bot.py | 1097 | Line 1097: "SELECT 1 FROM pro_users WHERE user_id=? AND char |
| HIGH | GS007 | gridsignal-bot.py | 1260 | Line 1260: 'SELECT outcome, pnl_pct FROM signals WHERE user_ |
| HIGH | GS007 | gridsignal-bot.py | 1294 | Line 1294: alerts = conn.execute('SELECT symbol FROM alerts  |
| HIGH | GS007 | gridsignal-bot.py | 1325 | Line 1325: alert_count = conn.execute('SELECT COUNT(*) FROM  |
| HIGH | GS007 | gridsignal-bot.py | 148 | Line 148: "SELECT 1 FROM pro_users WHERE user_id=? AND activ |
| HIGH | GS007 | gridsignal-bot.py | 249 | Line 249: row = conn.execute('SELECT user_id, username, firs |
| HIGH | GS007 | gridsignal-bot.py | 390 | Line 390: row = conn.execute('SELECT lang FROM users WHERE u |
| HIGH | GS007 | gridsignal-bot.py | 1064 | Line 1064: "SELECT paid_at, expires_at, active FROM pro_user |
| HIGH | GS007 | gridsignal-bot.py | 1097 | Line 1097: "SELECT 1 FROM pro_users WHERE user_id=? AND char |
| HIGH | GS007 | gridsignal-bot.py | 1260 | Line 1260: 'SELECT outcome, pnl_pct FROM signals WHERE user_ |
| HIGH | GS007 | gridsignal-bot.py | 1294 | Line 1294: alerts = conn.execute('SELECT symbol FROM alerts  |
| HIGH | GS007 | gridsignal-bot.py | 1325 | Line 1325: alert_count = conn.execute('SELECT COUNT(*) FROM  |
| HIGH | GS011 | rpc.py | 180 | Detected: key='started_at' |
| HIGH | GS011 | rpc.py | 180 | Detected: key='started_at' |
| HIGH | GS017 | config.example.yaml | 33 | Password variable with short value (19 chars). |
| HIGH | GS018 | api.py | 401 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | api.py | 301 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_entry.py | 626 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 392 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 512 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 771 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | api.py | 401 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | api.py | 301 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_entry.py | 626 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 392 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 512 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 771 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | dca.py | 172 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 48 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 127 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 257 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 393 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 579 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 589 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 626 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 663 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 965 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 1448 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 1726 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | self_learn.py | 163 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | self_learn.py | 163 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ml_scorer.py | 77 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_api.py | 287 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | paper_trade.py | 45 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 96 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 109 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 122 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 149 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 273 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 291 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | position_sizing.py | 56 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | position_sizing.py | 247 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | position_sizing.py | 333 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 406 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 420 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 950 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 1574 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 1786 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ws_client.py | 300 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ws_client.py | 302 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | dca.py | 172 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 48 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 127 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 257 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | exchange_adapter.py | 393 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 579 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 589 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 626 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 663 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 965 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 1448 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 1726 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ml_scorer.py | 77 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_api.py | 287 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | paper_trade.py | 45 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 96 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 109 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 122 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 149 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 273 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | paper_trade.py | 291 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | position_sizing.py | 56 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | position_sizing.py | 247 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | position_sizing.py | 333 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 406 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 420 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 950 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 1574 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 1786 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ws_client.py | 300 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ws_client.py | 302 | Float arithmetic for money leads to rounding errors exploita |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | dspy_optimizer.py | 84 |
| M | GS018 | optuna_tuner.py | 436 |
| H | GS000-LEGACY | bybit_ws_sdk.py | 38 |
| H | GS000-LEGACY | bybit_ws_sdk.py | 43 |
| H | GS000-LEGACY | lstm_regime.py | 531 |
| H | GS000-LEGACY | rl_agent.py | 139 |
| H | GS000-LEGACY | lstm_world_model.py | 417 |
| H | GS000-LEGACY | lstm_world_model.py | 439 |
| H | GS000-LEGACY | dspy_optimizer.py | 405 |
| M | GS000-LEGACY | rpc.py | 59 |
| M | GS007 | lstm_regime.py | 624 |
| M | GS007 | lstm_world_model.py | 292 |
| M | GS007 | lstm_world_model.py | 479 |
| M | GS007 | lstm_world_model.py | 571 |
| C | GS005 | dspy_optimizer.py | 84 |
| H | GS025 | bybit_ws_sdk.py | 38 |
| H | GS025 | bybit_ws_sdk.py | 43 |
| M | GS025 | gridsignal-bot.py | 1136 |
| M | GS029 | margin_alerts.py | 138 |
| M | GS029 | margin_alerts.py | 148 |
| M | GS029 | margin_alerts.py | 157 |
| M | GS029 | gridsignal-bot.py | 30 |
| M | GS029 | gridsignal-bot.py | 931 |
| M | GS029 | gridsignal-bot.py | 1136 |
| M | GS029 | proxy_server.py | 25 |
| M | GS029 | mcp_server.py | 39 |
| M | GS029 | rpc.py | 180 |
| L | GS003 | alerts.py | 57 |
| L | GS003 | alerts.py | 63 |
| L | GS003 | alerts.py | 64 |
| L | GS003 | alerts.py | 57 |
| L | GS003 | alerts.py | 63 |
| L | GS003 | alerts.py | 64 |
| L | GS003 | main.py | 188 |
| L | GS003 | main.py | 476 |
| L | GS003 | main.py | 478 |
| L | GS003 | main.py | 479 |
| L | GS003 | main.py | 480 |
| L | GS003 | main.py | 481 |
| L | GS003 | main.py | 962 |
| L | GS003 | main.py | 963 |
| L | GS003 | main.py | 965 |
| L | GS003 | main.py | 966 |
| L | GS003 | main.py | 971 |
| L | GS003 | main.py | 997 |
| L | GS003 | main.py | 1061 |
| L | GS003 | main.py | 1069 |
| L | GS003 | main.py | 1076 |
| L | GS003 | main.py | 1082 |
| L | GS003 | main.py | 1092 |
| L | GS003 | main.py | 1113 |
| L | GS003 | main.py | 1115 |
| L | GS003 | main.py | 1129 |
| L | GS003 | main.py | 1131 |
| L | GS003 | main.py | 1133 |
| L | GS003 | metrics.py | 96 |
| L | GS003 | metrics.py | 97 |
| L | GS003 | metrics.py | 98 |
| L | GS003 | metrics.py | 99 |
| L | GS003 | metrics.py | 105 |
| L | GS003 | metrics.py | 107 |
| L | GS003 | metrics.py | 109 |
| L | GS003 | metrics.py | 110 |
| L | GS003 | metrics.py | 113 |
| L | GS003 | push_notifier.py | 188 |
| L | GS003 | push_notifier.py | 194 |
| L | GS003 | push_notifier.py | 197 |
| L | GS003 | push_notifier.py | 200 |
| L | GS003 | push_notifier.py | 292 |
| L | GS003 | push_notifier.py | 295 |
| L | GS003 | walk_forward_validate.py | 20 |
| L | GS003 | walk_forward_validate.py | 28 |
| L | GS003 | walk_forward_validate.py | 32 |
| L | GS003 | walk_forward_validate.py | 57 |
| L | GS003 | walk_forward_validate.py | 58 |
| L | GS003 | walk_forward_validate.py | 60 |
| L | GS003 | walk_forward_validate.py | 61 |
| L | GS003 | walk_forward_validate.py | 69 |
| L | GS003 | walk_forward_validate.py | 72 |
| L | GS003 | walk_forward_validate.py | 74 |
| L | GS003 | walk_forward_validate.py | 76 |
| L | GS003 | main.py | 188 |
| L | GS003 | main.py | 476 |
| L | GS003 | main.py | 478 |
| L | GS003 | main.py | 479 |
| L | GS003 | main.py | 480 |
| L | GS003 | main.py | 481 |
| L | GS003 | main.py | 962 |
| L | GS003 | main.py | 963 |
| L | GS003 | main.py | 965 |
| L | GS003 | main.py | 966 |
| L | GS003 | main.py | 971 |
| L | GS003 | main.py | 997 |
| L | GS003 | main.py | 1061 |
| L | GS003 | main.py | 1069 |
| L | GS003 | main.py | 1076 |
| L | GS003 | main.py | 1082 |
| L | GS003 | main.py | 1092 |
| L | GS003 | main.py | 1113 |
| L | GS003 | main.py | 1115 |
| L | GS003 | main.py | 1129 |
| L | GS003 | main.py | 1131 |
| L | GS003 | main.py | 1133 |
| L | GS003 | metrics.py | 96 |
| L | GS003 | metrics.py | 97 |
| L | GS003 | metrics.py | 98 |
| L | GS003 | metrics.py | 99 |
| L | GS003 | metrics.py | 105 |
| L | GS003 | metrics.py | 107 |
| L | GS003 | metrics.py | 109 |
| L | GS003 | metrics.py | 110 |
| L | GS003 | metrics.py | 113 |
| L | GS003 | push_notifier.py | 188 |
| L | GS003 | push_notifier.py | 194 |
| L | GS003 | push_notifier.py | 197 |
| L | GS003 | push_notifier.py | 200 |
| L | GS003 | push_notifier.py | 292 |
| L | GS003 | push_notifier.py | 295 |
| L | GS003 | walk_forward_validate.py | 20 |
| L | GS003 | walk_forward_validate.py | 28 |
| L | GS003 | walk_forward_validate.py | 32 |
| L | GS003 | walk_forward_validate.py | 57 |
| L | GS003 | walk_forward_validate.py | 58 |
| L | GS003 | walk_forward_validate.py | 60 |
| L | GS003 | walk_forward_validate.py | 61 |
| L | GS003 | walk_forward_validate.py | 69 |
| L | GS003 | walk_forward_validate.py | 72 |
| L | GS003 | walk_forward_validate.py | 74 |
| L | GS003 | walk_forward_validate.py | 76 |
| L | GS008 | optimize_params.py | 24 |
| L | GS008 | optimize_params.py | 28 |
| L | GS008 | paper_trade.py | 34 |
| L | GS008 | rl_env.py | 40 |
| L | GS008 | optimize_params.py | 24 |
| L | GS008 | optimize_params.py | 28 |
| L | GS008 | paper_trade.py | 34 |
| L | GS008 | rl_env.py | 40 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| i | GS020 |  | 194 |
| i | GS020 |  | 263 |
| i | GS020 |  | 307 |
| i | GS020 |  | 324 |
| i | GS020 |  | 337 |
| i | GS020 |  | 188 |
| i | GS020 |  | 330 |
| i | GS020 |  | 135 |
| i | GS020 |  | 184 |
| i | GS020 |  | 192 |
| i | GS020 |  | 267 |
| i | GS020 |  | 141 |
| i | GS020 |  | 1579 |
| i | GS020 |  | 1579 |
| i | GS020 |  | 1753 |
| i | GS020 |  | 22 |
| i | GS020 |  | 23 |
| i | GS020 |  | 181 |
| i | GS020 |  | 752 |
| i | GS020 |  | 527 |
| i | GS020 |  | 1069 |
| i | GS020 |  | 1077 |
| i | GS020 |  | 1077 |
| i | GS020 |  | 1113 |
| i | GS020 |  | 15 |
| i | GS020 |  | 68 |
| i | GS020 |  | 1442 |
| i | GS020 |  | 1448 |
| i | GS020 |  | 1449 |
| i | GS020 |  | 1451 |
| i | GS020 |  | 1464 |
| i | GS020 |  | 1465 |
| i | GS020 |  | 1468 |
| i | GS020 |  | 1 |
| i | GS020 |  | 100 |
| i | GS020 |  | 5834 |
| i | GS020 |  | 5837 |
| i | GS020 |  | 93 |
| i | GS020 |  | 122 |
| i | GS020 |  | 670 |
| i | GS020 |  | 116 |
| i | GS020 |  | 21 |
| i | GS020 |  | 15 |
| i | GS020 |  | 22 |
| i | GS020 |  | 23 |
| i | GS020 |  | 175 |
| i | GS020 |  | 711 |
| i | GS020 |  | 507 |
| i | GS020 |  | 1014 |
| i | GS020 |  | 1022 |
| i | GS020 |  | 1022 |
| i | GS020 |  | 1058 |
| i | GS020 |  | 15 |
| i | GS020 |  | 68 |
| i | GS020 |  | 1429 |
| i | GS020 |  | 1435 |
| i | GS020 |  | 1436 |
| i | GS020 |  | 1438 |
| i | GS020 |  | 1449 |
| i | GS020 |  | 1450 |
| i | GS020 |  | 1453 |
| i | GS020 |  | 1 |
| i | GS020 |  | 719 |
| i | GS020 |  | 601 |
| i | GS020 |  | 1067 |
| i | GS020 |  | 459 |
| i | GS020 |  | 583 |
| i | GS020 |  | 993 |
| i | GS020 |  | 100 |
| i | GS020 |  | 163 |
| i | GS020 |  | 166 |
| i | GS020 |  | 583 |
| i | GS020 |  | 592 |
| i | GS020 |  | 652 |
| i | GS020 |  | 129 |
| i | GS020 |  | 697 |
| i | GS020 |  | 756 |
| i | GS020 |  | 931 |
| i | GS020 |  | 105 |
| i | GS020 |  | 107 |
| i | GS020 |  | 225 |
| i | GS020 |  | 235 |
| i | GS020 |  | 23 |
| i | GS020 |  | 376 |
| i | GS020 |  | 95 |
| i | GS020 |  | 97 |
| i | GS020 |  | 229 |
| i | GS020 |  | 977 |
| i | GS020 |  | 706 |
| i | GS020 |  | 765 |
| i | GS020 |  | 939 |
| ? | GS037-hardcoded_password | api.py | 31 |
| ? | GS037-hardcoded_password | api.py | 31 |
| ? | GS037-hardcoded_password | config.py | 253 |
| ? | GS037-hardcoded_password | ws_client.py | 166 |
| ? | GS037-hardcoded_password | config.py | 253 |
| ? | GS037-hardcoded_password | ws_client.py | 166 |
| H | GS000-LEGACY | bybit_ws_sdk.py | 38 |
| H | GS000-LEGACY | bybit_ws_sdk.py | 43 |
| H | GS008 | lstm_regime.py | 512 |
| H | GS008 | lstm_regime.py | 605 |
| H | GS008 | lstm_world_model.py | 402 |
| H | GS008 | lstm_world_model.py | 467 |
| H | GS008 | lstm_world_model.py | 565 |
| L | GS007 | lstm_regime.py | 624 |
| L | GS007 | lstm_world_model.py | 292 |
| L | GS007 | lstm_world_model.py | 479 |
| L | GS007 | lstm_world_model.py | 571 |
| M | GS000-LEGACY | bybit-ws-async.service | 8 |
| M | GS000-LEGACY | bybit-ws.service | 9 |
| H | GS025 | state.db | 0 |
| H | GS025 | openapi.yaml | 0 |
| H | GS025 | config.example.yaml | 0 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS025 | .mcp.json | 0 |
| H | ? | bybit-ws.service | 0 |
| M | ? | bybit-ws.service | 0 |
| M | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws.service | 0 |
| L | ? | bybit-ws-async.service | 0 |
| I | GS007 | adversarial_env.py | 100 |
| I | GS007 | adversarial_env.py | 104 |
| I | GS007 | adversarial_env.py | 100 |
| I | GS007 | adversarial_env.py | 104 |
| I | GS007 | gridsignal-bot.py | 197 |
| I | GS007 | gridsignal-bot.py | 202 |
| H | GS007 | gridsignal-bot.py | 148 |
| H | GS007 | gridsignal-bot.py | 249 |
| H | GS007 | gridsignal-bot.py | 390 |
| H | GS007 | gridsignal-bot.py | 1064 |
| H | GS007 | gridsignal-bot.py | 1097 |
| H | GS007 | gridsignal-bot.py | 1260 |
| H | GS007 | gridsignal-bot.py | 1294 |
| H | GS007 | gridsignal-bot.py | 1325 |
| I | GS007 | paper_api.py | 49 |
| I | GS007 | paper_trade.py | 188 |
| I | GS007 | rl_env.py | 73 |
| I | GS007 | rl_env.py | 86 |
| I | GS007 | state_db.py | 33 |
| I | GS007 | gridsignal-bot.py | 197 |
| I | GS007 | gridsignal-bot.py | 202 |
| H | GS007 | gridsignal-bot.py | 148 |
| H | GS007 | gridsignal-bot.py | 249 |
| H | GS007 | gridsignal-bot.py | 390 |
| H | GS007 | gridsignal-bot.py | 1064 |
| H | GS007 | gridsignal-bot.py | 1097 |
| H | GS007 | gridsignal-bot.py | 1260 |
| H | GS007 | gridsignal-bot.py | 1294 |
| H | GS007 | gridsignal-bot.py | 1325 |
| I | GS007 | paper_api.py | 49 |
| I | GS007 | paper_trade.py | 188 |
| I | GS007 | rl_env.py | 73 |
| I | GS007 | rl_env.py | 86 |
| I | GS007 | state_db.py | 33 |
| s | GS009 |  | 0 |
| L | GS011 | rpc.py | 455 |
| H | GS011 | rpc.py | 180 |
| L | GS011 | rpc.py | 455 |
| H | GS011 | rpc.py | 180 |
| L | GS012 | dspy_optimizer.py | 402 |
| L | GS012 | dspy_optimizer.py | 402 |
| H | GS017 | config.example.yaml | 33 |
| H | GS018 | api.py | 401 |
| H | GS018 | api.py | 301 |
| H | GS018 | auto_entry.py | 626 |
| H | GS018 | auto_short.py | 392 |
| H | GS018 | auto_short.py | 512 |
| H | GS018 | auto_short.py | 771 |
| H | GS018 | api.py | 401 |
| H | GS018 | api.py | 301 |
| H | GS018 | auto_entry.py | 626 |
| H | GS018 | auto_short.py | 392 |
| H | GS018 | auto_short.py | 512 |
| H | GS018 | auto_short.py | 771 |
| H | GS018 | dca.py | 172 |
| H | GS018 | exchange_adapter.py | 48 |
| H | GS018 | exchange_adapter.py | 127 |
| H | GS018 | exchange_adapter.py | 257 |
| H | GS018 | exchange_adapter.py | 393 |
| H | GS018 | gridsignal-bot.py | 579 |
| H | GS018 | gridsignal-bot.py | 589 |
| H | GS018 | gridsignal-bot.py | 626 |
| H | GS018 | gridsignal-bot.py | 663 |
| H | GS018 | gridsignal-bot.py | 965 |
| H | GS018 | gridsignal-bot.py | 1448 |
| H | GS018 | gridsignal-bot.py | 1726 |
| H | GS018 | self_learn.py | 163 |
| H | GS018 | self_learn.py | 163 |
| H | GS018 | ml_scorer.py | 77 |
| H | GS018 | paper_api.py | 287 |
| H | GS018 | paper_trade.py | 45 |
| H | GS018 | paper_trade.py | 96 |
| H | GS018 | paper_trade.py | 109 |
| H | GS018 | paper_trade.py | 122 |
| H | GS018 | paper_trade.py | 149 |
| H | GS018 | paper_trade.py | 273 |
| H | GS018 | paper_trade.py | 291 |
| H | GS018 | position_sizing.py | 56 |
| H | GS018 | position_sizing.py | 247 |
| H | GS018 | position_sizing.py | 333 |
| H | GS018 | rpc.py | 406 |
| H | GS018 | rpc.py | 420 |
| H | GS018 | rpc.py | 950 |
| H | GS018 | rpc.py | 1574 |
| H | GS018 | rpc.py | 1786 |
| H | GS018 | ws_client.py | 300 |
| H | GS018 | ws_client.py | 302 |
| H | GS018 | dca.py | 172 |
| H | GS018 | exchange_adapter.py | 48 |
| H | GS018 | exchange_adapter.py | 127 |
| H | GS018 | exchange_adapter.py | 257 |
| H | GS018 | exchange_adapter.py | 393 |
| H | GS018 | gridsignal-bot.py | 579 |
| H | GS018 | gridsignal-bot.py | 589 |
| H | GS018 | gridsignal-bot.py | 626 |
| H | GS018 | gridsignal-bot.py | 663 |
| H | GS018 | gridsignal-bot.py | 965 |
| H | GS018 | gridsignal-bot.py | 1448 |
| H | GS018 | gridsignal-bot.py | 1726 |
| H | GS018 | ml_scorer.py | 77 |
| H | GS018 | paper_api.py | 287 |
| H | GS018 | paper_trade.py | 45 |
| H | GS018 | paper_trade.py | 96 |
| H | GS018 | paper_trade.py | 109 |
| H | GS018 | paper_trade.py | 122 |
| H | GS018 | paper_trade.py | 149 |
| H | GS018 | paper_trade.py | 273 |
| H | GS018 | paper_trade.py | 291 |
| H | GS018 | position_sizing.py | 56 |
| H | GS018 | position_sizing.py | 247 |
| H | GS018 | position_sizing.py | 333 |
| H | GS018 | rpc.py | 406 |
| H | GS018 | rpc.py | 420 |
| H | GS018 | rpc.py | 950 |
| H | GS018 | rpc.py | 1574 |
| H | GS018 | rpc.py | 1786 |
| H | GS018 | ws_client.py | 300 |
| H | GS018 | ws_client.py | 302 |
| s | GS021 |  | 135 |
| s | GS021 |  | 135 |
| s | GS021 |  | 135 |
| s | GS021 |  | 662 |
| s | GS021 |  | 663 |
| s | GS021 |  | 21 |
| s | GS021 |  | 8 |
| s | GS021 |  | 33 |
| s | GS021 |  | 28 |
| s | GS021 |  | 95 |
| s | GS021 |  | 300 |
| s | GS021 |  | 300 |
| s | GS021 |  | 506 |
| s | GS021 |  | 506 |
| s | GS021 |  | 693 |
| s | GS021 |  | 1869 |
| s | GS021 |  | 6 |
| s | GS021 |  | 96 |
| s | GS021 |  | 135 |
| s | GS021 |  | 135 |
| s | GS021 |  | 135 |
| s | GS021 |  | 662 |
| s | GS021 |  | 663 |
| s | GS021 |  | 21 |
| s | GS021 |  | 8 |
| s | GS021 |  | 33 |
| s | GS021 |  | 28 |
| s | GS021 |  | 95 |
| s | GS021 |  | 300 |
| s | GS021 |  | 300 |
| s | GS021 |  | 506 |
| s | GS021 |  | 506 |
| s | GS021 |  | 693 |
| s | GS021 |  | 1869 |
| s | GS021 |  | 6 |
| s | GS021 |  | 40 |
| s | GS021 |  | 1628 |
| s | GS021 |  | 1898 |
| s | GS021 |  | 149 |
| s | GS021 |  | 264 |
| s | GS021 |  | 308 |
| s | GS021 |  | 125 |
| s | GS021 |  | 311 |
| s | GS021 |  | 457 |
| s | GS021 |  | 545 |
| s | GS021 |  | 6588 |
| s | GS021 |  | 248 |
| s | GS021 |  | 721 |
| s | GS021 |  | 225 |
| s | GS021 |  | 118 |
| s | GS021 |  | 294 |
| s | GS021 |  | 392 |
| s | GS021 |  | 468 |
| s | GS021 |  | 71 |
| s | GS021 |  | 36 |
| s | GS021 |  | 556 |
| s | GS021 |  | 679 |
| s | GS021 |  | 466 |
| s | GS021 |  | 470 |
| s | GS021 |  | 675 |
| s | GS021 |  | 516 |
| s | GS021 |  | 522 |
| s | GS021 |  | 21 |
| r | GS022 |  | 734 |
| r | GS022 |  | 735 |
| r | GS022 |  | 808 |
| r | GS022 |  | 809 |
| r | GS022 |  | 734 |
| r | GS022 |  | 735 |
| r | GS022 |  | 808 |
| r | GS022 |  | 809 |
| r | GS022 |  | 746 |
| r | GS022 |  | 1756 |
| r | GS022 |  | 1841 |
| r | GS022 |  | 2077 |
| r | GS022 |  | 2078 |
| r | GS022 |  | 2081 |
| r | GS022 |  | 2092 |
| r | GS022 |  | 2126 |
| r | GS022 |  | 2172 |
| r | GS022 |  | 2179 |
| r | GS022 |  | 2186 |
| r | GS022 |  | 2194 |
| r | GS022 |  | 2208 |
| r | GS022 |  | 2318 |
| r | GS022 |  | 2347 |
| r | GS022 |  | 2352 |
| r | GS022 |  | 2354 |
| r | GS022 |  | 2356 |
| r | GS022 |  | 2358 |
| r | GS022 |  | 2360 |
| r | GS022 |  | 2362 |
| r | GS022 |  | 2641 |
| r | GS022 |  | 2646 |
| r | GS022 |  | 2653 |
| r | GS022 |  | 2654 |
| r | GS022 |  | 2656 |
| r | GS022 |  | 2657 |
| r | GS022 |  | 2660 |
| r | GS022 |  | 2663 |
| r | GS022 |  | 2666 |
| r | GS022 |  | 2667 |
| r | GS022 |  | 2678 |
| r | GS022 |  | 2679 |
| r | GS022 |  | 2693 |
| r | GS022 |  | 2724 |
| r | GS022 |  | 2745 |
| r | GS022 |  | 49 |
| r | GS022 |  | 57 |
| r | GS022 |  | 98 |
| r | GS022 |  | 239 |
| r | GS022 |  | 241 |
| r | GS022 |  | 301 |
| r | GS022 |  | 357 |
| r | GS022 |  | 411 |
| r | GS022 |  | 421 |
| r | GS022 |  | 427 |
| r | GS022 |  | 430 |
| r | GS022 |  | 441 |
| r | GS022 |  | 447 |
| r | GS022 |  | 460 |
| r | GS022 |  | 523 |
| r | GS022 |  | 28 |
| r | GS022 |  | 29 |
| r | GS022 |  | 36 |
| r | GS022 |  | 37 |
| r | GS022 |  | 66 |
| r | GS022 |  | 2535 |
| r | GS022 |  | 300 |
| r | GS022 |  | 302 |
| r | GS022 |  | 6 |
| r | GS022 |  | 33 |
| r | GS022 |  | 37 |
| r | GS022 |  | 38 |
| r | GS022 |  | 56 |
| r | GS022 |  | 182 |
| r | GS022 |  | 394 |
| r | GS022 |  | 17 |
| r | GS022 |  | 236 |
| r | GS022 |  | 257 |
| r | GS022 |  | 349 |
| r | GS022 |  | 417 |
| r | GS022 |  | 458 |
| r | GS022 |  | 507 |
| r | GS022 |  | 94 |
| r | GS022 |  | 317 |
| r | GS022 |  | 135 |
| r | GS022 |  | 147 |
| r | GS022 |  | 575 |
| r | GS022 |  | 706 |
| r | GS022 |  | 579 |
| r | GS022 |  | 711 |
| r | GS022 |  | 1121 |
| r | GS022 |  | 1138 |
| r | GS022 |  | 1141 |
| r | GS022 |  | 1180 |
| r | GS022 |  | 370 |
| r | GS022 |  | 383 |
| r | GS022 |  | 434 |
| r | GS022 |  | 579 |
| r | GS022 |  | 629 |
| r | GS022 |  | 641 |
| r | GS022 |  | 652 |
| r | GS022 |  | 539 |
| r | GS022 |  | 543 |
| r | GS022 |  | 685 |
| r | GS022 |  | 1466 |
| r | GS022 |  | 1475 |
| r | GS022 |  | 1099 |
| r | GS022 |  | 86 |
| r | GS022 |  | 175 |
| r | GS022 |  | 382 |
| r | GS022 |  | 481 |
| r | GS022 |  | 157 |
| r | GS022 |  | 96 |
| r | GS022 |  | 118 |
| r | GS022 |  | 126 |
| r | GS022 |  | 20 |
| r | GS022 |  | 215 |
| r | GS022 |  | 113 |
| r | GS022 |  | 439 |
| r | GS022 |  | 481 |
| r | GS022 |  | 509 |
| r | GS022 |  | 511 |
| r | GS022 |  | 520 |
| r | GS022 |  | 530 |
| r | GS022 |  | 532 |
| r | GS022 |  | 677 |
| r | GS022 |  | 21 |
| r | GS022 |  | 49 |
| r | GS022 |  | 55 |
| r | GS022 |  | 60 |
| r | GS022 |  | 67 |
| r | GS022 |  | 225 |
| r | GS022 |  | 23 |
| r | GS022 |  | 156 |
| r | GS022 |  | 157 |
| r | GS022 |  | 203 |
| r | GS022 |  | 226 |
| r | GS022 |  | 230 |
| r | GS022 |  | 235 |
| r | GS022 |  | 352 |
| r | GS022 |  | 359 |
| r | GS022 |  | 58 |
| r | GS022 |  | 260 |
| r | GS022 |  | 693 |
| r | GS022 |  | 827 |
| r | GS022 |  | 892 |
| r | GS022 |  | 928 |
| r | GS022 |  | 1046 |
| r | GS022 |  | 1070 |
| r | GS022 |  | 1076 |
| r | GS022 |  | 1128 |
| r | GS022 |  | 37 |
| r | GS022 |  | 93 |
| r | GS022 |  | 284 |
| r | GS022 |  | 296 |
| r | GS022 |  | 491 |
| r | GS022 |  | 494 |
| r | GS022 |  | 496 |
| r | GS022 |  | 539 |
| r | GS022 |  | 541 |
| r | GS022 |  | 546 |
| r | GS022 |  | 549 |
| r | GS022 |  | 550 |
| r | GS022 |  | 551 |
| r | GS022 |  | 565 |
| r | GS022 |  | 584 |
| r | GS022 |  | 589 |
| r | GS022 |  | 627 |
| r | GS022 |  | 666 |
| r | GS022 |  | 669 |
| r | GS022 |  | 6 |
| r | GS022 |  | 23 |
| r | GS022 |  | 48 |
| r | GS022 |  | 70 |
| r | GS022 |  | 181 |
| r | GS022 |  | 192 |
| r | GS022 |  | 363 |
| r | GS022 |  | 374 |
| r | GS022 |  | 697 |
| r | GS022 |  | 404 |
| r | GS022 |  | 411 |
| r | GS022 |  | 470 |
| r | GS022 |  | 477 |
| r | GS022 |  | 117 |
| r | GS022 |  | 127 |
| r | GS022 |  | 369 |
| r | GS022 |  | 379 |
| r | GS022 |  | 795 |
| r | GS022 |  | 805 |
| r | GS022 |  | 978 |
| r | GS022 |  | 1382 |
| r | GS022 |  | 1395 |
| r | GS022 |  | 1672 |
| r | GS022 |  | 1682 |
| r | GS022 |  | 77 |
| r | GS022 |  | 87 |
| r | GS022 |  | 777 |
| r | GS022 |  | 787 |
| r | GS022 |  | 60 |
| r | GS022 |  | 110 |
| r | GS022 |  | 346 |
| r | GS022 |  | 347 |
| r | GS022 |  | 348 |
| r | GS022 |  | 349 |
| r | GS022 |  | 350 |
| r | GS022 |  | 351 |
| r | GS022 |  | 352 |
| r | GS022 |  | 352 |
| r | GS022 |  | 353 |
| r | GS022 |  | 354 |
| r | GS022 |  | 355 |
| r | GS022 |  | 366 |
| r | GS022 |  | 367 |
| r | GS022 |  | 368 |
| r | GS022 |  | 369 |
| r | GS022 |  | 370 |
| r | GS022 |  | 169 |
| r | GS022 |  | 335 |
| r | GS022 |  | 28 |
| r | GS022 |  | 29 |
| r | GS022 |  | 36 |
| r | GS022 |  | 37 |
| r | GS022 |  | 66 |
| r | GS022 |  | 2458 |
| r | GS022 |  | 26 |
| r | GS022 |  | 26 |
| r | GS022 |  | 70 |
| r | GS022 |  | 38 |
| r | GS022 |  | 189 |
| r | GS022 |  | 1614 |
| r | GS022 |  | 20 |
| r | GS022 |  | 46 |
| r | GS022 |  | 104 |
| r | GS022 |  | 22 |
| r | GS022 |  | 76 |
| r | GS022 |  | 78 |
| r | GS022 |  | 191 |
| r | GS022 |  | 196 |
| r | GS022 |  | 206 |
| r | GS022 |  | 218 |
| r | GS022 |  | 219 |
| r | GS022 |  | 246 |
| r | GS022 |  | 348 |
| r | GS022 |  | 566 |
| r | GS022 |  | 705 |
| r | GS022 |  | 771 |
| r | GS022 |  | 792 |
| r | GS022 |  | 873 |
| r | GS022 |  | 892 |
| r | GS022 |  | 363 |
| r | GS022 |  | 110 |
| r | GS022 |  | 518 |
| r | GS022 |  | 660 |
| r | GS022 |  | 491 |
| r | GS022 |  | 498 |
| r | GS022 |  | 499 |
| r | GS022 |  | 643 |
| r | GS022 |  | 1083 |
| r | GS022 |  | 1100 |
| r | GS022 |  | 303 |
| r | GS022 |  | 314 |
| r | GS022 |  | 378 |
| r | GS022 |  | 497 |
| r | GS022 |  | 534 |
| r | GS022 |  | 544 |
| r | GS022 |  | 555 |
| r | GS022 |  | 853 |
| r | GS022 |  | 77 |
| r | GS022 |  | 85 |
| r | GS022 |  | 84 |
| r | GS022 |  | 168 |
| r | GS022 |  | 365 |
| r | GS022 |  | 464 |
| r | GS022 |  | 151 |
| r | GS022 |  | 50 |
| r | GS022 |  | 97 |
| r | GS022 |  | 105 |
| r | GS022 |  | 17 |
| r | GS022 |  | 183 |
| r | GS022 |  | 86 |
| r | GS022 |  | 368 |
| r | GS022 |  | 410 |
| r | GS022 |  | 434 |
| r | GS022 |  | 436 |
| r | GS022 |  | 445 |
| r | GS022 |  | 455 |
| r | GS022 |  | 457 |
| r | GS022 |  | 594 |
| r | GS022 |  | 15 |
| r | GS022 |  | 38 |
| r | GS022 |  | 44 |
| r | GS022 |  | 49 |
| r | GS022 |  | 56 |
| r | GS022 |  | 199 |
| r | GS022 |  | 17 |
| r | GS022 |  | 129 |
| r | GS022 |  | 130 |
| r | GS022 |  | 176 |
| r | GS022 |  | 200 |
| r | GS022 |  | 204 |
| r | GS022 |  | 209 |
| r | GS022 |  | 316 |
| r | GS022 |  | 323 |
| r | GS022 |  | 49 |
| r | GS022 |  | 230 |
| r | GS022 |  | 642 |
| r | GS022 |  | 774 |
| r | GS022 |  | 837 |
| r | GS022 |  | 869 |
| r | GS022 |  | 987 |
| r | GS022 |  | 1010 |
| r | GS022 |  | 1016 |
| r | GS022 |  | 1062 |
| r | GS022 |  | 30 |
| r | GS022 |  | 214 |
| r | GS022 |  | 226 |
| r | GS022 |  | 344 |
| r | GS022 |  | 346 |
| r | GS022 |  | 351 |
| r | GS022 |  | 354 |
| r | GS022 |  | 355 |
| r | GS022 |  | 356 |
| r | GS022 |  | 370 |
| r | GS022 |  | 385 |
| r | GS022 |  | 390 |
| r | GS022 |  | 427 |
| r | GS022 |  | 456 |
| r | GS022 |  | 459 |
| r | GS022 |  | 82 |
| r | GS022 |  | 111 |
| r | GS022 |  | 132 |
| r | GS022 |  | 143 |
| r | GS022 |  | 146 |
| r | GS022 |  | 333 |
| r | GS022 |  | 344 |
| r | GS022 |  | 348 |
| r | GS022 |  | 349 |
| r | GS022 |  | 350 |
| r | GS022 |  | 351 |
| r | GS022 |  | 352 |
| r | GS022 |  | 353 |
| r | GS022 |  | 357 |
| r | GS022 |  | 419 |
| r | GS022 |  | 434 |
| r | GS022 |  | 179 |
| r | GS022 |  | 358 |
| r | GS022 |  | 359 |
| r | GS022 |  | 360 |
| r | GS022 |  | 361 |
| r | GS022 |  | 362 |
| r | GS022 |  | 363 |
| r | GS022 |  | 364 |
| r | GS022 |  | 364 |
| r | GS022 |  | 365 |
| r | GS022 |  | 366 |
| r | GS022 |  | 367 |
| r | GS022 |  | 380 |
| r | GS022 |  | 381 |
| r | GS022 |  | 382 |
| r | GS022 |  | 383 |
| r | GS022 |  | 384 |
| r | GS022 |  | 180 |
| r | GS022 |  | 80 |
| r | GS022 |  | 294 |
| r | GS022 |  | 448 |
| r | GS022 |  | 23 |
| r | GS022 |  | 42 |
| r | GS022 |  | 282 |
| r | GS022 |  | 298 |
| r | GS022 |  | 305 |
| r | GS022 |  | 339 |
| r | GS022 |  | 350 |
| r | GS022 |  | 353 |
| r | GS022 |  | 399 |
| r | GS022 |  | 495 |
| r | GS022 |  | 30 |
| r | GS022 |  | 82 |
| r | GS022 |  | 92 |
| r | GS022 |  | 57 |
| r | GS022 |  | 67 |
| r | GS022 |  | 320 |
| r | GS022 |  | 327 |
| r | GS022 |  | 449 |
| r | GS022 |  | 452 |
| r | GS022 |  | 464 |
| r | GS022 |  | 464 |
| r | GS022 |  | 526 |
| r | GS022 |  | 611 |
| r | GS022 |  | 80 |
| r | GS022 |  | 88 |
| r | GS022 |  | 109 |
| r | GS022 |  | 80 |
| r | GS022 |  | 349 |
| r | GS022 |  | 376 |
| r | GS022 |  | 379 |
| r | GS022 |  | 16 |
| r | GS022 |  | 22 |
| r | GS022 |  | 33 |
| r | GS022 |  | 34 |
| r | GS022 |  | 63 |
| r | GS022 |  | 73 |
| r | GS022 |  | 83 |
| r | GS022 |  | 471 |
| r | GS022 |  | 524 |
| r | GS022 |  | 552 |
| r | GS022 |  | 560 |
| r | GS022 |  | 564 |
| r | GS022 |  | 568 |
| r | GS022 |  | 571 |
| r | GS022 |  | 573 |
| r | GS022 |  | 580 |
| r | GS022 |  | 608 |
| r | GS022 |  | 609 |
| r | GS022 |  | 127 |
| r | GS022 |  | 354 |
| r | GS022 |  | 204 |
| r | GS022 |  | 206 |
| r | GS022 |  | 700 |
| r | GS022 |  | 104 |
| r | GS022 |  | 289 |
| r | GS022 |  | 299 |
| r | GS022 |  | 309 |
| r | GS022 |  | 313 |
| r | GS022 |  | 332 |
| r | GS022 |  | 344 |
| r | GS022 |  | 133 |
| r | GS022 |  | 173 |
| r | GS022 |  | 282 |
| r | GS022 |  | 350 |
| r | GS022 |  | 435 |
| r | GS022 |  | 62 |
| r | GS022 |  | 238 |
| r | GS022 |  | 243 |
| r | GS022 |  | 784 |
| r | GS022 |  | 80 |
| r | GS022 |  | 92 |
| r | GS022 |  | 116 |
| r | GS022 |  | 140 |
| r | GS022 |  | 164 |
| r | GS022 |  | 168 |
| r | GS022 |  | 391 |
| r | GS022 |  | 440 |
| r | GS022 |  | 596 |
| r | GS022 |  | 190 |
| r | GS022 |  | 207 |
| r | GS022 |  | 138 |
| r | GS022 |  | 167 |
| r | GS022 |  | 175 |
| r | GS022 |  | 238 |
| r | GS022 |  | 275 |
| r | GS022 |  | 327 |
| r | GS022 |  | 371 |
| r | GS022 |  | 373 |
| r | GS022 |  | 379 |
| r | GS022 |  | 482 |
| r | GS022 |  | 52 |
| r | GS022 |  | 82 |
| r | GS022 |  | 107 |
| r | GS022 |  | 119 |
| r | GS022 |  | 132 |
| r | GS022 |  | 30 |
| r | GS022 |  | 48 |
| r | GS022 |  | 58 |
| r | GS022 |  | 88 |
| r | GS022 |  | 106 |
| r | GS022 |  | 111 |
| r | GS022 |  | 117 |
| r | GS022 |  | 123 |
| r | GS022 |  | 132 |
| r | GS022 |  | 135 |
| r | GS022 |  | 137 |
| r | GS022 |  | 139 |
| r | GS022 |  | 142 |
| r | GS022 |  | 143 |
| r | GS022 |  | 151 |
| r | GS022 |  | 155 |
| r | GS022 |  | 158 |
| r | GS022 |  | 161 |
| r | GS022 |  | 162 |
| r | GS022 |  | 183 |
| r | GS022 |  | 186 |
| r | GS022 |  | 187 |
| r | GS022 |  | 219 |
| r | GS022 |  | 227 |
| r | GS022 |  | 228 |
| r | GS022 |  | 259 |
| r | GS022 |  | 264 |
| r | GS022 |  | 285 |
| r | GS022 |  | 317 |
| r | GS022 |  | 318 |
| r | GS022 |  | 326 |
| r | GS022 |  | 333 |
| r | GS022 |  | 344 |
| r | GS022 |  | 405 |
| r | GS022 |  | 438 |
| r | GS022 |  | 460 |
| r | GS022 |  | 484 |
| r | GS022 |  | 499 |
| r | GS022 |  | 592 |
| r | GS022 |  | 609 |
| r | GS022 |  | 620 |
| r | GS022 |  | 646 |
| r | GS022 |  | 661 |
| r | GS022 |  | 671 |
| r | GS022 |  | 690 |
| r | GS022 |  | 718 |
| r | GS022 |  | 758 |
| r | GS022 |  | 769 |
| r | GS022 |  | 64 |
| r | GS022 |  | 71 |
| r | GS022 |  | 108 |
| r | GS022 |  | 124 |
| r | GS022 |  | 138 |
| r | GS022 |  | 162 |
| r | GS022 |  | 176 |
| r | GS022 |  | 192 |
| r | GS022 |  | 205 |
| r | GS022 |  | 228 |
| r | GS022 |  | 244 |
| r | GS022 |  | 261 |
| r | GS022 |  | 277 |
| r | GS022 |  | 293 |
| r | GS022 |  | 310 |
| r | GS022 |  | 320 |
| r | GS022 |  | 341 |
| r | GS022 |  | 355 |
| r | GS022 |  | 369 |
| r | GS022 |  | 389 |
| r | GS022 |  | 411 |
| r | GS022 |  | 425 |
| r | GS022 |  | 439 |
| r | GS022 |  | 443 |
| r | GS022 |  | 447 |
| r | GS022 |  | 461 |
| r | GS022 |  | 489 |
| r | GS022 |  | 503 |
| r | GS022 |  | 520 |
| r | GS022 |  | 538 |
| r | GS022 |  | 582 |
| r | GS022 |  | 608 |
| r | GS022 |  | 651 |
| r | GS022 |  | 675 |
| r | GS022 |  | 78 |
| r | GS022 |  | 87 |
| r | GS022 |  | 92 |
| r | GS022 |  | 100 |
| r | GS022 |  | 109 |
| r | GS022 |  | 42 |
| r | GS022 |  | 58 |
| r | GS022 |  | 62 |
| r | GS022 |  | 66 |
| r | GS022 |  | 68 |
| r | GS022 |  | 70 |
| r | GS022 |  | 137 |
| r | GS022 |  | 142 |
| r | GS022 |  | 148 |
| r | GS022 |  | 152 |
| r | GS022 |  | 161 |
| r | GS022 |  | 63 |
| r | GS022 |  | 65 |
| r | GS022 |  | 13 |
| r | GS022 |  | 18 |
| r | GS022 |  | 112 |
| r | GS022 |  | 113 |
| r | GS022 |  | 121 |
| r | GS022 |  | 154 |
| r | GS022 |  | 156 |
| r | GS022 |  | 162 |
| r | GS022 |  | 80 |
| r | GS022 |  | 118 |
| r | GS022 |  | 162 |
| r | GS022 |  | 177 |
| r | GS022 |  | 182 |
| r | GS022 |  | 367 |
| r | GS022 |  | 386 |
| r | GS022 |  | 389 |
| r | GS022 |  | 392 |
| r | GS022 |  | 397 |
| r | GS022 |  | 461 |
| r | GS022 |  | 193 |
| r | GS022 |  | 225 |
| r | GS022 |  | 57 |
| r | GS022 |  | 61 |
| r | GS022 |  | 101 |
| r | GS022 |  | 144 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-permissive_cors |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-permissive_cors |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | lstm_regime.py | ? |
| ? | YAML-36ACF0AD | lstm_regime.py | ? |
| ? | YAML-36ACF0AD | lstm_world_model.py | ? |
| ? | YAML-36ACF0AD | lstm_world_model.py | ? |
| ? | YAML-36ACF0AD | lstm_world_model.py | ? |
| ? | YAML-36ACF0AD | lstm_regime.py | ? |
| ? | YAML-36ACF0AD | lstm_regime.py | ? |
| ? | YAML-36ACF0AD | lstm_world_model.py | ? |
| ? | YAML-36ACF0AD | lstm_world_model.py | ? |
| ? | YAML-36ACF0AD | lstm_world_model.py | ? |
| ? | YAML-B39DC08C | config.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | lstm_regime.py | ? |
| ? | YAML-B39DC08C | metrics.py | ? |
| ? | YAML-B39DC08C | ml_scorer.py | ? |
| ? | YAML-B39DC08C | optuna_tuner.py | ? |
| ? | YAML-B39DC08C | config.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | lstm_regime.py | ? |
| ? | YAML-B39DC08C | metrics.py | ? |
| ? | YAML-B39DC08C | ml_scorer.py | ? |
| ? | YAML-B39DC08C | optuna_tuner.py | ? |
| M | ? | gridsignal-bot.py | 1341 |
| M | ? | gridsignal-bot.py | 1343 |
| M | ? | gridsignal-bot.py | 1442 |
| M | ? | gridsignal-bot.py | 1444 |
| M | ? | gridsignal-bot.py | 1534 |
| M | ? | gridsignal-bot.py | 2099 |
| M | ? | run_dspy_train.py | 36 |
| M | ? | gridsignal_scanner.py | 46 |
| M | ? | mcp_server.py | 55 |
| M | ? | mcp_server.py | 70 |
| M | ? | mcp_server.py | 88 |
| M | ? | main.py | 135 |
| M | ? | optuna_tuner.py | 69 |
| M | ? | constants.py | 45 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:04:32.546873*