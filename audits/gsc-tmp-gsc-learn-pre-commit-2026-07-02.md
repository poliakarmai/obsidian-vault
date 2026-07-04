---
title: "GSC Audit: /tmp/gsc-learn/pre-commit"
date: 2026-07-02
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pre-commit

**Дата:** 02.07.2026 04:03  
**Путь:** `/tmp/gsc-learn/pre-commit`  
**Всего находок:** 38  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 16 | **LOW:** 18

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 13 |
| GS003 | 11 |
| GS008 | 7 |
| Outdated dependency pattern | 2 |
| GS015 | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .pre-commit-hooks.yaml (664) | 1 |
| GS009 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-hooks.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | util.py | 62 |
| M | ? | language_helpers.py | 28 |
| M | ? | fixtures.py | 125 |
| M | ? | repository.py | 71 |
| M | ? | util.py | 137 |
| M | ? | util.py | 149 |
| M | ? | util.py | 167 |
| M | ? | util.py | 168 |
| M | ? | util.py | 177 |
| M | ? | julia.py | 104 |
| M | ? | coursier.py | 41 |
| M | ? | node.py | 80 |
| M | ? | autoupdate.py | 147 |
| L | GS003 | hook_impl.py | 56 |
| L | GS003 | hook_impl.py | 59 |
| L | GS003 | migrate_config.py | 131 |
| L | GS003 | migrate_config.py | 134 |
| L | GS003 | validate_config.py | 15 |
| L | GS003 | validate_manifest.py | 15 |
| L | GS003 | check_hooks_apply.py | 25 |
| L | GS003 | check_useless_excludes.py | 41 |
| L | GS003 | check_useless_excludes.py | 62 |
| L | GS003 | foo.py | 7 |
| L | GS003 | foo.py | 8 |
| L | GS008 | color.py | 60 |
| L | GS008 | color.py | 61 |
| L | GS008 | color.py | 62 |
| L | GS008 | color.py | 63 |
| L | GS008 | constants.py | 9 |
| L | GS008 | constants.py | 11 |
| L | GS008 | constants.py | 13 |
| I | GS015 | main.py | 1 |
| M | ? | node.py | 80 |
| M | ? | store.py | 41 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .pre-commit-hooks.yaml | 0 |
| s | GS009 |  | 0 |
| M | ? | hook_impl.py | 46 |

---
*Сгенерировано GSC v0.6 · 2026-07-02T04:03:16.235853*