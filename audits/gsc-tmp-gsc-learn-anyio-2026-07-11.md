---
title: "GSC Audit: /tmp/gsc-learn/anyio"
date: 2026-07-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/anyio

**Дата:** 11.07.2026 04:00  
**Путь:** `/tmp/gsc-learn/anyio`  
**Всего находок:** 36  
**CRITICAL:** 3 | **HIGH:** 7 | **MEDIUM:** 24 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 21 |
| CVE-2026-55223: Insecure deserialization | 3 |
| pickle.load() — unsafe deserialization | 3 |
| Хардкод IP адреса | 2 |
| GS004 | 2 |
| GS008 | 1 |
| eval() or exec() usage | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | to_process.py | 95 | Match:         retval = pickle.loads(pickled_response) |
| CRITICAL | ? | to_process.py | 220 | Match:             command, *args = pickle.load(stdin.buffer |
| CRITICAL | ? | to_interpreter.py | 130 | Match:                 res = pickle.loads(res) |
| HIGH | ? | pytest_plugin.py | 344 | Match:                     addr = "::1" if family == socket. |
| HIGH | ? | _sockets.py | 507 | Match:         local_address = ("0.0.0.0", 0) |
| HIGH | ? | to_interpreter.py | 123 | Match:             exc_info = _interpreters.exec(self._inter |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | _asyncio.py | 2740 | Line 2740: transport, protocol = await loop.subprocess_exec( |
| HIGH | GS004 | to_interpreter.py | 123 | Line 123: exc_info = _interpreters.exec(self._interpreter_id |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | pytest_plugin.py | 70 |
| M | ? | from_thread.py | 491 |
| M | ? | from_thread.py | 492 |
| M | ? | _asyncio.py | 354 |
| M | ? | _asyncio.py | 469 |
| M | ? | _asyncio.py | 539 |
| M | ? | _asyncio.py | 540 |
| M | ? | _asyncio.py | 839 |
| M | ? | _asyncio.py | 840 |
| M | ? | _asyncio.py | 1154 |
| M | ? | _asyncio.py | 2224 |
| M | ? | _trio.py | 860 |
| M | ? | _trio.py | 1080 |
| M | ? | _trio.py | 1437 |
| M | ? | to_process.py | 97 |
| M | ? | _asyncio_selector_thread.py | 58 |
| M | ? | _contextmanagers.py | 43 |
| M | ? | _contextmanagers.py | 82 |
| M | ? | _contextmanagers.py | 129 |
| M | ? | _contextmanagers.py | 174 |
| M | ? | itertools.py | 135 |
| M | ? | to_process.py | 95 |
| M | ? | to_process.py | 220 |
| M | ? | to_interpreter.py | 130 |
| L | GS008 | _tasks.py | 42 |
| H | ? | pytest_plugin.py | 344 |
| H | ? | _sockets.py | 507 |
| H | ? | to_interpreter.py | 123 |
| C | ? | to_process.py | 95 |
| C | ? | to_process.py | 220 |
| C | ? | to_interpreter.py | 130 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | GS004 | _asyncio.py | 2740 |
| H | GS004 | to_interpreter.py | 123 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-11T04:00:19.868001*