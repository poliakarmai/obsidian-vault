---
title: "GSC Audit: /tmp/gsc-calibration/secrets-demo"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/secrets-demo

**Дата:** 08.08.2026 04:05  
**Путь:** `/tmp/gsc-calibration/secrets-demo`  
**Всего находок:** 12  
**CRITICAL:** 4 | **HIGH:** 2 | **MEDIUM:** 3 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS029 | 4 |
| GS025 | 2 |
| GS001 | 2 |
| GS015 | 1 |
| GS009 | 1 |
| GS017 | 1 |
| GS025-hardcoded_secret | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | app.py | 1 | Found: password = "SuperSecret123!" |
| CRITICAL | GS001 | expected.json | 1 | Found: "GS029" |
| CRITICAL | GS029 | app.py | 1 | Match: password = "SuperSecret123!" |
| CRITICAL | GS029 | app.py | 2 | Match: api_key = "sk_live_abcdef" |
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS017 | app.py | 1 | Password variable with short value (15 chars). |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS025 | app.py | 1 |
| M | GS029 | app.py | 1 |
| M | GS029 | app.py | 2 |
| C | GS001 | app.py | 1 |
| C | GS001 | expected.json | 1 |
| I | GS015 | app.py | 1 |
| C | GS029 | app.py | 1 |
| C | GS029 | app.py | 2 |
| H | GS025 | expected.json | 0 |
| s | GS009 |  | 0 |
| H | GS017 | app.py | 1 |
| ? | GS025-hardcoded_secret |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:05:21.481720*