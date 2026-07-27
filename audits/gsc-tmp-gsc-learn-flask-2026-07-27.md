---
title: "GSC Audit: /tmp/gsc-learn/flask"
date: 2026-07-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/flask

**Дата:** 27.07.2026 04:00  
**Путь:** `/tmp/gsc-learn/flask`  
**Всего находок:** 40  
**CRITICAL:** 0 | **HIGH:** 12 | **MEDIUM:** 12 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 15 |
| CVE-2026-37270: Hardcoded credential | 6 |
| Хардкод IP адреса | 6 |
| Python: assert in production | 5 |
| eval() or exec() usage | 2 |
| Bare except: | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS004 | 1 |
| GS009 | 1 |
| GS011 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | uv.lock | 1526 | Match: version = "2.4.7.3" |
| HIGH | ? | uv.lock | 1528 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 1530 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | testing.py | 131 | Match:             "REMOTE_ADDR": "127.0.0.1", |
| HIGH | ? | cli.py | 883 | Match: @click.option("--host", "-h", default="127.0.0.1", he |
| HIGH | ? | app.py | 730 | Match:                 host = "127.0.0.1" |
| HIGH | ? | config.py | 209 | Match:                 exec(compile(config_file.read(), file |
| HIGH | ? | cli.py | 1023 | Match:             eval(compile(f.read(), startup, "exec"),  |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | config.py | 209 | Line 209: exec(compile(config_file.read(), filename, "exec") |
| HIGH | GS011 | config.py | 66 | Found JWT secret in code: 'developm...'. JWT secrets must be |

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
| H | ? | uv.lock | 1526 |
| H | ? | uv.lock | 1528 |
| H | ? | uv.lock | 1530 |
| H | ? | testing.py | 131 |
| H | ? | cli.py | 883 |
| H | ? | app.py | 730 |
| H | ? | config.py | 209 |
| H | ? | cli.py | 1023 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | config.py | 209 |
| s | GS009 |  | 0 |
| H | GS011 | config.py | 66 |

---
*Сгенерировано GSC v0.6 · 2026-07-27T04:00:59.507928*