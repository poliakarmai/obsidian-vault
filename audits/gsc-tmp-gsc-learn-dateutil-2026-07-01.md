---
title: "GSC Audit: /tmp/gsc-learn/dateutil"
date: 2026-07-01
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/dateutil

**Дата:** 01.07.2026 04:07  
**Путь:** `/tmp/gsc-learn/dateutil`  
**Всего находок:** 319  
**CRITICAL:** 0 | **HIGH:** 5 | **MEDIUM:** 11 | **LOW:** 302

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 10 |
| GS003 | 6 |
| Generic code smell #24 | 5 |
| Generic code smell #27 | 5 |
| Generic code smell #30 | 5 |
| Generic code smell #33 | 5 |
| Generic code smell #36 | 5 |
| Generic code smell #39 | 5 |
| Generic code smell #42 | 5 |
| Generic code smell #45 | 5 |
| Generic code smell #48 | 5 |
| Generic code smell #51 | 5 |
| Generic code smell #54 | 5 |
| Generic code smell #57 | 5 |
| Generic code smell #60 | 5 |
| Generic code smell #63 | 5 |
| Generic code smell #66 | 5 |
| Generic code smell #69 | 5 |
| Generic code smell #72 | 5 |
| Generic code smell #75 | 5 |
| Generic code smell #78 | 5 |
| Generic code smell #81 | 5 |
| Generic code smell #84 | 5 |
| Generic code smell #87 | 5 |
| Generic code smell #90 | 5 |
| Generic code smell #93 | 5 |
| Generic code smell #96 | 5 |
| Generic code smell #99 | 5 |
| Generic code smell #102 | 5 |
| Generic code smell #105 | 5 |
| Generic code smell #108 | 5 |
| Generic code smell #111 | 5 |
| Generic code smell #114 | 5 |
| Generic code smell #117 | 5 |
| Generic code smell #120 | 5 |
| Generic code smell #123 | 5 |
| Generic code smell #126 | 5 |
| Generic code smell #129 | 5 |
| Generic code smell #132 | 5 |
| Generic code smell #135 | 5 |
| Generic code smell #138 | 5 |
| Generic code smell #141 | 5 |
| Generic code smell #144 | 5 |
| Generic code smell #147 | 5 |
| Generic code smell #150 | 5 |
| Generic code smell #153 | 5 |
| Generic code smell #156 | 5 |
| Generic code smell #159 | 5 |
| Generic code smell #162 | 5 |
| Generic code smell #165 | 5 |
| Generic code smell #168 | 5 |
| Generic code smell #171 | 5 |
| Generic code smell #174 | 5 |
| Generic code smell #177 | 5 |
| Generic code smell #180 | 5 |
| Generic code smell #183 | 5 |
| Generic code smell #186 | 5 |
| Generic code smell #189 | 5 |
| Generic code smell #192 | 5 |
| Generic code smell #195 | 5 |
| Generic code smell #198 | 5 |
| Bare except: | 1 |
| GS008 | 1 |
| World-readable file: appveyor.yml (664) | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| World-readable file: zonefile_metadata.json (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | appveyor.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | zonefile_metadata.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | win.py | 119 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| L | ? | _parser.py | 265 |
| L | ? | _parser.py | 267 |
| L | ? | _parser.py | 272 |
| L | ? | _parser.py | 823 |
| L | ? | _parser.py | 941 |
| M | ? | _parser.py | 367 |
| M | ? | _parser.py | 465 |
| M | ? | _parser.py | 470 |
| M | ? | _parser.py | 1457 |
| M | ? | _parser.py | 1523 |
| M | ? | _parser.py | 1531 |
| M | ? | _parser.py | 1568 |
| M | ? | _parser.py | 1572 |
| M | ? | updatezinfo.py | 56 |
| M | ? | relativedelta.py | 369 |
| L | GS003 | updatezinfo.py | 13 |
| L | GS003 | updatezinfo.py | 17 |
| L | GS003 | updatezinfo.py | 36 |
| L | GS003 | updatezinfo.py | 42 |
| L | GS003 | updatezinfo.py | 57 |
| L | GS003 | updatezinfo.py | 60 |
| L | GS008 | tz.py | 38 |
| H | ? | appveyor.yml | 0 |
| H | ? | codecov.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | ? | zonefile_metadata.json | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-01T04:07:24.642042*