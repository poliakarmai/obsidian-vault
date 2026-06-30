---
title: "GSC Audit: /tmp/gsc-learn/tox"
date: 2026-06-30
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/tox

**Дата:** 30.06.2026 04:05  
**Путь:** `/tmp/gsc-learn/tox`  
**Всего находок:** 132  
**CRITICAL:** 0 | **HIGH:** 3 | **MEDIUM:** 43 | **LOW:** 83

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 82 |
| Python: assert in production | 22 |
| Outdated dependency pattern | 16 |
| Синхронный код в async | 5 |
| GS015 | 2 |
| GS008 | 1 |
| Хардкод IP адреса | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | pyproject.toml | 124 | Match:   "sphinx-inline-tabs>=2025.12.21.14", |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | runner.py | 138 |
| M | ? | runner.py | 211 |
| M | ? | cmd_builder.py | 80 |
| M | ? | cmd_builder.py | 125 |
| M | ? | api.py | 189 |
| M | ? | pytest.py | 365 |
| M | ? | pytest.py | 369 |
| M | ? | pytest.py | 394 |
| M | ? | pytest.py | 400 |
| M | ? | pytest.py | 409 |
| M | ? | pytest.py | 410 |
| M | ? | pytest.py | 412 |
| M | ? | pytest.py | 527 |
| M | ? | stream.py | 89 |
| M | ? | env_select.py | 427 |
| M | ? | env_select.py | 443 |
| M | ? | env_select.py | 495 |
| M | ? | env_select.py | 502 |
| M | ? | env_select.py | 517 |
| M | ? | env_select.py | 547 |
| M | ? | env_select.py | 573 |
| M | ? | manager.py | 101 |
| L | GS003 | run.py | 37 |
| L | GS003 | depends.py | 30 |
| L | GS003 | depends.py | 36 |
| L | GS003 | depends.py | 37 |
| L | GS003 | depends.py | 48 |
| L | GS003 | depends.py | 49 |
| L | GS003 | list_env.py | 34 |
| L | GS003 | list_env.py | 47 |
| L | GS003 | list_env.py | 55 |
| L | GS003 | list_env.py | 56 |
| L | GS003 | man.py | 24 |
| L | GS003 | man.py | 25 |
| L | GS003 | man.py | 26 |
| L | GS003 | man.py | 29 |
| L | GS003 | man.py | 30 |
| L | GS003 | man.py | 33 |
| L | GS003 | man.py | 34 |
| L | GS003 | man.py | 35 |
| L | GS003 | man.py | 36 |
| L | GS003 | man.py | 38 |
| L | GS003 | man.py | 40 |
| L | GS003 | man.py | 43 |
| L | GS003 | man.py | 44 |
| L | GS003 | man.py | 49 |
| L | GS003 | man.py | 56 |
| L | GS003 | man.py | 57 |
| L | GS003 | man.py | 59 |
| L | GS003 | man.py | 61 |
| L | GS003 | man.py | 84 |
| L | GS003 | man.py | 86 |
| L | GS003 | man.py | 87 |
| L | GS003 | man.py | 91 |
| L | GS003 | man.py | 104 |
| L | GS003 | man.py | 106 |
| L | GS003 | man.py | 113 |
| L | GS003 | man.py | 114 |
| L | GS003 | man.py | 115 |
| L | GS003 | man.py | 116 |
| L | GS003 | man.py | 117 |
| L | GS003 | man.py | 118 |
| L | GS003 | quickstart.py | 43 |
| L | GS003 | common.py | 154 |
| L | GS003 | common.py | 210 |
| L | GS003 | schema.py | 252 |
| L | GS003 | schema.py | 266 |
| L | GS003 | common.py | 50 |
| L | GS003 | ini.py | 30 |
| L | GS003 | ini.py | 44 |
| L | GS003 | ini.py | 56 |
| L | GS003 | ini.py | 60 |
| L | GS003 | ini.py | 64 |
| L | GS003 | ini.py | 65 |
| L | GS003 | ini.py | 67 |
| L | GS003 | ini.py | 70 |
| L | GS003 | ini.py | 72 |
| L | GS003 | subprocess_adapter.py | 22 |
| L | GS003 | release.py | 25 |
| L | GS003 | release.py | 27 |
| L | GS003 | release.py | 31 |
| L | GS003 | release.py | 33 |
| L | GS003 | release.py | 37 |
| L | GS003 | release.py | 39 |
| L | GS003 | release.py | 43 |
| L | GS003 | release.py | 44 |
| L | GS003 | release.py | 48 |
| L | GS003 | release.py | 80 |
| L | GS003 | release.py | 83 |
| L | GS003 | release.py | 88 |
| L | GS003 | release.py | 91 |
| L | GS003 | release.py | 95 |
| L | GS003 | release.py | 100 |
| L | GS003 | release.py | 120 |
| L | GS003 | release.py | 122 |
| L | GS003 | release.py | 127 |
| L | GS003 | release.py | 133 |
| L | GS003 | release.py | 136 |
| L | GS003 | release.py | 138 |
| L | GS003 | release.py | 143 |
| L | GS003 | release.py | 154 |
| L | GS003 | release.py | 156 |
| L | GS003 | release.py | 158 |
| L | GS003 | release.py | 160 |
| L | GS008 | parallel.py | 23 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| H | ? | pyproject.toml | 124 |
| M | ? | generate_manpage.py | 117 |
| M | ? | dependency_groups.py | 71 |
| M | ? | extras.py | 20 |
| M | ? | pyproject.py | 215 |
| M | ? | pyproject.py | 367 |
| M | ? | runner.py | 36 |
| M | ? | package.py | 79 |
| M | ? | package.py | 85 |
| M | ? | schema.py | 65 |
| M | ? | toml_pyproject.py | 1 |
| M | ? | toml_pyproject.py | 86 |
| M | ? | toml_pyproject.py | 88 |
| M | ? | legacy_toml.py | 22 |
| M | ? | discover.py | 103 |
| M | ? | discover.py | 106 |
| M | ? | toml_tox.py | 13 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| s | GS009 |  | 0 |
| M | ? | subprocess_adapter.py | 119 |
| M | ? | subprocess_adapter.py | 138 |
| M | ? | subprocess_adapter.py | 180 |
| M | ? | subprocess_adapter.py | 217 |
| M | ? | man.py | 69 |

---
*Сгенерировано GSC v0.6 · 2026-06-30T04:05:57.129947*