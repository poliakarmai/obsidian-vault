---
title: "GSC Audit: reg-risk"
date: 2026-06-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — reg-risk

**Дата:** 27.06.2026 10:13  
**Путь:** `/tmp/gsc-zero-star/reg-risk`  
**Всего находок:** 76  
**CRITICAL:** 0 | **HIGH:** 7 | **MEDIUM:** 0 | **LOW:** 69

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 10 |
| Хардкод IP адреса | 5 |
| Generic code smell #24 | 1 |
| Generic code smell #27 | 1 |
| Generic code smell #30 | 1 |
| Generic code smell #33 | 1 |
| Generic code smell #36 | 1 |
| Generic code smell #39 | 1 |
| Generic code smell #42 | 1 |
| Generic code smell #45 | 1 |
| Generic code smell #48 | 1 |
| Generic code smell #51 | 1 |
| Generic code smell #54 | 1 |
| Generic code smell #57 | 1 |
| Generic code smell #60 | 1 |
| Generic code smell #63 | 1 |
| Generic code smell #66 | 1 |
| Generic code smell #69 | 1 |
| Generic code smell #72 | 1 |
| Generic code smell #75 | 1 |
| Generic code smell #78 | 1 |
| Generic code smell #81 | 1 |
| Generic code smell #84 | 1 |
| Generic code smell #87 | 1 |
| Generic code smell #90 | 1 |
| Generic code smell #93 | 1 |
| Generic code smell #96 | 1 |
| Generic code smell #99 | 1 |
| Generic code smell #102 | 1 |
| Generic code smell #105 | 1 |
| Generic code smell #108 | 1 |
| Generic code smell #111 | 1 |
| Generic code smell #114 | 1 |
| Generic code smell #117 | 1 |
| Generic code smell #120 | 1 |
| Generic code smell #123 | 1 |
| Generic code smell #126 | 1 |
| Generic code smell #129 | 1 |
| Generic code smell #132 | 1 |
| Generic code smell #135 | 1 |
| Generic code smell #138 | 1 |
| Generic code smell #141 | 1 |
| Generic code smell #144 | 1 |
| Generic code smell #147 | 1 |
| Generic code smell #150 | 1 |
| Generic code smell #153 | 1 |
| Generic code smell #156 | 1 |
| Generic code smell #159 | 1 |
| Generic code smell #162 | 1 |
| Generic code smell #165 | 1 |
| Generic code smell #168 | 1 |
| Generic code smell #171 | 1 |
| Generic code smell #174 | 1 |
| Generic code smell #177 | 1 |
| Generic code smell #180 | 1 |
| Generic code smell #183 | 1 |
| Generic code smell #186 | 1 |
| Generic code smell #189 | 1 |
| Generic code smell #192 | 1 |
| Generic code smell #195 | 1 |
| Generic code smell #198 | 1 |
| World-readable file: vercel.json (664) | 1 |
| World-readable file: render.yaml (664) | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | render.yaml | 6 | Match:     startCommand: gunicorn app:app --bind 0.0.0.0:$PO |
| HIGH | ? | app.py | 44 | Match: CORS(app, resources={r"/api/*": {"origins": ["http:// |
| HIGH | ? | app.py | 752 | Match:     app.run(host='0.0.0.0', port=port, debug=False) |
| HIGH | ? | index.html | 767 | Match:         const IS_LOCAL = window.location.hostname === |
| HIGH | ? | Procfile | 1 | Match: web: gunicorn app:app --bind 0.0.0.0:$PORT |
| HIGH | ? | vercel.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | render.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | ? | rule_engine.py | 199 |
| L | GS003 | app.py | 246 |
| L | GS003 | app.py | 427 |
| L | GS003 | app.py | 745 |
| L | GS003 | app.py | 746 |
| L | GS003 | app.py | 747 |
| L | GS003 | app.py | 748 |
| L | GS003 | app.py | 749 |
| L | GS003 | app.py | 750 |
| L | GS003 | app.py | 751 |
| L | GS003 | audit_logger.py | 207 |
| H | ? | render.yaml | 6 |
| H | ? | app.py | 44 |
| H | ? | app.py | 752 |
| H | ? | index.html | 767 |
| H | ? | Procfile | 1 |
| H | ? | vercel.json | 0 |
| H | ? | render.yaml | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-27T10:13:10.319222*