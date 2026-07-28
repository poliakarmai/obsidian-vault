---
title: "GSC Audit: /tmp/gsc-learn/urllib3"
date: 2026-07-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/urllib3

**Дата:** 28.07.2026 04:01  
**Путь:** `/tmp/gsc-learn/urllib3`  
**Всего находок:** 182  
**CRITICAL:** 0 | **HIGH:** 50 | **MEDIUM:** 25 | **LOW:** 74

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Хардкод IP адреса | 38 |
| GS015 | 32 |
| Python: assert in production | 21 |
| GS008 | 8 |
| GS003 | 7 |
| GS002 | 4 |
| GS014 | 4 |
| Python: File upload without content-type validation | 3 |
| Rust: .clone() in hot path | 2 |
| Generic code smell #24 | 1 |
| Generic code smell #27 | 1 |
| Generic code smell #30 | 1 |
| Generic code smell #33 | 1 |
| Generic code smell #36 | 1 |
| Generic code smell #39 | 1 |
| Generic code smell #42 | 1 |
| Generic code smell #45 | 1 |
| Generic code smell #48 | 1 |
| Generic code smell #51 | 1 |
| Generic code smell #54 | 1 |
| Generic code smell #57 | 1 |
| Generic code smell #60 | 1 |
| Generic code smell #63 | 1 |
| Generic code smell #66 | 1 |
| Generic code smell #69 | 1 |
| Generic code smell #72 | 1 |
| Generic code smell #75 | 1 |
| Generic code smell #78 | 1 |
| Generic code smell #81 | 1 |
| Generic code smell #84 | 1 |
| Generic code smell #87 | 1 |
| Generic code smell #90 | 1 |
| Generic code smell #93 | 1 |
| Generic code smell #96 | 1 |
| Generic code smell #99 | 1 |
| Generic code smell #102 | 1 |
| Generic code smell #105 | 1 |
| Generic code smell #108 | 1 |
| Generic code smell #111 | 1 |
| Generic code smell #114 | 1 |
| Generic code smell #117 | 1 |
| Generic code smell #120 | 1 |
| Generic code smell #123 | 1 |
| Generic code smell #126 | 1 |
| Generic code smell #129 | 1 |
| Generic code smell #132 | 1 |
| Generic code smell #135 | 1 |
| Generic code smell #138 | 1 |
| Generic code smell #141 | 1 |
| Generic code smell #144 | 1 |
| Generic code smell #147 | 1 |
| Generic code smell #150 | 1 |
| Generic code smell #153 | 1 |
| Generic code smell #156 | 1 |
| Generic code smell #159 | 1 |
| Generic code smell #162 | 1 |
| Generic code smell #165 | 1 |
| Generic code smell #168 | 1 |
| Generic code smell #171 | 1 |
| Generic code smell #174 | 1 |
| Generic code smell #177 | 1 |
| Generic code smell #180 | 1 |
| Generic code smell #183 | 1 |
| Generic code smell #186 | 1 |
| Generic code smell #189 | 1 |
| Generic code smell #192 | 1 |
| Generic code smell #195 | 1 |
| Generic code smell #198 | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| World-readable file: .eslintrc.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | app.py | 75 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | app.py | 78 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | app.py | 364 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | pyproject.toml | 46 | Match:   "brotlicffi>=1.2.0.0; platform_python_implementatio |
| HIGH | ? | pyproject.toml | 110 | Match:     "types-requests>=2.32.0.20241016", |
| HIGH | ? | pyproject.toml | 112 | Match:     "types-pysocks>=1.7.1.20251001", |
| HIGH | ? | testcase.py | 197 | Match:     host_alt = "127.0.0.1" |
| HIGH | ? | testcase.py | 228 | Match:     http_host_alt: typing.ClassVar[str] = "127.0.0.1" |
| HIGH | ? | testcase.py | 234 | Match:     https_host_alt: typing.ClassVar[str] = "127.0.0.1 |
| HIGH | ? | testcase.py | 242 | Match:     proxy_host_alt: typing.ClassVar[str] = "127.0.0.1 |
| HIGH | ? | testcase.py | 287 | Match:     http_host_alt = "127.0.0.1" |
| HIGH | ? | testcase.py | 290 | Match:     https_host_alt = "127.0.0.1" |
| HIGH | ? | testcase.py | 294 | Match:     proxy_host_alt = "127.0.0.1" |
| HIGH | ? | noxfile.py | 100 | Match:         "--allow-hosts=localhost,127.0.0.1,::1,127.0. |
| HIGH | ? | port_helpers.py | 10 | Match: HOST = "127.0.0.1" |
| HIGH | ? | uv.lock | 320 | Match: version = "1.2.0.1" |
| HIGH | ? | uv.lock | 325 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 327 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 328 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 329 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 330 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 331 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 332 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 333 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 334 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 335 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 336 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 337 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 338 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 339 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 340 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 2366 | Match: version = "1.7.1.20251001" |
| HIGH | ? | uv.lock | 2368 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 2370 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 2375 | Match: version = "2.33.0.20260408" |
| HIGH | ? | uv.lock | 2380 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 2382 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 2537 | Match:     { name = "brotlicffi", marker = "platform_python_ |
| HIGH | ? | uv.lock | 2634 | Match:     { name = "types-pysocks", specifier = ">=1.7.1.20 |
| HIGH | ? | uv.lock | 2635 | Match:     { name = "types-requests", specifier = ">=2.32.0. |
| HIGH | ? | ssl_match_hostname.py | 17 | Match: __version__ = "3.5.0.1" |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .eslintrc.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | cacert.key | 0 | File cacert.key has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | cacert.pem | 0 | File cacert.pem has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | server.crt | 0 | File server.crt has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | server.key | 0 | File server.key has permissions -rw-rw-r-- — readable by any |
| HIGH | ? | connectionpool.py | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | connectionpool.py | 352 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| L | ? | connection.py | 332 |
| M | ? | asgi_proxy.py | 41 |
| M | ? | hypercornserver.py | 24 |
| M | ? | hypercornserver.py | 127 |
| M | ? | app.py | 81 |
| M | ? | app.py | 158 |
| M | ? | app.py | 196 |
| M | ? | testcase.py | 34 |
| M | ? | testcase.py | 169 |
| M | ? | testcase.py | 170 |
| M | ? | noxfile.py | 238 |
| M | ? | noxfile.py | 242 |
| M | ? | noxfile.py | 305 |
| M | ? | noxfile.py | 306 |
| M | ? | port_helpers.py | 117 |
| M | ? | probe.py | 45 |
| M | ? | connection.py | 260 |
| M | ? | ssltransport.py | 137 |
| M | ? | ssltransport.py | 160 |
| M | ? | _collections.py | 335 |
| M | ? | response.py | 440 |
| M | ? | response.py | 973 |
| H | ? | app.py | 75 |
| H | ? | app.py | 78 |
| H | ? | app.py | 364 |
| L | GS003 | hypercornserver.py | 50 |
| L | GS003 | noxfile.py | 265 |
| L | GS003 | noxfile.py | 281 |
| L | GS003 | connection.py | 313 |
| L | GS003 | connection.py | 355 |
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
| H | ? | pyproject.toml | 46 |
| H | ? | pyproject.toml | 110 |
| H | ? | pyproject.toml | 112 |
| H | ? | testcase.py | 197 |
| H | ? | testcase.py | 228 |
| H | ? | testcase.py | 234 |
| H | ? | testcase.py | 242 |
| H | ? | testcase.py | 287 |
| H | ? | testcase.py | 290 |
| H | ? | testcase.py | 294 |
| H | ? | noxfile.py | 100 |
| H | ? | port_helpers.py | 10 |
| H | ? | uv.lock | 320 |
| H | ? | uv.lock | 325 |
| H | ? | uv.lock | 327 |
| H | ? | uv.lock | 328 |
| H | ? | uv.lock | 329 |
| H | ? | uv.lock | 330 |
| H | ? | uv.lock | 331 |
| H | ? | uv.lock | 332 |
| H | ? | uv.lock | 333 |
| H | ? | uv.lock | 334 |
| H | ? | uv.lock | 335 |
| H | ? | uv.lock | 336 |
| H | ? | uv.lock | 337 |
| H | ? | uv.lock | 338 |
| H | ? | uv.lock | 339 |
| H | ? | uv.lock | 340 |
| H | ? | uv.lock | 2366 |
| H | ? | uv.lock | 2368 |
| H | ? | uv.lock | 2370 |
| H | ? | uv.lock | 2375 |
| H | ? | uv.lock | 2380 |
| H | ? | uv.lock | 2382 |
| H | ? | uv.lock | 2537 |
| H | ? | uv.lock | 2634 |
| H | ? | uv.lock | 2635 |
| H | ? | ssl_match_hostname.py | 17 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | ? | .eslintrc.yml | 0 |
| H | GS002 | cacert.key | 0 |
| H | GS002 | cacert.pem | 0 |
| H | GS002 | server.crt | 0 |
| H | GS002 | server.key | 0 |
| s | GS009 |  | 0 |
| M | GS014 | cacert.key | 1 |
| M | GS014 | cacert.pem | 1 |
| M | GS014 | server.key | 1 |
| M | GS014 | duplicate_san.pem | 1 |
| H | ? | connectionpool.py | 349 |
| H | ? | connectionpool.py | 352 |

---
*Сгенерировано GSC v0.6 · 2026-07-28T04:01:50.311264*