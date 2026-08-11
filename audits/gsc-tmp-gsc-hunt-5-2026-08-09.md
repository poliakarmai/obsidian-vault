---
title: "GSC Audit: /tmp/gsc-hunt-5"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-5

**Дата:** 09.08.2026 12:04  
**Путь:** `/tmp/gsc-hunt-5`  
**Всего находок:** 33  
**CRITICAL:** 0 | **HIGH:** 9 | **MEDIUM:** 0 | **LOW:** 10

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 10 |
| GS015 | 5 |
| GS002 | 5 |
| GS007 | 3 |
| GS025-eval_usage | 2 |
| YAML-36ACF0AD | 2 |
| GS020 | 1 |
| GS025 | 1 |
| GS009 | 1 |
| GS021 | 1 |
| GS022 | 1 |
| GS025-debug_mode | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | internal.conf | 0 | File internal.conf has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | pushpin.conf | 0 | File pushpin.conf has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | internal.conf | 0 | File internal.conf has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | pushpin.conf | 0 | File pushpin.conf has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | supervisord.conf | 0 | File supervisord.conf has permissions -rw-rw-r-- — readable  |
| HIGH | GS007 | pollymer-1.1.1.js | 216 | Line 216: this._method = null; |
| HIGH | GS007 | pollymer-1.1.1.js | 267 | Line 267: this._method = method; |
| HIGH | GS007 | pollymer-1.1.1.js | 475 | Line 475: paramList.push("_method=" + encodeURIComponent(met |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS003 | cleanup.py | 10 |
| L | GS003 | cleanup.py | 14 |
| L | GS003 | cleanup.py | 23 |
| L | GS003 | WebhookInboxViewer.js | 13 |
| L | GS003 | WebhookInboxViewer.js | 22 |
| L | GS003 | WebhookInboxViewer.js | 25 |
| L | GS003 | WebhookInboxViewer.js | 30 |
| L | GS003 | WebhookInboxViewer.js | 46 |
| L | GS003 | pollymer-1.1.1.js | 33 |
| L | GS003 | pollymer-1.1.1.js | 36 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 22 |
| I | GS015 | wsgi.py | 25 |
| I | GS015 | urls.py | 1 |
| i | GS020 |  | 471 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS002 | internal.conf | 0 |
| H | GS002 | pushpin.conf | 0 |
| H | GS002 | internal.conf | 0 |
| H | GS002 | pushpin.conf | 0 |
| H | GS002 | supervisord.conf | 0 |
| H | GS007 | pollymer-1.1.1.js | 216 |
| H | GS007 | pollymer-1.1.1.js | 267 |
| H | GS007 | pollymer-1.1.1.js | 475 |
| s | GS009 |  | 0 |
| s | GS021 |  | 27 |
| r | GS022 |  | 323 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | YAML-36ACF0AD | json2.js | ? |
| ? | YAML-36ACF0AD | json2.js | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-09T12:04:12.817471*