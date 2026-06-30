---
title: "GSC Audit: AI-Scene-Intelligence-Engine"
date: 2026-06-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — AI-Scene-Intelligence-Engine

**Дата:** 27.06.2026 10:12  
**Путь:** `/tmp/gsc-zero-star/AI-Scene-Intelligence-Engine`  
**Всего находок:** 15  
**CRITICAL:** 0 | **HIGH:** 3 | **MEDIUM:** 1 | **LOW:** 11

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 11 |
| Bare except: | 1 |
| Python: SSRF via requests without URL validation | 1 |
| Хардкод IP адреса | 1 |
| User-controlled URL in request | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | streamlit_app.py | 13 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | streamlit_app.py | 4 | Match: API_URL = "http://127.0.0.1:8000" |
| HIGH | ? | streamlit_app.py | 13 | Match:     requests.get(f"{API_URL}/load") |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | streamlit_app.py | 14 |
| H | ? | streamlit_app.py | 13 |
| L | GS003 | parser.py | 78 |
| L | GS003 | parser.py | 86 |
| L | GS003 | parser.py | 88 |
| L | GS003 | parser.py | 90 |
| L | GS003 | retrieval.py | 18 |
| L | GS003 | retrieval.py | 20 |
| L | GS003 | retrieval.py | 27 |
| L | GS003 | retrieval.py | 34 |
| L | GS003 | retrieval.py | 38 |
| L | GS003 | retrieval.py | 51 |
| L | GS003 | retrieval.py | 59 |
| H | ? | streamlit_app.py | 4 |
| H | ? | streamlit_app.py | 13 |

---
*Сгенерировано GSC v0.6 · 2026-06-27T10:12:58.459143*