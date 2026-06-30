---
title: "GSC Audit: social-media-platform-backend"
date: 2026-06-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — social-media-platform-backend

**Дата:** 27.06.2026 10:12  
**Путь:** `/tmp/gsc-zero-star/social-media-platform-backend`  
**Всего находок:** 6  
**CRITICAL:** 0 | **HIGH:** 6 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: File upload without content-type validation | 6 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | views.py | 16 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 62 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 12 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 13 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 14 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 59 | File upload without MIME-type validation → malicious file up |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | views.py | 16 |
| H | ? | views.py | 62 |
| H | ? | models.py | 12 |
| H | ? | views.py | 13 |
| H | ? | views.py | 14 |
| H | ? | views.py | 59 |

---
*Сгенерировано GSC v0.6 · 2026-06-27T10:12:59.519986*