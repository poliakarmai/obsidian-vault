---
title: "GSC Audit: /tmp/gsc-learn/aiohttp"
date: 2026-07-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/aiohttp

**Дата:** 08.07.2026 04:00  
**Путь:** `/tmp/gsc-learn/aiohttp`  
**Всего находок:** 435  
**CRITICAL:** 0 | **HIGH:** 7 | **MEDIUM:** 156 | **LOW:** 271

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 151 |
| GS003 | 19 |
| GS008 | 15 |
| Generic code smell #24 | 4 |
| Generic code smell #27 | 4 |
| Generic code smell #30 | 4 |
| Generic code smell #33 | 4 |
| Generic code smell #36 | 4 |
| Generic code smell #39 | 4 |
| Generic code smell #42 | 4 |
| Generic code smell #45 | 4 |
| Generic code smell #48 | 4 |
| Generic code smell #51 | 4 |
| Generic code smell #54 | 4 |
| Generic code smell #57 | 4 |
| Generic code smell #60 | 4 |
| Generic code smell #63 | 4 |
| Generic code smell #66 | 4 |
| Generic code smell #69 | 4 |
| Generic code smell #72 | 4 |
| Generic code smell #75 | 4 |
| Generic code smell #78 | 4 |
| Generic code smell #81 | 4 |
| Generic code smell #84 | 4 |
| Generic code smell #87 | 4 |
| Generic code smell #90 | 4 |
| Generic code smell #93 | 4 |
| Generic code smell #96 | 4 |
| Generic code smell #99 | 4 |
| Generic code smell #102 | 4 |
| Generic code smell #105 | 4 |
| Generic code smell #108 | 4 |
| Generic code smell #111 | 4 |
| Generic code smell #114 | 4 |
| Generic code smell #117 | 4 |
| Generic code smell #120 | 4 |
| Generic code smell #123 | 4 |
| Generic code smell #126 | 4 |
| Generic code smell #129 | 4 |
| Generic code smell #132 | 4 |
| Generic code smell #135 | 4 |
| Generic code smell #138 | 4 |
| Generic code smell #141 | 4 |
| Generic code smell #144 | 4 |
| Generic code smell #147 | 4 |
| Generic code smell #150 | 4 |
| Generic code smell #153 | 4 |
| Generic code smell #156 | 4 |
| Generic code smell #159 | 4 |
| Generic code smell #162 | 4 |
| Generic code smell #165 | 4 |
| Generic code smell #168 | 4 |
| Generic code smell #171 | 4 |
| Generic code smell #174 | 4 |
| Generic code smell #177 | 4 |
| Generic code smell #180 | 4 |
| Generic code smell #183 | 4 |
| Generic code smell #186 | 4 |
| Generic code smell #189 | 4 |
| Generic code smell #192 | 4 |
| Generic code smell #195 | 4 |
| Generic code smell #198 | 4 |
| Outdated dependency pattern | 4 |
| Хардкод IP адреса | 1 |
| eval() or exec() usage | 1 |
| World-readable file: .codecov.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| World-readable file: .lgtm.yml (664) | 1 |
| GS004 | 1 |
| GS009 | 1 |
| GS012 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | web_runner.py | 126 | Match:         host = "0.0.0.0" if not self._host else self. |
| HIGH | ? | gen.py | 18 | Match:     exec(code, globs) |
| HIGH | ? | .codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .lgtm.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | gen.py | 18 | Line 18: exec(code, globs) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| L | ? | web_server.py | 42 |
| L | ? | client_proto.py | 143 |
| L | ? | web.py | 291 |
| L | ? | compression_utils.py | 28 |
| M | ? | http_writer.py | 146 |
| M | ? | http_writer.py | 245 |
| M | ? | http_writer.py | 263 |
| M | ? | http_writer.py | 294 |
| M | ? | helpers.py | 730 |
| M | ? | helpers.py | 835 |
| M | ? | helpers.py | 844 |
| M | ? | payload.py | 162 |
| M | ? | cookiejar.py | 551 |
| M | ? | client_reqrep.py | 301 |
| M | ? | client_reqrep.py | 303 |
| M | ? | client_reqrep.py | 416 |
| M | ? | client_reqrep.py | 619 |
| M | ? | client_reqrep.py | 832 |
| M | ? | client_reqrep.py | 910 |
| M | ? | client_reqrep.py | 946 |
| M | ? | client_reqrep.py | 954 |
| M | ? | client_reqrep.py | 1014 |
| M | ? | client_reqrep.py | 1093 |
| M | ? | client_reqrep.py | 1100 |
| M | ? | client_reqrep.py | 1273 |
| M | ? | client_reqrep.py | 1485 |
| M | ? | web_protocol.py | 401 |
| M | ? | web_protocol.py | 448 |
| M | ? | web_protocol.py | 466 |
| M | ? | web_protocol.py | 576 |
| M | ? | web_protocol.py | 658 |
| M | ? | web_protocol.py | 661 |
| M | ? | web_protocol.py | 662 |
| M | ? | web_protocol.py | 821 |
| M | ? | client_ws.py | 128 |
| M | ? | client_ws.py | 146 |
| M | ? | client_ws.py | 324 |
| M | ? | http_parser.py | 304 |
| M | ? | http_parser.py | 421 |
| M | ? | http_parser.py | 458 |
| M | ? | http_parser.py | 524 |
| M | ? | http_parser.py | 529 |
| M | ? | http_parser.py | 530 |
| M | ? | http_parser.py | 1184 |
| M | ? | client.py | 233 |
| M | ? | client.py | 239 |
| M | ? | client.py | 330 |
| M | ? | client.py | 524 |
| M | ? | client.py | 1150 |
| M | ? | client.py | 1152 |
| M | ? | client.py | 1165 |
| M | ? | client.py | 1512 |
| M | ? | client_proto.py | 133 |
| M | ? | client_proto.py | 178 |
| M | ? | client_proto.py | 179 |
| M | ? | connector.py | 554 |
| M | ? | connector.py | 1335 |
| M | ? | connector.py | 1441 |
| M | ? | connector.py | 1448 |
| M | ? | connector.py | 1500 |
| M | ? | connector.py | 1532 |
| M | ? | web_app.py | 63 |
| M | ? | web_middlewares.py | 85 |
| M | ? | base_protocol.py | 53 |
| M | ? | base_protocol.py | 57 |
| M | ? | base_protocol.py | 70 |
| M | ? | multipart.py | 390 |
| M | ? | multipart.py | 400 |
| M | ? | multipart.py | 422 |
| M | ? | multipart.py | 682 |
| M | ? | multipart.py | 1006 |
| M | ? | multipart.py | 1052 |
| M | ? | multipart.py | 1137 |
| M | ? | multipart.py | 1138 |
| M | ? | multipart.py | 1228 |
| M | ? | web_request.py | 873 |
| M | ? | web_request.py | 880 |
| M | ? | web_request.py | 886 |
| M | ? | web_request.py | 895 |
| M | ? | web_fileresponse.py | 124 |
| M | ? | web_fileresponse.py | 274 |
| M | ? | web_fileresponse.py | 394 |
| M | ? | streams.py | 253 |
| M | ? | streams.py | 286 |
| M | ? | streams.py | 372 |
| M | ? | streams.py | 731 |
| M | ? | web_ws.py | 151 |
| M | ? | web_ws.py | 173 |
| M | ? | web_ws.py | 194 |
| M | ? | web_ws.py | 265 |
| M | ? | web_ws.py | 385 |
| M | ? | web_ws.py | 524 |
| M | ? | web_ws.py | 536 |
| M | ? | web_ws.py | 540 |
| M | ? | web_ws.py | 541 |
| M | ? | web_response.py | 150 |
| M | ? | web_response.py | 244 |
| M | ? | web_response.py | 319 |
| M | ? | web_response.py | 320 |
| M | ? | web_response.py | 331 |
| M | ? | web_response.py | 372 |
| M | ? | web_response.py | 374 |
| M | ? | web_response.py | 435 |
| M | ? | web_response.py | 437 |
| M | ? | web_response.py | 450 |
| M | ? | web_response.py | 462 |
| M | ? | web_response.py | 463 |
| M | ? | web_response.py | 472 |
| M | ? | web_response.py | 479 |
| M | ? | web_response.py | 491 |
| M | ? | web_response.py | 645 |
| M | ? | web_response.py | 685 |
| M | ? | web_response.py | 686 |
| M | ? | web_response.py | 687 |
| M | ? | web_response.py | 729 |
| M | ? | client_middleware_digest_auth.py | 506 |
| M | ? | helpers.py | 44 |
| M | ? | helpers.py | 45 |
| M | ? | reader_py.py | 119 |
| M | ? | reader_py.py | 488 |
| M | ? | reader_py.py | 496 |
| M | ? | web_runner.py | 133 |
| M | ? | web_runner.py | 176 |
| M | ? | web_runner.py | 207 |
| M | ? | web_runner.py | 247 |
| M | ? | resolver.py | 83 |
| M | ? | resolver.py | 163 |
| M | ? | web_urldispatcher.py | 160 |
| M | ? | web_urldispatcher.py | 257 |
| M | ? | web_urldispatcher.py | 334 |
| M | ? | web_urldispatcher.py | 365 |
| M | ? | web_urldispatcher.py | 377 |
| M | ? | web_urldispatcher.py | 378 |
| M | ? | web_urldispatcher.py | 379 |
| M | ? | web_urldispatcher.py | 436 |
| M | ? | web_urldispatcher.py | 437 |
| M | ? | web_urldispatcher.py | 446 |
| M | ? | web_urldispatcher.py | 447 |
| M | ? | web_urldispatcher.py | 448 |
| M | ? | web_urldispatcher.py | 477 |
| M | ? | web_urldispatcher.py | 478 |
| M | ? | web_urldispatcher.py | 488 |
| M | ? | web_urldispatcher.py | 489 |
| M | ? | web_urldispatcher.py | 490 |
| M | ? | web_urldispatcher.py | 674 |
| M | ? | web_urldispatcher.py | 788 |
| M | ? | web_urldispatcher.py | 879 |
| M | ? | web_urldispatcher.py | 883 |
| M | ? | web_urldispatcher.py | 1041 |
| M | ? | web_urldispatcher.py | 1149 |
| M | ? | formdata.py | 154 |
| M | ? | worker.py | 104 |
| M | ? | worker.py | 106 |
| M | ? | worker.py | 146 |
| M | ? | check_sum.py | 18 |
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
| H | ? | web_runner.py | 126 |
| M | ? | sync-direct-runtime-deps.py | 2 |
| M | ? | sync-direct-runtime-deps.py | 12 |
| M | ? | sync-direct-runtime-deps.py | 20 |
| M | ? | gen.py | 10 |
| H | ? | gen.py | 18 |
| H | ? | .codecov.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | ? | .lgtm.yml | 0 |
| H | GS004 | gen.py | 18 |
| s | GS009 |  | 0 |
| L | GS012 | _cookie_helpers.py | 185 |
| M | ? | cleanup_changes.py | 38 |

---
*Сгенерировано GSC v0.6 · 2026-07-08T04:00:24.279042*