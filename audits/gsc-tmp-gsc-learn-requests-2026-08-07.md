---
title: "GSC Audit: /tmp/gsc-learn/requests"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/requests

**Дата:** 07.08.2026 04:06  
**Путь:** `/tmp/gsc-learn/requests`  
**Всего находок:** 204  
**CRITICAL:** 2 | **HIGH:** 3 | **MEDIUM:** 10 | **LOW:** 122

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 61 |
| Python: assert in production | 10 |
| GS021 | 5 |
| Generic code smell #24 | 2 |
| Generic code smell #27 | 2 |
| Generic code smell #30 | 2 |
| Generic code smell #33 | 2 |
| Generic code smell #36 | 2 |
| Generic code smell #39 | 2 |
| Generic code smell #42 | 2 |
| Generic code smell #45 | 2 |
| Generic code smell #48 | 2 |
| Generic code smell #51 | 2 |
| Generic code smell #54 | 2 |
| Generic code smell #57 | 2 |
| Generic code smell #60 | 2 |
| Generic code smell #63 | 2 |
| Generic code smell #66 | 2 |
| Generic code smell #69 | 2 |
| Generic code smell #72 | 2 |
| Generic code smell #75 | 2 |
| Generic code smell #78 | 2 |
| Generic code smell #81 | 2 |
| Generic code smell #84 | 2 |
| Generic code smell #87 | 2 |
| Generic code smell #90 | 2 |
| Generic code smell #93 | 2 |
| Generic code smell #96 | 2 |
| Generic code smell #99 | 2 |
| Generic code smell #102 | 2 |
| Generic code smell #105 | 2 |
| Generic code smell #108 | 2 |
| Generic code smell #111 | 2 |
| Generic code smell #114 | 2 |
| Generic code smell #117 | 2 |
| Generic code smell #120 | 2 |
| Generic code smell #123 | 2 |
| Generic code smell #126 | 2 |
| Generic code smell #129 | 2 |
| Generic code smell #132 | 2 |
| Generic code smell #135 | 2 |
| Generic code smell #138 | 2 |
| Generic code smell #141 | 2 |
| Generic code smell #144 | 2 |
| Generic code smell #147 | 2 |
| Generic code smell #150 | 2 |
| Generic code smell #153 | 2 |
| Generic code smell #156 | 2 |
| Generic code smell #159 | 2 |
| Generic code smell #162 | 2 |
| Generic code smell #165 | 2 |
| Generic code smell #168 | 2 |
| Generic code smell #171 | 2 |
| Generic code smell #174 | 2 |
| Generic code smell #177 | 2 |
| Generic code smell #180 | 2 |
| Generic code smell #183 | 2 |
| Generic code smell #186 | 2 |
| Generic code smell #189 | 2 |
| Generic code smell #192 | 2 |
| Generic code smell #195 | 2 |
| Generic code smell #198 | 2 |
| GS001 | 2 |
| GS003 | 2 |
| GS008 | 2 |
| Хардкод IP адреса | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | pyproject.toml | 87 | Found: "py310" |
| CRITICAL | GS001 | pyproject.toml | 100 | Found: "UP031" |
| HIGH | ? | requests-logo.svg | 1 | Match: <svg id="Layer_1" data-name="Layer 1" xmlns="http://w |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| L | ? | _types.py | 60 |
| L | ? | _types.py | 61 |
| M | ? | _internal_utils.py | 46 |
| M | ? | cookies.py | 46 |
| M | ? | sessions.py | 317 |
| M | ? | sessions.py | 318 |
| M | ? | sessions.py | 350 |
| M | ? | sessions.py | 637 |
| M | ? | adapters.py | 375 |
| M | ? | adapters.py | 481 |
| M | ? | adapters.py | 581 |
| M | ? | adapters.py | 659 |
| C | GS001 | pyproject.toml | 87 |
| C | GS001 | pyproject.toml | 100 |
| L | GS003 | certs.py | 18 |
| L | GS003 | help.py | 128 |
| L | GS008 | _internal_utils.py | 20 |
| L | GS008 | adapters.py | 82 |
| H | ? | requests-logo.svg | 1 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| s | GS009 |  | 0 |
| s | GS021 |  | 53 |
| s | GS021 |  | 59 |
| s | GS021 |  | 64 |
| s | GS021 |  | 33 |
| s | GS021 |  | 143 |
| r | GS022 |  | 15 |
| r | GS022 |  | 36 |
| r | GS022 |  | 41 |
| r | GS022 |  | 98 |
| r | GS022 |  | 118 |
| r | GS022 |  | 126 |
| r | GS022 |  | 20 |
| r | GS022 |  | 215 |
| r | GS022 |  | 112 |
| r | GS022 |  | 441 |
| r | GS022 |  | 483 |
| r | GS022 |  | 511 |
| r | GS022 |  | 513 |
| r | GS022 |  | 522 |
| r | GS022 |  | 532 |
| r | GS022 |  | 534 |
| r | GS022 |  | 679 |
| r | GS022 |  | 21 |
| r | GS022 |  | 49 |
| r | GS022 |  | 55 |
| r | GS022 |  | 60 |
| r | GS022 |  | 67 |
| r | GS022 |  | 225 |
| r | GS022 |  | 23 |
| r | GS022 |  | 156 |
| r | GS022 |  | 157 |
| r | GS022 |  | 203 |
| r | GS022 |  | 226 |
| r | GS022 |  | 230 |
| r | GS022 |  | 235 |
| r | GS022 |  | 352 |
| r | GS022 |  | 359 |
| r | GS022 |  | 58 |
| r | GS022 |  | 260 |
| r | GS022 |  | 693 |
| r | GS022 |  | 827 |
| r | GS022 |  | 892 |
| r | GS022 |  | 928 |
| r | GS022 |  | 1046 |
| r | GS022 |  | 1070 |
| r | GS022 |  | 1076 |
| r | GS022 |  | 1128 |
| r | GS022 |  | 37 |
| r | GS022 |  | 93 |
| r | GS022 |  | 284 |
| r | GS022 |  | 296 |
| r | GS022 |  | 491 |
| r | GS022 |  | 494 |
| r | GS022 |  | 496 |
| r | GS022 |  | 539 |
| r | GS022 |  | 541 |
| r | GS022 |  | 546 |
| r | GS022 |  | 549 |
| r | GS022 |  | 550 |
| r | GS022 |  | 551 |
| r | GS022 |  | 565 |
| r | GS022 |  | 584 |
| r | GS022 |  | 589 |
| r | GS022 |  | 627 |
| r | GS022 |  | 666 |
| r | GS022 |  | 669 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T04:06:58.409603*