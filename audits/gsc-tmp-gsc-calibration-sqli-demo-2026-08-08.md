---
title: "GSC Audit: /tmp/gsc-calibration/sqli-demo"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/sqli-demo

**Дата:** 08.08.2026 04:05  
**Путь:** `/tmp/gsc-calibration/sqli-demo`  
**Всего находок:** 8  
**CRITICAL:** 5 | **HIGH:** 1 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS005 | 3 |
| GS001 | 1 |
| GS015 | 1 |
| GS025 | 1 |
| GS009 | 1 |
| GS024 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | app.py | 2 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 2 |  |
| CRITICAL | GS001 | expected.json | 1 | Found: "GS005" |
| CRITICAL | GS005 | app.py | 2 | Line 2: return db.execute(f"SELECT * FROM u WHERE id={x}") |
| CRITICAL | GS024 | app.py | 2 | LLM confidence: 100%. The f-string directly interpolates the |
| HIGH | GS025 | expected.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | app.py | 2 |
| C | GS005 | app.py | 2 |
| C | GS001 | expected.json | 1 |
| I | GS015 | app.py | 1 |
| H | GS025 | expected.json | 0 |
| C | GS005 | app.py | 2 |
| s | GS009 |  | 0 |
| C | GS024 | app.py | 2 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:05:25.179113*