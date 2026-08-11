---
title: "GSC Audit: /tmp/gsc-external/CPA-X"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/CPA-X

**Дата:** 09.08.2026 06:28  
**Путь:** `/tmp/gsc-external/CPA-X`  
**Всего находок:** 197  
**CRITICAL:** 1 | **HIGH:** 11 | **MEDIUM:** 22 | **LOW:** 54

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 54 |
| GS020 | 34 |
| GS015 | 31 |
| GS021 | 30 |
| GS029 | 16 |
| GS025 | 12 |
| GS022 | 9 |
| Синхронный код в async | 4 |
| YAML-B39DC08C | 2 |
| GS018 | 1 |
| GS000-LEGACY | 1 |
| GS009 | 1 |
| GS025-no_rate_limit_auth | 1 |
| Deep analysis requires OpenRouter API key | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS025 | auto_install.py | 107 | Match:         os.chmod(temp_name, 0o644) |
| HIGH | GS025 | auto_install.py | 143 |  |
| HIGH | GS025 | auto_install.py | 160 |  |
| HIGH | GS025 | auto_install.py | 161 |  |
| HIGH | GS025 | auto_install.py | 162 |  |
| HIGH | GS025 | auto_install.py | 167 |  |
| HIGH | GS025 | auto_install.py | 169 |  |
| HIGH | GS025 | auto_install.py | 170 |  |
| HIGH | GS025 | auto_install.py | 171 |  |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | install.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS018 | app.py | 3181 | Cancel/refund function lacks state check. Risk: refund after |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS025 | auto_install.py | 107 |
| H | GS025 | auto_install.py | 143 |
| H | GS025 | auto_install.py | 160 |
| H | GS025 | auto_install.py | 161 |
| H | GS025 | auto_install.py | 162 |
| H | GS025 | auto_install.py | 167 |
| H | GS025 | auto_install.py | 169 |
| H | GS025 | auto_install.py | 170 |
| H | GS025 | auto_install.py | 171 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS025 | install.json | 0 |
| H | GS018 | app.py | 3181 |
| M | GS025 | app.py | 2144 |
| M | GS029 | app.py | 1273 |
| M | GS029 | app.py | 1505 |
| M | GS029 | app.py | 2024 |
| M | GS029 | app.py | 2144 |
| M | GS029 | app.py | 2165 |
| M | GS029 | app.py | 2261 |
| M | GS029 | app.py | 2328 |
| M | GS029 | app.py | 2461 |
| M | GS029 | app.py | 2683 |
| M | GS029 | app.py | 2698 |
| M | GS029 | app.py | 2825 |
| M | GS029 | app.py | 3711 |
| M | GS029 | app.py | 3776 |
| M | GS029 | app.py | 3888 |
| M | GS029 | app.py | 4040 |
| M | GS029 | app.py | 4380 |
| L | GS003 | app.py | 75 |
| L | GS003 | app.py | 82 |
| L | GS003 | app.py | 258 |
| L | GS003 | app.py | 372 |
| L | GS003 | app.py | 519 |
| L | GS003 | app.py | 612 |
| L | GS003 | app.py | 630 |
| L | GS003 | app.py | 844 |
| L | GS003 | app.py | 847 |
| L | GS003 | app.py | 884 |
| L | GS003 | app.py | 895 |
| L | GS003 | app.py | 1083 |
| L | GS003 | app.py | 1096 |
| L | GS003 | app.py | 1128 |
| L | GS003 | app.py | 1150 |
| L | GS003 | app.py | 1171 |
| L | GS003 | app.py | 1525 |
| L | GS003 | app.py | 1795 |
| L | GS003 | app.py | 1839 |
| L | GS003 | app.py | 1984 |
| L | GS003 | app.py | 2004 |
| L | GS003 | app.py | 2188 |
| L | GS003 | app.py | 2727 |
| L | GS003 | app.py | 2750 |
| L | GS003 | app.py | 3330 |
| L | GS003 | app.py | 3419 |
| L | GS003 | app.py | 3556 |
| L | GS003 | app.py | 3560 |
| L | GS003 | app.py | 3566 |
| L | GS003 | app.py | 3571 |
| L | GS003 | app.py | 3580 |
| L | GS003 | app.py | 3583 |
| L | GS003 | app.py | 3589 |
| L | GS003 | app.py | 3762 |
| L | GS003 | app.py | 4650 |
| L | GS003 | app.py | 4672 |
| L | GS003 | app.py | 4893 |
| L | GS003 | app.py | 4984 |
| L | GS003 | app.py | 5010 |
| L | GS003 | app.py | 5026 |
| L | GS003 | app.py | 5056 |
| L | GS003 | app.py | 5072 |
| L | GS003 | app.py | 5100 |
| L | GS003 | app.py | 5162 |
| L | GS003 | app.py | 5230 |
| L | GS003 | app.py | 5361 |
| L | GS003 | app.py | 5553 |
| L | GS003 | app.py | 5595 |
| L | GS003 | app.py | 5601 |
| L | GS003 | app.py | 5612 |
| L | GS003 | auto_install.py | 64 |
| L | GS003 | doctor.py | 356 |
| L | GS003 | doctor.py | 359 |
| L | GS003 | doctor.py | 365 |
| I | GS015 | app.py | 4436 |
| I | GS015 | app.py | 4441 |
| I | GS015 | app.py | 4453 |
| I | GS015 | app.py | 4552 |
| I | GS015 | app.py | 4557 |
| I | GS015 | app.py | 4566 |
| I | GS015 | app.py | 4599 |
| I | GS015 | app.py | 4609 |
| I | GS015 | app.py | 4614 |
| I | GS015 | app.py | 4675 |
| I | GS015 | app.py | 4436 |
| I | GS015 | app.py | 4441 |
| I | GS015 | app.py | 4453 |
| I | GS015 | app.py | 4552 |
| I | GS015 | app.py | 4557 |
| I | GS015 | app.py | 4566 |
| I | GS015 | app.py | 4599 |
| I | GS015 | app.py | 4609 |
| I | GS015 | app.py | 4614 |
| I | GS015 | app.py | 4675 |
| I | GS015 | app.py | 4436 |
| I | GS015 | app.py | 4441 |
| I | GS015 | app.py | 4453 |
| I | GS015 | app.py | 4552 |
| I | GS015 | app.py | 4557 |
| I | GS015 | app.py | 4566 |
| I | GS015 | app.py | 4599 |
| I | GS015 | app.py | 4609 |
| I | GS015 | app.py | 4614 |
| I | GS015 | app.py | 4675 |
| I | GS015 | app.py | 91 |
| i | GS020 |  | 1921 |
| i | GS020 |  | 2256 |
| i | GS020 |  | 2284 |
| i | GS020 |  | 2303 |
| i | GS020 |  | 2309 |
| i | GS020 |  | 2331 |
| i | GS020 |  | 2395 |
| i | GS020 |  | 2396 |
| i | GS020 |  | 2397 |
| i | GS020 |  | 2403 |
| i | GS020 |  | 2404 |
| i | GS020 |  | 2405 |
| i | GS020 |  | 2552 |
| i | GS020 |  | 2732 |
| i | GS020 |  | 2778 |
| i | GS020 |  | 2797 |
| i | GS020 |  | 2809 |
| i | GS020 |  | 2816 |
| i | GS020 |  | 2888 |
| i | GS020 |  | 2889 |
| i | GS020 |  | 2896 |
| i | GS020 |  | 2897 |
| i | GS020 |  | 2904 |
| i | GS020 |  | 2922 |
| i | GS020 |  | 2927 |
| i | GS020 |  | 3072 |
| i | GS020 |  | 3074 |
| i | GS020 |  | 3077 |
| i | GS020 |  | 1995 |
| i | GS020 |  | 2007 |
| i | GS020 |  | 2825 |
| i | GS020 |  | 2828 |
| i | GS020 |  | 2831 |
| i | GS020 |  | 2842 |
| M | GS000-LEGACY | auto_install.py | 33 |
| s | GS009 |  | 0 |
| c | GS021 |  | 4566 |
| c | GS021 |  | 4675 |
| c | GS021 |  | 4707 |
| c | GS021 |  | 4725 |
| c | GS021 |  | 4739 |
| c | GS021 |  | 4754 |
| c | GS021 |  | 4771 |
| c | GS021 |  | 4793 |
| c | GS021 |  | 4839 |
| c | GS021 |  | 4868 |
| c | GS021 |  | 4899 |
| c | GS021 |  | 5029 |
| c | GS021 |  | 5077 |
| c | GS021 |  | 5105 |
| c | GS021 |  | 5124 |
| c | GS021 |  | 5188 |
| c | GS021 |  | 5267 |
| c | GS021 |  | 5364 |
| c | GS021 |  | 5428 |
| s | GS021 |  | 117 |
| s | GS021 |  | 141 |
| s | GS021 |  | 556 |
| s | GS021 |  | 626 |
| s | GS021 |  | 951 |
| s | GS021 |  | 4310 |
| s | GS021 |  | 4310 |
| s | GS021 |  | 5599 |
| s | GS021 |  | 558 |
| s | GS021 |  | 288 |
| s | GS021 |  | 290 |
| r | GS022 |  | 553 |
| r | GS022 |  | 576 |
| r | GS022 |  | 949 |
| r | GS022 |  | 950 |
| r | GS022 |  | 1308 |
| r | GS022 |  | 2249 |
| r | GS022 |  | 3009 |
| r | GS022 |  | 5353 |
| r | GS022 |  | 5454 |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | YAML-B39DC08C | app.py | ? |
| ? | YAML-B39DC08C | doctor.py | ? |
| M | ? | auto_install.py | 14 |
| M | ? | auto_install.py | 57 |
| M | ? | doctor.py | 38 |
| M | ? | app.py | 1897 |
| I | ? |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T06:28:10.404291*