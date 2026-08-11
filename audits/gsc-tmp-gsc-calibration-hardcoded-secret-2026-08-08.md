---
title: "GSC Audit: /tmp/gsc-calibration/hardcoded-secret"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/hardcoded-secret

**Дата:** 08.08.2026 04:05  
**Путь:** `/tmp/gsc-calibration/hardcoded-secret`  
**Всего находок:** 9  
**CRITICAL:** 3 | **HIGH:** 2 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS029 | 2 |
| GS001 | 2 |
| GS015 | 1 |
| GS025 | 1 |
| GS009 | 1 |
| GS017 | 1 |
| GS025-hardcoded_secret | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | app.py | 1 | Found: TOKEN="ghp_abc123def456" |
| CRITICAL | GS001 | expected.json | 1 | Found: "GS029" |
| CRITICAL | GS029 | app.py | 2 | Match: secret="mysecret" |
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS017 | app.py | 2 | Password variable with short value (8 chars). |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS029 | app.py | 2 |
| C | GS001 | app.py | 1 |
| C | GS001 | expected.json | 1 |
| I | GS015 | app.py | 1 |
| C | GS029 | app.py | 2 |
| H | GS025 | expected.json | 0 |
| s | GS009 |  | 0 |
| H | GS017 | app.py | 2 |
| ? | GS025-hardcoded_secret |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:05:14.296410*