---
title: "GSC Audit: /tmp/gsc-external/SALib"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/SALib

**Дата:** 08.08.2026 19:16  
**Путь:** `/tmp/gsc-external/SALib`  
**Всего находок:** 56  
**CRITICAL:** 6 | **HIGH:** 6 | **MEDIUM:** 11 | **LOW:** 29

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 29 |
| GS018 | 11 |
| GS001 | 6 |
| GS025 | 5 |
| GS021 | 3 |
| GS000-LEGACY | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | CITATION.cff | 6 | Found: cid: "0000 |
| CRITICAL | GS001 | CITATION.cff | 9 | Found: cid: "0000 |
| CRITICAL | GS001 | CITATION.cff | 12 | Found: cid: "0000 |
| CRITICAL | GS001 | CITATION.cff | 23 | Found: cid: "0000 |
| CRITICAL | GS001 | CITATION.cff | 26 | Found: cid: "0000 |
| CRITICAL | GS001 | CITATION.cff | 29 | Found: cid: "0000 |
| HIGH | GS000-LEGACY | CITATION.cff | 14 | Match: version: 1.4.6.1 |
| HIGH | GS025 | environment.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .zenodo.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .coveralls.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS018 | problem.py | 146 |
| M | GS018 | problem.py | 656 |
| M | GS018 | problem.py | 657 |
| M | GS018 | problem.py | 658 |
| M | GS018 | strategy.py | 114 |
| M | GS018 | strategy.py | 124 |
| M | GS018 | strategy.py | 213 |
| M | GS018 | strategy.py | 214 |
| M | GS018 | strategy.py | 217 |
| M | GS018 | heatmap.py | 38 |
| M | GS018 | morris.py | 36 |
| C | GS001 | CITATION.cff | 6 |
| C | GS001 | CITATION.cff | 9 |
| C | GS001 | CITATION.cff | 12 |
| C | GS001 | CITATION.cff | 23 |
| C | GS001 | CITATION.cff | 26 |
| C | GS001 | CITATION.cff | 29 |
| L | GS003 | delta.py | 293 |
| L | GS003 | dgsm.py | 100 |
| L | GS003 | discrepancy.py | 120 |
| L | GS003 | enhanced_hdmr.py | 1522 |
| L | GS003 | enhanced_hdmr.py | 1524 |
| L | GS003 | enhanced_hdmr.py | 1525 |
| L | GS003 | enhanced_hdmr.py | 1532 |
| L | GS003 | enhanced_hdmr.py | 1548 |
| L | GS003 | enhanced_hdmr.py | 1561 |
| L | GS003 | enhanced_hdmr.py | 1565 |
| L | GS003 | ff.py | 94 |
| L | GS003 | hdmr.py | 943 |
| L | GS003 | hdmr.py | 944 |
| L | GS003 | hdmr.py | 947 |
| L | GS003 | hdmr.py | 954 |
| L | GS003 | hdmr.py | 970 |
| L | GS003 | hdmr.py | 983 |
| L | GS003 | hdmr.py | 987 |
| L | GS003 | morris.py | 167 |
| L | GS003 | pawn.py | 173 |
| L | GS003 | rbd_fast.py | 102 |
| L | GS003 | rsa.py | 136 |
| L | GS003 | sobol.py | 204 |
| L | GS003 | lake_problem.py | 197 |
| L | GS003 | lake_problem.py | 198 |
| L | GS003 | oakley2004.py | 333 |
| L | GS003 | oakley2004.py | 361 |
| L | GS003 | oakley2004.py | 363 |
| L | GS003 | problem.py | 310 |
| H | GS000-LEGACY | CITATION.cff | 14 |
| H | GS025 | environment.yml | 0 |
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS025 | .zenodo.json | 0 |
| H | GS025 | .readthedocs.yml | 0 |
| H | GS025 | .coveralls.yml | 0 |
| s | GS009 |  | 0 |
| s | GS021 |  | 84 |
| s | GS021 |  | 84 |
| s | GS021 |  | 84 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T19:16:45.520445*