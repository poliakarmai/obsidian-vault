---
title: "GSC Audit: /tmp/gsc-learn/starlette"
date: 2026-08-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/starlette

**Дата:** 06.08.2026 04:19  
**Путь:** `/tmp/gsc-learn/starlette`  
**Всего находок:** 193  
**CRITICAL:** 2 | **HIGH:** 10 | **MEDIUM:** 91 | **LOW:** 59

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 87 |
| GS022 | 17 |
| GS025-debug_mode | 9 |
| Хардкод IP адреса | 5 |
| CVE-2026-56233: Path traversal | 2 |
| CVE-2026-56356: Cross-site scripting (XSS) | 2 |
| GS020 | 2 |
| GS019 | 2 |
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
| CVE-2026-56318: Information disclosure | 1 |
| CVE-2026-37270: Hardcoded credential | 1 |
| GS001 | 1 |
| GS015 | 1 |
| Hardcoded encryption key | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | pyproject.toml | 98 | Found: "UP031" |
| CRITICAL | ? | datastructures.py | 171 | Match:             url = str(self.replace(password="******** |
| HIGH | ? | responses.py | 539 |  |
| HIGH | ? | responses.py | 544 |  |
| HIGH | ? | pyproject.toml | 58 | Match:     "types-PyYAML==6.0.12.20250516", |
| HIGH | ? | uv.lock | 1517 | Match:     { name = "types-pyyaml", specifier = "==6.0.12.20 |
| HIGH | ? | uv.lock | 1629 | Match: version = "6.0.12.20250516" |
| HIGH | ? | uv.lock | 1631 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 1633 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS019 | authentication.py | 106 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | requests.py | 179 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| L | ? | exceptions.py | 26 |
| M | ? | gzip_benchmark.py | 106 |
| M | ? | gzip_benchmark.py | 108 |
| M | ? | gzip_benchmark.py | 110 |
| M | ? | gzip_benchmark.py | 111 |
| M | ? | gzip_benchmark.py | 112 |
| M | ? | gzip_benchmark.py | 113 |
| M | ? | gzip_benchmark.py | 115 |
| M | ? | gzip_benchmark.py | 116 |
| M | ? | gzip_benchmark.py | 118 |
| M | ? | gzip_benchmark.py | 119 |
| M | ? | gzip_benchmark.py | 120 |
| M | ? | gzip_benchmark.py | 121 |
| M | ? | gzip_benchmark.py | 149 |
| M | ? | gzip_benchmark.py | 153 |
| M | ? | gzip_benchmark.py | 208 |
| M | ? | gzip_benchmark.py | 265 |
| M | ? | gzip_benchmark.py | 266 |
| M | ? | gzip_benchmark.py | 267 |
| M | ? | gzip_benchmark.py | 268 |
| M | ? | gzip_benchmark.py | 270 |
| M | ? | gzip_benchmark.py | 272 |
| M | ? | gzip_benchmark.py | 337 |
| M | ? | routing.py | 133 |
| M | ? | routing.py | 207 |
| M | ? | routing.py | 264 |
| M | ? | routing.py | 302 |
| M | ? | routing.py | 346 |
| M | ? | routing.py | 369 |
| M | ? | routing.py | 370 |
| M | ? | routing.py | 461 |
| M | ? | routing.py | 663 |
| M | ? | formparsers.py | 66 |
| M | ? | formparsers.py | 161 |
| M | ? | formparsers.py | 283 |
| M | ? | formparsers.py | 286 |
| M | ? | schemas.py | 22 |
| M | ? | schemas.py | 23 |
| M | ? | schemas.py | 106 |
| M | ? | authentication.py | 48 |
| M | ? | authentication.py | 65 |
| M | ? | authentication.py | 84 |
| M | ? | staticfiles.py | 77 |
| M | ? | staticfiles.py | 78 |
| M | ? | staticfiles.py | 80 |
| M | ? | staticfiles.py | 91 |
| M | ? | requests.py | 87 |
| M | ? | requests.py | 171 |
| M | ? | requests.py | 180 |
| M | ? | requests.py | 185 |
| M | ? | requests.py | 219 |
| M | ? | requests.py | 276 |
| M | ? | convertors.py | 28 |
| M | ? | convertors.py | 29 |
| M | ? | convertors.py | 51 |
| M | ? | convertors.py | 63 |
| M | ? | convertors.py | 64 |
| M | ? | convertors.py | 65 |
| M | ? | responses.py | 120 |
| M | ? | endpoints.py | 19 |
| M | ? | endpoints.py | 62 |
| M | ? | endpoints.py | 116 |
| M | ? | websockets.py | 29 |
| M | ? | templating.py | 91 |
| M | ? | testclient.py | 159 |
| M | ? | testclient.py | 332 |
| M | ? | testclient.py | 337 |
| M | ? | testclient.py | 338 |
| M | ? | testclient.py | 359 |
| M | ? | testclient.py | 727 |
| M | ? | testclient.py | 743 |
| M | ? | datastructures.py | 36 |
| M | ? | datastructures.py | 37 |
| M | ? | datastructures.py | 64 |
| M | ? | datastructures.py | 182 |
| M | ? | datastructures.py | 263 |
| M | ? | datastructures.py | 388 |
| M | ? | datastructures.py | 513 |
| M | ? | datastructures.py | 514 |
| M | ? | datastructures.py | 517 |
| M | ? | base.py | 171 |
| M | ? | base.py | 178 |
| M | ? | wsgi.py | 82 |
| M | ? | exceptions.py | 44 |
| M | ? | exceptions.py | 66 |
| M | ? | exceptions.py | 72 |
| M | ? | trustedhost.py | 23 |
| M | ? | trustedhost.py | 25 |
| H | ? | responses.py | 539 |
| H | ? | responses.py | 544 |
| M | ? | datastructures.py | 171 |
| M | ? | errors.py | 75 |
| M | ? | errors.py | 78 |
| M | ? | datastructures.py | 171 |
| C | GS001 | pyproject.toml | 98 |
| I | GS015 | wsgi.py | 1 |
| i | GS020 |  | 75 |
| i | GS020 |  | 78 |
| H | ? | pyproject.toml | 58 |
| H | ? | uv.lock | 1517 |
| H | ? | uv.lock | 1629 |
| H | ? | uv.lock | 1631 |
| H | ? | uv.lock | 1633 |
| C | ? | datastructures.py | 171 |
| H | ? | mkdocs.yml | 0 |
| s | GS009 |  | 0 |
| H | GS019 | authentication.py | 106 |
| H | GS019 | requests.py | 179 |
| s | GS021 |  | 51 |
| r | GS022 |  | 705 |
| r | GS022 |  | 142 |
| r | GS022 |  | 110 |
| r | GS022 |  | 112 |
| r | GS022 |  | 116 |
| r | GS022 |  | 129 |
| r | GS022 |  | 203 |
| r | GS022 |  | 453 |
| r | GS022 |  | 60 |
| r | GS022 |  | 65 |
| r | GS022 |  | 65 |
| r | GS022 |  | 141 |
| r | GS022 |  | 189 |
| r | GS022 |  | 191 |
| r | GS022 |  | 202 |
| r | GS022 |  | 12 |
| r | GS022 |  | 55 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-06T04:19:37.723153*