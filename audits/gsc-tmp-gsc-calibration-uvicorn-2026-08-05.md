---
title: "GSC Audit: /tmp/gsc-calibration/uvicorn"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/uvicorn

**Дата:** 05.08.2026 07:49  
**Путь:** `/tmp/gsc-calibration/uvicorn`  
**Всего находок:** 60  
**CRITICAL:** 1 | **HIGH:** 13 | **MEDIUM:** 24 | **LOW:** 2

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 23 |
| GS021 | 14 |
| Хардкод IP адреса | 12 |
| GS015 | 3 |
| GS008 | 2 |
| GS022 | 2 |
| Cache poisoning: unkeyed headers | 1 |
| GS001 | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | pyproject.toml | 109 | Found: "UP031" |
| HIGH | ? | pyproject.toml | 61 | Match:     "types-pyyaml>=6.0.12.20260518", |
| HIGH | ? | uv.lock | 1670 | Match: version = "6.0.12.20260518" |
| HIGH | ? | uv.lock | 1672 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 1674 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 1772 | Match:     { name = "types-pyyaml", specifier = ">=6.0.12.20 |
| HIGH | ? | config.py | 195 | Match:         host: str = "127.0.0.1", |
| HIGH | ? | config.py | 357 | Match:             self.forwarded_allow_ips = os.environ.get |
| HIGH | ? | server.py | 213 | Match:             host = "0.0.0.0" if config.host is None e |
| HIGH | ? | main.py | 66 | Match:     default="127.0.0.1", |
| HIGH | ? | main.py | 248 | Match:     "$FORWARDED_ALLOW_IPS environment variable if ava |
| HIGH | ? | main.py | 497 | Match:     host: str = "127.0.0.1", |
| HIGH | ? | proxy_headers.py | 24 | Match:     def __init__(self, app: ASGI3Application, trusted |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | config.py | 434 |
| M | ? | config.py | 460 |
| M | ? | multiprocess.py | 103 |
| M | ? | basereload.py | 89 |
| M | ? | server.py | 153 |
| M | ? | server.py | 166 |
| M | ? | server.py | 185 |
| M | ? | on.py | 103 |
| M | ? | on.py | 111 |
| M | ? | on.py | 112 |
| M | ? | on.py | 116 |
| M | ? | on.py | 117 |
| M | ? | on.py | 124 |
| M | ? | on.py | 125 |
| M | ? | on.py | 129 |
| M | ? | on.py | 130 |
| M | ? | wsproto_impl.py | 64 |
| M | ? | wsproto_impl.py | 318 |
| M | ? | websockets_sansio_impl.py | 343 |
| M | ? | websockets_sansio_impl.py | 384 |
| M | ? | websockets_sansio_impl.py | 394 |
| M | ? | wsgi.py | 76 |
| M | ? | wsgi.py | 97 |
| M | ? | main.py | 228 |
| C | GS001 | pyproject.toml | 109 |
| L | GS008 | flow_control.py | 5 |
| L | GS008 | flow_control.py | 7 |
| I | GS015 | main.py | 1 |
| I | GS015 | wsgi.py | 1 |
| I | GS015 | server.py | 1 |
| H | ? | pyproject.toml | 61 |
| H | ? | uv.lock | 1670 |
| H | ? | uv.lock | 1672 |
| H | ? | uv.lock | 1674 |
| H | ? | uv.lock | 1772 |
| H | ? | config.py | 195 |
| H | ? | config.py | 357 |
| H | ? | server.py | 213 |
| H | ? | main.py | 66 |
| H | ? | main.py | 248 |
| H | ? | main.py | 497 |
| H | ? | proxy_headers.py | 24 |
| H | ? | mkdocs.yml | 0 |
| s | GS009 |  | 0 |
| s | GS021 |  | 51 |
| s | GS021 |  | 52 |
| s | GS021 |  | 217 |
| s | GS021 |  | 219 |
| s | GS021 |  | 195 |
| s | GS021 |  | 357 |
| s | GS021 |  | 213 |
| s | GS021 |  | 66 |
| s | GS021 |  | 248 |
| s | GS021 |  | 497 |
| s | GS021 |  | 86 |
| s | GS021 |  | 87 |
| s | GS021 |  | 53 |
| s | GS021 |  | 24 |
| r | GS022 |  | 239 |
| r | GS022 |  | 256 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T07:49:41.800257*