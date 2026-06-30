---
title: "GSC Audit: receipts"
date: 2026-06-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — receipts

**Дата:** 27.06.2026 10:13  
**Путь:** `/tmp/gsc-zero-star/receipts`  
**Всего находок:** 4  
**CRITICAL:** 0 | **HIGH:** 4 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Хардкод IP адреса | 2 |
| World-readable file: docker-compose.yml (664) | 1 |
| GS002 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | main.py | 12 | Match:     allow_origins=[FRONTEND_URL, "http://localhost:30 |
| HIGH | ? | Dockerfile | 7 | Match: CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--p |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | nginx.conf | 0 | File nginx.conf has permissions -rw-rw-r-- — readable by any |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | main.py | 12 |
| H | ? | Dockerfile | 7 |
| H | ? | docker-compose.yml | 0 |
| H | GS002 | nginx.conf | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-27T10:13:01.715991*