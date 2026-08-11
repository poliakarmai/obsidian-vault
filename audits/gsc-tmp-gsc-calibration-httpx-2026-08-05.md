---
title: "GSC Audit: /tmp/gsc-calibration/httpx"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/httpx

**Дата:** 05.08.2026 07:49  
**Путь:** `/tmp/gsc-calibration/httpx`  
**Всего находок:** 140  
**CRITICAL:** 0 | **HIGH:** 5 | **MEDIUM:** 28 | **LOW:** 2

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 90 |
| Python: assert in production | 27 |
| GS021 | 12 |
| GS008 | 2 |
| GS015 | 2 |
| Хардкод IP адреса | 2 |
| GS019 | 2 |
| CVE-2026-37270: Hardcoded credential | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | wsgi.py | 82 | Match:         remote_addr: str = "127.0.0.1", |
| HIGH | ? | asgi.py | 92 | Match:         client: tuple[str, int] = ("127.0.0.1", 123), |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS019 | _client.py | 273 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | _client.py | 284 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | _urlparse.py | 290 |
| M | ? | _urlparse.py | 306 |
| M | ? | default.py | 234 |
| M | ? | default.py | 252 |
| M | ? | default.py | 378 |
| M | ? | default.py | 396 |
| M | ? | wsgi.py | 138 |
| M | ? | wsgi.py | 139 |
| M | ? | asgi.py | 103 |
| M | ? | asgi.py | 152 |
| M | ? | asgi.py | 159 |
| M | ? | asgi.py | 181 |
| M | ? | asgi.py | 182 |
| M | ? | asgi.py | 183 |
| M | ? | _config.py | 97 |
| M | ? | _config.py | 98 |
| M | ? | _config.py | 99 |
| M | ? | _config.py | 100 |
| M | ? | _auth.py | 235 |
| M | ? | _client.py | 1016 |
| M | ? | _client.py | 1732 |
| M | ? | _decoders.py | 181 |
| M | ? | _urls.py | 426 |
| M | ? | _urls.py | 427 |
| M | ? | _models.py | 473 |
| M | ? | _models.py | 487 |
| M | ? | _models.py | 1201 |
| M | ? | wsgi.py | 116 |
| L | GS008 | _config.py | 246 |
| L | GS008 | _config.py | 247 |
| I | GS015 | asgi.py | 1 |
| I | GS015 | wsgi.py | 1 |
| H | ? | wsgi.py | 82 |
| H | ? | asgi.py | 92 |
| H | ? | mkdocs.yml | 0 |
| s | GS009 |  | 0 |
| H | GS019 | _client.py | 273 |
| H | GS019 | _client.py | 284 |
| s | GS021 |  | 191 |
| s | GS021 |  | 192 |
| s | GS021 |  | 196 |
| s | GS021 |  | 197 |
| s | GS021 |  | 202 |
| s | GS021 |  | 203 |
| s | GS021 |  | 208 |
| s | GS021 |  | 211 |
| s | GS021 |  | 71 |
| s | GS021 |  | 44 |
| s | GS021 |  | 82 |
| s | GS021 |  | 92 |
| r | GS022 |  | 226 |
| r | GS022 |  | 228 |
| r | GS022 |  | 2 |
| r | GS022 |  | 198 |
| r | GS022 |  | 213 |
| r | GS022 |  | 219 |
| r | GS022 |  | 229 |
| r | GS022 |  | 269 |
| r | GS022 |  | 282 |
| r | GS022 |  | 286 |
| r | GS022 |  | 361 |
| r | GS022 |  | 376 |
| r | GS022 |  | 392 |
| r | GS022 |  | 411 |
| r | GS022 |  | 433 |
| r | GS022 |  | 439 |
| r | GS022 |  | 444 |
| r | GS022 |  | 271 |
| r | GS022 |  | 210 |
| r | GS022 |  | 553 |
| r | GS022 |  | 206 |
| r | GS022 |  | 288 |
| r | GS022 |  | 295 |
| r | GS022 |  | 296 |
| r | GS022 |  | 366 |
| r | GS022 |  | 391 |
| r | GS022 |  | 396 |
| r | GS022 |  | 481 |
| r | GS022 |  | 517 |
| r | GS022 |  | 524 |
| r | GS022 |  | 760 |
| r | GS022 |  | 1005 |
| r | GS022 |  | 1474 |
| r | GS022 |  | 1721 |
| r | GS022 |  | 126 |
| r | GS022 |  | 131 |
| r | GS022 |  | 133 |
| r | GS022 |  | 138 |
| r | GS022 |  | 140 |
| r | GS022 |  | 142 |
| r | GS022 |  | 147 |
| r | GS022 |  | 149 |
| r | GS022 |  | 151 |
| r | GS022 |  | 156 |
| r | GS022 |  | 158 |
| r | GS022 |  | 172 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 17 |
| r | GS022 |  | 45 |
| r | GS022 |  | 47 |
| r | GS022 |  | 52 |
| r | GS022 |  | 54 |
| r | GS022 |  | 61 |
| r | GS022 |  | 61 |
| r | GS022 |  | 62 |
| r | GS022 |  | 63 |
| r | GS022 |  | 97 |
| r | GS022 |  | 117 |
| r | GS022 |  | 176 |
| r | GS022 |  | 179 |
| r | GS022 |  | 182 |
| r | GS022 |  | 185 |
| r | GS022 |  | 203 |
| r | GS022 |  | 206 |
| r | GS022 |  | 209 |
| r | GS022 |  | 212 |
| r | GS022 |  | 228 |
| r | GS022 |  | 228 |
| r | GS022 |  | 229 |
| r | GS022 |  | 251 |
| r | GS022 |  | 268 |
| r | GS022 |  | 308 |
| r | GS022 |  | 320 |
| r | GS022 |  | 335 |
| r | GS022 |  | 340 |
| r | GS022 |  | 360 |
| r | GS022 |  | 366 |
| r | GS022 |  | 366 |
| r | GS022 |  | 372 |
| r | GS022 |  | 412 |
| r | GS022 |  | 399 |
| r | GS022 |  | 399 |
| r | GS022 |  | 629 |
| r | GS022 |  | 170 |
| r | GS022 |  | 197 |
| r | GS022 |  | 239 |
| r | GS022 |  | 314 |
| r | GS022 |  | 341 |
| r | GS022 |  | 383 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T07:49:19.741246*