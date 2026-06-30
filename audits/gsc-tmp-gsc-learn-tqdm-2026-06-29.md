---
title: "GSC Audit: /tmp/gsc-learn/tqdm"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/tqdm

**Дата:** 29.06.2026 04:06  
**Путь:** `/tmp/gsc-learn/tqdm`  
**Всего находок:** 73  
**CRITICAL:** 3 | **HIGH:** 6 | **MEDIUM:** 5 | **LOW:** 59

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Bare except: | 3 |
| GS005 | 3 |
| Python: assert in production | 2 |
| Generic code smell #24 | 1 |
| Generic code smell #27 | 1 |
| Generic code smell #30 | 1 |
| Generic code smell #33 | 1 |
| Generic code smell #36 | 1 |
| Generic code smell #39 | 1 |
| Generic code smell #42 | 1 |
| Generic code smell #45 | 1 |
| Generic code smell #48 | 1 |
| Generic code smell #51 | 1 |
| Generic code smell #54 | 1 |
| Generic code smell #57 | 1 |
| Generic code smell #60 | 1 |
| Generic code smell #63 | 1 |
| Generic code smell #66 | 1 |
| Generic code smell #69 | 1 |
| Generic code smell #72 | 1 |
| Generic code smell #75 | 1 |
| Generic code smell #78 | 1 |
| Generic code smell #81 | 1 |
| Generic code smell #84 | 1 |
| Generic code smell #87 | 1 |
| Generic code smell #90 | 1 |
| Generic code smell #93 | 1 |
| Generic code smell #96 | 1 |
| Generic code smell #99 | 1 |
| Generic code smell #102 | 1 |
| Generic code smell #105 | 1 |
| Generic code smell #108 | 1 |
| Generic code smell #111 | 1 |
| Generic code smell #114 | 1 |
| Generic code smell #117 | 1 |
| Generic code smell #120 | 1 |
| Generic code smell #123 | 1 |
| Generic code smell #126 | 1 |
| Generic code smell #129 | 1 |
| Generic code smell #132 | 1 |
| Generic code smell #135 | 1 |
| Generic code smell #138 | 1 |
| Generic code smell #141 | 1 |
| Generic code smell #144 | 1 |
| Generic code smell #147 | 1 |
| Generic code smell #150 | 1 |
| Generic code smell #153 | 1 |
| Generic code smell #156 | 1 |
| Generic code smell #159 | 1 |
| Generic code smell #162 | 1 |
| Generic code smell #165 | 1 |
| Generic code smell #168 | 1 |
| Generic code smell #171 | 1 |
| Generic code smell #174 | 1 |
| Generic code smell #177 | 1 |
| Generic code smell #180 | 1 |
| Generic code smell #183 | 1 |
| Generic code smell #186 | 1 |
| Generic code smell #189 | 1 |
| Generic code smell #192 | 1 |
| Generic code smell #195 | 1 |
| Generic code smell #198 | 1 |
| World-readable file: environment.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .zenodo.json (664) | 1 |
| World-readable file: .prospector.yml (664) | 1 |
| World-readable file: asv.conf.json (664) | 1 |
| GS004 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | rich.py | 41 | Line 41: return Text( |
| CRITICAL | GS005 | rich.py | 58 | Line 58: return Text(f"? {self.unit}/s", style="progress.dat |
| CRITICAL | GS005 | rich.py | 68 | Line 68: return Text(f"{speed/unit:,.{precision}f} {suffix}{ |
| HIGH | ? | environment.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .zenodo.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .prospector.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | asv.conf.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | cli.py | 38 | Line 38: return literal_eval(f'"{val}"').encode() |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | logging.py | 31 |
| M | ? | notebook.py | 254 |
| M | ? | notebook.py | 264 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| L | ? | cli.py | 125 |
| M | ? | std.py | 125 |
| M | ? | std.py | 155 |
| H | ? | environment.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .zenodo.json | 0 |
| H | ? | .prospector.yml | 0 |
| H | ? | asv.conf.json | 0 |
| H | GS004 | cli.py | 38 |
| C | GS005 | rich.py | 41 |
| C | GS005 | rich.py | 58 |
| C | GS005 | rich.py | 68 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T04:06:52.018534*