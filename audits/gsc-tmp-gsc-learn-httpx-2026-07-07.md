---
title: "GSC Audit: /tmp/gsc-learn/httpx"
date: 2026-07-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/httpx

**Дата:** 07.07.2026 04:00  
**Путь:** `/tmp/gsc-learn/httpx`  
**Всего находок:** 35  
**CRITICAL:** 0 | **HIGH:** 3 | **MEDIUM:** 27 | **LOW:** 2

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 27 |
| GS008 | 2 |
| GS015 | 2 |
| Хардкод IP адреса | 2 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | asgi.py | 92 | Match:         client: tuple[str, int] = ("127.0.0.1", 123), |
| HIGH | ? | wsgi.py | 82 | Match:         remote_addr: str = "127.0.0.1", |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | _models.py | 473 |
| M | ? | _models.py | 487 |
| M | ? | _models.py | 1201 |
| M | ? | _urls.py | 426 |
| M | ? | _urls.py | 427 |
| M | ? | _decoders.py | 181 |
| M | ? | _client.py | 1016 |
| M | ? | _client.py | 1732 |
| M | ? | _auth.py | 235 |
| M | ? | _config.py | 97 |
| M | ? | _config.py | 98 |
| M | ? | _config.py | 99 |
| M | ? | _config.py | 100 |
| M | ? | asgi.py | 103 |
| M | ? | asgi.py | 152 |
| M | ? | asgi.py | 159 |
| M | ? | asgi.py | 181 |
| M | ? | asgi.py | 182 |
| M | ? | asgi.py | 183 |
| M | ? | wsgi.py | 138 |
| M | ? | wsgi.py | 139 |
| M | ? | default.py | 234 |
| M | ? | default.py | 252 |
| M | ? | default.py | 378 |
| M | ? | default.py | 396 |
| M | ? | _urlparse.py | 290 |
| M | ? | _urlparse.py | 306 |
| L | GS008 | _config.py | 246 |
| L | GS008 | _config.py | 247 |
| I | GS015 | asgi.py | 1 |
| I | GS015 | wsgi.py | 1 |
| H | ? | asgi.py | 92 |
| H | ? | wsgi.py | 82 |
| H | ? | mkdocs.yml | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-07T04:00:46.477283*