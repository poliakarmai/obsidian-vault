---
title: "GSC Audit: /tmp/pwned_robot"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/pwned_robot

**Дата:** 11.08.2026 05:38  
**Путь:** `/tmp/pwned_robot`  
**Всего находок:** 21  
**CRITICAL:** 3 | **HIGH:** 1 | **MEDIUM:** 6 | **LOW:** 3

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 4 |
| GS029 | 3 |
| GS008 | 3 |
| GS021 | 3 |
| GS022 | 3 |
| GS010 | 1 |
| GS025 | 1 |
| GS015 | 1 |
| GS009 | 1 |
| GS018 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS029 | handlers.py | 522 | Match:         key = "unmonitor_removed" if removed else "un |
| CRITICAL | GS000-LEGACY | config.py | 19 | Match:     TELEGRAM_TOKEN: str = Field(..., min_length=1) |
| CRITICAL | GS000-LEGACY | config.py | 26 | Match:     DB_PASSWORD: str = Field(..., min_length=1) |
| HIGH | GS018 | handlers.py | 611 | Cancel/refund function lacks state check. Risk: refund after |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS010 | security.py | 291 |
| M | GS025 | handlers.py | 387 |
| M | GS029 | handlers.py | 387 |
| M | GS029 | handlers.py | 522 |
| L | GS008 | handlers.py | 26 |
| L | GS008 | scheduler.py | 19 |
| L | GS008 | strings.py | 14 |
| I | GS015 | main.py | 193 |
| C | GS029 | handlers.py | 522 |
| C | GS000-LEGACY | config.py | 19 |
| C | GS000-LEGACY | config.py | 26 |
| M | GS000-LEGACY | setup_service.sh | 132 |
| M | GS000-LEGACY | setup_service.sh | 119 |
| s | GS009 |  | 0 |
| H | GS018 | handlers.py | 611 |
| s | GS021 |  | 23 |
| s | GS021 |  | 38 |
| s | GS021 |  | 198 |
| r | GS022 |  | 75 |
| r | GS022 |  | 83 |
| r | GS022 |  | 62 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T05:38:57.029801*