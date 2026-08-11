---
title: "GSC Audit: /tmp/gsc-learn/urllib3"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/urllib3

**Дата:** 08.08.2026 04:03  
**Путь:** `/tmp/gsc-learn/urllib3`  
**Всего находок:** 282  
**CRITICAL:** 0 | **HIGH:** 50 | **MEDIUM:** 25 | **LOW:** 74

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 100 |
| GS021 | 59 |
| GS022 | 41 |
| GS015 | 32 |
| GS018 | 21 |
| GS008 | 8 |
| GS003 | 7 |
| GS002 | 4 |
| GS014 | 4 |
| GS025 | 3 |
| Rust: .clone() in hot path | 2 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS000-LEGACY | app.py | 75 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | app.py | 78 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | app.py | 364 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | pyproject.toml | 47 | Match:   "brotlicffi>=1.2.0.0; platform_python_implementatio |
| HIGH | GS000-LEGACY | pyproject.toml | 111 | Match:     "types-requests>=2.32.0.20241016", |
| HIGH | GS000-LEGACY | pyproject.toml | 113 | Match:     "types-pysocks>=1.7.1.20251001", |
| HIGH | GS000-LEGACY | testcase.py | 197 | Match:     host_alt = "127.0.0.1" |
| HIGH | GS000-LEGACY | testcase.py | 228 | Match:     http_host_alt: typing.ClassVar[str] = "127.0.0.1" |
| HIGH | GS000-LEGACY | testcase.py | 234 | Match:     https_host_alt: typing.ClassVar[str] = "127.0.0.1 |
| HIGH | GS000-LEGACY | testcase.py | 242 | Match:     proxy_host_alt: typing.ClassVar[str] = "127.0.0.1 |
| HIGH | GS000-LEGACY | testcase.py | 287 | Match:     http_host_alt = "127.0.0.1" |
| HIGH | GS000-LEGACY | testcase.py | 290 | Match:     https_host_alt = "127.0.0.1" |
| HIGH | GS000-LEGACY | testcase.py | 294 | Match:     proxy_host_alt = "127.0.0.1" |
| HIGH | GS000-LEGACY | noxfile.py | 100 | Match:         "--allow-hosts=localhost,127.0.0.1,::1,127.0. |
| HIGH | GS000-LEGACY | port_helpers.py | 10 | Match: HOST = "127.0.0.1" |
| HIGH | GS000-LEGACY | uv.lock | 320 | Match: version = "1.2.0.1" |
| HIGH | GS000-LEGACY | uv.lock | 325 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | GS000-LEGACY | uv.lock | 327 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 328 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 329 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 330 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 331 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 332 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 333 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 334 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 335 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 336 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 337 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 338 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 339 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 340 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 2366 | Match: version = "1.7.1.20251001" |
| HIGH | GS000-LEGACY | uv.lock | 2368 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | GS000-LEGACY | uv.lock | 2370 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 2375 | Match: version = "2.33.0.20260408" |
| HIGH | GS000-LEGACY | uv.lock | 2380 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | GS000-LEGACY | uv.lock | 2382 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | GS000-LEGACY | uv.lock | 2537 | Match:     { name = "brotlicffi", marker = "platform_python_ |
| HIGH | GS000-LEGACY | uv.lock | 2634 | Match:     { name = "types-pysocks", specifier = ">=1.7.1.20 |
| HIGH | GS000-LEGACY | uv.lock | 2635 | Match:     { name = "types-requests", specifier = ">=2.32.0. |
| HIGH | GS000-LEGACY | ssl_match_hostname.py | 17 | Match: __version__ = "3.5.0.1" |
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .eslintrc.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | cacert.key | 0 | File cacert.key has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | cacert.pem | 0 | File cacert.pem has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | server.crt | 0 | File server.crt has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | server.key | 0 | File server.key has permissions -rw-rw-r-- — readable by any |
| HIGH | ? | connectionpool.py | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | connectionpool.py | 352 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| L | GS000-LEGACY | connection.py | 333 |
| M | GS018 | asgi_proxy.py | 41 |
| M | GS018 | hypercornserver.py | 24 |
| M | GS018 | hypercornserver.py | 127 |
| M | GS018 | app.py | 81 |
| M | GS018 | app.py | 158 |
| M | GS018 | app.py | 196 |
| M | GS018 | testcase.py | 34 |
| M | GS018 | testcase.py | 169 |
| M | GS018 | testcase.py | 170 |
| M | GS018 | noxfile.py | 238 |
| M | GS018 | noxfile.py | 242 |
| M | GS018 | noxfile.py | 305 |
| M | GS018 | noxfile.py | 306 |
| M | GS018 | port_helpers.py | 117 |
| M | GS018 | probe.py | 45 |
| M | GS018 | connection.py | 261 |
| M | GS018 | ssltransport.py | 137 |
| M | GS018 | ssltransport.py | 160 |
| M | GS018 | _collections.py | 335 |
| M | GS018 | response.py | 440 |
| M | GS018 | response.py | 973 |
| H | GS000-LEGACY | app.py | 75 |
| H | GS000-LEGACY | app.py | 78 |
| H | GS000-LEGACY | app.py | 364 |
| L | GS003 | hypercornserver.py | 50 |
| L | GS003 | noxfile.py | 265 |
| L | GS003 | noxfile.py | 281 |
| L | GS003 | connection.py | 344 |
| L | GS003 | connection.py | 386 |
| L | GS003 | emscripten_fetch_worker.js | 40 |
| L | GS003 | emscripten_fetch_worker.js | 100 |
| L | GS008 | socketserver.py | 40 |
| L | GS008 | socketserver.py | 86 |
| L | GS008 | fetch.py | 66 |
| L | GS008 | request.py | 20 |
| L | GS008 | ssl_.py | 21 |
| L | GS008 | ssl_.py | 104 |
| L | GS008 | url.py | 65 |
| L | GS008 | url.py | 67 |
| I | GS015 | app.py | 37 |
| I | GS015 | app.py | 38 |
| I | GS015 | app.py | 39 |
| I | GS015 | app.py | 44 |
| I | GS015 | app.py | 51 |
| I | GS015 | app.py | 59 |
| I | GS015 | app.py | 60 |
| I | GS015 | app.py | 73 |
| I | GS015 | app.py | 104 |
| I | GS015 | app.py | 113 |
| I | GS015 | app.py | 37 |
| I | GS015 | app.py | 38 |
| I | GS015 | app.py | 39 |
| I | GS015 | app.py | 44 |
| I | GS015 | app.py | 51 |
| I | GS015 | app.py | 59 |
| I | GS015 | app.py | 60 |
| I | GS015 | app.py | 73 |
| I | GS015 | app.py | 104 |
| I | GS015 | app.py | 113 |
| I | GS015 | app.py | 37 |
| I | GS015 | app.py | 38 |
| I | GS015 | app.py | 39 |
| I | GS015 | app.py | 44 |
| I | GS015 | app.py | 51 |
| I | GS015 | app.py | 59 |
| I | GS015 | app.py | 60 |
| I | GS015 | app.py | 73 |
| I | GS015 | app.py | 104 |
| I | GS015 | app.py | 113 |
| I | GS015 | app.py | 19 |
| I | GS015 | app.py | 26 |
| H | GS000-LEGACY | pyproject.toml | 47 |
| H | GS000-LEGACY | pyproject.toml | 111 |
| H | GS000-LEGACY | pyproject.toml | 113 |
| H | GS000-LEGACY | testcase.py | 197 |
| H | GS000-LEGACY | testcase.py | 228 |
| H | GS000-LEGACY | testcase.py | 234 |
| H | GS000-LEGACY | testcase.py | 242 |
| H | GS000-LEGACY | testcase.py | 287 |
| H | GS000-LEGACY | testcase.py | 290 |
| H | GS000-LEGACY | testcase.py | 294 |
| H | GS000-LEGACY | noxfile.py | 100 |
| H | GS000-LEGACY | port_helpers.py | 10 |
| H | GS000-LEGACY | uv.lock | 320 |
| H | GS000-LEGACY | uv.lock | 325 |
| H | GS000-LEGACY | uv.lock | 327 |
| H | GS000-LEGACY | uv.lock | 328 |
| H | GS000-LEGACY | uv.lock | 329 |
| H | GS000-LEGACY | uv.lock | 330 |
| H | GS000-LEGACY | uv.lock | 331 |
| H | GS000-LEGACY | uv.lock | 332 |
| H | GS000-LEGACY | uv.lock | 333 |
| H | GS000-LEGACY | uv.lock | 334 |
| H | GS000-LEGACY | uv.lock | 335 |
| H | GS000-LEGACY | uv.lock | 336 |
| H | GS000-LEGACY | uv.lock | 337 |
| H | GS000-LEGACY | uv.lock | 338 |
| H | GS000-LEGACY | uv.lock | 339 |
| H | GS000-LEGACY | uv.lock | 340 |
| H | GS000-LEGACY | uv.lock | 2366 |
| H | GS000-LEGACY | uv.lock | 2368 |
| H | GS000-LEGACY | uv.lock | 2370 |
| H | GS000-LEGACY | uv.lock | 2375 |
| H | GS000-LEGACY | uv.lock | 2380 |
| H | GS000-LEGACY | uv.lock | 2382 |
| H | GS000-LEGACY | uv.lock | 2537 |
| H | GS000-LEGACY | uv.lock | 2634 |
| H | GS000-LEGACY | uv.lock | 2635 |
| H | GS000-LEGACY | ssl_match_hostname.py | 17 |
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS025 | .readthedocs.yml | 0 |
| H | GS025 | .eslintrc.yml | 0 |
| H | GS002 | cacert.key | 0 |
| H | GS002 | cacert.pem | 0 |
| H | GS002 | server.crt | 0 |
| H | GS002 | server.key | 0 |
| s | GS009 |  | 0 |
| M | GS014 | cacert.key | 1 |
| M | GS014 | cacert.pem | 1 |
| M | GS014 | server.key | 1 |
| M | GS014 | duplicate_san.pem | 1 |
| s | GS021 |  | 100 |
| s | GS021 |  | 100 |
| s | GS021 |  | 100 |
| s | GS021 |  | 254 |
| s | GS021 |  | 139 |
| s | GS021 |  | 72 |
| s | GS021 |  | 85 |
| s | GS021 |  | 109 |
| s | GS021 |  | 48 |
| s | GS021 |  | 196 |
| s | GS021 |  | 197 |
| s | GS021 |  | 220 |
| s | GS021 |  | 227 |
| s | GS021 |  | 228 |
| s | GS021 |  | 233 |
| s | GS021 |  | 234 |
| s | GS021 |  | 241 |
| s | GS021 |  | 242 |
| s | GS021 |  | 286 |
| s | GS021 |  | 287 |
| s | GS021 |  | 289 |
| s | GS021 |  | 290 |
| s | GS021 |  | 294 |
| s | GS021 |  | 104 |
| s | GS021 |  | 112 |
| s | GS021 |  | 116 |
| s | GS021 |  | 116 |
| s | GS021 |  | 157 |
| s | GS021 |  | 168 |
| s | GS021 |  | 183 |
| s | GS021 |  | 184 |
| s | GS021 |  | 187 |
| s | GS021 |  | 193 |
| s | GS021 |  | 201 |
| s | GS021 |  | 212 |
| s | GS021 |  | 214 |
| s | GS021 |  | 217 |
| s | GS021 |  | 231 |
| s | GS021 |  | 246 |
| s | GS021 |  | 248 |
| s | GS021 |  | 10 |
| s | GS021 |  | 21 |
| s | GS021 |  | 59 |
| s | GS021 |  | 62 |
| s | GS021 |  | 94 |
| s | GS021 |  | 94 |
| s | GS021 |  | 197 |
| s | GS021 |  | 198 |
| s | GS021 |  | 200 |
| s | GS021 |  | 201 |
| s | GS021 |  | 34 |
| s | GS021 |  | 223 |
| s | GS021 |  | 261 |
| s | GS021 |  | 125 |
| s | GS021 |  | 311 |
| s | GS021 |  | 459 |
| s | GS021 |  | 547 |
| s | GS021 |  | 522 |
| s | GS021 |  | 21 |
| r | GS022 |  | 126 |
| r | GS022 |  | 57 |
| r | GS022 |  | 135 |
| r | GS022 |  | 147 |
| r | GS022 |  | 575 |
| r | GS022 |  | 706 |
| r | GS022 |  | 579 |
| r | GS022 |  | 711 |
| r | GS022 |  | 1129 |
| r | GS022 |  | 1146 |
| r | GS022 |  | 1149 |
| r | GS022 |  | 1189 |
| r | GS022 |  | 372 |
| r | GS022 |  | 385 |
| r | GS022 |  | 436 |
| r | GS022 |  | 581 |
| r | GS022 |  | 648 |
| r | GS022 |  | 660 |
| r | GS022 |  | 671 |
| r | GS022 |  | 542 |
| r | GS022 |  | 546 |
| r | GS022 |  | 688 |
| r | GS022 |  | 1470 |
| r | GS022 |  | 1479 |
| r | GS022 |  | 1204 |
| r | GS022 |  | 86 |
| r | GS022 |  | 168 |
| r | GS022 |  | 212 |
| r | GS022 |  | 227 |
| r | GS022 |  | 232 |
| r | GS022 |  | 461 |
| r | GS022 |  | 480 |
| r | GS022 |  | 483 |
| r | GS022 |  | 486 |
| r | GS022 |  | 491 |
| r | GS022 |  | 559 |
| r | GS022 |  | 193 |
| r | GS022 |  | 225 |
| r | GS022 |  | 57 |
| r | GS022 |  | 61 |
| r | GS022 |  | 101 |
| H | ? | connectionpool.py | 349 |
| H | ? | connectionpool.py | 352 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:03:04.870511*