---
title: "GSC Audit: /tmp/gsc-learn/aiohttp"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/aiohttp

**Дата:** 08.08.2026 04:03  
**Путь:** `/tmp/gsc-learn/aiohttp`  
**Всего находок:** 573  
**CRITICAL:** 0 | **HIGH:** 10 | **MEDIUM:** 157 | **LOW:** 271

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 241 |
| GS018 | 152 |
| GS021 | 65 |
| GS022 | 44 |
| GS003 | 19 |
| GS020 | 17 |
| GS008 | 16 |
| GS025 | 4 |
| GS007 | 3 |
| GS025-hardcoded_secret | 3 |
| GS025-debug_mode | 3 |
| GS004 | 1 |
| GS009 | 1 |
| GS012 | 1 |
| GS025-wildcard_bind | 1 |
| GS025-eval_usage | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS000-LEGACY | web_runner.py | 170 | Match:         host = "0.0.0.0" if not self._host else self. |
| HIGH | GS008 | gen.py | 18 | Match:     exec(code, globs) |
| HIGH | GS025 | .codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .lgtm.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | gen.py | 18 | Line 18: exec(code, globs) |
| HIGH | GS007 | web_exceptions.py | 327 | Line 327: self._method = method |
| HIGH | GS007 | web_request.py | 156 | Line 156: self._method = message.method |
| HIGH | GS007 | web_urldispatcher.py | 179 | Line 179: self._method = method |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| L | GS000-LEGACY | web_server.py | 42 |
| L | GS000-LEGACY | client_proto.py | 143 |
| L | GS000-LEGACY | web.py | 291 |
| L | GS000-LEGACY | compression_utils.py | 28 |
| M | GS018 | http_writer.py | 146 |
| M | GS018 | http_writer.py | 245 |
| M | GS018 | http_writer.py | 263 |
| M | GS018 | http_writer.py | 294 |
| M | GS018 | helpers.py | 730 |
| M | GS018 | helpers.py | 835 |
| M | GS018 | helpers.py | 844 |
| M | GS018 | payload.py | 162 |
| M | GS018 | cookiejar.py | 553 |
| M | GS018 | client_reqrep.py | 301 |
| M | GS018 | client_reqrep.py | 303 |
| M | GS018 | client_reqrep.py | 416 |
| M | GS018 | client_reqrep.py | 619 |
| M | GS018 | client_reqrep.py | 832 |
| M | GS018 | client_reqrep.py | 910 |
| M | GS018 | client_reqrep.py | 946 |
| M | GS018 | client_reqrep.py | 954 |
| M | GS018 | client_reqrep.py | 1014 |
| M | GS018 | client_reqrep.py | 1093 |
| M | GS018 | client_reqrep.py | 1100 |
| M | GS018 | client_reqrep.py | 1278 |
| M | GS018 | client_reqrep.py | 1490 |
| M | GS018 | web_protocol.py | 401 |
| M | GS018 | web_protocol.py | 448 |
| M | GS018 | web_protocol.py | 466 |
| M | GS018 | web_protocol.py | 576 |
| M | GS018 | web_protocol.py | 658 |
| M | GS018 | web_protocol.py | 661 |
| M | GS018 | web_protocol.py | 662 |
| M | GS018 | web_protocol.py | 821 |
| M | GS018 | client_ws.py | 128 |
| M | GS018 | client_ws.py | 146 |
| M | GS018 | client_ws.py | 324 |
| M | GS018 | http_parser.py | 304 |
| M | GS018 | http_parser.py | 421 |
| M | GS018 | http_parser.py | 458 |
| M | GS018 | http_parser.py | 529 |
| M | GS018 | http_parser.py | 534 |
| M | GS018 | http_parser.py | 535 |
| M | GS018 | http_parser.py | 1202 |
| M | GS018 | client.py | 236 |
| M | GS018 | client.py | 242 |
| M | GS018 | client.py | 335 |
| M | GS018 | client.py | 538 |
| M | GS018 | client.py | 1164 |
| M | GS018 | client.py | 1166 |
| M | GS018 | client.py | 1179 |
| M | GS018 | client.py | 1526 |
| M | GS018 | client_proto.py | 133 |
| M | GS018 | client_proto.py | 178 |
| M | GS018 | client_proto.py | 179 |
| M | GS018 | connector.py | 636 |
| M | GS018 | connector.py | 1421 |
| M | GS018 | connector.py | 1529 |
| M | GS018 | connector.py | 1536 |
| M | GS018 | connector.py | 1588 |
| M | GS018 | connector.py | 1620 |
| M | GS018 | web_app.py | 63 |
| M | GS018 | web_middlewares.py | 85 |
| M | GS018 | base_protocol.py | 53 |
| M | GS018 | base_protocol.py | 57 |
| M | GS018 | base_protocol.py | 70 |
| M | GS018 | multipart.py | 401 |
| M | GS018 | multipart.py | 411 |
| M | GS018 | multipart.py | 433 |
| M | GS018 | multipart.py | 693 |
| M | GS018 | multipart.py | 1017 |
| M | GS018 | multipart.py | 1063 |
| M | GS018 | multipart.py | 1148 |
| M | GS018 | multipart.py | 1149 |
| M | GS018 | multipart.py | 1239 |
| M | GS018 | web_request.py | 479 |
| M | GS018 | web_request.py | 892 |
| M | GS018 | web_request.py | 899 |
| M | GS018 | web_request.py | 905 |
| M | GS018 | web_request.py | 914 |
| M | GS018 | web_fileresponse.py | 129 |
| M | GS018 | web_fileresponse.py | 282 |
| M | GS018 | web_fileresponse.py | 402 |
| M | GS018 | streams.py | 253 |
| M | GS018 | streams.py | 286 |
| M | GS018 | streams.py | 372 |
| M | GS018 | streams.py | 731 |
| M | GS018 | web_ws.py | 151 |
| M | GS018 | web_ws.py | 173 |
| M | GS018 | web_ws.py | 194 |
| M | GS018 | web_ws.py | 265 |
| M | GS018 | web_ws.py | 385 |
| M | GS018 | web_ws.py | 524 |
| M | GS018 | web_ws.py | 536 |
| M | GS018 | web_ws.py | 540 |
| M | GS018 | web_ws.py | 541 |
| M | GS018 | web_response.py | 150 |
| M | GS018 | web_response.py | 244 |
| M | GS018 | web_response.py | 321 |
| M | GS018 | web_response.py | 322 |
| M | GS018 | web_response.py | 333 |
| M | GS018 | web_response.py | 374 |
| M | GS018 | web_response.py | 376 |
| M | GS018 | web_response.py | 437 |
| M | GS018 | web_response.py | 439 |
| M | GS018 | web_response.py | 452 |
| M | GS018 | web_response.py | 464 |
| M | GS018 | web_response.py | 465 |
| M | GS018 | web_response.py | 474 |
| M | GS018 | web_response.py | 481 |
| M | GS018 | web_response.py | 493 |
| M | GS018 | web_response.py | 647 |
| M | GS018 | web_response.py | 687 |
| M | GS018 | web_response.py | 688 |
| M | GS018 | web_response.py | 689 |
| M | GS018 | web_response.py | 731 |
| M | GS018 | client_middleware_digest_auth.py | 506 |
| M | GS018 | helpers.py | 44 |
| M | GS018 | helpers.py | 45 |
| M | GS018 | reader_py.py | 119 |
| M | GS018 | reader_py.py | 503 |
| M | GS018 | reader_py.py | 511 |
| M | GS018 | web_runner.py | 177 |
| M | GS018 | web_runner.py | 221 |
| M | GS018 | web_runner.py | 252 |
| M | GS018 | web_runner.py | 292 |
| M | GS018 | resolver.py | 83 |
| M | GS018 | resolver.py | 163 |
| M | GS018 | web_urldispatcher.py | 160 |
| M | GS018 | web_urldispatcher.py | 257 |
| M | GS018 | web_urldispatcher.py | 334 |
| M | GS018 | web_urldispatcher.py | 365 |
| M | GS018 | web_urldispatcher.py | 377 |
| M | GS018 | web_urldispatcher.py | 378 |
| M | GS018 | web_urldispatcher.py | 379 |
| M | GS018 | web_urldispatcher.py | 436 |
| M | GS018 | web_urldispatcher.py | 437 |
| M | GS018 | web_urldispatcher.py | 446 |
| M | GS018 | web_urldispatcher.py | 447 |
| M | GS018 | web_urldispatcher.py | 448 |
| M | GS018 | web_urldispatcher.py | 477 |
| M | GS018 | web_urldispatcher.py | 478 |
| M | GS018 | web_urldispatcher.py | 488 |
| M | GS018 | web_urldispatcher.py | 489 |
| M | GS018 | web_urldispatcher.py | 490 |
| M | GS018 | web_urldispatcher.py | 674 |
| M | GS018 | web_urldispatcher.py | 788 |
| M | GS018 | web_urldispatcher.py | 879 |
| M | GS018 | web_urldispatcher.py | 883 |
| M | GS018 | web_urldispatcher.py | 1041 |
| M | GS018 | web_urldispatcher.py | 1149 |
| M | GS018 | formdata.py | 154 |
| M | GS018 | worker.py | 104 |
| M | GS018 | worker.py | 106 |
| M | GS018 | worker.py | 146 |
| M | GS018 | check_sum.py | 18 |
| L | GS003 | client_reqrep.py | 471 |
| L | GS003 | client_reqrep.py | 475 |
| L | GS003 | web.py | 390 |
| L | GS003 | bench-asyncio-write.py | 99 |
| L | GS003 | bench-asyncio-write.py | 100 |
| L | GS003 | bench-asyncio-write.py | 121 |
| L | GS003 | check_changes.py | 34 |
| L | GS003 | check_changes.py | 44 |
| L | GS003 | check_changes.py | 45 |
| L | GS003 | check_changes.py | 49 |
| L | GS003 | check_changes.py | 50 |
| L | GS003 | check_changes.py | 51 |
| L | GS003 | check_changes.py | 53 |
| L | GS003 | check_sum.py | 22 |
| L | GS003 | check_sum.py | 33 |
| L | GS003 | check_sum.py | 42 |
| L | GS003 | check_sum.py | 45 |
| L | GS003 | cleanup_changes.py | 40 |
| L | GS003 | cleanup_changes.py | 41 |
| L | GS008 | helpers.py | 12 |
| L | GS008 | helpers.py | 13 |
| L | GS008 | helpers.py | 14 |
| L | GS008 | helpers.py | 15 |
| L | GS008 | helpers.py | 16 |
| L | GS008 | helpers.py | 17 |
| L | GS008 | helpers.py | 18 |
| L | GS008 | models.py | 151 |
| L | GS008 | models.py | 152 |
| L | GS008 | helpers.py | 69 |
| L | GS008 | helpers.py | 1132 |
| L | GS008 | helpers.py | 1133 |
| L | GS008 | http_websocket.py | 29 |
| L | GS008 | typedefs.py | 10 |
| L | GS008 | typedefs.py | 11 |
| i | GS020 |  | 472 |
| i | GS020 |  | 881 |
| i | GS020 |  | 884 |
| i | GS020 |  | 304 |
| i | GS020 |  | 56 |
| i | GS020 |  | 80 |
| i | GS020 |  | 168 |
| i | GS020 |  | 156 |
| i | GS020 |  | 620 |
| i | GS020 |  | 399 |
| i | GS020 |  | 472 |
| i | GS020 |  | 678 |
| i | GS020 |  | 697 |
| i | GS020 |  | 699 |
| i | GS020 |  | 700 |
| i | GS020 |  | 706 |
| i | GS020 |  | 696 |
| H | GS000-LEGACY | web_runner.py | 170 |
| M | GS000-LEGACY | sync-direct-runtime-deps.py | 2 |
| M | GS000-LEGACY | sync-direct-runtime-deps.py | 12 |
| M | GS000-LEGACY | sync-direct-runtime-deps.py | 20 |
| M | GS000-LEGACY | gen.py | 10 |
| H | GS008 | gen.py | 18 |
| H | GS025 | .codecov.yml | 0 |
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS025 | .readthedocs.yml | 0 |
| H | GS025 | .lgtm.yml | 0 |
| H | GS004 | gen.py | 18 |
| H | GS007 | web_exceptions.py | 327 |
| H | GS007 | web_request.py | 156 |
| H | GS007 | web_urldispatcher.py | 179 |
| s | GS009 |  | 0 |
| L | GS012 | _cookie_helpers.py | 185 |
| s | GS021 |  | 130 |
| s | GS021 |  | 131 |
| s | GS021 |  | 132 |
| s | GS021 |  | 418 |
| s | GS021 |  | 403 |
| s | GS021 |  | 170 |
| s | GS021 |  | 29 |
| s | GS021 |  | 30 |
| s | GS021 |  | 55 |
| s | GS021 |  | 134 |
| s | GS021 |  | 525 |
| s | GS021 |  | 569 |
| s | GS021 |  | 35 |
| s | GS021 |  | 100 |
| s | GS021 |  | 114 |
| s | GS021 |  | 120 |
| s | GS021 |  | 126 |
| s | GS021 |  | 132 |
| s | GS021 |  | 139 |
| s | GS021 |  | 147 |
| s | GS021 |  | 55 |
| s | GS021 |  | 67 |
| s | GS021 |  | 13 |
| s | GS021 |  | 256 |
| s | GS021 |  | 266 |
| s | GS021 |  | 272 |
| s | GS021 |  | 280 |
| s | GS021 |  | 291 |
| s | GS021 |  | 307 |
| s | GS021 |  | 317 |
| s | GS021 |  | 7 |
| s | GS021 |  | 13 |
| s | GS021 |  | 16 |
| s | GS021 |  | 250 |
| s | GS021 |  | 272 |
| s | GS021 |  | 281 |
| s | GS021 |  | 290 |
| s | GS021 |  | 294 |
| s | GS021 |  | 301 |
| s | GS021 |  | 13 |
| s | GS021 |  | 13 |
| s | GS021 |  | 64 |
| s | GS021 |  | 12 |
| s | GS021 |  | 13 |
| s | GS021 |  | 129 |
| s | GS021 |  | 143 |
| s | GS021 |  | 160 |
| s | GS021 |  | 170 |
| s | GS021 |  | 162 |
| s | GS021 |  | 179 |
| s | GS021 |  | 183 |
| s | GS021 |  | 191 |
| s | GS021 |  | 202 |
| s | GS021 |  | 210 |
| s | GS021 |  | 211 |
| s | GS021 |  | 219 |
| s | GS021 |  | 226 |
| s | GS021 |  | 21 |
| s | GS021 |  | 30 |
| s | GS021 |  | 22 |
| s | GS021 |  | 38 |
| s | GS021 |  | 32 |
| s | GS021 |  | 130 |
| s | GS021 |  | 130 |
| s | GS021 |  | 141 |
| r | GS022 |  | 172 |
| r | GS022 |  | 266 |
| r | GS022 |  | 271 |
| r | GS022 |  | 290 |
| r | GS022 |  | 186 |
| r | GS022 |  | 104 |
| r | GS022 |  | 109 |
| r | GS022 |  | 220 |
| r | GS022 |  | 325 |
| r | GS022 |  | 406 |
| r | GS022 |  | 422 |
| r | GS022 |  | 618 |
| r | GS022 |  | 407 |
| r | GS022 |  | 411 |
| r | GS022 |  | 509 |
| r | GS022 |  | 804 |
| r | GS022 |  | 843 |
| r | GS022 |  | 83 |
| r | GS022 |  | 264 |
| r | GS022 |  | 287 |
| r | GS022 |  | 694 |
| r | GS022 |  | 698 |
| r | GS022 |  | 333 |
| r | GS022 |  | 459 |
| r | GS022 |  | 460 |
| r | GS022 |  | 534 |
| r | GS022 |  | 561 |
| r | GS022 |  | 563 |
| r | GS022 |  | 612 |
| r | GS022 |  | 660 |
| r | GS022 |  | 809 |
| r | GS022 |  | 1383 |
| r | GS022 |  | 215 |
| r | GS022 |  | 277 |
| r | GS022 |  | 438 |
| r | GS022 |  | 275 |
| r | GS022 |  | 459 |
| r | GS022 |  | 462 |
| r | GS022 |  | 787 |
| r | GS022 |  | 234 |
| r | GS022 |  | 435 |
| r | GS022 |  | 10 |
| r | GS022 |  | 37 |
| r | GS022 |  | 44 |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| M | ? | cleanup_changes.py | 38 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:03:55.398902*