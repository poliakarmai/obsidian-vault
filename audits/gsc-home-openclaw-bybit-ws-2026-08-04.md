---
title: "GSC Audit: /home/openclaw/bybit-ws"
date: 2026-08-04
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/bybit-ws

**Дата:** 04.08.2026 22:27  
**Путь:** `/home/openclaw/bybit-ws`  
**Всего находок:** 1647  
**CRITICAL:** 122 | **HIGH:** 127 | **MEDIUM:** 34 | **LOW:** 642

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 584 |
| GS003 | 563 |
| GS001 | 120 |
| GS018 | 74 |
| GS008 | 65 |
| GS021 | 63 |
| GS020 | 54 |
| GS007 | 34 |
| Хардкод IP адреса | 15 |
| Синхронный код в async | 14 |
| CVE-2026-37270: Hardcoded credential | 9 |
| Python: File upload without content-type validation | 5 |
| eval() or exec() usage | 5 |
| CVE-2026-55223: Insecure deserialization | 4 |
| pickle.load() — unsafe deserialization | 4 |
| Python: SSRF via requests without URL validation | 2 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 2 |
| GS015 | 2 |
| User-controlled URL in request | 2 |
| Systemd: RestrictSUIDSGID= not set | 2 |
| GS012 | 2 |
| SQL injection risk: f-string in query | 1 |
| Python: assert in production | 1 |
| Python: CORS misconfiguration — allow all origins | 1 |
| CVE-2026-55721: SQL injection | 1 |
| CVE-2026-56318: Information disclosure | 1 |
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
| GS009 | 1 |
| GS017 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | dspy_optimizer.py | 84 | OWASP A03: Injection |
| CRITICAL | ? | dspy_optimizer.py | 84 |  |
| CRITICAL | GS001 | manifest.json | 49 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 50 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 79 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 80 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 104 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 105 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 134 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 135 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 194 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 195 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 199 | Found: "bb99ea1c68a69d471092864992cf8e7e" |
| CRITICAL | GS001 | manifest.json | 200 | Found: "bb99ea1c68a69d471092864992cf8e7e" |
| CRITICAL | GS001 | manifest.json | 214 | Found: "db89d498366178e38bb452334f1d2a38" |
| CRITICAL | GS001 | manifest.json | 215 | Found: "db89d498366178e38bb452334f1d2a38" |
| CRITICAL | GS001 | manifest.json | 229 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 230 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 329 | Found: "cb2430ec4b172e2c0bc58e1bc8140f5e" |
| CRITICAL | GS001 | manifest.json | 330 | Found: "cb2430ec4b172e2c0bc58e1bc8140f5e" |
| CRITICAL | GS001 | manifest.json | 334 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 335 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 404 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 405 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 409 | Found: "bb99ea1c68a69d471092864992cf8e7e" |
| CRITICAL | GS001 | manifest.json | 410 | Found: "bb99ea1c68a69d471092864992cf8e7e" |
| CRITICAL | GS001 | manifest.json | 424 | Found: "db89d498366178e38bb452334f1d2a38" |
| CRITICAL | GS001 | manifest.json | 425 | Found: "db89d498366178e38bb452334f1d2a38" |
| CRITICAL | GS001 | manifest.json | 439 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 440 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 539 | Found: "cb2430ec4b172e2c0bc58e1bc8140f5e" |
| CRITICAL | GS001 | manifest.json | 540 | Found: "cb2430ec4b172e2c0bc58e1bc8140f5e" |
| CRITICAL | GS001 | manifest.json | 544 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 545 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 49 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 50 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 79 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 80 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 104 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 105 | Found: "ad157b1cc9e437e59adb268582fade28" |
| CRITICAL | GS001 | manifest.json | 134 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 135 | Found: "bc96c8a3cef71f9543e23ba5487004b8" |
| CRITICAL | GS001 | manifest.json | 194 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 195 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 229 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 230 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 284 | Found: "ab87b1540e3191445b33b783035f8911" |
| CRITICAL | GS001 | manifest.json | 285 | Found: "ab87b1540e3191445b33b783035f8911" |
| CRITICAL | GS001 | manifest.json | 314 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 315 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 334 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 335 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 404 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 405 | Found: "cb23926cfe99dc500832478c104bda95" |
| CRITICAL | GS001 | manifest.json | 439 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 440 | Found: "ee60af25e9619a6ca7f731b6a71e679c" |
| CRITICAL | GS001 | manifest.json | 494 | Found: "ab87b1540e3191445b33b783035f8911" |
| CRITICAL | GS001 | manifest.json | 495 | Found: "ab87b1540e3191445b33b783035f8911" |
| CRITICAL | GS001 | manifest.json | 524 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 525 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 544 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 545 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 549 | Found: "da85f599c96f647ab284064055a450e0" |
| CRITICAL | GS001 | manifest.json | 550 | Found: "da85f599c96f647ab284064055a450e0" |
| CRITICAL | GS001 | manifest.json | 574 | Found: "ed283e1273dfe8d3dbb83a87b93fb694" |
| CRITICAL | GS001 | manifest.json | 575 | Found: "ed283e1273dfe8d3dbb83a87b93fb694" |
| CRITICAL | GS001 | manifest.json | 664 | Found: "ca982f9724487d9011519c673de18eb2" |
| CRITICAL | GS001 | manifest.json | 665 | Found: "ca982f9724487d9011519c673de18eb2" |
| CRITICAL | GS001 | manifest.json | 114 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 115 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 284 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 285 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 289 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 290 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 304 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 305 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 479 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 480 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 494 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 495 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 499 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 500 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 504 | Found: "da85f599c96f647ab284064055a450e0" |
| CRITICAL | GS001 | manifest.json | 505 | Found: "da85f599c96f647ab284064055a450e0" |
| CRITICAL | GS001 | manifest.json | 549 | Found: "ea92ee30f8cbd8b180839b51931acd03" |
| CRITICAL | GS001 | manifest.json | 550 | Found: "ea92ee30f8cbd8b180839b51931acd03" |
| CRITICAL | GS001 | manifest.json | 619 | Found: "ca982f9724487d9011519c673de18eb2" |
| CRITICAL | GS001 | manifest.json | 620 | Found: "ca982f9724487d9011519c673de18eb2" |
| CRITICAL | GS001 | manifest.json | 794 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 795 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 879 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 880 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 914 | Found: "ce32b2ac1805547f5d87fa6cc078fb21" |
| CRITICAL | GS001 | manifest.json | 959 | Found: "ef7874ae68816c6dc914693f04f1483d" |
| CRITICAL | GS001 | manifest.json | 984 | Found: "dd7903c49acd41a05c8365850c8ecba1" |
| CRITICAL | GS001 | manifest.json | 114 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 115 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 284 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 285 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 289 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 290 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 304 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 305 | Found: "fc15d27848c8e94ceaff7ebd99c44810" |
| CRITICAL | GS001 | manifest.json | 479 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 480 | Found: "be40e21a48377af8677d645d6a829513" |
| CRITICAL | GS001 | manifest.json | 494 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 495 | Found: "af506c0d20e4cda6ec782b783b74f439" |
| CRITICAL | GS001 | manifest.json | 499 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 500 | Found: "ed29c082f028e247224cf292cfcb7269" |
| CRITICAL | GS001 | manifest.json | 504 | Found: "da85f599c96f647ab284064055a450e0" |
| CRITICAL | GS001 | manifest.json | 505 | Found: "da85f599c96f647ab284064055a450e0" |
| CRITICAL | GS001 | manifest.json | 549 | Found: "ea92ee30f8cbd8b180839b51931acd03" |
| CRITICAL | GS001 | manifest.json | 550 | Found: "ea92ee30f8cbd8b180839b51931acd03" |
| CRITICAL | GS001 | manifest.json | 619 | Found: "ca982f9724487d9011519c673de18eb2" |
| CRITICAL | GS001 | manifest.json | 620 | Found: "ca982f9724487d9011519c673de18eb2" |
| CRITICAL | GS001 | manifest.json | 794 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 795 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 879 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 880 | Found: "bd6211bae177dbfb0913baf09284b09e" |
| CRITICAL | GS001 | manifest.json | 914 | Found: "ce32b2ac1805547f5d87fa6cc078fb21" |
| CRITICAL | GS001 | manifest.json | 959 | Found: "ef7874ae68816c6dc914693f04f1483d" |
| CRITICAL | GS001 | manifest.json | 984 | Found: "dd7903c49acd41a05c8365850c8ecba1" |
| HIGH | ? | bybit_ws_sdk.py | 38 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | bybit_ws_sdk.py | 43 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | lstm_regime.py | 531 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | rl_agent.py | 139 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | lstm_world_model.py | 417 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | lstm_world_model.py | 439 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | dspy_optimizer.py | 405 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | bybit_ws_sdk.py | 38 |  |
| HIGH | ? | bybit_ws_sdk.py | 43 |  |
| HIGH | ? | docker-entrypoint.sh | 16 | Match: echo "   RPC: http://0.0.0.0:8766" |
| HIGH | ? | docker-entrypoint.sh | 17 | Match: echo "   Health: http://0.0.0.0:8766/health" |
| HIGH | ? | config.py | 135 | Match:     'bind': '127.0.0.1',      # default to localhost; |
| HIGH | ? | main_async.py | 661 | Match:         ws_push_thread = start_ws_server(port=8768, b |
| HIGH | ? | main_async.py | 662 | Match:         log_event('📡 WebSocket push server on 127.0.0 |
| HIGH | ? | config.example.yaml | 412 | Match:   rpc_bind: "127.0.0.1" |
| HIGH | ? | proxy_server.py | 6 | Match: RPC = 'http://127.0.0.1:8766' |
| HIGH | ? | proxy_server.py | 96 | Match:     HTTPServer(('127.0.0.1', 9999), P).serve_forever( |
| HIGH | ? | dashboard.html | 126 | Match: const WS_URL = 'ws://127.0.0.1:8767/ws'; |
| HIGH | ? | mcp_server.py | 28 | Match: RPC_BASE = f"http://127.0.0.1:{RPC_PORT}" |
| HIGH | ? | rpc.py | 95 | Match: def start_ws_server(port=8767, bind='127.0.0.1'): |
| HIGH | ? | rpc.py | 300 | Match:     handler.send_header("Access-Control-Allow-Origin" |
| HIGH | ? | rpc.py | 465 | Match:         self.send_header("Access-Control-Allow-Origin |
| HIGH | ? | rpc.py | 648 | Match:             "rpc_host": "127.0.0.1", |
| HIGH | ? | rpc.py | 1765 | Match: def start_rpc_server(port=8766, bind='127.0.0.1'): |
| HIGH | ? | bybit_ws_sdk.py | 38 | Match:         r = requests.get(f"{self.base_url}{path}", ti |
| HIGH | ? | bybit_ws_sdk.py | 43 | Match:         r = requests.post(f"{self.base_url}{path}", j |
| HIGH | ? | lstm_regime.py | 512 | Match:         model.eval() |
| HIGH | ? | lstm_regime.py | 605 | Match:         model.eval() |
| HIGH | ? | lstm_world_model.py | 402 | Match:         model.eval() |
| HIGH | ? | lstm_world_model.py | 467 | Match:     model.eval() |
| HIGH | ? | lstm_world_model.py | 565 | Match:     model.eval() |
| HIGH | ? | state.db | 0 | Permissions 644 — should be 600 |
| HIGH | ? | openapi.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | config.example.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
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
| HIGH | GS017 | config.example.yaml | 33 | Password variable with short value (19 chars). |
| HIGH | GS018 | api.py | 401 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | api.py | 301 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_entry.py | 626 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 384 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 504 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | auto_short.py | 762 | Float arithmetic for money leads to rounding errors exploita |
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
| HIGH | GS018 | rpc.py | 905 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 1529 | Float arithmetic for money leads to rounding errors exploita |
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
| HIGH | GS018 | rpc.py | 905 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | rpc.py | 1529 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ws_client.py | 300 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | ws_client.py | 302 | Float arithmetic for money leads to rounding errors exploita |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | dspy_optimizer.py | 84 |
| M | ? | optuna_tuner.py | 436 |
| H | ? | bybit_ws_sdk.py | 38 |
| H | ? | bybit_ws_sdk.py | 43 |
| H | ? | lstm_regime.py | 531 |
| H | ? | rl_agent.py | 139 |
| H | ? | lstm_world_model.py | 417 |
| H | ? | lstm_world_model.py | 439 |
| H | ? | dspy_optimizer.py | 405 |
| M | ? | rpc.py | 59 |
| M | ? | lstm_regime.py | 624 |
| M | ? | lstm_world_model.py | 292 |
| M | ? | lstm_world_model.py | 479 |
| M | ? | lstm_world_model.py | 571 |
| C | ? | dspy_optimizer.py | 84 |
| H | ? | bybit_ws_sdk.py | 38 |
| H | ? | bybit_ws_sdk.py | 43 |
| M | ? | gridsignal-bot.py | 1136 |
| M | ? | margin_alerts.py | 138 |
| M | ? | margin_alerts.py | 148 |
| M | ? | margin_alerts.py | 157 |
| M | ? | gridsignal-bot.py | 30 |
| M | ? | gridsignal-bot.py | 931 |
| M | ? | gridsignal-bot.py | 1136 |
| M | ? | proxy_server.py | 25 |
| M | ? | mcp_server.py | 39 |
| M | ? | rpc.py | 180 |
| C | GS001 | manifest.json | 49 |
| C | GS001 | manifest.json | 50 |
| C | GS001 | manifest.json | 79 |
| C | GS001 | manifest.json | 80 |
| C | GS001 | manifest.json | 104 |
| C | GS001 | manifest.json | 105 |
| C | GS001 | manifest.json | 134 |
| C | GS001 | manifest.json | 135 |
| C | GS001 | manifest.json | 194 |
| C | GS001 | manifest.json | 195 |
| C | GS001 | manifest.json | 199 |
| C | GS001 | manifest.json | 200 |
| C | GS001 | manifest.json | 214 |
| C | GS001 | manifest.json | 215 |
| C | GS001 | manifest.json | 229 |
| C | GS001 | manifest.json | 230 |
| C | GS001 | manifest.json | 329 |
| C | GS001 | manifest.json | 330 |
| C | GS001 | manifest.json | 334 |
| C | GS001 | manifest.json | 335 |
| C | GS001 | manifest.json | 404 |
| C | GS001 | manifest.json | 405 |
| C | GS001 | manifest.json | 409 |
| C | GS001 | manifest.json | 410 |
| C | GS001 | manifest.json | 424 |
| C | GS001 | manifest.json | 425 |
| C | GS001 | manifest.json | 439 |
| C | GS001 | manifest.json | 440 |
| C | GS001 | manifest.json | 539 |
| C | GS001 | manifest.json | 540 |
| C | GS001 | manifest.json | 544 |
| C | GS001 | manifest.json | 545 |
| C | GS001 | manifest.json | 49 |
| C | GS001 | manifest.json | 50 |
| C | GS001 | manifest.json | 79 |
| C | GS001 | manifest.json | 80 |
| C | GS001 | manifest.json | 104 |
| C | GS001 | manifest.json | 105 |
| C | GS001 | manifest.json | 134 |
| C | GS001 | manifest.json | 135 |
| C | GS001 | manifest.json | 194 |
| C | GS001 | manifest.json | 195 |
| C | GS001 | manifest.json | 229 |
| C | GS001 | manifest.json | 230 |
| C | GS001 | manifest.json | 284 |
| C | GS001 | manifest.json | 285 |
| C | GS001 | manifest.json | 314 |
| C | GS001 | manifest.json | 315 |
| C | GS001 | manifest.json | 334 |
| C | GS001 | manifest.json | 335 |
| C | GS001 | manifest.json | 404 |
| C | GS001 | manifest.json | 405 |
| C | GS001 | manifest.json | 439 |
| C | GS001 | manifest.json | 440 |
| C | GS001 | manifest.json | 494 |
| C | GS001 | manifest.json | 495 |
| C | GS001 | manifest.json | 524 |
| C | GS001 | manifest.json | 525 |
| C | GS001 | manifest.json | 544 |
| C | GS001 | manifest.json | 545 |
| C | GS001 | manifest.json | 549 |
| C | GS001 | manifest.json | 550 |
| C | GS001 | manifest.json | 574 |
| C | GS001 | manifest.json | 575 |
| C | GS001 | manifest.json | 664 |
| C | GS001 | manifest.json | 665 |
| C | GS001 | manifest.json | 114 |
| C | GS001 | manifest.json | 115 |
| C | GS001 | manifest.json | 284 |
| C | GS001 | manifest.json | 285 |
| C | GS001 | manifest.json | 289 |
| C | GS001 | manifest.json | 290 |
| C | GS001 | manifest.json | 304 |
| C | GS001 | manifest.json | 305 |
| C | GS001 | manifest.json | 479 |
| C | GS001 | manifest.json | 480 |
| C | GS001 | manifest.json | 494 |
| C | GS001 | manifest.json | 495 |
| C | GS001 | manifest.json | 499 |
| C | GS001 | manifest.json | 500 |
| C | GS001 | manifest.json | 504 |
| C | GS001 | manifest.json | 505 |
| C | GS001 | manifest.json | 549 |
| C | GS001 | manifest.json | 550 |
| C | GS001 | manifest.json | 619 |
| C | GS001 | manifest.json | 620 |
| C | GS001 | manifest.json | 794 |
| C | GS001 | manifest.json | 795 |
| C | GS001 | manifest.json | 879 |
| C | GS001 | manifest.json | 880 |
| C | GS001 | manifest.json | 914 |
| C | GS001 | manifest.json | 959 |
| C | GS001 | manifest.json | 984 |
| C | GS001 | manifest.json | 114 |
| C | GS001 | manifest.json | 115 |
| C | GS001 | manifest.json | 284 |
| C | GS001 | manifest.json | 285 |
| C | GS001 | manifest.json | 289 |
| C | GS001 | manifest.json | 290 |
| C | GS001 | manifest.json | 304 |
| C | GS001 | manifest.json | 305 |
| C | GS001 | manifest.json | 479 |
| C | GS001 | manifest.json | 480 |
| C | GS001 | manifest.json | 494 |
| C | GS001 | manifest.json | 495 |
| C | GS001 | manifest.json | 499 |
| C | GS001 | manifest.json | 500 |
| C | GS001 | manifest.json | 504 |
| C | GS001 | manifest.json | 505 |
| C | GS001 | manifest.json | 549 |
| C | GS001 | manifest.json | 550 |
| C | GS001 | manifest.json | 619 |
| C | GS001 | manifest.json | 620 |
| C | GS001 | manifest.json | 794 |
| C | GS001 | manifest.json | 795 |
| C | GS001 | manifest.json | 879 |
| C | GS001 | manifest.json | 880 |
| C | GS001 | manifest.json | 914 |
| C | GS001 | manifest.json | 959 |
| C | GS001 | manifest.json | 984 |
| L | GS003 | adversarial_env.py | 181 |
| L | GS003 | adversarial_env.py | 182 |
| L | GS003 | adversarial_env.py | 185 |
| L | GS003 | alerts.py | 57 |
| L | GS003 | alerts.py | 63 |
| L | GS003 | alerts.py | 64 |
| L | GS003 | adversarial_env.py | 181 |
| L | GS003 | adversarial_env.py | 182 |
| L | GS003 | adversarial_env.py | 185 |
| L | GS003 | alerts.py | 57 |
| L | GS003 | alerts.py | 63 |
| L | GS003 | alerts.py | 64 |
| L | GS003 | backtest.py | 398 |
| L | GS003 | backtest.py | 404 |
| L | GS003 | backtest.py | 406 |
| L | GS003 | backtest.py | 407 |
| L | GS003 | backtest.py | 408 |
| L | GS003 | backtest.py | 409 |
| L | GS003 | backtest.py | 410 |
| L | GS003 | backtest.py | 411 |
| L | GS003 | backtest.py | 412 |
| L | GS003 | backtest.py | 413 |
| L | GS003 | backtest.py | 414 |
| L | GS003 | backtest.py | 415 |
| L | GS003 | backtest.py | 416 |
| L | GS003 | backtest.py | 417 |
| L | GS003 | backtest.py | 418 |
| L | GS003 | backtest.py | 419 |
| L | GS003 | backtest.py | 420 |
| L | GS003 | backtest.py | 421 |
| L | GS003 | backtest.py | 424 |
| L | GS003 | backtest.py | 425 |
| L | GS003 | backtest.py | 426 |
| L | GS003 | backtest.py | 427 |
| L | GS003 | backtest.py | 428 |
| L | GS003 | backtest.py | 429 |
| L | GS003 | backtest.py | 430 |
| L | GS003 | backtest.py | 431 |
| L | GS003 | backtest.py | 432 |
| L | GS003 | backtest.py | 433 |
| L | GS003 | backtest.py | 434 |
| L | GS003 | backtest.py | 436 |
| L | GS003 | backtest.py | 438 |
| L | GS003 | backtest.py | 439 |
| L | GS003 | backtest.py | 457 |
| L | GS003 | backtest.py | 461 |
| L | GS003 | backtest.py | 463 |
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
| L | GS008 | auto_entry.py | 34 |
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
| L | GS008 | self_learn.py | 57 |
| L | GS008 | self_learn.py | 65 |
| L | GS008 | mean_revert.py | 26 |
| L | GS008 | optimize_params.py | 24 |
| L | GS008 | optimize_params.py | 28 |
| L | GS008 | paper_trade.py | 34 |
| L | GS008 | post_trade.py | 20 |
| L | GS008 | pump_detect.py | 33 |
| L | GS008 | pump_detect.py | 38 |
| L | GS008 | regime.py | 289 |
| L | GS008 | regime.py | 299 |
| L | GS008 | regime.py | 309 |
| L | GS008 | rl_env.py | 40 |
| L | GS008 | rpc.py | 116 |
| L | GS008 | session_params.py | 50 |
| L | GS008 | utils.py | 68 |
| L | GS008 | utils.py | 69 |
| L | GS008 | utils.py | 70 |
| L | GS008 | utils.py | 71 |
| L | GS008 | utils.py | 72 |
| L | GS008 | ws_client.py | 96 |
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
| I | GS015 | main.py | 1 |
| i | GS020 |  | 194 |
| i | GS020 |  | 263 |
| i | GS020 |  | 307 |
| i | GS020 |  | 324 |
| i | GS020 |  | 337 |
| i | GS020 |  | 135 |
| i | GS020 |  | 184 |
| i | GS020 |  | 192 |
| i | GS020 |  | 267 |
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
| i | GS020 |  | 95 |
| i | GS020 |  | 97 |
| i | GS020 |  | 229 |
| i | GS020 |  | 977 |
| H | ? | docker-entrypoint.sh | 16 |
| H | ? | docker-entrypoint.sh | 17 |
| H | ? | config.py | 135 |
| H | ? | main_async.py | 661 |
| H | ? | main_async.py | 662 |
| H | ? | config.example.yaml | 412 |
| H | ? | proxy_server.py | 6 |
| H | ? | proxy_server.py | 96 |
| H | ? | dashboard.html | 126 |
| H | ? | mcp_server.py | 28 |
| H | ? | rpc.py | 95 |
| H | ? | rpc.py | 300 |
| H | ? | rpc.py | 465 |
| H | ? | rpc.py | 648 |
| H | ? | rpc.py | 1765 |
| H | ? | bybit_ws_sdk.py | 38 |
| H | ? | bybit_ws_sdk.py | 43 |
| H | ? | lstm_regime.py | 512 |
| H | ? | lstm_regime.py | 605 |
| H | ? | lstm_world_model.py | 402 |
| H | ? | lstm_world_model.py | 467 |
| H | ? | lstm_world_model.py | 565 |
| L | ? | lstm_regime.py | 624 |
| L | ? | lstm_world_model.py | 292 |
| L | ? | lstm_world_model.py | 479 |
| L | ? | lstm_world_model.py | 571 |
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
| L | GS012 | dspy_optimizer.py | 402 |
| L | GS012 | dspy_optimizer.py | 402 |
| H | GS017 | config.example.yaml | 33 |
| H | GS018 | api.py | 401 |
| H | GS018 | api.py | 301 |
| H | GS018 | auto_entry.py | 626 |
| H | GS018 | auto_short.py | 384 |
| H | GS018 | auto_short.py | 504 |
| H | GS018 | auto_short.py | 762 |
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
| H | GS018 | rpc.py | 905 |
| H | GS018 | rpc.py | 1529 |
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
| s | GS021 |  | 6 |
| s | GS021 |  | 96 |
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
| r | GS022 |  | 689 |
| r | GS022 |  | 690 |
| r | GS022 |  | 763 |
| r | GS022 |  | 764 |
| r | GS022 |  | 689 |
| r | GS022 |  | 690 |
| r | GS022 |  | 763 |
| r | GS022 |  | 764 |
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
*Сгенерировано GSC v0.6 · 2026-08-04T22:27:42.101380*