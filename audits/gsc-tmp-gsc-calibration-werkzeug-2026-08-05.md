---
title: "GSC Audit: /tmp/gsc-calibration/werkzeug"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/werkzeug

**Дата:** 05.08.2026 07:48  
**Путь:** `/tmp/gsc-calibration/werkzeug`  
**Всего находок:** 152  
**CRITICAL:** 0 | **HIGH:** 15 | **MEDIUM:** 8 | **LOW:** 12

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 56 |
| GS021 | 53 |
| Python: assert in production | 8 |
| GS003 | 7 |
| Хардкод IP адреса | 6 |
| GS020 | 5 |
| GS012 | 5 |
| eval() or exec() usage | 3 |
| CVE-2026-56233: Path traversal | 2 |
| GS015 | 2 |
| GS004 | 2 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | security.py | 181 |  |
| HIGH | ? | utils.py | 199 |  |
| HIGH | ? | serving.py | 685 | Match:     host = "fd31:f903:5ab5:1::1" if family == socket. |
| HIGH | ? | serving.py | 691 | Match:             return "::1" if family == socket.AF_INET6 |
| HIGH | ? | serving.py | 844 | Match:             if self.host in {"0.0.0.0", "::"}: |
| HIGH | ? | serving.py | 847 | Match:                 if self.host == "0.0.0.0": |
| HIGH | ? | serving.py | 848 | Match:                     localhost = "127.0.0.1" |
| HIGH | ? | serving.py | 1083 | Match:         if hostname not in {"0.0.0.0", "[::]"}: |
| HIGH | ? | rules.py | 736 | Match:         exec(code, globs, locs) |
| HIGH | ? | console.py | 177 | Match:             exec(code, self.locals) |
| HIGH | ? | console.py | 213 | Match:     def eval(self, code: str) -> str: |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | console.py | 177 | Line 177: exec(code, self.locals) |
| HIGH | GS004 | rules.py | 736 | Line 736: exec(code, globs, locs) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | range.py | 271 |
| M | ? | map.py | 770 |
| M | ? | map.py | 825 |
| M | ? | rules.py | 700 |
| M | ? | _internal.py | 39 |
| M | ? | serving.py | 260 |
| M | ? | serving.py | 261 |
| M | ? | serving.py | 301 |
| H | ? | security.py | 181 |
| H | ? | utils.py | 199 |
| L | GS003 | profiler.py | 152 |
| L | GS003 | profiler.py | 154 |
| L | GS003 | profiler.py | 156 |
| L | GS003 | serving.py | 761 |
| L | GS003 | serving.py | 764 |
| L | GS003 | serving.py | 772 |
| L | GS003 | debugger.js | 43 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 1 |
| i | GS020 |  | 157 |
| i | GS020 |  | 219 |
| i | GS020 |  | 225 |
| i | GS020 |  | 250 |
| i | GS020 |  | 273 |
| H | ? | serving.py | 685 |
| H | ? | serving.py | 691 |
| H | ? | serving.py | 844 |
| H | ? | serving.py | 847 |
| H | ? | serving.py | 848 |
| H | ? | serving.py | 1083 |
| H | ? | rules.py | 736 |
| H | ? | console.py | 177 |
| H | ? | console.py | 213 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | console.py | 177 |
| H | GS004 | rules.py | 736 |
| s | GS009 |  | 0 |
| L | GS012 | map.py | 157 |
| L | GS012 | map.py | 175 |
| L | GS012 | map.py | 399 |
| L | GS012 | map.py | 623 |
| L | GS012 | map.py | 926 |
| s | GS021 |  | 73 |
| s | GS021 |  | 18 |
| s | GS021 |  | 18 |
| s | GS021 |  | 13 |
| s | GS021 |  | 13 |
| s | GS021 |  | 26 |
| s | GS021 |  | 26 |
| s | GS021 |  | 13 |
| s | GS021 |  | 13 |
| s | GS021 |  | 8 |
| s | GS021 |  | 27 |
| s | GS021 |  | 31 |
| s | GS021 |  | 31 |
| s | GS021 |  | 79 |
| s | GS021 |  | 38 |
| s | GS021 |  | 33 |
| s | GS021 |  | 33 |
| s | GS021 |  | 71 |
| s | GS021 |  | 71 |
| s | GS021 |  | 40 |
| s | GS021 |  | 34 |
| s | GS021 |  | 34 |
| s | GS021 |  | 24 |
| s | GS021 |  | 124 |
| s | GS021 |  | 194 |
| s | GS021 |  | 437 |
| s | GS021 |  | 833 |
| s | GS021 |  | 856 |
| s | GS021 |  | 889 |
| s | GS021 |  | 910 |
| s | GS021 |  | 928 |
| s | GS021 |  | 949 |
| s | GS021 |  | 993 |
| s | GS021 |  | 1209 |
| s | GS021 |  | 1396 |
| s | GS021 |  | 680 |
| s | GS021 |  | 691 |
| s | GS021 |  | 844 |
| s | GS021 |  | 847 |
| s | GS021 |  | 848 |
| s | GS021 |  | 848 |
| s | GS021 |  | 851 |
| s | GS021 |  | 854 |
| s | GS021 |  | 983 |
| s | GS021 |  | 1032 |
| s | GS021 |  | 1039 |
| s | GS021 |  | 1083 |
| s | GS021 |  | 303 |
| s | GS021 |  | 303 |
| s | GS021 |  | 305 |
| s | GS021 |  | 43 |
| s | GS021 |  | 126 |
| s | GS021 |  | 139 |
| r | GS022 |  | 23 |
| r | GS022 |  | 31 |
| r | GS022 |  | 66 |
| r | GS022 |  | 392 |
| r | GS022 |  | 423 |
| r | GS022 |  | 427 |
| r | GS022 |  | 431 |
| r | GS022 |  | 434 |
| r | GS022 |  | 948 |
| r | GS022 |  | 991 |
| r | GS022 |  | 651 |
| r | GS022 |  | 655 |
| r | GS022 |  | 684 |
| r | GS022 |  | 780 |
| r | GS022 |  | 788 |
| r | GS022 |  | 811 |
| r | GS022 |  | 43 |
| r | GS022 |  | 104 |
| r | GS022 |  | 162 |
| r | GS022 |  | 232 |
| r | GS022 |  | 255 |
| r | GS022 |  | 314 |
| r | GS022 |  | 755 |
| r | GS022 |  | 485 |
| r | GS022 |  | 158 |
| r | GS022 |  | 223 |
| r | GS022 |  | 226 |
| r | GS022 |  | 231 |
| r | GS022 |  | 233 |
| r | GS022 |  | 236 |
| r | GS022 |  | 240 |
| r | GS022 |  | 243 |
| r | GS022 |  | 245 |
| r | GS022 |  | 20 |
| r | GS022 |  | 369 |
| r | GS022 |  | 29 |
| r | GS022 |  | 57 |
| r | GS022 |  | 62 |
| r | GS022 |  | 65 |
| r | GS022 |  | 93 |
| r | GS022 |  | 17 |
| r | GS022 |  | 19 |
| r | GS022 |  | 29 |
| r | GS022 |  | 41 |
| r | GS022 |  | 61 |
| r | GS022 |  | 16 |
| r | GS022 |  | 18 |
| r | GS022 |  | 28 |
| r | GS022 |  | 12 |
| r | GS022 |  | 46 |
| r | GS022 |  | 51 |
| r | GS022 |  | 40 |
| r | GS022 |  | 55 |
| r | GS022 |  | 84 |
| r | GS022 |  | 241 |
| r | GS022 |  | 267 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T07:48:49.796651*