---
title: "GSC Audit: /home/openclaw/gsc/corpus/gs007_bac"
date: 2026-07-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc/corpus/gs007_bac

**Дата:** 28.07.2026 19:18  
**Путь:** `/home/openclaw/gsc/corpus/gs007_bac`  
**Всего находок:** 12  
**CRITICAL:** 0 | **HIGH:** 6 | **MEDIUM:** 0 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS007 | 9 |
| Python: File upload without content-type validation | 1 |
| GS003 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | fastapi_support.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | GS007 | express_files.js | 17 | Line 17: Ticket.findById(req.params.id).then(ticket => {  // |
| HIGH | GS007 | express_files.js | 12 | Line 12: res.sendFile(`/uploads/${req.params.fileId}`);  //  |
| HIGH | GS007 | fastapi_support.py | 35 | Line 35: @app.get("/attachments/{file_id}")  # GS007: file e |
| HIGH | GS007 | laravel_tickets.php | 29 | Line 29: $ticket->add_subscriber($request->user());  // GS00 |
| HIGH | GS007 | schema.sql | 12 | Line 12: SELECT * FROM tickets WHERE user_id = $1;  -- GS007 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | fastapi_support.py | 38 |
| L | GS003 | django_cross_org.py | 33 |
| I | GS007 | django_cross_org.py | 13 |
| H | GS007 | express_files.js | 17 |
| H | GS007 | express_files.js | 12 |
| H | GS007 | fastapi_support.py | 35 |
| H | GS007 | laravel_tickets.php | 29 |
| I | GS007 | schema.sql | 6 |
| I | GS007 | schema.sql | 6 |
| I | GS007 | schema.sql | 6 |
| H | GS007 | schema.sql | 12 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-28T19:18:36.319061*