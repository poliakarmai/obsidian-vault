---
title: "GSC Audit: /home/openclaw/gsc/corpus/gs007_bac"
date: 2026-07-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc/corpus/gs007_bac

**Дата:** 29.07.2026 20:04  
**Путь:** `/home/openclaw/gsc/corpus/gs007_bac`  
**Всего находок:** 19  
**CRITICAL:** 0 | **HIGH:** 12 | **MEDIUM:** 0 | **LOW:** 2

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS007 | 15 |
| Python: File upload without content-type validation | 1 |
| GS003 | 1 |
| GS008 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | fastapi_support.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | GS007 | batch_and_override.py | 31 | Line 31: Order.objects.bulk_create(  # GS007: batch operatio |
| HIGH | GS007 | batch_and_override.py | 39 | Line 39: HTTP_METHOD_OVERRIDE = "X-HTTP-Method-Override"  #  |
| HIGH | GS007 | batch_and_override.py | 39 | Line 39: HTTP_METHOD_OVERRIDE = "X-HTTP-Method-Override"  #  |
| HIGH | GS007 | batch_and_override.py | 44 | Line 44: _method = request.POST.get("_method", request.metho |
| HIGH | GS007 | batch_and_override.py | 44 | Line 44: _method = request.POST.get("_method", request.metho |
| HIGH | GS007 | batch_and_override.py | 45 | Line 45: if _method == "DELETE": |
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
| L | GS008 | batch_and_override.py | 39 |
| H | GS007 | batch_and_override.py | 31 |
| H | GS007 | batch_and_override.py | 39 |
| H | GS007 | batch_and_override.py | 39 |
| H | GS007 | batch_and_override.py | 44 |
| H | GS007 | batch_and_override.py | 44 |
| H | GS007 | batch_and_override.py | 45 |
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
*Сгенерировано GSC v0.6 · 2026-07-29T20:04:47.916396*