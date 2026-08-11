---
title: "GSC Audit: /tmp/tmpb2ys9j41"
date: 2026-08-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpb2ys9j41

**Дата:** 06.08.2026 21:48  
**Путь:** `/tmp/tmpb2ys9j41`  
**Всего находок:** 7  
**CRITICAL:** 3 | **HIGH:** 0 | **MEDIUM:** 0 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS001 | 2 |
| CVE-2026-56413: Command injection | 1 |
| GS003 | 1 |
| GS015 | 1 |
| GS009 | 1 |
| GS025-hardcoded_secret | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | app.py | 7 |  |
| CRITICAL | GS001 | app.py | 4 | Found: API_KEY = "sk-abcdef12345678901234567890abcdef1234567 |
| CRITICAL | GS001 | app.py | 4 | Found: sk-abcdef12345678901234567890abcdef1234567890 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | app.py | 7 |
| C | GS001 | app.py | 4 |
| C | GS001 | app.py | 4 |
| L | GS003 | app.py | 9 |
| I | GS015 | app.py | 1 |
| s | GS009 |  | 0 |
| ? | GS025-hardcoded_secret |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-06T21:48:18.497784*