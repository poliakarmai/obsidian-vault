---
title: "GSC Audit: /tmp/bybit-scan"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/bybit-scan

**Дата:** 07.08.2026 15:09  
**Путь:** `/tmp/bybit-scan`  
**Всего находок:** 439  
**CRITICAL:** 2 | **HIGH:** 69 | **MEDIUM:** 29 | **LOW:** 300

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 264 |
| GS018 | 37 |
| GS008 | 36 |
| GS007 | 25 |
| GS000-LEGACY | 19 |
| GS021 | 16 |
| Синхронный код в async | 14 |
| GS029 | 8 |
| GS025-eval_usage | 6 |
| GS022 | 4 |
| GS025 | 3 |
| GS005 | 2 |
| GS015 | 1 |
| GS020 | 1 |
| GS009 | 1 |
| GS012 | 1 |
| GS025-permissive_cors | 1 |

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
| HIGH | GS000-LEGACY | config.py | 135 | Match:     'bind': '127.0.0.1',      # default to localhost; |
| HIGH | GS000-LEGACY | main_async.py | 661 | Match:         ws_push_thread = start_ws_server(port=8768, b |
| HIGH | GS000-LEGACY | main_async.py | 662 | Match:         log_event('📡 WebSocket push server on 127.0.0 |
| HIGH | GS000-LEGACY | mcp_server.py | 28 | Match: RPC_BASE = f"http://127.0.0.1:{RPC_PORT}" |
| HIGH | GS000-LEGACY | rpc.py | 95 | Match: def start_ws_server(port=8767, bind='127.0.0.1'): |
| HIGH | GS000-LEGACY | rpc.py | 300 | Match:     handler.send_header("Access-Control-Allow-Origin" |
| HIGH | GS000-LEGACY | rpc.py | 465 | Match:         self.send_header("Access-Control-Allow-Origin |
| HIGH | GS000-LEGACY | rpc.py | 648 | Match:             "rpc_host": "127.0.0.1", |
| HIGH | GS000-LEGACY | rpc.py | 1765 | Match: def start_rpc_server(port=8766, bind='127.0.0.1'): |
| HIGH | GS000-LEGACY | bybit_ws_sdk.py | 38 | Match:         r = requests.get(f"{self.base_url}{path}", ti |
| HIGH | GS000-LEGACY | bybit_ws_sdk.py | 43 | Match:         r = requests.post(f"{self.base_url}{path}", j |
| HIGH | GS008 | lstm_regime.py | 512 | Match:         model.eval() |
| HIGH | GS008 | lstm_regime.py | 605 | Match:         model.eval() |
| HIGH | GS008 | lstm_world_model.py | 402 | Match:         model.eval() |
| HIGH | GS008 | lstm_world_model.py | 467 | Match:     model.eval() |
| HIGH | GS008 | lstm_world_model.py | 565 | Match:     model.eval() |
| HIGH | GS007 | gridsignal-bot.py | 148 | Line 148: "SELECT 1 FROM pro_users WHERE user_id=? AND activ |
| HIGH | GS007 | gridsignal-bot.py | 249 | Line 249: row = conn.execute('SELECT user_id, username, firs |
| HIGH | GS007 | gridsignal-bot.py | 390 | Line 390: row = conn.execute('SELECT lang FROM users WHERE u |
| HIGH | GS007 | gridsignal-bot.py | 1064 | Line 1064: "SELECT paid_at, expires_at, active FROM pro_user |
| HIGH | GS007 | gridsignal-bot.py | 1097 | Line 1097: "SELECT 1 FROM pro_users WHERE user_id=? AND char |
| HIGH | GS007 | gridsignal-bot.py | 1260 | Line 1260: 'SELECT outcome, pnl_pct FROM signals WHERE user_ |
| HIGH | GS007 | gridsignal-bot.py | 1294 | Line 1294: alerts = conn.execute('SELECT symbol FROM alerts  |
| HIGH | GS007 | gridsignal-bot.py | 1325 | Line 1325: alert_count = conn.execute('SELECT COUNT(*) FROM  |
| HIGH | GS018 | api.py | 401 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | api.py | 301 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_entry.py | 626 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 384 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 504 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 762 | Float arithmetic for money leads to rounding errors exploita |
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
| HIGH | GS018 | rpc.py | 905 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 1529 | Float arithmetic for money leads to rounding errors exploita |
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
| M | GS029 | mcp_server.py | 39 |
| M | GS029 | rpc.py | 180 |
| L | GS003 | adversarial_env.py | 181 |
| L | GS003 | adversarial_env.py | 182 |
| L | GS003 | adversarial_env.py | 185 |
| L | GS003 | alerts.py | 57 |
| L | GS003 | alerts.py | 63 |
| L | GS003 | alerts.py | 64 |
| L | GS003 | bybit_ws_sdk.py | 119 |
| L | GS003 | bybit_ws_sdk.py | 124 |
| L | GS003 | bybit_ws_sdk.py | 128 |
| L | GS003 | dashboard.py | 884 |
| L | GS003 | dashboard.py | 888 |
| L | GS003 | dashboard.py | 889 |
| L | GS003 | dashboard.py | 890 |
| L | GS003 | dashboard.py | 891 |
| L | GS003 | dashboard.py | 892 |
| L | GS003 | dashboard.py | 895 |
| L | GS003 | dashboard.py | 899 |
| L | GS003 | dashboard.py | 901 |
| L | GS003 | dspy_optimizer.py | 79 |
| L | GS003 | dspy_optimizer.py | 257 |
| L | GS003 | dspy_optimizer.py | 266 |
| L | GS003 | dspy_optimizer.py | 275 |
| L | GS003 | dspy_optimizer.py | 282 |
| L | GS003 | dspy_optimizer.py | 296 |
| L | GS003 | dspy_optimizer.py | 304 |
| L | GS003 | dspy_optimizer.py | 322 |
| L | GS003 | dspy_optimizer.py | 584 |
| L | GS003 | dspy_optimizer.py | 612 |
| L | GS003 | dspy_optimizer.py | 614 |
| L | GS003 | dspy_optimizer.py | 617 |
| L | GS003 | dspy_optimizer.py | 618 |
| L | GS003 | dspy_optimizer.py | 620 |
| L | GS003 | dspy_optimizer.py | 621 |
| L | GS003 | dspy_optimizer.py | 623 |
| L | GS003 | ensemble.py | 262 |
| L | GS003 | ensemble.py | 263 |
| L | GS003 | ensemble.py | 265 |
| L | GS003 | ensemble.py | 266 |
| L | GS003 | ensemble.py | 269 |
| L | GS003 | ensemble.py | 271 |
| L | GS003 | funding_tracker.py | 223 |
| L | GS003 | funding_tracker.py | 225 |
| L | GS003 | funding_tracker.py | 227 |
| L | GS003 | funding_tracker.py | 232 |
| L | GS003 | funding_tracker.py | 234 |
| L | GS003 | gridsignal-bot.py | 33 |
| L | GS003 | gridsignal-bot.py | 35 |
| L | GS003 | gridsignal-bot.py | 37 |
| L | GS003 | gridsignal-bot.py | 99 |
| L | GS003 | gridsignal-bot.py | 123 |
| L | GS003 | gridsignal-bot.py | 303 |
| L | GS003 | gridsignal-bot.py | 345 |
| L | GS003 | gridsignal-bot.py | 367 |
| L | GS003 | gridsignal-bot.py | 370 |
| L | GS003 | gridsignal-bot.py | 373 |
| L | GS003 | gridsignal-bot.py | 1348 |
| L | GS003 | gridsignal-bot.py | 1451 |
| L | GS003 | gridsignal-bot.py | 1544 |
| L | GS003 | gridsignal-bot.py | 2473 |
| L | GS003 | gridsignal-bot.py | 2528 |
| L | GS003 | gridsignal_scanner.py | 751 |
| L | GS003 | gridsignal_scanner.py | 753 |
| L | GS003 | gridsignal_scanner.py | 755 |
| L | GS003 | gridsignal_scanner.py | 757 |
| L | GS003 | lstm_regime.py | 64 |
| L | GS003 | lstm_regime.py | 434 |
| L | GS003 | lstm_regime.py | 438 |
| L | GS003 | lstm_regime.py | 441 |
| L | GS003 | lstm_regime.py | 443 |
| L | GS003 | lstm_regime.py | 445 |
| L | GS003 | lstm_regime.py | 448 |
| L | GS003 | lstm_regime.py | 450 |
| L | GS003 | lstm_regime.py | 456 |
| L | GS003 | lstm_regime.py | 459 |
| L | GS003 | lstm_regime.py | 489 |
| L | GS003 | lstm_regime.py | 525 |
| L | GS003 | lstm_regime.py | 526 |
| L | GS003 | lstm_regime.py | 554 |
| L | GS003 | lstm_regime.py | 556 |
| L | GS003 | lstm_regime.py | 602 |
| L | GS003 | lstm_regime.py | 609 |
| L | GS003 | lstm_regime.py | 651 |
| L | GS003 | lstm_regime.py | 696 |
| L | GS003 | lstm_regime.py | 796 |
| L | GS003 | lstm_regime.py | 800 |
| L | GS003 | lstm_regime.py | 802 |
| L | GS003 | lstm_regime.py | 807 |
| L | GS003 | lstm_regime.py | 810 |
| L | GS003 | lstm_regime.py | 812 |
| L | GS003 | lstm_regime.py | 814 |
| L | GS003 | lstm_world_model.py | 293 |
| L | GS003 | lstm_world_model.py | 297 |
| L | GS003 | lstm_world_model.py | 298 |
| L | GS003 | lstm_world_model.py | 302 |
| L | GS003 | lstm_world_model.py | 310 |
| L | GS003 | lstm_world_model.py | 312 |
| L | GS003 | lstm_world_model.py | 320 |
| L | GS003 | lstm_world_model.py | 328 |
| L | GS003 | lstm_world_model.py | 329 |
| L | GS003 | lstm_world_model.py | 332 |
| L | GS003 | lstm_world_model.py | 334 |
| L | GS003 | lstm_world_model.py | 340 |
| L | GS003 | lstm_world_model.py | 375 |
| L | GS003 | lstm_world_model.py | 427 |
| L | GS003 | lstm_world_model.py | 431 |
| L | GS003 | lstm_world_model.py | 447 |
| L | GS003 | lstm_world_model.py | 448 |
| L | GS003 | lstm_world_model.py | 473 |
| L | GS003 | lstm_world_model.py | 691 |
| L | GS003 | lstm_world_model.py | 693 |
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
| L | GS003 | main_async.py | 606 |
| L | GS003 | main_async.py | 622 |
| L | GS003 | margin_alerts.py | 202 |
| L | GS003 | margin_alerts.py | 204 |
| L | GS003 | margin_alerts.py | 208 |
| L | GS003 | margin_alerts.py | 213 |
| L | GS003 | margin_alerts.py | 215 |
| L | GS003 | margin_alerts.py | 216 |
| L | GS003 | margin_alerts.py | 217 |
| L | GS003 | margin_alerts.py | 218 |
| L | GS003 | margin_alerts.py | 221 |
| L | GS003 | margin_alerts.py | 224 |
| L | GS003 | margin_alerts.py | 227 |
| L | GS003 | margin_alerts.py | 229 |
| L | GS003 | margin_alerts.py | 231 |
| L | GS003 | metrics.py | 96 |
| L | GS003 | metrics.py | 97 |
| L | GS003 | metrics.py | 98 |
| L | GS003 | metrics.py | 99 |
| L | GS003 | metrics.py | 105 |
| L | GS003 | metrics.py | 107 |
| L | GS003 | metrics.py | 109 |
| L | GS003 | metrics.py | 110 |
| L | GS003 | metrics.py | 113 |
| L | GS003 | ml_scorer.py | 33 |
| L | GS003 | ml_scorer.py | 140 |
| L | GS003 | ml_scorer.py | 148 |
| L | GS003 | ml_scorer.py | 151 |
| L | GS003 | ml_scorer.py | 164 |
| L | GS003 | ml_scorer.py | 186 |
| L | GS003 | ml_scorer.py | 188 |
| L | GS003 | ml_scorer.py | 205 |
| L | GS003 | ml_scorer.py | 220 |
| L | GS003 | ml_scorer.py | 231 |
| L | GS003 | ml_scorer.py | 294 |
| L | GS003 | ml_scorer.py | 316 |
| L | GS003 | ml_scorer.py | 408 |
| L | GS003 | ml_scorer.py | 410 |
| L | GS003 | optimize_params.py | 78 |
| L | GS003 | optimize_params.py | 184 |
| L | GS003 | optimize_params.py | 198 |
| L | GS003 | optimize_params.py | 205 |
| L | GS003 | optimize_params.py | 230 |
| L | GS003 | optimize_params.py | 232 |
| L | GS003 | optuna_tuner.py | 94 |
| L | GS003 | optuna_tuner.py | 277 |
| L | GS003 | optuna_tuner.py | 281 |
| L | GS003 | optuna_tuner.py | 283 |
| L | GS003 | optuna_tuner.py | 307 |
| L | GS003 | optuna_tuner.py | 314 |
| L | GS003 | optuna_tuner.py | 316 |
| L | GS003 | optuna_tuner.py | 319 |
| L | GS003 | optuna_tuner.py | 364 |
| L | GS003 | optuna_tuner.py | 386 |
| L | GS003 | optuna_tuner.py | 399 |
| L | GS003 | optuna_tuner.py | 401 |
| L | GS003 | optuna_tuner.py | 403 |
| L | GS003 | optuna_tuner.py | 433 |
| L | GS003 | paper_trade.py | 458 |
| L | GS003 | paper_trade.py | 479 |
| L | GS003 | paper_trade.py | 481 |
| L | GS003 | paper_trade.py | 482 |
| L | GS003 | paper_trade.py | 483 |
| L | GS003 | paper_trade.py | 484 |
| L | GS003 | paper_trade.py | 485 |
| L | GS003 | paper_trade.py | 486 |
| L | GS003 | paper_trade.py | 487 |
| L | GS003 | paper_trade.py | 488 |
| L | GS003 | paper_trade.py | 489 |
| L | GS003 | paper_trade.py | 490 |
| L | GS003 | paper_trade.py | 491 |
| L | GS003 | paper_trade.py | 492 |
| L | GS003 | paper_trade.py | 493 |
| L | GS003 | paper_trade.py | 494 |
| L | GS003 | paper_trade.py | 497 |
| L | GS003 | paper_trade.py | 498 |
| L | GS003 | paper_trade.py | 502 |
| L | GS003 | partial_tp.py | 249 |
| L | GS003 | partial_tp.py | 251 |
| L | GS003 | push_notifier.py | 188 |
| L | GS003 | push_notifier.py | 194 |
| L | GS003 | push_notifier.py | 197 |
| L | GS003 | push_notifier.py | 200 |
| L | GS003 | push_notifier.py | 292 |
| L | GS003 | push_notifier.py | 295 |
| L | GS003 | rl_agent.py | 42 |
| L | GS003 | rl_agent.py | 53 |
| L | GS003 | rl_agent.py | 57 |
| L | GS003 | rl_agent.py | 61 |
| L | GS003 | rl_agent.py | 67 |
| L | GS003 | rl_agent.py | 70 |
| L | GS003 | rl_agent.py | 72 |
| L | GS003 | rl_agent.py | 115 |
| L | GS003 | rl_agent.py | 135 |
| L | GS003 | rl_agent.py | 153 |
| L | GS003 | rl_agent.py | 188 |
| L | GS003 | rl_agent.py | 262 |
| L | GS003 | rl_agent.py | 267 |
| L | GS003 | rl_agent.py | 270 |
| L | GS003 | rl_agent.py | 272 |
| L | GS003 | rl_env.py | 342 |
| L | GS003 | rl_env.py | 359 |
| L | GS003 | rl_env.py | 370 |
| L | GS003 | run_dspy_train.py | 25 |
| L | GS003 | run_dspy_train.py | 29 |
| L | GS003 | run_dspy_train.py | 34 |
| L | GS003 | run_dspy_train.py | 42 |
| L | GS003 | run_dspy_train.py | 44 |
| L | GS003 | scan_unpack.py | 91 |
| L | GS003 | scan_unpack.py | 94 |
| L | GS003 | scan_unpack.py | 110 |
| L | GS003 | scan_unpack.py | 112 |
| L | GS003 | scan_unpack.py | 113 |
| L | GS003 | scan_unpack.py | 117 |
| L | GS003 | scan_unpack.py | 119 |
| L | GS003 | short_strategy.py | 481 |
| L | GS003 | short_strategy.py | 482 |
| L | GS003 | short_strategy.py | 489 |
| L | GS003 | short_strategy.py | 494 |
| L | GS003 | short_strategy.py | 503 |
| L | GS003 | short_strategy.py | 506 |
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
| L | GS008 | auto_entry.py | 34 |
| L | GS008 | constants.py | 17 |
| L | GS008 | constants.py | 18 |
| L | GS008 | constants.py | 19 |
| L | GS008 | constants.py | 20 |
| L | GS008 | constants.py | 21 |
| L | GS008 | constants.py | 22 |
| L | GS008 | constants.py | 23 |
| L | GS008 | constants.py | 26 |
| L | GS008 | constants.py | 28 |
| L | GS008 | constants.py | 31 |
| L | GS008 | constants.py | 34 |
| L | GS008 | funding_entry.py | 24 |
| L | GS008 | mean_revert.py | 26 |
| L | GS008 | optimize_params.py | 24 |
| L | GS008 | optimize_params.py | 28 |
| L | GS008 | paper_trade.py | 34 |
| L | GS008 | pump_detect.py | 33 |
| L | GS008 | pump_detect.py | 38 |
| L | GS008 | regime.py | 289 |
| L | GS008 | regime.py | 299 |
| L | GS008 | regime.py | 309 |
| L | GS008 | rl_env.py | 40 |
| L | GS008 | rpc.py | 116 |
| L | GS008 | unified_sl.py | 16 |
| L | GS008 | utils.py | 68 |
| L | GS008 | utils.py | 69 |
| L | GS008 | utils.py | 70 |
| L | GS008 | utils.py | 71 |
| L | GS008 | utils.py | 72 |
| L | GS008 | ws_client.py | 96 |
| I | GS015 | main.py | 1 |
| i | GS020 |  | 1579 |
| H | GS000-LEGACY | config.py | 135 |
| H | GS000-LEGACY | main_async.py | 661 |
| H | GS000-LEGACY | main_async.py | 662 |
| H | GS000-LEGACY | mcp_server.py | 28 |
| H | GS000-LEGACY | rpc.py | 95 |
| H | GS000-LEGACY | rpc.py | 300 |
| H | GS000-LEGACY | rpc.py | 465 |
| H | GS000-LEGACY | rpc.py | 648 |
| H | GS000-LEGACY | rpc.py | 1765 |
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
| s | GS009 |  | 0 |
| L | GS012 | dspy_optimizer.py | 402 |
| H | GS018 | api.py | 401 |
| H | GS018 | api.py | 301 |
| H | GS018 | auto_entry.py | 626 |
| H | GS018 | auto_short.py | 384 |
| H | GS018 | auto_short.py | 504 |
| H | GS018 | auto_short.py | 762 |
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
| H | GS018 | rpc.py | 905 |
| H | GS018 | rpc.py | 1529 |
| H | GS018 | ws_client.py | 300 |
| H | GS018 | ws_client.py | 302 |
| s | GS021 |  | 135 |
| s | GS021 |  | 135 |
| s | GS021 |  | 135 |
| s | GS021 |  | 661 |
| s | GS021 |  | 662 |
| s | GS021 |  | 21 |
| s | GS021 |  | 8 |
| s | GS021 |  | 33 |
| s | GS021 |  | 28 |
| s | GS021 |  | 95 |
| s | GS021 |  | 300 |
| s | GS021 |  | 300 |
| s | GS021 |  | 465 |
| s | GS021 |  | 465 |
| s | GS021 |  | 648 |
| s | GS021 |  | 1765 |
| r | GS022 |  | 689 |
| r | GS022 |  | 690 |
| r | GS022 |  | 763 |
| r | GS022 |  | 764 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-permissive_cors |  | ? |
| ? | GS025-eval_usage |  | ? |
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
*Сгенерировано GSC v0.6 · 2026-08-07T15:09:20.288520*