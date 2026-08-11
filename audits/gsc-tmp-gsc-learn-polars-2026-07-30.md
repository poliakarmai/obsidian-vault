---
title: "GSC Audit: /tmp/gsc-learn/polars"
date: 2026-07-30
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/polars

**Дата:** 30.07.2026 04:01  
**Путь:** `/tmp/gsc-learn/polars`  
**Всего находок:** 7470  
**CRITICAL:** 19 | **HIGH:** 6735 | **MEDIUM:** 52 | **LOW:** 657

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 6705 |
| GS003 | 355 |
| Python: assert in production | 41 |
| GS001 | 15 |
| eval() or exec() usage | 12 |
| CVE-2026-37270: Hardcoded credential | 8 |
| GS007 | 6 |
| GS012 | 6 |
| GS014 | 6 |
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
| Python: File upload without content-type validation | 3 |
| CVE-2026-56233: Path traversal | 3 |
| Postgres URL with password | 2 |
| Hardcoded encryption key | 2 |
| Outdated dependency pattern | 2 |
| GS004 | 2 |
| CVE-2026-56413: Command injection | 1 |
| GS008 | 1 |
| World-readable file: dprint.json (664) | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS005 | 1 |
| GS009 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | various.py | 679 |  |
| CRITICAL | GS001 | flake.nix | 144 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 156 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 161 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 166 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 171 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 176 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 181 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 186 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 199 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 204 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 209 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 214 | Found: pwd = "py-polars" |
| CRITICAL | GS001 | flake.nix | 225 | Found: pwd = "crates" |
| CRITICAL | GS001 | flake.nix | 244 | Found: pwd = "crates" |
| CRITICAL | GS001 | frame.py | 4418 | Found: sqlite:////path/to/databa |
| CRITICAL | ? | utils.rs | 67 | Match:     let mut out_key = '\u{1D17A}'.to_string(); |
| CRITICAL | ? | _executor.py | 498 | Match:         param_key = "parameters" |
| CRITICAL | GS005 | frame.py | 4600 | Line 4600: cursor.execute(f"DROP TABLE IF EXISTS {table_name |
| HIGH | ? | config.py | 266 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | config.py | 280 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | config.py | 461 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | frame.py | 4417 | Redteam Kit |
| HIGH | ? | frame.py | 4445 | Redteam Kit |
| HIGH | ? | udfs.py | 626 |  |
| HIGH | ? | frame.py | 4286 |  |
| HIGH | ? | frame.py | 4287 |  |
| HIGH | ? | launch.py | 76 | Match:     exec( |
| HIGH | ? | _dataset.py | 114 | Match:                 pa_predicate_expr = eval( |
| HIGH | ? | array.py | 819 | Match:     def eval(self, expr: Expr, *, as_list: bool = Fal |
| HIGH | ? | series.py | 5296 | Match:         >>> s_from_str_repr = eval(s.to_init_repr()) |
| HIGH | ? | series.py | 6216 | Match:               `s.list.eval(pl.element().sqrt())`. |
| HIGH | ? | list.py | 1002 | Match:     def eval(self, expr: Expr, *, parallel: bool = Fa |
| HIGH | ? | array.py | 385 | Match:         return self.eval( |
| HIGH | ? | array.py | 597 | Match:         return self.eval(F.element().reverse()) |
| HIGH | ? | array.py | 1018 | Match:     def eval(self, expr: Expr, *, as_list: bool = Fal |
| HIGH | ? | list.py | 479 | Match:         return self.eval(F.element().reverse()) |
| HIGH | ? | list.py | 507 | Match:         return self.eval(F.element().unique(maintain_ |
| HIGH | ? | list.py | 1323 | Match:     def eval(self, expr: Expr, *, parallel: bool = Fa |
| HIGH | ? | dprint.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | launch.py | 76 | Line 76: exec( |
| HIGH | GS004 | various.py | 679 | Line 679: subprocess.run(cmd, shell=True) |
| HIGH | GS014 | frame.py | 4417 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | frame.py | 4445 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | functions.py | 367 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | functions.py | 438 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | functions.py | 445 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | functions.py | 458 | Database URL contains password in plaintext. Use environment |
| HIGH | ? | mod.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 407 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | map.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | binview.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 506 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | offset.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | offset.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 351 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | static_array.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | static_array.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 746 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 768 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 776 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 534 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 420 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 429 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 495 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 355 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 362 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 420 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | ffi.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 355 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | arity_assign.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | concatenate.rs | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | conversion.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | bitmap_ops.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | bitmap_ops.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | bitmap_ops.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | bitmap_ops.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | immutable.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | immutable.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | immutable.rs | 755 | Clone in performance-critical code — consider references |
| HIGH | ? | immutable.rs | 758 | Clone in performance-critical code — consider references |
| HIGH | ? | immutable.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | immutable.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 476 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 495 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 545 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 542 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 545 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 739 | Clone in performance-critical code — consider references |
| HIGH | ? | expression.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | expression.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | expression.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | expression.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | expression.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | in_memory_linearize.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_group_by.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_group_by.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_group_by.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_group_by.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_group_by.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_group_by.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_group_by.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | peak_minmax.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | peak_minmax.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | peak_minmax.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | negative_slice.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 493 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | gather_every.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | repeat.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | unordered_union.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | unordered_union.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | rle_id.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | rle_id.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | rle_id.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | morsel_resize_pipeline.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_morsel_sender.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_morsel_sender.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_morsel_sender.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_morsel_sender.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | hstack_columns.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | hstack_columns.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | file_provider.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | file_provider.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | file_provider.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_distributor.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_key.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_key.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_key.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | partitioner.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | partitioner.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_encoder.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | morsel_serializer.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | morsel_serializer.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | morsel_serializer.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | io_writer.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_encoder.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_encoder.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_encoder.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | single_file.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | single_file.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | partition_by.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | sorted_group_by.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | sorted_group_by.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | sorted_group_by.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | sorted_group_by.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | sorted_group_by.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | callback_sink.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | callback_sink.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | simple_projection.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | simple_projection.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | reduce.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | backward_fill.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | is_sorted.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | ordered_union.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | forward_fill.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | forward_fill.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | forward_fill.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | forward_fill.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | forward_fill.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | forward_fill.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | forward_fill.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_group_by.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_data_fetch.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_data_fetch.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_data_fetch.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_data_fetch.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_data_fetch.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | pipeline_budget.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | pipeline_budget.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | batch.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 309 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 590 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 592 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 648 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 670 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_decode.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata_utils.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata_utils.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | projection.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | projection.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | projection.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_data_fetch.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_data_fetch.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_data_fetch.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_data_fetch.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_data_fetch.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_data_fetch.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group_data_fetch.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | forbid_extra_columns.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | forbid_extra_columns.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | apply_extra_ops.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | row_deletions.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_operation_pushdown.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_operation_pushdown.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | transform.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 602 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 654 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_slice.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_projections.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve_projections.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 407 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | initialization.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | bridge.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | post_apply_extra_ops.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | post_apply_extra_ops.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | post_apply_extra_ops.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | post_apply_extra_ops.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | post_apply_extra_ops.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 466 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 566 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 596 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 617 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | reader_starter.rs | 661 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_reader.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_reader.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_reader.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | line_batch_source.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | line_batch_source.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | line_batch_processor.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | row_index_limit_pass.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | negative_slice_pass.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | negative_slice_pass.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | negative_slice_pass.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | negative_slice_pass.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | negative_slice_pass.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_reader.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | chunk_reader.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | line_batch_distributor.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | line_batch_distributor.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 430 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 480 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 534 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_data_fetch.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_data_fetch.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_data_fetch.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_data_fetch.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_data_fetch.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_decode.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_decode.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_decode.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_decode.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_decode.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_decode.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | record_batch_decode.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | strptime_infer.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | strptime_infer.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | strptime_infer.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | strptime_infer.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | strptime_infer.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 815 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 816 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 863 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 1065 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 1173 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 1507 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 1508 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 1539 | Clone in performance-critical code — consider references |
| HIGH | ? | equi_join.rs | 1572 | Clone in performance-critical code — consider references |
| HIGH | ? | cross_join.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | cross_join.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | cross_join.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | cross_join.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | cross_join.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | range_join.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | range_join.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | range_join.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | range_join.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | range_join.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | range_join.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | range_join.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 502 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 616 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | semi_anti_join.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | semi_anti_join.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | semi_anti_join.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | semi_anti_join.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | semi_anti_join.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | semi_anti_join.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | semi_anti_join.rs | 459 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 735 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 756 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 822 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 833 | Clone in performance-critical code — consider references |
| HIGH | ? | asof_join.rs | 836 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | multiplexer.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | sorted_unique.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | sorted_unique.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | columnar_function.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | columnar_function.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | columnar_function.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | with_row_index.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | with_row_index.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | with_row_index.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | in_memory_source.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | in_memory_source.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | skeleton.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | skeleton.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | skeleton.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | skeleton.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 789 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 816 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 824 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 832 | Clone in performance-critical code — consider references |
| HIGH | ? | python_dataset.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 629 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 647 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 668 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 687 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 748 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 756 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 768 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 784 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 831 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 833 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 840 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 897 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 898 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 901 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 904 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 931 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 966 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 970 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 971 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 973 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 974 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 977 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 997 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 999 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1000 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1006 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1011 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1035 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1039 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1040 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1042 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1045 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1046 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1048 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1065 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1067 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1070 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1108 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1113 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1123 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1144 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1175 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1188 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1213 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1223 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1243 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1245 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1249 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1254 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1346 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1352 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1356 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1379 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1384 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1389 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1403 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1408 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1411 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1425 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1431 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1436 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1454 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1461 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1464 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1469 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1489 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1491 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1529 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1536 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1570 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1575 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1576 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1582 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1583 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1610 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1613 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1640 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1643 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1648 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1688 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1710 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1724 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1736 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1739 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1748 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1771 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1772 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1774 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1813 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1816 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1832 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1842 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1844 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1888 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1891 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1898 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1915 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1926 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1934 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1937 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1955 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1961 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1965 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1974 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1979 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 1992 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2002 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2003 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2008 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2013 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2026 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2035 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2052 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2057 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2060 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2061 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2104 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2126 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2143 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2248 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2252 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2256 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2291 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2318 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2322 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2326 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2334 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2358 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2359 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2364 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2366 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2401 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2405 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2407 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2408 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2427 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2434 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2451 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2454 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2457 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2463 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2492 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2498 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2535 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2542 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2547 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2548 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2559 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2568 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2569 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2583 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2605 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2632 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2641 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2645 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2655 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2665 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2711 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2714 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2752 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2758 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2781 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2821 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2862 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2865 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2867 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2887 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2888 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2890 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2895 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_expr.rs | 2940 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 683 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 691 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 758 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 793 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 796 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 824 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 836 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 847 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 850 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 900 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 930 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 932 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 939 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 941 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 947 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 961 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 986 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 987 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 999 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1067 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1076 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1084 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1095 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1097 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1100 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1106 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1118 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1119 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1132 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1135 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1151 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1164 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1169 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1172 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1180 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1185 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1190 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1225 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1228 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1253 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1273 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1275 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1276 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1290 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_group_by.rs | 1291 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 719 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 794 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 491 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 578 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 597 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 631 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 737 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 775 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 776 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 785 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 795 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 835 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 883 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 896 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 956 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 969 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 980 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1003 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1004 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1005 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1006 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1008 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1053 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1054 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1055 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1060 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1061 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1083 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1089 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1094 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1176 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1212 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1214 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1215 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1217 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1219 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1220 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1288 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1327 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1340 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1341 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1346 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1358 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1369 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1377 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1418 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1434 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1442 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1443 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1448 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1463 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1486 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1487 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1492 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1497 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1518 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1521 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1567 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1568 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1576 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1583 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1608 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1616 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1645 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1646 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1647 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1654 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1691 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1724 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1744 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1767 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1779 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1811 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1849 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1858 | Clone in performance-critical code — consider references |
| HIGH | ? | lower_ir.rs | 1866 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 472 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 473 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 526 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 535 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 557 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 584 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 601 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 637 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 650 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 663 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 725 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 736 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 753 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 754 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 776 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 787 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 809 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 849 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 867 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 870 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 871 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 872 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 874 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 875 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 877 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 878 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 880 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 882 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 883 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 964 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 978 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 987 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1009 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1016 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1017 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1040 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1047 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1048 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1070 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1087 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1088 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1094 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1096 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1100 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1101 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1102 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1106 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1107 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1151 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1152 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1155 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1156 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1253 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1254 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1255 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1262 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1263 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1264 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1265 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1283 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1286 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1287 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1313 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1316 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1317 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1325 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1326 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1327 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1328 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1329 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1330 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1357 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1358 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1361 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1362 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1367 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1368 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1369 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1370 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1405 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1424 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1447 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1454 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1474 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1530 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1563 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1567 | Clone in performance-critical code — consider references |
| HIGH | ? | to_graph.rs | 1582 | Clone in performance-critical code — consider references |
| HIGH | ? | pipe.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | pipe.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | execute.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | execute.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | execute.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | execute.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | execute.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | single_key.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | single_key.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | single_key.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | row_encoded.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | execution_state.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 473 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 486 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 685 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 474 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 597 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 711 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 773 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 1128 | Clone in performance-critical code — consider references |
| HIGH | ? | window.rs | 1208 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | structeval.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | structeval.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | structeval.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | structeval.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | structeval.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | structeval.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | structeval.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | column.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | column.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | column.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | ternary.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | element.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | element.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | sortby.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | sortby.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | sortby.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | sortby.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | sortby.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | sortby.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 358 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 480 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 535 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 590 | Clone in performance-critical code — consider references |
| HIGH | ? | eval.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | alias.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | alias.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | alias.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | group_iter.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | count.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | count.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 384 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 561 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | aggregation.rs | 639 | Clone in performance-critical code — consider references |
| HIGH | ? | gather.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | gather.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 351 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 491 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 576 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | first_last.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | first_last.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | first_last.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | implode.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | implode.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | implode.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | implode.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | implode.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | implode.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | first_last_nonnull.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | first_last_nonnull.rs | 459 | Clone in performance-critical code — consider references |
| HIGH | ? | first_last_nonnull.rs | 470 | Clone in performance-critical code — consider references |
| HIGH | ? | approx_n_unique.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 646 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 647 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 796 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 797 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max_by.rs | 813 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | cov.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | cov.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | cov.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | cov.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 361 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 620 | Clone in performance-critical code — consider references |
| HIGH | ? | planner.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | hash_keys.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | hash_keys.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | hash_keys.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | single_key.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | single_key.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | row_encoded.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | binview.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 532 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 288 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 702 | Clone in performance-critical code — consider references |
| HIGH | ? | misc.rs | 751 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | cat.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | cat.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | cat.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | random.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | random.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 480 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 521 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 823 | Clone in performance-critical code — consider references |
| HIGH | ? | groups_dispatch.rs | 880 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | shift_and_fill.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | shift_and_fill.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | time_range.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | time_range.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime_range.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime_range.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime_range.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | linear_space.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | linear_space.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | linear_space.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | linear_space.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | linear_space.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | linear_space.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | int_range.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | int_range.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | pow.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_by.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_enum.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_enum.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | pl_path.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | pl_path.rs | 635 | Clone in performance-critical code — consider references |
| HIGH | ? | arena.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | collection.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | error_capture.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | python_convert_registry.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | order_statistic_tree.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | python_function.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | idx_vec.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | idx_vec.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | idx_vec.rs | 471 | Clone in performance-critical code — consider references |
| HIGH | ? | key.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | total_ord.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | total_ord.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | total_ord.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | pl_ref_str.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | version_0.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | version_0.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | version_0.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | callback.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | callback.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 839 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 851 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 854 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 904 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1064 | Clone in performance-critical code — consider references |
| HIGH | ? | source.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype_expr.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype_expr.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_dsl.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_dsl.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_dsl.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | python_delta_dv_provider.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | python_delta_dv_provider.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | selectors.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | selectors.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | sink.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | sink.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | sink.rs | 417 | Clone in performance-critical code — consider references |
| HIGH | ? | sink.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | sink.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | sink.rs | 517 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 309 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 313 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 470 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 475 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 533 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 600 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 663 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 720 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | serializable_plan.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 356 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 384 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 502 | Clone in performance-critical code — consider references |
| HIGH | ? | scan_sources.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 854 | Clone in performance-critical code — consider references |
| HIGH | ? | serde_expr.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | agg.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | agg.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | udf.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | udf.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | udf.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | constants.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | constants.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | constants.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | constants.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 355 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 356 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | lit.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | builder_ir.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_sort.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | deep_copy.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | stack_opt.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | stack_opt.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | fused.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 626 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 697 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 713 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 736 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 926 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 956 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 966 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 992 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 998 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1028 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1034 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1081 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1106 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1107 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1110 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1193 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1234 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1239 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1293 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1334 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1337 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1338 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1445 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1518 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1629 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1642 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1689 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1695 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1716 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1718 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1726 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1758 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1956 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2072 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2073 | Clone in performance-critical code — consider references |
| HIGH | ? | edge.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | edge.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_pushdown_lp.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 355 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 356 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | expand_datasets.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 362 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 562 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 555 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 719 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 720 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 722 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 729 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 730 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 745 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 751 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 756 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 764 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 769 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 849 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 852 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 853 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 858 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 866 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 867 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 869 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 872 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 879 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 881 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 901 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 906 | Clone in performance-critical code — consider references |
| HIGH | ? | predicate_pruning.rs | 915 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | keys.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | expr.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | expr.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_pushdown_expr.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_pushdown_expr.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_pushdown_expr.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_pushdown_expr.rs | 427 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | cluster_with_columns.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 420 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 567 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 585 | Clone in performance-critical code — consider references |
| HIGH | ? | sortedness.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_and_project.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_and_project.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_and_project.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | collapse_and_project.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_states.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_states.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_states.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_states.rs | 431 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_states.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_states.rs | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_states.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | cspe.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | cspe.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 545 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 865 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 925 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 937 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 1019 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 1064 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 1112 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 1113 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | csee.rs | 1115 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 944 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 945 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify_functions.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify_functions.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify_functions.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify_functions.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify_functions.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify_functions.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify_functions.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | parquet_metadata_prune.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | parquet_metadata_prune.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | flatten_merge_sorted.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | python_udf.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | dsl.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | count.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | count.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | count.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | prune.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | prune.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | prune.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | prune.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | prune.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | prune.rs | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | expr.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | stack_opt.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | stack_opt.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | stack_opt.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | ir_to_dsl.rs | 8 | Clone in performance-critical code — consider references |
| HIGH | ? | ir_to_dsl.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | ir_to_dsl.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 486 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 607 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 806 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 909 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 910 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 960 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 961 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1009 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1010 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1048 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1049 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1109 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1110 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1160 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1161 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1162 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1204 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1205 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1235 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1236 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1313 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1314 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1364 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1378 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1390 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1400 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1409 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1410 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1464 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1471 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1498 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1507 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1513 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1563 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1570 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1573 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1629 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1640 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 715 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 725 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 359 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 570 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 578 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 609 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 618 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 691 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 697 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 698 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 711 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 733 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 736 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 745 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 749 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 771 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 772 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 793 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 812 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 823 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 825 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 854 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 855 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 868 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 890 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 891 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_expansion.rs | 919 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 557 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 773 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 775 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 783 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 803 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 858 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 877 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 927 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 934 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 940 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 987 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 991 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1013 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1021 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1031 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1059 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1065 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1096 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1098 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1112 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1200 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1235 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1240 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1245 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1255 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1264 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1274 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1283 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1337 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1338 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1342 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1343 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1396 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1427 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1676 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1687 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1729 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1731 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1732 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1734 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1736 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1737 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1738 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1742 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1743 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1745 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1773 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1788 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1800 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1818 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 633 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 684 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 743 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 831 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 862 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 863 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 867 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 892 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 899 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 926 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 945 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 965 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 976 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1044 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1209 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1211 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1246 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1248 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1297 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1300 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1319 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1323 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1324 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1331 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1335 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1336 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1369 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1374 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1389 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1390 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1400 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1411 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1412 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1413 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1414 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1423 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1424 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1425 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1435 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1454 | Clone in performance-critical code — consider references |
| HIGH | ? | scans.rs | 1462 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 539 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_to_ir.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 493 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 523 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 534 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 780 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 781 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 788 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 791 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1112 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1143 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1165 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 883 | Clone in performance-critical code — consider references |
| HIGH | ? | unoptimized.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | unoptimized.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | unoptimized.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | unoptimized.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | unoptimized.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | unoptimized.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | skip_batches.rs | 751 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | column_expr.rs | 429 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | cat.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | plugin.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | plugin.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | cum.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | cum.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 466 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 532 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 557 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 561 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 566 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 648 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 689 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 695 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 728 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 746 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 776 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 789 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 811 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 844 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 661 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 704 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 888 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 901 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 917 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 919 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 950 | Clone in performance-critical code — consider references |
| HIGH | ? | filter_constraint.rs | 996 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 298 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 470 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 472 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 473 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 788 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 804 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 875 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 890 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 904 | Clone in performance-critical code — consider references |
| HIGH | ? | or_factoring.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_ir.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | tree_traversal.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | tree_traversal.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | tree_traversal.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | tree_traversal.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | tree_traversal.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | tree_traversal.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | tree_traversal.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | csv.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | csv.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | csv.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | csv.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | csv.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | file_list_reader.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | file_list_reader.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | file_list_reader.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | anonymous_scan.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | dot.rs | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | dot.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | dot.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 646 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 767 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1056 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1106 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1152 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1563 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1926 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2331 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2332 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2357 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2358 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2361 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2362 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2365 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2366 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2369 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2370 | Clone in performance-critical code — consider references |
| HIGH | ? | err.rs | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_arenas.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_arenas.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_arenas.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_arenas.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_arenas.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_arenas.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_arenas.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | storage.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | storage.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 476 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 868 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 869 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 872 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | page.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | page.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | from_thrift.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | from_thrift.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | row_metadata.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | row_metadata.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | schema_descriptor.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | schema_descriptor.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | schema_descriptor.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | file_metadata_serde.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | column_chunk_metadata.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | file_metadata.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | file_metadata.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | file_metadata_thrift.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_len_binary.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_len_binary.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_len_binary.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_len_binary.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | encoder.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | encoder.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 586 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 626 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 773 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 810 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 820 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 838 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 933 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 936 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 989 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1050 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1079 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1110 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1120 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1136 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1146 | Clone in performance-critical code — consider references |
| HIGH | ? | row_group.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | basic.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | basic.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 567 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 585 | Clone in performance-critical code — consider references |
| HIGH | ? | basic.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 623 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 688 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 744 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 793 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | pages.rs | 893 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 466 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 652 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 826 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 534 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | integer.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | integer.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | float.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | float.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 652 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 686 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | optional_masked_dense.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | optional_masked_dense.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | optional_masked_dense.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | required_masked_dense.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | optional.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | nested.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 1226 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 1231 | Clone in performance-critical code — consider references |
| HIGH | ? | convert.rs | 1240 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 576 | Clone in performance-critical code — consider references |
| HIGH | ? | statistics.rs | 604 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | cum_agg.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | clip.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | clip.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | clip.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | clip.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | clip.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate_by.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate_by.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate_by.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate_by.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate_by.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolate_by.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | fused.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | fused.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | fused.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | is_unique.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | is_unique.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | is_unique.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | is_unique.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | is_unique.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | is_unique.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | is_unique.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | log.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | log.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | is_first_distinct.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | unique.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | unique.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | unique.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | ewm_by.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 459 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 585 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 609 | Clone in performance-critical code — consider references |
| HIGH | ? | is_in.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | diff.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | abs.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | pct_change.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | floor_divide.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | floor_divide.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | floor_divide.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | index_of.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | rle.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | search_sorted.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | is_last_distinct.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | is_last_distinct.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | is_last_distinct.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | is_last_distinct.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | is_last_distinct.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | is_last_distinct.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | is_last_distinct.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | horizontal.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | concat_arr.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | business.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | business.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | business.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | business.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | eager.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | eager.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | eager.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | various.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | various.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | various.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | various.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | cut.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | cut.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | cut.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | cut.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | cut.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | cut.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | cut.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | hist.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | hist.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | to_struct.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 601 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 631 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 824 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 839 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked.rs | 1043 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | split.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | substring.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | substring.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | substring.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | substring.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | substring.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | substring.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | substring.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | json_path.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | json_path.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | json_path.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | json_path.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 637 | Clone in performance-critical code — consider references |
| HIGH | ? | extract.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | extract.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | extract.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | extract.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | extract.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | extract.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | concat.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 298 | Clone in performance-critical code — consider references |
| HIGH | ? | find_many.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | escape_regex.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | strip.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | strip.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | normalize.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | gather_skip_nulls.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | replace_time_zone.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | replace_time_zone.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | replace_time_zone.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | repeat_by.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | repeat_by.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | repeat_by.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | peaks.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | dispersion.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | min_max.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | sets.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 502 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 691 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 728 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 743 | Clone in performance-critical code — consider references |
| HIGH | ? | namespace.rs | 780 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | sum_mean.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | get.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | count.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | to_struct.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | to_struct.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 358 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | cross_join.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys_dispatch.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys_dispatch.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys_inner.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys_outer.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | single_keys_outer.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | groups.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch_left_right.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch_left_right.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch_left_right.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_join.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | unpivot.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | unpivot.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | unpivot.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | stats.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_frame.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_manager.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_manager.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_manager.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_manager.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_manager.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_manager.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 368 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | spill_token.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | task.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | task.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | task.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | wait_group.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | wait_group.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | linearizer.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | connector.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | connector.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | task_parker.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | distributor_channel.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | sql.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | arrow_c_stream.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | arrow_c_stream.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | import.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | import.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | c_interface.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | c_interface.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | numpy_ufunc.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | numpy_ufunc.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | scatter.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | buffers.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | buffers.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | buffers.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | buffers.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | buffers.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | map.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | map.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | map.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 578 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 597 | Clone in performance-critical code — consider references |
| HIGH | ? | construction.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | construction.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | exitable.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | optflags.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 744 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 852 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 911 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 1179 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 1545 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 1548 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_nodes.rs | 2013 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 474 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 485 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 523 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | visit.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | visit.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | visit.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 542 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 586 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 597 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 617 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 684 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 843 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 875 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 891 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 905 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 916 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 920 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 925 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 931 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 937 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 957 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 993 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1017 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1044 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1095 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1125 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1139 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1145 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1150 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1261 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1269 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1276 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1283 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1288 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1294 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1303 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1308 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1314 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1320 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1326 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1332 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1338 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1344 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1350 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1358 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1370 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1381 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1393 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1401 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1408 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1413 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1430 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1433 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1460 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1466 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1489 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1500 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1505 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1506 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1510 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1514 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1523 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1532 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1538 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1547 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1607 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1642 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1650 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1683 | Clone in performance-critical code — consider references |
| HIGH | ? | lazygroupby.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | lazygroupby.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | lazygroupby.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | lazygroupby.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | lazygroupby.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | lazygroupby.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | on_startup.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | on_startup.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | on_startup.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | on_startup.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | on_startup.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | on_startup.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | on_startup.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | io.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | whenthen.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | whenthen.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | whenthen.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | whenthen.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | whenthen.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | whenthen.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | eager.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | io.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | io.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | map.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | map.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | map.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | construction.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | construction.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | construction.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | to_numpy_series.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | to_numpy_series.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | to_numpy_df.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | to_py.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | to_py.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | to_py.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | to_py.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | to_py.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | to_rust.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | to_rust.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | to_rust.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | to_rust.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 355 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 475 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1473 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1968 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked_array.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 355 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | selector.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 8 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | datatype.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | name.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | struct.rs | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | struct.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | struct.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | struct.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | struct.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | struct.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | meta.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 420 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 471 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 476 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 485 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 493 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 517 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 533 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 578 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 583 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 618 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 622 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 684 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 688 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 698 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 702 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 714 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 720 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 737 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 746 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 751 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 754 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 765 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 774 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 783 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 787 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 790 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 795 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 804 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 816 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 843 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 853 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 859 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 865 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 883 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 900 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 904 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 910 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 916 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 920 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 924 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 928 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 932 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 936 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 939 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 945 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 949 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 961 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 982 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 993 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1009 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1026 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1038 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1059 | Clone in performance-critical code — consider references |
| HIGH | ? | general.rs | 1075 | Clone in performance-critical code — consider references |
| HIGH | ? | unity.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | deserialize.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | infer_schema.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | infer_schema.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | infer_schema.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | infer_schema.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | infer_schema.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | serde.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | new.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | new.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | new.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | new.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | new.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | named_from.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 477 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 517 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 555 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 560 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 567 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 647 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 691 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 695 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 708 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 712 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 746 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 748 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 750 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 888 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 893 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 907 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 931 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 938 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 956 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 963 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1055 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1056 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1066 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1067 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1210 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 754 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 756 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 760 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 775 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 787 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 919 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 922 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | amortized_iter.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | amortized_iter.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | comparison.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | comparison.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | comparison.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | comparison.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | comparison.rs | 418 | Clone in performance-critical code — consider references |
| HIGH | ? | comparison.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 479 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 635 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 639 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 645 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 654 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 677 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 730 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 756 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 777 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 779 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 812 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 865 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 911 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 980 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 583 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 600 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | series_trait.rs | 634 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 427 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 557 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | date.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | date.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | date.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | date.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | date.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 298 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 415 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 429 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_offset.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 417 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | floats.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | floats.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | object.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | object.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | borrowed.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | borrowed.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | borrowed.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | borrowed.rs | 480 | Clone in performance-critical code — consider references |
| HIGH | ? | borrowed.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | borrowed.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | list_utils.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 415 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 682 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 683 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 824 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 874 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 881 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 903 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 936 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 937 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 8 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 617 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 734 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 735 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 812 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | extend.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | extend.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | reshape.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | iceberg.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | iceberg.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | iceberg.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | iceberg.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | iceberg.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | field.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 521 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1182 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1350 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1355 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1367 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1377 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1390 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1397 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1404 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1411 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1551 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1575 | Clone in performance-critical code — consider references |
| HIGH | ? | dtype.rs | 1634 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 850 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 856 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 1019 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 1020 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 1063 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 1089 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 1127 | Clone in performance-critical code — consider references |
| HIGH | ? | any_value.rs | 1131 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 418 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 635 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 648 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | proptest.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | generic.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | generic.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | _serde.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | _serde.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | _serde.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | _serde.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | series.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | chunked_array.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | df.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | fmt.rs | 688 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 928 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1358 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1360 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1363 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1370 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1403 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 583 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 587 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | supertype.rs | 687 | Clone in performance-critical code — consider references |
| HIGH | ? | flatten.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | flatten.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 629 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 654 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 661 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 687 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 750 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 764 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 785 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 805 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 817 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 872 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 999 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1000 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1001 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_extension.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_extension.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | drop.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | null.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | anonymous.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | anonymous.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 506 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 616 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 622 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 645 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 650 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 652 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 687 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 690 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 692 | Clone in performance-critical code — consider references |
| HIGH | ? | cast.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | date.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | date.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | bitwise.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1021 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1321 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 313 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 359 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 417 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 418 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | numeric.rs | 431 | Clone in performance-critical code — consider references |
| HIGH | ? | from_iterator_par.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 359 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | iterator.rs | 470 | Clone in performance-critical code — consider references |
| HIGH | ? | float.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | time.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | chunkops.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | chunkops.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | chunkops.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | chunkops.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | chunkops.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | chunkops.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | chunkops.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 570 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 586 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 592 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 594 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 617 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 631 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 632 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_repr.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | extend.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | extend.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | extend.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | rolling_window.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | nulls.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | nulls.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | nulls.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | nulls.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | nulls.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | nulls.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 620 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 756 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 784 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 792 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 866 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | append.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | full.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | full.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | full.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | full.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | full.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | full.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | reverse.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | set.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | explode_and_offsets.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 430 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 472 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 620 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 623 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 714 | Clone in performance-critical code — consider references |
| HIGH | ? | quantile.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | quantile.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | quantile.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | quantile.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | shift.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | row_encode.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | row_encode.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | row_encode.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 298 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 356 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | zip.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 606 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 714 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 755 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 775 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 779 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 804 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 838 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 871 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 886 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 891 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 921 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 923 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 934 | Clone in performance-critical code — consider references |
| HIGH | ? | arity.rs | 936 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 555 | Clone in performance-critical code — consider references |
| HIGH | ? | apply.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | nesting_utils.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | nesting_utils.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | nesting_utils.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | nesting_utils.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | nesting_utils.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | nesting_utils.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | gather.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | gather.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | gather.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | fill_null.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | fill_null.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | fill_null.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | vector_hasher.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | vector_hasher.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | vector_hasher.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | vector_hasher.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | vector_hasher.rs | 521 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | explode.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 661 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 823 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 859 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 879 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1194 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1321 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1376 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1393 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1438 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1461 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1472 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1511 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1520 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1588 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1652 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1819 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1896 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1989 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2028 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2037 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2335 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2453 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2478 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2539 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2551 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2645 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2659 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2729 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2754 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3036 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 748 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 805 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 491 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 677 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 754 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | agg_list.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | categorical.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 358 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 477 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 535 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | into_groups.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | into_groups.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | position.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | position.rs | 730 | Clone in performance-critical code — consider references |
| HIGH | ? | position.rs | 760 | Clone in performance-critical code — consider references |
| HIGH | ? | hashing.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | broadcast.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | chunks.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | chunks.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | top_k.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 663 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 677 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 732 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 733 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 811 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 971 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 988 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1065 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1071 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1198 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1212 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1243 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1244 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1248 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1331 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1344 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1379 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1385 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1445 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1446 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1698 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | scalar.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | from.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | arithmetic.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | arithmetic.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | transpose.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | transpose.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 523 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 566 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 584 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 594 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 604 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 609 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 620 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 626 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 632 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 663 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 751 | Clone in performance-critical code — consider references |
| HIGH | ? | av_buffer.rs | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | tests.rs | 8 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | dyn_array.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | dyn_array.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | dyn_array.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 486 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 601 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 602 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 604 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 606 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 607 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 609 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 610 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 616 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 618 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 692 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 721 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 736 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | utf8_to.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary_to.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary_to.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal_to.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | temporal.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive_to.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive_to.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive_to.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive_to.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive_to.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive_to.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive_to.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_to.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | binview_to.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | binview_to.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | binview_to.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | binview_to.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | binview_to.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | view.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | view.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | view.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | view.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | array.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_nulls.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | struct_.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | rank.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | quantile.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | sum.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | sum.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | sum.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | sum.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | mean.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | mean.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | mean.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | mean.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | mean.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | primitive.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | binary.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | structure.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | fixed_size_list.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | binview.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | binview.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | trim_lists_to_normalized_offsets.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | trim_lists_to_normalized_offsets.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | trim_lists_to_normalized_offsets.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | trim_lists_to_normalized_offsets.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | trim_lists_to_normalized_offsets.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | trim_lists_to_normalized_offsets.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | dictionary.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | boolean.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_dictionary.rs | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | propagate_dictionary.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | signed.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | signed.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | signed.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | unsigned.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | unsigned.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 916 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | entry.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | eviction.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_lock.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_lock.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_lock.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_lock.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_lock.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_lock.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | glob.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 808 | Clone in performance-critical code — consider references |
| HIGH | ? | dns.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | dns.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | dns.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | dns.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | polars_object_store.rs | 683 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 361 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 384 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 475 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 556 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 594 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 629 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | object_store_setup.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | multipart_upload.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | multipart_upload.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | internal_writer.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | internal_writer.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | admission.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | admission.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | credential_provider.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | credential_provider.rs | 629 | Clone in performance-critical code — consider references |
| HIGH | ? | credential_provider.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | credential_provider.rs | 814 | Clone in performance-critical code — consider references |
| HIGH | ? | key_value_metadata.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | writer.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | batched_writer.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | mmap.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | async_impl.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 570 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | hugging_face.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | shared.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | shared.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | shared.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 431 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 493 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | predicates.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | hive.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | bytes_bufferer.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | bytes_bufferer.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | other.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | other.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | byte_source.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | byte_source.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | compression.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | compression.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | write_impl.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | write_impl.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | write_impl.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | write_impl.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | writer.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | writer.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | writer.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | schema_inference.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | schema_inference.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | schema_inference.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | read_impl.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 427 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 560 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 567 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 802 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 818 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | reader.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 890 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 892 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 894 | Clone in performance-critical code — consider references |
| HIGH | ? | core.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | write.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | write.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | read.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 471 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 355 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_stream.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_stream.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_stream.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_stream.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | mmap.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | mmap.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | mmap.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | mmap.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | mmap.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_reader_async.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_reader_async.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | ipc_file.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 526 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | round.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | truncate.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | truncate.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | truncate.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | truncate.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | truncate.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | truncate.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | truncate.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | upsample.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | upsample.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | upsample.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | upsample.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | upsample.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | upsample.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | offset_by.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | offset_by.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | offset_by.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | duration.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 362 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 562 | Clone in performance-critical code — consider references |
| HIGH | ? | dispatch.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 533 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | month_end.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | replace.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | month_start.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | encode.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | decode.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | decode.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | decode.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 466 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 523 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | merge_sorted.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | python_scan.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by_streaming.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by_streaming.rs | 309 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | projection.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | projection_utils.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | projection_utils.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | projection_utils.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | executor.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by_rolling.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by_rolling.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | join.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | stack.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | group_by_dynamic.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | sort.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | sort.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 495 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 542 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | lp.rs | 748 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 298 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 864 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 865 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 893 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 918 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 919 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 921 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 984 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 989 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1036 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1378 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1399 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1420 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1426 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1427 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1456 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1457 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1505 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1510 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1530 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1565 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1592 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1705 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1750 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1837 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1869 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1871 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1889 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1891 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1914 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1938 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1942 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1947 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1953 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 1961 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2005 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2022 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2030 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2031 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2034 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2037 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2152 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2153 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2179 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2180 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2241 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2245 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2258 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2279 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2285 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2302 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2320 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2410 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2426 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2435 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2442 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2448 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2455 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2462 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2463 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2510 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2512 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2517 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2519 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2528 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2530 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2533 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2543 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2553 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2688 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2691 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2749 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2773 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2819 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2829 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2833 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2838 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2855 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2857 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 2873 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 3090 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 3094 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 3177 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 3184 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 3189 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 3270 | Clone in performance-critical code — consider references |
| HIGH | ? | context.rs | 3272 | Clone in performance-critical code — consider references |
| HIGH | ? | table_functions.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | table_functions.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | table_functions.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | table_functions.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 407 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | subquery.rs | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_visitors.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_visitors.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_visitors.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_visitors.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_visitors.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 708 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 779 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 951 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 957 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 976 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 991 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 998 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1090 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1149 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1168 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1169 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1171 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1214 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1216 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1472 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1482 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1486 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1490 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1496 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1524 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1525 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1527 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1529 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1531 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1583 | Clone in performance-critical code — consider references |
| HIGH | ? | sql_expr.rs | 1648 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1243 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1332 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1339 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1340 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1341 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1343 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1353 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1355 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1417 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1475 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1482 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1484 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1486 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1488 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1489 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1499 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1501 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1577 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1581 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1596 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1597 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1767 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 1992 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2016 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2208 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2214 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2306 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2324 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2449 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2458 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2460 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2520 | Clone in performance-critical code — consider references |
| HIGH | ? | functions.rs | 2585 | Clone in performance-critical code — consider references |
| HIGH | ? | distances.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | expressions.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | expressions.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | expressions.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 545 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.py | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | dataframe.py | 1385 | Clone in performance-critical code — consider references |
| HIGH | ? | series.py | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.py | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | slice.py | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | series.py | 853 | Clone in performance-critical code — consider references |
| HIGH | ? | series.py | 1428 | Clone in performance-critical code — consider references |
| HIGH | ? | series.py | 1431 | Clone in performance-critical code — consider references |
| HIGH | ? | series.py | 3053 | Clone in performance-critical code — consider references |
| HIGH | ? | series.py | 5537 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 765 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 4808 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 5066 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 5224 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 1611 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 1614 | Clone in performance-critical code — consider references |
| HIGH | ? | frame.py | 9248 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| L | ? | _providers.py | 158 |
| L | ? | _providers.py | 520 |
| L | ? | udfs.py | 366 |
| L | ? | udfs.py | 778 |
| L | ? | udfs.py | 1236 |
| M | ? | run.py | 75 |
| M | ? | run.py | 81 |
| M | ? | run.py | 14 |
| M | ? | run.py | 17 |
| M | ? | run.py | 21 |
| M | ? | run.py | 22 |
| M | ? | _providers.py | 193 |
| M | ? | _providers.py | 224 |
| M | ? | _sink.py | 239 |
| M | ? | _utils.py | 105 |
| M | ? | _utils.py | 279 |
| M | ? | _utils.py | 424 |
| M | ? | _utils.py | 552 |
| M | ? | _utils.py | 567 |
| M | ? | _utils.py | 568 |
| M | ? | _utils.py | 577 |
| M | ? | _utils.py | 723 |
| M | ? | _utils.py | 724 |
| M | ? | _dataset.py | 76 |
| M | ? | _dataset.py | 107 |
| M | ? | _dataset.py | 238 |
| M | ? | _dataset.py | 258 |
| M | ? | _dataset.py | 327 |
| M | ? | _dataset.py | 331 |
| M | ? | _dataset.py | 356 |
| M | ? | _plr.py | 102 |
| M | ? | ext.py | 38 |
| M | ? | series.py | 861 |
| M | ? | series.py | 881 |
| M | ? | series.py | 887 |
| M | ? | series.py | 894 |
| M | ? | series.py | 903 |
| M | ? | series.py | 1687 |
| M | ? | extension.py | 33 |
| M | ? | extension.py | 38 |
| M | ? | extension.py | 39 |
| M | ? | extension.py | 40 |
| M | ? | classes.py | 759 |
| M | ? | classes.py | 760 |
| M | ? | lazy.py | 1333 |
| M | ? | lazy.py | 1334 |
| H | ? | config.py | 266 |
| H | ? | config.py | 280 |
| H | ? | config.py | 461 |
| H | ? | frame.py | 4417 |
| H | ? | frame.py | 4445 |
| H | ? | udfs.py | 626 |
| H | ? | frame.py | 4286 |
| H | ? | frame.py | 4287 |
| C | ? | various.py | 679 |
| M | ? | _executor.py | 498 |
| M | ? | _executor.py | 507 |
| M | ? | frame.py | 3042 |
| M | ? | frame.py | 3692 |
| M | ? | frame.py | 4048 |
| M | ? | frame.py | 4315 |
| M | ? | frame.py | 9186 |
| M | ? | frame.py | 12710 |
| C | GS001 | flake.nix | 144 |
| C | GS001 | flake.nix | 156 |
| C | GS001 | flake.nix | 161 |
| C | GS001 | flake.nix | 166 |
| C | GS001 | flake.nix | 171 |
| C | GS001 | flake.nix | 176 |
| C | GS001 | flake.nix | 181 |
| C | GS001 | flake.nix | 186 |
| C | GS001 | flake.nix | 199 |
| C | GS001 | flake.nix | 204 |
| C | GS001 | flake.nix | 209 |
| C | GS001 | flake.nix | 214 |
| C | GS001 | flake.nix | 225 |
| C | GS001 | flake.nix | 244 |
| C | GS001 | frame.py | 4418 |
| L | GS003 | launch.py | 61 |
| L | GS003 | logging.py | 19 |
| L | GS003 | client.py | 673 |
| L | GS003 | client.py | 682 |
| L | GS003 | frame.py | 5908 |
| L | GS003 | _builder.py | 222 |
| L | GS003 | plugins.py | 88 |
| L | GS003 | versions.py | 51 |
| L | GS003 | versions.py | 53 |
| L | GS003 | versions.py | 54 |
| L | GS003 | versions.py | 55 |
| L | GS003 | versions.py | 56 |
| L | GS003 | versions.py | 57 |
| L | GS003 | versions.py | 58 |
| L | GS003 | versions.py | 62 |
| L | GS003 | versions.py | 64 |
| L | GS003 | versions.py | 67 |
| L | GS003 | versions.py | 68 |
| L | GS003 | run.py | 37 |
| L | GS003 | run.py | 60 |
| L | GS003 | run.py | 82 |
| L | GS003 | run.py | 5 |
| L | GS003 | run.py | 7 |
| L | GS003 | run.py | 12 |
| L | GS003 | run.py | 15 |
| L | GS003 | cargo-fail-warning.py | 27 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | lib.rs | 27 |
| L | GS003 | lib.rs | 28 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | mod.rs | 1114 |
| L | GS003 | mod.rs | 1115 |
| L | GS003 | mod.rs | 1116 |
| L | GS003 | mod.rs | 1117 |
| L | GS003 | mod.rs | 1131 |
| L | GS003 | mod.rs | 763 |
| L | GS003 | config.rs | 42 |
| L | GS003 | time_zone.rs | 68 |
| L | GS003 | into_groups.rs | 67 |
| L | GS003 | df.rs | 111 |
| L | GS003 | df.rs | 119 |
| L | GS003 | df.rs | 141 |
| L | GS003 | warning.rs | 7 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | eval.rs | 285 |
| L | GS003 | ternary.rs | 166 |
| L | GS003 | ternary.rs | 174 |
| L | GS003 | ternary.rs | 228 |
| L | GS003 | ternary.rs | 249 |
| L | GS003 | ternary.rs | 314 |
| L | GS003 | execution_state.rs | 248 |
| L | GS003 | execution_state.rs | 268 |
| L | GS003 | execution_state.rs | 274 |
| L | GS003 | admission.rs | 152 |
| L | GS003 | mod.rs | 201 |
| L | GS003 | mod.rs | 269 |
| L | GS003 | mod.rs | 297 |
| L | GS003 | model.rs | 78 |
| L | GS003 | regime.rs | 145 |
| L | GS003 | concurrency_config.rs | 14 |
| L | GS003 | concurrency_config.rs | 27 |
| L | GS003 | concurrency_config.rs | 40 |
| L | GS003 | credential_provider.rs | 453 |
| L | GS003 | credential_provider.rs | 479 |
| L | GS003 | credential_provider.rs | 496 |
| L | GS003 | dns.rs | 126 |
| L | GS003 | dns.rs | 276 |
| L | GS003 | object_store_setup.rs | 76 |
| L | GS003 | object_store_setup.rs | 90 |
| L | GS003 | object_store_setup.rs | 233 |
| L | GS003 | object_store_setup.rs | 376 |
| L | GS003 | options.rs | 169 |
| L | GS003 | options.rs | 583 |
| L | GS003 | options.rs | 734 |
| L | GS003 | options.rs | 746 |
| L | GS003 | options.rs | 764 |
| L | GS003 | polars_object_store.rs | 185 |
| L | GS003 | configs.rs | 58 |
| L | GS003 | configs.rs | 78 |
| L | GS003 | cache.rs | 19 |
| L | GS003 | cache.rs | 114 |
| L | GS003 | cache.rs | 132 |
| L | GS003 | cache.rs | 142 |
| L | GS003 | cache_lock.rs | 39 |
| L | GS003 | cache_lock.rs | 45 |
| L | GS003 | cache_lock.rs | 52 |
| L | GS003 | entry.rs | 66 |
| L | GS003 | entry.rs | 77 |
| L | GS003 | entry.rs | 101 |
| L | GS003 | entry.rs | 128 |
| L | GS003 | entry.rs | 138 |
| L | GS003 | entry.rs | 175 |
| L | GS003 | entry.rs | 195 |
| L | GS003 | eviction.rs | 84 |
| L | GS003 | eviction.rs | 102 |
| L | GS003 | eviction.rs | 113 |
| L | GS003 | eviction.rs | 126 |
| L | GS003 | eviction.rs | 137 |
| L | GS003 | eviction.rs | 143 |
| L | GS003 | eviction.rs | 157 |
| L | GS003 | eviction.rs | 183 |
| L | GS003 | eviction.rs | 196 |
| L | GS003 | ipc_file.rs | 134 |
| L | GS003 | ipc_file.rs | 227 |
| L | GS003 | mmap.rs | 98 |
| L | GS003 | read_impl.rs | 73 |
| L | GS003 | read_impl.rs | 138 |
| L | GS003 | mod.rs | 24 |
| L | GS003 | mod.rs | 31 |
| L | GS003 | mod.rs | 42 |
| L | GS003 | pl_async.rs | 123 |
| L | GS003 | shared.rs | 82 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | mod.rs | 882 |
| L | GS003 | cache.rs | 67 |
| L | GS003 | cache.rs | 77 |
| L | GS003 | cache.rs | 125 |
| L | GS003 | cache.rs | 141 |
| L | GS003 | cache.rs | 153 |
| L | GS003 | executor.rs | 32 |
| L | GS003 | ext_context.rs | 13 |
| L | GS003 | filter.rs | 123 |
| L | GS003 | filter.rs | 138 |
| L | GS003 | group_by.rs | 126 |
| L | GS003 | group_by.rs | 130 |
| L | GS003 | group_by_dynamic.rs | 95 |
| L | GS003 | group_by_rolling.rs | 128 |
| L | GS003 | group_by_streaming.rs | 188 |
| L | GS003 | group_by_streaming.rs | 193 |
| L | GS003 | group_by_streaming.rs | 198 |
| L | GS003 | group_by_streaming.rs | 203 |
| L | GS003 | group_by_streaming.rs | 228 |
| L | GS003 | group_by_streaming.rs | 235 |
| L | GS003 | group_by_streaming.rs | 240 |
| L | GS003 | group_by_streaming.rs | 248 |
| L | GS003 | group_by_streaming.rs | 266 |
| L | GS003 | hconcat.rs | 15 |
| L | GS003 | hconcat.rs | 22 |
| L | GS003 | hconcat.rs | 36 |
| L | GS003 | join.rs | 46 |
| L | GS003 | join.rs | 50 |
| L | GS003 | join.rs | 114 |
| L | GS003 | merge_sorted.rs | 42 |
| L | GS003 | projection.rs | 91 |
| L | GS003 | python_scan.rs | 59 |
| L | GS003 | slice.rs | 14 |
| L | GS003 | sort.rs | 55 |
| L | GS003 | stack.rs | 118 |
| L | GS003 | udf.rs | 14 |
| L | GS003 | union.rs | 18 |
| L | GS003 | union.rs | 33 |
| L | GS003 | union.rs | 35 |
| L | GS003 | union.rs | 85 |
| L | GS003 | unique.rs | 14 |
| L | GS003 | functions.rs | 126 |
| L | GS003 | functions.rs | 127 |
| L | GS003 | functions.rs | 155 |
| L | GS003 | functions.rs | 156 |
| L | GS003 | functions.rs | 158 |
| L | GS003 | functions.rs | 163 |
| L | GS003 | functions.rs | 164 |
| L | GS003 | functions.rs | 168 |
| L | GS003 | functions.rs | 228 |
| L | GS003 | functions.rs | 264 |
| L | GS003 | functions.rs | 281 |
| L | GS003 | functions.rs | 320 |
| L | GS003 | functions.rs | 406 |
| L | GS003 | stats.rs | 56 |
| L | GS003 | spill_file.rs | 80 |
| L | GS003 | spill_file.rs | 88 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | sort_merge.rs | 238 |
| L | GS003 | sort_merge.rs | 246 |
| L | GS003 | sort_merge.rs | 274 |
| L | GS003 | sort_merge.rs | 337 |
| L | GS003 | sort_merge.rs | 346 |
| L | GS003 | mod.rs | 183 |
| L | GS003 | mod.rs | 196 |
| L | GS003 | mod.rs | 704 |
| L | GS003 | mod.rs | 804 |
| L | GS003 | reader.rs | 264 |
| L | GS003 | reader.rs | 291 |
| L | GS003 | reader.rs | 315 |
| L | GS003 | build.rs | 7 |
| L | GS003 | build.rs | 10 |
| L | GS003 | build.rs | 35 |
| L | GS003 | dsl-schema.rs | 89 |
| L | GS003 | dsl-schema.rs | 98 |
| L | GS003 | dsl-schema.rs | 100 |
| L | GS003 | dsl-schema.rs | 101 |
| L | GS003 | dsl-schema.rs | 105 |
| L | GS003 | plan.rs | 326 |
| L | GS003 | plan.rs | 355 |
| L | GS003 | expr_expansion.rs | 66 |
| L | GS003 | scans.rs | 1137 |
| L | GS003 | scans.rs | 1181 |
| L | GS003 | scans.rs | 1220 |
| L | GS003 | scans.rs | 1257 |
| L | GS003 | scans.rs | 1448 |
| L | GS003 | debug.rs | 7 |
| L | GS003 | debug.rs | 10 |
| L | GS003 | debug.rs | 12 |
| L | GS003 | expr_ir.rs | 263 |
| L | GS003 | cache_states.rs | 368 |
| L | GS003 | csee.rs | 841 |
| L | GS003 | expand_datasets.rs | 244 |
| L | GS003 | expand_datasets.rs | 522 |
| L | GS003 | mod.rs | 150 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | dataset_provider_funcs.rs | 55 |
| L | GS003 | on_startup.rs | 93 |
| L | GS003 | on_startup.rs | 101 |
| L | GS003 | timeout.rs | 54 |
| L | GS003 | timeout.rs | 79 |
| L | GS003 | timeout.rs | 81 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | execute.rs | 331 |
| L | GS003 | execute.rs | 351 |
| L | GS003 | execute.rs | 379 |
| L | GS003 | graph.rs | 103 |
| L | GS003 | graph.rs | 123 |
| L | GS003 | partition_distributor.rs | 206 |
| L | GS003 | partition_distributor.rs | 293 |
| L | GS003 | partition_distributor.rs | 299 |
| L | GS003 | mod.rs | 93 |
| L | GS003 | mod.rs | 164 |
| L | GS003 | partition_by.rs | 116 |
| L | GS003 | partition_by.rs | 207 |
| L | GS003 | single_file.rs | 96 |
| L | GS003 | single_file.rs | 142 |
| L | GS003 | single_file.rs | 147 |
| L | GS003 | mod.rs | 70 |
| L | GS003 | mod.rs | 57 |
| L | GS003 | mod.rs | 60 |
| L | GS003 | mod.rs | 63 |
| L | GS003 | batch.rs | 214 |
| L | GS003 | batch.rs | 270 |
| L | GS003 | builder.rs | 69 |
| L | GS003 | line_batch_source.rs | 52 |
| L | GS003 | line_batch_source.rs | 86 |
| L | GS003 | mod.rs | 350 |
| L | GS003 | mod.rs | 451 |
| L | GS003 | builder.rs | 88 |
| L | GS003 | metadata.rs | 55 |
| L | GS003 | metadata.rs | 77 |
| L | GS003 | mod.rs | 270 |
| L | GS003 | mod.rs | 314 |
| L | GS003 | mod.rs | 317 |
| L | GS003 | mod.rs | 377 |
| L | GS003 | mod.rs | 622 |
| L | GS003 | record_batch_data_fetch.rs | 199 |
| L | GS003 | lines.rs | 62 |
| L | GS003 | row_deletions.rs | 123 |
| L | GS003 | row_deletions.rs | 143 |
| L | GS003 | row_deletions.rs | 273 |
| L | GS003 | resolve_slice.rs | 60 |
| L | GS003 | resolve_slice.rs | 125 |
| L | GS003 | resolve_slice.rs | 198 |
| L | GS003 | resolve_slice.rs | 219 |
| L | GS003 | mod.rs | 142 |
| L | GS003 | mod.rs | 271 |
| L | GS003 | initialization.rs | 43 |
| L | GS003 | initialization.rs | 113 |
| L | GS003 | initialization.rs | 135 |
| L | GS003 | initialization.rs | 143 |
| L | GS003 | initialization.rs | 214 |
| L | GS003 | initialization.rs | 228 |
| L | GS003 | initialization.rs | 257 |
| L | GS003 | initialization.rs | 301 |
| L | GS003 | initialization.rs | 356 |
| L | GS003 | attach_reader_to_bridge.rs | 33 |
| L | GS003 | post_apply_extra_ops.rs | 149 |
| L | GS003 | reader_starter.rs | 100 |
| L | GS003 | reader_starter.rs | 109 |
| L | GS003 | reader_starter.rs | 123 |
| L | GS003 | reader_starter.rs | 129 |
| L | GS003 | reader_starter.rs | 250 |
| L | GS003 | reader_starter.rs | 292 |
| L | GS003 | reader_starter.rs | 396 |
| L | GS003 | reader_starter.rs | 488 |
| L | GS003 | reader_starter.rs | 648 |
| L | GS003 | reader_starter.rs | 674 |
| L | GS003 | builder.rs | 69 |
| L | GS003 | line_batch_distributor.rs | 41 |
| L | GS003 | line_batch_distributor.rs | 84 |
| L | GS003 | line_batch_distributor.rs | 151 |
| L | GS003 | line_batch_processor.rs | 49 |
| L | GS003 | line_batch_processor.rs | 74 |
| L | GS003 | line_batch_processor.rs | 87 |
| L | GS003 | mod.rs | 244 |
| L | GS003 | mod.rs | 283 |
| L | GS003 | mod.rs | 309 |
| L | GS003 | mod.rs | 514 |
| L | GS003 | mod.rs | 525 |
| L | GS003 | mod.rs | 551 |
| L | GS003 | mod.rs | 563 |
| L | GS003 | mod.rs | 577 |
| L | GS003 | negative_slice_pass.rs | 48 |
| L | GS003 | negative_slice_pass.rs | 71 |
| L | GS003 | negative_slice_pass.rs | 78 |
| L | GS003 | negative_slice_pass.rs | 101 |
| L | GS003 | negative_slice_pass.rs | 107 |
| L | GS003 | negative_slice_pass.rs | 114 |
| L | GS003 | negative_slice_pass.rs | 151 |
| L | GS003 | row_index_limit_pass.rs | 34 |
| L | GS003 | row_index_limit_pass.rs | 89 |
| L | GS003 | builder.rs | 108 |
| L | GS003 | init.rs | 51 |
| L | GS003 | init.rs | 141 |
| L | GS003 | init.rs | 358 |
| L | GS003 | metadata_utils.rs | 62 |
| L | GS003 | metadata_utils.rs | 84 |
| L | GS003 | mod.rs | 248 |
| L | GS003 | mod.rs | 276 |
| L | GS003 | mod.rs | 464 |
| L | GS003 | statistics.rs | 163 |
| L | GS003 | pipeline_budget.rs | 70 |
| L | GS003 | equi_join.rs | 327 |
| L | GS003 | equi_join.rs | 347 |
| L | GS003 | equi_join.rs | 381 |
| L | GS003 | lower_ir.rs | 664 |
| L | GS003 | lower_ir.rs | 684 |
| L | GS003 | skeleton.rs | 221 |
| L | GS003 | skeleton.rs | 225 |
| L | GS003 | skeleton.rs | 227 |
| L | GS003 | test.rs | 82 |
| L | GS003 | build.rs | 2 |
| L | GS003 | build.rs | 5 |
| L | GS003 | mem.rs | 169 |
| L | GS003 | sys.rs | 29 |
| L | GS003 | build.rs | 4 |
| L | GS003 | build.rs | 5 |
| L | GS003 | build.rs | 4 |
| L | GS003 | build.rs | 5 |
| L | GS003 | build.rs | 4 |
| L | GS003 | build.rs | 5 |
| L | GS003 | build.rs | 4 |
| L | GS003 | build.rs | 5 |
| L | GS003 | lib.rs | 23 |
| L | GS003 | derive.rs | 51 |
| L | GS008 | frame.py | 187 |
| C | ? | utils.rs | 67 |
| C | ? | _executor.py | 498 |
| M | ? | template.py | 32 |
| M | ? | template.py | 37 |
| H | ? | launch.py | 76 |
| H | ? | _dataset.py | 114 |
| H | ? | array.py | 819 |
| H | ? | series.py | 5296 |
| H | ? | series.py | 6216 |
| H | ? | list.py | 1002 |
| H | ? | array.py | 385 |
| H | ? | array.py | 597 |
| H | ? | array.py | 1018 |
| H | ? | list.py | 479 |
| H | ? | list.py | 507 |
| H | ? | list.py | 1323 |
| H | ? | dprint.json | 0 |
| H | ? | mkdocs.yml | 0 |
| H | GS004 | launch.py | 76 |
| H | GS004 | various.py | 679 |
| C | GS005 | frame.py | 4600 |
| I | GS007 | frame.py | 1165 |
| I | GS007 | frame.py | 2775 |
| I | GS007 | frame.py | 10000 |
| I | GS007 | _inference.py | 119 |
| I | GS007 | _inference.py | 130 |
| I | GS007 | functions.py | 1114 |
| s | GS009 |  | 0 |
| L | GS012 | config.py | 266 |
| L | GS012 | config.py | 280 |
| L | GS012 | config.py | 322 |
| L | GS012 | config.py | 358 |
| L | GS012 | config.py | 417 |
| L | GS012 | config.py | 461 |
| H | GS014 | frame.py | 4417 |
| H | GS014 | frame.py | 4445 |
| H | GS014 | functions.py | 367 |
| H | GS014 | functions.py | 438 |
| H | GS014 | functions.py | 445 |
| H | GS014 | functions.py | 458 |
| M | ? | various.py | 679 |
| H | ? | mod.rs | 104 |
| H | ? | mod.rs | 148 |
| H | ? | mod.rs | 194 |
| H | ? | mod.rs | 197 |
| H | ? | mod.rs | 199 |
| H | ? | mod.rs | 242 |
| H | ? | array.rs | 363 |
| H | ? | array.rs | 407 |
| H | ? | array.rs | 455 |
| H | ? | array.rs | 498 |
| H | ? | mod.rs | 104 |
| H | ? | mod.rs | 132 |
| H | ? | mod.rs | 150 |
| H | ? | mod.rs | 152 |
| H | ? | mod.rs | 165 |
| H | ? | mod.rs | 174 |
| H | ? | mod.rs | 179 |
| H | ? | mod.rs | 191 |
| H | ? | mod.rs | 204 |
| H | ? | list.rs | 40 |
| H | ? | map.rs | 39 |
| H | ? | binview.rs | 23 |
| H | ? | deserialize.rs | 25 |
| H | ? | deserialize.rs | 48 |
| H | ? | deserialize.rs | 61 |
| H | ? | schema.rs | 35 |
| H | ? | nested.rs | 79 |
| H | ? | nested.rs | 89 |
| H | ? | nested.rs | 135 |
| H | ? | nested.rs | 165 |
| H | ? | nested.rs | 167 |
| H | ? | nested.rs | 176 |
| H | ? | nested.rs | 178 |
| H | ? | nested.rs | 276 |
| H | ? | nested.rs | 287 |
| H | ? | boolean.rs | 20 |
| H | ? | common.rs | 290 |
| H | ? | common.rs | 506 |
| H | ? | schema.rs | 89 |
| H | ? | schema.rs | 292 |
| H | ? | mod.rs | 139 |
| H | ? | mod.rs | 263 |
| H | ? | mod.rs | 297 |
| H | ? | mod.rs | 317 |
| H | ? | primitive.rs | 29 |
| H | ? | deserialize.rs | 34 |
| H | ? | common.rs | 290 |
| H | ? | common.rs | 294 |
| H | ? | common.rs | 328 |
| H | ? | common.rs | 364 |
| H | ? | common.rs | 365 |
| H | ? | common.rs | 371 |
| H | ? | common.rs | 372 |
| H | ? | common.rs | 374 |
| H | ? | dictionary.rs | 42 |
| H | ? | schema.rs | 402 |
| H | ? | offset.rs | 664 |
| H | ? | offset.rs | 665 |
| H | ? | field.rs | 49 |
| H | ? | field.rs | 112 |
| H | ? | field.rs | 115 |
| H | ? | mod.rs | 340 |
| H | ? | mod.rs | 394 |
| H | ? | mod.rs | 398 |
| H | ? | mod.rs | 403 |
| H | ? | mod.rs | 412 |
| H | ? | mod.rs | 421 |
| H | ? | mod.rs | 589 |
| H | ? | mod.rs | 69 |
| H | ? | mod.rs | 70 |
| H | ? | mod.rs | 187 |
| H | ? | mod.rs | 448 |
| H | ? | mod.rs | 630 |
| H | ? | ffi.rs | 85 |
| H | ? | iterator.rs | 139 |
| H | ? | mod.rs | 119 |
| H | ? | mod.rs | 127 |
| H | ? | mod.rs | 159 |
| H | ? | mod.rs | 180 |
| H | ? | mod.rs | 198 |
| H | ? | mod.rs | 208 |
| H | ? | mod.rs | 351 |
| H | ? | mod.rs | 369 |
| H | ? | mod.rs | 376 |
| H | ? | ffi.rs | 14 |
| H | ? | ffi.rs | 27 |
| H | ? | ffi.rs | 33 |
| H | ? | proptest.rs | 17 |
| H | ? | proptest.rs | 19 |
| H | ? | proptest.rs | 24 |
| H | ? | mutable.rs | 36 |
| H | ? | mutable.rs | 43 |
| H | ? | mutable.rs | 175 |
| H | ? | mutable.rs | 185 |
| H | ? | builder.rs | 48 |
| H | ? | static_array.rs | 398 |
| H | ? | static_array.rs | 400 |
| H | ? | null.rs | 101 |
| H | ? | null.rs | 143 |
| H | ? | null.rs | 185 |
| H | ? | null.rs | 199 |
| H | ? | null.rs | 204 |
| H | ? | null.rs | 214 |
| H | ? | null.rs | 244 |
| H | ? | proptest.rs | 127 |
| H | ? | proptest.rs | 134 |
| H | ? | proptest.rs | 135 |
| H | ? | proptest.rs | 143 |
| H | ? | proptest.rs | 144 |
| H | ? | proptest.rs | 269 |
| H | ? | proptest.rs | 275 |
| H | ? | mod.rs | 154 |
| H | ? | mod.rs | 155 |
| H | ? | mod.rs | 156 |
| H | ? | mod.rs | 157 |
| H | ? | mod.rs | 159 |
| H | ? | mod.rs | 306 |
| H | ? | mod.rs | 319 |
| H | ? | mod.rs | 569 |
| H | ? | mod.rs | 571 |
| H | ? | mod.rs | 656 |
| H | ? | mod.rs | 657 |
| H | ? | mod.rs | 658 |
| H | ? | mod.rs | 671 |
| H | ? | mod.rs | 672 |
| H | ? | mod.rs | 673 |
| H | ? | mod.rs | 746 |
| H | ? | mod.rs | 752 |
| H | ? | mod.rs | 768 |
| H | ? | mod.rs | 770 |
| H | ? | mod.rs | 776 |
| H | ? | mod.rs | 778 |
| H | ? | ffi.rs | 37 |
| H | ? | ffi.rs | 44 |
| H | ? | ffi.rs | 46 |
| H | ? | ffi.rs | 47 |
| H | ? | ffi.rs | 49 |
| H | ? | ffi.rs | 57 |
| H | ? | proptest.rs | 10 |
| H | ? | proptest.rs | 28 |
| H | ? | mutable.rs | 44 |
| H | ? | mutable.rs | 45 |
| H | ? | mutable.rs | 46 |
| H | ? | mutable.rs | 47 |
| H | ? | mutable.rs | 211 |
| H | ? | mutable.rs | 242 |
| H | ? | builder.rs | 94 |
| H | ? | builder.rs | 159 |
| H | ? | builder.rs | 267 |
| H | ? | mod.rs | 203 |
| H | ? | mod.rs | 233 |
| H | ? | mod.rs | 246 |
| H | ? | mod.rs | 435 |
| H | ? | mod.rs | 449 |
| H | ? | mod.rs | 451 |
| H | ? | mod.rs | 454 |
| H | ? | mod.rs | 456 |
| H | ? | ffi.rs | 18 |
| H | ? | ffi.rs | 20 |
| H | ? | ffi.rs | 31 |
| H | ? | mutable.rs | 90 |
| H | ? | mutable.rs | 111 |
| H | ? | mutable.rs | 154 |
| H | ? | mod.rs | 433 |
| H | ? | mod.rs | 461 |
| H | ? | mod.rs | 463 |
| H | ? | mod.rs | 467 |
| H | ? | mod.rs | 469 |
| H | ? | ffi.rs | 36 |
| H | ? | ffi.rs | 43 |
| H | ? | ffi.rs | 45 |
| H | ? | ffi.rs | 46 |
| H | ? | ffi.rs | 53 |
| H | ? | builder.rs | 52 |
| H | ? | mod.rs | 513 |
| H | ? | mod.rs | 529 |
| H | ? | mod.rs | 534 |
| H | ? | mod.rs | 544 |
| H | ? | mod.rs | 548 |
| H | ? | ffi.rs | 35 |
| H | ? | ffi.rs | 42 |
| H | ? | ffi.rs | 44 |
| H | ? | ffi.rs | 51 |
| H | ? | proptest.rs | 13 |
| H | ? | fmt.rs | 78 |
| H | ? | fmt.rs | 87 |
| H | ? | mutable.rs | 420 |
| H | ? | mutable.rs | 429 |
| H | ? | builder.rs | 48 |
| H | ? | mod.rs | 494 |
| H | ? | mod.rs | 495 |
| H | ? | mod.rs | 496 |
| H | ? | mod.rs | 514 |
| H | ? | mod.rs | 516 |
| H | ? | mod.rs | 520 |
| H | ? | mod.rs | 522 |
| H | ? | mod.rs | 538 |
| H | ? | ffi.rs | 36 |
| H | ? | ffi.rs | 43 |
| H | ? | ffi.rs | 45 |
| H | ? | ffi.rs | 46 |
| H | ? | ffi.rs | 53 |
| H | ? | mod.rs | 130 |
| H | ? | mod.rs | 143 |
| H | ? | mod.rs | 271 |
| H | ? | mod.rs | 294 |
| H | ? | mod.rs | 300 |
| H | ? | ffi.rs | 14 |
| H | ? | ffi.rs | 22 |
| H | ? | ffi.rs | 36 |
| H | ? | proptest.rs | 16 |
| H | ? | proptest.rs | 20 |
| H | ? | proptest.rs | 29 |
| H | ? | builder.rs | 57 |
| H | ? | mod.rs | 83 |
| H | ? | mod.rs | 94 |
| H | ? | mod.rs | 193 |
| H | ? | mod.rs | 208 |
| H | ? | mod.rs | 210 |
| H | ? | mod.rs | 214 |
| H | ? | mod.rs | 216 |
| H | ? | ffi.rs | 20 |
| H | ? | ffi.rs | 41 |
| H | ? | ffi.rs | 48 |
| H | ? | ffi.rs | 50 |
| H | ? | ffi.rs | 51 |
| H | ? | ffi.rs | 58 |
| H | ? | mod.rs | 93 |
| H | ? | mod.rs | 100 |
| H | ? | mod.rs | 254 |
| H | ? | mod.rs | 269 |
| H | ? | mod.rs | 272 |
| H | ? | mod.rs | 275 |
| H | ? | mod.rs | 278 |
| H | ? | ffi.rs | 20 |
| H | ? | ffi.rs | 41 |
| H | ? | ffi.rs | 48 |
| H | ? | ffi.rs | 50 |
| H | ? | ffi.rs | 51 |
| H | ? | ffi.rs | 58 |
| H | ? | proptest.rs | 19 |
| H | ? | proptest.rs | 32 |
| H | ? | proptest.rs | 35 |
| H | ? | proptest.rs | 36 |
| H | ? | proptest.rs | 38 |
| H | ? | mutable.rs | 27 |
| H | ? | mutable.rs | 34 |
| H | ? | mutable.rs | 127 |
| H | ? | mutable.rs | 138 |
| H | ? | mutable.rs | 150 |
| H | ? | mutable.rs | 198 |
| H | ? | mutable.rs | 277 |
| H | ? | mutable.rs | 287 |
| H | ? | builder.rs | 51 |
| H | ? | mod.rs | 201 |
| H | ? | mod.rs | 274 |
| H | ? | mod.rs | 355 |
| H | ? | mod.rs | 362 |
| H | ? | mod.rs | 405 |
| H | ? | mod.rs | 420 |
| H | ? | mod.rs | 425 |
| H | ? | ffi.rs | 34 |
| H | ? | ffi.rs | 41 |
| H | ? | ffi.rs | 43 |
| H | ? | ffi.rs | 50 |
| H | ? | proptest.rs | 10 |
| H | ? | builder.rs | 45 |
| H | ? | mod.rs | 238 |
| H | ? | mod.rs | 255 |
| H | ? | mod.rs | 261 |
| H | ? | ffi.rs | 34 |
| H | ? | ffi.rs | 42 |
| H | ? | ffi.rs | 44 |
| H | ? | ffi.rs | 51 |
| H | ? | builder.rs | 56 |
| H | ? | mod.rs | 178 |
| H | ? | mod.rs | 202 |
| H | ? | mod.rs | 398 |
| H | ? | mod.rs | 400 |
| H | ? | mod.rs | 406 |
| H | ? | mod.rs | 408 |
| H | ? | ffi.rs | 22 |
| H | ? | ffi.rs | 30 |
| H | ? | ffi.rs | 36 |
| H | ? | builder.rs | 343 |
| H | ? | builder.rs | 344 |
| H | ? | builder.rs | 346 |
| H | ? | builder.rs | 348 |
| H | ? | builder.rs | 349 |
| H | ? | builder.rs | 355 |
| H | ? | builder.rs | 364 |
| H | ? | builder.rs | 373 |
| H | ? | builder.rs | 375 |
| H | ? | builder.rs | 376 |
| H | ? | arity_assign.rs | 63 |
| H | ? | bitwise.rs | 15 |
| H | ? | bitwise.rs | 25 |
| H | ? | bitwise.rs | 35 |
| H | ? | bitwise.rs | 44 |
| H | ? | bitwise.rs | 54 |
| H | ? | bitwise.rs | 64 |
| H | ? | bitwise.rs | 74 |
| H | ? | concatenate.rs | 115 |
| H | ? | concatenate.rs | 121 |
| H | ? | concatenate.rs | 134 |
| H | ? | concatenate.rs | 149 |
| H | ? | concatenate.rs | 178 |
| H | ? | concatenate.rs | 209 |
| H | ? | concatenate.rs | 270 |
| H | ? | concatenate.rs | 350 |
| H | ? | concatenate.rs | 398 |
| H | ? | concatenate.rs | 422 |
| H | ? | concatenate.rs | 438 |
| H | ? | utils.rs | 19 |
| H | ? | utils.rs | 20 |
| H | ? | utils.rs | 21 |
| H | ? | utils.rs | 29 |
| H | ? | utils.rs | 30 |
| H | ? | utils.rs | 49 |
| H | ? | conversion.rs | 21 |
| H | ? | mod.rs | 75 |
| H | ? | mod.rs | 207 |
| H | ? | mod.rs | 210 |
| H | ? | mod.rs | 228 |
| H | ? | mod.rs | 240 |
| H | ? | mod.rs | 247 |
| H | ? | list.rs | 117 |
| H | ? | list.rs | 118 |
| H | ? | list.rs | 152 |
| H | ? | list.rs | 155 |
| H | ? | slice.rs | 28 |
| H | ? | slice.rs | 34 |
| H | ? | fixed_size_list.rs | 79 |
| H | ? | fixed_size_list.rs | 90 |
| H | ? | set.rs | 22 |
| H | ? | set.rs | 26 |
| H | ? | set.rs | 37 |
| H | ? | bitmap_ops.rs | 330 |
| H | ? | bitmap_ops.rs | 331 |
| H | ? | bitmap_ops.rs | 411 |
| H | ? | bitmap_ops.rs | 412 |
| H | ? | mod.rs | 276 |
| H | ? | iterator.rs | 419 |
| H | ? | iterator.rs | 422 |
| H | ? | iterator.rs | 462 |
| H | ? | iterator.rs | 463 |
| H | ? | immutable.rs | 173 |
| H | ? | immutable.rs | 208 |
| H | ? | immutable.rs | 755 |
| H | ? | immutable.rs | 758 |
| H | ? | immutable.rs | 801 |
| H | ? | immutable.rs | 807 |
| H | ? | stream.rs | 123 |
| H | ? | array.rs | 476 |
| H | ? | array.rs | 495 |
| H | ? | array.rs | 545 |
| H | ? | array.rs | 549 |
| H | ? | schema.rs | 72 |
| H | ? | schema.rs | 83 |
| H | ? | schema.rs | 92 |
| H | ? | schema.rs | 103 |
| H | ? | schema.rs | 109 |
| H | ? | schema.rs | 219 |
| H | ? | schema.rs | 542 |
| H | ? | schema.rs | 543 |
| H | ? | schema.rs | 544 |
| H | ? | schema.rs | 545 |
| H | ? | schema.rs | 546 |
| H | ? | schema.rs | 547 |
| H | ? | schema.rs | 739 |
| H | ? | expression.rs | 27 |
| H | ? | expression.rs | 28 |
| H | ? | expression.rs | 29 |
| H | ? | expression.rs | 80 |
| H | ? | expression.rs | 81 |
| H | ? | in_memory_linearize.rs | 58 |
| H | ? | rolling_group_by.rs | 67 |
| H | ? | rolling_group_by.rs | 77 |
| H | ? | rolling_group_by.rs | 78 |
| H | ? | rolling_group_by.rs | 80 |
| H | ? | rolling_group_by.rs | 126 |
| H | ? | rolling_group_by.rs | 294 |
| H | ? | rolling_group_by.rs | 353 |
| H | ? | ewm.rs | 63 |
| H | ? | peak_minmax.rs | 142 |
| H | ? | peak_minmax.rs | 159 |
| H | ? | peak_minmax.rs | 177 |
| H | ? | negative_slice.rs | 133 |
| H | ? | merge_sorted.rs | 347 |
| H | ? | merge_sorted.rs | 409 |
| H | ? | merge_sorted.rs | 433 |
| H | ? | merge_sorted.rs | 493 |
| H | ? | merge_sorted.rs | 499 |
| H | ? | merge_sorted.rs | 515 |
| H | ? | merge_sorted.rs | 520 |
| H | ? | merge_sorted.rs | 527 |
| H | ? | gather_every.rs | 88 |
| H | ? | repeat.rs | 122 |
| H | ? | unordered_union.rs | 72 |
| H | ? | unordered_union.rs | 75 |
| H | ? | rle_id.rs | 71 |
| H | ? | rle_id.rs | 79 |
| H | ? | rle_id.rs | 80 |
| H | ? | mod.rs | 150 |
| H | ? | mod.rs | 219 |
| H | ? | mod.rs | 241 |
| H | ? | mod.rs | 245 |
| H | ? | mod.rs | 253 |
| H | ? | morsel_resize_pipeline.rs | 140 |
| H | ? | partition_morsel_sender.rs | 106 |
| H | ? | partition_morsel_sender.rs | 109 |
| H | ? | partition_morsel_sender.rs | 120 |
| H | ? | partition_morsel_sender.rs | 143 |
| H | ? | hstack_columns.rs | 59 |
| H | ? | hstack_columns.rs | 62 |
| H | ? | file_provider.rs | 33 |
| H | ? | file_provider.rs | 88 |
| H | ? | file_provider.rs | 96 |
| H | ? | partition_distributor.rs | 116 |
| H | ? | partition_distributor.rs | 122 |
| H | ? | partition_distributor.rs | 148 |
| H | ? | partition_distributor.rs | 154 |
| H | ? | partition_distributor.rs | 183 |
| H | ? | partition_distributor.rs | 250 |
| H | ? | partition_distributor.rs | 255 |
| H | ? | partition_distributor.rs | 283 |
| H | ? | partition_key.rs | 33 |
| H | ? | partition_key.rs | 42 |
| H | ? | partition_key.rs | 56 |
| H | ? | partitioner.rs | 146 |
| H | ? | partitioner.rs | 158 |
| H | ? | mod.rs | 34 |
| H | ? | mod.rs | 65 |
| H | ? | mod.rs | 79 |
| H | ? | mod.rs | 81 |
| H | ? | mod.rs | 85 |
| H | ? | mod.rs | 93 |
| H | ? | mod.rs | 98 |
| H | ? | mod.rs | 105 |
| H | ? | row_group_encoder.rs | 78 |
| H | ? | mod.rs | 79 |
| H | ? | mod.rs | 127 |
| H | ? | morsel_serializer.rs | 42 |
| H | ? | mod.rs | 72 |
| H | ? | morsel_serializer.rs | 92 |
| H | ? | morsel_serializer.rs | 95 |
| H | ? | mod.rs | 94 |
| H | ? | io_writer.rs | 73 |
| H | ? | record_batch_encoder.rs | 105 |
| H | ? | record_batch_encoder.rs | 163 |
| H | ? | record_batch_encoder.rs | 171 |
| H | ? | single_file.rs | 63 |
| H | ? | single_file.rs | 76 |
| H | ? | partition_by.rs | 72 |
| H | ? | partition_by.rs | 74 |
| H | ? | partition_by.rs | 95 |
| H | ? | partition_by.rs | 156 |
| H | ? | partition_by.rs | 178 |
| H | ? | partition_by.rs | 179 |
| H | ? | partition_by.rs | 181 |
| H | ? | partition_by.rs | 187 |
| H | ? | top_k.rs | 115 |
| H | ? | top_k.rs | 181 |
| H | ? | top_k.rs | 193 |
| H | ? | top_k.rs | 250 |
| H | ? | top_k.rs | 256 |
| H | ? | top_k.rs | 297 |
| H | ? | top_k.rs | 342 |
| H | ? | top_k.rs | 348 |
| H | ? | top_k.rs | 357 |
| H | ? | top_k.rs | 388 |
| H | ? | top_k.rs | 414 |
| H | ? | top_k.rs | 444 |
| H | ? | top_k.rs | 445 |
| H | ? | top_k.rs | 446 |
| H | ? | sorted_group_by.rs | 41 |
| H | ? | sorted_group_by.rs | 99 |
| H | ? | sorted_group_by.rs | 193 |
| H | ? | sorted_group_by.rs | 194 |
| H | ? | sorted_group_by.rs | 243 |
| H | ? | is_first_distinct.rs | 25 |
| H | ? | is_first_distinct.rs | 73 |
| H | ? | is_first_distinct.rs | 93 |
| H | ? | callback_sink.rs | 58 |
| H | ? | callback_sink.rs | 116 |
| H | ? | simple_projection.rs | 67 |
| H | ? | simple_projection.rs | 70 |
| H | ? | interpolate.rs | 99 |
| H | ? | interpolate.rs | 100 |
| H | ? | interpolate.rs | 101 |
| H | ? | interpolate.rs | 117 |
| H | ? | interpolate.rs | 119 |
| H | ? | interpolate.rs | 162 |
| H | ? | interpolate.rs | 181 |
| H | ? | interpolate.rs | 182 |
| H | ? | interpolate.rs | 195 |
| H | ? | interpolate.rs | 196 |
| H | ? | interpolate.rs | 200 |
| H | ? | interpolate.rs | 223 |
| H | ? | reduce.rs | 149 |
| H | ? | backward_fill.rs | 86 |
| H | ? | backward_fill.rs | 89 |
| H | ? | backward_fill.rs | 105 |
| H | ? | backward_fill.rs | 107 |
| H | ? | backward_fill.rs | 131 |
| H | ? | backward_fill.rs | 154 |
| H | ? | backward_fill.rs | 156 |
| H | ? | backward_fill.rs | 182 |
| H | ? | backward_fill.rs | 187 |
| H | ? | backward_fill.rs | 193 |
| H | ? | is_sorted.rs | 188 |
| H | ? | ordered_union.rs | 84 |
| H | ? | forward_fill.rs | 78 |
| H | ? | forward_fill.rs | 115 |
| H | ? | forward_fill.rs | 125 |
| H | ? | forward_fill.rs | 134 |
| H | ? | forward_fill.rs | 139 |
| H | ? | forward_fill.rs | 171 |
| H | ? | forward_fill.rs | 172 |
| H | ? | shift.rs | 49 |
| H | ? | shift.rs | 78 |
| H | ? | shift.rs | 138 |
| H | ? | shift.rs | 156 |
| H | ? | dynamic_group_by.rs | 74 |
| H | ? | dynamic_group_by.rs | 84 |
| H | ? | dynamic_group_by.rs | 86 |
| H | ? | dynamic_group_by.rs | 200 |
| H | ? | dynamic_group_by.rs | 386 |
| H | ? | dynamic_group_by.rs | 389 |
| H | ? | dynamic_group_by.rs | 390 |
| H | ? | dynamic_group_by.rs | 451 |
| H | ? | group_by.rs | 70 |
| H | ? | group_by.rs | 154 |
| H | ? | group_by.rs | 173 |
| H | ? | group_by.rs | 318 |
| H | ? | group_by.rs | 319 |
| H | ? | group_by.rs | 510 |
| H | ? | group_by.rs | 569 |
| H | ? | chunk_data_fetch.rs | 34 |
| H | ? | chunk_data_fetch.rs | 40 |
| H | ? | chunk_data_fetch.rs | 56 |
| H | ? | chunk_data_fetch.rs | 59 |
| H | ? | chunk_data_fetch.rs | 63 |
| H | ? | pipeline_budget.rs | 59 |
| H | ? | pipeline_budget.rs | 63 |
| H | ? | batch.rs | 47 |
| H | ? | batch.rs | 65 |
| H | ? | batch.rs | 133 |
| H | ? | batch.rs | 196 |
| H | ? | batch.rs | 202 |
| H | ? | batch.rs | 224 |
| H | ? | batch.rs | 226 |
| H | ? | batch.rs | 239 |
| H | ? | batch.rs | 251 |
| H | ? | batch.rs | 277 |
| H | ? | mod.rs | 86 |
| H | ? | mod.rs | 87 |
| H | ? | mod.rs | 88 |
| H | ? | mod.rs | 89 |
| H | ? | mod.rs | 107 |
| H | ? | mod.rs | 111 |
| H | ? | mod.rs | 170 |
| H | ? | mod.rs | 194 |
| H | ? | mod.rs | 220 |
| H | ? | mod.rs | 223 |
| H | ? | mod.rs | 237 |
| H | ? | mod.rs | 241 |
| H | ? | mod.rs | 268 |
| H | ? | mod.rs | 269 |
| H | ? | mod.rs | 272 |
| H | ? | mod.rs | 310 |
| H | ? | mod.rs | 332 |
| H | ? | mod.rs | 349 |
| H | ? | mod.rs | 367 |
| H | ? | mod.rs | 371 |
| H | ? | row_group_decode.rs | 76 |
| H | ? | row_group_decode.rs | 84 |
| H | ? | row_group_decode.rs | 124 |
| H | ? | row_group_decode.rs | 162 |
| H | ? | row_group_decode.rs | 163 |
| H | ? | row_group_decode.rs | 181 |
| H | ? | row_group_decode.rs | 182 |
| H | ? | row_group_decode.rs | 185 |
| H | ? | row_group_decode.rs | 186 |
| H | ? | row_group_decode.rs | 193 |
| H | ? | row_group_decode.rs | 194 |
| H | ? | row_group_decode.rs | 195 |
| H | ? | row_group_decode.rs | 197 |
| H | ? | row_group_decode.rs | 212 |
| H | ? | row_group_decode.rs | 246 |
| H | ? | row_group_decode.rs | 271 |
| H | ? | row_group_decode.rs | 309 |
| H | ? | row_group_decode.rs | 318 |
| H | ? | row_group_decode.rs | 319 |
| H | ? | row_group_decode.rs | 373 |
| H | ? | row_group_decode.rs | 375 |
| H | ? | row_group_decode.rs | 376 |
| H | ? | row_group_decode.rs | 387 |
| H | ? | row_group_decode.rs | 440 |
| H | ? | row_group_decode.rs | 441 |
| H | ? | row_group_decode.rs | 442 |
| H | ? | row_group_decode.rs | 449 |
| H | ? | row_group_decode.rs | 450 |
| H | ? | row_group_decode.rs | 451 |
| H | ? | row_group_decode.rs | 452 |
| H | ? | row_group_decode.rs | 500 |
| H | ? | row_group_decode.rs | 552 |
| H | ? | row_group_decode.rs | 564 |
| H | ? | row_group_decode.rs | 579 |
| H | ? | row_group_decode.rs | 581 |
| H | ? | row_group_decode.rs | 582 |
| H | ? | row_group_decode.rs | 589 |
| H | ? | row_group_decode.rs | 590 |
| H | ? | row_group_decode.rs | 591 |
| H | ? | row_group_decode.rs | 592 |
| H | ? | row_group_decode.rs | 593 |
| H | ? | row_group_decode.rs | 648 |
| H | ? | row_group_decode.rs | 670 |
| H | ? | row_group_decode.rs | 674 |
| H | ? | metadata_utils.rs | 36 |
| H | ? | metadata_utils.rs | 94 |
| H | ? | projection.rs | 37 |
| H | ? | projection.rs | 52 |
| H | ? | projection.rs | 53 |
| H | ? | init.rs | 38 |
| H | ? | init.rs | 42 |
| H | ? | init.rs | 62 |
| H | ? | init.rs | 64 |
| H | ? | init.rs | 87 |
| H | ? | init.rs | 89 |
| H | ? | init.rs | 151 |
| H | ? | init.rs | 155 |
| H | ? | init.rs | 162 |
| H | ? | init.rs | 206 |
| H | ? | init.rs | 245 |
| H | ? | init.rs | 291 |
| H | ? | init.rs | 320 |
| H | ? | init.rs | 321 |
| H | ? | init.rs | 323 |
| H | ? | statistics.rs | 101 |
| H | ? | statistics.rs | 104 |
| H | ? | statistics.rs | 105 |
| H | ? | statistics.rs | 110 |
| H | ? | statistics.rs | 220 |
| H | ? | statistics.rs | 221 |
| H | ? | statistics.rs | 228 |
| H | ? | row_group_data_fetch.rs | 121 |
| H | ? | row_group_data_fetch.rs | 122 |
| H | ? | row_group_data_fetch.rs | 123 |
| H | ? | row_group_data_fetch.rs | 155 |
| H | ? | row_group_data_fetch.rs | 199 |
| H | ? | row_group_data_fetch.rs | 224 |
| H | ? | row_group_data_fetch.rs | 230 |
| H | ? | builder.rs | 132 |
| H | ? | builder.rs | 146 |
| H | ? | builder.rs | 153 |
| H | ? | mod.rs | 110 |
| H | ? | mod.rs | 115 |
| H | ? | mod.rs | 201 |
| H | ? | mod.rs | 224 |
| H | ? | forbid_extra_columns.rs | 27 |
| H | ? | forbid_extra_columns.rs | 28 |
| H | ? | apply_extra_ops.rs | 116 |
| H | ? | apply_extra_ops.rs | 131 |
| H | ? | apply_extra_ops.rs | 146 |
| H | ? | apply_extra_ops.rs | 148 |
| H | ? | apply_extra_ops.rs | 179 |
| H | ? | apply_extra_ops.rs | 183 |
| H | ? | apply_extra_ops.rs | 264 |
| H | ? | apply_extra_ops.rs | 327 |
| H | ? | row_deletions.rs | 138 |
| H | ? | row_deletions.rs | 160 |
| H | ? | row_deletions.rs | 177 |
| H | ? | row_deletions.rs | 220 |
| H | ? | row_deletions.rs | 294 |
| H | ? | row_deletions.rs | 295 |
| H | ? | row_deletions.rs | 296 |
| H | ? | row_deletions.rs | 302 |
| H | ? | row_deletions.rs | 303 |
| H | ? | row_deletions.rs | 328 |
| H | ? | row_deletions.rs | 487 |
| H | ? | row_deletions.rs | 515 |
| H | ? | row_deletions.rs | 518 |
| H | ? | row_deletions.rs | 558 |
| H | ? | reader_operation_pushdown.rs | 52 |
| H | ? | reader_operation_pushdown.rs | 99 |
| H | ? | mod.rs | 48 |
| H | ? | mod.rs | 52 |
| H | ? | transform.rs | 48 |
| H | ? | transform.rs | 64 |
| H | ? | transform.rs | 76 |
| H | ? | transform.rs | 91 |
| H | ? | transform.rs | 105 |
| H | ? | transform.rs | 118 |
| H | ? | transform.rs | 121 |
| H | ? | transform.rs | 130 |
| H | ? | transform.rs | 146 |
| H | ? | transform.rs | 161 |
| H | ? | transform.rs | 175 |
| H | ? | transform.rs | 189 |
| H | ? | transform.rs | 203 |
| H | ? | builder.rs | 39 |
| H | ? | builder.rs | 40 |
| H | ? | builder.rs | 75 |
| H | ? | builder.rs | 155 |
| H | ? | builder.rs | 156 |
| H | ? | builder.rs | 245 |
| H | ? | builder.rs | 257 |
| H | ? | builder.rs | 478 |
| H | ? | builder.rs | 602 |
| H | ? | builder.rs | 625 |
| H | ? | builder.rs | 654 |
| H | ? | builder.rs | 656 |
| H | ? | builder.rs | 664 |
| H | ? | mod.rs | 65 |
| H | ? | mod.rs | 103 |
| H | ? | mod.rs | 327 |
| H | ? | builder.rs | 62 |
| H | ? | builder.rs | 79 |
| H | ? | builder.rs | 118 |
| H | ? | builder.rs | 152 |
| H | ? | builder.rs | 153 |
| H | ? | builder.rs | 162 |
| H | ? | builder.rs | 235 |
| H | ? | builder.rs | 247 |
| H | ? | resolve_slice.rs | 22 |
| H | ? | resolve_slice.rs | 25 |
| H | ? | resolve_slice.rs | 33 |
| H | ? | resolve_slice.rs | 54 |
| H | ? | resolve_slice.rs | 73 |
| H | ? | resolve_slice.rs | 81 |
| H | ? | resolve_slice.rs | 82 |
| H | ? | resolve_slice.rs | 100 |
| H | ? | resolve_slice.rs | 101 |
| H | ? | resolve_slice.rs | 102 |
| H | ? | resolve_slice.rs | 103 |
| H | ? | resolve_slice.rs | 112 |
| H | ? | resolve_slice.rs | 156 |
| H | ? | resolve_slice.rs | 208 |
| H | ? | resolve_slice.rs | 215 |
| H | ? | resolve_projections.rs | 43 |
| H | ? | resolve_projections.rs | 49 |
| H | ? | initialization.rs | 62 |
| H | ? | initialization.rs | 162 |
| H | ? | initialization.rs | 163 |
| H | ? | initialization.rs | 167 |
| H | ? | initialization.rs | 172 |
| H | ? | initialization.rs | 207 |
| H | ? | initialization.rs | 208 |
| H | ? | initialization.rs | 219 |
| H | ? | initialization.rs | 220 |
| H | ? | initialization.rs | 232 |
| H | ? | initialization.rs | 239 |
| H | ? | initialization.rs | 241 |
| H | ? | initialization.rs | 276 |
| H | ? | initialization.rs | 281 |
| H | ? | initialization.rs | 296 |
| H | ? | initialization.rs | 328 |
| H | ? | initialization.rs | 329 |
| H | ? | initialization.rs | 330 |
| H | ? | initialization.rs | 336 |
| H | ? | initialization.rs | 337 |
| H | ? | initialization.rs | 344 |
| H | ? | initialization.rs | 345 |
| H | ? | initialization.rs | 346 |
| H | ? | initialization.rs | 347 |
| H | ? | initialization.rs | 348 |
| H | ? | initialization.rs | 366 |
| H | ? | initialization.rs | 367 |
| H | ? | initialization.rs | 383 |
| H | ? | initialization.rs | 405 |
| H | ? | initialization.rs | 407 |
| H | ? | initialization.rs | 408 |
| H | ? | initialization.rs | 409 |
| H | ? | initialization.rs | 445 |
| H | ? | bridge.rs | 101 |
| H | ? | post_apply_extra_ops.rs | 42 |
| H | ? | post_apply_extra_ops.rs | 91 |
| H | ? | post_apply_extra_ops.rs | 121 |
| H | ? | post_apply_extra_ops.rs | 122 |
| H | ? | post_apply_extra_ops.rs | 123 |
| H | ? | reader_starter.rs | 88 |
| H | ? | reader_starter.rs | 184 |
| H | ? | reader_starter.rs | 194 |
| H | ? | reader_starter.rs | 196 |
| H | ? | reader_starter.rs | 236 |
| H | ? | reader_starter.rs | 337 |
| H | ? | reader_starter.rs | 342 |
| H | ? | reader_starter.rs | 450 |
| H | ? | reader_starter.rs | 464 |
| H | ? | reader_starter.rs | 466 |
| H | ? | reader_starter.rs | 543 |
| H | ? | reader_starter.rs | 564 |
| H | ? | reader_starter.rs | 566 |
| H | ? | reader_starter.rs | 574 |
| H | ? | reader_starter.rs | 596 |
| H | ? | reader_starter.rs | 599 |
| H | ? | reader_starter.rs | 617 |
| H | ? | reader_starter.rs | 644 |
| H | ? | reader_starter.rs | 661 |
| H | ? | mod.rs | 86 |
| H | ? | mod.rs | 87 |
| H | ? | mod.rs | 88 |
| H | ? | mod.rs | 89 |
| H | ? | mod.rs | 108 |
| H | ? | mod.rs | 116 |
| H | ? | mod.rs | 162 |
| H | ? | mod.rs | 240 |
| H | ? | mod.rs | 280 |
| H | ? | mod.rs | 301 |
| H | ? | mod.rs | 331 |
| H | ? | mod.rs | 339 |
| H | ? | mod.rs | 367 |
| H | ? | mod.rs | 373 |
| H | ? | mod.rs | 405 |
| H | ? | mod.rs | 441 |
| H | ? | chunk_reader.rs | 33 |
| H | ? | chunk_reader.rs | 36 |
| H | ? | chunk_reader.rs | 42 |
| H | ? | line_batch_source.rs | 191 |
| H | ? | line_batch_source.rs | 209 |
| H | ? | builder.rs | 95 |
| H | ? | mod.rs | 85 |
| H | ? | mod.rs | 86 |
| H | ? | mod.rs | 87 |
| H | ? | mod.rs | 88 |
| H | ? | mod.rs | 107 |
| H | ? | mod.rs | 115 |
| H | ? | mod.rs | 163 |
| H | ? | mod.rs | 207 |
| H | ? | mod.rs | 213 |
| H | ? | mod.rs | 374 |
| H | ? | mod.rs | 444 |
| H | ? | line_batch_processor.rs | 133 |
| H | ? | row_index_limit_pass.rs | 65 |
| H | ? | negative_slice_pass.rs | 175 |
| H | ? | negative_slice_pass.rs | 176 |
| H | ? | negative_slice_pass.rs | 177 |
| H | ? | negative_slice_pass.rs | 192 |
| H | ? | negative_slice_pass.rs | 205 |
| H | ? | chunk_reader.rs | 50 |
| H | ? | chunk_reader.rs | 90 |
| H | ? | line_batch_distributor.rs | 201 |
| H | ? | line_batch_distributor.rs | 224 |
| H | ? | mod.rs | 99 |
| H | ? | mod.rs | 100 |
| H | ? | mod.rs | 101 |
| H | ? | mod.rs | 102 |
| H | ? | mod.rs | 120 |
| H | ? | mod.rs | 124 |
| H | ? | mod.rs | 142 |
| H | ? | mod.rs | 143 |
| H | ? | mod.rs | 202 |
| H | ? | mod.rs | 232 |
| H | ? | mod.rs | 237 |
| H | ? | mod.rs | 297 |
| H | ? | mod.rs | 324 |
| H | ? | mod.rs | 327 |
| H | ? | mod.rs | 339 |
| H | ? | mod.rs | 347 |
| H | ? | mod.rs | 430 |
| H | ? | mod.rs | 480 |
| H | ? | mod.rs | 490 |
| H | ? | mod.rs | 534 |
| H | ? | mod.rs | 579 |
| H | ? | metadata.rs | 34 |
| H | ? | metadata.rs | 87 |
| H | ? | record_batch_data_fetch.rs | 69 |
| H | ? | record_batch_data_fetch.rs | 85 |
| H | ? | record_batch_data_fetch.rs | 138 |
| H | ? | record_batch_data_fetch.rs | 151 |
| H | ? | record_batch_data_fetch.rs | 154 |
| H | ? | record_batch_decode.rs | 38 |
| H | ? | record_batch_decode.rs | 39 |
| H | ? | record_batch_decode.rs | 40 |
| H | ? | record_batch_decode.rs | 68 |
| H | ? | record_batch_decode.rs | 88 |
| H | ? | record_batch_decode.rs | 113 |
| H | ? | record_batch_decode.rs | 156 |
| H | ? | builder.rs | 113 |
| H | ? | builder.rs | 117 |
| H | ? | builder.rs | 133 |
| H | ? | zip.rs | 104 |
| H | ? | zip.rs | 329 |
| H | ? | zip.rs | 376 |
| H | ? | strptime_infer.rs | 81 |
| H | ? | strptime_infer.rs | 96 |
| H | ? | strptime_infer.rs | 203 |
| H | ? | strptime_infer.rs | 224 |
| H | ? | strptime_infer.rs | 225 |
| H | ? | rle.rs | 92 |
| H | ? | rle.rs | 95 |
| H | ? | rle.rs | 111 |
| H | ? | rle.rs | 149 |
| H | ? | rle.rs | 152 |
| H | ? | rle.rs | 163 |
| H | ? | rle.rs | 219 |
| H | ? | mod.rs | 79 |
| H | ? | mod.rs | 87 |
| H | ? | equi_join.rs | 95 |
| H | ? | equi_join.rs | 100 |
| H | ? | equi_join.rs | 106 |
| H | ? | equi_join.rs | 118 |
| H | ? | equi_join.rs | 157 |
| H | ? | equi_join.rs | 164 |
| H | ? | equi_join.rs | 178 |
| H | ? | equi_join.rs | 195 |
| H | ? | equi_join.rs | 207 |
| H | ? | equi_join.rs | 424 |
| H | ? | equi_join.rs | 510 |
| H | ? | equi_join.rs | 568 |
| H | ? | equi_join.rs | 658 |
| H | ? | equi_join.rs | 659 |
| H | ? | equi_join.rs | 680 |
| H | ? | equi_join.rs | 815 |
| H | ? | equi_join.rs | 816 |
| H | ? | equi_join.rs | 863 |
| H | ? | equi_join.rs | 1065 |
| H | ? | equi_join.rs | 1173 |
| H | ? | equi_join.rs | 1507 |
| H | ? | equi_join.rs | 1508 |
| H | ? | equi_join.rs | 1539 |
| H | ? | equi_join.rs | 1572 |
| H | ? | cross_join.rs | 53 |
| H | ? | cross_join.rs | 168 |
| H | ? | cross_join.rs | 169 |
| H | ? | cross_join.rs | 195 |
| H | ? | cross_join.rs | 203 |
| H | ? | range_join.rs | 155 |
| H | ? | range_join.rs | 330 |
| H | ? | range_join.rs | 331 |
| H | ? | range_join.rs | 405 |
| H | ? | range_join.rs | 419 |
| H | ? | range_join.rs | 442 |
| H | ? | range_join.rs | 444 |
| H | ? | merge_join.rs | 140 |
| H | ? | merge_join.rs | 146 |
| H | ? | merge_join.rs | 164 |
| H | ? | merge_join.rs | 165 |
| H | ? | merge_join.rs | 307 |
| H | ? | merge_join.rs | 319 |
| H | ? | merge_join.rs | 394 |
| H | ? | merge_join.rs | 501 |
| H | ? | merge_join.rs | 502 |
| H | ? | merge_join.rs | 513 |
| H | ? | merge_join.rs | 537 |
| H | ? | merge_join.rs | 564 |
| H | ? | merge_join.rs | 581 |
| H | ? | merge_join.rs | 589 |
| H | ? | merge_join.rs | 616 |
| H | ? | merge_join.rs | 619 |
| H | ? | merge_join.rs | 640 |
| H | ? | merge_join.rs | 642 |
| H | ? | semi_anti_join.rs | 34 |
| H | ? | semi_anti_join.rs | 185 |
| H | ? | semi_anti_join.rs | 186 |
| H | ? | semi_anti_join.rs | 308 |
| H | ? | semi_anti_join.rs | 326 |
| H | ? | semi_anti_join.rs | 439 |
| H | ? | semi_anti_join.rs | 459 |
| H | ? | asof_join.rs | 306 |
| H | ? | asof_join.rs | 346 |
| H | ? | asof_join.rs | 377 |
| H | ? | asof_join.rs | 381 |
| H | ? | asof_join.rs | 405 |
| H | ? | asof_join.rs | 413 |
| H | ? | asof_join.rs | 416 |
| H | ? | asof_join.rs | 614 |
| H | ? | asof_join.rs | 619 |
| H | ? | asof_join.rs | 735 |
| H | ? | asof_join.rs | 741 |
| H | ? | asof_join.rs | 756 |
| H | ? | asof_join.rs | 822 |
| H | ? | asof_join.rs | 833 |
| H | ? | asof_join.rs | 836 |
| H | ? | utils.rs | 78 |
| H | ? | utils.rs | 167 |
| H | ? | multiplexer.rs | 134 |
| H | ? | multiplexer.rs | 136 |
| H | ? | multiplexer.rs | 145 |
| H | ? | multiplexer.rs | 159 |
| H | ? | multiplexer.rs | 160 |
| H | ? | multiplexer.rs | 171 |
| H | ? | multiplexer.rs | 201 |
| H | ? | multiplexer.rs | 205 |
| H | ? | sorted_unique.rs | 122 |
| H | ? | sorted_unique.rs | 125 |
| H | ? | columnar_function.rs | 82 |
| H | ? | columnar_function.rs | 83 |
| H | ? | columnar_function.rs | 94 |
| H | ? | with_row_index.rs | 54 |
| H | ? | with_row_index.rs | 74 |
| H | ? | with_row_index.rs | 79 |
| H | ? | in_memory_source.rs | 96 |
| H | ? | in_memory_source.rs | 111 |
| H | ? | skeleton.rs | 97 |
| H | ? | skeleton.rs | 98 |
| H | ? | skeleton.rs | 125 |
| H | ? | skeleton.rs | 159 |
| H | ? | mod.rs | 789 |
| H | ? | mod.rs | 816 |
| H | ? | mod.rs | 824 |
| H | ? | mod.rs | 832 |
| H | ? | python_dataset.rs | 56 |
| H | ? | lower_expr.rs | 405 |
| H | ? | lower_expr.rs | 416 |
| H | ? | lower_expr.rs | 531 |
| H | ? | lower_expr.rs | 540 |
| H | ? | lower_expr.rs | 571 |
| H | ? | lower_expr.rs | 595 |
| H | ? | lower_expr.rs | 614 |
| H | ? | lower_expr.rs | 619 |
| H | ? | lower_expr.rs | 629 |
| H | ? | lower_expr.rs | 642 |
| H | ? | lower_expr.rs | 643 |
| H | ? | lower_expr.rs | 647 |
| H | ? | lower_expr.rs | 665 |
| H | ? | lower_expr.rs | 667 |
| H | ? | lower_expr.rs | 668 |
| H | ? | lower_expr.rs | 674 |
| H | ? | lower_expr.rs | 679 |
| H | ? | lower_expr.rs | 687 |
| H | ? | lower_expr.rs | 694 |
| H | ? | lower_expr.rs | 718 |
| H | ? | lower_expr.rs | 726 |
| H | ? | lower_expr.rs | 748 |
| H | ? | lower_expr.rs | 756 |
| H | ? | lower_expr.rs | 757 |
| H | ? | lower_expr.rs | 762 |
| H | ? | lower_expr.rs | 763 |
| H | ? | lower_expr.rs | 768 |
| H | ? | lower_expr.rs | 784 |
| H | ? | lower_expr.rs | 831 |
| H | ? | lower_expr.rs | 833 |
| H | ? | lower_expr.rs | 834 |
| H | ? | lower_expr.rs | 840 |
| H | ? | lower_expr.rs | 897 |
| H | ? | lower_expr.rs | 898 |
| H | ? | lower_expr.rs | 901 |
| H | ? | lower_expr.rs | 904 |
| H | ? | lower_expr.rs | 931 |
| H | ? | lower_expr.rs | 966 |
| H | ? | lower_expr.rs | 970 |
| H | ? | lower_expr.rs | 971 |
| H | ? | lower_expr.rs | 973 |
| H | ? | lower_expr.rs | 974 |
| H | ? | lower_expr.rs | 977 |
| H | ? | lower_expr.rs | 997 |
| H | ? | lower_expr.rs | 999 |
| H | ? | lower_expr.rs | 1000 |
| H | ? | lower_expr.rs | 1006 |
| H | ? | lower_expr.rs | 1011 |
| H | ? | lower_expr.rs | 1035 |
| H | ? | lower_expr.rs | 1039 |
| H | ? | lower_expr.rs | 1040 |
| H | ? | lower_expr.rs | 1042 |
| H | ? | lower_expr.rs | 1045 |
| H | ? | lower_expr.rs | 1046 |
| H | ? | lower_expr.rs | 1048 |
| H | ? | lower_expr.rs | 1065 |
| H | ? | lower_expr.rs | 1067 |
| H | ? | lower_expr.rs | 1070 |
| H | ? | lower_expr.rs | 1108 |
| H | ? | lower_expr.rs | 1113 |
| H | ? | lower_expr.rs | 1123 |
| H | ? | lower_expr.rs | 1144 |
| H | ? | lower_expr.rs | 1175 |
| H | ? | lower_expr.rs | 1188 |
| H | ? | lower_expr.rs | 1213 |
| H | ? | lower_expr.rs | 1223 |
| H | ? | lower_expr.rs | 1243 |
| H | ? | lower_expr.rs | 1245 |
| H | ? | lower_expr.rs | 1249 |
| H | ? | lower_expr.rs | 1254 |
| H | ? | lower_expr.rs | 1346 |
| H | ? | lower_expr.rs | 1352 |
| H | ? | lower_expr.rs | 1356 |
| H | ? | lower_expr.rs | 1379 |
| H | ? | lower_expr.rs | 1384 |
| H | ? | lower_expr.rs | 1389 |
| H | ? | lower_expr.rs | 1403 |
| H | ? | lower_expr.rs | 1408 |
| H | ? | lower_expr.rs | 1411 |
| H | ? | lower_expr.rs | 1425 |
| H | ? | lower_expr.rs | 1431 |
| H | ? | lower_expr.rs | 1436 |
| H | ? | lower_expr.rs | 1454 |
| H | ? | lower_expr.rs | 1461 |
| H | ? | lower_expr.rs | 1464 |
| H | ? | lower_expr.rs | 1469 |
| H | ? | lower_expr.rs | 1489 |
| H | ? | lower_expr.rs | 1491 |
| H | ? | lower_expr.rs | 1529 |
| H | ? | lower_expr.rs | 1536 |
| H | ? | lower_expr.rs | 1570 |
| H | ? | lower_expr.rs | 1575 |
| H | ? | lower_expr.rs | 1576 |
| H | ? | lower_expr.rs | 1582 |
| H | ? | lower_expr.rs | 1583 |
| H | ? | lower_expr.rs | 1610 |
| H | ? | lower_expr.rs | 1613 |
| H | ? | lower_expr.rs | 1640 |
| H | ? | lower_expr.rs | 1643 |
| H | ? | lower_expr.rs | 1648 |
| H | ? | lower_expr.rs | 1688 |
| H | ? | lower_expr.rs | 1710 |
| H | ? | lower_expr.rs | 1724 |
| H | ? | lower_expr.rs | 1736 |
| H | ? | lower_expr.rs | 1739 |
| H | ? | lower_expr.rs | 1748 |
| H | ? | lower_expr.rs | 1771 |
| H | ? | lower_expr.rs | 1772 |
| H | ? | lower_expr.rs | 1774 |
| H | ? | lower_expr.rs | 1813 |
| H | ? | lower_expr.rs | 1816 |
| H | ? | lower_expr.rs | 1832 |
| H | ? | lower_expr.rs | 1842 |
| H | ? | lower_expr.rs | 1844 |
| H | ? | lower_expr.rs | 1888 |
| H | ? | lower_expr.rs | 1891 |
| H | ? | lower_expr.rs | 1898 |
| H | ? | lower_expr.rs | 1915 |
| H | ? | lower_expr.rs | 1926 |
| H | ? | lower_expr.rs | 1934 |
| H | ? | lower_expr.rs | 1937 |
| H | ? | lower_expr.rs | 1955 |
| H | ? | lower_expr.rs | 1961 |
| H | ? | lower_expr.rs | 1965 |
| H | ? | lower_expr.rs | 1974 |
| H | ? | lower_expr.rs | 1979 |
| H | ? | lower_expr.rs | 1992 |
| H | ? | lower_expr.rs | 2002 |
| H | ? | lower_expr.rs | 2003 |
| H | ? | lower_expr.rs | 2008 |
| H | ? | lower_expr.rs | 2013 |
| H | ? | lower_expr.rs | 2026 |
| H | ? | lower_expr.rs | 2035 |
| H | ? | lower_expr.rs | 2052 |
| H | ? | lower_expr.rs | 2057 |
| H | ? | lower_expr.rs | 2060 |
| H | ? | lower_expr.rs | 2061 |
| H | ? | lower_expr.rs | 2104 |
| H | ? | lower_expr.rs | 2126 |
| H | ? | lower_expr.rs | 2143 |
| H | ? | lower_expr.rs | 2248 |
| H | ? | lower_expr.rs | 2252 |
| H | ? | lower_expr.rs | 2256 |
| H | ? | lower_expr.rs | 2291 |
| H | ? | lower_expr.rs | 2318 |
| H | ? | lower_expr.rs | 2322 |
| H | ? | lower_expr.rs | 2326 |
| H | ? | lower_expr.rs | 2334 |
| H | ? | lower_expr.rs | 2358 |
| H | ? | lower_expr.rs | 2359 |
| H | ? | lower_expr.rs | 2364 |
| H | ? | lower_expr.rs | 2366 |
| H | ? | lower_expr.rs | 2401 |
| H | ? | lower_expr.rs | 2405 |
| H | ? | lower_expr.rs | 2407 |
| H | ? | lower_expr.rs | 2408 |
| H | ? | lower_expr.rs | 2427 |
| H | ? | lower_expr.rs | 2434 |
| H | ? | lower_expr.rs | 2451 |
| H | ? | lower_expr.rs | 2454 |
| H | ? | lower_expr.rs | 2457 |
| H | ? | lower_expr.rs | 2463 |
| H | ? | lower_expr.rs | 2492 |
| H | ? | lower_expr.rs | 2498 |
| H | ? | lower_expr.rs | 2535 |
| H | ? | lower_expr.rs | 2542 |
| H | ? | lower_expr.rs | 2547 |
| H | ? | lower_expr.rs | 2548 |
| H | ? | lower_expr.rs | 2559 |
| H | ? | lower_expr.rs | 2568 |
| H | ? | lower_expr.rs | 2569 |
| H | ? | lower_expr.rs | 2583 |
| H | ? | lower_expr.rs | 2605 |
| H | ? | lower_expr.rs | 2632 |
| H | ? | lower_expr.rs | 2641 |
| H | ? | lower_expr.rs | 2645 |
| H | ? | lower_expr.rs | 2655 |
| H | ? | lower_expr.rs | 2665 |
| H | ? | lower_expr.rs | 2711 |
| H | ? | lower_expr.rs | 2714 |
| H | ? | lower_expr.rs | 2752 |
| H | ? | lower_expr.rs | 2758 |
| H | ? | lower_expr.rs | 2781 |
| H | ? | lower_expr.rs | 2821 |
| H | ? | lower_expr.rs | 2862 |
| H | ? | lower_expr.rs | 2865 |
| H | ? | lower_expr.rs | 2867 |
| H | ? | lower_expr.rs | 2887 |
| H | ? | lower_expr.rs | 2888 |
| H | ? | lower_expr.rs | 2890 |
| H | ? | lower_expr.rs | 2895 |
| H | ? | lower_expr.rs | 2940 |
| H | ? | lower_group_by.rs | 50 |
| H | ? | lower_group_by.rs | 53 |
| H | ? | lower_group_by.rs | 58 |
| H | ? | lower_group_by.rs | 106 |
| H | ? | lower_group_by.rs | 137 |
| H | ? | lower_group_by.rs | 146 |
| H | ? | lower_group_by.rs | 151 |
| H | ? | lower_group_by.rs | 173 |
| H | ? | lower_group_by.rs | 180 |
| H | ? | lower_group_by.rs | 278 |
| H | ? | lower_group_by.rs | 336 |
| H | ? | lower_group_by.rs | 345 |
| H | ? | lower_group_by.rs | 424 |
| H | ? | lower_group_by.rs | 425 |
| H | ? | lower_group_by.rs | 433 |
| H | ? | lower_group_by.rs | 490 |
| H | ? | lower_group_by.rs | 548 |
| H | ? | lower_group_by.rs | 553 |
| H | ? | lower_group_by.rs | 598 |
| H | ? | lower_group_by.rs | 638 |
| H | ? | lower_group_by.rs | 642 |
| H | ? | lower_group_by.rs | 680 |
| H | ? | lower_group_by.rs | 683 |
| H | ? | lower_group_by.rs | 691 |
| H | ? | lower_group_by.rs | 758 |
| H | ? | lower_group_by.rs | 761 |
| H | ? | lower_group_by.rs | 793 |
| H | ? | lower_group_by.rs | 796 |
| H | ? | lower_group_by.rs | 798 |
| H | ? | lower_group_by.rs | 824 |
| H | ? | lower_group_by.rs | 829 |
| H | ? | lower_group_by.rs | 836 |
| H | ? | lower_group_by.rs | 847 |
| H | ? | lower_group_by.rs | 850 |
| H | ? | lower_group_by.rs | 873 |
| H | ? | lower_group_by.rs | 885 |
| H | ? | lower_group_by.rs | 900 |
| H | ? | lower_group_by.rs | 913 |
| H | ? | lower_group_by.rs | 930 |
| H | ? | lower_group_by.rs | 932 |
| H | ? | lower_group_by.rs | 939 |
| H | ? | lower_group_by.rs | 941 |
| H | ? | lower_group_by.rs | 947 |
| H | ? | lower_group_by.rs | 961 |
| H | ? | lower_group_by.rs | 986 |
| H | ? | lower_group_by.rs | 987 |
| H | ? | lower_group_by.rs | 999 |
| H | ? | lower_group_by.rs | 1067 |
| H | ? | lower_group_by.rs | 1076 |
| H | ? | lower_group_by.rs | 1084 |
| H | ? | lower_group_by.rs | 1092 |
| H | ? | lower_group_by.rs | 1095 |
| H | ? | lower_group_by.rs | 1097 |
| H | ? | lower_group_by.rs | 1100 |
| H | ? | lower_group_by.rs | 1103 |
| H | ? | lower_group_by.rs | 1106 |
| H | ? | lower_group_by.rs | 1118 |
| H | ? | lower_group_by.rs | 1119 |
| H | ? | lower_group_by.rs | 1132 |
| H | ? | lower_group_by.rs | 1135 |
| H | ? | lower_group_by.rs | 1151 |
| H | ? | lower_group_by.rs | 1164 |
| H | ? | lower_group_by.rs | 1169 |
| H | ? | lower_group_by.rs | 1172 |
| H | ? | lower_group_by.rs | 1180 |
| H | ? | lower_group_by.rs | 1185 |
| H | ? | lower_group_by.rs | 1190 |
| H | ? | lower_group_by.rs | 1225 |
| H | ? | lower_group_by.rs | 1228 |
| H | ? | lower_group_by.rs | 1250 |
| H | ? | lower_group_by.rs | 1253 |
| H | ? | lower_group_by.rs | 1273 |
| H | ? | lower_group_by.rs | 1275 |
| H | ? | lower_group_by.rs | 1276 |
| H | ? | lower_group_by.rs | 1290 |
| H | ? | lower_group_by.rs | 1291 |
| H | ? | fmt.rs | 719 |
| H | ? | fmt.rs | 723 |
| H | ? | fmt.rs | 794 |
| H | ? | fmt.rs | 798 |
| H | ? | lower_ir.rs | 58 |
| H | ? | lower_ir.rs | 67 |
| H | ? | lower_ir.rs | 93 |
| H | ? | lower_ir.rs | 108 |
| H | ? | lower_ir.rs | 111 |
| H | ? | lower_ir.rs | 134 |
| H | ? | lower_ir.rs | 136 |
| H | ? | lower_ir.rs | 199 |
| H | ? | lower_ir.rs | 209 |
| H | ? | lower_ir.rs | 240 |
| H | ? | lower_ir.rs | 253 |
| H | ? | lower_ir.rs | 255 |
| H | ? | lower_ir.rs | 270 |
| H | ? | lower_ir.rs | 294 |
| H | ? | lower_ir.rs | 311 |
| H | ? | lower_ir.rs | 317 |
| H | ? | lower_ir.rs | 326 |
| H | ? | lower_ir.rs | 348 |
| H | ? | lower_ir.rs | 378 |
| H | ? | lower_ir.rs | 382 |
| H | ? | lower_ir.rs | 390 |
| H | ? | lower_ir.rs | 392 |
| H | ? | lower_ir.rs | 406 |
| H | ? | lower_ir.rs | 490 |
| H | ? | lower_ir.rs | 491 |
| H | ? | lower_ir.rs | 492 |
| H | ? | lower_ir.rs | 512 |
| H | ? | lower_ir.rs | 515 |
| H | ? | lower_ir.rs | 530 |
| H | ? | lower_ir.rs | 531 |
| H | ? | lower_ir.rs | 549 |
| H | ? | lower_ir.rs | 565 |
| H | ? | lower_ir.rs | 569 |
| H | ? | lower_ir.rs | 571 |
| H | ? | lower_ir.rs | 572 |
| H | ? | lower_ir.rs | 578 |
| H | ? | lower_ir.rs | 597 |
| H | ? | lower_ir.rs | 631 |
| H | ? | lower_ir.rs | 651 |
| H | ? | lower_ir.rs | 737 |
| H | ? | lower_ir.rs | 762 |
| H | ? | lower_ir.rs | 763 |
| H | ? | lower_ir.rs | 775 |
| H | ? | lower_ir.rs | 776 |
| H | ? | lower_ir.rs | 785 |
| H | ? | lower_ir.rs | 795 |
| H | ? | lower_ir.rs | 835 |
| H | ? | lower_ir.rs | 883 |
| H | ? | lower_ir.rs | 896 |
| H | ? | lower_ir.rs | 956 |
| H | ? | lower_ir.rs | 969 |
| H | ? | lower_ir.rs | 980 |
| H | ? | lower_ir.rs | 1003 |
| H | ? | lower_ir.rs | 1004 |
| H | ? | lower_ir.rs | 1005 |
| H | ? | lower_ir.rs | 1006 |
| H | ? | lower_ir.rs | 1008 |
| H | ? | lower_ir.rs | 1053 |
| H | ? | lower_ir.rs | 1054 |
| H | ? | lower_ir.rs | 1055 |
| H | ? | lower_ir.rs | 1060 |
| H | ? | lower_ir.rs | 1061 |
| H | ? | lower_ir.rs | 1083 |
| H | ? | lower_ir.rs | 1089 |
| H | ? | lower_ir.rs | 1092 |
| H | ? | lower_ir.rs | 1094 |
| H | ? | lower_ir.rs | 1176 |
| H | ? | lower_ir.rs | 1212 |
| H | ? | lower_ir.rs | 1214 |
| H | ? | lower_ir.rs | 1215 |
| H | ? | lower_ir.rs | 1217 |
| H | ? | lower_ir.rs | 1219 |
| H | ? | lower_ir.rs | 1220 |
| H | ? | lower_ir.rs | 1288 |
| H | ? | lower_ir.rs | 1327 |
| H | ? | lower_ir.rs | 1340 |
| H | ? | lower_ir.rs | 1341 |
| H | ? | lower_ir.rs | 1346 |
| H | ? | lower_ir.rs | 1358 |
| H | ? | lower_ir.rs | 1369 |
| H | ? | lower_ir.rs | 1377 |
| H | ? | lower_ir.rs | 1418 |
| H | ? | lower_ir.rs | 1434 |
| H | ? | lower_ir.rs | 1442 |
| H | ? | lower_ir.rs | 1443 |
| H | ? | lower_ir.rs | 1448 |
| H | ? | lower_ir.rs | 1463 |
| H | ? | lower_ir.rs | 1486 |
| H | ? | lower_ir.rs | 1487 |
| H | ? | lower_ir.rs | 1492 |
| H | ? | lower_ir.rs | 1497 |
| H | ? | lower_ir.rs | 1518 |
| H | ? | lower_ir.rs | 1521 |
| H | ? | lower_ir.rs | 1567 |
| H | ? | lower_ir.rs | 1568 |
| H | ? | lower_ir.rs | 1576 |
| H | ? | lower_ir.rs | 1583 |
| H | ? | lower_ir.rs | 1608 |
| H | ? | lower_ir.rs | 1616 |
| H | ? | lower_ir.rs | 1645 |
| H | ? | lower_ir.rs | 1646 |
| H | ? | lower_ir.rs | 1647 |
| H | ? | lower_ir.rs | 1654 |
| H | ? | lower_ir.rs | 1691 |
| H | ? | lower_ir.rs | 1724 |
| H | ? | lower_ir.rs | 1744 |
| H | ? | lower_ir.rs | 1767 |
| H | ? | lower_ir.rs | 1779 |
| H | ? | lower_ir.rs | 1811 |
| H | ? | lower_ir.rs | 1849 |
| H | ? | lower_ir.rs | 1858 |
| H | ? | lower_ir.rs | 1866 |
| H | ? | to_graph.rs | 115 |
| H | ? | to_graph.rs | 119 |
| H | ? | to_graph.rs | 165 |
| H | ? | to_graph.rs | 166 |
| H | ? | to_graph.rs | 182 |
| H | ? | to_graph.rs | 183 |
| H | ? | to_graph.rs | 228 |
| H | ? | to_graph.rs | 242 |
| H | ? | to_graph.rs | 286 |
| H | ? | to_graph.rs | 291 |
| H | ? | to_graph.rs | 294 |
| H | ? | to_graph.rs | 300 |
| H | ? | to_graph.rs | 317 |
| H | ? | to_graph.rs | 337 |
| H | ? | to_graph.rs | 340 |
| H | ? | to_graph.rs | 343 |
| H | ? | to_graph.rs | 345 |
| H | ? | to_graph.rs | 377 |
| H | ? | to_graph.rs | 421 |
| H | ? | to_graph.rs | 425 |
| H | ? | to_graph.rs | 428 |
| H | ? | to_graph.rs | 453 |
| H | ? | to_graph.rs | 472 |
| H | ? | to_graph.rs | 473 |
| H | ? | to_graph.rs | 482 |
| H | ? | to_graph.rs | 484 |
| H | ? | to_graph.rs | 497 |
| H | ? | to_graph.rs | 500 |
| H | ? | to_graph.rs | 512 |
| H | ? | to_graph.rs | 526 |
| H | ? | to_graph.rs | 535 |
| H | ? | to_graph.rs | 536 |
| H | ? | to_graph.rs | 537 |
| H | ? | to_graph.rs | 557 |
| H | ? | to_graph.rs | 558 |
| H | ? | to_graph.rs | 571 |
| H | ? | to_graph.rs | 577 |
| H | ? | to_graph.rs | 584 |
| H | ? | to_graph.rs | 595 |
| H | ? | to_graph.rs | 598 |
| H | ? | to_graph.rs | 601 |
| H | ? | to_graph.rs | 603 |
| H | ? | to_graph.rs | 637 |
| H | ? | to_graph.rs | 649 |
| H | ? | to_graph.rs | 650 |
| H | ? | to_graph.rs | 653 |
| H | ? | to_graph.rs | 662 |
| H | ? | to_graph.rs | 663 |
| H | ? | to_graph.rs | 694 |
| H | ? | to_graph.rs | 705 |
| H | ? | to_graph.rs | 725 |
| H | ? | to_graph.rs | 736 |
| H | ? | to_graph.rs | 752 |
| H | ? | to_graph.rs | 753 |
| H | ? | to_graph.rs | 754 |
| H | ? | to_graph.rs | 776 |
| H | ? | to_graph.rs | 787 |
| H | ? | to_graph.rs | 798 |
| H | ? | to_graph.rs | 809 |
| H | ? | to_graph.rs | 849 |
| H | ? | to_graph.rs | 867 |
| H | ? | to_graph.rs | 870 |
| H | ? | to_graph.rs | 871 |
| H | ? | to_graph.rs | 872 |
| H | ? | to_graph.rs | 874 |
| H | ? | to_graph.rs | 875 |
| H | ? | to_graph.rs | 877 |
| H | ? | to_graph.rs | 878 |
| H | ? | to_graph.rs | 880 |
| H | ? | to_graph.rs | 882 |
| H | ? | to_graph.rs | 883 |
| H | ? | to_graph.rs | 884 |
| H | ? | to_graph.rs | 885 |
| H | ? | to_graph.rs | 964 |
| H | ? | to_graph.rs | 978 |
| H | ? | to_graph.rs | 987 |
| H | ? | to_graph.rs | 1009 |
| H | ? | to_graph.rs | 1016 |
| H | ? | to_graph.rs | 1017 |
| H | ? | to_graph.rs | 1040 |
| H | ? | to_graph.rs | 1047 |
| H | ? | to_graph.rs | 1048 |
| H | ? | to_graph.rs | 1070 |
| H | ? | to_graph.rs | 1087 |
| H | ? | to_graph.rs | 1088 |
| H | ? | to_graph.rs | 1094 |
| H | ? | to_graph.rs | 1096 |
| H | ? | to_graph.rs | 1100 |
| H | ? | to_graph.rs | 1101 |
| H | ? | to_graph.rs | 1102 |
| H | ? | to_graph.rs | 1106 |
| H | ? | to_graph.rs | 1107 |
| H | ? | to_graph.rs | 1151 |
| H | ? | to_graph.rs | 1152 |
| H | ? | to_graph.rs | 1155 |
| H | ? | to_graph.rs | 1156 |
| H | ? | to_graph.rs | 1250 |
| H | ? | to_graph.rs | 1253 |
| H | ? | to_graph.rs | 1254 |
| H | ? | to_graph.rs | 1255 |
| H | ? | to_graph.rs | 1262 |
| H | ? | to_graph.rs | 1263 |
| H | ? | to_graph.rs | 1264 |
| H | ? | to_graph.rs | 1265 |
| H | ? | to_graph.rs | 1283 |
| H | ? | to_graph.rs | 1286 |
| H | ? | to_graph.rs | 1287 |
| H | ? | to_graph.rs | 1313 |
| H | ? | to_graph.rs | 1316 |
| H | ? | to_graph.rs | 1317 |
| H | ? | to_graph.rs | 1325 |
| H | ? | to_graph.rs | 1326 |
| H | ? | to_graph.rs | 1327 |
| H | ? | to_graph.rs | 1328 |
| H | ? | to_graph.rs | 1329 |
| H | ? | to_graph.rs | 1330 |
| H | ? | to_graph.rs | 1357 |
| H | ? | to_graph.rs | 1358 |
| H | ? | to_graph.rs | 1361 |
| H | ? | to_graph.rs | 1362 |
| H | ? | to_graph.rs | 1367 |
| H | ? | to_graph.rs | 1368 |
| H | ? | to_graph.rs | 1369 |
| H | ? | to_graph.rs | 1370 |
| H | ? | to_graph.rs | 1405 |
| H | ? | to_graph.rs | 1424 |
| H | ? | to_graph.rs | 1447 |
| H | ? | to_graph.rs | 1454 |
| H | ? | to_graph.rs | 1474 |
| H | ? | to_graph.rs | 1530 |
| H | ? | to_graph.rs | 1563 |
| H | ? | to_graph.rs | 1567 |
| H | ? | to_graph.rs | 1582 |
| H | ? | pipe.rs | 77 |
| H | ? | pipe.rs | 310 |
| H | ? | execute.rs | 160 |
| H | ? | execute.rs | 163 |
| H | ? | execute.rs | 222 |
| H | ? | execute.rs | 240 |
| H | ? | execute.rs | 369 |
| H | ? | mod.rs | 54 |
| H | ? | mod.rs | 92 |
| H | ? | single_key.rs | 82 |
| H | ? | single_key.rs | 94 |
| H | ? | single_key.rs | 115 |
| H | ? | row_encoded.rs | 32 |
| H | ? | execution_state.rs | 191 |
| H | ? | execution_state.rs | 212 |
| H | ? | execution_state.rs | 216 |
| H | ? | execution_state.rs | 217 |
| H | ? | execution_state.rs | 219 |
| H | ? | execution_state.rs | 221 |
| H | ? | execution_state.rs | 223 |
| H | ? | execution_state.rs | 224 |
| H | ? | execution_state.rs | 225 |
| H | ? | execution_state.rs | 243 |
| H | ? | execution_state.rs | 278 |
| H | ? | literal.rs | 33 |
| H | ? | literal.rs | 35 |
| H | ? | literal.rs | 126 |
| H | ? | field.rs | 54 |
| H | ? | field.rs | 65 |
| H | ? | field.rs | 72 |
| H | ? | mod.rs | 205 |
| H | ? | mod.rs | 454 |
| H | ? | mod.rs | 473 |
| H | ? | mod.rs | 484 |
| H | ? | mod.rs | 486 |
| H | ? | mod.rs | 497 |
| H | ? | mod.rs | 685 |
| H | ? | window.rs | 199 |
| H | ? | window.rs | 388 |
| H | ? | window.rs | 390 |
| H | ? | window.rs | 394 |
| H | ? | window.rs | 433 |
| H | ? | window.rs | 474 |
| H | ? | window.rs | 484 |
| H | ? | window.rs | 498 |
| H | ? | window.rs | 515 |
| H | ? | window.rs | 572 |
| H | ? | window.rs | 574 |
| H | ? | window.rs | 581 |
| H | ? | window.rs | 589 |
| H | ? | window.rs | 597 |
| H | ? | window.rs | 598 |
| H | ? | window.rs | 625 |
| H | ? | window.rs | 641 |
| H | ? | window.rs | 711 |
| H | ? | window.rs | 717 |
| H | ? | window.rs | 773 |
| H | ? | window.rs | 1128 |
| H | ? | window.rs | 1208 |
| H | ? | binary.rs | 162 |
| H | ? | binary.rs | 163 |
| H | ? | binary.rs | 204 |
| H | ? | binary.rs | 210 |
| H | ? | binary.rs | 211 |
| H | ? | binary.rs | 217 |
| H | ? | binary.rs | 374 |
| H | ? | filter.rs | 77 |
| H | ? | filter.rs | 132 |
| H | ? | rolling.rs | 30 |
| H | ? | rolling.rs | 48 |
| H | ? | rolling.rs | 55 |
| H | ? | rolling.rs | 63 |
| H | ? | rolling.rs | 90 |
| H | ? | rolling.rs | 104 |
| H | ? | rolling.rs | 249 |
| H | ? | cast.rs | 50 |
| H | ? | cast.rs | 66 |
| H | ? | cast.rs | 93 |
| H | ? | structeval.rs | 54 |
| H | ? | structeval.rs | 113 |
| H | ? | structeval.rs | 170 |
| H | ? | structeval.rs | 220 |
| H | ? | structeval.rs | 224 |
| H | ? | structeval.rs | 272 |
| H | ? | structeval.rs | 374 |
| H | ? | column.rs | 63 |
| H | ? | column.rs | 99 |
| H | ? | column.rs | 161 |
| H | ? | ternary.rs | 60 |
| H | ? | ternary.rs | 94 |
| H | ? | ternary.rs | 187 |
| H | ? | ternary.rs | 270 |
| H | ? | ternary.rs | 276 |
| H | ? | ternary.rs | 282 |
| H | ? | ternary.rs | 296 |
| H | ? | ternary.rs | 299 |
| H | ? | ternary.rs | 301 |
| H | ? | ternary.rs | 302 |
| H | ? | ternary.rs | 329 |
| H | ? | element.rs | 23 |
| H | ? | element.rs | 40 |
| H | ? | sortby.rs | 112 |
| H | ? | sortby.rs | 113 |
| H | ? | sortby.rs | 115 |
| H | ? | sortby.rs | 133 |
| H | ? | sortby.rs | 267 |
| H | ? | sortby.rs | 345 |
| H | ? | eval.rs | 72 |
| H | ? | eval.rs | 138 |
| H | ? | eval.rs | 139 |
| H | ? | eval.rs | 179 |
| H | ? | eval.rs | 180 |
| H | ? | eval.rs | 256 |
| H | ? | eval.rs | 314 |
| H | ? | eval.rs | 323 |
| H | ? | eval.rs | 325 |
| H | ? | eval.rs | 336 |
| H | ? | eval.rs | 357 |
| H | ? | eval.rs | 358 |
| H | ? | eval.rs | 391 |
| H | ? | eval.rs | 393 |
| H | ? | eval.rs | 396 |
| H | ? | eval.rs | 443 |
| H | ? | eval.rs | 448 |
| H | ? | eval.rs | 457 |
| H | ? | eval.rs | 480 |
| H | ? | eval.rs | 535 |
| H | ? | eval.rs | 571 |
| H | ? | eval.rs | 573 |
| H | ? | eval.rs | 590 |
| H | ? | eval.rs | 595 |
| H | ? | alias.rs | 22 |
| H | ? | alias.rs | 57 |
| H | ? | alias.rs | 58 |
| H | ? | apply.rs | 124 |
| H | ? | apply.rs | 129 |
| H | ? | apply.rs | 164 |
| H | ? | apply.rs | 176 |
| H | ? | apply.rs | 211 |
| H | ? | apply.rs | 216 |
| H | ? | apply.rs | 233 |
| H | ? | apply.rs | 297 |
| H | ? | apply.rs | 400 |
| H | ? | apply.rs | 448 |
| H | ? | apply.rs | 612 |
| H | ? | group_iter.rs | 20 |
| H | ? | group_iter.rs | 27 |
| H | ? | group_iter.rs | 38 |
| H | ? | group_iter.rs | 56 |
| H | ? | group_iter.rs | 68 |
| H | ? | group_iter.rs | 85 |
| H | ? | group_iter.rs | 98 |
| H | ? | group_iter.rs | 115 |
| H | ? | group_iter.rs | 128 |
| H | ? | group_iter.rs | 160 |
| H | ? | group_iter.rs | 175 |
| H | ? | group_iter.rs | 202 |
| H | ? | group_iter.rs | 207 |
| H | ? | group_iter.rs | 216 |
| H | ? | group_iter.rs | 244 |
| H | ? | count.rs | 86 |
| H | ? | count.rs | 89 |
| H | ? | aggregation.rs | 68 |
| H | ? | aggregation.rs | 71 |
| H | ? | aggregation.rs | 81 |
| H | ? | aggregation.rs | 94 |
| H | ? | aggregation.rs | 97 |
| H | ? | aggregation.rs | 107 |
| H | ? | aggregation.rs | 118 |
| H | ? | aggregation.rs | 119 |
| H | ? | aggregation.rs | 121 |
| H | ? | aggregation.rs | 128 |
| H | ? | aggregation.rs | 130 |
| H | ? | aggregation.rs | 137 |
| H | ? | aggregation.rs | 139 |
| H | ? | aggregation.rs | 144 |
| H | ? | aggregation.rs | 150 |
| H | ? | aggregation.rs | 155 |
| H | ? | aggregation.rs | 160 |
| H | ? | aggregation.rs | 163 |
| H | ? | aggregation.rs | 168 |
| H | ? | aggregation.rs | 171 |
| H | ? | aggregation.rs | 181 |
| H | ? | aggregation.rs | 184 |
| H | ? | aggregation.rs | 204 |
| H | ? | aggregation.rs | 301 |
| H | ? | aggregation.rs | 384 |
| H | ? | aggregation.rs | 438 |
| H | ? | aggregation.rs | 439 |
| H | ? | aggregation.rs | 456 |
| H | ? | aggregation.rs | 561 |
| H | ? | aggregation.rs | 580 |
| H | ? | aggregation.rs | 639 |
| H | ? | gather.rs | 98 |
| H | ? | gather.rs | 116 |
| H | ? | mod.rs | 253 |
| H | ? | mod.rs | 254 |
| H | ? | mod.rs | 350 |
| H | ? | mod.rs | 351 |
| H | ? | mod.rs | 392 |
| H | ? | mod.rs | 490 |
| H | ? | mod.rs | 491 |
| H | ? | mod.rs | 525 |
| H | ? | mod.rs | 576 |
| H | ? | mod.rs | 582 |
| H | ? | min_max.rs | 52 |
| H | ? | min_max.rs | 94 |
| H | ? | min_max.rs | 544 |
| H | ? | min_max.rs | 598 |
| H | ? | min_max.rs | 611 |
| H | ? | min_max.rs | 665 |
| H | ? | first_last.rs | 370 |
| H | ? | first_last.rs | 454 |
| H | ? | first_last.rs | 467 |
| H | ? | implode.rs | 102 |
| H | ? | implode.rs | 179 |
| H | ? | implode.rs | 246 |
| H | ? | implode.rs | 280 |
| H | ? | implode.rs | 371 |
| H | ? | implode.rs | 383 |
| H | ? | first_last_nonnull.rs | 347 |
| H | ? | first_last_nonnull.rs | 459 |
| H | ? | first_last_nonnull.rs | 470 |
| H | ? | approx_n_unique.rs | 55 |
| H | ? | min_max_by.rs | 25 |
| H | ? | min_max_by.rs | 61 |
| H | ? | min_max_by.rs | 77 |
| H | ? | min_max_by.rs | 113 |
| H | ? | min_max_by.rs | 501 |
| H | ? | min_max_by.rs | 559 |
| H | ? | min_max_by.rs | 646 |
| H | ? | min_max_by.rs | 647 |
| H | ? | min_max_by.rs | 796 |
| H | ? | min_max_by.rs | 797 |
| H | ? | min_max_by.rs | 813 |
| H | ? | convert.rs | 186 |
| H | ? | convert.rs | 187 |
| H | ? | convert.rs | 214 |
| H | ? | convert.rs | 215 |
| H | ? | cov.rs | 53 |
| H | ? | cov.rs | 148 |
| H | ? | cov.rs | 198 |
| H | ? | cov.rs | 293 |
| H | ? | planner.rs | 140 |
| H | ? | planner.rs | 158 |
| H | ? | planner.rs | 280 |
| H | ? | planner.rs | 303 |
| H | ? | planner.rs | 305 |
| H | ? | planner.rs | 321 |
| H | ? | planner.rs | 361 |
| H | ? | planner.rs | 382 |
| H | ? | planner.rs | 405 |
| H | ? | planner.rs | 447 |
| H | ? | planner.rs | 488 |
| H | ? | planner.rs | 514 |
| H | ? | planner.rs | 524 |
| H | ? | planner.rs | 552 |
| H | ? | planner.rs | 553 |
| H | ? | planner.rs | 581 |
| H | ? | planner.rs | 582 |
| H | ? | planner.rs | 615 |
| H | ? | planner.rs | 620 |
| H | ? | planner.rs | 659 |
| H | ? | hash_keys.rs | 146 |
| H | ? | hash_keys.rs | 148 |
| H | ? | hash_keys.rs | 404 |
| H | ? | single_key.rs | 70 |
| H | ? | single_key.rs | 153 |
| H | ? | row_encoded.rs | 55 |
| H | ? | binview.rs | 84 |
| H | ? | mod.rs | 170 |
| H | ? | mod.rs | 219 |
| H | ? | mod.rs | 220 |
| H | ? | mod.rs | 221 |
| H | ? | mod.rs | 222 |
| H | ? | mod.rs | 223 |
| H | ? | mod.rs | 224 |
| H | ? | mod.rs | 225 |
| H | ? | mod.rs | 226 |
| H | ? | mod.rs | 228 |
| H | ? | mod.rs | 230 |
| H | ? | mod.rs | 238 |
| H | ? | mod.rs | 244 |
| H | ? | mod.rs | 256 |
| H | ? | mod.rs | 257 |
| H | ? | mod.rs | 258 |
| H | ? | mod.rs | 259 |
| H | ? | mod.rs | 261 |
| H | ? | mod.rs | 263 |
| H | ? | mod.rs | 264 |
| H | ? | mod.rs | 265 |
| H | ? | mod.rs | 317 |
| H | ? | mod.rs | 336 |
| H | ? | mod.rs | 395 |
| H | ? | mod.rs | 396 |
| H | ? | mod.rs | 409 |
| H | ? | mod.rs | 410 |
| H | ? | mod.rs | 522 |
| H | ? | mod.rs | 532 |
| H | ? | mod.rs | 536 |
| H | ? | misc.rs | 36 |
| H | ? | misc.rs | 80 |
| H | ? | misc.rs | 109 |
| H | ? | misc.rs | 190 |
| H | ? | misc.rs | 196 |
| H | ? | misc.rs | 213 |
| H | ? | misc.rs | 223 |
| H | ? | misc.rs | 240 |
| H | ? | misc.rs | 250 |
| H | ? | misc.rs | 275 |
| H | ? | misc.rs | 288 |
| H | ? | misc.rs | 296 |
| H | ? | misc.rs | 318 |
| H | ? | misc.rs | 411 |
| H | ? | misc.rs | 423 |
| H | ? | misc.rs | 440 |
| H | ? | misc.rs | 465 |
| H | ? | misc.rs | 501 |
| H | ? | misc.rs | 573 |
| H | ? | misc.rs | 581 |
| H | ? | misc.rs | 603 |
| H | ? | misc.rs | 680 |
| H | ? | misc.rs | 700 |
| H | ? | misc.rs | 702 |
| H | ? | misc.rs | 751 |
| H | ? | strings.rs | 58 |
| H | ? | strings.rs | 84 |
| H | ? | strings.rs | 98 |
| H | ? | strings.rs | 114 |
| H | ? | strings.rs | 377 |
| H | ? | strings.rs | 398 |
| H | ? | strings.rs | 603 |
| H | ? | strings.rs | 624 |
| H | ? | strings.rs | 644 |
| H | ? | cat.rs | 34 |
| H | ? | cat.rs | 43 |
| H | ? | cat.rs | 48 |
| H | ? | random.rs | 28 |
| H | ? | random.rs | 51 |
| H | ? | binary.rs | 52 |
| H | ? | binary.rs | 62 |
| H | ? | binary.rs | 72 |
| H | ? | binary.rs | 120 |
| H | ? | binary.rs | 128 |
| H | ? | binary.rs | 136 |
| H | ? | datetime.rs | 83 |
| H | ? | datetime.rs | 113 |
| H | ? | datetime.rs | 275 |
| H | ? | datetime.rs | 276 |
| H | ? | datetime.rs | 285 |
| H | ? | datetime.rs | 291 |
| H | ? | array.rs | 38 |
| H | ? | array.rs | 48 |
| H | ? | array.rs | 50 |
| H | ? | array.rs | 95 |
| H | ? | array.rs | 138 |
| H | ? | array.rs | 212 |
| H | ? | list.rs | 78 |
| H | ? | list.rs | 154 |
| H | ? | list.rs | 230 |
| H | ? | list.rs | 248 |
| H | ? | list.rs | 377 |
| H | ? | list.rs | 379 |
| H | ? | list.rs | 382 |
| H | ? | list.rs | 385 |
| H | ? | list.rs | 387 |
| H | ? | list.rs | 406 |
| H | ? | list.rs | 416 |
| H | ? | rolling.rs | 35 |
| H | ? | rolling.rs | 159 |
| H | ? | rolling.rs | 161 |
| H | ? | rolling.rs | 177 |
| H | ? | rolling.rs | 179 |
| H | ? | rolling.rs | 191 |
| H | ? | rolling.rs | 192 |
| H | ? | rolling.rs | 201 |
| H | ? | rolling.rs | 205 |
| H | ? | rolling.rs | 210 |
| H | ? | rolling.rs | 230 |
| H | ? | groups_dispatch.rs | 93 |
| H | ? | groups_dispatch.rs | 150 |
| H | ? | groups_dispatch.rs | 381 |
| H | ? | groups_dispatch.rs | 383 |
| H | ? | groups_dispatch.rs | 480 |
| H | ? | groups_dispatch.rs | 497 |
| H | ? | groups_dispatch.rs | 521 |
| H | ? | groups_dispatch.rs | 581 |
| H | ? | groups_dispatch.rs | 588 |
| H | ? | groups_dispatch.rs | 726 |
| H | ? | groups_dispatch.rs | 823 |
| H | ? | groups_dispatch.rs | 880 |
| H | ? | struct_.rs | 17 |
| H | ? | struct_.rs | 38 |
| H | ? | struct_.rs | 39 |
| H | ? | struct_.rs | 43 |
| H | ? | struct_.rs | 54 |
| H | ? | struct_.rs | 60 |
| H | ? | struct_.rs | 71 |
| H | ? | struct_.rs | 77 |
| H | ? | struct_.rs | 91 |
| H | ? | struct_.rs | 111 |
| H | ? | struct_.rs | 125 |
| H | ? | struct_.rs | 127 |
| H | ? | struct_.rs | 134 |
| H | ? | shift_and_fill.rs | 112 |
| H | ? | shift_and_fill.rs | 134 |
| H | ? | extension.rs | 11 |
| H | ? | extension.rs | 40 |
| H | ? | extension.rs | 44 |
| H | ? | boolean.rs | 58 |
| H | ? | boolean.rs | 60 |
| H | ? | boolean.rs | 67 |
| H | ? | boolean.rs | 69 |
| H | ? | boolean.rs | 79 |
| H | ? | boolean.rs | 83 |
| H | ? | boolean.rs | 182 |
| H | ? | boolean.rs | 207 |
| H | ? | boolean.rs | 229 |
| H | ? | bitwise.rs | 50 |
| H | ? | bitwise.rs | 54 |
| H | ? | bitwise.rs | 58 |
| H | ? | time_range.rs | 28 |
| H | ? | time_range.rs | 50 |
| H | ? | mod.rs | 18 |
| H | ? | mod.rs | 21 |
| H | ? | datetime_range.rs | 115 |
| H | ? | datetime_range.rs | 137 |
| H | ? | datetime_range.rs | 167 |
| H | ? | linear_space.rs | 36 |
| H | ? | linear_space.rs | 49 |
| H | ? | linear_space.rs | 63 |
| H | ? | linear_space.rs | 85 |
| H | ? | linear_space.rs | 159 |
| H | ? | linear_space.rs | 160 |
| H | ? | int_range.rs | 24 |
| H | ? | int_range.rs | 51 |
| H | ? | horizontal.rs | 15 |
| H | ? | horizontal.rs | 16 |
| H | ? | horizontal.rs | 18 |
| H | ? | horizontal.rs | 48 |
| H | ? | horizontal.rs | 58 |
| H | ? | horizontal.rs | 60 |
| H | ? | horizontal.rs | 94 |
| H | ? | horizontal.rs | 105 |
| H | ? | horizontal.rs | 106 |
| H | ? | horizontal.rs | 108 |
| H | ? | horizontal.rs | 109 |
| H | ? | horizontal.rs | 125 |
| H | ? | horizontal.rs | 128 |
| H | ? | horizontal.rs | 143 |
| H | ? | horizontal.rs | 145 |
| H | ? | horizontal.rs | 149 |
| H | ? | horizontal.rs | 153 |
| H | ? | horizontal.rs | 154 |
| H | ? | horizontal.rs | 170 |
| H | ? | horizontal.rs | 173 |
| H | ? | pow.rs | 26 |
| H | ? | pow.rs | 47 |
| H | ? | pow.rs | 50 |
| H | ? | pow.rs | 55 |
| H | ? | pow.rs | 58 |
| H | ? | pow.rs | 86 |
| H | ? | pow.rs | 89 |
| H | ? | pow.rs | 91 |
| H | ? | pow.rs | 94 |
| H | ? | rolling_by.rs | 26 |
| H | ? | cache.rs | 32 |
| H | ? | slice_enum.rs | 41 |
| H | ? | slice_enum.rs | 53 |
| H | ? | pl_path.rs | 330 |
| H | ? | pl_path.rs | 635 |
| H | ? | arena.rs | 145 |
| H | ? | collection.rs | 91 |
| H | ? | error_capture.rs | 14 |
| H | ? | python_convert_registry.rs | 107 |
| H | ? | order_statistic_tree.rs | 505 |
| H | ? | python_function.rs | 72 |
| H | ? | idx_vec.rs | 221 |
| H | ? | idx_vec.rs | 455 |
| H | ? | idx_vec.rs | 471 |
| H | ? | key.rs | 103 |
| H | ? | total_ord.rs | 194 |
| H | ? | total_ord.rs | 551 |
| H | ? | total_ord.rs | 608 |
| H | ? | pl_ref_str.rs | 27 |
| H | ? | version_0.rs | 64 |
| H | ? | version_0.rs | 71 |
| H | ? | version_0.rs | 102 |
| H | ? | callback.rs | 103 |
| H | ? | callback.rs | 104 |
| H | ? | string.rs | 180 |
| H | ? | mod.rs | 422 |
| H | ? | mod.rs | 449 |
| H | ? | mod.rs | 839 |
| H | ? | mod.rs | 851 |
| H | ? | mod.rs | 854 |
| H | ? | mod.rs | 904 |
| H | ? | mod.rs | 1064 |
| H | ? | source.rs | 37 |
| H | ? | python_udf.rs | 115 |
| H | ? | python_udf.rs | 140 |
| H | ? | python_udf.rs | 158 |
| H | ? | python_udf.rs | 171 |
| H | ? | python_udf.rs | 180 |
| H | ? | python_udf.rs | 186 |
| H | ? | python_udf.rs | 187 |
| H | ? | datatype_expr.rs | 103 |
| H | ? | datatype_expr.rs | 204 |
| H | ? | selector.rs | 182 |
| H | ? | selector.rs | 234 |
| H | ? | selector.rs | 253 |
| H | ? | selector.rs | 305 |
| H | ? | array.rs | 149 |
| H | ? | list.rs | 193 |
| H | ? | builder_dsl.rs | 32 |
| H | ? | builder_dsl.rs | 46 |
| H | ? | builder_dsl.rs | 305 |
| H | ? | plan.rs | 200 |
| H | ? | plan.rs | 201 |
| H | ? | plan.rs | 202 |
| H | ? | plan.rs | 203 |
| H | ? | plan.rs | 204 |
| H | ? | plan.rs | 205 |
| H | ? | plan.rs | 206 |
| H | ? | plan.rs | 207 |
| H | ? | plan.rs | 208 |
| H | ? | plan.rs | 209 |
| H | ? | plan.rs | 210 |
| H | ? | plan.rs | 211 |
| H | ? | plan.rs | 212 |
| H | ? | plan.rs | 213 |
| H | ? | plan.rs | 214 |
| H | ? | plan.rs | 215 |
| H | ? | plan.rs | 216 |
| H | ? | plan.rs | 217 |
| H | ? | plan.rs | 218 |
| H | ? | plan.rs | 219 |
| H | ? | plan.rs | 220 |
| H | ? | plan.rs | 222 |
| H | ? | plan.rs | 224 |
| H | ? | plan.rs | 225 |
| H | ? | plan.rs | 233 |
| H | ? | plan.rs | 248 |
| H | ? | plan.rs | 252 |
| H | ? | plan.rs | 262 |
| H | ? | mod.rs | 211 |
| H | ? | mod.rs | 738 |
| H | ? | python_delta_dv_provider.rs | 42 |
| H | ? | python_delta_dv_provider.rs | 60 |
| H | ? | struct_.rs | 33 |
| H | ? | concat.rs | 54 |
| H | ? | concat.rs | 65 |
| H | ? | concat.rs | 109 |
| H | ? | concat.rs | 121 |
| H | ? | concat.rs | 147 |
| H | ? | selectors.rs | 64 |
| H | ? | selectors.rs | 101 |
| H | ? | sink.rs | 105 |
| H | ? | sink.rs | 133 |
| H | ? | sink.rs | 417 |
| H | ? | sink.rs | 421 |
| H | ? | sink.rs | 425 |
| H | ? | sink.rs | 517 |
| H | ? | serializable_plan.rs | 195 |
| H | ? | serializable_plan.rs | 199 |
| H | ? | serializable_plan.rs | 211 |
| H | ? | serializable_plan.rs | 212 |
| H | ? | serializable_plan.rs | 213 |
| H | ? | serializable_plan.rs | 217 |
| H | ? | serializable_plan.rs | 224 |
| H | ? | serializable_plan.rs | 238 |
| H | ? | serializable_plan.rs | 239 |
| H | ? | serializable_plan.rs | 240 |
| H | ? | serializable_plan.rs | 242 |
| H | ? | serializable_plan.rs | 243 |
| H | ? | serializable_plan.rs | 255 |
| H | ? | serializable_plan.rs | 256 |
| H | ? | serializable_plan.rs | 257 |
| H | ? | serializable_plan.rs | 258 |
| H | ? | serializable_plan.rs | 275 |
| H | ? | serializable_plan.rs | 285 |
| H | ? | serializable_plan.rs | 286 |
| H | ? | serializable_plan.rs | 294 |
| H | ? | serializable_plan.rs | 309 |
| H | ? | serializable_plan.rs | 311 |
| H | ? | serializable_plan.rs | 312 |
| H | ? | serializable_plan.rs | 313 |
| H | ? | serializable_plan.rs | 315 |
| H | ? | serializable_plan.rs | 320 |
| H | ? | serializable_plan.rs | 329 |
| H | ? | serializable_plan.rs | 331 |
| H | ? | serializable_plan.rs | 340 |
| H | ? | serializable_plan.rs | 365 |
| H | ? | serializable_plan.rs | 382 |
| H | ? | serializable_plan.rs | 399 |
| H | ? | serializable_plan.rs | 453 |
| H | ? | serializable_plan.rs | 457 |
| H | ? | serializable_plan.rs | 468 |
| H | ? | serializable_plan.rs | 469 |
| H | ? | serializable_plan.rs | 470 |
| H | ? | serializable_plan.rs | 475 |
| H | ? | serializable_plan.rs | 482 |
| H | ? | serializable_plan.rs | 496 |
| H | ? | serializable_plan.rs | 497 |
| H | ? | serializable_plan.rs | 498 |
| H | ? | serializable_plan.rs | 500 |
| H | ? | serializable_plan.rs | 501 |
| H | ? | serializable_plan.rs | 513 |
| H | ? | serializable_plan.rs | 514 |
| H | ? | serializable_plan.rs | 515 |
| H | ? | serializable_plan.rs | 516 |
| H | ? | serializable_plan.rs | 533 |
| H | ? | serializable_plan.rs | 543 |
| H | ? | serializable_plan.rs | 544 |
| H | ? | serializable_plan.rs | 554 |
| H | ? | serializable_plan.rs | 569 |
| H | ? | serializable_plan.rs | 571 |
| H | ? | serializable_plan.rs | 572 |
| H | ? | serializable_plan.rs | 573 |
| H | ? | serializable_plan.rs | 575 |
| H | ? | serializable_plan.rs | 580 |
| H | ? | serializable_plan.rs | 589 |
| H | ? | serializable_plan.rs | 591 |
| H | ? | serializable_plan.rs | 600 |
| H | ? | serializable_plan.rs | 625 |
| H | ? | serializable_plan.rs | 642 |
| H | ? | serializable_plan.rs | 658 |
| H | ? | serializable_plan.rs | 663 |
| H | ? | serializable_plan.rs | 664 |
| H | ? | serializable_plan.rs | 674 |
| H | ? | serializable_plan.rs | 681 |
| H | ? | serializable_plan.rs | 720 |
| H | ? | serializable_plan.rs | 761 |
| H | ? | serializable_plan.rs | 762 |
| H | ? | serializable_plan.rs | 770 |
| H | ? | scan_sources.rs | 87 |
| H | ? | scan_sources.rs | 96 |
| H | ? | scan_sources.rs | 200 |
| H | ? | scan_sources.rs | 236 |
| H | ? | scan_sources.rs | 263 |
| H | ? | scan_sources.rs | 356 |
| H | ? | scan_sources.rs | 357 |
| H | ? | scan_sources.rs | 376 |
| H | ? | scan_sources.rs | 384 |
| H | ? | scan_sources.rs | 416 |
| H | ? | scan_sources.rs | 428 |
| H | ? | scan_sources.rs | 453 |
| H | ? | scan_sources.rs | 489 |
| H | ? | scan_sources.rs | 502 |
| H | ? | scan_sources.rs | 508 |
| H | ? | meta.rs | 33 |
| H | ? | mod.rs | 450 |
| H | ? | mod.rs | 854 |
| H | ? | serde_expr.rs | 43 |
| H | ? | agg.rs | 23 |
| H | ? | agg.rs | 31 |
| H | ? | udf.rs | 70 |
| H | ? | udf.rs | 78 |
| H | ? | udf.rs | 84 |
| H | ? | constants.rs | 15 |
| H | ? | constants.rs | 19 |
| H | ? | constants.rs | 23 |
| H | ? | constants.rs | 27 |
| H | ? | lit.rs | 158 |
| H | ? | lit.rs | 244 |
| H | ? | lit.rs | 329 |
| H | ? | lit.rs | 331 |
| H | ? | lit.rs | 354 |
| H | ? | lit.rs | 355 |
| H | ? | lit.rs | 356 |
| H | ? | lit.rs | 416 |
| H | ? | lit.rs | 421 |
| H | ? | hive.rs | 106 |
| H | ? | hive.rs | 124 |
| H | ? | hive.rs | 127 |
| H | ? | builder_ir.rs | 103 |
| H | ? | builder_ir.rs | 136 |
| H | ? | builder_ir.rs | 162 |
| H | ? | builder_ir.rs | 212 |
| H | ? | builder_ir.rs | 232 |
| H | ? | builder_ir.rs | 245 |
| H | ? | builder_ir.rs | 246 |
| H | ? | builder_ir.rs | 248 |
| H | ? | builder_ir.rs | 289 |
| H | ? | builder_ir.rs | 294 |
| H | ? | builder_ir.rs | 295 |
| H | ? | builder_ir.rs | 297 |
| H | ? | builder_ir.rs | 311 |
| H | ? | collapse_sort.rs | 72 |
| H | ? | collapse_sort.rs | 73 |
| H | ? | collapse_sort.rs | 74 |
| H | ? | collapse_sort.rs | 78 |
| H | ? | collapse_sort.rs | 79 |
| H | ? | collapse_sort.rs | 80 |
| H | ? | collapse_sort.rs | 95 |
| H | ? | collapse_sort.rs | 105 |
| H | ? | collapse_sort.rs | 110 |
| H | ? | collapse_sort.rs | 161 |
| H | ? | deep_copy.rs | 31 |
| H | ? | mod.rs | 277 |
| H | ? | stack_opt.rs | 106 |
| H | ? | stack_opt.rs | 108 |
| H | ? | fused.rs | 125 |
| H | ? | mod.rs | 138 |
| H | ? | mod.rs | 185 |
| H | ? | mod.rs | 190 |
| H | ? | mod.rs | 196 |
| H | ? | mod.rs | 345 |
| H | ? | mod.rs | 519 |
| H | ? | mod.rs | 520 |
| H | ? | mod.rs | 569 |
| H | ? | mod.rs | 626 |
| H | ? | mod.rs | 697 |
| H | ? | mod.rs | 707 |
| H | ? | mod.rs | 713 |
| H | ? | mod.rs | 736 |
| H | ? | mod.rs | 741 |
| H | ? | mod.rs | 926 |
| H | ? | mod.rs | 956 |
| H | ? | mod.rs | 966 |
| H | ? | mod.rs | 992 |
| H | ? | mod.rs | 998 |
| H | ? | mod.rs | 1028 |
| H | ? | mod.rs | 1034 |
| H | ? | mod.rs | 1081 |
| H | ? | mod.rs | 1106 |
| H | ? | mod.rs | 1107 |
| H | ? | mod.rs | 1110 |
| H | ? | mod.rs | 1193 |
| H | ? | mod.rs | 1234 |
| H | ? | mod.rs | 1239 |
| H | ? | mod.rs | 1293 |
| H | ? | mod.rs | 1334 |
| H | ? | mod.rs | 1337 |
| H | ? | mod.rs | 1338 |
| H | ? | mod.rs | 1445 |
| H | ? | mod.rs | 1518 |
| H | ? | mod.rs | 1574 |
| H | ? | mod.rs | 1629 |
| H | ? | mod.rs | 1642 |
| H | ? | mod.rs | 1689 |
| H | ? | mod.rs | 1695 |
| H | ? | mod.rs | 1716 |
| H | ? | mod.rs | 1718 |
| H | ? | mod.rs | 1726 |
| H | ? | mod.rs | 1758 |
| H | ? | mod.rs | 1956 |
| H | ? | mod.rs | 2072 |
| H | ? | mod.rs | 2073 |
| H | ? | edge.rs | 44 |
| H | ? | edge.rs | 83 |
| H | ? | slice_pushdown_lp.rs | 323 |
| H | ? | expand_datasets.rs | 68 |
| H | ? | expand_datasets.rs | 80 |
| H | ? | expand_datasets.rs | 240 |
| H | ? | expand_datasets.rs | 347 |
| H | ? | expand_datasets.rs | 350 |
| H | ? | expand_datasets.rs | 353 |
| H | ? | expand_datasets.rs | 354 |
| H | ? | expand_datasets.rs | 355 |
| H | ? | expand_datasets.rs | 356 |
| H | ? | expand_datasets.rs | 391 |
| H | ? | expand_datasets.rs | 393 |
| H | ? | expand_datasets.rs | 444 |
| H | ? | expand_datasets.rs | 462 |
| H | ? | expand_datasets.rs | 463 |
| H | ? | mod.rs | 163 |
| H | ? | mod.rs | 265 |
| H | ? | mod.rs | 271 |
| H | ? | mod.rs | 362 |
| H | ? | mod.rs | 425 |
| H | ? | mod.rs | 217 |
| H | ? | mod.rs | 256 |
| H | ? | mod.rs | 272 |
| H | ? | mod.rs | 277 |
| H | ? | mod.rs | 374 |
| H | ? | mod.rs | 378 |
| H | ? | mod.rs | 531 |
| H | ? | mod.rs | 537 |
| H | ? | mod.rs | 538 |
| H | ? | mod.rs | 562 |
| H | ? | predicate_pruning.rs | 258 |
| H | ? | predicate_pruning.rs | 305 |
| H | ? | predicate_pruning.rs | 555 |
| H | ? | predicate_pruning.rs | 624 |
| H | ? | predicate_pruning.rs | 651 |
| H | ? | predicate_pruning.rs | 716 |
| H | ? | predicate_pruning.rs | 719 |
| H | ? | predicate_pruning.rs | 720 |
| H | ? | predicate_pruning.rs | 722 |
| H | ? | predicate_pruning.rs | 729 |
| H | ? | predicate_pruning.rs | 730 |
| H | ? | predicate_pruning.rs | 745 |
| H | ? | predicate_pruning.rs | 751 |
| H | ? | predicate_pruning.rs | 756 |
| H | ? | predicate_pruning.rs | 763 |
| H | ? | predicate_pruning.rs | 764 |
| H | ? | predicate_pruning.rs | 769 |
| H | ? | predicate_pruning.rs | 849 |
| H | ? | predicate_pruning.rs | 852 |
| H | ? | predicate_pruning.rs | 853 |
| H | ? | predicate_pruning.rs | 858 |
| H | ? | predicate_pruning.rs | 866 |
| H | ? | predicate_pruning.rs | 867 |
| H | ? | predicate_pruning.rs | 869 |
| H | ? | predicate_pruning.rs | 872 |
| H | ? | predicate_pruning.rs | 879 |
| H | ? | predicate_pruning.rs | 881 |
| H | ? | predicate_pruning.rs | 901 |
| H | ? | predicate_pruning.rs | 906 |
| H | ? | predicate_pruning.rs | 915 |
| H | ? | dynamic.rs | 134 |
| H | ? | hive.rs | 11 |
| H | ? | hive.rs | 87 |
| H | ? | hive.rs | 94 |
| H | ? | hive.rs | 106 |
| H | ? | hive.rs | 117 |
| H | ? | hive.rs | 118 |
| H | ? | hive.rs | 119 |
| H | ? | hive.rs | 121 |
| H | ? | hive.rs | 122 |
| H | ? | hive.rs | 175 |
| H | ? | hive.rs | 186 |
| H | ? | hive.rs | 192 |
| H | ? | hive.rs | 201 |
| H | ? | hive.rs | 209 |
| H | ? | hive.rs | 211 |
| H | ? | hive.rs | 214 |
| H | ? | hive.rs | 216 |
| H | ? | hive.rs | 222 |
| H | ? | hive.rs | 223 |
| H | ? | hive.rs | 224 |
| H | ? | hive.rs | 225 |
| H | ? | hive.rs | 249 |
| H | ? | hive.rs | 250 |
| H | ? | hive.rs | 251 |
| H | ? | hive.rs | 252 |
| H | ? | hive.rs | 271 |
| H | ? | hive.rs | 272 |
| H | ? | hive.rs | 273 |
| H | ? | hive.rs | 274 |
| H | ? | group_by.rs | 53 |
| H | ? | group_by.rs | 55 |
| H | ? | group_by.rs | 77 |
| H | ? | keys.rs | 23 |
| H | ? | utils.rs | 62 |
| H | ? | utils.rs | 115 |
| H | ? | utils.rs | 139 |
| H | ? | utils.rs | 143 |
| H | ? | utils.rs | 174 |
| H | ? | utils.rs | 211 |
| H | ? | utils.rs | 259 |
| H | ? | utils.rs | 266 |
| H | ? | utils.rs | 289 |
| H | ? | utils.rs | 397 |
| H | ? | utils.rs | 516 |
| H | ? | mod.rs | 187 |
| H | ? | expr.rs | 334 |
| H | ? | expr.rs | 492 |
| H | ? | slice_pushdown_expr.rs | 146 |
| H | ? | slice_pushdown_expr.rs | 221 |
| H | ? | slice_pushdown_expr.rs | 405 |
| H | ? | slice_pushdown_expr.rs | 427 |
| H | ? | cluster_with_columns.rs | 70 |
| H | ? | cluster_with_columns.rs | 105 |
| H | ? | cluster_with_columns.rs | 126 |
| H | ? | cluster_with_columns.rs | 130 |
| H | ? | cluster_with_columns.rs | 141 |
| H | ? | cluster_with_columns.rs | 146 |
| H | ? | cluster_with_columns.rs | 152 |
| H | ? | cluster_with_columns.rs | 168 |
| H | ? | filter_constraint.rs | 39 |
| H | ? | sortedness.rs | 201 |
| H | ? | sortedness.rs | 250 |
| H | ? | sortedness.rs | 255 |
| H | ? | sortedness.rs | 264 |
| H | ? | sortedness.rs | 287 |
| H | ? | sortedness.rs | 295 |
| H | ? | sortedness.rs | 324 |
| H | ? | sortedness.rs | 326 |
| H | ? | sortedness.rs | 335 |
| H | ? | sortedness.rs | 364 |
| H | ? | sortedness.rs | 390 |
| H | ? | sortedness.rs | 393 |
| H | ? | sortedness.rs | 410 |
| H | ? | sortedness.rs | 420 |
| H | ? | sortedness.rs | 436 |
| H | ? | sortedness.rs | 451 |
| H | ? | sortedness.rs | 515 |
| H | ? | sortedness.rs | 550 |
| H | ? | sortedness.rs | 567 |
| H | ? | sortedness.rs | 585 |
| H | ? | sortedness.rs | 599 |
| H | ? | collapse_and_project.rs | 55 |
| H | ? | collapse_and_project.rs | 78 |
| H | ? | collapse_and_project.rs | 89 |
| H | ? | collapse_and_project.rs | 99 |
| H | ? | cache_states.rs | 291 |
| H | ? | cache_states.rs | 345 |
| H | ? | cache_states.rs | 406 |
| H | ? | cache_states.rs | 431 |
| H | ? | cache_states.rs | 436 |
| H | ? | cache_states.rs | 446 |
| H | ? | cache_states.rs | 448 |
| H | ? | cspe.rs | 263 |
| H | ? | cspe.rs | 293 |
| H | ? | csee.rs | 142 |
| H | ? | csee.rs | 545 |
| H | ? | csee.rs | 550 |
| H | ? | csee.rs | 678 |
| H | ? | csee.rs | 865 |
| H | ? | csee.rs | 912 |
| H | ? | csee.rs | 925 |
| H | ? | csee.rs | 937 |
| H | ? | csee.rs | 1019 |
| H | ? | csee.rs | 1064 |
| H | ? | csee.rs | 1112 |
| H | ? | csee.rs | 1113 |
| H | ? | csee.rs | 1114 |
| H | ? | csee.rs | 1115 |
| H | ? | mod.rs | 290 |
| H | ? | mod.rs | 443 |
| H | ? | mod.rs | 464 |
| H | ? | mod.rs | 468 |
| H | ? | mod.rs | 494 |
| H | ? | mod.rs | 543 |
| H | ? | mod.rs | 944 |
| H | ? | mod.rs | 945 |
| H | ? | arity.rs | 28 |
| H | ? | arity.rs | 36 |
| H | ? | arity.rs | 105 |
| H | ? | arity.rs | 113 |
| H | ? | arity.rs | 167 |
| H | ? | arity.rs | 178 |
| H | ? | simplify_functions.rs | 99 |
| H | ? | simplify_functions.rs | 104 |
| H | ? | simplify_functions.rs | 127 |
| H | ? | simplify_functions.rs | 132 |
| H | ? | simplify_functions.rs | 216 |
| H | ? | simplify_functions.rs | 233 |
| H | ? | simplify_functions.rs | 350 |
| H | ? | parquet_metadata_prune.rs | 67 |
| H | ? | parquet_metadata_prune.rs | 92 |
| H | ? | flatten_merge_sorted.rs | 38 |
| H | ? | mod.rs | 209 |
| H | ? | mod.rs | 217 |
| H | ? | mod.rs | 235 |
| H | ? | mod.rs | 238 |
| H | ? | python_udf.rs | 14 |
| H | ? | dsl.rs | 126 |
| H | ? | schema.rs | 39 |
| H | ? | schema.rs | 43 |
| H | ? | schema.rs | 58 |
| H | ? | schema.rs | 66 |
| H | ? | schema.rs | 79 |
| H | ? | schema.rs | 93 |
| H | ? | schema.rs | 114 |
| H | ? | schema.rs | 116 |
| H | ? | schema.rs | 119 |
| H | ? | schema.rs | 130 |
| H | ? | schema.rs | 132 |
| H | ? | schema.rs | 138 |
| H | ? | schema.rs | 142 |
| H | ? | schema.rs | 150 |
| H | ? | schema.rs | 162 |
| H | ? | schema.rs | 168 |
| H | ? | schema.rs | 171 |
| H | ? | schema.rs | 181 |
| H | ? | schema.rs | 183 |
| H | ? | count.rs | 39 |
| H | ? | count.rs | 43 |
| H | ? | count.rs | 56 |
| H | ? | prune.rs | 96 |
| H | ? | prune.rs | 103 |
| H | ? | prune.rs | 141 |
| H | ? | prune.rs | 153 |
| H | ? | prune.rs | 272 |
| H | ? | prune.rs | 285 |
| H | ? | lp.rs | 97 |
| H | ? | expr.rs | 214 |
| H | ? | schema.rs | 25 |
| H | ? | schema.rs | 84 |
| H | ? | schema.rs | 87 |
| H | ? | schema.rs | 122 |
| H | ? | schema.rs | 155 |
| H | ? | schema.rs | 166 |
| H | ? | schema.rs | 168 |
| H | ? | schema.rs | 234 |
| H | ? | schema.rs | 236 |
| H | ? | schema.rs | 295 |
| H | ? | schema.rs | 335 |
| H | ? | schema.rs | 341 |
| H | ? | utils.rs | 15 |
| H | ? | utils.rs | 37 |
| H | ? | stack_opt.rs | 149 |
| H | ? | stack_opt.rs | 150 |
| H | ? | stack_opt.rs | 168 |
| H | ? | ir_to_dsl.rs | 8 |
| H | ? | ir_to_dsl.rs | 206 |
| H | ? | ir_to_dsl.rs | 209 |
| H | ? | mod.rs | 65 |
| H | ? | mod.rs | 74 |
| H | ? | mod.rs | 103 |
| H | ? | mod.rs | 123 |
| H | ? | mod.rs | 128 |
| H | ? | mod.rs | 157 |
| H | ? | mod.rs | 168 |
| H | ? | mod.rs | 214 |
| H | ? | mod.rs | 259 |
| H | ? | mod.rs | 260 |
| H | ? | mod.rs | 261 |
| H | ? | mod.rs | 289 |
| H | ? | mod.rs | 325 |
| H | ? | mod.rs | 486 |
| H | ? | mod.rs | 573 |
| H | ? | mod.rs | 574 |
| H | ? | mod.rs | 607 |
| H | ? | mod.rs | 611 |
| H | ? | mod.rs | 717 |
| H | ? | mod.rs | 718 |
| H | ? | mod.rs | 723 |
| H | ? | mod.rs | 726 |
| H | ? | mod.rs | 806 |
| H | ? | mod.rs | 807 |
| H | ? | mod.rs | 884 |
| H | ? | mod.rs | 885 |
| H | ? | mod.rs | 909 |
| H | ? | mod.rs | 910 |
| H | ? | mod.rs | 960 |
| H | ? | mod.rs | 961 |
| H | ? | mod.rs | 1009 |
| H | ? | mod.rs | 1010 |
| H | ? | mod.rs | 1048 |
| H | ? | mod.rs | 1049 |
| H | ? | mod.rs | 1109 |
| H | ? | mod.rs | 1110 |
| H | ? | mod.rs | 1160 |
| H | ? | mod.rs | 1161 |
| H | ? | mod.rs | 1162 |
| H | ? | mod.rs | 1204 |
| H | ? | mod.rs | 1205 |
| H | ? | mod.rs | 1235 |
| H | ? | mod.rs | 1236 |
| H | ? | mod.rs | 1313 |
| H | ? | mod.rs | 1314 |
| H | ? | mod.rs | 1364 |
| H | ? | mod.rs | 1378 |
| H | ? | mod.rs | 1390 |
| H | ? | mod.rs | 1400 |
| H | ? | mod.rs | 1409 |
| H | ? | mod.rs | 1410 |
| H | ? | mod.rs | 1464 |
| H | ? | mod.rs | 1471 |
| H | ? | mod.rs | 1498 |
| H | ? | mod.rs | 1507 |
| H | ? | mod.rs | 1513 |
| H | ? | mod.rs | 1563 |
| H | ? | mod.rs | 1570 |
| H | ? | mod.rs | 1573 |
| H | ? | mod.rs | 1629 |
| H | ? | mod.rs | 1640 |
| H | ? | binary.rs | 67 |
| H | ? | binary.rs | 83 |
| H | ? | binary.rs | 131 |
| H | ? | binary.rs | 333 |
| H | ? | binary.rs | 334 |
| H | ? | binary.rs | 340 |
| H | ? | binary.rs | 424 |
| H | ? | binary.rs | 581 |
| H | ? | binary.rs | 665 |
| H | ? | binary.rs | 676 |
| H | ? | binary.rs | 715 |
| H | ? | binary.rs | 725 |
| H | ? | datetime.rs | 70 |
| H | ? | datetime.rs | 73 |
| H | ? | datetime.rs | 88 |
| H | ? | datetime.rs | 98 |
| H | ? | datetime.rs | 108 |
| H | ? | datetime.rs | 122 |
| H | ? | datetime.rs | 125 |
| H | ? | datetime.rs | 134 |
| H | ? | datetime.rs | 165 |
| H | ? | datetime.rs | 174 |
| H | ? | is_in.rs | 55 |
| H | ? | is_in.rs | 57 |
| H | ? | is_in.rs | 76 |
| H | ? | is_in.rs | 81 |
| H | ? | is_in.rs | 88 |
| H | ? | is_in.rs | 90 |
| H | ? | is_in.rs | 174 |
| H | ? | is_in.rs | 177 |
| H | ? | expr_expansion.rs | 32 |
| H | ? | expr_expansion.rs | 186 |
| H | ? | expr_expansion.rs | 267 |
| H | ? | expr_expansion.rs | 275 |
| H | ? | expr_expansion.rs | 289 |
| H | ? | expr_expansion.rs | 303 |
| H | ? | expr_expansion.rs | 306 |
| H | ? | expr_expansion.rs | 312 |
| H | ? | expr_expansion.rs | 314 |
| H | ? | expr_expansion.rs | 331 |
| H | ? | expr_expansion.rs | 359 |
| H | ? | expr_expansion.rs | 365 |
| H | ? | expr_expansion.rs | 366 |
| H | ? | expr_expansion.rs | 378 |
| H | ? | expr_expansion.rs | 387 |
| H | ? | expr_expansion.rs | 389 |
| H | ? | expr_expansion.rs | 569 |
| H | ? | expr_expansion.rs | 570 |
| H | ? | expr_expansion.rs | 571 |
| H | ? | expr_expansion.rs | 578 |
| H | ? | expr_expansion.rs | 579 |
| H | ? | expr_expansion.rs | 580 |
| H | ? | expr_expansion.rs | 603 |
| H | ? | expr_expansion.rs | 609 |
| H | ? | expr_expansion.rs | 618 |
| H | ? | expr_expansion.rs | 656 |
| H | ? | expr_expansion.rs | 669 |
| H | ? | expr_expansion.rs | 691 |
| H | ? | expr_expansion.rs | 697 |
| H | ? | expr_expansion.rs | 698 |
| H | ? | expr_expansion.rs | 711 |
| H | ? | expr_expansion.rs | 717 |
| H | ? | expr_expansion.rs | 718 |
| H | ? | expr_expansion.rs | 733 |
| H | ? | expr_expansion.rs | 736 |
| H | ? | expr_expansion.rs | 745 |
| H | ? | expr_expansion.rs | 749 |
| H | ? | expr_expansion.rs | 761 |
| H | ? | expr_expansion.rs | 762 |
| H | ? | expr_expansion.rs | 763 |
| H | ? | expr_expansion.rs | 770 |
| H | ? | expr_expansion.rs | 771 |
| H | ? | expr_expansion.rs | 772 |
| H | ? | expr_expansion.rs | 793 |
| H | ? | expr_expansion.rs | 812 |
| H | ? | expr_expansion.rs | 823 |
| H | ? | expr_expansion.rs | 825 |
| H | ? | expr_expansion.rs | 830 |
| H | ? | expr_expansion.rs | 854 |
| H | ? | expr_expansion.rs | 855 |
| H | ? | expr_expansion.rs | 868 |
| H | ? | expr_expansion.rs | 890 |
| H | ? | expr_expansion.rs | 891 |
| H | ? | expr_expansion.rs | 919 |
| H | ? | mod.rs | 135 |
| H | ? | mod.rs | 136 |
| H | ? | mod.rs | 137 |
| H | ? | mod.rs | 138 |
| H | ? | mod.rs | 139 |
| H | ? | mod.rs | 163 |
| H | ? | mod.rs | 174 |
| H | ? | mod.rs | 365 |
| H | ? | mod.rs | 369 |
| H | ? | mod.rs | 557 |
| H | ? | mod.rs | 573 |
| H | ? | mod.rs | 773 |
| H | ? | mod.rs | 775 |
| H | ? | mod.rs | 778 |
| H | ? | mod.rs | 783 |
| H | ? | mod.rs | 803 |
| H | ? | mod.rs | 858 |
| H | ? | mod.rs | 873 |
| H | ? | mod.rs | 877 |
| H | ? | mod.rs | 927 |
| H | ? | mod.rs | 934 |
| H | ? | mod.rs | 940 |
| H | ? | mod.rs | 987 |
| H | ? | mod.rs | 991 |
| H | ? | mod.rs | 1013 |
| H | ? | mod.rs | 1021 |
| H | ? | mod.rs | 1031 |
| H | ? | mod.rs | 1059 |
| H | ? | mod.rs | 1065 |
| H | ? | mod.rs | 1096 |
| H | ? | mod.rs | 1098 |
| H | ? | mod.rs | 1112 |
| H | ? | mod.rs | 1200 |
| H | ? | mod.rs | 1201 |
| H | ? | mod.rs | 1202 |
| H | ? | mod.rs | 1235 |
| H | ? | mod.rs | 1240 |
| H | ? | mod.rs | 1245 |
| H | ? | mod.rs | 1255 |
| H | ? | mod.rs | 1264 |
| H | ? | mod.rs | 1269 |
| H | ? | mod.rs | 1274 |
| H | ? | mod.rs | 1283 |
| H | ? | mod.rs | 1337 |
| H | ? | mod.rs | 1338 |
| H | ? | mod.rs | 1342 |
| H | ? | mod.rs | 1343 |
| H | ? | mod.rs | 1396 |
| H | ? | mod.rs | 1427 |
| H | ? | mod.rs | 1676 |
| H | ? | mod.rs | 1687 |
| H | ? | mod.rs | 1729 |
| H | ? | mod.rs | 1731 |
| H | ? | mod.rs | 1732 |
| H | ? | mod.rs | 1734 |
| H | ? | mod.rs | 1736 |
| H | ? | mod.rs | 1737 |
| H | ? | mod.rs | 1738 |
| H | ? | mod.rs | 1742 |
| H | ? | mod.rs | 1743 |
| H | ? | mod.rs | 1745 |
| H | ? | mod.rs | 1773 |
| H | ? | mod.rs | 1788 |
| H | ? | mod.rs | 1800 |
| H | ? | mod.rs | 1818 |
| H | ? | scans.rs | 80 |
| H | ? | scans.rs | 118 |
| H | ? | scans.rs | 134 |
| H | ? | scans.rs | 135 |
| H | ? | scans.rs | 152 |
| H | ? | scans.rs | 167 |
| H | ? | scans.rs | 223 |
| H | ? | scans.rs | 234 |
| H | ? | scans.rs | 235 |
| H | ? | scans.rs | 239 |
| H | ? | scans.rs | 269 |
| H | ? | scans.rs | 273 |
| H | ? | scans.rs | 282 |
| H | ? | scans.rs | 436 |
| H | ? | scans.rs | 444 |
| H | ? | scans.rs | 513 |
| H | ? | scans.rs | 538 |
| H | ? | scans.rs | 575 |
| H | ? | scans.rs | 633 |
| H | ? | scans.rs | 640 |
| H | ? | scans.rs | 679 |
| H | ? | scans.rs | 684 |
| H | ? | scans.rs | 706 |
| H | ? | scans.rs | 716 |
| H | ? | scans.rs | 743 |
| H | ? | scans.rs | 828 |
| H | ? | scans.rs | 831 |
| H | ? | scans.rs | 862 |
| H | ? | scans.rs | 863 |
| H | ? | scans.rs | 867 |
| H | ? | scans.rs | 892 |
| H | ? | scans.rs | 899 |
| H | ? | scans.rs | 912 |
| H | ? | scans.rs | 926 |
| H | ? | scans.rs | 945 |
| H | ? | scans.rs | 965 |
| H | ? | scans.rs | 976 |
| H | ? | scans.rs | 1044 |
| H | ? | scans.rs | 1114 |
| H | ? | scans.rs | 1209 |
| H | ? | scans.rs | 1211 |
| H | ? | scans.rs | 1246 |
| H | ? | scans.rs | 1248 |
| H | ? | scans.rs | 1297 |
| H | ? | scans.rs | 1300 |
| H | ? | scans.rs | 1319 |
| H | ? | scans.rs | 1323 |
| H | ? | scans.rs | 1324 |
| H | ? | scans.rs | 1331 |
| H | ? | scans.rs | 1335 |
| H | ? | scans.rs | 1336 |
| H | ? | scans.rs | 1369 |
| H | ? | scans.rs | 1374 |
| H | ? | scans.rs | 1389 |
| H | ? | scans.rs | 1390 |
| H | ? | scans.rs | 1400 |
| H | ? | scans.rs | 1411 |
| H | ? | scans.rs | 1412 |
| H | ? | scans.rs | 1413 |
| H | ? | scans.rs | 1414 |
| H | ? | scans.rs | 1423 |
| H | ? | scans.rs | 1424 |
| H | ? | scans.rs | 1425 |
| H | ? | scans.rs | 1435 |
| H | ? | scans.rs | 1454 |
| H | ? | scans.rs | 1462 |
| H | ? | expr_to_ir.rs | 21 |
| H | ? | expr_to_ir.rs | 26 |
| H | ? | expr_to_ir.rs | 44 |
| H | ? | expr_to_ir.rs | 164 |
| H | ? | expr_to_ir.rs | 370 |
| H | ? | expr_to_ir.rs | 372 |
| H | ? | expr_to_ir.rs | 487 |
| H | ? | expr_to_ir.rs | 488 |
| H | ? | expr_to_ir.rs | 490 |
| H | ? | expr_to_ir.rs | 538 |
| H | ? | expr_to_ir.rs | 539 |
| H | ? | expr_to_ir.rs | 546 |
| H | ? | expr_to_ir.rs | 553 |
| H | ? | expr_to_ir.rs | 554 |
| H | ? | expr_to_ir.rs | 571 |
| H | ? | expr_to_ir.rs | 608 |
| H | ? | concat.rs | 24 |
| H | ? | concat.rs | 45 |
| H | ? | concat.rs | 46 |
| H | ? | concat.rs | 76 |
| H | ? | concat.rs | 92 |
| H | ? | functions.rs | 493 |
| H | ? | functions.rs | 504 |
| H | ? | functions.rs | 523 |
| H | ? | functions.rs | 534 |
| H | ? | functions.rs | 780 |
| H | ? | functions.rs | 781 |
| H | ? | functions.rs | 788 |
| H | ? | functions.rs | 791 |
| H | ? | functions.rs | 1103 |
| H | ? | functions.rs | 1112 |
| H | ? | functions.rs | 1143 |
| H | ? | functions.rs | 1165 |
| H | ? | join.rs | 183 |
| H | ? | join.rs | 188 |
| H | ? | join.rs | 197 |
| H | ? | join.rs | 202 |
| H | ? | join.rs | 208 |
| H | ? | join.rs | 210 |
| H | ? | join.rs | 228 |
| H | ? | join.rs | 230 |
| H | ? | join.rs | 280 |
| H | ? | join.rs | 290 |
| H | ? | join.rs | 291 |
| H | ? | join.rs | 412 |
| H | ? | join.rs | 426 |
| H | ? | join.rs | 643 |
| H | ? | format.rs | 883 |
| H | ? | unoptimized.rs | 50 |
| H | ? | unoptimized.rs | 62 |
| H | ? | unoptimized.rs | 67 |
| H | ? | unoptimized.rs | 75 |
| H | ? | unoptimized.rs | 122 |
| H | ? | unoptimized.rs | 134 |
| H | ? | schema.rs | 144 |
| H | ? | schema.rs | 153 |
| H | ? | schema.rs | 155 |
| H | ? | schema.rs | 171 |
| H | ? | schema.rs | 176 |
| H | ? | schema.rs | 184 |
| H | ? | schema.rs | 204 |
| H | ? | mod.rs | 329 |
| H | ? | mod.rs | 33 |
| H | ? | skip_batches.rs | 50 |
| H | ? | skip_batches.rs | 81 |
| H | ? | skip_batches.rs | 91 |
| H | ? | skip_batches.rs | 124 |
| H | ? | skip_batches.rs | 125 |
| H | ? | skip_batches.rs | 129 |
| H | ? | skip_batches.rs | 546 |
| H | ? | skip_batches.rs | 751 |
| H | ? | column_expr.rs | 88 |
| H | ? | column_expr.rs | 204 |
| H | ? | column_expr.rs | 205 |
| H | ? | column_expr.rs | 231 |
| H | ? | column_expr.rs | 234 |
| H | ? | column_expr.rs | 266 |
| H | ? | column_expr.rs | 378 |
| H | ? | column_expr.rs | 404 |
| H | ? | column_expr.rs | 429 |
| H | ? | strings.rs | 163 |
| H | ? | strings.rs | 165 |
| H | ? | strings.rs | 169 |
| H | ? | strings.rs | 184 |
| H | ? | strings.rs | 196 |
| H | ? | cat.rs | 36 |
| H | ? | binary.rs | 38 |
| H | ? | datetime.rs | 112 |
| H | ? | datetime.rs | 117 |
| H | ? | datetime.rs | 150 |
| H | ? | datetime.rs | 153 |
| H | ? | array.rs | 59 |
| H | ? | array.rs | 103 |
| H | ? | array.rs | 145 |
| H | ? | array.rs | 165 |
| H | ? | array.rs | 239 |
| H | ? | plugin.rs | 18 |
| H | ? | plugin.rs | 54 |
| H | ? | cum.rs | 11 |
| H | ? | cum.rs | 26 |
| H | ? | list.rs | 114 |
| H | ? | list.rs | 152 |
| H | ? | list.rs | 210 |
| H | ? | struct_.rs | 28 |
| H | ? | struct_.rs | 38 |
| H | ? | struct_.rs | 48 |
| H | ? | struct_.rs | 58 |
| H | ? | struct_.rs | 71 |
| H | ? | struct_.rs | 86 |
| H | ? | struct_.rs | 87 |
| H | ? | extension.rs | 14 |
| H | ? | extension.rs | 16 |
| H | ? | extension.rs | 17 |
| H | ? | range.rs | 84 |
| H | ? | range.rs | 101 |
| H | ? | range.rs | 102 |
| H | ? | boolean.rs | 65 |
| H | ? | bitwise.rs | 45 |
| H | ? | schema.rs | 96 |
| H | ? | schema.rs | 98 |
| H | ? | schema.rs | 175 |
| H | ? | schema.rs | 179 |
| H | ? | schema.rs | 200 |
| H | ? | schema.rs | 201 |
| H | ? | schema.rs | 258 |
| H | ? | schema.rs | 263 |
| H | ? | schema.rs | 264 |
| H | ? | schema.rs | 299 |
| H | ? | schema.rs | 317 |
| H | ? | schema.rs | 320 |
| H | ? | schema.rs | 352 |
| H | ? | schema.rs | 371 |
| H | ? | schema.rs | 375 |
| H | ? | schema.rs | 383 |
| H | ? | schema.rs | 397 |
| H | ? | schema.rs | 404 |
| H | ? | schema.rs | 443 |
| H | ? | schema.rs | 447 |
| H | ? | schema.rs | 466 |
| H | ? | schema.rs | 500 |
| H | ? | schema.rs | 505 |
| H | ? | schema.rs | 511 |
| H | ? | schema.rs | 532 |
| H | ? | schema.rs | 557 |
| H | ? | schema.rs | 559 |
| H | ? | schema.rs | 561 |
| H | ? | schema.rs | 566 |
| H | ? | schema.rs | 603 |
| H | ? | schema.rs | 619 |
| H | ? | schema.rs | 627 |
| H | ? | schema.rs | 641 |
| H | ? | schema.rs | 648 |
| H | ? | schema.rs | 673 |
| H | ? | schema.rs | 689 |
| H | ? | schema.rs | 695 |
| H | ? | schema.rs | 723 |
| H | ? | schema.rs | 728 |
| H | ? | schema.rs | 746 |
| H | ? | schema.rs | 776 |
| H | ? | schema.rs | 789 |
| H | ? | schema.rs | 811 |
| H | ? | schema.rs | 837 |
| H | ? | schema.rs | 844 |
| H | ? | filter_constraint.rs | 240 |
| H | ? | filter_constraint.rs | 243 |
| H | ? | filter_constraint.rs | 246 |
| H | ? | filter_constraint.rs | 250 |
| H | ? | filter_constraint.rs | 499 |
| H | ? | filter_constraint.rs | 655 |
| H | ? | filter_constraint.rs | 661 |
| H | ? | filter_constraint.rs | 672 |
| H | ? | filter_constraint.rs | 676 |
| H | ? | filter_constraint.rs | 680 |
| H | ? | filter_constraint.rs | 704 |
| H | ? | filter_constraint.rs | 888 |
| H | ? | filter_constraint.rs | 901 |
| H | ? | filter_constraint.rs | 917 |
| H | ? | filter_constraint.rs | 919 |
| H | ? | filter_constraint.rs | 950 |
| H | ? | filter_constraint.rs | 996 |
| H | ? | schema.rs | 90 |
| H | ? | schema.rs | 92 |
| H | ? | schema.rs | 118 |
| H | ? | schema.rs | 146 |
| H | ? | schema.rs | 227 |
| H | ? | schema.rs | 259 |
| H | ? | schema.rs | 270 |
| H | ? | schema.rs | 286 |
| H | ? | schema.rs | 298 |
| H | ? | schema.rs | 310 |
| H | ? | schema.rs | 311 |
| H | ? | schema.rs | 328 |
| H | ? | schema.rs | 329 |
| H | ? | schema.rs | 349 |
| H | ? | schema.rs | 352 |
| H | ? | schema.rs | 456 |
| H | ? | schema.rs | 458 |
| H | ? | schema.rs | 468 |
| H | ? | schema.rs | 470 |
| H | ? | schema.rs | 472 |
| H | ? | schema.rs | 473 |
| H | ? | schema.rs | 483 |
| H | ? | schema.rs | 788 |
| H | ? | schema.rs | 804 |
| H | ? | schema.rs | 875 |
| H | ? | schema.rs | 890 |
| H | ? | schema.rs | 904 |
| H | ? | or_factoring.rs | 198 |
| H | ? | builder.rs | 563 |
| H | ? | expr_ir.rs | 113 |
| H | ? | expr_ir.rs | 140 |
| H | ? | expr_ir.rs | 145 |
| H | ? | expr_ir.rs | 150 |
| H | ? | expr_ir.rs | 162 |
| H | ? | expr_ir.rs | 169 |
| H | ? | expr_ir.rs | 177 |
| H | ? | expr_ir.rs | 179 |
| H | ? | expr_ir.rs | 221 |
| H | ? | expr_ir.rs | 246 |
| H | ? | expr_ir.rs | 306 |
| H | ? | utils.rs | 59 |
| H | ? | utils.rs | 136 |
| H | ? | utils.rs | 137 |
| H | ? | utils.rs | 147 |
| H | ? | utils.rs | 151 |
| H | ? | utils.rs | 162 |
| H | ? | utils.rs | 197 |
| H | ? | utils.rs | 301 |
| H | ? | utils.rs | 318 |
| H | ? | utils.rs | 347 |
| H | ? | tree_traversal.rs | 33 |
| H | ? | tree_traversal.rs | 101 |
| H | ? | tree_traversal.rs | 114 |
| H | ? | tree_traversal.rs | 125 |
| H | ? | tree_traversal.rs | 126 |
| H | ? | tree_traversal.rs | 150 |
| H | ? | tree_traversal.rs | 172 |
| H | ? | csv.rs | 184 |
| H | ? | csv.rs | 209 |
| H | ? | csv.rs | 308 |
| H | ? | csv.rs | 343 |
| H | ? | csv.rs | 353 |
| H | ? | file_list_reader.rs | 28 |
| H | ? | file_list_reader.rs | 33 |
| H | ? | file_list_reader.rs | 54 |
| H | ? | anonymous_scan.rs | 71 |
| H | ? | dot.rs | 9 |
| H | ? | dot.rs | 11 |
| H | ? | dot.rs | 20 |
| H | ? | functions.rs | 25 |
| H | ? | functions.rs | 58 |
| H | ? | functions.rs | 64 |
| H | ? | mod.rs | 219 |
| H | ? | mod.rs | 224 |
| H | ? | mod.rs | 231 |
| H | ? | mod.rs | 238 |
| H | ? | mod.rs | 646 |
| H | ? | mod.rs | 680 |
| H | ? | mod.rs | 767 |
| H | ? | mod.rs | 1056 |
| H | ? | mod.rs | 1106 |
| H | ? | mod.rs | 1152 |
| H | ? | mod.rs | 1174 |
| H | ? | mod.rs | 1563 |
| H | ? | mod.rs | 1926 |
| H | ? | mod.rs | 2331 |
| H | ? | mod.rs | 2332 |
| H | ? | mod.rs | 2357 |
| H | ? | mod.rs | 2358 |
| H | ? | mod.rs | 2361 |
| H | ? | mod.rs | 2362 |
| H | ? | mod.rs | 2365 |
| H | ? | mod.rs | 2366 |
| H | ? | mod.rs | 2369 |
| H | ? | mod.rs | 2370 |
| H | ? | err.rs | 9 |
| H | ? | cached_arenas.rs | 23 |
| H | ? | cached_arenas.rs | 33 |
| H | ? | cached_arenas.rs | 54 |
| H | ? | cached_arenas.rs | 64 |
| H | ? | cached_arenas.rs | 89 |
| H | ? | cached_arenas.rs | 103 |
| H | ? | cached_arenas.rs | 116 |
| H | ? | buffer.rs | 53 |
| H | ? | buffer.rs | 248 |
| H | ? | buffer.rs | 261 |
| H | ? | buffer.rs | 383 |
| H | ? | storage.rs | 187 |
| H | ? | storage.rs | 209 |
| H | ? | series.rs | 468 |
| H | ? | series.rs | 476 |
| H | ? | series.rs | 489 |
| H | ? | series.rs | 494 |
| H | ? | series.rs | 509 |
| H | ? | series.rs | 527 |
| H | ? | series.rs | 531 |
| H | ? | utils.rs | 115 |
| H | ? | utils.rs | 123 |
| H | ? | utils.rs | 135 |
| H | ? | utils.rs | 320 |
| H | ? | utils.rs | 464 |
| H | ? | utils.rs | 465 |
| H | ? | utils.rs | 868 |
| H | ? | utils.rs | 869 |
| H | ? | utils.rs | 872 |
| H | ? | mod.rs | 53 |
| H | ? | mod.rs | 105 |
| H | ? | mod.rs | 109 |
| H | ? | mod.rs | 242 |
| H | ? | mod.rs | 246 |
| H | ? | file.rs | 237 |
| H | ? | file.rs | 239 |
| H | ? | file.rs | 241 |
| H | ? | stream.rs | 174 |
| H | ? | stream.rs | 176 |
| H | ? | stream.rs | 178 |
| H | ? | page.rs | 169 |
| H | ? | page.rs | 172 |
| H | ? | statistics.rs | 23 |
| H | ? | statistics.rs | 24 |
| H | ? | statistics.rs | 68 |
| H | ? | statistics.rs | 81 |
| H | ? | statistics.rs | 94 |
| H | ? | statistics.rs | 119 |
| H | ? | statistics.rs | 316 |
| H | ? | statistics.rs | 320 |
| H | ? | from_thrift.rs | 90 |
| H | ? | from_thrift.rs | 129 |
| H | ? | row_metadata.rs | 24 |
| H | ? | row_metadata.rs | 94 |
| H | ? | schema_descriptor.rs | 68 |
| H | ? | schema_descriptor.rs | 163 |
| H | ? | schema_descriptor.rs | 176 |
| H | ? | file_metadata_serde.rs | 103 |
| H | ? | column_chunk_metadata.rs | 74 |
| H | ? | file_metadata.rs | 140 |
| H | ? | file_metadata.rs | 170 |
| H | ? | file_metadata_thrift.rs | 136 |
| H | ? | binary.rs | 24 |
| H | ? | binary.rs | 25 |
| H | ? | binary.rs | 33 |
| H | ? | binary.rs | 34 |
| H | ? | fixed_len_binary.rs | 40 |
| H | ? | fixed_len_binary.rs | 44 |
| H | ? | fixed_len_binary.rs | 55 |
| H | ? | fixed_len_binary.rs | 56 |
| H | ? | encoder.rs | 13 |
| H | ? | mod.rs | 45 |
| H | ? | mod.rs | 58 |
| H | ? | mod.rs | 79 |
| H | ? | mod.rs | 95 |
| H | ? | mod.rs | 108 |
| H | ? | mod.rs | 122 |
| H | ? | mod.rs | 143 |
| H | ? | mod.rs | 16 |
| H | ? | encoder.rs | 13 |
| H | ? | stream.rs | 122 |
| H | ? | stream.rs | 134 |
| H | ? | reader.rs | 54 |
| H | ? | reader.rs | 158 |
| H | ? | reader.rs | 231 |
| H | ? | reader.rs | 304 |
| H | ? | reader.rs | 328 |
| H | ? | mod.rs | 86 |
| H | ? | mod.rs | 353 |
| H | ? | mod.rs | 372 |
| H | ? | mod.rs | 373 |
| H | ? | mod.rs | 378 |
| H | ? | mod.rs | 507 |
| H | ? | mod.rs | 510 |
| H | ? | mod.rs | 586 |
| H | ? | mod.rs | 613 |
| H | ? | mod.rs | 626 |
| H | ? | mod.rs | 678 |
| H | ? | mod.rs | 707 |
| H | ? | mod.rs | 773 |
| H | ? | mod.rs | 800 |
| H | ? | mod.rs | 810 |
| H | ? | mod.rs | 820 |
| H | ? | mod.rs | 830 |
| H | ? | mod.rs | 838 |
| H | ? | mod.rs | 933 |
| H | ? | mod.rs | 936 |
| H | ? | mod.rs | 989 |
| H | ? | mod.rs | 1050 |
| H | ? | mod.rs | 1079 |
| H | ? | mod.rs | 1110 |
| H | ? | mod.rs | 1120 |
| H | ? | mod.rs | 1136 |
| H | ? | mod.rs | 1146 |
| H | ? | row_group.rs | 123 |
| H | ? | basic.rs | 92 |
| H | ? | nested.rs | 29 |
| H | ? | basic.rs | 86 |
| H | ? | nested.rs | 33 |
| H | ? | dictionary.rs | 209 |
| H | ? | dictionary.rs | 252 |
| H | ? | dictionary.rs | 304 |
| H | ? | dictionary.rs | 314 |
| H | ? | dictionary.rs | 364 |
| H | ? | dictionary.rs | 369 |
| H | ? | dictionary.rs | 370 |
| H | ? | dictionary.rs | 377 |
| H | ? | dictionary.rs | 423 |
| H | ? | dictionary.rs | 440 |
| H | ? | dictionary.rs | 501 |
| H | ? | dictionary.rs | 524 |
| H | ? | dictionary.rs | 548 |
| H | ? | dictionary.rs | 567 |
| H | ? | dictionary.rs | 585 |
| H | ? | basic.rs | 174 |
| H | ? | nested.rs | 37 |
| H | ? | mod.rs | 292 |
| H | ? | mod.rs | 330 |
| H | ? | schema.rs | 70 |
| H | ? | schema.rs | 71 |
| H | ? | schema.rs | 98 |
| H | ? | schema.rs | 255 |
| H | ? | schema.rs | 319 |
| H | ? | pages.rs | 180 |
| H | ? | pages.rs | 224 |
| H | ? | pages.rs | 247 |
| H | ? | pages.rs | 270 |
| H | ? | pages.rs | 357 |
| H | ? | pages.rs | 379 |
| H | ? | pages.rs | 421 |
| H | ? | pages.rs | 581 |
| H | ? | pages.rs | 623 |
| H | ? | pages.rs | 688 |
| H | ? | pages.rs | 693 |
| H | ? | pages.rs | 694 |
| H | ? | pages.rs | 700 |
| H | ? | pages.rs | 744 |
| H | ? | pages.rs | 793 |
| H | ? | pages.rs | 800 |
| H | ? | pages.rs | 893 |
| H | ? | utils.rs | 108 |
| H | ? | simple.rs | 67 |
| H | ? | simple.rs | 190 |
| H | ? | simple.rs | 221 |
| H | ? | simple.rs | 268 |
| H | ? | simple.rs | 295 |
| H | ? | simple.rs | 348 |
| H | ? | simple.rs | 386 |
| H | ? | simple.rs | 434 |
| H | ? | simple.rs | 466 |
| H | ? | mod.rs | 528 |
| H | ? | mod.rs | 608 |
| H | ? | mod.rs | 652 |
| H | ? | mod.rs | 694 |
| H | ? | mod.rs | 826 |
| H | ? | mod.rs | 827 |
| H | ? | mod.rs | 183 |
| H | ? | mod.rs | 214 |
| H | ? | dictionary.rs | 22 |
| H | ? | mod.rs | 534 |
| H | ? | mod.rs | 547 |
| H | ? | mod.rs | 548 |
| H | ? | integer.rs | 208 |
| H | ? | integer.rs | 352 |
| H | ? | float.rs | 179 |
| H | ? | float.rs | 228 |
| H | ? | mod.rs | 651 |
| H | ? | mod.rs | 652 |
| H | ? | mod.rs | 686 |
| H | ? | filter.rs | 68 |
| H | ? | categorical.rs | 93 |
| H | ? | categorical.rs | 141 |
| H | ? | optional_masked_dense.rs | 256 |
| H | ? | optional_masked_dense.rs | 258 |
| H | ? | optional_masked_dense.rs | 259 |
| H | ? | mod.rs | 169 |
| H | ? | mod.rs | 196 |
| H | ? | mod.rs | 198 |
| H | ? | mod.rs | 242 |
| H | ? | mod.rs | 272 |
| H | ? | required_masked_dense.rs | 209 |
| H | ? | optional.rs | 60 |
| H | ? | nested.rs | 35 |
| H | ? | nested.rs | 41 |
| H | ? | nested.rs | 50 |
| H | ? | nested.rs | 56 |
| H | ? | nested.rs | 87 |
| H | ? | nested.rs | 89 |
| H | ? | nested.rs | 94 |
| H | ? | nested.rs | 104 |
| H | ? | nested.rs | 111 |
| H | ? | nested.rs | 126 |
| H | ? | nested.rs | 141 |
| H | ? | nested.rs | 147 |
| H | ? | nested.rs | 193 |
| H | ? | nested.rs | 201 |
| H | ? | nested.rs | 209 |
| H | ? | nested.rs | 226 |
| H | ? | nested.rs | 234 |
| H | ? | convert.rs | 29 |
| H | ? | convert.rs | 233 |
| H | ? | convert.rs | 291 |
| H | ? | convert.rs | 312 |
| H | ? | convert.rs | 347 |
| H | ? | convert.rs | 398 |
| H | ? | convert.rs | 403 |
| H | ? | convert.rs | 1226 |
| H | ? | convert.rs | 1231 |
| H | ? | convert.rs | 1240 |
| H | ? | statistics.rs | 135 |
| H | ? | statistics.rs | 266 |
| H | ? | statistics.rs | 576 |
| H | ? | statistics.rs | 604 |
| H | ? | ewm.rs | 27 |
| H | ? | ewm.rs | 33 |
| H | ? | ewm.rs | 39 |
| H | ? | ewm.rs | 82 |
| H | ? | ewm.rs | 94 |
| H | ? | ewm.rs | 106 |
| H | ? | ewm.rs | 128 |
| H | ? | ewm.rs | 140 |
| H | ? | ewm.rs | 152 |
| H | ? | cum_agg.rs | 75 |
| H | ? | cum_agg.rs | 116 |
| H | ? | cum_agg.rs | 122 |
| H | ? | cum_agg.rs | 137 |
| H | ? | cum_agg.rs | 145 |
| H | ? | cum_agg.rs | 158 |
| H | ? | cum_agg.rs | 164 |
| H | ? | cum_agg.rs | 179 |
| H | ? | cum_agg.rs | 187 |
| H | ? | cum_agg.rs | 329 |
| H | ? | cum_agg.rs | 364 |
| H | ? | cum_agg.rs | 402 |
| H | ? | cum_agg.rs | 435 |
| H | ? | clip.rs | 68 |
| H | ? | clip.rs | 102 |
| H | ? | clip.rs | 136 |
| H | ? | clip.rs | 159 |
| H | ? | clip.rs | 202 |
| H | ? | duration.rs | 9 |
| H | ? | duration.rs | 20 |
| H | ? | duration.rs | 21 |
| H | ? | duration.rs | 22 |
| H | ? | interpolate.rs | 49 |
| H | ? | interpolate.rs | 103 |
| H | ? | interpolate.rs | 105 |
| H | ? | interpolate.rs | 112 |
| H | ? | interpolate.rs | 113 |
| H | ? | interpolate.rs | 115 |
| H | ? | interpolate.rs | 116 |
| H | ? | interpolate.rs | 137 |
| H | ? | interpolate.rs | 138 |
| H | ? | interpolate.rs | 140 |
| H | ? | interpolate.rs | 141 |
| H | ? | interpolate.rs | 184 |
| H | ? | interpolate_by.rs | 96 |
| H | ? | interpolate_by.rs | 158 |
| H | ? | interpolate_by.rs | 160 |
| H | ? | interpolate_by.rs | 178 |
| H | ? | interpolate_by.rs | 260 |
| H | ? | interpolate_by.rs | 262 |
| H | ? | fused.rs | 41 |
| H | ? | fused.rs | 92 |
| H | ? | fused.rs | 142 |
| H | ? | strings.rs | 20 |
| H | ? | is_unique.rs | 40 |
| H | ? | is_unique.rs | 44 |
| H | ? | is_unique.rs | 46 |
| H | ? | is_unique.rs | 84 |
| H | ? | is_unique.rs | 93 |
| H | ? | is_unique.rs | 94 |
| H | ? | is_unique.rs | 95 |
| H | ? | log.rs | 113 |
| H | ? | log.rs | 116 |
| H | ? | is_first_distinct.rs | 24 |
| H | ? | is_first_distinct.rs | 35 |
| H | ? | is_first_distinct.rs | 73 |
| H | ? | is_first_distinct.rs | 89 |
| H | ? | is_first_distinct.rs | 104 |
| H | ? | is_first_distinct.rs | 110 |
| H | ? | is_first_distinct.rs | 112 |
| H | ? | round.rs | 39 |
| H | ? | round.rs | 63 |
| H | ? | round.rs | 88 |
| H | ? | round.rs | 140 |
| H | ? | round.rs | 189 |
| H | ? | round.rs | 284 |
| H | ? | round.rs | 304 |
| H | ? | round.rs | 324 |
| H | ? | round.rs | 344 |
| H | ? | unique.rs | 34 |
| H | ? | unique.rs | 36 |
| H | ? | unique.rs | 126 |
| H | ? | ewm_by.rs | 223 |
| H | ? | is_in.rs | 46 |
| H | ? | is_in.rs | 132 |
| H | ? | is_in.rs | 219 |
| H | ? | is_in.rs | 238 |
| H | ? | is_in.rs | 256 |
| H | ? | is_in.rs | 318 |
| H | ? | is_in.rs | 336 |
| H | ? | is_in.rs | 383 |
| H | ? | is_in.rs | 392 |
| H | ? | is_in.rs | 410 |
| H | ? | is_in.rs | 455 |
| H | ? | is_in.rs | 459 |
| H | ? | is_in.rs | 482 |
| H | ? | is_in.rs | 490 |
| H | ? | is_in.rs | 504 |
| H | ? | is_in.rs | 512 |
| H | ? | is_in.rs | 525 |
| H | ? | is_in.rs | 579 |
| H | ? | is_in.rs | 585 |
| H | ? | is_in.rs | 591 |
| H | ? | is_in.rs | 609 |
| H | ? | is_in.rs | 615 |
| H | ? | diff.rs | 10 |
| H | ? | abs.rs | 35 |
| H | ? | pct_change.rs | 23 |
| H | ? | floor_divide.rs | 16 |
| H | ? | floor_divide.rs | 17 |
| H | ? | floor_divide.rs | 18 |
| H | ? | rank.rs | 70 |
| H | ? | rank.rs | 76 |
| H | ? | rank.rs | 77 |
| H | ? | rank.rs | 82 |
| H | ? | rank.rs | 83 |
| H | ? | rank.rs | 91 |
| H | ? | rank.rs | 92 |
| H | ? | rank.rs | 116 |
| H | ? | rank.rs | 140 |
| H | ? | rank.rs | 153 |
| H | ? | rank.rs | 163 |
| H | ? | rank.rs | 173 |
| H | ? | rank.rs | 183 |
| H | ? | index_of.rs | 137 |
| H | ? | replace.rs | 52 |
| H | ? | replace.rs | 165 |
| H | ? | replace.rs | 253 |
| H | ? | replace.rs | 276 |
| H | ? | replace.rs | 295 |
| H | ? | replace.rs | 321 |
| H | ? | rle.rs | 81 |
| H | ? | rle.rs | 165 |
| H | ? | rle.rs | 171 |
| H | ? | rle.rs | 189 |
| H | ? | search_sorted.rs | 39 |
| H | ? | search_sorted.rs | 61 |
| H | ? | search_sorted.rs | 78 |
| H | ? | search_sorted.rs | 84 |
| H | ? | search_sorted.rs | 94 |
| H | ? | search_sorted.rs | 99 |
| H | ? | search_sorted.rs | 106 |
| H | ? | search_sorted.rs | 112 |
| H | ? | is_last_distinct.rs | 15 |
| H | ? | is_last_distinct.rs | 17 |
| H | ? | is_last_distinct.rs | 110 |
| H | ? | is_last_distinct.rs | 122 |
| H | ? | is_last_distinct.rs | 139 |
| H | ? | is_last_distinct.rs | 156 |
| H | ? | is_last_distinct.rs | 172 |
| H | ? | horizontal.rs | 142 |
| H | ? | horizontal.rs | 168 |
| H | ? | horizontal.rs | 224 |
| H | ? | horizontal.rs | 236 |
| H | ? | horizontal.rs | 243 |
| H | ? | horizontal.rs | 247 |
| H | ? | horizontal.rs | 294 |
| H | ? | horizontal.rs | 329 |
| H | ? | horizontal.rs | 352 |
| H | ? | concat_arr.rs | 65 |
| H | ? | concat_arr.rs | 71 |
| H | ? | concat_arr.rs | 97 |
| H | ? | concat_arr.rs | 112 |
| H | ? | concat_arr.rs | 118 |
| H | ? | concat_arr.rs | 119 |
| H | ? | concat_arr.rs | 134 |
| H | ? | concat_arr.rs | 140 |
| H | ? | concat_arr.rs | 141 |
| H | ? | business.rs | 54 |
| H | ? | business.rs | 213 |
| H | ? | business.rs | 218 |
| H | ? | business.rs | 391 |
| H | ? | eager.rs | 12 |
| H | ? | eager.rs | 31 |
| H | ? | eager.rs | 49 |
| H | ? | various.rs | 32 |
| H | ? | various.rs | 34 |
| H | ? | various.rs | 65 |
| H | ? | various.rs | 119 |
| H | ? | cut.rs | 25 |
| H | ? | cut.rs | 30 |
| H | ? | cut.rs | 96 |
| H | ? | cut.rs | 204 |
| H | ? | cut.rs | 210 |
| H | ? | cut.rs | 265 |
| H | ? | cut.rs | 274 |
| H | ? | hist.rs | 227 |
| H | ? | hist.rs | 229 |
| H | ? | top_k.rs | 27 |
| H | ? | top_k.rs | 71 |
| H | ? | top_k.rs | 106 |
| H | ? | top_k.rs | 113 |
| H | ? | top_k.rs | 170 |
| H | ? | top_k.rs | 255 |
| H | ? | top_k.rs | 259 |
| H | ? | top_k.rs | 278 |
| H | ? | dispersion.rs | 14 |
| H | ? | dispersion.rs | 20 |
| H | ? | dispersion.rs | 27 |
| H | ? | dispersion.rs | 33 |
| H | ? | dispersion.rs | 37 |
| H | ? | dispersion.rs | 49 |
| H | ? | dispersion.rs | 55 |
| H | ? | dispersion.rs | 62 |
| H | ? | dispersion.rs | 68 |
| H | ? | dispersion.rs | 72 |
| H | ? | dispersion.rs | 84 |
| H | ? | dispersion.rs | 90 |
| H | ? | dispersion.rs | 97 |
| H | ? | dispersion.rs | 109 |
| H | ? | dispersion.rs | 121 |
| H | ? | dispersion.rs | 127 |
| H | ? | dispersion.rs | 134 |
| H | ? | dispersion.rs | 148 |
| H | ? | dispersion.rs | 154 |
| H | ? | dispersion.rs | 158 |
| H | ? | min_max.rs | 30 |
| H | ? | namespace.rs | 31 |
| H | ? | namespace.rs | 137 |
| H | ? | namespace.rs | 152 |
| H | ? | namespace.rs | 192 |
| H | ? | sum_mean.rs | 60 |
| H | ? | sum_mean.rs | 173 |
| H | ? | join.rs | 15 |
| H | ? | join.rs | 55 |
| H | ? | join.rs | 98 |
| H | ? | get.rs | 29 |
| H | ? | get.rs | 30 |
| H | ? | get.rs | 34 |
| H | ? | get.rs | 39 |
| H | ? | get.rs | 49 |
| H | ? | get.rs | 54 |
| H | ? | get.rs | 78 |
| H | ? | get.rs | 95 |
| H | ? | get.rs | 102 |
| H | ? | to_struct.rs | 42 |
| H | ? | namespace.rs | 63 |
| H | ? | namespace.rs | 96 |
| H | ? | namespace.rs | 115 |
| H | ? | namespace.rs | 195 |
| H | ? | slice.rs | 114 |
| H | ? | slice.rs | 121 |
| H | ? | slice.rs | 133 |
| H | ? | slice.rs | 176 |
| H | ? | slice.rs | 186 |
| H | ? | slice.rs | 200 |
| H | ? | slice.rs | 210 |
| H | ? | chunked.rs | 202 |
| H | ? | chunked.rs | 227 |
| H | ? | chunked.rs | 232 |
| H | ? | chunked.rs | 302 |
| H | ? | chunked.rs | 327 |
| H | ? | chunked.rs | 332 |
| H | ? | chunked.rs | 400 |
| H | ? | chunked.rs | 432 |
| H | ? | chunked.rs | 450 |
| H | ? | chunked.rs | 511 |
| H | ? | chunked.rs | 601 |
| H | ? | chunked.rs | 631 |
| H | ? | chunked.rs | 718 |
| H | ? | chunked.rs | 824 |
| H | ? | chunked.rs | 839 |
| H | ? | chunked.rs | 885 |
| H | ? | chunked.rs | 1043 |
| H | ? | split.rs | 153 |
| H | ? | split.rs | 168 |
| H | ? | split.rs | 186 |
| H | ? | split.rs | 197 |
| H | ? | split.rs | 203 |
| H | ? | split.rs | 221 |
| H | ? | split.rs | 316 |
| H | ? | split.rs | 332 |
| H | ? | split.rs | 346 |
| H | ? | split.rs | 354 |
| H | ? | split.rs | 371 |
| H | ? | split.rs | 386 |
| H | ? | substring.rs | 241 |
| H | ? | substring.rs | 248 |
| H | ? | substring.rs | 262 |
| H | ? | substring.rs | 303 |
| H | ? | substring.rs | 316 |
| H | ? | substring.rs | 330 |
| H | ? | substring.rs | 342 |
| H | ? | json_path.rs | 17 |
| H | ? | json_path.rs | 57 |
| H | ? | json_path.rs | 105 |
| H | ? | json_path.rs | 238 |
| H | ? | namespace.rs | 61 |
| H | ? | namespace.rs | 190 |
| H | ? | namespace.rs | 193 |
| H | ? | namespace.rs | 244 |
| H | ? | namespace.rs | 248 |
| H | ? | namespace.rs | 342 |
| H | ? | namespace.rs | 367 |
| H | ? | namespace.rs | 391 |
| H | ? | namespace.rs | 434 |
| H | ? | namespace.rs | 478 |
| H | ? | namespace.rs | 568 |
| H | ? | namespace.rs | 637 |
| H | ? | extract.rs | 51 |
| H | ? | extract.rs | 66 |
| H | ? | extract.rs | 69 |
| H | ? | extract.rs | 156 |
| H | ? | extract.rs | 163 |
| H | ? | extract.rs | 170 |
| H | ? | concat.rs | 9 |
| H | ? | concat.rs | 14 |
| H | ? | concat.rs | 19 |
| H | ? | concat.rs | 23 |
| H | ? | concat.rs | 47 |
| H | ? | concat.rs | 69 |
| H | ? | concat.rs | 87 |
| H | ? | find_many.rs | 56 |
| H | ? | find_many.rs | 107 |
| H | ? | find_many.rs | 124 |
| H | ? | find_many.rs | 171 |
| H | ? | find_many.rs | 177 |
| H | ? | find_many.rs | 203 |
| H | ? | find_many.rs | 218 |
| H | ? | find_many.rs | 264 |
| H | ? | find_many.rs | 270 |
| H | ? | find_many.rs | 298 |
| H | ? | find_many.rs | 310 |
| H | ? | escape_regex.rs | 10 |
| H | ? | strip.rs | 127 |
| H | ? | strip.rs | 139 |
| H | ? | normalize.rs | 19 |
| H | ? | gather_skip_nulls.rs | 168 |
| H | ? | replace_time_zone.rs | 18 |
| H | ? | replace_time_zone.rs | 33 |
| H | ? | replace_time_zone.rs | 143 |
| H | ? | repeat_by.rs | 156 |
| H | ? | repeat_by.rs | 164 |
| H | ? | repeat_by.rs | 248 |
| H | ? | peaks.rs | 10 |
| H | ? | dispersion.rs | 16 |
| H | ? | dispersion.rs | 22 |
| H | ? | dispersion.rs | 31 |
| H | ? | dispersion.rs | 38 |
| H | ? | dispersion.rs | 44 |
| H | ? | dispersion.rs | 61 |
| H | ? | dispersion.rs | 67 |
| H | ? | dispersion.rs | 74 |
| H | ? | dispersion.rs | 80 |
| H | ? | dispersion.rs | 97 |
| H | ? | dispersion.rs | 103 |
| H | ? | dispersion.rs | 112 |
| H | ? | min_max.rs | 73 |
| H | ? | min_max.rs | 100 |
| H | ? | min_max.rs | 158 |
| H | ? | min_max.rs | 191 |
| H | ? | min_max.rs | 218 |
| H | ? | sets.rs | 188 |
| H | ? | sets.rs | 189 |
| H | ? | sets.rs | 234 |
| H | ? | sets.rs | 291 |
| H | ? | sets.rs | 292 |
| H | ? | sets.rs | 333 |
| H | ? | sets.rs | 336 |
| H | ? | sets.rs | 397 |
| H | ? | sets.rs | 398 |
| H | ? | namespace.rs | 86 |
| H | ? | namespace.rs | 98 |
| H | ? | namespace.rs | 134 |
| H | ? | namespace.rs | 222 |
| H | ? | namespace.rs | 274 |
| H | ? | namespace.rs | 286 |
| H | ? | namespace.rs | 311 |
| H | ? | namespace.rs | 325 |
| H | ? | namespace.rs | 343 |
| H | ? | namespace.rs | 360 |
| H | ? | namespace.rs | 377 |
| H | ? | namespace.rs | 393 |
| H | ? | namespace.rs | 435 |
| H | ? | namespace.rs | 441 |
| H | ? | namespace.rs | 469 |
| H | ? | namespace.rs | 494 |
| H | ? | namespace.rs | 502 |
| H | ? | namespace.rs | 530 |
| H | ? | namespace.rs | 575 |
| H | ? | namespace.rs | 593 |
| H | ? | namespace.rs | 649 |
| H | ? | namespace.rs | 667 |
| H | ? | namespace.rs | 691 |
| H | ? | namespace.rs | 705 |
| H | ? | namespace.rs | 728 |
| H | ? | namespace.rs | 743 |
| H | ? | namespace.rs | 780 |
| H | ? | sum_mean.rs | 70 |
| H | ? | sum_mean.rs | 154 |
| H | ? | sum_mean.rs | 212 |
| H | ? | sum_mean.rs | 225 |
| H | ? | sum_mean.rs | 231 |
| H | ? | sum_mean.rs | 240 |
| H | ? | sum_mean.rs | 247 |
| H | ? | sum_mean.rs | 253 |
| H | ? | get.rs | 17 |
| H | ? | get.rs | 75 |
| H | ? | get.rs | 85 |
| H | ? | get.rs | 93 |
| H | ? | count.rs | 62 |
| H | ? | to_struct.rs | 87 |
| H | ? | to_struct.rs | 160 |
| H | ? | mod.rs | 120 |
| H | ? | mod.rs | 144 |
| H | ? | mod.rs | 149 |
| H | ? | mod.rs | 190 |
| H | ? | mod.rs | 202 |
| H | ? | mod.rs | 264 |
| H | ? | mod.rs | 274 |
| H | ? | mod.rs | 308 |
| H | ? | mod.rs | 345 |
| H | ? | mod.rs | 358 |
| H | ? | mod.rs | 363 |
| H | ? | mod.rs | 386 |
| H | ? | mod.rs | 389 |
| H | ? | mod.rs | 413 |
| H | ? | mod.rs | 423 |
| H | ? | mod.rs | 671 |
| H | ? | mod.rs | 675 |
| H | ? | merge_sorted.rs | 29 |
| H | ? | merge_sorted.rs | 31 |
| H | ? | merge_sorted.rs | 50 |
| H | ? | merge_sorted.rs | 84 |
| H | ? | merge_sorted.rs | 108 |
| H | ? | merge_sorted.rs | 117 |
| H | ? | merge_sorted.rs | 168 |
| H | ? | cross_join.rs | 173 |
| H | ? | mod.rs | 72 |
| H | ? | mod.rs | 99 |
| H | ? | mod.rs | 205 |
| H | ? | mod.rs | 206 |
| H | ? | mod.rs | 209 |
| H | ? | mod.rs | 215 |
| H | ? | single_keys_dispatch.rs | 706 |
| H | ? | single_keys_dispatch.rs | 707 |
| H | ? | single_keys.rs | 31 |
| H | ? | single_keys.rs | 57 |
| H | ? | single_keys.rs | 176 |
| H | ? | single_keys_inner.rs | 60 |
| H | ? | single_keys_outer.rs | 59 |
| H | ? | single_keys_outer.rs | 233 |
| H | ? | mod.rs | 312 |
| H | ? | groups.rs | 593 |
| H | ? | dispatch_left_right.rs | 47 |
| H | ? | dispatch_left_right.rs | 63 |
| H | ? | dispatch_left_right.rs | 69 |
| H | ? | merge_join.rs | 283 |
| H | ? | merge_join.rs | 284 |
| H | ? | merge_join.rs | 347 |
| H | ? | general.rs | 33 |
| H | ? | general.rs | 64 |
| H | ? | general.rs | 67 |
| H | ? | general.rs | 78 |
| H | ? | general.rs | 82 |
| H | ? | general.rs | 83 |
| H | ? | unpivot.rs | 99 |
| H | ? | unpivot.rs | 100 |
| H | ? | unpivot.rs | 134 |
| H | ? | mod.rs | 276 |
| H | ? | stats.rs | 120 |
| H | ? | spill_frame.rs | 26 |
| H | ? | memory_manager.rs | 90 |
| H | ? | memory_manager.rs | 101 |
| H | ? | memory_manager.rs | 103 |
| H | ? | memory_manager.rs | 104 |
| H | ? | memory_manager.rs | 108 |
| H | ? | memory_manager.rs | 158 |
| H | ? | spill_token.rs | 82 |
| H | ? | spill_token.rs | 225 |
| H | ? | spill_token.rs | 278 |
| H | ? | spill_token.rs | 341 |
| H | ? | spill_token.rs | 368 |
| H | ? | spill_token.rs | 380 |
| H | ? | spill_token.rs | 581 |
| H | ? | spill_token.rs | 644 |
| H | ? | mod.rs | 331 |
| H | ? | mod.rs | 569 |
| H | ? | task.rs | 102 |
| H | ? | task.rs | 129 |
| H | ? | task.rs | 206 |
| H | ? | wait_group.rs | 59 |
| H | ? | wait_group.rs | 80 |
| H | ? | linearizer.rs | 76 |
| H | ? | connector.rs | 20 |
| H | ? | connector.rs | 32 |
| H | ? | task_parker.rs | 65 |
| H | ? | distributor_channel.rs | 54 |
| H | ? | lib.rs | 34 |
| H | ? | mod.rs | 150 |
| H | ? | mod.rs | 159 |
| H | ? | mod.rs | 244 |
| H | ? | file.rs | 425 |
| H | ? | file.rs | 499 |
| H | ? | file.rs | 505 |
| H | ? | sql.rs | 18 |
| H | ? | arrow_c_stream.rs | 52 |
| H | ? | arrow_c_stream.rs | 87 |
| H | ? | import.rs | 52 |
| H | ? | import.rs | 119 |
| H | ? | mod.rs | 39 |
| H | ? | c_interface.rs | 53 |
| H | ? | c_interface.rs | 58 |
| H | ? | numpy_ufunc.rs | 44 |
| H | ? | numpy_ufunc.rs | 50 |
| H | ? | scatter.rs | 33 |
| H | ? | buffers.rs | 124 |
| H | ? | buffers.rs | 164 |
| H | ? | buffers.rs | 175 |
| H | ? | buffers.rs | 349 |
| H | ? | buffers.rs | 354 |
| H | ? | map.rs | 22 |
| H | ? | map.rs | 28 |
| H | ? | map.rs | 46 |
| H | ? | general.rs | 20 |
| H | ? | general.rs | 57 |
| H | ? | general.rs | 179 |
| H | ? | general.rs | 183 |
| H | ? | general.rs | 199 |
| H | ? | general.rs | 209 |
| H | ? | general.rs | 554 |
| H | ? | general.rs | 578 |
| H | ? | general.rs | 582 |
| H | ? | general.rs | 597 |
| H | ? | construction.rs | 47 |
| H | ? | construction.rs | 391 |
| H | ? | mod.rs | 30 |
| H | ? | exitable.rs | 13 |
| H | ? | optflags.rs | 31 |
| H | ? | expr_nodes.rs | 744 |
| H | ? | expr_nodes.rs | 752 |
| H | ? | expr_nodes.rs | 852 |
| H | ? | expr_nodes.rs | 873 |
| H | ? | expr_nodes.rs | 911 |
| H | ? | expr_nodes.rs | 912 |
| H | ? | expr_nodes.rs | 1179 |
| H | ? | expr_nodes.rs | 1545 |
| H | ? | expr_nodes.rs | 1548 |
| H | ? | expr_nodes.rs | 2013 |
| H | ? | nodes.rs | 103 |
| H | ? | nodes.rs | 460 |
| H | ? | nodes.rs | 474 |
| H | ? | nodes.rs | 485 |
| H | ? | nodes.rs | 522 |
| H | ? | nodes.rs | 523 |
| H | ? | nodes.rs | 553 |
| H | ? | visit.rs | 76 |
| H | ? | visit.rs | 130 |
| H | ? | visit.rs | 241 |
| H | ? | general.rs | 49 |
| H | ? | general.rs | 299 |
| H | ? | general.rs | 520 |
| H | ? | general.rs | 542 |
| H | ? | general.rs | 558 |
| H | ? | general.rs | 569 |
| H | ? | general.rs | 580 |
| H | ? | general.rs | 586 |
| H | ? | general.rs | 597 |
| H | ? | general.rs | 617 |
| H | ? | general.rs | 641 |
| H | ? | general.rs | 681 |
| H | ? | general.rs | 684 |
| H | ? | general.rs | 731 |
| H | ? | general.rs | 770 |
| H | ? | general.rs | 843 |
| H | ? | general.rs | 875 |
| H | ? | general.rs | 891 |
| H | ? | general.rs | 905 |
| H | ? | general.rs | 916 |
| H | ? | general.rs | 920 |
| H | ? | general.rs | 925 |
| H | ? | general.rs | 931 |
| H | ? | general.rs | 937 |
| H | ? | general.rs | 957 |
| H | ? | general.rs | 993 |
| H | ? | general.rs | 1017 |
| H | ? | general.rs | 1044 |
| H | ? | general.rs | 1095 |
| H | ? | general.rs | 1125 |
| H | ? | general.rs | 1139 |
| H | ? | general.rs | 1145 |
| H | ? | general.rs | 1150 |
| H | ? | general.rs | 1261 |
| H | ? | general.rs | 1269 |
| H | ? | general.rs | 1276 |
| H | ? | general.rs | 1283 |
| H | ? | general.rs | 1288 |
| H | ? | general.rs | 1294 |
| H | ? | general.rs | 1303 |
| H | ? | general.rs | 1308 |
| H | ? | general.rs | 1314 |
| H | ? | general.rs | 1320 |
| H | ? | general.rs | 1326 |
| H | ? | general.rs | 1332 |
| H | ? | general.rs | 1338 |
| H | ? | general.rs | 1344 |
| H | ? | general.rs | 1350 |
| H | ? | general.rs | 1358 |
| H | ? | general.rs | 1370 |
| H | ? | general.rs | 1381 |
| H | ? | general.rs | 1393 |
| H | ? | general.rs | 1401 |
| H | ? | general.rs | 1408 |
| H | ? | general.rs | 1413 |
| H | ? | general.rs | 1430 |
| H | ? | general.rs | 1433 |
| H | ? | general.rs | 1460 |
| H | ? | general.rs | 1466 |
| H | ? | general.rs | 1489 |
| H | ? | general.rs | 1500 |
| H | ? | general.rs | 1505 |
| H | ? | general.rs | 1506 |
| H | ? | general.rs | 1510 |
| H | ? | general.rs | 1514 |
| H | ? | general.rs | 1523 |
| H | ? | general.rs | 1532 |
| H | ? | general.rs | 1538 |
| H | ? | general.rs | 1547 |
| H | ? | general.rs | 1607 |
| H | ? | general.rs | 1642 |
| H | ? | general.rs | 1650 |
| H | ? | general.rs | 1683 |
| H | ? | lazygroupby.rs | 23 |
| H | ? | lazygroupby.rs | 32 |
| H | ? | lazygroupby.rs | 38 |
| H | ? | lazygroupby.rs | 43 |
| H | ? | lazygroupby.rs | 49 |
| H | ? | lazygroupby.rs | 52 |
| H | ? | on_startup.rs | 47 |
| H | ? | on_startup.rs | 153 |
| H | ? | on_startup.rs | 156 |
| H | ? | on_startup.rs | 223 |
| H | ? | on_startup.rs | 229 |
| H | ? | on_startup.rs | 239 |
| H | ? | on_startup.rs | 250 |
| H | ? | extension.rs | 37 |
| H | ? | extension.rs | 70 |
| H | ? | extension.rs | 110 |
| H | ? | io.rs | 67 |
| H | ? | whenthen.rs | 42 |
| H | ? | whenthen.rs | 51 |
| H | ? | whenthen.rs | 56 |
| H | ? | whenthen.rs | 72 |
| H | ? | whenthen.rs | 81 |
| H | ? | whenthen.rs | 86 |
| H | ? | eager.rs | 28 |
| H | ? | lazy.rs | 496 |
| H | ? | series.rs | 67 |
| H | ? | series.rs | 79 |
| H | ? | series.rs | 97 |
| H | ? | series.rs | 109 |
| H | ? | series.rs | 123 |
| H | ? | series.rs | 135 |
| H | ? | series.rs | 150 |
| H | ? | series.rs | 163 |
| H | ? | series.rs | 179 |
| H | ? | series.rs | 192 |
| H | ? | series.rs | 207 |
| H | ? | series.rs | 219 |
| H | ? | series.rs | 235 |
| H | ? | series.rs | 249 |
| H | ? | series.rs | 263 |
| H | ? | series.rs | 275 |
| H | ? | series.rs | 296 |
| H | ? | series.rs | 310 |
| H | ? | series.rs | 325 |
| H | ? | series.rs | 338 |
| H | ? | lazy.rs | 26 |
| H | ? | lazy.rs | 46 |
| H | ? | mod.rs | 27 |
| H | ? | io.rs | 74 |
| H | ? | io.rs | 83 |
| H | ? | export.rs | 50 |
| H | ? | export.rs | 85 |
| H | ? | export.rs | 87 |
| H | ? | export.rs | 109 |
| H | ? | export.rs | 111 |
| H | ? | export.rs | 150 |
| H | ? | export.rs | 154 |
| H | ? | export.rs | 156 |
| H | ? | export.rs | 176 |
| H | ? | map.rs | 29 |
| H | ? | map.rs | 113 |
| H | ? | map.rs | 158 |
| H | ? | general.rs | 130 |
| H | ? | general.rs | 171 |
| H | ? | general.rs | 217 |
| H | ? | general.rs | 227 |
| H | ? | general.rs | 254 |
| H | ? | general.rs | 274 |
| H | ? | general.rs | 390 |
| H | ? | general.rs | 478 |
| H | ? | general.rs | 565 |
| H | ? | construction.rs | 123 |
| H | ? | construction.rs | 165 |
| H | ? | construction.rs | 197 |
| H | ? | to_numpy_series.rs | 102 |
| H | ? | to_numpy_series.rs | 273 |
| H | ? | to_numpy_df.rs | 94 |
| H | ? | to_py.rs | 43 |
| H | ? | to_py.rs | 72 |
| H | ? | to_py.rs | 135 |
| H | ? | to_py.rs | 145 |
| H | ? | to_py.rs | 166 |
| H | ? | to_rust.rs | 71 |
| H | ? | to_rust.rs | 117 |
| H | ? | to_rust.rs | 142 |
| H | ? | to_rust.rs | 163 |
| H | ? | mod.rs | 102 |
| H | ? | mod.rs | 293 |
| H | ? | mod.rs | 299 |
| H | ? | mod.rs | 323 |
| H | ? | mod.rs | 343 |
| H | ? | mod.rs | 355 |
| H | ? | mod.rs | 475 |
| H | ? | mod.rs | 481 |
| H | ? | mod.rs | 731 |
| H | ? | mod.rs | 1473 |
| H | ? | mod.rs | 1968 |
| H | ? | any_value.rs | 54 |
| H | ? | any_value.rs | 488 |
| H | ? | any_value.rs | 579 |
| H | ? | chunked_array.rs | 46 |
| H | ? | string.rs | 13 |
| H | ? | string.rs | 29 |
| H | ? | string.rs | 53 |
| H | ? | string.rs | 74 |
| H | ? | string.rs | 78 |
| H | ? | string.rs | 83 |
| H | ? | string.rs | 91 |
| H | ? | string.rs | 98 |
| H | ? | string.rs | 102 |
| H | ? | string.rs | 107 |
| H | ? | string.rs | 114 |
| H | ? | string.rs | 118 |
| H | ? | string.rs | 122 |
| H | ? | string.rs | 126 |
| H | ? | string.rs | 131 |
| H | ? | string.rs | 135 |
| H | ? | string.rs | 139 |
| H | ? | string.rs | 145 |
| H | ? | string.rs | 154 |
| H | ? | string.rs | 161 |
| H | ? | string.rs | 165 |
| H | ? | string.rs | 170 |
| H | ? | string.rs | 178 |
| H | ? | string.rs | 185 |
| H | ? | string.rs | 192 |
| H | ? | string.rs | 193 |
| H | ? | string.rs | 201 |
| H | ? | string.rs | 202 |
| H | ? | string.rs | 207 |
| H | ? | string.rs | 211 |
| H | ? | string.rs | 215 |
| H | ? | string.rs | 220 |
| H | ? | string.rs | 224 |
| H | ? | string.rs | 229 |
| H | ? | string.rs | 235 |
| H | ? | string.rs | 243 |
| H | ? | string.rs | 248 |
| H | ? | string.rs | 253 |
| H | ? | string.rs | 260 |
| H | ? | string.rs | 267 |
| H | ? | string.rs | 276 |
| H | ? | string.rs | 283 |
| H | ? | string.rs | 287 |
| H | ? | string.rs | 291 |
| H | ? | string.rs | 296 |
| H | ? | string.rs | 303 |
| H | ? | string.rs | 319 |
| H | ? | string.rs | 328 |
| H | ? | string.rs | 335 |
| H | ? | string.rs | 341 |
| H | ? | string.rs | 355 |
| H | ? | string.rs | 375 |
| H | ? | string.rs | 395 |
| H | ? | string.rs | 408 |
| H | ? | binary.rs | 10 |
| H | ? | binary.rs | 17 |
| H | ? | binary.rs | 21 |
| H | ? | binary.rs | 26 |
| H | ? | binary.rs | 31 |
| H | ? | binary.rs | 36 |
| H | ? | binary.rs | 41 |
| H | ? | binary.rs | 59 |
| H | ? | binary.rs | 66 |
| H | ? | binary.rs | 71 |
| H | ? | binary.rs | 78 |
| H | ? | binary.rs | 82 |
| H | ? | binary.rs | 87 |
| H | ? | datetime.rs | 17 |
| H | ? | datetime.rs | 24 |
| H | ? | datetime.rs | 28 |
| H | ? | datetime.rs | 32 |
| H | ? | datetime.rs | 41 |
| H | ? | datetime.rs | 52 |
| H | ? | datetime.rs | 67 |
| H | ? | datetime.rs | 78 |
| H | ? | datetime.rs | 82 |
| H | ? | datetime.rs | 86 |
| H | ? | datetime.rs | 91 |
| H | ? | datetime.rs | 95 |
| H | ? | datetime.rs | 99 |
| H | ? | datetime.rs | 114 |
| H | ? | datetime.rs | 131 |
| H | ? | datetime.rs | 137 |
| H | ? | datetime.rs | 140 |
| H | ? | datetime.rs | 143 |
| H | ? | datetime.rs | 147 |
| H | ? | datetime.rs | 153 |
| H | ? | datetime.rs | 156 |
| H | ? | datetime.rs | 159 |
| H | ? | datetime.rs | 162 |
| H | ? | datetime.rs | 165 |
| H | ? | datetime.rs | 168 |
| H | ? | datetime.rs | 171 |
| H | ? | datetime.rs | 174 |
| H | ? | datetime.rs | 177 |
| H | ? | datetime.rs | 180 |
| H | ? | datetime.rs | 183 |
| H | ? | datetime.rs | 186 |
| H | ? | datetime.rs | 189 |
| H | ? | datetime.rs | 192 |
| H | ? | datetime.rs | 195 |
| H | ? | datetime.rs | 198 |
| H | ? | datetime.rs | 201 |
| H | ? | datetime.rs | 204 |
| H | ? | datetime.rs | 207 |
| H | ? | datetime.rs | 210 |
| H | ? | datetime.rs | 213 |
| H | ? | datetime.rs | 216 |
| H | ? | datetime.rs | 219 |
| H | ? | datetime.rs | 223 |
| H | ? | datetime.rs | 230 |
| H | ? | datetime.rs | 236 |
| H | ? | selector.rs | 52 |
| H | ? | selector.rs | 58 |
| H | ? | selector.rs | 64 |
| H | ? | selector.rs | 70 |
| H | ? | array.rs | 12 |
| H | ? | array.rs | 16 |
| H | ? | array.rs | 20 |
| H | ? | array.rs | 24 |
| H | ? | array.rs | 28 |
| H | ? | array.rs | 32 |
| H | ? | array.rs | 36 |
| H | ? | array.rs | 40 |
| H | ? | array.rs | 44 |
| H | ? | array.rs | 49 |
| H | ? | array.rs | 60 |
| H | ? | array.rs | 64 |
| H | ? | array.rs | 69 |
| H | ? | array.rs | 77 |
| H | ? | array.rs | 86 |
| H | ? | array.rs | 94 |
| H | ? | array.rs | 100 |
| H | ? | array.rs | 110 |
| H | ? | array.rs | 120 |
| H | ? | array.rs | 128 |
| H | ? | array.rs | 133 |
| H | ? | array.rs | 143 |
| H | ? | array.rs | 147 |
| H | ? | list.rs | 13 |
| H | ? | list.rs | 17 |
| H | ? | list.rs | 23 |
| H | ? | list.rs | 31 |
| H | ? | list.rs | 35 |
| H | ? | list.rs | 39 |
| H | ? | list.rs | 43 |
| H | ? | list.rs | 49 |
| H | ? | list.rs | 57 |
| H | ? | list.rs | 65 |
| H | ? | list.rs | 72 |
| H | ? | list.rs | 76 |
| H | ? | list.rs | 80 |
| H | ? | list.rs | 84 |
| H | ? | list.rs | 88 |
| H | ? | list.rs | 92 |
| H | ? | list.rs | 96 |
| H | ? | list.rs | 100 |
| H | ? | list.rs | 109 |
| H | ? | list.rs | 113 |
| H | ? | list.rs | 118 |
| H | ? | list.rs | 129 |
| H | ? | list.rs | 134 |
| H | ? | list.rs | 147 |
| H | ? | list.rs | 163 |
| H | ? | list.rs | 172 |
| H | ? | list.rs | 181 |
| H | ? | list.rs | 188 |
| H | ? | list.rs | 195 |
| H | ? | list.rs | 208 |
| H | ? | rolling.rs | 27 |
| H | ? | rolling.rs | 44 |
| H | ? | rolling.rs | 63 |
| H | ? | rolling.rs | 80 |
| H | ? | rolling.rs | 99 |
| H | ? | rolling.rs | 115 |
| H | ? | rolling.rs | 135 |
| H | ? | rolling.rs | 153 |
| H | ? | rolling.rs | 174 |
| H | ? | rolling.rs | 193 |
| H | ? | rolling.rs | 214 |
| H | ? | rolling.rs | 233 |
| H | ? | rolling.rs | 252 |
| H | ? | rolling.rs | 271 |
| H | ? | rolling.rs | 296 |
| H | ? | rolling.rs | 320 |
| H | ? | rolling.rs | 346 |
| H | ? | rolling.rs | 369 |
| H | ? | rolling.rs | 389 |
| H | ? | rolling.rs | 410 |
| H | ? | rolling.rs | 432 |
| H | ? | extension.rs | 9 |
| H | ? | extension.rs | 13 |
| H | ? | categorical.rs | 9 |
| H | ? | categorical.rs | 13 |
| H | ? | categorical.rs | 17 |
| H | ? | categorical.rs | 21 |
| H | ? | categorical.rs | 25 |
| H | ? | categorical.rs | 30 |
| H | ? | categorical.rs | 34 |
| H | ? | categorical.rs | 38 |
| H | ? | bitwise.rs | 8 |
| H | ? | bitwise.rs | 12 |
| H | ? | bitwise.rs | 16 |
| H | ? | bitwise.rs | 20 |
| H | ? | bitwise.rs | 24 |
| H | ? | bitwise.rs | 28 |
| H | ? | bitwise.rs | 32 |
| H | ? | bitwise.rs | 36 |
| H | ? | bitwise.rs | 40 |
| H | ? | datatype.rs | 46 |
| H | ? | datatype.rs | 54 |
| H | ? | datatype.rs | 58 |
| H | ? | datatype.rs | 62 |
| H | ? | datatype.rs | 67 |
| H | ? | datatype.rs | 80 |
| H | ? | datatype.rs | 84 |
| H | ? | datatype.rs | 88 |
| H | ? | datatype.rs | 92 |
| H | ? | datatype.rs | 97 |
| H | ? | datatype.rs | 103 |
| H | ? | datatype.rs | 107 |
| H | ? | datatype.rs | 111 |
| H | ? | datatype.rs | 115 |
| H | ? | datatype.rs | 120 |
| H | ? | datatype.rs | 128 |
| H | ? | datatype.rs | 135 |
| H | ? | name.rs | 10 |
| H | ? | name.rs | 15 |
| H | ? | name.rs | 22 |
| H | ? | name.rs | 26 |
| H | ? | name.rs | 30 |
| H | ? | name.rs | 34 |
| H | ? | name.rs | 39 |
| H | ? | name.rs | 47 |
| H | ? | name.rs | 54 |
| H | ? | name.rs | 58 |
| H | ? | struct.rs | 9 |
| H | ? | struct.rs | 13 |
| H | ? | struct.rs | 17 |
| H | ? | struct.rs | 21 |
| H | ? | struct.rs | 26 |
| H | ? | struct.rs | 31 |
| H | ? | meta.rs | 19 |
| H | ? | meta.rs | 28 |
| H | ? | meta.rs | 39 |
| H | ? | meta.rs | 47 |
| H | ? | meta.rs | 51 |
| H | ? | meta.rs | 55 |
| H | ? | meta.rs | 59 |
| H | ? | meta.rs | 64 |
| H | ? | meta.rs | 70 |
| H | ? | meta.rs | 80 |
| H | ? | general.rs | 43 |
| H | ? | general.rs | 46 |
| H | ? | general.rs | 49 |
| H | ? | general.rs | 52 |
| H | ? | general.rs | 55 |
| H | ? | general.rs | 58 |
| H | ? | general.rs | 61 |
| H | ? | general.rs | 68 |
| H | ? | general.rs | 72 |
| H | ? | general.rs | 75 |
| H | ? | general.rs | 78 |
| H | ? | general.rs | 81 |
| H | ? | general.rs | 84 |
| H | ? | general.rs | 87 |
| H | ? | general.rs | 90 |
| H | ? | general.rs | 94 |
| H | ? | general.rs | 97 |
| H | ? | general.rs | 100 |
| H | ? | general.rs | 103 |
| H | ? | general.rs | 107 |
| H | ? | general.rs | 111 |
| H | ? | general.rs | 115 |
| H | ? | general.rs | 119 |
| H | ? | general.rs | 123 |
| H | ? | general.rs | 127 |
| H | ? | general.rs | 131 |
| H | ? | general.rs | 135 |
| H | ? | general.rs | 140 |
| H | ? | general.rs | 144 |
| H | ? | general.rs | 147 |
| H | ? | general.rs | 150 |
| H | ? | general.rs | 153 |
| H | ? | general.rs | 156 |
| H | ? | general.rs | 159 |
| H | ? | general.rs | 162 |
| H | ? | general.rs | 165 |
| H | ? | general.rs | 169 |
| H | ? | general.rs | 171 |
| H | ? | general.rs | 176 |
| H | ? | general.rs | 178 |
| H | ? | general.rs | 182 |
| H | ? | general.rs | 185 |
| H | ? | general.rs | 189 |
| H | ? | general.rs | 204 |
| H | ? | general.rs | 219 |
| H | ? | general.rs | 234 |
| H | ? | general.rs | 247 |
| H | ? | general.rs | 251 |
| H | ? | general.rs | 255 |
| H | ? | general.rs | 258 |
| H | ? | general.rs | 261 |
| H | ? | general.rs | 265 |
| H | ? | general.rs | 270 |
| H | ? | general.rs | 273 |
| H | ? | general.rs | 284 |
| H | ? | general.rs | 289 |
| H | ? | general.rs | 301 |
| H | ? | general.rs | 306 |
| H | ? | general.rs | 312 |
| H | ? | general.rs | 317 |
| H | ? | general.rs | 323 |
| H | ? | general.rs | 328 |
| H | ? | general.rs | 333 |
| H | ? | general.rs | 337 |
| H | ? | general.rs | 341 |
| H | ? | general.rs | 346 |
| H | ? | general.rs | 353 |
| H | ? | general.rs | 360 |
| H | ? | general.rs | 365 |
| H | ? | general.rs | 378 |
| H | ? | general.rs | 394 |
| H | ? | general.rs | 403 |
| H | ? | general.rs | 408 |
| H | ? | general.rs | 412 |
| H | ? | general.rs | 416 |
| H | ? | general.rs | 420 |
| H | ? | general.rs | 424 |
| H | ? | general.rs | 428 |
| H | ? | general.rs | 432 |
| H | ? | general.rs | 436 |
| H | ? | general.rs | 440 |
| H | ? | general.rs | 445 |
| H | ? | general.rs | 452 |
| H | ? | general.rs | 458 |
| H | ? | general.rs | 463 |
| H | ? | general.rs | 467 |
| H | ? | general.rs | 471 |
| H | ? | general.rs | 476 |
| H | ? | general.rs | 485 |
| H | ? | general.rs | 489 |
| H | ? | general.rs | 493 |
| H | ? | general.rs | 497 |
| H | ? | general.rs | 501 |
| H | ? | general.rs | 505 |
| H | ? | general.rs | 509 |
| H | ? | general.rs | 513 |
| H | ? | general.rs | 517 |
| H | ? | general.rs | 522 |
| H | ? | general.rs | 533 |
| H | ? | general.rs | 538 |
| H | ? | general.rs | 543 |
| H | ? | general.rs | 548 |
| H | ? | general.rs | 553 |
| H | ? | general.rs | 558 |
| H | ? | general.rs | 563 |
| H | ? | general.rs | 568 |
| H | ? | general.rs | 573 |
| H | ? | general.rs | 578 |
| H | ? | general.rs | 583 |
| H | ? | general.rs | 588 |
| H | ? | general.rs | 593 |
| H | ? | general.rs | 598 |
| H | ? | general.rs | 603 |
| H | ? | general.rs | 608 |
| H | ? | general.rs | 613 |
| H | ? | general.rs | 618 |
| H | ? | general.rs | 622 |
| H | ? | general.rs | 655 |
| H | ? | general.rs | 674 |
| H | ? | general.rs | 680 |
| H | ? | general.rs | 684 |
| H | ? | general.rs | 688 |
| H | ? | general.rs | 693 |
| H | ? | general.rs | 698 |
| H | ? | general.rs | 702 |
| H | ? | general.rs | 706 |
| H | ? | general.rs | 710 |
| H | ? | general.rs | 714 |
| H | ? | general.rs | 717 |
| H | ? | general.rs | 720 |
| H | ? | general.rs | 723 |
| H | ? | general.rs | 726 |
| H | ? | general.rs | 731 |
| H | ? | general.rs | 737 |
| H | ? | general.rs | 741 |
| H | ? | general.rs | 746 |
| H | ? | general.rs | 751 |
| H | ? | general.rs | 754 |
| H | ? | general.rs | 757 |
| H | ? | general.rs | 761 |
| H | ? | general.rs | 765 |
| H | ? | general.rs | 774 |
| H | ? | general.rs | 778 |
| H | ? | general.rs | 783 |
| H | ? | general.rs | 787 |
| H | ? | general.rs | 790 |
| H | ? | general.rs | 795 |
| H | ? | general.rs | 799 |
| H | ? | general.rs | 804 |
| H | ? | general.rs | 816 |
| H | ? | general.rs | 830 |
| H | ? | general.rs | 843 |
| H | ? | general.rs | 853 |
| H | ? | general.rs | 859 |
| H | ? | general.rs | 865 |
| H | ? | general.rs | 883 |
| H | ? | general.rs | 900 |
| H | ? | general.rs | 904 |
| H | ? | general.rs | 910 |
| H | ? | general.rs | 913 |
| H | ? | general.rs | 916 |
| H | ? | general.rs | 920 |
| H | ? | general.rs | 924 |
| H | ? | general.rs | 928 |
| H | ? | general.rs | 932 |
| H | ? | general.rs | 936 |
| H | ? | general.rs | 939 |
| H | ? | general.rs | 945 |
| H | ? | general.rs | 949 |
| H | ? | general.rs | 961 |
| H | ? | general.rs | 982 |
| H | ? | general.rs | 993 |
| H | ? | general.rs | 1009 |
| H | ? | general.rs | 1026 |
| H | ? | general.rs | 1038 |
| H | ? | general.rs | 1059 |
| H | ? | general.rs | 1075 |
| H | ? | unity.rs | 223 |
| H | ? | deserialize.rs | 56 |
| H | ? | deserialize.rs | 207 |
| H | ? | deserialize.rs | 287 |
| H | ? | deserialize.rs | 292 |
| H | ? | infer_schema.rs | 81 |
| H | ? | infer_schema.rs | 143 |
| H | ? | infer_schema.rs | 150 |
| H | ? | infer_schema.rs | 179 |
| H | ? | infer_schema.rs | 180 |
| H | ? | mod.rs | 63 |
| H | ? | mod.rs | 87 |
| H | ? | mod.rs | 191 |
| H | ? | mod.rs | 208 |
| H | ? | mod.rs | 210 |
| H | ? | serde.rs | 37 |
| H | ? | serde.rs | 189 |
| H | ? | serde.rs | 190 |
| H | ? | serde.rs | 204 |
| H | ? | serde.rs | 231 |
| H | ? | serde.rs | 237 |
| H | ? | serde.rs | 238 |
| H | ? | serde.rs | 328 |
| H | ? | new.rs | 20 |
| H | ? | new.rs | 40 |
| H | ? | new.rs | 48 |
| H | ? | new.rs | 74 |
| H | ? | new.rs | 75 |
| H | ? | named_from.rs | 188 |
| H | ? | mod.rs | 41 |
| H | ? | mod.rs | 64 |
| H | ? | mod.rs | 213 |
| H | ? | mod.rs | 276 |
| H | ? | mod.rs | 357 |
| H | ? | mod.rs | 402 |
| H | ? | mod.rs | 403 |
| H | ? | mod.rs | 477 |
| H | ? | categorical.rs | 106 |
| H | ? | categorical.rs | 124 |
| H | ? | categorical.rs | 125 |
| H | ? | categorical.rs | 206 |
| H | ? | categorical.rs | 218 |
| H | ? | mod.rs | 179 |
| H | ? | mod.rs | 186 |
| H | ? | mod.rs | 208 |
| H | ? | mod.rs | 245 |
| H | ? | mod.rs | 426 |
| H | ? | mod.rs | 450 |
| H | ? | mod.rs | 461 |
| H | ? | mod.rs | 508 |
| H | ? | mod.rs | 517 |
| H | ? | mod.rs | 528 |
| H | ? | mod.rs | 529 |
| H | ? | mod.rs | 540 |
| H | ? | mod.rs | 541 |
| H | ? | mod.rs | 547 |
| H | ? | mod.rs | 550 |
| H | ? | mod.rs | 553 |
| H | ? | mod.rs | 555 |
| H | ? | mod.rs | 560 |
| H | ? | mod.rs | 567 |
| H | ? | mod.rs | 581 |
| H | ? | mod.rs | 599 |
| H | ? | mod.rs | 647 |
| H | ? | mod.rs | 658 |
| H | ? | mod.rs | 662 |
| H | ? | mod.rs | 678 |
| H | ? | mod.rs | 691 |
| H | ? | mod.rs | 695 |
| H | ? | mod.rs | 708 |
| H | ? | mod.rs | 712 |
| H | ? | mod.rs | 746 |
| H | ? | mod.rs | 748 |
| H | ? | mod.rs | 750 |
| H | ? | mod.rs | 752 |
| H | ? | mod.rs | 757 |
| H | ? | mod.rs | 761 |
| H | ? | mod.rs | 873 |
| H | ? | mod.rs | 888 |
| H | ? | mod.rs | 893 |
| H | ? | mod.rs | 907 |
| H | ? | mod.rs | 912 |
| H | ? | mod.rs | 931 |
| H | ? | mod.rs | 938 |
| H | ? | mod.rs | 956 |
| H | ? | mod.rs | 963 |
| H | ? | mod.rs | 1055 |
| H | ? | mod.rs | 1056 |
| H | ? | mod.rs | 1066 |
| H | ? | mod.rs | 1067 |
| H | ? | mod.rs | 1210 |
| H | ? | iterator.rs | 220 |
| H | ? | any_value.rs | 137 |
| H | ? | any_value.rs | 151 |
| H | ? | any_value.rs | 152 |
| H | ? | any_value.rs | 158 |
| H | ? | any_value.rs | 518 |
| H | ? | any_value.rs | 572 |
| H | ? | any_value.rs | 738 |
| H | ? | any_value.rs | 754 |
| H | ? | any_value.rs | 756 |
| H | ? | any_value.rs | 760 |
| H | ? | any_value.rs | 775 |
| H | ? | any_value.rs | 787 |
| H | ? | any_value.rs | 798 |
| H | ? | any_value.rs | 837 |
| H | ? | any_value.rs | 919 |
| H | ? | any_value.rs | 922 |
| H | ? | proptest.rs | 116 |
| H | ? | proptest.rs | 119 |
| H | ? | proptest.rs | 122 |
| H | ? | proptest.rs | 125 |
| H | ? | proptest.rs | 128 |
| H | ? | proptest.rs | 131 |
| H | ? | proptest.rs | 135 |
| H | ? | proptest.rs | 139 |
| H | ? | proptest.rs | 143 |
| H | ? | proptest.rs | 147 |
| H | ? | proptest.rs | 151 |
| H | ? | proptest.rs | 155 |
| H | ? | proptest.rs | 156 |
| H | ? | proptest.rs | 161 |
| H | ? | proptest.rs | 162 |
| H | ? | proptest.rs | 166 |
| H | ? | proptest.rs | 167 |
| H | ? | proptest.rs | 172 |
| H | ? | proptest.rs | 173 |
| H | ? | proptest.rs | 178 |
| H | ? | proptest.rs | 179 |
| H | ? | proptest.rs | 198 |
| H | ? | proptest.rs | 200 |
| H | ? | proptest.rs | 202 |
| H | ? | proptest.rs | 204 |
| H | ? | proptest.rs | 215 |
| H | ? | proptest.rs | 217 |
| H | ? | proptest.rs | 219 |
| H | ? | proptest.rs | 221 |
| H | ? | proptest.rs | 232 |
| H | ? | proptest.rs | 336 |
| H | ? | proptest.rs | 366 |
| H | ? | proptest.rs | 369 |
| H | ? | proptest.rs | 376 |
| H | ? | proptest.rs | 397 |
| H | ? | proptest.rs | 401 |
| H | ? | proptest.rs | 419 |
| H | ? | proptest.rs | 425 |
| H | ? | proptest.rs | 436 |
| H | ? | proptest.rs | 450 |
| H | ? | proptest.rs | 455 |
| H | ? | amortized_iter.rs | 30 |
| H | ? | amortized_iter.rs | 31 |
| H | ? | comparison.rs | 109 |
| H | ? | comparison.rs | 230 |
| H | ? | comparison.rs | 382 |
| H | ? | comparison.rs | 399 |
| H | ? | comparison.rs | 418 |
| H | ? | comparison.rs | 434 |
| H | ? | from.rs | 93 |
| H | ? | from.rs | 101 |
| H | ? | from.rs | 104 |
| H | ? | from.rs | 112 |
| H | ? | from.rs | 123 |
| H | ? | from.rs | 130 |
| H | ? | from.rs | 143 |
| H | ? | from.rs | 269 |
| H | ? | from.rs | 436 |
| H | ? | from.rs | 461 |
| H | ? | from.rs | 479 |
| H | ? | from.rs | 482 |
| H | ? | from.rs | 520 |
| H | ? | from.rs | 537 |
| H | ? | from.rs | 598 |
| H | ? | from.rs | 635 |
| H | ? | from.rs | 639 |
| H | ? | from.rs | 645 |
| H | ? | from.rs | 649 |
| H | ? | from.rs | 654 |
| H | ? | from.rs | 664 |
| H | ? | from.rs | 677 |
| H | ? | from.rs | 693 |
| H | ? | from.rs | 706 |
| H | ? | from.rs | 709 |
| H | ? | from.rs | 730 |
| H | ? | from.rs | 741 |
| H | ? | from.rs | 756 |
| H | ? | from.rs | 777 |
| H | ? | from.rs | 779 |
| H | ? | from.rs | 812 |
| H | ? | from.rs | 865 |
| H | ? | from.rs | 911 |
| H | ? | from.rs | 980 |
| H | ? | series_trait.rs | 97 |
| H | ? | series_trait.rs | 104 |
| H | ? | series_trait.rs | 111 |
| H | ? | series_trait.rs | 119 |
| H | ? | series_trait.rs | 126 |
| H | ? | series_trait.rs | 133 |
| H | ? | series_trait.rs | 140 |
| H | ? | series_trait.rs | 147 |
| H | ? | series_trait.rs | 155 |
| H | ? | series_trait.rs | 163 |
| H | ? | series_trait.rs | 171 |
| H | ? | series_trait.rs | 583 |
| H | ? | series_trait.rs | 600 |
| H | ? | series_trait.rs | 615 |
| H | ? | series_trait.rs | 634 |
| H | ? | string.rs | 191 |
| H | ? | duration.rs | 140 |
| H | ? | duration.rs | 188 |
| H | ? | duration.rs | 210 |
| H | ? | duration.rs | 251 |
| H | ? | duration.rs | 427 |
| H | ? | duration.rs | 525 |
| H | ? | duration.rs | 531 |
| H | ? | duration.rs | 536 |
| H | ? | duration.rs | 543 |
| H | ? | duration.rs | 551 |
| H | ? | duration.rs | 557 |
| H | ? | duration.rs | 564 |
| H | ? | duration.rs | 580 |
| H | ? | mod.rs | 322 |
| H | ? | mod.rs | 550 |
| H | ? | date.rs | 103 |
| H | ? | date.rs | 300 |
| H | ? | date.rs | 318 |
| H | ? | date.rs | 406 |
| H | ? | date.rs | 412 |
| H | ? | binary.rs | 187 |
| H | ? | datetime.rs | 44 |
| H | ? | datetime.rs | 79 |
| H | ? | datetime.rs | 88 |
| H | ? | datetime.rs | 108 |
| H | ? | datetime.rs | 127 |
| H | ? | datetime.rs | 141 |
| H | ? | datetime.rs | 243 |
| H | ? | datetime.rs | 251 |
| H | ? | datetime.rs | 257 |
| H | ? | datetime.rs | 264 |
| H | ? | datetime.rs | 270 |
| H | ? | datetime.rs | 278 |
| H | ? | datetime.rs | 291 |
| H | ? | datetime.rs | 298 |
| H | ? | datetime.rs | 300 |
| H | ? | datetime.rs | 308 |
| H | ? | datetime.rs | 329 |
| H | ? | datetime.rs | 348 |
| H | ? | datetime.rs | 380 |
| H | ? | datetime.rs | 392 |
| H | ? | datetime.rs | 401 |
| H | ? | datetime.rs | 409 |
| H | ? | datetime.rs | 415 |
| H | ? | datetime.rs | 422 |
| H | ? | datetime.rs | 429 |
| H | ? | datetime.rs | 443 |
| H | ? | datetime.rs | 446 |
| H | ? | array.rs | 42 |
| H | ? | array.rs | 51 |
| H | ? | array.rs | 119 |
| H | ? | array.rs | 198 |
| H | ? | array.rs | 236 |
| H | ? | array.rs | 242 |
| H | ? | array.rs | 263 |
| H | ? | array.rs | 269 |
| H | ? | array.rs | 274 |
| H | ? | null.rs | 55 |
| H | ? | null.rs | 77 |
| H | ? | null.rs | 99 |
| H | ? | null.rs | 181 |
| H | ? | null.rs | 205 |
| H | ? | null.rs | 209 |
| H | ? | null.rs | 213 |
| H | ? | null.rs | 217 |
| H | ? | null.rs | 222 |
| H | ? | null.rs | 234 |
| H | ? | null.rs | 238 |
| H | ? | null.rs | 242 |
| H | ? | null.rs | 246 |
| H | ? | null.rs | 255 |
| H | ? | null.rs | 268 |
| H | ? | null.rs | 281 |
| H | ? | null.rs | 291 |
| H | ? | null.rs | 302 |
| H | ? | null.rs | 308 |
| H | ? | null.rs | 317 |
| H | ? | null.rs | 321 |
| H | ? | null.rs | 325 |
| H | ? | null.rs | 329 |
| H | ? | null.rs | 333 |
| H | ? | null.rs | 343 |
| H | ? | null.rs | 344 |
| H | ? | null.rs | 350 |
| H | ? | null.rs | 354 |
| H | ? | null.rs | 402 |
| H | ? | null.rs | 412 |
| H | ? | list.rs | 29 |
| H | ? | list.rs | 38 |
| H | ? | list.rs | 177 |
| H | ? | list.rs | 215 |
| H | ? | list.rs | 221 |
| H | ? | list.rs | 242 |
| H | ? | list.rs | 248 |
| H | ? | list.rs | 253 |
| H | ? | struct_.rs | 51 |
| H | ? | struct_.rs | 58 |
| H | ? | struct_.rs | 74 |
| H | ? | struct_.rs | 81 |
| H | ? | struct_.rs | 91 |
| H | ? | struct_.rs | 215 |
| H | ? | struct_.rs | 249 |
| H | ? | struct_.rs | 255 |
| H | ? | struct_.rs | 279 |
| H | ? | struct_.rs | 284 |
| H | ? | struct_.rs | 289 |
| H | ? | struct_.rs | 305 |
| H | ? | struct_.rs | 311 |
| H | ? | struct_.rs | 316 |
| H | ? | binary_offset.rs | 154 |
| H | ? | time.rs | 102 |
| H | ? | time.rs | 112 |
| H | ? | time.rs | 279 |
| H | ? | time.rs | 297 |
| H | ? | time.rs | 379 |
| H | ? | time.rs | 385 |
| H | ? | time.rs | 391 |
| H | ? | time.rs | 397 |
| H | ? | time.rs | 403 |
| H | ? | time.rs | 417 |
| H | ? | extension.rs | 15 |
| H | ? | extension.rs | 22 |
| H | ? | extension.rs | 83 |
| H | ? | extension.rs | 84 |
| H | ? | extension.rs | 128 |
| H | ? | extension.rs | 134 |
| H | ? | extension.rs | 135 |
| H | ? | extension.rs | 281 |
| H | ? | extension.rs | 286 |
| H | ? | categorical.rs | 21 |
| H | ? | categorical.rs | 34 |
| H | ? | categorical.rs | 102 |
| H | ? | categorical.rs | 112 |
| H | ? | categorical.rs | 140 |
| H | ? | categorical.rs | 141 |
| H | ? | categorical.rs | 191 |
| H | ? | categorical.rs | 192 |
| H | ? | categorical.rs | 253 |
| H | ? | boolean.rs | 213 |
| H | ? | decimal.rs | 53 |
| H | ? | decimal.rs | 64 |
| H | ? | decimal.rs | 70 |
| H | ? | decimal.rs | 76 |
| H | ? | decimal.rs | 82 |
| H | ? | decimal.rs | 352 |
| H | ? | decimal.rs | 463 |
| H | ? | decimal.rs | 478 |
| H | ? | decimal.rs | 541 |
| H | ? | floats.rs | 253 |
| H | ? | floats.rs | 338 |
| H | ? | object.rs | 186 |
| H | ? | object.rs | 195 |
| H | ? | borrowed.rs | 360 |
| H | ? | borrowed.rs | 372 |
| H | ? | borrowed.rs | 402 |
| H | ? | borrowed.rs | 480 |
| H | ? | borrowed.rs | 580 |
| H | ? | borrowed.rs | 671 |
| H | ? | list_utils.rs | 98 |
| H | ? | list.rs | 12 |
| H | ? | list.rs | 16 |
| H | ? | list.rs | 20 |
| H | ? | list.rs | 24 |
| H | ? | list.rs | 28 |
| H | ? | list.rs | 93 |
| H | ? | list.rs | 94 |
| H | ? | list.rs | 102 |
| H | ? | list.rs | 107 |
| H | ? | list.rs | 252 |
| H | ? | list.rs | 323 |
| H | ? | list.rs | 415 |
| H | ? | list.rs | 484 |
| H | ? | list.rs | 490 |
| H | ? | list.rs | 581 |
| H | ? | list.rs | 582 |
| H | ? | list.rs | 682 |
| H | ? | list.rs | 683 |
| H | ? | list.rs | 824 |
| H | ? | list.rs | 874 |
| H | ? | list.rs | 881 |
| H | ? | list.rs | 903 |
| H | ? | list.rs | 936 |
| H | ? | list.rs | 937 |
| H | ? | fixed_size_list.rs | 8 |
| H | ? | fixed_size_list.rs | 12 |
| H | ? | fixed_size_list.rs | 16 |
| H | ? | fixed_size_list.rs | 20 |
| H | ? | fixed_size_list.rs | 24 |
| H | ? | fixed_size_list.rs | 61 |
| H | ? | fixed_size_list.rs | 237 |
| H | ? | fixed_size_list.rs | 238 |
| H | ? | fixed_size_list.rs | 257 |
| H | ? | fixed_size_list.rs | 291 |
| H | ? | fixed_size_list.rs | 318 |
| H | ? | fixed_size_list.rs | 326 |
| H | ? | fixed_size_list.rs | 401 |
| H | ? | fixed_size_list.rs | 447 |
| H | ? | fixed_size_list.rs | 453 |
| H | ? | fixed_size_list.rs | 617 |
| H | ? | fixed_size_list.rs | 734 |
| H | ? | fixed_size_list.rs | 735 |
| H | ? | fixed_size_list.rs | 812 |
| H | ? | builder.rs | 182 |
| H | ? | extend.rs | 11 |
| H | ? | extend.rs | 17 |
| H | ? | null.rs | 26 |
| H | ? | null.rs | 37 |
| H | ? | null.rs | 55 |
| H | ? | null.rs | 75 |
| H | ? | null.rs | 98 |
| H | ? | reshape.rs | 24 |
| H | ? | reshape.rs | 27 |
| H | ? | reshape.rs | 34 |
| H | ? | reshape.rs | 37 |
| H | ? | reshape.rs | 40 |
| H | ? | reshape.rs | 67 |
| H | ? | reshape.rs | 70 |
| H | ? | reshape.rs | 72 |
| H | ? | reshape.rs | 87 |
| H | ? | reshape.rs | 94 |
| H | ? | reshape.rs | 99 |
| H | ? | reshape.rs | 100 |
| H | ? | reshape.rs | 142 |
| H | ? | reshape.rs | 143 |
| H | ? | reshape.rs | 164 |
| H | ? | reshape.rs | 170 |
| H | ? | reshape.rs | 193 |
| H | ? | reshape.rs | 194 |
| H | ? | reshape.rs | 206 |
| H | ? | reshape.rs | 221 |
| H | ? | reshape.rs | 254 |
| H | ? | reshape.rs | 294 |
| H | ? | reshape.rs | 320 |
| H | ? | iceberg.rs | 87 |
| H | ? | iceberg.rs | 98 |
| H | ? | iceberg.rs | 150 |
| H | ? | iceberg.rs | 185 |
| H | ? | iceberg.rs | 203 |
| H | ? | mod.rs | 37 |
| H | ? | mod.rs | 49 |
| H | ? | mod.rs | 61 |
| H | ? | mod.rs | 69 |
| H | ? | mod.rs | 70 |
| H | ? | mod.rs | 82 |
| H | ? | mod.rs | 105 |
| H | ? | field.rs | 131 |
| H | ? | field.rs | 136 |
| H | ? | field.rs | 196 |
| H | ? | field.rs | 320 |
| H | ? | dtype.rs | 521 |
| H | ? | dtype.rs | 527 |
| H | ? | dtype.rs | 537 |
| H | ? | dtype.rs | 1182 |
| H | ? | dtype.rs | 1350 |
| H | ? | dtype.rs | 1355 |
| H | ? | dtype.rs | 1367 |
| H | ? | dtype.rs | 1377 |
| H | ? | dtype.rs | 1390 |
| H | ? | dtype.rs | 1397 |
| H | ? | dtype.rs | 1404 |
| H | ? | dtype.rs | 1411 |
| H | ? | dtype.rs | 1551 |
| H | ? | dtype.rs | 1575 |
| H | ? | dtype.rs | 1634 |
| H | ? | any_value.rs | 175 |
| H | ? | any_value.rs | 186 |
| H | ? | any_value.rs | 198 |
| H | ? | any_value.rs | 210 |
| H | ? | any_value.rs | 218 |
| H | ? | any_value.rs | 262 |
| H | ? | any_value.rs | 272 |
| H | ? | any_value.rs | 274 |
| H | ? | any_value.rs | 278 |
| H | ? | any_value.rs | 464 |
| H | ? | any_value.rs | 468 |
| H | ? | any_value.rs | 478 |
| H | ? | any_value.rs | 482 |
| H | ? | any_value.rs | 500 |
| H | ? | any_value.rs | 505 |
| H | ? | any_value.rs | 510 |
| H | ? | any_value.rs | 515 |
| H | ? | any_value.rs | 520 |
| H | ? | any_value.rs | 651 |
| H | ? | any_value.rs | 850 |
| H | ? | any_value.rs | 856 |
| H | ? | any_value.rs | 1019 |
| H | ? | any_value.rs | 1020 |
| H | ? | any_value.rs | 1063 |
| H | ? | any_value.rs | 1089 |
| H | ? | any_value.rs | 1127 |
| H | ? | any_value.rs | 1131 |
| H | ? | proptest.rs | 107 |
| H | ? | proptest.rs | 113 |
| H | ? | proptest.rs | 117 |
| H | ? | proptest.rs | 127 |
| H | ? | proptest.rs | 133 |
| H | ? | proptest.rs | 174 |
| H | ? | proptest.rs | 237 |
| H | ? | proptest.rs | 369 |
| H | ? | proptest.rs | 372 |
| H | ? | proptest.rs | 386 |
| H | ? | proptest.rs | 390 |
| H | ? | proptest.rs | 394 |
| H | ? | proptest.rs | 398 |
| H | ? | proptest.rs | 402 |
| H | ? | proptest.rs | 406 |
| H | ? | proptest.rs | 412 |
| H | ? | proptest.rs | 418 |
| H | ? | proptest.rs | 423 |
| H | ? | proptest.rs | 635 |
| H | ? | proptest.rs | 636 |
| H | ? | proptest.rs | 648 |
| H | ? | proptest.rs | 649 |
| H | ? | proptest.rs | 672 |
| H | ? | generic.rs | 33 |
| H | ? | generic.rs | 34 |
| H | ? | _serde.rs | 129 |
| H | ? | _serde.rs | 138 |
| H | ? | _serde.rs | 149 |
| H | ? | _serde.rs | 216 |
| H | ? | mod.rs | 15 |
| H | ? | mod.rs | 22 |
| H | ? | mod.rs | 35 |
| H | ? | mod.rs | 45 |
| H | ? | series.rs | 12 |
| H | ? | chunked_array.rs | 11 |
| H | ? | df.rs | 163 |
| H | ? | fmt.rs | 642 |
| H | ? | fmt.rs | 688 |
| H | ? | mod.rs | 170 |
| H | ? | mod.rs | 218 |
| H | ? | mod.rs | 242 |
| H | ? | mod.rs | 264 |
| H | ? | mod.rs | 327 |
| H | ? | mod.rs | 655 |
| H | ? | mod.rs | 913 |
| H | ? | mod.rs | 928 |
| H | ? | mod.rs | 1358 |
| H | ? | mod.rs | 1360 |
| H | ? | mod.rs | 1363 |
| H | ? | mod.rs | 1370 |
| H | ? | mod.rs | 1403 |
| H | ? | supertype.rs | 156 |
| H | ? | supertype.rs | 332 |
| H | ? | supertype.rs | 349 |
| H | ? | supertype.rs | 385 |
| H | ? | supertype.rs | 392 |
| H | ? | supertype.rs | 413 |
| H | ? | supertype.rs | 454 |
| H | ? | supertype.rs | 492 |
| H | ? | supertype.rs | 498 |
| H | ? | supertype.rs | 507 |
| H | ? | supertype.rs | 510 |
| H | ? | supertype.rs | 583 |
| H | ? | supertype.rs | 587 |
| H | ? | supertype.rs | 595 |
| H | ? | supertype.rs | 611 |
| H | ? | supertype.rs | 687 |
| H | ? | flatten.rs | 20 |
| H | ? | flatten.rs | 41 |
| H | ? | mod.rs | 274 |
| H | ? | mod.rs | 385 |
| H | ? | mod.rs | 399 |
| H | ? | mod.rs | 435 |
| H | ? | mod.rs | 503 |
| H | ? | mod.rs | 512 |
| H | ? | mod.rs | 527 |
| H | ? | mod.rs | 629 |
| H | ? | mod.rs | 654 |
| H | ? | mod.rs | 661 |
| H | ? | mod.rs | 687 |
| H | ? | mod.rs | 750 |
| H | ? | mod.rs | 764 |
| H | ? | mod.rs | 785 |
| H | ? | mod.rs | 805 |
| H | ? | mod.rs | 817 |
| H | ? | mod.rs | 828 |
| H | ? | mod.rs | 829 |
| H | ? | mod.rs | 872 |
| H | ? | mod.rs | 999 |
| H | ? | mod.rs | 1000 |
| H | ? | mod.rs | 1001 |
| H | ? | registry.rs | 91 |
| H | ? | registry.rs | 105 |
| H | ? | registry.rs | 151 |
| H | ? | registry.rs | 163 |
| H | ? | registry.rs | 169 |
| H | ? | registry.rs | 174 |
| H | ? | registry.rs | 183 |
| H | ? | mod.rs | 67 |
| H | ? | mod.rs | 213 |
| H | ? | mod.rs | 217 |
| H | ? | mod.rs | 242 |
| H | ? | mod.rs | 247 |
| H | ? | iterator.rs | 134 |
| H | ? | polars_extension.rs | 68 |
| H | ? | polars_extension.rs | 74 |
| H | ? | drop.rs | 45 |
| H | ? | list.rs | 64 |
| H | ? | list.rs | 74 |
| H | ? | list.rs | 83 |
| H | ? | builder.rs | 50 |
| H | ? | builder.rs | 183 |
| H | ? | builder.rs | 291 |
| H | ? | builder.rs | 312 |
| H | ? | builder.rs | 327 |
| H | ? | binary.rs | 62 |
| H | ? | string.rs | 11 |
| H | ? | string.rs | 12 |
| H | ? | null.rs | 30 |
| H | ? | fixed_size_list.rs | 86 |
| H | ? | fixed_size_list.rs | 88 |
| H | ? | fixed_size_list.rs | 137 |
| H | ? | fixed_size_list.rs | 153 |
| H | ? | fixed_size_list.rs | 161 |
| H | ? | categorical.rs | 21 |
| H | ? | mod.rs | 48 |
| H | ? | mod.rs | 104 |
| H | ? | mod.rs | 110 |
| H | ? | mod.rs | 116 |
| H | ? | mod.rs | 125 |
| H | ? | mod.rs | 135 |
| H | ? | null.rs | 44 |
| H | ? | anonymous.rs | 19 |
| H | ? | anonymous.rs | 25 |
| H | ? | mod.rs | 74 |
| H | ? | mod.rs | 87 |
| H | ? | mod.rs | 119 |
| H | ? | mod.rs | 132 |
| H | ? | mod.rs | 139 |
| H | ? | mod.rs | 143 |
| H | ? | mod.rs | 160 |
| H | ? | mod.rs | 161 |
| H | ? | mod.rs | 173 |
| H | ? | mod.rs | 175 |
| H | ? | mod.rs | 180 |
| H | ? | mod.rs | 182 |
| H | ? | iterator.rs | 63 |
| H | ? | iterator.rs | 69 |
| H | ? | iterator.rs | 78 |
| H | ? | iterator.rs | 89 |
| H | ? | iterator.rs | 90 |
| H | ? | iterator.rs | 94 |
| H | ? | iterator.rs | 114 |
| H | ? | iterator.rs | 131 |
| H | ? | iterator.rs | 140 |
| H | ? | iterator.rs | 152 |
| H | ? | iterator.rs | 163 |
| H | ? | iterator.rs | 181 |
| H | ? | iterator.rs | 189 |
| H | ? | iterator.rs | 200 |
| H | ? | iterator.rs | 213 |
| H | ? | iterator.rs | 228 |
| H | ? | iterator.rs | 230 |
| H | ? | cast.rs | 109 |
| H | ? | cast.rs | 145 |
| H | ? | cast.rs | 150 |
| H | ? | cast.rs | 165 |
| H | ? | cast.rs | 166 |
| H | ? | cast.rs | 189 |
| H | ? | cast.rs | 209 |
| H | ? | cast.rs | 215 |
| H | ? | cast.rs | 217 |
| H | ? | cast.rs | 260 |
| H | ? | cast.rs | 274 |
| H | ? | cast.rs | 289 |
| H | ? | cast.rs | 296 |
| H | ? | cast.rs | 301 |
| H | ? | cast.rs | 308 |
| H | ? | cast.rs | 316 |
| H | ? | cast.rs | 322 |
| H | ? | cast.rs | 332 |
| H | ? | cast.rs | 335 |
| H | ? | cast.rs | 340 |
| H | ? | cast.rs | 343 |
| H | ? | cast.rs | 360 |
| H | ? | cast.rs | 376 |
| H | ? | cast.rs | 391 |
| H | ? | cast.rs | 393 |
| H | ? | cast.rs | 410 |
| H | ? | cast.rs | 412 |
| H | ? | cast.rs | 426 |
| H | ? | cast.rs | 432 |
| H | ? | cast.rs | 469 |
| H | ? | cast.rs | 487 |
| H | ? | cast.rs | 489 |
| H | ? | cast.rs | 506 |
| H | ? | cast.rs | 564 |
| H | ? | cast.rs | 580 |
| H | ? | cast.rs | 582 |
| H | ? | cast.rs | 616 |
| H | ? | cast.rs | 622 |
| H | ? | cast.rs | 625 |
| H | ? | cast.rs | 627 |
| H | ? | cast.rs | 630 |
| H | ? | cast.rs | 645 |
| H | ? | cast.rs | 650 |
| H | ? | cast.rs | 652 |
| H | ? | cast.rs | 655 |
| H | ? | cast.rs | 660 |
| H | ? | cast.rs | 662 |
| H | ? | cast.rs | 681 |
| H | ? | cast.rs | 687 |
| H | ? | cast.rs | 690 |
| H | ? | cast.rs | 692 |
| H | ? | cast.rs | 731 |
| H | ? | from.rs | 67 |
| H | ? | from.rs | 128 |
| H | ? | duration.rs | 47 |
| H | ? | mod.rs | 46 |
| H | ? | mod.rs | 47 |
| H | ? | mod.rs | 136 |
| H | ? | mod.rs | 137 |
| H | ? | mod.rs | 144 |
| H | ? | mod.rs | 150 |
| H | ? | date.rs | 32 |
| H | ? | date.rs | 45 |
| H | ? | datetime.rs | 57 |
| H | ? | datetime.rs | 64 |
| H | ? | time.rs | 31 |
| H | ? | time.rs | 42 |
| H | ? | time.rs | 72 |
| H | ? | extension.rs | 16 |
| H | ? | extension.rs | 29 |
| H | ? | categorical.rs | 210 |
| H | ? | categorical.rs | 216 |
| H | ? | categorical.rs | 243 |
| H | ? | categorical.rs | 252 |
| H | ? | categorical.rs | 273 |
| H | ? | categorical.rs | 274 |
| H | ? | categorical.rs | 280 |
| H | ? | categorical.rs | 291 |
| H | ? | categorical.rs | 292 |
| H | ? | categorical.rs | 308 |
| H | ? | decimal.rs | 91 |
| H | ? | decimal.rs | 92 |
| H | ? | decimal.rs | 97 |
| H | ? | decimal.rs | 140 |
| H | ? | decimal.rs | 151 |
| H | ? | decimal.rs | 164 |
| H | ? | decimal.rs | 186 |
| H | ? | mod.rs | 37 |
| H | ? | mod.rs | 42 |
| H | ? | mod.rs | 43 |
| H | ? | mod.rs | 49 |
| H | ? | mod.rs | 50 |
| H | ? | mod.rs | 58 |
| H | ? | mod.rs | 92 |
| H | ? | mod.rs | 128 |
| H | ? | mod.rs | 162 |
| H | ? | mod.rs | 193 |
| H | ? | mod.rs | 217 |
| H | ? | mod.rs | 223 |
| H | ? | mod.rs | 253 |
| H | ? | mod.rs | 261 |
| H | ? | mod.rs | 269 |
| H | ? | mod.rs | 315 |
| H | ? | mod.rs | 326 |
| H | ? | mod.rs | 360 |
| H | ? | mod.rs | 388 |
| H | ? | mod.rs | 393 |
| H | ? | mod.rs | 395 |
| H | ? | bitwise.rs | 73 |
| H | ? | bitwise.rs | 75 |
| H | ? | bitwise.rs | 76 |
| H | ? | bitwise.rs | 84 |
| H | ? | bitwise.rs | 85 |
| H | ? | bitwise.rs | 117 |
| H | ? | bitwise.rs | 118 |
| H | ? | bitwise.rs | 149 |
| H | ? | bitwise.rs | 150 |
| H | ? | bitwise.rs | 156 |
| H | ? | bitwise.rs | 157 |
| H | ? | mod.rs | 201 |
| H | ? | mod.rs | 205 |
| H | ? | mod.rs | 209 |
| H | ? | mod.rs | 213 |
| H | ? | mod.rs | 221 |
| H | ? | mod.rs | 225 |
| H | ? | mod.rs | 229 |
| H | ? | mod.rs | 233 |
| H | ? | mod.rs | 1021 |
| H | ? | mod.rs | 1321 |
| H | ? | categorical.rs | 40 |
| H | ? | categorical.rs | 48 |
| H | ? | categorical.rs | 52 |
| H | ? | categorical.rs | 60 |
| H | ? | categorical.rs | 72 |
| H | ? | categorical.rs | 97 |
| H | ? | categorical.rs | 107 |
| H | ? | categorical.rs | 108 |
| H | ? | categorical.rs | 109 |
| H | ? | categorical.rs | 115 |
| H | ? | categorical.rs | 122 |
| H | ? | categorical.rs | 141 |
| H | ? | categorical.rs | 147 |
| H | ? | categorical.rs | 152 |
| H | ? | categorical.rs | 163 |
| H | ? | categorical.rs | 180 |
| H | ? | categorical.rs | 186 |
| H | ? | categorical.rs | 198 |
| H | ? | categorical.rs | 213 |
| H | ? | categorical.rs | 232 |
| H | ? | categorical.rs | 234 |
| H | ? | categorical.rs | 256 |
| H | ? | categorical.rs | 272 |
| H | ? | scalar.rs | 73 |
| H | ? | mod.rs | 79 |
| H | ? | mod.rs | 94 |
| H | ? | mod.rs | 140 |
| H | ? | numeric.rs | 260 |
| H | ? | numeric.rs | 264 |
| H | ? | numeric.rs | 271 |
| H | ? | numeric.rs | 272 |
| H | ? | numeric.rs | 273 |
| H | ? | numeric.rs | 281 |
| H | ? | numeric.rs | 282 |
| H | ? | numeric.rs | 283 |
| H | ? | numeric.rs | 291 |
| H | ? | numeric.rs | 292 |
| H | ? | numeric.rs | 293 |
| H | ? | numeric.rs | 301 |
| H | ? | numeric.rs | 302 |
| H | ? | numeric.rs | 303 |
| H | ? | numeric.rs | 311 |
| H | ? | numeric.rs | 312 |
| H | ? | numeric.rs | 313 |
| H | ? | numeric.rs | 321 |
| H | ? | numeric.rs | 322 |
| H | ? | numeric.rs | 323 |
| H | ? | numeric.rs | 329 |
| H | ? | numeric.rs | 335 |
| H | ? | numeric.rs | 341 |
| H | ? | numeric.rs | 347 |
| H | ? | numeric.rs | 353 |
| H | ? | numeric.rs | 359 |
| H | ? | numeric.rs | 365 |
| H | ? | numeric.rs | 371 |
| H | ? | numeric.rs | 377 |
| H | ? | numeric.rs | 383 |
| H | ? | numeric.rs | 389 |
| H | ? | numeric.rs | 397 |
| H | ? | numeric.rs | 398 |
| H | ? | numeric.rs | 399 |
| H | ? | numeric.rs | 404 |
| H | ? | numeric.rs | 409 |
| H | ? | numeric.rs | 417 |
| H | ? | numeric.rs | 418 |
| H | ? | numeric.rs | 419 |
| H | ? | numeric.rs | 425 |
| H | ? | numeric.rs | 431 |
| H | ? | from_iterator_par.rs | 166 |
| H | ? | mod.rs | 68 |
| H | ? | mod.rs | 71 |
| H | ? | mod.rs | 79 |
| H | ? | mod.rs | 117 |
| H | ? | mod.rs | 120 |
| H | ? | mod.rs | 128 |
| H | ? | mod.rs | 135 |
| H | ? | mod.rs | 139 |
| H | ? | mod.rs | 160 |
| H | ? | mod.rs | 161 |
| H | ? | mod.rs | 173 |
| H | ? | mod.rs | 175 |
| H | ? | mod.rs | 178 |
| H | ? | mod.rs | 186 |
| H | ? | mod.rs | 188 |
| H | ? | mod.rs | 207 |
| H | ? | mod.rs | 223 |
| H | ? | mod.rs | 231 |
| H | ? | mod.rs | 232 |
| H | ? | mod.rs | 243 |
| H | ? | iterator.rs | 53 |
| H | ? | iterator.rs | 62 |
| H | ? | iterator.rs | 71 |
| H | ? | iterator.rs | 94 |
| H | ? | iterator.rs | 146 |
| H | ? | iterator.rs | 152 |
| H | ? | iterator.rs | 161 |
| H | ? | iterator.rs | 175 |
| H | ? | iterator.rs | 187 |
| H | ? | iterator.rs | 205 |
| H | ? | iterator.rs | 227 |
| H | ? | iterator.rs | 251 |
| H | ? | iterator.rs | 274 |
| H | ? | iterator.rs | 297 |
| H | ? | iterator.rs | 320 |
| H | ? | iterator.rs | 337 |
| H | ? | iterator.rs | 359 |
| H | ? | iterator.rs | 376 |
| H | ? | iterator.rs | 390 |
| H | ? | iterator.rs | 404 |
| H | ? | iterator.rs | 424 |
| H | ? | iterator.rs | 440 |
| H | ? | iterator.rs | 456 |
| H | ? | iterator.rs | 468 |
| H | ? | iterator.rs | 470 |
| H | ? | float.rs | 42 |
| H | ? | duration.rs | 19 |
| H | ? | duration.rs | 77 |
| H | ? | duration.rs | 89 |
| H | ? | datetime.rs | 45 |
| H | ? | datetime.rs | 83 |
| H | ? | datetime.rs | 128 |
| H | ? | datetime.rs | 171 |
| H | ? | time.rs | 48 |
| H | ? | chunkops.rs | 30 |
| H | ? | chunkops.rs | 41 |
| H | ? | chunkops.rs | 225 |
| H | ? | chunkops.rs | 332 |
| H | ? | chunkops.rs | 337 |
| H | ? | chunkops.rs | 345 |
| H | ? | chunkops.rs | 352 |
| H | ? | explode.rs | 148 |
| H | ? | explode.rs | 190 |
| H | ? | explode.rs | 200 |
| H | ? | mod.rs | 511 |
| H | ? | mod.rs | 515 |
| H | ? | mod.rs | 516 |
| H | ? | mod.rs | 569 |
| H | ? | mod.rs | 570 |
| H | ? | mod.rs | 574 |
| H | ? | mod.rs | 586 |
| H | ? | mod.rs | 592 |
| H | ? | mod.rs | 594 |
| H | ? | mod.rs | 598 |
| H | ? | mod.rs | 612 |
| H | ? | mod.rs | 613 |
| H | ? | mod.rs | 617 |
| H | ? | mod.rs | 631 |
| H | ? | mod.rs | 632 |
| H | ? | bit_repr.rs | 16 |
| H | ? | bit_repr.rs | 21 |
| H | ? | bit_repr.rs | 34 |
| H | ? | bit_repr.rs | 44 |
| H | ? | bit_repr.rs | 53 |
| H | ? | bit_repr.rs | 62 |
| H | ? | bit_repr.rs | 71 |
| H | ? | bit_repr.rs | 84 |
| H | ? | extend.rs | 57 |
| H | ? | extend.rs | 128 |
| H | ? | extend.rs | 219 |
| H | ? | rolling_window.rs | 102 |
| H | ? | nulls.rs | 10 |
| H | ? | nulls.rs | 13 |
| H | ? | nulls.rs | 19 |
| H | ? | nulls.rs | 22 |
| H | ? | nulls.rs | 76 |
| H | ? | nulls.rs | 78 |
| H | ? | mod.rs | 132 |
| H | ? | mod.rs | 144 |
| H | ? | mod.rs | 150 |
| H | ? | mod.rs | 174 |
| H | ? | mod.rs | 182 |
| H | ? | mod.rs | 199 |
| H | ? | mod.rs | 239 |
| H | ? | mod.rs | 261 |
| H | ? | mod.rs | 272 |
| H | ? | mod.rs | 412 |
| H | ? | mod.rs | 460 |
| H | ? | mod.rs | 468 |
| H | ? | mod.rs | 531 |
| H | ? | mod.rs | 549 |
| H | ? | mod.rs | 568 |
| H | ? | mod.rs | 620 |
| H | ? | mod.rs | 627 |
| H | ? | mod.rs | 709 |
| H | ? | mod.rs | 710 |
| H | ? | mod.rs | 756 |
| H | ? | mod.rs | 784 |
| H | ? | mod.rs | 792 |
| H | ? | mod.rs | 866 |
| H | ? | categorical.rs | 12 |
| H | ? | categorical.rs | 53 |
| H | ? | categorical.rs | 57 |
| H | ? | categorical.rs | 78 |
| H | ? | append.rs | 13 |
| H | ? | append.rs | 182 |
| H | ? | append.rs | 187 |
| H | ? | append.rs | 209 |
| H | ? | append.rs | 214 |
| H | ? | append.rs | 235 |
| H | ? | append.rs | 240 |
| H | ? | append.rs | 275 |
| H | ? | full.rs | 114 |
| H | ? | full.rs | 155 |
| H | ? | full.rs | 174 |
| H | ? | full.rs | 182 |
| H | ? | full.rs | 214 |
| H | ? | full.rs | 237 |
| H | ? | reverse.rs | 18 |
| H | ? | reverse.rs | 35 |
| H | ? | reverse.rs | 38 |
| H | ? | reverse.rs | 51 |
| H | ? | reverse.rs | 54 |
| H | ? | reverse.rs | 66 |
| H | ? | reverse.rs | 68 |
| H | ? | reverse.rs | 75 |
| H | ? | reverse.rs | 77 |
| H | ? | reverse.rs | 107 |
| H | ? | set.rs | 60 |
| H | ? | set.rs | 77 |
| H | ? | set.rs | 92 |
| H | ? | set.rs | 115 |
| H | ? | set.rs | 176 |
| H | ? | set.rs | 199 |
| H | ? | set.rs | 230 |
| H | ? | set.rs | 247 |
| H | ? | set.rs | 262 |
| H | ? | set.rs | 293 |
| H | ? | set.rs | 310 |
| H | ? | filter.rs | 25 |
| H | ? | filter.rs | 54 |
| H | ? | filter.rs | 55 |
| H | ? | filter.rs | 60 |
| H | ? | filter.rs | 70 |
| H | ? | explode_and_offsets.rs | 17 |
| H | ? | explode_and_offsets.rs | 54 |
| H | ? | explode_and_offsets.rs | 68 |
| H | ? | explode_and_offsets.rs | 70 |
| H | ? | explode_and_offsets.rs | 92 |
| H | ? | explode_and_offsets.rs | 186 |
| H | ? | explode_and_offsets.rs | 261 |
| H | ? | explode_and_offsets.rs | 262 |
| H | ? | explode_and_offsets.rs | 276 |
| H | ? | explode_and_offsets.rs | 277 |
| H | ? | explode_and_offsets.rs | 326 |
| H | ? | mod.rs | 62 |
| H | ? | mod.rs | 408 |
| H | ? | mod.rs | 430 |
| H | ? | mod.rs | 451 |
| H | ? | mod.rs | 472 |
| H | ? | mod.rs | 608 |
| H | ? | mod.rs | 611 |
| H | ? | mod.rs | 612 |
| H | ? | mod.rs | 615 |
| H | ? | mod.rs | 620 |
| H | ? | mod.rs | 623 |
| H | ? | mod.rs | 624 |
| H | ? | mod.rs | 627 |
| H | ? | mod.rs | 710 |
| H | ? | mod.rs | 714 |
| H | ? | quantile.rs | 247 |
| H | ? | quantile.rs | 262 |
| H | ? | quantile.rs | 307 |
| H | ? | quantile.rs | 325 |
| H | ? | shift.rs | 17 |
| H | ? | shift.rs | 18 |
| H | ? | shift.rs | 26 |
| H | ? | shift.rs | 27 |
| H | ? | shift.rs | 62 |
| H | ? | shift.rs | 64 |
| H | ? | shift.rs | 98 |
| H | ? | shift.rs | 100 |
| H | ? | shift.rs | 137 |
| H | ? | shift.rs | 138 |
| H | ? | shift.rs | 171 |
| H | ? | shift.rs | 174 |
| H | ? | row_encode.rs | 108 |
| H | ? | row_encode.rs | 303 |
| H | ? | row_encode.rs | 314 |
| H | ? | mod.rs | 98 |
| H | ? | mod.rs | 122 |
| H | ? | mod.rs | 136 |
| H | ? | mod.rs | 226 |
| H | ? | mod.rs | 237 |
| H | ? | mod.rs | 245 |
| H | ? | mod.rs | 290 |
| H | ? | mod.rs | 298 |
| H | ? | mod.rs | 304 |
| H | ? | mod.rs | 356 |
| H | ? | mod.rs | 360 |
| H | ? | zip.rs | 26 |
| H | ? | zip.rs | 27 |
| H | ? | zip.rs | 31 |
| H | ? | zip.rs | 36 |
| H | ? | zip.rs | 60 |
| H | ? | zip.rs | 102 |
| H | ? | zip.rs | 103 |
| H | ? | zip.rs | 104 |
| H | ? | zip.rs | 131 |
| H | ? | zip.rs | 150 |
| H | ? | zip.rs | 161 |
| H | ? | zip.rs | 239 |
| H | ? | zip.rs | 242 |
| H | ? | zip.rs | 245 |
| H | ? | zip.rs | 246 |
| H | ? | zip.rs | 295 |
| H | ? | zip.rs | 349 |
| H | ? | zip.rs | 360 |
| H | ? | zip.rs | 424 |
| H | ? | arity.rs | 92 |
| H | ? | arity.rs | 104 |
| H | ? | arity.rs | 121 |
| H | ? | arity.rs | 126 |
| H | ? | arity.rs | 144 |
| H | ? | arity.rs | 160 |
| H | ? | arity.rs | 168 |
| H | ? | arity.rs | 187 |
| H | ? | arity.rs | 195 |
| H | ? | arity.rs | 213 |
| H | ? | arity.rs | 225 |
| H | ? | arity.rs | 240 |
| H | ? | arity.rs | 269 |
| H | ? | arity.rs | 346 |
| H | ? | arity.rs | 366 |
| H | ? | arity.rs | 385 |
| H | ? | arity.rs | 422 |
| H | ? | arity.rs | 515 |
| H | ? | arity.rs | 531 |
| H | ? | arity.rs | 559 |
| H | ? | arity.rs | 606 |
| H | ? | arity.rs | 625 |
| H | ? | arity.rs | 644 |
| H | ? | arity.rs | 714 |
| H | ? | arity.rs | 755 |
| H | ? | arity.rs | 775 |
| H | ? | arity.rs | 779 |
| H | ? | arity.rs | 800 |
| H | ? | arity.rs | 804 |
| H | ? | arity.rs | 828 |
| H | ? | arity.rs | 834 |
| H | ? | arity.rs | 838 |
| H | ? | arity.rs | 871 |
| H | ? | arity.rs | 873 |
| H | ? | arity.rs | 884 |
| H | ? | arity.rs | 886 |
| H | ? | arity.rs | 891 |
| H | ? | arity.rs | 921 |
| H | ? | arity.rs | 923 |
| H | ? | arity.rs | 934 |
| H | ? | arity.rs | 936 |
| H | ? | apply.rs | 41 |
| H | ? | apply.rs | 68 |
| H | ? | apply.rs | 91 |
| H | ? | apply.rs | 116 |
| H | ? | apply.rs | 131 |
| H | ? | apply.rs | 176 |
| H | ? | apply.rs | 178 |
| H | ? | apply.rs | 188 |
| H | ? | apply.rs | 225 |
| H | ? | apply.rs | 236 |
| H | ? | apply.rs | 273 |
| H | ? | apply.rs | 320 |
| H | ? | apply.rs | 334 |
| H | ? | apply.rs | 413 |
| H | ? | apply.rs | 421 |
| H | ? | apply.rs | 440 |
| H | ? | apply.rs | 454 |
| H | ? | apply.rs | 468 |
| H | ? | apply.rs | 481 |
| H | ? | apply.rs | 507 |
| H | ? | apply.rs | 546 |
| H | ? | apply.rs | 555 |
| H | ? | apply.rs | 581 |
| H | ? | nesting_utils.rs | 63 |
| H | ? | nesting_utils.rs | 104 |
| H | ? | nesting_utils.rs | 168 |
| H | ? | nesting_utils.rs | 211 |
| H | ? | nesting_utils.rs | 274 |
| H | ? | nesting_utils.rs | 320 |
| H | ? | gather.rs | 124 |
| H | ? | gather.rs | 253 |
| H | ? | gather.rs | 289 |
| H | ? | fill_null.rs | 72 |
| H | ? | fill_null.rs | 230 |
| H | ? | fill_null.rs | 239 |
| H | ? | vector_hasher.rs | 251 |
| H | ? | vector_hasher.rs | 304 |
| H | ? | vector_hasher.rs | 489 |
| H | ? | vector_hasher.rs | 518 |
| H | ? | vector_hasher.rs | 521 |
| H | ? | explode.rs | 67 |
| H | ? | explode.rs | 147 |
| H | ? | explode.rs | 296 |
| H | ? | explode.rs | 300 |
| H | ? | explode.rs | 320 |
| H | ? | explode.rs | 322 |
| H | ? | dataframe.rs | 199 |
| H | ? | dataframe.rs | 300 |
| H | ? | mod.rs | 172 |
| H | ? | mod.rs | 390 |
| H | ? | mod.rs | 438 |
| H | ? | mod.rs | 563 |
| H | ? | mod.rs | 661 |
| H | ? | mod.rs | 823 |
| H | ? | mod.rs | 859 |
| H | ? | mod.rs | 879 |
| H | ? | mod.rs | 884 |
| H | ? | mod.rs | 1174 |
| H | ? | mod.rs | 1194 |
| H | ? | mod.rs | 1269 |
| H | ? | mod.rs | 1321 |
| H | ? | mod.rs | 1376 |
| H | ? | mod.rs | 1393 |
| H | ? | mod.rs | 1438 |
| H | ? | mod.rs | 1461 |
| H | ? | mod.rs | 1472 |
| H | ? | mod.rs | 1511 |
| H | ? | mod.rs | 1520 |
| H | ? | mod.rs | 1588 |
| H | ? | mod.rs | 1652 |
| H | ? | mod.rs | 1819 |
| H | ? | mod.rs | 1896 |
| H | ? | mod.rs | 1989 |
| H | ? | mod.rs | 2028 |
| H | ? | mod.rs | 2037 |
| H | ? | mod.rs | 2335 |
| H | ? | mod.rs | 2453 |
| H | ? | mod.rs | 2478 |
| H | ? | mod.rs | 2539 |
| H | ? | mod.rs | 2551 |
| H | ? | mod.rs | 2645 |
| H | ? | mod.rs | 2659 |
| H | ? | mod.rs | 2729 |
| H | ? | mod.rs | 2754 |
| H | ? | mod.rs | 3036 |
| H | ? | mod.rs | 65 |
| H | ? | mod.rs | 748 |
| H | ? | mod.rs | 757 |
| H | ? | mod.rs | 805 |
| H | ? | string.rs | 26 |
| H | ? | string.rs | 29 |
| H | ? | string.rs | 89 |
| H | ? | string.rs | 91 |
| H | ? | string.rs | 151 |
| H | ? | string.rs | 154 |
| H | ? | string.rs | 206 |
| H | ? | string.rs | 209 |
| H | ? | mod.rs | 311 |
| H | ? | mod.rs | 491 |
| H | ? | mod.rs | 494 |
| H | ? | mod.rs | 569 |
| H | ? | mod.rs | 572 |
| H | ? | mod.rs | 677 |
| H | ? | mod.rs | 679 |
| H | ? | mod.rs | 754 |
| H | ? | mod.rs | 757 |
| H | ? | agg_list.rs | 85 |
| H | ? | agg_list.rs | 147 |
| H | ? | agg_list.rs | 161 |
| H | ? | agg_list.rs | 168 |
| H | ? | agg_list.rs | 245 |
| H | ? | agg_list.rs | 260 |
| H | ? | agg_list.rs | 268 |
| H | ? | agg_list.rs | 279 |
| H | ? | agg_list.rs | 284 |
| H | ? | agg_list.rs | 289 |
| H | ? | agg_list.rs | 290 |
| H | ? | agg_list.rs | 293 |
| H | ? | agg_list.rs | 296 |
| H | ? | agg_list.rs | 317 |
| H | ? | agg_list.rs | 320 |
| H | ? | agg_list.rs | 321 |
| H | ? | agg_list.rs | 324 |
| H | ? | agg_list.rs | 327 |
| H | ? | categorical.rs | 67 |
| H | ? | categorical.rs | 133 |
| H | ? | boolean.rs | 82 |
| H | ? | boolean.rs | 85 |
| H | ? | boolean.rs | 128 |
| H | ? | boolean.rs | 130 |
| H | ? | boolean.rs | 176 |
| H | ? | boolean.rs | 179 |
| H | ? | boolean.rs | 225 |
| H | ? | boolean.rs | 228 |
| H | ? | boolean.rs | 292 |
| H | ? | dispatch.rs | 62 |
| H | ? | dispatch.rs | 103 |
| H | ? | dispatch.rs | 302 |
| H | ? | dispatch.rs | 358 |
| H | ? | dispatch.rs | 365 |
| H | ? | dispatch.rs | 366 |
| H | ? | dispatch.rs | 367 |
| H | ? | dispatch.rs | 414 |
| H | ? | dispatch.rs | 421 |
| H | ? | dispatch.rs | 422 |
| H | ? | dispatch.rs | 423 |
| H | ? | dispatch.rs | 477 |
| H | ? | dispatch.rs | 497 |
| H | ? | dispatch.rs | 535 |
| H | ? | dispatch.rs | 580 |
| H | ? | into_groups.rs | 329 |
| H | ? | into_groups.rs | 350 |
| H | ? | position.rs | 289 |
| H | ? | position.rs | 730 |
| H | ? | position.rs | 760 |
| H | ? | hashing.rs | 194 |
| H | ? | broadcast.rs | 25 |
| H | ? | chunks.rs | 21 |
| H | ? | chunks.rs | 85 |
| H | ? | top_k.rs | 22 |
| H | ? | mod.rs | 64 |
| H | ? | mod.rs | 117 |
| H | ? | mod.rs | 132 |
| H | ? | mod.rs | 204 |
| H | ? | mod.rs | 511 |
| H | ? | mod.rs | 518 |
| H | ? | mod.rs | 519 |
| H | ? | mod.rs | 538 |
| H | ? | mod.rs | 547 |
| H | ? | mod.rs | 663 |
| H | ? | mod.rs | 677 |
| H | ? | mod.rs | 678 |
| H | ? | mod.rs | 732 |
| H | ? | mod.rs | 733 |
| H | ? | mod.rs | 811 |
| H | ? | mod.rs | 829 |
| H | ? | mod.rs | 971 |
| H | ? | mod.rs | 988 |
| H | ? | mod.rs | 1065 |
| H | ? | mod.rs | 1071 |
| H | ? | mod.rs | 1198 |
| H | ? | mod.rs | 1212 |
| H | ? | mod.rs | 1243 |
| H | ? | mod.rs | 1244 |
| H | ? | mod.rs | 1248 |
| H | ? | mod.rs | 1331 |
| H | ? | mod.rs | 1344 |
| H | ? | mod.rs | 1379 |
| H | ? | mod.rs | 1385 |
| H | ? | mod.rs | 1445 |
| H | ? | mod.rs | 1446 |
| H | ? | mod.rs | 1698 |
| H | ? | scalar.rs | 93 |
| H | ? | scalar.rs | 132 |
| H | ? | scalar.rs | 145 |
| H | ? | scalar.rs | 146 |
| H | ? | scalar.rs | 164 |
| H | ? | scalar.rs | 165 |
| H | ? | scalar.rs | 173 |
| H | ? | scalar.rs | 181 |
| H | ? | scalar.rs | 182 |
| H | ? | scalar.rs | 208 |
| H | ? | scalar.rs | 213 |
| H | ? | scalar.rs | 214 |
| H | ? | scalar.rs | 227 |
| H | ? | scalar.rs | 256 |
| H | ? | scalar.rs | 261 |
| H | ? | scalar.rs | 262 |
| H | ? | scalar.rs | 274 |
| H | ? | scalar.rs | 284 |
| H | ? | scalar.rs | 299 |
| H | ? | scalar.rs | 310 |
| H | ? | scalar.rs | 377 |
| H | ? | scalar.rs | 378 |
| H | ? | scalar.rs | 391 |
| H | ? | from.rs | 20 |
| H | ? | arithmetic.rs | 12 |
| H | ? | arithmetic.rs | 154 |
| H | ? | dataframe.rs | 87 |
| H | ? | dataframe.rs | 89 |
| H | ? | dataframe.rs | 130 |
| H | ? | dataframe.rs | 132 |
| H | ? | mod.rs | 121 |
| H | ? | mod.rs | 133 |
| H | ? | transpose.rs | 85 |
| H | ? | transpose.rs | 260 |
| H | ? | av_buffer.rs | 158 |
| H | ? | av_buffer.rs | 172 |
| H | ? | av_buffer.rs | 177 |
| H | ? | av_buffer.rs | 182 |
| H | ? | av_buffer.rs | 187 |
| H | ? | av_buffer.rs | 192 |
| H | ? | av_buffer.rs | 198 |
| H | ? | av_buffer.rs | 204 |
| H | ? | av_buffer.rs | 207 |
| H | ? | av_buffer.rs | 215 |
| H | ? | av_buffer.rs | 221 |
| H | ? | av_buffer.rs | 226 |
| H | ? | av_buffer.rs | 231 |
| H | ? | av_buffer.rs | 236 |
| H | ? | av_buffer.rs | 242 |
| H | ? | av_buffer.rs | 248 |
| H | ? | av_buffer.rs | 254 |
| H | ? | av_buffer.rs | 260 |
| H | ? | av_buffer.rs | 265 |
| H | ? | av_buffer.rs | 314 |
| H | ? | av_buffer.rs | 331 |
| H | ? | av_buffer.rs | 523 |
| H | ? | av_buffer.rs | 566 |
| H | ? | av_buffer.rs | 579 |
| H | ? | av_buffer.rs | 584 |
| H | ? | av_buffer.rs | 589 |
| H | ? | av_buffer.rs | 594 |
| H | ? | av_buffer.rs | 599 |
| H | ? | av_buffer.rs | 604 |
| H | ? | av_buffer.rs | 609 |
| H | ? | av_buffer.rs | 614 |
| H | ? | av_buffer.rs | 620 |
| H | ? | av_buffer.rs | 626 |
| H | ? | av_buffer.rs | 632 |
| H | ? | av_buffer.rs | 638 |
| H | ? | av_buffer.rs | 663 |
| H | ? | av_buffer.rs | 678 |
| H | ? | av_buffer.rs | 751 |
| H | ? | av_buffer.rs | 757 |
| H | ? | builder.rs | 21 |
| H | ? | builder.rs | 42 |
| H | ? | builder.rs | 59 |
| H | ? | builder.rs | 104 |
| H | ? | builder.rs | 132 |
| H | ? | builder.rs | 161 |
| H | ? | builder.rs | 191 |
| H | ? | builder.rs | 215 |
| H | ? | tests.rs | 8 |
| H | ? | functions.rs | 22 |
| H | ? | functions.rs | 23 |
| H | ? | functions.rs | 37 |
| H | ? | functions.rs | 38 |
| H | ? | array.rs | 150 |
| H | ? | list.rs | 46 |
| H | ? | list.rs | 48 |
| H | ? | list.rs | 146 |
| H | ? | dictionary.rs | 27 |
| H | ? | dictionary.rs | 29 |
| H | ? | dictionary.rs | 56 |
| H | ? | dictionary.rs | 58 |
| H | ? | boolean.rs | 19 |
| H | ? | boolean.rs | 61 |
| H | ? | boolean.rs | 67 |
| H | ? | dyn_array.rs | 15 |
| H | ? | dyn_array.rs | 30 |
| H | ? | dyn_array.rs | 31 |
| H | ? | mod.rs | 101 |
| H | ? | mod.rs | 121 |
| H | ? | mod.rs | 122 |
| H | ? | mod.rs | 132 |
| H | ? | mod.rs | 134 |
| H | ? | mod.rs | 143 |
| H | ? | mod.rs | 145 |
| H | ? | mod.rs | 168 |
| H | ? | mod.rs | 237 |
| H | ? | mod.rs | 251 |
| H | ? | mod.rs | 419 |
| H | ? | mod.rs | 486 |
| H | ? | mod.rs | 513 |
| H | ? | mod.rs | 529 |
| H | ? | mod.rs | 577 |
| H | ? | mod.rs | 601 |
| H | ? | mod.rs | 602 |
| H | ? | mod.rs | 603 |
| H | ? | mod.rs | 604 |
| H | ? | mod.rs | 606 |
| H | ? | mod.rs | 607 |
| H | ? | mod.rs | 608 |
| H | ? | mod.rs | 609 |
| H | ? | mod.rs | 610 |
| H | ? | mod.rs | 612 |
| H | ? | mod.rs | 614 |
| H | ? | mod.rs | 615 |
| H | ? | mod.rs | 616 |
| H | ? | mod.rs | 618 |
| H | ? | mod.rs | 671 |
| H | ? | mod.rs | 681 |
| H | ? | mod.rs | 692 |
| H | ? | mod.rs | 717 |
| H | ? | mod.rs | 721 |
| H | ? | mod.rs | 731 |
| H | ? | mod.rs | 736 |
| H | ? | utf8_to.rs | 27 |
| H | ? | utf8_to.rs | 40 |
| H | ? | utf8_to.rs | 51 |
| H | ? | utf8_to.rs | 63 |
| H | ? | utf8_to.rs | 64 |
| H | ? | utf8_to.rs | 96 |
| H | ? | utf8_to.rs | 120 |
| H | ? | utf8_to.rs | 121 |
| H | ? | dictionary_to.rs | 19 |
| H | ? | dictionary_to.rs | 44 |
| H | ? | decimal_to.rs | 26 |
| H | ? | temporal.rs | 133 |
| H | ? | primitive_to.rs | 241 |
| H | ? | primitive_to.rs | 307 |
| H | ? | primitive_to.rs | 320 |
| H | ? | primitive_to.rs | 321 |
| H | ? | primitive_to.rs | 357 |
| H | ? | primitive_to.rs | 374 |
| H | ? | primitive_to.rs | 565 |
| H | ? | binary_to.rs | 74 |
| H | ? | binary_to.rs | 88 |
| H | ? | binary_to.rs | 105 |
| H | ? | binary_to.rs | 106 |
| H | ? | binary_to.rs | 121 |
| H | ? | binary_to.rs | 149 |
| H | ? | binary_to.rs | 182 |
| H | ? | binary_to.rs | 228 |
| H | ? | binary_to.rs | 262 |
| H | ? | binary_to.rs | 266 |
| H | ? | binview_to.rs | 64 |
| H | ? | binview_to.rs | 65 |
| H | ? | binview_to.rs | 84 |
| H | ? | binview_to.rs | 166 |
| H | ? | binview_to.rs | 252 |
| H | ? | view.rs | 53 |
| H | ? | view.rs | 90 |
| H | ? | view.rs | 128 |
| H | ? | view.rs | 166 |
| H | ? | array.rs | 13 |
| H | ? | array.rs | 30 |
| H | ? | array.rs | 33 |
| H | ? | array.rs | 50 |
| H | ? | array.rs | 53 |
| H | ? | array.rs | 73 |
| H | ? | array.rs | 75 |
| H | ? | array.rs | 77 |
| H | ? | list.rs | 12 |
| H | ? | list.rs | 29 |
| H | ? | list.rs | 31 |
| H | ? | list.rs | 48 |
| H | ? | list.rs | 50 |
| H | ? | list.rs | 70 |
| H | ? | list.rs | 72 |
| H | ? | list.rs | 74 |
| H | ? | boolean.rs | 55 |
| H | ? | propagate_nulls.rs | 28 |
| H | ? | propagate_nulls.rs | 98 |
| H | ? | propagate_nulls.rs | 99 |
| H | ? | propagate_nulls.rs | 101 |
| H | ? | propagate_nulls.rs | 108 |
| H | ? | propagate_nulls.rs | 134 |
| H | ? | propagate_nulls.rs | 184 |
| H | ? | propagate_nulls.rs | 187 |
| H | ? | propagate_nulls.rs | 211 |
| H | ? | propagate_nulls.rs | 225 |
| H | ? | propagate_nulls.rs | 250 |
| H | ? | propagate_nulls.rs | 259 |
| H | ? | propagate_nulls.rs | 263 |
| H | ? | propagate_nulls.rs | 266 |
| H | ? | mod.rs | 34 |
| H | ? | mod.rs | 40 |
| H | ? | mod.rs | 50 |
| H | ? | mod.rs | 64 |
| H | ? | mod.rs | 74 |
| H | ? | mod.rs | 82 |
| H | ? | mod.rs | 95 |
| H | ? | mod.rs | 109 |
| H | ? | mod.rs | 119 |
| H | ? | mod.rs | 184 |
| H | ? | struct_.rs | 31 |
| H | ? | struct_.rs | 50 |
| H | ? | struct_.rs | 67 |
| H | ? | struct_.rs | 74 |
| H | ? | moment.rs | 189 |
| H | ? | moment.rs | 197 |
| H | ? | rank.rs | 94 |
| H | ? | quantile.rs | 160 |
| H | ? | moment.rs | 177 |
| H | ? | moment.rs | 254 |
| H | ? | moment.rs | 302 |
| H | ? | moment.rs | 370 |
| H | ? | moment.rs | 439 |
| H | ? | moment.rs | 518 |
| H | ? | sum.rs | 89 |
| H | ? | sum.rs | 95 |
| H | ? | sum.rs | 115 |
| H | ? | sum.rs | 130 |
| H | ? | mean.rs | 119 |
| H | ? | mean.rs | 130 |
| H | ? | mean.rs | 157 |
| H | ? | mean.rs | 171 |
| H | ? | mean.rs | 185 |
| H | ? | mod.rs | 47 |
| H | ? | mod.rs | 52 |
| H | ? | mod.rs | 99 |
| H | ? | mod.rs | 117 |
| H | ? | mod.rs | 128 |
| H | ? | mod.rs | 141 |
| H | ? | mod.rs | 149 |
| H | ? | primitive.rs | 77 |
| H | ? | binary.rs | 31 |
| H | ? | list.rs | 143 |
| H | ? | structure.rs | 33 |
| H | ? | fixed_size_list.rs | 200 |
| H | ? | boolean.rs | 68 |
| H | ? | binview.rs | 16 |
| H | ? | binview.rs | 18 |
| H | ? | trim_lists_to_normalized_offsets.rs | 34 |
| H | ? | trim_lists_to_normalized_offsets.rs | 39 |
| H | ? | trim_lists_to_normalized_offsets.rs | 54 |
| H | ? | trim_lists_to_normalized_offsets.rs | 67 |
| H | ? | trim_lists_to_normalized_offsets.rs | 94 |
| H | ? | trim_lists_to_normalized_offsets.rs | 98 |
| H | ? | dictionary.rs | 47 |
| H | ? | boolean.rs | 166 |
| H | ? | boolean.rs | 167 |
| H | ? | boolean.rs | 168 |
| H | ? | mod.rs | 37 |
| H | ? | mod.rs | 48 |
| H | ? | mod.rs | 65 |
| H | ? | mod.rs | 74 |
| H | ? | mod.rs | 76 |
| H | ? | mod.rs | 92 |
| H | ? | boolean.rs | 69 |
| H | ? | propagate_dictionary.rs | 12 |
| H | ? | propagate_dictionary.rs | 15 |
| H | ? | signed.rs | 105 |
| H | ? | signed.rs | 144 |
| H | ? | signed.rs | 176 |
| H | ? | unsigned.rs | 88 |
| H | ? | unsigned.rs | 118 |
| H | ? | decimal.rs | 916 |
| H | ? | cache.rs | 16 |
| H | ? | cache.rs | 46 |
| H | ? | cache.rs | 47 |
| H | ? | cache.rs | 116 |
| H | ? | cache.rs | 120 |
| H | ? | cache.rs | 134 |
| H | ? | cache.rs | 138 |
| H | ? | cache.rs | 148 |
| H | ? | cache.rs | 150 |
| H | ? | cache.rs | 154 |
| H | ? | entry.rs | 68 |
| H | ? | entry.rs | 79 |
| H | ? | entry.rs | 103 |
| H | ? | entry.rs | 118 |
| H | ? | entry.rs | 130 |
| H | ? | entry.rs | 140 |
| H | ? | entry.rs | 204 |
| H | ? | entry.rs | 223 |
| H | ? | entry.rs | 266 |
| H | ? | entry.rs | 336 |
| H | ? | entry.rs | 343 |
| H | ? | eviction.rs | 299 |
| H | ? | utils.rs | 68 |
| H | ? | utils.rs | 86 |
| H | ? | utils.rs | 89 |
| H | ? | utils.rs | 93 |
| H | ? | utils.rs | 98 |
| H | ? | utils.rs | 101 |
| H | ? | utils.rs | 103 |
| H | ? | utils.rs | 106 |
| H | ? | utils.rs | 129 |
| H | ? | utils.rs | 130 |
| H | ? | cache_lock.rs | 27 |
| H | ? | cache_lock.rs | 29 |
| H | ? | cache_lock.rs | 118 |
| H | ? | cache_lock.rs | 144 |
| H | ? | cache_lock.rs | 205 |
| H | ? | cache_lock.rs | 234 |
| H | ? | glob.rs | 229 |
| H | ? | options.rs | 113 |
| H | ? | options.rs | 385 |
| H | ? | options.rs | 445 |
| H | ? | options.rs | 808 |
| H | ? | dns.rs | 174 |
| H | ? | dns.rs | 188 |
| H | ? | dns.rs | 217 |
| H | ? | dns.rs | 311 |
| H | ? | polars_object_store.rs | 32 |
| H | ? | polars_object_store.rs | 107 |
| H | ? | polars_object_store.rs | 139 |
| H | ? | polars_object_store.rs | 154 |
| H | ? | polars_object_store.rs | 164 |
| H | ? | polars_object_store.rs | 177 |
| H | ? | polars_object_store.rs | 219 |
| H | ? | polars_object_store.rs | 256 |
| H | ? | polars_object_store.rs | 273 |
| H | ? | polars_object_store.rs | 333 |
| H | ? | polars_object_store.rs | 360 |
| H | ? | polars_object_store.rs | 457 |
| H | ? | polars_object_store.rs | 640 |
| H | ? | polars_object_store.rs | 642 |
| H | ? | polars_object_store.rs | 683 |
| H | ? | object_store_setup.rs | 142 |
| H | ? | object_store_setup.rs | 244 |
| H | ? | object_store_setup.rs | 254 |
| H | ? | object_store_setup.rs | 266 |
| H | ? | object_store_setup.rs | 281 |
| H | ? | object_store_setup.rs | 353 |
| H | ? | object_store_setup.rs | 361 |
| H | ? | object_store_setup.rs | 384 |
| H | ? | object_store_setup.rs | 410 |
| H | ? | object_store_setup.rs | 475 |
| H | ? | object_store_setup.rs | 483 |
| H | ? | object_store_setup.rs | 499 |
| H | ? | object_store_setup.rs | 504 |
| H | ? | object_store_setup.rs | 508 |
| H | ? | object_store_setup.rs | 556 |
| H | ? | object_store_setup.rs | 571 |
| H | ? | object_store_setup.rs | 591 |
| H | ? | object_store_setup.rs | 594 |
| H | ? | object_store_setup.rs | 625 |
| H | ? | object_store_setup.rs | 629 |
| H | ? | object_store_setup.rs | 636 |
| H | ? | object_store_setup.rs | 658 |
| H | ? | multipart_upload.rs | 24 |
| H | ? | multipart_upload.rs | 33 |
| H | ? | internal_writer.rs | 97 |
| H | ? | internal_writer.rs | 117 |
| H | ? | mod.rs | 159 |
| H | ? | mod.rs | 160 |
| H | ? | mod.rs | 161 |
| H | ? | mod.rs | 162 |
| H | ? | admission.rs | 175 |
| H | ? | admission.rs | 184 |
| H | ? | credential_provider.rs | 504 |
| H | ? | credential_provider.rs | 629 |
| H | ? | credential_provider.rs | 707 |
| H | ? | credential_provider.rs | 814 |
| H | ? | key_value_metadata.rs | 96 |
| H | ? | writer.rs | 27 |
| H | ? | batched_writer.rs | 209 |
| H | ? | read_impl.rs | 117 |
| H | ? | read_impl.rs | 149 |
| H | ? | read_impl.rs | 224 |
| H | ? | read_impl.rs | 259 |
| H | ? | read_impl.rs | 367 |
| H | ? | read_impl.rs | 393 |
| H | ? | read_impl.rs | 463 |
| H | ? | mmap.rs | 47 |
| H | ? | reader.rs | 92 |
| H | ? | reader.rs | 138 |
| H | ? | reader.rs | 145 |
| H | ? | reader.rs | 205 |
| H | ? | reader.rs | 230 |
| H | ? | async_impl.rs | 95 |
| H | ? | utils.rs | 26 |
| H | ? | utils.rs | 55 |
| H | ? | mod.rs | 173 |
| H | ? | mod.rs | 290 |
| H | ? | mod.rs | 570 |
| H | ? | mod.rs | 638 |
| H | ? | mod.rs | 640 |
| H | ? | hugging_face.rs | 267 |
| H | ? | shared.rs | 66 |
| H | ? | shared.rs | 128 |
| H | ? | shared.rs | 129 |
| H | ? | predicates.rs | 86 |
| H | ? | predicates.rs | 104 |
| H | ? | predicates.rs | 231 |
| H | ? | predicates.rs | 287 |
| H | ? | predicates.rs | 373 |
| H | ? | predicates.rs | 374 |
| H | ? | predicates.rs | 378 |
| H | ? | predicates.rs | 379 |
| H | ? | predicates.rs | 431 |
| H | ? | predicates.rs | 434 |
| H | ? | predicates.rs | 435 |
| H | ? | predicates.rs | 445 |
| H | ? | predicates.rs | 448 |
| H | ? | predicates.rs | 449 |
| H | ? | predicates.rs | 483 |
| H | ? | predicates.rs | 492 |
| H | ? | predicates.rs | 493 |
| H | ? | predicates.rs | 508 |
| H | ? | predicates.rs | 516 |
| H | ? | hive.rs | 34 |
| H | ? | bytes_bufferer.rs | 45 |
| H | ? | bytes_bufferer.rs | 46 |
| H | ? | other.rs | 58 |
| H | ? | other.rs | 150 |
| H | ? | byte_source.rs | 61 |
| H | ? | byte_source.rs | 71 |
| H | ? | compression.rs | 202 |
| H | ? | compression.rs | 353 |
| H | ? | write_impl.rs | 29 |
| H | ? | write_impl.rs | 30 |
| H | ? | write_impl.rs | 31 |
| H | ? | write_impl.rs | 215 |
| H | ? | writer.rs | 63 |
| H | ? | writer.rs | 184 |
| H | ? | writer.rs | 224 |
| H | ? | options.rs | 127 |
| H | ? | schema_inference.rs | 227 |
| H | ? | schema_inference.rs | 241 |
| H | ? | schema_inference.rs | 255 |
| H | ? | parser.rs | 133 |
| H | ? | read_impl.rs | 76 |
| H | ? | read_impl.rs | 193 |
| H | ? | read_impl.rs | 198 |
| H | ? | read_impl.rs | 202 |
| H | ? | read_impl.rs | 205 |
| H | ? | read_impl.rs | 206 |
| H | ? | read_impl.rs | 209 |
| H | ? | read_impl.rs | 210 |
| H | ? | read_impl.rs | 212 |
| H | ? | read_impl.rs | 237 |
| H | ? | read_impl.rs | 247 |
| H | ? | read_impl.rs | 265 |
| H | ? | read_impl.rs | 338 |
| H | ? | read_impl.rs | 339 |
| H | ? | read_impl.rs | 348 |
| H | ? | read_impl.rs | 439 |
| H | ? | read_impl.rs | 490 |
| H | ? | streaming.rs | 141 |
| H | ? | streaming.rs | 165 |
| H | ? | streaming.rs | 322 |
| H | ? | streaming.rs | 346 |
| H | ? | streaming.rs | 427 |
| H | ? | streaming.rs | 432 |
| H | ? | streaming.rs | 434 |
| H | ? | streaming.rs | 460 |
| H | ? | streaming.rs | 560 |
| H | ? | streaming.rs | 565 |
| H | ? | streaming.rs | 567 |
| H | ? | streaming.rs | 593 |
| H | ? | streaming.rs | 802 |
| H | ? | streaming.rs | 807 |
| H | ? | streaming.rs | 818 |
| H | ? | streaming.rs | 827 |
| H | ? | reader.rs | 111 |
| H | ? | reader.rs | 115 |
| H | ? | reader.rs | 116 |
| H | ? | reader.rs | 118 |
| H | ? | reader.rs | 119 |
| H | ? | reader.rs | 120 |
| H | ? | reader.rs | 121 |
| H | ? | reader.rs | 123 |
| H | ? | reader.rs | 193 |
| H | ? | builder.rs | 577 |
| H | ? | builder.rs | 644 |
| H | ? | builder.rs | 656 |
| H | ? | builder.rs | 664 |
| H | ? | builder.rs | 672 |
| H | ? | builder.rs | 890 |
| H | ? | builder.rs | 892 |
| H | ? | builder.rs | 894 |
| H | ? | core.rs | 133 |
| H | ? | buffer.rs | 241 |
| H | ? | buffer.rs | 332 |
| H | ? | write.rs | 68 |
| H | ? | write.rs | 86 |
| H | ? | read.rs | 118 |
| H | ? | schema.rs | 58 |
| H | ? | schema.rs | 115 |
| H | ? | schema.rs | 251 |
| H | ? | schema.rs | 254 |
| H | ? | schema.rs | 471 |
| H | ? | mod.rs | 150 |
| H | ? | mod.rs | 195 |
| H | ? | mod.rs | 316 |
| H | ? | mod.rs | 317 |
| H | ? | mod.rs | 355 |
| H | ? | ipc_stream.rs | 123 |
| H | ? | ipc_stream.rs | 126 |
| H | ? | ipc_stream.rs | 180 |
| H | ? | ipc_stream.rs | 184 |
| H | ? | mmap.rs | 36 |
| H | ? | mmap.rs | 49 |
| H | ? | mmap.rs | 74 |
| H | ? | mmap.rs | 94 |
| H | ? | mmap.rs | 105 |
| H | ? | ipc_reader_async.rs | 75 |
| H | ? | ipc_reader_async.rs | 154 |
| H | ? | ipc_file.rs | 148 |
| H | ? | ipc_file.rs | 157 |
| H | ? | ipc_file.rs | 166 |
| H | ? | ipc_file.rs | 232 |
| H | ? | ipc_file.rs | 251 |
| H | ? | ipc_file.rs | 293 |
| H | ? | ipc_file.rs | 295 |
| H | ? | ipc_file.rs | 314 |
| H | ? | ipc_file.rs | 332 |
| H | ? | ipc_file.rs | 345 |
| H | ? | dynamic.rs | 128 |
| H | ? | dynamic.rs | 142 |
| H | ? | dynamic.rs | 213 |
| H | ? | dynamic.rs | 382 |
| H | ? | dynamic.rs | 383 |
| H | ? | dynamic.rs | 391 |
| H | ? | dynamic.rs | 395 |
| H | ? | dynamic.rs | 397 |
| H | ? | dynamic.rs | 401 |
| H | ? | dynamic.rs | 411 |
| H | ? | dynamic.rs | 412 |
| H | ? | dynamic.rs | 526 |
| H | ? | dynamic.rs | 573 |
| H | ? | mod.rs | 314 |
| H | ? | round.rs | 46 |
| H | ? | round.rs | 60 |
| H | ? | round.rs | 63 |
| H | ? | round.rs | 64 |
| H | ? | round.rs | 101 |
| H | ? | round.rs | 123 |
| H | ? | truncate.rs | 51 |
| H | ? | truncate.rs | 56 |
| H | ? | truncate.rs | 70 |
| H | ? | truncate.rs | 73 |
| H | ? | truncate.rs | 74 |
| H | ? | truncate.rs | 105 |
| H | ? | truncate.rs | 132 |
| H | ? | upsample.rs | 132 |
| H | ? | upsample.rs | 142 |
| H | ? | upsample.rs | 227 |
| H | ? | upsample.rs | 255 |
| H | ? | upsample.rs | 267 |
| H | ? | upsample.rs | 268 |
| H | ? | offset_by.rs | 27 |
| H | ? | offset_by.rs | 78 |
| H | ? | offset_by.rs | 113 |
| H | ? | duration.rs | 104 |
| H | ? | duration.rs | 121 |
| H | ? | duration.rs | 137 |
| H | ? | dispatch.rs | 44 |
| H | ? | dispatch.rs | 67 |
| H | ? | dispatch.rs | 88 |
| H | ? | dispatch.rs | 187 |
| H | ? | dispatch.rs | 227 |
| H | ? | dispatch.rs | 255 |
| H | ? | dispatch.rs | 325 |
| H | ? | dispatch.rs | 362 |
| H | ? | dispatch.rs | 406 |
| H | ? | dispatch.rs | 443 |
| H | ? | dispatch.rs | 562 |
| H | ? | dispatch.rs | 640 |
| H | ? | datetime.rs | 30 |
| H | ? | infer.rs | 302 |
| H | ? | infer.rs | 306 |
| H | ? | infer.rs | 445 |
| H | ? | infer.rs | 446 |
| H | ? | infer.rs | 464 |
| H | ? | infer.rs | 509 |
| H | ? | infer.rs | 514 |
| H | ? | infer.rs | 533 |
| H | ? | mod.rs | 80 |
| H | ? | mod.rs | 98 |
| H | ? | mod.rs | 112 |
| H | ? | mod.rs | 135 |
| H | ? | mod.rs | 159 |
| H | ? | mod.rs | 195 |
| H | ? | mod.rs | 253 |
| H | ? | mod.rs | 293 |
| H | ? | mod.rs | 325 |
| H | ? | month_end.rs | 92 |
| H | ? | replace.rs | 100 |
| H | ? | replace.rs | 101 |
| H | ? | replace.rs | 127 |
| H | ? | month_start.rs | 86 |
| H | ? | encode.rs | 74 |
| H | ? | decode.rs | 274 |
| H | ? | decode.rs | 292 |
| H | ? | decode.rs | 352 |
| H | ? | lib.rs | 312 |
| H | ? | lib.rs | 330 |
| H | ? | lib.rs | 334 |
| H | ? | schema.rs | 460 |
| H | ? | schema.rs | 463 |
| H | ? | schema.rs | 466 |
| H | ? | schema.rs | 482 |
| H | ? | schema.rs | 500 |
| H | ? | schema.rs | 505 |
| H | ? | schema.rs | 523 |
| H | ? | schema.rs | 531 |
| H | ? | schema.rs | 547 |
| H | ? | schema.rs | 553 |
| H | ? | cache.rs | 103 |
| H | ? | merge_sorted.rs | 21 |
| H | ? | mod.rs | 23 |
| H | ? | mod.rs | 47 |
| H | ? | mod.rs | 52 |
| H | ? | mod.rs | 53 |
| H | ? | mod.rs | 54 |
| H | ? | python_scan.rs | 80 |
| H | ? | group_by_streaming.rs | 296 |
| H | ? | group_by_streaming.rs | 309 |
| H | ? | filter.rs | 134 |
| H | ? | projection.rs | 109 |
| H | ? | projection_utils.rs | 171 |
| H | ? | projection_utils.rs | 177 |
| H | ? | projection_utils.rs | 198 |
| H | ? | group_by.rs | 147 |
| H | ? | executor.rs | 43 |
| H | ? | group_by_rolling.rs | 34 |
| H | ? | group_by_rolling.rs | 145 |
| H | ? | join.rs | 107 |
| H | ? | join.rs | 108 |
| H | ? | stack.rs | 136 |
| H | ? | group_by_dynamic.rs | 113 |
| H | ? | sort.rs | 46 |
| H | ? | sort.rs | 73 |
| H | ? | mod.rs | 72 |
| H | ? | mod.rs | 75 |
| H | ? | mod.rs | 76 |
| H | ? | mod.rs | 90 |
| H | ? | mod.rs | 93 |
| H | ? | mod.rs | 94 |
| H | ? | mod.rs | 117 |
| H | ? | mod.rs | 141 |
| H | ? | mod.rs | 142 |
| H | ? | mod.rs | 153 |
| H | ? | mod.rs | 158 |
| H | ? | mod.rs | 166 |
| H | ? | mod.rs | 178 |
| H | ? | mod.rs | 191 |
| H | ? | mod.rs | 192 |
| H | ? | mod.rs | 201 |
| H | ? | mod.rs | 205 |
| H | ? | mod.rs | 229 |
| H | ? | functions.rs | 41 |
| H | ? | functions.rs | 112 |
| H | ? | functions.rs | 123 |
| H | ? | functions.rs | 138 |
| H | ? | functions.rs | 139 |
| H | ? | functions.rs | 242 |
| H | ? | functions.rs | 388 |
| H | ? | functions.rs | 454 |
| H | ? | functions.rs | 495 |
| H | ? | functions.rs | 500 |
| H | ? | functions.rs | 504 |
| H | ? | functions.rs | 513 |
| H | ? | functions.rs | 520 |
| H | ? | functions.rs | 542 |
| H | ? | functions.rs | 581 |
| H | ? | functions.rs | 603 |
| H | ? | lp.rs | 67 |
| H | ? | lp.rs | 194 |
| H | ? | lp.rs | 271 |
| H | ? | lp.rs | 274 |
| H | ? | lp.rs | 369 |
| H | ? | lp.rs | 614 |
| H | ? | lp.rs | 674 |
| H | ? | lp.rs | 748 |
| H | ? | context.rs | 59 |
| H | ? | context.rs | 91 |
| H | ? | context.rs | 98 |
| H | ? | context.rs | 298 |
| H | ? | context.rs | 299 |
| H | ? | context.rs | 300 |
| H | ? | context.rs | 446 |
| H | ? | context.rs | 679 |
| H | ? | context.rs | 834 |
| H | ? | context.rs | 864 |
| H | ? | context.rs | 865 |
| H | ? | context.rs | 893 |
| H | ? | context.rs | 918 |
| H | ? | context.rs | 919 |
| H | ? | context.rs | 921 |
| H | ? | context.rs | 984 |
| H | ? | context.rs | 989 |
| H | ? | context.rs | 1036 |
| H | ? | context.rs | 1378 |
| H | ? | context.rs | 1399 |
| H | ? | context.rs | 1420 |
| H | ? | context.rs | 1426 |
| H | ? | context.rs | 1427 |
| H | ? | context.rs | 1456 |
| H | ? | context.rs | 1457 |
| H | ? | context.rs | 1505 |
| H | ? | context.rs | 1510 |
| H | ? | context.rs | 1530 |
| H | ? | context.rs | 1565 |
| H | ? | context.rs | 1592 |
| H | ? | context.rs | 1705 |
| H | ? | context.rs | 1750 |
| H | ? | context.rs | 1837 |
| H | ? | context.rs | 1869 |
| H | ? | context.rs | 1871 |
| H | ? | context.rs | 1889 |
| H | ? | context.rs | 1891 |
| H | ? | context.rs | 1914 |
| H | ? | context.rs | 1938 |
| H | ? | context.rs | 1942 |
| H | ? | context.rs | 1947 |
| H | ? | context.rs | 1953 |
| H | ? | context.rs | 1961 |
| H | ? | context.rs | 2005 |
| H | ? | context.rs | 2022 |
| H | ? | context.rs | 2030 |
| H | ? | context.rs | 2031 |
| H | ? | context.rs | 2034 |
| H | ? | context.rs | 2037 |
| H | ? | context.rs | 2152 |
| H | ? | context.rs | 2153 |
| H | ? | context.rs | 2179 |
| H | ? | context.rs | 2180 |
| H | ? | context.rs | 2241 |
| H | ? | context.rs | 2245 |
| H | ? | context.rs | 2258 |
| H | ? | context.rs | 2279 |
| H | ? | context.rs | 2285 |
| H | ? | context.rs | 2302 |
| H | ? | context.rs | 2320 |
| H | ? | context.rs | 2410 |
| H | ? | context.rs | 2426 |
| H | ? | context.rs | 2435 |
| H | ? | context.rs | 2442 |
| H | ? | context.rs | 2448 |
| H | ? | context.rs | 2455 |
| H | ? | context.rs | 2462 |
| H | ? | context.rs | 2463 |
| H | ? | context.rs | 2510 |
| H | ? | context.rs | 2512 |
| H | ? | context.rs | 2517 |
| H | ? | context.rs | 2519 |
| H | ? | context.rs | 2528 |
| H | ? | context.rs | 2530 |
| H | ? | context.rs | 2533 |
| H | ? | context.rs | 2543 |
| H | ? | context.rs | 2553 |
| H | ? | context.rs | 2688 |
| H | ? | context.rs | 2691 |
| H | ? | context.rs | 2749 |
| H | ? | context.rs | 2773 |
| H | ? | context.rs | 2819 |
| H | ? | context.rs | 2829 |
| H | ? | context.rs | 2833 |
| H | ? | context.rs | 2838 |
| H | ? | context.rs | 2855 |
| H | ? | context.rs | 2857 |
| H | ? | context.rs | 2873 |
| H | ? | context.rs | 3090 |
| H | ? | context.rs | 3094 |
| H | ? | context.rs | 3177 |
| H | ? | context.rs | 3184 |
| H | ? | context.rs | 3189 |
| H | ? | context.rs | 3270 |
| H | ? | context.rs | 3272 |
| H | ? | table_functions.rs | 90 |
| H | ? | table_functions.rs | 102 |
| H | ? | table_functions.rs | 111 |
| H | ? | table_functions.rs | 122 |
| H | ? | subquery.rs | 223 |
| H | ? | subquery.rs | 224 |
| H | ? | subquery.rs | 225 |
| H | ? | subquery.rs | 226 |
| H | ? | subquery.rs | 231 |
| H | ? | subquery.rs | 379 |
| H | ? | subquery.rs | 403 |
| H | ? | subquery.rs | 404 |
| H | ? | subquery.rs | 405 |
| H | ? | subquery.rs | 407 |
| H | ? | subquery.rs | 409 |
| H | ? | subquery.rs | 434 |
| H | ? | subquery.rs | 435 |
| H | ? | subquery.rs | 438 |
| H | ? | sql_visitors.rs | 87 |
| H | ? | sql_visitors.rs | 91 |
| H | ? | sql_visitors.rs | 196 |
| H | ? | sql_visitors.rs | 200 |
| H | ? | sql_visitors.rs | 236 |
| H | ? | sql_expr.rs | 116 |
| H | ? | sql_expr.rs | 278 |
| H | ? | sql_expr.rs | 294 |
| H | ? | sql_expr.rs | 393 |
| H | ? | sql_expr.rs | 394 |
| H | ? | sql_expr.rs | 412 |
| H | ? | sql_expr.rs | 424 |
| H | ? | sql_expr.rs | 483 |
| H | ? | sql_expr.rs | 489 |
| H | ? | sql_expr.rs | 496 |
| H | ? | sql_expr.rs | 508 |
| H | ? | sql_expr.rs | 514 |
| H | ? | sql_expr.rs | 529 |
| H | ? | sql_expr.rs | 537 |
| H | ? | sql_expr.rs | 541 |
| H | ? | sql_expr.rs | 558 |
| H | ? | sql_expr.rs | 708 |
| H | ? | sql_expr.rs | 709 |
| H | ? | sql_expr.rs | 716 |
| H | ? | sql_expr.rs | 717 |
| H | ? | sql_expr.rs | 779 |
| H | ? | sql_expr.rs | 951 |
| H | ? | sql_expr.rs | 957 |
| H | ? | sql_expr.rs | 976 |
| H | ? | sql_expr.rs | 991 |
| H | ? | sql_expr.rs | 998 |
| H | ? | sql_expr.rs | 1090 |
| H | ? | sql_expr.rs | 1092 |
| H | ? | sql_expr.rs | 1149 |
| H | ? | sql_expr.rs | 1168 |
| H | ? | sql_expr.rs | 1169 |
| H | ? | sql_expr.rs | 1171 |
| H | ? | sql_expr.rs | 1214 |
| H | ? | sql_expr.rs | 1216 |
| H | ? | sql_expr.rs | 1472 |
| H | ? | sql_expr.rs | 1482 |
| H | ? | sql_expr.rs | 1486 |
| H | ? | sql_expr.rs | 1490 |
| H | ? | sql_expr.rs | 1496 |
| H | ? | sql_expr.rs | 1524 |
| H | ? | sql_expr.rs | 1525 |
| H | ? | sql_expr.rs | 1527 |
| H | ? | sql_expr.rs | 1529 |
| H | ? | sql_expr.rs | 1531 |
| H | ? | sql_expr.rs | 1583 |
| H | ? | sql_expr.rs | 1648 |
| H | ? | functions.rs | 1243 |
| H | ? | functions.rs | 1332 |
| H | ? | functions.rs | 1339 |
| H | ? | functions.rs | 1340 |
| H | ? | functions.rs | 1341 |
| H | ? | functions.rs | 1343 |
| H | ? | functions.rs | 1353 |
| H | ? | functions.rs | 1355 |
| H | ? | functions.rs | 1417 |
| H | ? | functions.rs | 1475 |
| H | ? | functions.rs | 1482 |
| H | ? | functions.rs | 1484 |
| H | ? | functions.rs | 1486 |
| H | ? | functions.rs | 1488 |
| H | ? | functions.rs | 1489 |
| H | ? | functions.rs | 1499 |
| H | ? | functions.rs | 1501 |
| H | ? | functions.rs | 1577 |
| H | ? | functions.rs | 1581 |
| H | ? | functions.rs | 1596 |
| H | ? | functions.rs | 1597 |
| H | ? | functions.rs | 1767 |
| H | ? | functions.rs | 1992 |
| H | ? | functions.rs | 2016 |
| H | ? | functions.rs | 2208 |
| H | ? | functions.rs | 2214 |
| H | ? | functions.rs | 2306 |
| H | ? | functions.rs | 2324 |
| H | ? | functions.rs | 2449 |
| H | ? | functions.rs | 2458 |
| H | ? | functions.rs | 2460 |
| H | ? | functions.rs | 2520 |
| H | ? | functions.rs | 2585 |
| H | ? | distances.rs | 95 |
| H | ? | expressions.rs | 89 |
| H | ? | expressions.rs | 180 |
| H | ? | expressions.rs | 212 |
| H | ? | lib.rs | 102 |
| H | ? | types.rs | 264 |
| H | ? | types.rs | 416 |
| H | ? | types.rs | 422 |
| H | ? | types.rs | 452 |
| H | ? | types.rs | 465 |
| H | ? | types.rs | 501 |
| H | ? | types.rs | 545 |
| H | ? | types.rs | 599 |
| H | ? | dataframe.py | 281 |
| H | ? | dataframe.py | 1385 |
| H | ? | series.py | 546 |
| H | ? | slice.py | 93 |
| H | ? | slice.py | 166 |
| H | ? | series.py | 853 |
| H | ? | series.py | 1428 |
| H | ? | series.py | 1431 |
| H | ? | series.py | 3053 |
| H | ? | series.py | 5537 |
| H | ? | frame.py | 762 |
| H | ? | frame.py | 765 |
| H | ? | frame.py | 4808 |
| H | ? | frame.py | 5066 |
| H | ? | frame.py | 5224 |
| H | ? | frame.py | 1611 |
| H | ? | frame.py | 1614 |
| H | ? | frame.py | 9248 |

---
*Сгенерировано GSC v0.6 · 2026-07-30T04:01:56.081186*