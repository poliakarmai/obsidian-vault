---
title: "GSC Audit: ."
date: 2026-06-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — .

**Дата:** 27.06.2026 14:16  
**Путь:** `/home/openclaw/bybit-ws`  
**Всего находок:** 456  
**CRITICAL:** 3 | **HIGH:** 32 | **MEDIUM:** 21 | **LOW:** 400

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 391 |
| Хардкод IP адреса | 17 |
| Синхронный код в async | 14 |
| Python: File upload without content-type validation | 4 |
| Python: assert in production | 2 |
| Python: SSRF via requests without URL validation | 2 |
| User-controlled URL in request | 2 |
| eval() or exec() usage | 2 |
| Systemd: RestrictSUIDSGID= not set | 2 |
| GS005 | 2 |
| SQL injection risk: f-string in query | 1 |
| Python: CORS misconfiguration — allow all origins | 1 |
| pickle.load() — unsafe deserialization | 1 |
| Systemd: EnvironmentFile without quotes → word splitting | 1 |
| Systemd: ExecStart with shell metacharacters | 1 |
| World-readable file: state.db (644) | 1 |
| World-readable file: openapi.yaml (664) | 1 |
| World-readable file: config.example.yaml (664) | 1 |
| World-readable file: docker-compose.yml (664) | 1 |
| Systemd: NoNewPrivileges= not set | 1 |
| Systemd: ProtectSystem= not set | 1 |
| Systemd: ProtectHome= not set | 1 |
| Systemd: PrivateTmp= not set | 1 |
| Systemd: ProtectProc= not set | 1 |
| Systemd: MemoryDenyWriteExecute= not set | 1 |
| Systemd: RestrictRealtime= not set | 1 |
| Systemd: RemoveIPC= not set | 1 |
| Systemd: LockPersonality= not set | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | dspy_optimizer.py | 84 | OWASP A03: Injection |
| CRITICAL | GS005 | dspy_optimizer.py | 83 | Line 83: rows = conn.execute( |
| CRITICAL | GS005 | dspy_optimizer.py | 83 | Line 83: rows = conn.execute( |
| HIGH | ? | bybit_ws_sdk.py | 38 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | bybit_ws_sdk.py | 43 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | dspy_optimizer.py | 404 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | rl_agent.py | 139 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | lstm_regime.py | 527 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | dspy_optimizer.py | 405 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | main_async.py | 390 | Match:         ws_push_thread = start_ws_server(port=8767, b |
| HIGH | ? | main_async.py | 391 | Match:         log_event('📡 WebSocket push server on 127.0.0 |
| HIGH | ? | main_async.py | 358 | Match:         ws_push_thread = start_ws_server(port=8767, b |
| HIGH | ? | main_async.py | 359 | Match:         log_event('📡 WebSocket push server on 127.0.0 |
| HIGH | ? | config.py | 135 | Match:     'bind': '127.0.0.1',      # default to localhost; |
| HIGH | ? | docker-entrypoint.sh | 16 | Match: echo "   RPC: http://0.0.0.0:8766" |
| HIGH | ? | docker-entrypoint.sh | 17 | Match: echo "   Health: http://0.0.0.0:8766/health" |
| HIGH | ? | rpc.py | 95 | Match: def start_ws_server(port=8767, bind='127.0.0.1'): |
| HIGH | ? | rpc.py | 299 | Match:     handler.send_header("Access-Control-Allow-Origin" |
| HIGH | ? | rpc.py | 451 | Match:         self.send_header("Access-Control-Allow-Origin |
| HIGH | ? | rpc.py | 605 | Match:             "rpc_host": "127.0.0.1", |
| HIGH | ? | rpc.py | 1568 | Match: def start_rpc_server(port=8766, bind='127.0.0.1'): |
| HIGH | ? | dashboard.html | 125 | Match: const WS_URL = 'ws://127.0.0.1:8767/ws'; |
| HIGH | ? | proxy_server.py | 6 | Match: RPC = 'http://127.0.0.1:8766' |
| HIGH | ? | proxy_server.py | 96 | Match:     HTTPServer(('127.0.0.1', 9999), P).serve_forever( |
| HIGH | ? | mcp_server.py | 28 | Match: RPC_BASE = f"http://127.0.0.1:{RPC_PORT}" |
| HIGH | ? | config.example.yaml | 412 | Match:   rpc_bind: "127.0.0.1" |
| HIGH | ? | bybit_ws_sdk.py | 38 | Match:         r = requests.get(f"{self.base_url}{path}", ti |
| HIGH | ? | bybit_ws_sdk.py | 43 | Match:         r = requests.post(f"{self.base_url}{path}", j |
| HIGH | ? | lstm_regime.py | 508 | Match:         model.eval() |
| HIGH | ? | lstm_regime.py | 601 | Match:         model.eval() |
| HIGH | ? | state.db | 0 | Permissions 644 — should be 600 |
| HIGH | ? | openapi.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | config.example.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | bybit-ws.service | 0 | NoNewPrivileges= not set |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | dspy_optimizer.py | 84 |
| M | ? | optuna_tuner.py | 431 |
| M | ? | optuna_tuner.py | 431 |
| H | ? | bybit_ws_sdk.py | 38 |
| H | ? | bybit_ws_sdk.py | 43 |
| H | ? | dspy_optimizer.py | 404 |
| H | ? | rl_agent.py | 139 |
| H | ? | lstm_regime.py | 527 |
| H | ? | dspy_optimizer.py | 405 |
| M | ? | rpc.py | 59 |
| L | GS003 | adversarial_env.py | 181 |
| L | GS003 | adversarial_env.py | 182 |
| L | GS003 | adversarial_env.py | 185 |
| L | GS003 | alerts.py | 57 |
| L | GS003 | backtest.py | 51 |
| L | GS003 | backtest.py | 203 |
| L | GS003 | backtest.py | 208 |
| L | GS003 | backtest.py | 209 |
| L | GS003 | backtest.py | 211 |
| L | GS003 | backtest.py | 213 |
| L | GS003 | alerts.py | 57 |
| L | GS003 | backtest.py | 51 |
| L | GS003 | backtest.py | 203 |
| L | GS003 | backtest.py | 208 |
| L | GS003 | backtest.py | 209 |
| L | GS003 | backtest.py | 211 |
| L | GS003 | backtest.py | 213 |
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
| L | GS003 | dspy_optimizer.py | 256 |
| L | GS003 | dspy_optimizer.py | 265 |
| L | GS003 | dspy_optimizer.py | 274 |
| L | GS003 | dspy_optimizer.py | 281 |
| L | GS003 | dspy_optimizer.py | 295 |
| L | GS003 | dspy_optimizer.py | 303 |
| L | GS003 | dspy_optimizer.py | 321 |
| L | GS003 | dspy_optimizer.py | 583 |
| L | GS003 | dspy_optimizer.py | 611 |
| L | GS003 | dspy_optimizer.py | 613 |
| L | GS003 | dspy_optimizer.py | 616 |
| L | GS003 | dspy_optimizer.py | 617 |
| L | GS003 | dspy_optimizer.py | 619 |
| L | GS003 | dspy_optimizer.py | 620 |
| L | GS003 | dspy_optimizer.py | 622 |
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
| L | GS003 | gridsignal-bot.py | 2471 |
| L | GS003 | gridsignal-bot.py | 2526 |
| L | GS003 | gridsignal_scanner.py | 751 |
| L | GS003 | gridsignal_scanner.py | 753 |
| L | GS003 | gridsignal_scanner.py | 755 |
| L | GS003 | gridsignal_scanner.py | 757 |
| L | GS003 | lstm_regime.py | 61 |
| L | GS003 | lstm_regime.py | 430 |
| L | GS003 | lstm_regime.py | 434 |
| L | GS003 | lstm_regime.py | 437 |
| L | GS003 | lstm_regime.py | 439 |
| L | GS003 | lstm_regime.py | 441 |
| L | GS003 | lstm_regime.py | 444 |
| L | GS003 | lstm_regime.py | 446 |
| L | GS003 | lstm_regime.py | 452 |
| L | GS003 | lstm_regime.py | 455 |
| L | GS003 | lstm_regime.py | 485 |
| L | GS003 | lstm_regime.py | 521 |
| L | GS003 | lstm_regime.py | 522 |
| L | GS003 | lstm_regime.py | 550 |
| L | GS003 | lstm_regime.py | 552 |
| L | GS003 | lstm_regime.py | 598 |
| L | GS003 | lstm_regime.py | 605 |
| L | GS003 | lstm_regime.py | 645 |
| L | GS003 | lstm_regime.py | 690 |
| L | GS003 | lstm_regime.py | 790 |
| L | GS003 | lstm_regime.py | 794 |
| L | GS003 | lstm_regime.py | 796 |
| L | GS003 | lstm_regime.py | 801 |
| L | GS003 | lstm_regime.py | 804 |
| L | GS003 | lstm_regime.py | 806 |
| L | GS003 | lstm_regime.py | 808 |
| L | GS003 | main.py | 188 |
| L | GS003 | main.py | 476 |
| L | GS003 | main.py | 478 |
| L | GS003 | main.py | 479 |
| L | GS003 | main.py | 480 |
| L | GS003 | main.py | 481 |
| L | GS003 | main.py | 963 |
| L | GS003 | main.py | 964 |
| L | GS003 | main.py | 966 |
| L | GS003 | main.py | 967 |
| L | GS003 | main.py | 972 |
| L | GS003 | main.py | 998 |
| L | GS003 | main.py | 1062 |
| L | GS003 | main.py | 1070 |
| L | GS003 | main.py | 1077 |
| L | GS003 | main.py | 1083 |
| L | GS003 | main.py | 1093 |
| L | GS003 | main.py | 1114 |
| L | GS003 | main.py | 1116 |
| L | GS003 | main.py | 1130 |
| L | GS003 | main.py | 1132 |
| L | GS003 | main.py | 1134 |
| L | GS003 | main_async.py | 339 |
| L | GS003 | main_async.py | 349 |
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
| L | GS003 | metrics.py | 91 |
| L | GS003 | metrics.py | 92 |
| L | GS003 | metrics.py | 93 |
| L | GS003 | metrics.py | 94 |
| L | GS003 | metrics.py | 100 |
| L | GS003 | metrics.py | 102 |
| L | GS003 | metrics.py | 104 |
| L | GS003 | metrics.py | 105 |
| L | GS003 | metrics.py | 108 |
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
| L | GS003 | optuna_tuner.py | 89 |
| L | GS003 | optuna_tuner.py | 272 |
| L | GS003 | optuna_tuner.py | 276 |
| L | GS003 | optuna_tuner.py | 278 |
| L | GS003 | optuna_tuner.py | 302 |
| L | GS003 | optuna_tuner.py | 309 |
| L | GS003 | optuna_tuner.py | 311 |
| L | GS003 | optuna_tuner.py | 314 |
| L | GS003 | optuna_tuner.py | 359 |
| L | GS003 | optuna_tuner.py | 381 |
| L | GS003 | optuna_tuner.py | 394 |
| L | GS003 | optuna_tuner.py | 396 |
| L | GS003 | optuna_tuner.py | 398 |
| L | GS003 | optuna_tuner.py | 428 |
| L | GS003 | partial_tp.py | 248 |
| L | GS003 | partial_tp.py | 250 |
| L | GS003 | push_notifier.py | 180 |
| L | GS003 | push_notifier.py | 186 |
| L | GS003 | push_notifier.py | 189 |
| L | GS003 | push_notifier.py | 192 |
| L | GS003 | push_notifier.py | 280 |
| L | GS003 | push_notifier.py | 283 |
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
| L | GS003 | ensemble.py | 261 |
| L | GS003 | ensemble.py | 262 |
| L | GS003 | ensemble.py | 264 |
| L | GS003 | ensemble.py | 265 |
| L | GS003 | ensemble.py | 268 |
| L | GS003 | ensemble.py | 270 |
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
| L | GS003 | gridsignal-bot.py | 2471 |
| L | GS003 | gridsignal-bot.py | 2526 |
| L | GS003 | gridsignal_scanner.py | 751 |
| L | GS003 | gridsignal_scanner.py | 753 |
| L | GS003 | gridsignal_scanner.py | 755 |
| L | GS003 | gridsignal_scanner.py | 757 |
| L | GS003 | lstm_regime.py | 61 |
| L | GS003 | lstm_regime.py | 430 |
| L | GS003 | lstm_regime.py | 434 |
| L | GS003 | lstm_regime.py | 437 |
| L | GS003 | lstm_regime.py | 439 |
| L | GS003 | lstm_regime.py | 441 |
| L | GS003 | lstm_regime.py | 444 |
| L | GS003 | lstm_regime.py | 446 |
| L | GS003 | lstm_regime.py | 452 |
| L | GS003 | lstm_regime.py | 455 |
| L | GS003 | lstm_regime.py | 485 |
| L | GS003 | lstm_regime.py | 521 |
| L | GS003 | lstm_regime.py | 522 |
| L | GS003 | lstm_regime.py | 550 |
| L | GS003 | lstm_regime.py | 552 |
| L | GS003 | lstm_regime.py | 598 |
| L | GS003 | lstm_regime.py | 605 |
| L | GS003 | lstm_regime.py | 645 |
| L | GS003 | lstm_regime.py | 690 |
| L | GS003 | lstm_regime.py | 790 |
| L | GS003 | lstm_regime.py | 794 |
| L | GS003 | lstm_regime.py | 796 |
| L | GS003 | lstm_regime.py | 801 |
| L | GS003 | lstm_regime.py | 804 |
| L | GS003 | lstm_regime.py | 806 |
| L | GS003 | lstm_regime.py | 808 |
| L | GS003 | main.py | 188 |
| L | GS003 | main.py | 476 |
| L | GS003 | main.py | 478 |
| L | GS003 | main.py | 479 |
| L | GS003 | main.py | 480 |
| L | GS003 | main.py | 481 |
| L | GS003 | main.py | 963 |
| L | GS003 | main.py | 964 |
| L | GS003 | main.py | 966 |
| L | GS003 | main.py | 967 |
| L | GS003 | main.py | 972 |
| L | GS003 | main.py | 998 |
| L | GS003 | main.py | 1062 |
| L | GS003 | main.py | 1070 |
| L | GS003 | main.py | 1077 |
| L | GS003 | main.py | 1083 |
| L | GS003 | main.py | 1093 |
| L | GS003 | main.py | 1114 |
| L | GS003 | main.py | 1116 |
| L | GS003 | main.py | 1130 |
| L | GS003 | main.py | 1132 |
| L | GS003 | main.py | 1134 |
| L | GS003 | main_async.py | 307 |
| L | GS003 | main_async.py | 317 |
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
| L | GS003 | metrics.py | 91 |
| L | GS003 | metrics.py | 92 |
| L | GS003 | metrics.py | 93 |
| L | GS003 | metrics.py | 94 |
| L | GS003 | metrics.py | 100 |
| L | GS003 | metrics.py | 102 |
| L | GS003 | metrics.py | 104 |
| L | GS003 | metrics.py | 105 |
| L | GS003 | metrics.py | 108 |
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
| L | GS003 | optuna_tuner.py | 89 |
| L | GS003 | optuna_tuner.py | 272 |
| L | GS003 | optuna_tuner.py | 276 |
| L | GS003 | optuna_tuner.py | 278 |
| L | GS003 | optuna_tuner.py | 302 |
| L | GS003 | optuna_tuner.py | 309 |
| L | GS003 | optuna_tuner.py | 311 |
| L | GS003 | optuna_tuner.py | 314 |
| L | GS003 | optuna_tuner.py | 359 |
| L | GS003 | optuna_tuner.py | 381 |
| L | GS003 | optuna_tuner.py | 394 |
| L | GS003 | optuna_tuner.py | 396 |
| L | GS003 | optuna_tuner.py | 398 |
| L | GS003 | optuna_tuner.py | 428 |
| L | GS003 | partial_tp.py | 248 |
| L | GS003 | partial_tp.py | 250 |
| L | GS003 | push_notifier.py | 185 |
| L | GS003 | push_notifier.py | 191 |
| L | GS003 | push_notifier.py | 194 |
| L | GS003 | push_notifier.py | 197 |
| L | GS003 | push_notifier.py | 285 |
| L | GS003 | push_notifier.py | 288 |
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
| L | GS003 | walkforward_rf.py | 21 |
| L | GS003 | walkforward_rf.py | 76 |
| L | GS003 | walkforward_rf.py | 96 |
| L | GS003 | walkforward_rf.py | 128 |
| L | GS003 | walkforward_rf.py | 131 |
| L | GS003 | walkforward_rf.py | 133 |
| L | GS003 | walkforward_rf.py | 139 |
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
| H | ? | main_async.py | 390 |
| H | ? | main_async.py | 391 |
| H | ? | main_async.py | 358 |
| H | ? | main_async.py | 359 |
| H | ? | config.py | 135 |
| H | ? | docker-entrypoint.sh | 16 |
| H | ? | docker-entrypoint.sh | 17 |
| H | ? | rpc.py | 95 |
| H | ? | rpc.py | 299 |
| H | ? | rpc.py | 451 |
| H | ? | rpc.py | 605 |
| H | ? | rpc.py | 1568 |
| H | ? | dashboard.html | 125 |
| H | ? | proxy_server.py | 6 |
| H | ? | proxy_server.py | 96 |
| H | ? | mcp_server.py | 28 |
| H | ? | config.example.yaml | 412 |
| H | ? | bybit_ws_sdk.py | 38 |
| H | ? | bybit_ws_sdk.py | 43 |
| H | ? | lstm_regime.py | 508 |
| H | ? | lstm_regime.py | 601 |
| L | ? | lstm_regime.py | 618 |
| M | ? | bybit-ws-async.service | 8 |
| M | ? | bybit-ws.service | 9 |
| H | ? | state.db | 0 |
| H | ? | openapi.yaml | 0 |
| H | ? | config.example.yaml | 0 |
| H | ? | docker-compose.yml | 0 |
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
| C | GS005 | dspy_optimizer.py | 83 |
| C | GS005 | dspy_optimizer.py | 83 |
| M | ? | optuna_tuner.py | 64 |
| M | ? | optuna_tuner.py | 64 |
| M | ? | backtest.py | 26 |
| M | ? | main.py | 135 |
| M | ? | gridsignal-bot.py | 1341 |
| M | ? | gridsignal-bot.py | 1343 |
| M | ? | gridsignal-bot.py | 1442 |
| M | ? | gridsignal-bot.py | 1444 |
| M | ? | gridsignal-bot.py | 1534 |
| M | ? | gridsignal-bot.py | 2099 |
| M | ? | mcp_server.py | 55 |
| M | ? | mcp_server.py | 70 |
| M | ? | mcp_server.py | 88 |
| M | ? | gridsignal_scanner.py | 46 |

---
*Сгенерировано GSC v0.6 · 2026-06-27T14:16:08.039123*