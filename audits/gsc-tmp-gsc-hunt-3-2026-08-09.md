---
title: "GSC Audit: /tmp/gsc-hunt-3"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-3

**Дата:** 09.08.2026 09:51  
**Путь:** `/tmp/gsc-hunt-3`  
**Всего находок:** 14  
**CRITICAL:** 0 | **HIGH:** 10 | **MEDIUM:** 2 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS018 | 6 |
| GS025 | 5 |
| GS029 | 1 |
| GS007 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | mcp_server.py | 134 |  |
| HIGH | GS025 | mcp_server.py | 275 |  |
| HIGH | GS025 | mcp_server.py | 304 |  |
| HIGH | GS025 | mcp_server.py | 352 |  |
| HIGH | GS018 | mcp_server.py | 108 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | mcp_server.py | 120 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | mcp_server.py | 141 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | mcp_server.py | 181 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | mcp_server.py | 206 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | mcp_server.py | 234 | Float arithmetic for money leads to rounding errors exploita |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS025 | mcp_server.py | 134 |
| H | GS025 | mcp_server.py | 275 |
| H | GS025 | mcp_server.py | 304 |
| H | GS025 | mcp_server.py | 352 |
| M | GS025 | mcp_server.py | 197 |
| M | GS029 | mcp_server.py | 197 |
| I | GS007 | middleware.py | 77 |
| s | GS009 |  | 0 |
| H | GS018 | mcp_server.py | 108 |
| H | GS018 | mcp_server.py | 120 |
| H | GS018 | mcp_server.py | 141 |
| H | GS018 | mcp_server.py | 181 |
| H | GS018 | mcp_server.py | 206 |
| H | GS018 | mcp_server.py | 234 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T09:51:38.969995*