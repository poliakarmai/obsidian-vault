---
title: "GSC Audit: /tmp/gsc-hunt-2"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-2

**Дата:** 11.08.2026 07:05  
**Путь:** `/tmp/gsc-hunt-2`  
**Всего находок:** 121  
**CRITICAL:** 1 | **HIGH:** 7 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS020 | 47 |
| GS015 | 31 |
| GS021 | 20 |
| GS022 | 7 |
| GS025 | 6 |
| YAML-B39DC08C | 4 |
| GS029 | 1 |
| GS009 | 1 |
| GS019 | 1 |
| GS025-wildcard_bind | 1 |
| GS025-no_rate_limit_auth | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS029 | index.html | 945 | Match:       ? `<div class="card-cb-wrap"><input type="check |
| HIGH | GS025 | app.py | 1066 |  |
| HIGH | GS025 | app.py | 1071 |  |
| HIGH | GS025 | app.py | 1073 |  |
| HIGH | GS025 | app.py | 1086 |  |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | pyrightconfig.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS019 | app.py | 2163 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS025 | app.py | 1066 |
| H | GS025 | app.py | 1071 |
| H | GS025 | app.py | 1073 |
| H | GS025 | app.py | 1086 |
| I | GS015 | app.py | 2045 |
| I | GS015 | app.py | 2162 |
| I | GS015 | app.py | 2187 |
| I | GS015 | app.py | 2195 |
| I | GS015 | app.py | 2210 |
| I | GS015 | app.py | 2399 |
| I | GS015 | app.py | 2405 |
| I | GS015 | app.py | 2417 |
| I | GS015 | app.py | 2427 |
| I | GS015 | app.py | 2471 |
| I | GS015 | app.py | 2045 |
| I | GS015 | app.py | 2162 |
| I | GS015 | app.py | 2187 |
| I | GS015 | app.py | 2195 |
| I | GS015 | app.py | 2210 |
| I | GS015 | app.py | 2399 |
| I | GS015 | app.py | 2405 |
| I | GS015 | app.py | 2417 |
| I | GS015 | app.py | 2427 |
| I | GS015 | app.py | 2471 |
| I | GS015 | app.py | 2045 |
| I | GS015 | app.py | 2162 |
| I | GS015 | app.py | 2187 |
| I | GS015 | app.py | 2195 |
| I | GS015 | app.py | 2210 |
| I | GS015 | app.py | 2399 |
| I | GS015 | app.py | 2405 |
| I | GS015 | app.py | 2417 |
| I | GS015 | app.py | 2427 |
| I | GS015 | app.py | 2471 |
| I | GS015 | app.py | 32 |
| i | GS020 |  | 490 |
| i | GS020 |  | 493 |
| i | GS020 |  | 522 |
| i | GS020 |  | 667 |
| i | GS020 |  | 679 |
| i | GS020 |  | 778 |
| i | GS020 |  | 913 |
| i | GS020 |  | 916 |
| i | GS020 |  | 1001 |
| i | GS020 |  | 1009 |
| i | GS020 |  | 1010 |
| i | GS020 |  | 1077 |
| i | GS020 |  | 1101 |
| i | GS020 |  | 1118 |
| i | GS020 |  | 1119 |
| i | GS020 |  | 1124 |
| i | GS020 |  | 1130 |
| i | GS020 |  | 1132 |
| i | GS020 |  | 1140 |
| i | GS020 |  | 1147 |
| i | GS020 |  | 1152 |
| i | GS020 |  | 1294 |
| i | GS020 |  | 1300 |
| i | GS020 |  | 1309 |
| i | GS020 |  | 1312 |
| i | GS020 |  | 1313 |
| i | GS020 |  | 1412 |
| i | GS020 |  | 1420 |
| i | GS020 |  | 1423 |
| i | GS020 |  | 1500 |
| i | GS020 |  | 1520 |
| i | GS020 |  | 496 |
| i | GS020 |  | 500 |
| i | GS020 |  | 568 |
| i | GS020 |  | 571 |
| i | GS020 |  | 775 |
| i | GS020 |  | 980 |
| i | GS020 |  | 985 |
| i | GS020 |  | 985 |
| i | GS020 |  | 985 |
| i | GS020 |  | 1025 |
| i | GS020 |  | 1066 |
| i | GS020 |  | 94 |
| i | GS020 |  | 64 |
| i | GS020 |  | 86 |
| i | GS020 |  | 169 |
| i | GS020 |  | 173 |
| C | GS029 | index.html | 945 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS025 | pyrightconfig.json | 0 |
| s | GS009 |  | 0 |
| H | GS019 | app.py | 2163 |
| c | GS021 |  | 2045 |
| c | GS021 |  | 2162 |
| c | GS021 |  | 2187 |
| c | GS021 |  | 2399 |
| c | GS021 |  | 2405 |
| c | GS021 |  | 2417 |
| c | GS021 |  | 2492 |
| c | GS021 |  | 2624 |
| c | GS021 |  | 2665 |
| c | GS021 |  | 2683 |
| c | GS021 |  | 2764 |
| c | GS021 |  | 2804 |
| c | GS021 |  | 2834 |
| s | GS021 |  | 938 |
| s | GS021 |  | 3137 |
| s | GS021 |  | 1452 |
| s | GS021 |  | 1452 |
| s | GS021 |  | 2384 |
| s | GS021 |  | 1064 |
| s | GS021 |  | 1098 |
| r | GS022 |  | 2176 |
| r | GS022 |  | 825 |
| r | GS022 |  | 839 |
| r | GS022 |  | 847 |
| r | GS022 |  | 1965 |
| r | GS022 |  | 2002 |
| r | GS022 |  | 2765 |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | YAML-B39DC08C | app.py | ? |
| ? | YAML-B39DC08C | app.py | ? |
| ? | YAML-B39DC08C | app.py | ? |
| ? | YAML-B39DC08C | app.py | ? |
| M | ? | app.py | 335 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T07:05:50.697727*