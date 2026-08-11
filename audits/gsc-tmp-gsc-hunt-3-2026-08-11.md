---
title: "GSC Audit: /tmp/gsc-hunt-3"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-3

**Дата:** 11.08.2026 07:06  
**Путь:** `/tmp/gsc-hunt-3`  
**Всего находок:** 111  
**CRITICAL:** 28 | **HIGH:** 7 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 28 |
| GS005 | 27 |
| GS020 | 19 |
| GS021 | 9 |
| GS025-eval_usage | 5 |
| YAML-36ACF0AD | 5 |
| GS004 | 4 |
| GS007 | 2 |
| YAML-SSTI001 | 2 |
| GS010 | 1 |
| GS001 | 1 |
| GS015 | 1 |
| GS037-hardcoded_password | 1 |
| GS037-debug_true | 1 |
| GS025 | 1 |
| GS009 | 1 |
| GS019 | 1 |
| YAML-B39DC08C | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | docker.py | 307 | OWASP A03: Injection |
| CRITICAL | GS005 | docker.py | 324 | OWASP A03: Injection |
| CRITICAL | GS005 | docker.py | 341 | OWASP A03: Injection |
| CRITICAL | GS005 | docker.py | 355 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 63 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 73 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 83 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 94 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 108 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 117 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 132 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 138 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 158 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 168 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 179 | OWASP A03: Injection |
| CRITICAL | GS005 | slimselect.js | 1 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 63 |  |
| CRITICAL | GS005 | seed.py | 73 |  |
| CRITICAL | GS005 | seed.py | 83 |  |
| CRITICAL | GS005 | seed.py | 94 |  |
| CRITICAL | GS005 | seed.py | 108 |  |
| CRITICAL | GS005 | seed.py | 117 |  |
| CRITICAL | GS005 | seed.py | 132 |  |
| CRITICAL | GS005 | seed.py | 138 |  |
| CRITICAL | GS005 | seed.py | 158 |  |
| CRITICAL | GS005 | seed.py | 168 |  |
| CRITICAL | GS005 | seed.py | 179 |  |
| CRITICAL | GS001 | config.py | 7 | Found: sqlite:////containery_data/containery.db |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | docker.py | 86 | Line 86: def create_exec(self, endpoint, payload, host=None) |
| HIGH | GS004 | docker.py | 234 | Line 234: def resize_exec(self, sid, exec_id, cols, rows): |
| HIGH | GS004 | socketio.py | 63 | Line 63: exec_id = docker.create_exec(exec_create_endpoint,  |
| HIGH | GS004 | socketio.py | 102 | Line 102: docker.resize_exec(sid, exec_id, cols, rows) |
| HIGH | GS019 | routes.py | 14 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | ? | xterm.js | 1 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | docker.py | 307 |
| C | GS005 | docker.py | 324 |
| C | GS005 | docker.py | 341 |
| C | GS005 | docker.py | 355 |
| C | GS005 | seed.py | 63 |
| C | GS005 | seed.py | 73 |
| C | GS005 | seed.py | 83 |
| C | GS005 | seed.py | 94 |
| C | GS005 | seed.py | 108 |
| C | GS005 | seed.py | 117 |
| C | GS005 | seed.py | 132 |
| C | GS005 | seed.py | 138 |
| C | GS005 | seed.py | 158 |
| C | GS005 | seed.py | 168 |
| C | GS005 | seed.py | 179 |
| C | GS005 | slimselect.js | 1 |
| M | GS010 | docker.py | 247 |
| C | GS005 | seed.py | 63 |
| C | GS005 | seed.py | 73 |
| C | GS005 | seed.py | 83 |
| C | GS005 | seed.py | 94 |
| C | GS005 | seed.py | 108 |
| C | GS005 | seed.py | 117 |
| C | GS005 | seed.py | 132 |
| C | GS005 | seed.py | 138 |
| C | GS005 | seed.py | 158 |
| C | GS005 | seed.py | 168 |
| C | GS005 | seed.py | 179 |
| C | GS001 | config.py | 7 |
| I | GS015 | wsgi.py | 1 |
| i | GS020 |  | 36 |
| i | GS020 |  | 43 |
| i | GS020 |  | 129 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| ? | GS037-hardcoded_password | seed.py | 28 |
| ? | GS037-debug_true | config.py | 13 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS004 | docker.py | 86 |
| H | GS004 | docker.py | 234 |
| H | GS004 | socketio.py | 63 |
| H | GS004 | socketio.py | 102 |
| I | GS007 | xterm.js | 1 |
| I | GS007 | xterm.js | 1 |
| s | GS009 |  | 0 |
| H | GS019 | routes.py | 14 |
| s | GS021 |  | 4 |
| s | GS021 |  | 10 |
| s | GS021 |  | 122 |
| s | GS021 |  | 70 |
| s | GS021 |  | 83 |
| s | GS021 |  | 1 |
| s | GS021 |  | 6 |
| s | GS021 |  | 6 |
| s | GS021 |  | 6 |
| r | GS022 |  | 3 |
| r | GS022 |  | 19 |
| r | GS022 |  | 20 |
| r | GS022 |  | 21 |
| r | GS022 |  | 54 |
| r | GS022 |  | 73 |
| r | GS022 |  | 21 |
| r | GS022 |  | 22 |
| r | GS022 |  | 34 |
| r | GS022 |  | 48 |
| r | GS022 |  | 2 |
| r | GS022 |  | 16 |
| r | GS022 |  | 22 |
| r | GS022 |  | 7 |
| r | GS022 |  | 15 |
| r | GS022 |  | 13 |
| r | GS022 |  | 8 |
| r | GS022 |  | 7 |
| r | GS022 |  | 7 |
| r | GS022 |  | 92 |
| r | GS022 |  | 17 |
| r | GS022 |  | 80 |
| r | GS022 |  | 101 |
| r | GS022 |  | 10 |
| r | GS022 |  | 2 |
| r | GS022 |  | 1 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | socket.io.min.js | ? |
| ? | YAML-36ACF0AD | xterm.js | ? |
| ? | YAML-36ACF0AD | xterm.js | ? |
| ? | YAML-36ACF0AD | xterm.js | ? |
| ? | YAML-36ACF0AD | xterm.js | ? |
| ? | YAML-B39DC08C | xterm.js | ? |
| ? | YAML-SSTI001 | info.html | ? |
| ? | YAML-SSTI001 | info.html | ? |
| H | ? | xterm.js | 1 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T07:06:12.602228*