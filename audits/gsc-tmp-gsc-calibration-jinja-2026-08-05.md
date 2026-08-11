---
title: "GSC Audit: /tmp/gsc-calibration/jinja"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/jinja

**Дата:** 05.08.2026 07:48  
**Путь:** `/tmp/gsc-calibration/jinja`  
**Всего находок:** 52  
**CRITICAL:** 2 | **HIGH:** 9 | **MEDIUM:** 18 | **LOW:** 15

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 15 |
| GS008 | 13 |
| GS022 | 4 |
| GS020 | 3 |
| Python: File upload without content-type validation | 2 |
| CVE-2026-54696: Buffer overflow | 2 |
| eval() or exec() usage | 2 |
| GS004 | 2 |
| GS012 | 2 |
| CVE-2026-55223: Insecure deserialization | 1 |
| GS001 | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |
| GS017 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | pyproject.toml | 134 | Found: "UP038" |
| CRITICAL | ? | bccache.py | 71 | Match:         checksum = pickle.load(f) |
| HIGH | ? | compiler.py | 1986 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | compiler.py | 1987 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | environment.py | 1225 | Match:         exec(code, namespace) |
| HIGH | ? | debug.py | 126 | Match:         exec(code, globals, locals) |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | debug.py | 126 | Line 126: exec(code, globals, locals) |
| HIGH | GS004 | environment.py | 1225 | Line 1225: exec(code, namespace) |
| HIGH | GS017 | lexer.py | 430 | Password length = 1 chars. |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | environment.py | 129 |
| M | ? | environment.py | 132 |
| M | ? | environment.py | 137 |
| M | ? | environment.py | 850 |
| M | ? | environment.py | 851 |
| M | ? | environment.py | 918 |
| M | ? | loaders.py | 324 |
| M | ? | loaders.py | 326 |
| M | ? | filters.py | 904 |
| M | ? | filters.py | 905 |
| M | ? | idtracking.py | 136 |
| M | ? | nodes.py | 64 |
| M | ? | nodes.py | 65 |
| M | ? | compiler.py | 826 |
| M | ? | lexer.py | 694 |
| H | ? | compiler.py | 1986 |
| H | ? | compiler.py | 1987 |
| M | ? | idtracking.py | 158 |
| M | ? | compiler.py | 739 |
| M | ? | bccache.py | 71 |
| C | GS001 | pyproject.toml | 134 |
| L | GS008 | constants.py | 2 |
| L | GS008 | defaults.py | 14 |
| L | GS008 | defaults.py | 15 |
| L | GS008 | defaults.py | 16 |
| L | GS008 | defaults.py | 17 |
| L | GS008 | defaults.py | 18 |
| L | GS008 | defaults.py | 19 |
| L | GS008 | defaults.py | 22 |
| L | GS008 | defaults.py | 23 |
| L | GS008 | defaults.py | 25 |
| L | GS008 | defaults.py | 29 |
| L | GS008 | filters.py | 1812 |
| L | GS008 | tests.py | 216 |
| i | GS020 |  | 1211 |
| i | GS020 |  | 10 |
| i | GS020 |  | 7 |
| H | ? | environment.py | 1225 |
| H | ? | debug.py | 126 |
| C | ? | bccache.py | 71 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | debug.py | 126 |
| H | GS004 | environment.py | 1225 |
| s | GS009 |  | 0 |
| L | GS012 | compiler.py | 1986 |
| L | GS012 | compiler.py | 1987 |
| H | GS017 | lexer.py | 430 |
| r | GS022 |  | 270 |
| r | GS022 |  | 278 |
| r | GS022 |  | 322 |
| r | GS022 |  | 327 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T07:48:29.114360*