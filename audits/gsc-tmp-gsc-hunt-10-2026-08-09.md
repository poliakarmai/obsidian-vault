---
title: "GSC Audit: /tmp/gsc-hunt-10"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-10

**Дата:** 09.08.2026 09:55  
**Путь:** `/tmp/gsc-hunt-10`  
**Всего находок:** 31  
**CRITICAL:** 1 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 11

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 11 |
| GS020 | 8 |
| GS022 | 7 |
| GS025 | 2 |
| GS005 | 1 |
| GS009 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | coordinator.py | 1157 | OWASP A03: Injection |
| HIGH | GS025 | manifest.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | services.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | coordinator.py | 1157 |
| L | GS003 | reolink-recording-card.js | 82 |
| L | GS003 | reolink-recording-card.js | 100 |
| L | GS003 | reolink-recording-card.js | 145 |
| L | GS003 | reolink-recording-card.js | 336 |
| L | GS003 | reolink-recording-card.js | 352 |
| L | GS003 | reolink-recording-card.js | 384 |
| L | GS003 | reolink-recording-card.js | 455 |
| L | GS003 | reolink-recording-card.js | 468 |
| L | GS003 | reolink-recording-card.js | 478 |
| L | GS003 | reolink-recording-card.js | 490 |
| L | GS003 | reolink-recording-card.js | 543 |
| i | GS020 |  | 146 |
| i | GS020 |  | 408 |
| i | GS020 |  | 650 |
| i | GS020 |  | 207 |
| i | GS020 |  | 218 |
| i | GS020 |  | 577 |
| i | GS020 |  | 626 |
| i | GS020 |  | 694 |
| H | GS025 | manifest.json | 0 |
| H | GS025 | services.yaml | 0 |
| s | GS009 |  | 0 |
| s | GS021 |  | 87 |
| r | GS022 |  | 699 |
| r | GS022 |  | 898 |
| r | GS022 |  | 65 |
| r | GS022 |  | 171 |
| r | GS022 |  | 192 |
| r | GS022 |  | 502 |
| r | GS022 |  | 503 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T09:55:24.917951*