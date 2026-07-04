---
title: "GSC Audit: /tmp/gsc-learn/pydantic"
date: 2026-07-01
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pydantic

**Дата:** 01.07.2026 04:07  
**Путь:** `/tmp/gsc-learn/pydantic`  
**Всего находок:** 646  
**CRITICAL:** 6 | **HIGH:** 338 | **MEDIUM:** 78 | **LOW:** 221

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 328 |
| Python: assert in production | 75 |
| GS003 | 36 |
| GS008 | 8 |
| GS014 | 5 |
| Generic code smell #24 | 3 |
| Generic code smell #27 | 3 |
| Generic code smell #30 | 3 |
| Generic code smell #33 | 3 |
| Generic code smell #36 | 3 |
| Generic code smell #39 | 3 |
| Generic code smell #42 | 3 |
| Generic code smell #45 | 3 |
| Generic code smell #48 | 3 |
| Generic code smell #51 | 3 |
| Generic code smell #54 | 3 |
| Generic code smell #57 | 3 |
| Generic code smell #60 | 3 |
| Generic code smell #63 | 3 |
| Generic code smell #66 | 3 |
| Generic code smell #69 | 3 |
| Generic code smell #72 | 3 |
| Generic code smell #75 | 3 |
| Generic code smell #78 | 3 |
| Generic code smell #81 | 3 |
| Generic code smell #84 | 3 |
| Generic code smell #87 | 3 |
| Generic code smell #90 | 3 |
| Generic code smell #93 | 3 |
| Generic code smell #96 | 3 |
| Generic code smell #99 | 3 |
| Generic code smell #102 | 3 |
| Generic code smell #105 | 3 |
| Generic code smell #108 | 3 |
| Generic code smell #111 | 3 |
| Generic code smell #114 | 3 |
| Generic code smell #117 | 3 |
| Generic code smell #120 | 3 |
| Generic code smell #123 | 3 |
| Generic code smell #126 | 3 |
| Generic code smell #129 | 3 |
| Generic code smell #132 | 3 |
| Generic code smell #135 | 3 |
| Generic code smell #138 | 3 |
| Generic code smell #141 | 3 |
| Generic code smell #144 | 3 |
| Generic code smell #147 | 3 |
| Generic code smell #150 | 3 |
| Generic code smell #153 | 3 |
| Generic code smell #156 | 3 |
| Generic code smell #159 | 3 |
| Generic code smell #162 | 3 |
| Generic code smell #165 | 3 |
| Generic code smell #168 | 3 |
| Generic code smell #171 | 3 |
| Generic code smell #174 | 3 |
| Generic code smell #177 | 3 |
| Generic code smell #180 | 3 |
| Generic code smell #183 | 3 |
| Generic code smell #186 | 3 |
| Generic code smell #189 | 3 |
| Generic code smell #192 | 3 |
| Generic code smell #195 | 3 |
| Generic code smell #198 | 3 |
| GS015 | 2 |
| Hardcoded encryption key | 2 |
| Outdated dependency pattern | 2 |
| Weak password validation | 2 |
| pickle.load() — unsafe deserialization | 2 |
| eval() or exec() usage | 1 |
| World-readable file: .yamlfmt.yaml (664) | 1 |
| World-readable file: .markdownlint.yaml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | _known_annotated_metadata.py | 265 | Match:                     js_constraint_key = 'minItems' if |
| CRITICAL | ? | _known_annotated_metadata.py | 267 | Match:                     js_constraint_key = 'minLength' i |
| CRITICAL | ? | networks.py | 173 | Match:     min_length = 1 |
| CRITICAL | ? | _config.py | 275 | Match:     str_min_length=0, |
| CRITICAL | ? | parse.py | 55 | Match:         return pickle.loads(bb) |
| CRITICAL | ? | parse.py | 42 | Match:         return pickle.loads(bb) |
| HIGH | ? | utils.py | 195 | Match:         eval('__IPYTHON__') |
| HIGH | ? | .yamlfmt.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .markdownlint.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS014 | networks.py | 765 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | networks.py | 767 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | networks.py | 770 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | networks.py | 778 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | networks.py | 778 | Database URL contains password in plaintext. Use environment |
| HIGH | ? | build_tools.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 351 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 473 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | bytes.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | bytes.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | bytes.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | bytes.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | float.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | decimal.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | fraction.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | uuid.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | uuid.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | any.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | timedelta.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime_etc.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | model.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | model.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | model.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | simple.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | complex.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | complex.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | missing_sentinel.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | union.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | union.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | union.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | extra.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | errors.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | errors.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | errors.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | errors.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | filter.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | computed_fields.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | computed_fields.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | fields.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | fields.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | fields.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | fields.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | fields.rs | 418 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | infer.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 300 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 365 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 561 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 596 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 793 | Clone in performance-critical code — consider references |
| HIGH | ? | input_python.rs | 794 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | datetime.rs | 810 | Clone in performance-critical code — consider references |
| HIGH | ? | return_enums.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | return_enums.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | return_enums.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | return_enums.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | return_enums.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | return_enums.rs | 607 | Clone in performance-critical code — consider references |
| HIGH | ? | input_json.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | input_json.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | input_json.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | input_string.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | input_string.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | input_string.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | input_string.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | line_error.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | location.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | validation_exception.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | validation_exception.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | union.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | definitions.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | custom_error.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | custom_error.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | is_instance.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | is_instance.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 587 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments_v3.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 473 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 476 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 633 | Clone in performance-critical code — consider references |
| HIGH | ? | model_fields.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 351 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | dataclass.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | model.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | model.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | model.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | model.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | uuid.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | complex.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | complex.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 313 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | none.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | lookup_tree.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | lookup_tree.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | url.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | chain.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | call.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | dict.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | dict.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | with_default.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | literal.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | generator.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | validation_state.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | is_subclass.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | is_subclass.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | string.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | missing_sentinel.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | union.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | union.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | union.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | any.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | lookup_key.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | lookup_key.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | lookup_key.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | timedelta.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | bool.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | bool.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | callable.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | callable.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | int.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | int.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | int.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | int.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | int.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | int.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | int.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 357 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| L | ? | json_schema.py | 1463 |
| L | ? | fields.py | 450 |
| L | ? | fields.py | 460 |
| M | ? | decorator.py | 122 |
| M | ? | pipeline.py | 434 |
| M | ? | pipeline.py | 553 |
| M | ? | pipeline.py | 598 |
| M | ? | pipeline.py | 609 |
| M | ? | pipeline.py | 624 |
| M | ? | pipeline.py | 671 |
| M | ? | pipeline.py | 678 |
| M | ? | networks.py | 1357 |
| M | ? | mypy.py | 182 |
| M | ? | mypy.py | 217 |
| M | ? | mypy.py | 395 |
| M | ? | mypy.py | 431 |
| M | ? | mypy.py | 710 |
| M | ? | mypy.py | 894 |
| M | ? | mypy.py | 939 |
| M | ? | mypy.py | 942 |
| M | ? | mypy.py | 945 |
| M | ? | mypy.py | 1377 |
| M | ? | decorator.py | 105 |
| M | ? | networks.py | 277 |
| M | ? | networks.py | 365 |
| M | ? | networks.py | 738 |
| M | ? | mypy.py | 167 |
| M | ? | mypy.py | 182 |
| M | ? | mypy.py | 183 |
| M | ? | mypy.py | 860 |
| M | ? | utils.py | 665 |
| M | ? | _hypothesis_plugin.py | 212 |
| M | ? | _hypothesis_plugin.py | 258 |
| M | ? | _hypothesis_plugin.py | 268 |
| M | ? | _hypothesis_plugin.py | 271 |
| M | ? | _hypothesis_plugin.py | 289 |
| M | ? | _hypothesis_plugin.py | 293 |
| M | ? | _hypothesis_plugin.py | 305 |
| M | ? | _hypothesis_plugin.py | 318 |
| M | ? | _hypothesis_plugin.py | 321 |
| M | ? | _hypothesis_plugin.py | 339 |
| M | ? | _hypothesis_plugin.py | 346 |
| M | ? | _hypothesis_plugin.py | 377 |
| M | ? | generics.py | 293 |
| M | ? | generics.py | 389 |
| M | ? | generics.py | 393 |
| M | ? | schema.py | 526 |
| M | ? | schema.py | 715 |
| M | ? | class_validators.py | 89 |
| M | ? | fields.py | 763 |
| M | ? | fields.py | 768 |
| M | ? | fields.py | 853 |
| M | ? | fields.py | 856 |
| M | ? | fields.py | 1103 |
| M | ? | fields.py | 1104 |
| M | ? | fields.py | 1124 |
| M | ? | fields.py | 1135 |
| M | ? | fields.py | 1179 |
| M | ? | dataclasses.py | 112 |
| M | ? | dataclasses.py | 113 |
| M | ? | _discriminated_union.py | 163 |
| M | ? | _validators.py | 350 |
| M | ? | _model_construction.py | 664 |
| M | ? | _generics.py | 308 |
| M | ? | _generate_schema.py | 1359 |
| M | ? | _generate_schema.py | 1366 |
| M | ? | _generate_schema.py | 1581 |
| M | ? | _generate_schema.py | 2003 |
| M | ? | _generate_schema.py | 2070 |
| M | ? | _generate_schema.py | 2468 |
| M | ? | _generate_schema.py | 2631 |
| M | ? | _decorators.py | 569 |
| M | ? | _decorators.py | 685 |
| M | ? | _decorators.py | 778 |
| M | ? | type_adapter.py | 730 |
| M | ? | type_adapter.py | 784 |
| M | ? | json_schema.py | 2591 |
| M | ? | validate_call_decorator.py | 37 |
| L | GS003 | _core_utils.py | 172 |
| L | GS003 | mypy.py | 267 |
| L | GS003 | mypy.py | 277 |
| L | GS003 | run_tests.py | 19 |
| L | GS003 | run_tests.py | 20 |
| L | GS003 | run_tests.py | 37 |
| L | GS003 | run_tests.py | 57 |
| L | GS003 | prepare.py | 32 |
| L | GS003 | prepare.py | 44 |
| L | GS003 | prepare.py | 45 |
| L | GS003 | prepare.py | 46 |
| L | GS003 | prepare.py | 47 |
| L | GS003 | prepare.py | 48 |
| L | GS003 | prepare.py | 49 |
| L | GS003 | prepare.py | 118 |
| L | GS003 | prepare.py | 123 |
| L | GS003 | prepare.py | 131 |
| L | GS003 | prepare.py | 135 |
| L | GS003 | prepare.py | 138 |
| L | GS003 | prepare.py | 168 |
| L | GS003 | push.py | 56 |
| L | GS003 | push.py | 75 |
| L | GS003 | push.py | 76 |
| L | GS003 | push.py | 110 |
| L | GS003 | push.py | 111 |
| L | GS003 | push.py | 130 |
| L | GS003 | push.py | 131 |
| L | GS003 | push.py | 145 |
| L | GS003 | push.py | 149 |
| L | GS003 | push.py | 150 |
| L | GS003 | build.rs | 4 |
| L | GS003 | build.rs | 6 |
| L | GS003 | build.rs | 12 |
| L | GS003 | build.rs | 14 |
| L | GS003 | build.rs | 15 |
| L | GS003 | build.rs | 23 |
| L | GS008 | _generate_schema.py | 336 |
| L | GS008 | _known_annotated_metadata.py | 42 |
| L | GS008 | _known_annotated_metadata.py | 52 |
| L | GS008 | _known_annotated_metadata.py | 53 |
| L | GS008 | mypy.py | 92 |
| L | GS008 | mypy.py | 105 |
| L | GS008 | mypy.py | 1289 |
| L | GS008 | shared.py | 12 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| C | ? | _known_annotated_metadata.py | 265 |
| C | ? | _known_annotated_metadata.py | 267 |
| M | ? | mypy.py | 1436 |
| M | ? | mypy.py | 945 |
| C | ? | networks.py | 173 |
| C | ? | _config.py | 275 |
| H | ? | utils.py | 195 |
| C | ? | parse.py | 55 |
| C | ? | parse.py | 42 |
| H | ? | .yamlfmt.yaml | 0 |
| H | ? | .markdownlint.yaml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | mkdocs.yml | 0 |
| s | GS009 |  | 0 |
| H | GS014 | networks.py | 765 |
| H | GS014 | networks.py | 767 |
| H | GS014 | networks.py | 770 |
| H | GS014 | networks.py | 778 |
| H | GS014 | networks.py | 778 |
| M | ? | shared.py | 8 |
| H | ? | build_tools.rs | 146 |
| H | ? | url.rs | 115 |
| H | ? | url.rs | 219 |
| H | ? | url.rs | 351 |
| H | ? | url.rs | 473 |
| H | ? | enum_.rs | 37 |
| H | ? | enum_.rs | 38 |
| H | ? | enum_.rs | 39 |
| H | ? | enum_.rs | 66 |
| H | ? | bytes.rs | 57 |
| H | ? | bytes.rs | 58 |
| H | ? | bytes.rs | 59 |
| H | ? | bytes.rs | 75 |
| H | ? | float.rs | 95 |
| H | ? | dataclass.rs | 116 |
| H | ? | dataclass.rs | 152 |
| H | ? | dataclass.rs | 221 |
| H | ? | decimal.rs | 27 |
| H | ? | fraction.rs | 29 |
| H | ? | uuid.rs | 39 |
| H | ? | uuid.rs | 49 |
| H | ? | typed_dict.rs | 106 |
| H | ? | typed_dict.rs | 126 |
| H | ? | url.rs | 31 |
| H | ? | url.rs | 47 |
| H | ? | function.rs | 171 |
| H | ? | function.rs | 196 |
| H | ? | function.rs | 408 |
| H | ? | function.rs | 444 |
| H | ? | function.rs | 551 |
| H | ? | function.rs | 552 |
| H | ? | function.rs | 553 |
| H | ? | function.rs | 554 |
| H | ? | function.rs | 571 |
| H | ? | function.rs | 572 |
| H | ? | function.rs | 573 |
| H | ? | function.rs | 574 |
| H | ? | generator.rs | 66 |
| H | ? | generator.rs | 77 |
| H | ? | generator.rs | 109 |
| H | ? | generator.rs | 156 |
| H | ? | generator.rs | 158 |
| H | ? | generator.rs | 185 |
| H | ? | any.rs | 33 |
| H | ? | timedelta.rs | 50 |
| H | ? | datetime_etc.rs | 96 |
| H | ? | format.rs | 105 |
| H | ? | format.rs | 119 |
| H | ? | format.rs | 189 |
| H | ? | model.rs | 178 |
| H | ? | model.rs | 212 |
| H | ? | model.rs | 213 |
| H | ? | simple.rs | 33 |
| H | ? | simple.rs | 111 |
| H | ? | simple.rs | 125 |
| H | ? | complex.rs | 24 |
| H | ? | complex.rs | 36 |
| H | ? | literal.rs | 122 |
| H | ? | literal.rs | 126 |
| H | ? | string.rs | 36 |
| H | ? | string.rs | 46 |
| H | ? | string.rs | 49 |
| H | ? | missing_sentinel.rs | 37 |
| H | ? | union.rs | 300 |
| H | ? | union.rs | 425 |
| H | ? | union.rs | 443 |
| H | ? | extra.rs | 285 |
| H | ? | extra.rs | 286 |
| H | ? | extra.rs | 294 |
| H | ? | extra.rs | 296 |
| H | ? | extra.rs | 297 |
| H | ? | extra.rs | 299 |
| H | ? | extra.rs | 301 |
| H | ? | extra.rs | 303 |
| H | ? | extra.rs | 304 |
| H | ? | extra.rs | 311 |
| H | ? | extra.rs | 320 |
| H | ? | extra.rs | 322 |
| H | ? | extra.rs | 330 |
| H | ? | extra.rs | 331 |
| H | ? | extra.rs | 333 |
| H | ? | extra.rs | 334 |
| H | ? | extra.rs | 337 |
| H | ? | extra.rs | 338 |
| H | ? | extra.rs | 386 |
| H | ? | extra.rs | 387 |
| H | ? | extra.rs | 461 |
| H | ? | extra.rs | 463 |
| H | ? | extra.rs | 501 |
| H | ? | extra.rs | 503 |
| H | ? | errors.rs | 159 |
| H | ? | errors.rs | 160 |
| H | ? | errors.rs | 161 |
| H | ? | errors.rs | 162 |
| H | ? | filter.rs | 25 |
| H | ? | filter.rs | 33 |
| H | ? | filter.rs | 58 |
| H | ? | computed_fields.rs | 52 |
| H | ? | computed_fields.rs | 102 |
| H | ? | fields.rs | 140 |
| H | ? | fields.rs | 194 |
| H | ? | fields.rs | 381 |
| H | ? | fields.rs | 416 |
| H | ? | fields.rs | 418 |
| H | ? | mod.rs | 79 |
| H | ? | infer.rs | 62 |
| H | ? | infer.rs | 99 |
| H | ? | infer.rs | 261 |
| H | ? | infer.rs | 263 |
| H | ? | input_python.rs | 88 |
| H | ? | input_python.rs | 110 |
| H | ? | input_python.rs | 114 |
| H | ? | input_python.rs | 132 |
| H | ? | input_python.rs | 153 |
| H | ? | input_python.rs | 250 |
| H | ? | input_python.rs | 292 |
| H | ? | input_python.rs | 300 |
| H | ? | input_python.rs | 308 |
| H | ? | input_python.rs | 336 |
| H | ? | input_python.rs | 341 |
| H | ? | input_python.rs | 365 |
| H | ? | input_python.rs | 530 |
| H | ? | input_python.rs | 536 |
| H | ? | input_python.rs | 561 |
| H | ? | input_python.rs | 563 |
| H | ? | input_python.rs | 596 |
| H | ? | input_python.rs | 598 |
| H | ? | input_python.rs | 793 |
| H | ? | input_python.rs | 794 |
| H | ? | datetime.rs | 152 |
| H | ? | datetime.rs | 251 |
| H | ? | datetime.rs | 254 |
| H | ? | datetime.rs | 810 |
| H | ? | return_enums.rs | 390 |
| H | ? | return_enums.rs | 452 |
| H | ? | return_enums.rs | 484 |
| H | ? | return_enums.rs | 511 |
| H | ? | return_enums.rs | 537 |
| H | ? | return_enums.rs | 607 |
| H | ? | input_json.rs | 168 |
| H | ? | input_json.rs | 287 |
| H | ? | input_json.rs | 296 |
| H | ? | input_string.rs | 82 |
| H | ? | input_string.rs | 104 |
| H | ? | input_string.rs | 114 |
| H | ? | input_string.rs | 176 |
| H | ? | line_error.rs | 91 |
| H | ? | location.rs | 113 |
| H | ? | types.rs | 106 |
| H | ? | types.rs | 657 |
| H | ? | validation_exception.rs | 65 |
| H | ? | validation_exception.rs | 463 |
| H | ? | union.rs | 19 |
| H | ? | definitions.rs | 52 |
| H | ? | definitions.rs | 53 |
| H | ? | definitions.rs | 54 |
| H | ? | definitions.rs | 157 |
| H | ? | definitions.rs | 167 |
| H | ? | definitions.rs | 174 |
| H | ? | definitions.rs | 190 |
| H | ? | definitions.rs | 216 |
| H | ? | custom_error.rs | 56 |
| H | ? | custom_error.rs | 57 |
| H | ? | is_instance.rs | 70 |
| H | ? | is_instance.rs | 73 |
| H | ? | arguments_v3.rs | 105 |
| H | ? | arguments_v3.rs | 106 |
| H | ? | arguments_v3.rs | 186 |
| H | ? | arguments_v3.rs | 338 |
| H | ? | arguments_v3.rs | 339 |
| H | ? | arguments_v3.rs | 353 |
| H | ? | arguments_v3.rs | 392 |
| H | ? | arguments_v3.rs | 425 |
| H | ? | arguments_v3.rs | 462 |
| H | ? | arguments_v3.rs | 481 |
| H | ? | arguments_v3.rs | 559 |
| H | ? | arguments_v3.rs | 587 |
| H | ? | arguments_v3.rs | 657 |
| H | ? | arguments_v3.rs | 679 |
| H | ? | arguments_v3.rs | 693 |
| H | ? | enum_.rs | 55 |
| H | ? | enum_.rs | 60 |
| H | ? | enum_.rs | 107 |
| H | ? | enum_.rs | 114 |
| H | ? | enum_.rs | 131 |
| H | ? | enum_.rs | 156 |
| H | ? | model_fields.rs | 98 |
| H | ? | model_fields.rs | 151 |
| H | ? | model_fields.rs | 168 |
| H | ? | model_fields.rs | 214 |
| H | ? | model_fields.rs | 242 |
| H | ? | model_fields.rs | 331 |
| H | ? | model_fields.rs | 335 |
| H | ? | model_fields.rs | 346 |
| H | ? | model_fields.rs | 364 |
| H | ? | model_fields.rs | 383 |
| H | ? | model_fields.rs | 445 |
| H | ? | model_fields.rs | 465 |
| H | ? | model_fields.rs | 473 |
| H | ? | model_fields.rs | 476 |
| H | ? | model_fields.rs | 494 |
| H | ? | model_fields.rs | 564 |
| H | ? | model_fields.rs | 633 |
| H | ? | model_fields.rs | 655 |
| H | ? | dataclass.rs | 79 |
| H | ? | dataclass.rs | 100 |
| H | ? | dataclass.rs | 159 |
| H | ? | dataclass.rs | 185 |
| H | ? | dataclass.rs | 220 |
| H | ? | dataclass.rs | 228 |
| H | ? | dataclass.rs | 261 |
| H | ? | dataclass.rs | 320 |
| H | ? | dataclass.rs | 333 |
| H | ? | dataclass.rs | 351 |
| H | ? | dataclass.rs | 399 |
| H | ? | dataclass.rs | 411 |
| H | ? | dataclass.rs | 412 |
| H | ? | dataclass.rs | 419 |
| H | ? | dataclass.rs | 432 |
| H | ? | dataclass.rs | 488 |
| H | ? | dataclass.rs | 614 |
| H | ? | dataclass.rs | 638 |
| H | ? | model.rs | 206 |
| H | ? | model.rs | 262 |
| H | ? | model.rs | 279 |
| H | ? | model.rs | 307 |
| H | ? | uuid.rs | 117 |
| H | ? | complex.rs | 41 |
| H | ? | complex.rs | 43 |
| H | ? | typed_dict.rs | 116 |
| H | ? | typed_dict.rs | 179 |
| H | ? | typed_dict.rs | 193 |
| H | ? | typed_dict.rs | 196 |
| H | ? | typed_dict.rs | 221 |
| H | ? | typed_dict.rs | 250 |
| H | ? | typed_dict.rs | 313 |
| H | ? | typed_dict.rs | 333 |
| H | ? | typed_dict.rs | 340 |
| H | ? | typed_dict.rs | 352 |
| H | ? | none.rs | 24 |
| H | ? | lookup_tree.rs | 164 |
| H | ? | lookup_tree.rs | 175 |
| H | ? | url.rs | 139 |
| H | ? | url.rs | 160 |
| H | ? | url.rs | 211 |
| H | ? | url.rs | 275 |
| H | ? | url.rs | 390 |
| H | ? | url.rs | 411 |
| H | ? | url.rs | 461 |
| H | ? | url.rs | 465 |
| H | ? | url.rs | 527 |
| H | ? | mod.rs | 150 |
| H | ? | mod.rs | 152 |
| H | ? | mod.rs | 366 |
| H | ? | chain.rs | 66 |
| H | ? | call.rs | 54 |
| H | ? | function.rs | 70 |
| H | ? | function.rs | 109 |
| H | ? | function.rs | 183 |
| H | ? | function.rs | 250 |
| H | ? | function.rs | 252 |
| H | ? | function.rs | 256 |
| H | ? | function.rs | 277 |
| H | ? | function.rs | 318 |
| H | ? | function.rs | 320 |
| H | ? | function.rs | 324 |
| H | ? | function.rs | 346 |
| H | ? | function.rs | 372 |
| H | ? | function.rs | 398 |
| H | ? | function.rs | 403 |
| H | ? | function.rs | 404 |
| H | ? | function.rs | 507 |
| H | ? | function.rs | 509 |
| H | ? | function.rs | 511 |
| H | ? | function.rs | 547 |
| H | ? | function.rs | 549 |
| H | ? | dict.rs | 134 |
| H | ? | dict.rs | 154 |
| H | ? | with_default.rs | 189 |
| H | ? | literal.rs | 263 |
| H | ? | literal.rs | 284 |
| H | ? | literal.rs | 287 |
| H | ? | generator.rs | 78 |
| H | ? | generator.rs | 257 |
| H | ? | generator.rs | 261 |
| H | ? | generator.rs | 262 |
| H | ? | generator.rs | 263 |
| H | ? | generator.rs | 264 |
| H | ? | generator.rs | 296 |
| H | ? | generator.rs | 299 |
| H | ? | generator.rs | 339 |
| H | ? | generator.rs | 342 |
| H | ? | validation_state.rs | 76 |
| H | ? | is_subclass.rs | 65 |
| H | ? | is_subclass.rs | 68 |
| H | ? | string.rs | 56 |
| H | ? | string.rs | 58 |
| H | ? | string.rs | 162 |
| H | ? | string.rs | 311 |
| H | ? | string.rs | 316 |
| H | ? | missing_sentinel.rs | 27 |
| H | ? | union.rs | 409 |
| H | ? | union.rs | 411 |
| H | ? | union.rs | 424 |
| H | ? | any.rs | 27 |
| H | ? | lookup_key.rs | 184 |
| H | ? | lookup_key.rs | 193 |
| H | ? | lookup_key.rs | 352 |
| H | ? | timedelta.rs | 84 |
| H | ? | bool.rs | 32 |
| H | ? | bool.rs | 34 |
| H | ? | callable.rs | 25 |
| H | ? | callable.rs | 42 |
| H | ? | int.rs | 62 |
| H | ? | int.rs | 64 |
| H | ? | int.rs | 130 |
| H | ? | int.rs | 141 |
| H | ? | int.rs | 152 |
| H | ? | int.rs | 163 |
| H | ? | int.rs | 175 |
| H | ? | arguments.rs | 88 |
| H | ? | arguments.rs | 107 |
| H | ? | arguments.rs | 230 |
| H | ? | arguments.rs | 237 |
| H | ? | arguments.rs | 263 |
| H | ? | arguments.rs | 330 |
| H | ? | arguments.rs | 347 |
| H | ? | arguments.rs | 357 |

---
*Сгенерировано GSC v0.6 · 2026-07-01T04:07:40.836034*