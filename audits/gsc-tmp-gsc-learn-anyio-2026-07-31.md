---
title: "GSC Audit: /tmp/gsc-learn/anyio"
date: 2026-07-31
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/anyio

**Дата:** 31.07.2026 04:02  
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
| HIGH | ? | pytest_plugin.py | 344 | Match:                     addr = "::1" if fam == socket.AF_ |
| HIGH | ? | _sockets.py | 507 | Match:         local_address = ("0.0.0.0", 0) |
| HIGH | ? | to_interpreter.py | 123 | Match:             exc_info = _interpreters.exec(self._inter |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | _asyncio.py | 2746 | Line 2746: transport, protocol = await loop.subprocess_exec( |
| HIGH | GS004 | to_interpreter.py | 123 | Line 123: exc_info = _interpreters.exec(self._interpreter_id |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | pytest_plugin.py | 70 |
| M | ? | from_thread.py | 493 |
| M | ? | from_thread.py | 494 |
| M | ? | _asyncio.py | 355 |
| M | ? | _asyncio.py | 468 |
| M | ? | _asyncio.py | 538 |
| M | ? | _asyncio.py | 539 |
| M | ? | _asyncio.py | 842 |
| M | ? | _asyncio.py | 843 |
| M | ? | _asyncio.py | 1163 |
| M | ? | _asyncio.py | 2234 |
| M | ? | _trio.py | 861 |
| M | ? | _trio.py | 1087 |
| M | ? | _trio.py | 1444 |
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
| L | GS008 | _tasks.py | 40 |
| H | ? | pytest_plugin.py | 344 |
| H | ? | _sockets.py | 507 |
| H | ? | to_interpreter.py | 123 |
| C | ? | to_process.py | 95 |
| C | ? | to_process.py | 220 |
| C | ? | to_interpreter.py | 130 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | GS004 | _asyncio.py | 2746 |
| H | GS004 | to_interpreter.py | 123 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-31T04:02:00.333966*