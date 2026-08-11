---
title: "GSC Audit: /tmp/gsc-external/grocery-app"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/grocery-app

**Дата:** 09.08.2026 06:45  
**Путь:** `/tmp/gsc-external/grocery-app`  
**Всего находок:** 82  
**CRITICAL:** 1 | **HIGH:** 1 | **MEDIUM:** 11 | **LOW:** 59

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 59 |
| GS010 | 10 |
| YAML-B39DC08C | 5 |
| GS007 | 2 |
| GS020 | 2 |
| GS025 | 1 |
| GS015 | 1 |
| GS009 | 1 |
| Deep analysis requires OpenRouter API key | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS007 | location_lookupc.py | 37 | Match:                     return pickle.load(f) |
| HIGH | GS025 | railway.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS007 | location_lookupc.py | 37 |
| H | GS025 | railway.json | 0 |
| M | GS010 | supermarket.py | 398 |
| M | GS010 | px_utils.py | 34 |
| M | GS010 | px_utils.py | 97 |
| M | GS010 | px_utils.py | 131 |
| M | GS010 | px_utils.py | 141 |
| M | GS010 | px_utils.py | 168 |
| M | GS010 | px_utils.py | 182 |
| M | GS010 | px_utils.py | 236 |
| M | GS010 | px_utils.py | 240 |
| M | GS010 | walmart_px.py | 357 |
| M | GS007 | location_lookupc.py | 37 |
| L | GS003 | supermarket.py | 132 |
| L | GS003 | supermarket.py | 137 |
| L | GS003 | supermarket.py | 233 |
| L | GS003 | supermarket.py | 236 |
| L | GS003 | supermarket.py | 247 |
| L | GS003 | supermarket.py | 250 |
| L | GS003 | supermarket.py | 264 |
| L | GS003 | supermarket.py | 268 |
| L | GS003 | supermarket.py | 281 |
| L | GS003 | supermarket.py | 310 |
| L | GS003 | supermarket.py | 318 |
| L | GS003 | supermarket.py | 321 |
| L | GS003 | supermarket.py | 331 |
| L | GS003 | supermarket.py | 343 |
| L | GS003 | supermarket.py | 348 |
| L | GS003 | supermarket.py | 367 |
| L | GS003 | supermarket.py | 377 |
| L | GS003 | supermarket.py | 381 |
| L | GS003 | supermarket.py | 385 |
| L | GS003 | supermarket.py | 386 |
| L | GS003 | supermarket.py | 390 |
| L | GS003 | supermarket.py | 396 |
| L | GS003 | supermarket.py | 397 |
| L | GS003 | supermarket.py | 399 |
| L | GS003 | supermarket.py | 402 |
| L | GS003 | supermarket.py | 403 |
| L | GS003 | supermarket.py | 406 |
| L | GS003 | supermarket.py | 612 |
| L | GS003 | supermarket.py | 613 |
| L | GS003 | supermarket.py | 619 |
| L | GS003 | supermarket.py | 628 |
| L | GS003 | supermarket.py | 674 |
| L | GS003 | supermarket.py | 676 |
| L | GS003 | supermarket.py | 678 |
| L | GS003 | supermarket.py | 679 |
| L | GS003 | supermarket.py | 685 |
| L | GS003 | supermarket.py | 687 |
| L | GS003 | supermarket.py | 692 |
| L | GS003 | supermarket.py | 784 |
| L | GS003 | supermarket.py | 786 |
| L | GS003 | supermarket.py | 794 |
| L | GS003 | supermarket.py | 813 |
| L | GS003 | supermarket.py | 821 |
| L | GS003 | supermarket.py | 825 |
| L | GS003 | supermarket.py | 834 |
| L | GS003 | supermarket.py | 839 |
| L | GS003 | supermarket.py | 843 |
| L | GS003 | supermarket.py | 852 |
| L | GS003 | supermarket.py | 1028 |
| L | GS003 | supermarket.py | 1048 |
| L | GS003 | supermarket.py | 1064 |
| L | GS003 | supermarket.py | 1076 |
| L | GS003 | supermarket.py | 1082 |
| L | GS003 | supermarket.py | 1088 |
| L | GS003 | location_lookupc.py | 33 |
| L | GS003 | location_lookupc.py | 36 |
| L | GS003 | helpers.py | 11 |
| L | GS003 | helpers.py | 18 |
| L | GS003 | helpers.py | 50 |
| I | GS015 | app.py | 8 |
| i | GS020 |  | 136 |
| i | GS020 |  | 150 |
| s | GS009 |  | 0 |
| ? | YAML-B39DC08C | supermarket.py | ? |
| ? | YAML-B39DC08C | supermarket.py | ? |
| ? | YAML-B39DC08C | supermarket.py | ? |
| ? | YAML-B39DC08C | supermarket.py | ? |
| ? | YAML-B39DC08C | supermarket.py | ? |
| I | ? |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T06:45:19.930249*