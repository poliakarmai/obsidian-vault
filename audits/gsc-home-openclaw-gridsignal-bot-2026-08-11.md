---
title: "GSC Audit: /home/openclaw/gridsignal-bot"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gridsignal-bot

**Дата:** 11.08.2026 09:16  
**Путь:** `/home/openclaw/gridsignal-bot`  
**Всего находок:** 39  
**CRITICAL:** 0 | **HIGH:** 14 | **MEDIUM:** 10 | **LOW:** 1

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS007 | 9 |
| GS018 | 7 |
| GS020 | 6 |
| Синхронный код в async | 6 |
| YAML-B39DC08C | 4 |
| GS029 | 3 |
| GS025 | 1 |
| GS008 | 1 |
| GS009 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS007 | gridsignal-bot.py | 124 | Line 124: "SELECT 1 FROM pro_users WHERE user_id=? AND activ |
| HIGH | GS007 | gridsignal-bot.py | 224 | Line 224: row = conn.execute('SELECT user_id, username, firs |
| HIGH | GS007 | gridsignal-bot.py | 365 | Line 365: row = conn.execute('SELECT lang FROM users WHERE u |
| HIGH | GS007 | gridsignal-bot.py | 1039 | Line 1039: "SELECT paid_at, expires_at, active FROM pro_user |
| HIGH | GS007 | gridsignal-bot.py | 1222 | Line 1222: 'SELECT outcome, pnl_pct FROM signals WHERE user_ |
| HIGH | GS007 | gridsignal-bot.py | 1256 | Line 1256: alerts = conn.execute('SELECT symbol FROM alerts  |
| HIGH | GS007 | gridsignal-bot.py | 1287 | Line 1287: alert_count = conn.execute('SELECT COUNT(*) FROM  |
| HIGH | GS018 | gridsignal-bot.py | 554 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 564 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 601 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 638 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 940 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 1410 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | gridsignal-bot.py | 1675 | Float arithmetic for money leads to rounding errors exploita |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS025 | gridsignal-bot.py | 1108 |
| M | GS029 | gridsignal-bot.py | 30 |
| M | GS029 | gridsignal-bot.py | 906 |
| M | GS029 | gridsignal-bot.py | 1108 |
| L | GS008 | gridsignal-bot.py | 44 |
| i | GS020 |  | 135 |
| i | GS020 |  | 184 |
| i | GS020 |  | 192 |
| i | GS020 |  | 267 |
| i | GS020 |  | 141 |
| i | GS020 |  | 1528 |
| I | GS007 | gridsignal-bot.py | 172 |
| I | GS007 | gridsignal-bot.py | 177 |
| H | GS007 | gridsignal-bot.py | 124 |
| H | GS007 | gridsignal-bot.py | 224 |
| H | GS007 | gridsignal-bot.py | 365 |
| H | GS007 | gridsignal-bot.py | 1039 |
| H | GS007 | gridsignal-bot.py | 1222 |
| H | GS007 | gridsignal-bot.py | 1256 |
| H | GS007 | gridsignal-bot.py | 1287 |
| s | GS009 |  | 0 |
| H | GS018 | gridsignal-bot.py | 554 |
| H | GS018 | gridsignal-bot.py | 564 |
| H | GS018 | gridsignal-bot.py | 601 |
| H | GS018 | gridsignal-bot.py | 638 |
| H | GS018 | gridsignal-bot.py | 940 |
| H | GS018 | gridsignal-bot.py | 1410 |
| H | GS018 | gridsignal-bot.py | 1675 |
| s | GS021 |  | 21 |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| ? | YAML-B39DC08C | gridsignal-bot.py | ? |
| M | ? | gridsignal-bot.py | 1303 |
| M | ? | gridsignal-bot.py | 1305 |
| M | ? | gridsignal-bot.py | 1404 |
| M | ? | gridsignal-bot.py | 1406 |
| M | ? | gridsignal-bot.py | 1483 |
| M | ? | gridsignal-bot.py | 2043 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:16:32.722880*