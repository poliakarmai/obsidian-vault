---
title: "GSC Audit: /tmp/gs024-test/flask"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gs024-test/flask

**Дата:** 05.08.2026 06:19  
**Путь:** `/tmp/gs024-test/flask`  
**Всего находок:** 62  
**CRITICAL:** 1 | **HIGH:** 15 | **MEDIUM:** 12 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 15 |
| GS021 | 10 |
| GS020 | 7 |
| CVE-2026-37270: Hardcoded credential | 6 |
| Хардкод IP адреса | 6 |
| Python: assert in production | 5 |
| eval() or exec() usage | 2 |
| GS007 | 2 |
| Bare except: | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS004 | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS017 | 1 |
| GS019 | 1 |
| GS022 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS019 | config.py | 66 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | ? | uv.lock | 1537 | Match: version = "2.4.7.3" |
| HIGH | ? | uv.lock | 1539 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 1541 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | testing.py | 131 | Match:             "REMOTE_ADDR": "127.0.0.1", |
| HIGH | ? | cli.py | 883 | Match: @click.option("--host", "-h", default="127.0.0.1", he |
| HIGH | ? | app.py | 730 | Match:                 host = "127.0.0.1" |
| HIGH | ? | config.py | 209 | Match:                 exec(compile(config_file.read(), file |
| HIGH | ? | cli.py | 1023 | Match:             eval(compile(f.read(), startup, "exec"),  |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | config.py | 209 | Line 209: exec(compile(config_file.read(), filename, "exec") |
| HIGH | GS007 | app.py | 1214 | Line 1214: _anchor=_anchor, _method=_method, _scheme=_scheme |
| HIGH | GS007 | helpers.py | 247 | Line 247: _method=_method, |
| HIGH | GS011 | config.py | 66 | Found JWT secret in code: 'developm...'. JWT secrets must be |
| HIGH | GS017 | config.py | 360 | Password length = 1 chars. |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | app.py | 1601 |
| M | ? | views.py | 190 |
| M | ? | testing.py | 59 |
| M | ? | debughelpers.py | 59 |
| M | ? | scaffold.py | 705 |
| M | ? | app.py | 352 |
| M | ? | tag.py | 101 |
| M | ? | tag.py | 135 |
| M | ? | tag.py | 161 |
| M | ? | tag.py | 179 |
| M | ? | tag.py | 193 |
| M | ? | tag.py | 207 |
| I | GS015 | app.py | 1119 |
| I | GS015 | app.py | 1119 |
| I | GS015 | app.py | 1119 |
| I | GS015 | app.py | 126 |
| I | GS015 | app.py | 143 |
| I | GS015 | app.py | 144 |
| I | GS015 | app.py | 1573 |
| I | GS015 | app.py | 1577 |
| I | GS015 | app.py | 626 |
| I | GS015 | app.py | 626 |
| I | GS015 | app.py | 626 |
| I | GS015 | app.py | 76 |
| I | GS015 | app.py | 93 |
| I | GS015 | app.py | 94 |
| I | GS015 | app.py | 400 |
| i | GS020 |  | 151 |
| i | GS020 |  | 159 |
| i | GS020 |  | 211 |
| i | GS020 |  | 10 |
| i | GS020 |  | 12 |
| i | GS020 |  | 10 |
| i | GS020 |  | 12 |
| H | ? | uv.lock | 1537 |
| H | ? | uv.lock | 1539 |
| H | ? | uv.lock | 1541 |
| H | ? | testing.py | 131 |
| H | ? | cli.py | 883 |
| H | ? | app.py | 730 |
| H | ? | config.py | 209 |
| H | ? | cli.py | 1023 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | config.py | 209 |
| H | GS007 | app.py | 1214 |
| H | GS007 | helpers.py | 247 |
| s | GS009 |  | 0 |
| H | GS011 | config.py | 66 |
| H | GS017 | config.py | 360 |
| C | GS019 | config.py | 66 |
| s | GS021 |  | 66 |
| s | GS021 |  | 131 |
| s | GS021 |  | 883 |
| s | GS021 |  | 668 |
| s | GS021 |  | 670 |
| s | GS021 |  | 730 |
| c | GS021 |  | 626 |
| s | GS021 |  | 11 |
| s | GS021 |  | 12 |
| c | GS021 |  | 14 |
| r | GS022 |  | 588 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T06:19:00.535033*