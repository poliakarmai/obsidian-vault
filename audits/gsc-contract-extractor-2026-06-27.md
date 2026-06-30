---
title: "GSC Audit: contract-extractor"
date: 2026-06-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — contract-extractor

**Дата:** 27.06.2026 10:13  
**Путь:** `/tmp/gsc-zero-star/contract-extractor`  
**Всего находок:** 34  
**CRITICAL:** 2 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 30

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 30 |
| GS001 | 2 |
| Хардкод IP адреса | 2 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | connection.py | 7 | Found: sqlite:///./data/po_databa |
| CRITICAL | GS001 | connection.py | 7 | Found: DATABASE_URL = "sqlite:///./data/po_database.db" |
| HIGH | ? | icons.svg | 7 | Match:     <path fill="#08060d" d="M16.224 3.768a14.5 14.5 0 |
| HIGH | ? | icons.svg | 22 | Match:     <path fill="#08060d" fill-rule="evenodd" d="M1.89 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | connection.py | 7 |
| C | GS001 | connection.py | 7 |
| L | GS003 | check_db.py | 10 |
| L | GS003 | check_db.py | 14 |
| L | GS003 | check_db.py | 15 |
| L | GS003 | check_db.py | 16 |
| L | GS003 | check_db.py | 17 |
| L | GS003 | check_db.py | 18 |
| L | GS003 | delete_data.py | 12 |
| L | GS003 | delete_data.py | 15 |
| L | GS003 | delete_data.py | 22 |
| L | GS003 | delete_data.py | 25 |
| L | GS003 | delete_data.py | 29 |
| L | GS003 | benchmark_text.py | 12 |
| L | GS003 | benchmark_text.py | 40 |
| L | GS003 | benchmark_text.py | 79 |
| L | GS003 | benchmark_text.py | 82 |
| L | GS003 | benchmark_text.py | 85 |
| L | GS003 | benchmark_text.py | 87 |
| L | GS003 | extraction.py | 9 |
| L | GS003 | extraction.py | 81 |
| L | GS003 | models.py | 9 |
| L | GS003 | models.py | 14 |
| L | GS003 | models.py | 16 |
| L | GS003 | models.py | 46 |
| L | GS003 | main.py | 66 |
| L | GS003 | main.py | 90 |
| L | GS003 | main.py | 160 |
| L | GS003 | main.py | 213 |
| L | GS003 | main.py | 215 |
| L | GS003 | patch_db.py | 12 |
| L | GS003 | patch_db.py | 14 |
| H | ? | icons.svg | 7 |
| H | ? | icons.svg | 22 |

---
*Сгенерировано GSC v0.6 · 2026-06-27T10:13:00.691705*