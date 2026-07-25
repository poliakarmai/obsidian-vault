---
title: "GSC Audit: /tmp/gsc-learn/black"
date: 2026-07-23
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/black

**Дата:** 23.07.2026 04:02  
**Путь:** `/tmp/gsc-learn/black`  
**Всего находок:** 287  
**CRITICAL:** 3 | **HIGH:** 20 | **MEDIUM:** 164 | **LOW:** 98

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 148 |
| GS003 | 35 |
| Rust: .clone() in hot path | 11 |
| Outdated dependency pattern | 10 |
| GS008 | 4 |
| eval() or exec() usage | 4 |
| CVE-2026-55223: Insecure deserialization | 3 |
| pickle.load() — unsafe deserialization | 3 |
| Синхронный код в async | 3 |
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
| GS015 | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .prettierrc.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| World-readable file: action.yml (664) | 1 |
| World-readable file: .pre-commit-hooks.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | grammar.py | 124 | Match:             d = pickle.load(f) |
| CRITICAL | ? | grammar.py | 129 | Match:         self._update(pickle.loads(pkl)) |
| CRITICAL | ? | cache.py | 80 | Match:                 data: dict[str, tuple[float, int, str |
| HIGH | ? | literals.py | 4 | Match: """Safely evaluate Python string literals without usi |
| HIGH | ? | conv.py | 186 | Match:             rawbitset = eval(mo.group(1)) |
| HIGH | ? | conv.py | 212 | Match:                 y = eval(y) |
| HIGH | ? | pgen.py | 100 | Match:             value = eval(label) |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .prettierrc.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | action.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-hooks.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | pytree.py | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | pytree.py | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | linegen.py | 2219 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 1041 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 1699 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 1720 | Clone in performance-critical code — consider references |
| HIGH | ? | trans.py | 1748 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| L | ? | pytree.py | 772 |
| M | ? | diff_shades_gha_helper.py | 90 |
| M | ? | diff_shades_gha_helper.py | 97 |
| M | ? | diff_shades_gha_helper.py | 101 |
| M | ? | diff_shades_gha_helper.py | 102 |
| M | ? | diff_shades_gha_helper.py | 131 |
| M | ? | generate_schema.py | 17 |
| M | ? | driver.py | 95 |
| M | ? | driver.py | 141 |
| M | ? | driver.py | 160 |
| M | ? | driver.py | 191 |
| M | ? | driver.py | 193 |
| M | ? | driver.py | 302 |
| M | ? | parse.py | 34 |
| M | ? | parse.py | 230 |
| M | ? | parse.py | 270 |
| M | ? | parse.py | 332 |
| M | ? | parse.py | 366 |
| M | ? | parse.py | 391 |
| M | ? | literals.py | 24 |
| M | ? | literals.py | 45 |
| M | ? | literals.py | 49 |
| M | ? | literals.py | 50 |
| M | ? | conv.py | 79 |
| M | ? | conv.py | 80 |
| M | ? | conv.py | 123 |
| M | ? | conv.py | 125 |
| M | ? | conv.py | 134 |
| M | ? | conv.py | 140 |
| M | ? | conv.py | 144 |
| M | ? | conv.py | 148 |
| M | ? | conv.py | 150 |
| M | ? | conv.py | 155 |
| M | ? | conv.py | 158 |
| M | ? | conv.py | 162 |
| M | ? | conv.py | 169 |
| M | ? | conv.py | 174 |
| M | ? | conv.py | 177 |
| M | ? | conv.py | 178 |
| M | ? | conv.py | 179 |
| M | ? | conv.py | 181 |
| M | ? | conv.py | 184 |
| M | ? | conv.py | 194 |
| M | ? | conv.py | 201 |
| M | ? | conv.py | 206 |
| M | ? | conv.py | 215 |
| M | ? | conv.py | 220 |
| M | ? | conv.py | 223 |
| M | ? | conv.py | 225 |
| M | ? | conv.py | 227 |
| M | ? | conv.py | 230 |
| M | ? | conv.py | 232 |
| M | ? | conv.py | 235 |
| M | ? | conv.py | 237 |
| M | ? | conv.py | 240 |
| M | ? | conv.py | 246 |
| M | ? | pgen.py | 65 |
| M | ? | pgen.py | 89 |
| M | ? | pgen.py | 90 |
| M | ? | pgen.py | 99 |
| M | ? | pgen.py | 147 |
| M | ? | pgen.py | 186 |
| M | ? | pgen.py | 194 |
| M | ? | pgen.py | 195 |
| M | ? | pgen.py | 203 |
| M | ? | pgen.py | 340 |
| M | ? | pgen.py | 341 |
| M | ? | pgen.py | 351 |
| M | ? | pgen.py | 352 |
| M | ? | pgen.py | 353 |
| M | ? | pgen.py | 359 |
| M | ? | pgen.py | 360 |
| M | ? | pgen.py | 361 |
| M | ? | pgen.py | 371 |
| M | ? | pytree.py | 72 |
| M | ? | pytree.py | 129 |
| M | ? | pytree.py | 130 |
| M | ? | pytree.py | 202 |
| M | ? | pytree.py | 216 |
| M | ? | pytree.py | 270 |
| M | ? | pytree.py | 274 |
| M | ? | pytree.py | 286 |
| M | ? | pytree.py | 302 |
| M | ? | pytree.py | 505 |
| M | ? | pytree.py | 521 |
| M | ? | pytree.py | 540 |
| M | ? | pytree.py | 585 |
| M | ? | pytree.py | 619 |
| M | ? | pytree.py | 623 |
| M | ? | pytree.py | 660 |
| M | ? | pytree.py | 706 |
| M | ? | pytree.py | 708 |
| M | ? | pytree.py | 760 |
| M | ? | pytree.py | 762 |
| M | ? | pytree.py | 765 |
| M | ? | pytree.py | 848 |
| M | ? | pytree.py | 853 |
| M | ? | pytree.py | 857 |
| M | ? | pytree.py | 993 |
| M | ? | pytree.py | 999 |
| M | ? | pytree.py | 1023 |
| M | ? | pygram.py | 185 |
| M | ? | pygram.py | 186 |
| M | ? | strings.py | 70 |
| M | ? | strings.py | 133 |
| M | ? | strings.py | 136 |
| M | ? | strings.py | 140 |
| M | ? | strings.py | 148 |
| M | ? | strings.py | 190 |
| M | ? | strings.py | 335 |
| M | ? | files.py | 351 |
| M | ? | files.py | 353 |
| M | ? | linegen.py | 1765 |
| M | ? | comments.py | 103 |
| M | ? | comments.py | 324 |
| M | ? | comments.py | 332 |
| M | ? | comments.py | 536 |
| M | ? | comments.py | 537 |
| M | ? | trans.py | 733 |
| M | ? | trans.py | 1126 |
| M | ? | trans.py | 1324 |
| M | ? | trans.py | 1522 |
| M | ? | trans.py | 1960 |
| M | ? | trans.py | 2104 |
| M | ? | trans.py | 2389 |
| M | ? | trans.py | 2396 |
| M | ? | trans.py | 2581 |
| M | ? | trans.py | 2582 |
| M | ? | trans.py | 2584 |
| M | ? | trans.py | 2585 |
| M | ? | schema.py | 8 |
| M | ? | handle_ipynb_magics.py | 192 |
| M | ? | handle_ipynb_magics.py | 217 |
| M | ? | mode.py | 32 |
| M | ? | lines.py | 379 |
| M | ? | lines.py | 380 |
| M | ? | lines.py | 608 |
| M | ? | lines.py | 629 |
| M | ? | lines.py | 698 |
| M | ? | lines.py | 1038 |
| M | ? | lines.py | 1175 |
| M | ? | lines.py | 1645 |
| M | ? | nodes.py | 200 |
| M | ? | nodes.py | 359 |
| M | ? | nodes.py | 389 |
| M | ? | nodes.py | 854 |
| M | ? | nodes.py | 855 |
| M | ? | nodes.py | 1097 |
| M | ? | parsing.py | 109 |
| M | ? | grammar.py | 124 |
| M | ? | grammar.py | 129 |
| M | ? | cache.py | 80 |
| L | GS003 | main.py | 36 |
| L | GS003 | main.py | 53 |
| L | GS003 | main.py | 66 |
| L | GS003 | main.py | 92 |
| L | GS003 | main.py | 111 |
| L | GS003 | main.py | 143 |
| L | GS003 | main.py | 158 |
| L | GS003 | main.py | 167 |
| L | GS003 | main.py | 168 |
| L | GS003 | main.py | 195 |
| L | GS003 | main.py | 197 |
| L | GS003 | main.py | 199 |
| L | GS003 | check_pre_commit_rev_in_example.py | 42 |
| L | GS003 | check_version_in_basics_example.py | 38 |
| L | GS003 | diff_shades_gha_helper.py | 46 |
| L | GS003 | diff_shades_gha_helper.py | 48 |
| L | GS003 | diff_shades_gha_helper.py | 59 |
| L | GS003 | diff_shades_gha_helper.py | 76 |
| L | GS003 | diff_shades_gha_helper.py | 193 |
| L | GS003 | generate_schema.py | 70 |
| L | GS003 | conv.py | 66 |
| L | GS003 | conv.py | 75 |
| L | GS003 | conv.py | 116 |
| L | GS003 | grammar.py | 156 |
| L | GS003 | grammar.py | 159 |
| L | GS003 | grammar.py | 161 |
| L | GS003 | grammar.py | 163 |
| L | GS003 | grammar.py | 165 |
| L | GS003 | grammar.py | 167 |
| L | GS003 | grammar.py | 158 |
| L | GS003 | grammar.py | 160 |
| L | GS003 | grammar.py | 162 |
| L | GS003 | grammar.py | 164 |
| L | GS003 | grammar.py | 166 |
| L | GS003 | literals.py | 61 |
| L | GS008 | const.py | 1 |
| L | GS008 | const.py | 2 |
| L | GS008 | const.py | 3 |
| L | GS008 | const.py | 4 |
| I | GS015 | main.py | 1 |
| M | ? | main.py | 63 |
| M | ? | main.py | 67 |
| M | ? | main.py | 93 |
| M | ? | main.py | 113 |
| M | ? | generate_schema.py | 59 |
| M | ? | files.py | 99 |
| M | ? | files.py | 100 |
| M | ? | files.py | 102 |
| M | ? | files.py | 110 |
| M | ? | files.py | 112 |
| H | ? | literals.py | 4 |
| H | ? | conv.py | 186 |
| H | ? | conv.py | 212 |
| H | ? | pgen.py | 100 |
| C | ? | grammar.py | 124 |
| C | ? | grammar.py | 129 |
| C | ? | cache.py | 80 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .prettierrc.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | ? | action.yml | 0 |
| H | ? | .pre-commit-hooks.yaml | 0 |
| s | GS009 |  | 0 |
| M | ? | black.vim | 77 |
| M | ? | black.vim | 152 |
| M | ? | diff_shades_gha_helper.py | 172 |
| H | ? | pytree.py | 101 |
| H | ? | pytree.py | 306 |
| H | ? | linegen.py | 2219 |
| H | ? | trans.py | 109 |
| H | ? | trans.py | 112 |
| H | ? | trans.py | 536 |
| H | ? | trans.py | 579 |
| H | ? | trans.py | 1041 |
| H | ? | trans.py | 1699 |
| H | ? | trans.py | 1720 |
| H | ? | trans.py | 1748 |

---
*Сгенерировано GSC v0.6 · 2026-07-23T04:02:14.997965*