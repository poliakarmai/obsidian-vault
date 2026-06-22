---
tags: [bybit-ws, audit, backlog, trading]
created: 2026-06-16
---

# Bybit-ws Audit Backlog (16 июня 2026)

3-эшелонный аудит выявил 7 CRITICAL + 12 HIGH + 12 MEDIUM + 7 LOW.
CRITICAL пофикшены (6569dbc), остальное — в бэклог.

## 🟠 HIGH (6 из 12 не исправлены)

| # | Что | Файл | Почему отложено |
|---|-----|------|-----------------|
| H1 | auto_tp только для LONG (SHORT без авто-TP) | `auto_tp.py:62` | По стратегии — осознанно |
| H2 | trailing_sl только для LONG | `trailing_sl.py:17` | По стратегии — осознанно |
| H3 | Прибыльные позиции без SL при развороте | `auto_sl.py:57-61` | Трейлинг-SL отдельный механизм |
| H4 | RPC через CLI subprocess + гонка с REST | `rpc.py:100-117` | Архитектурное, не баг |
| H5 | Proxy 0.0.0.0:9997 без авторизации | `web/proxy_server.py:40` | Сервис не запущен |
| H6 | Нет ссылок на оф. доку Bybit API | Все файлы | Техдолг |

## 🟡 MEDIUM

| # | Что | Файл |
|---|-----|------|
| M1 | Bare `except: pass` в критичных местах | `main.py:453,505` |
| M2 | DCA обходит circuit breaker | `main.py:593-595` |
| M3 | auto_short без проверки существующих лимиток | `auto_short.py:216-225` |
| M4 | pumps.json без file lock (гонка данных) | `pump_detect.py:52-53` |
| M5 | check_strategy_compliance только для Buy | `reporting.py:120-121` |
| M6 | metrics.py краш при отсутствии файла | `metrics.py:13` |

## 🟢 LOW

| # | Что | Файл |
|---|-----|------|
| L1 | auto_entry парсит subprocess stdout (хрупко) | `auto_entry.py:41-54` |
| L2 | DAILY_DRAWDOWN_LIMIT = 1.0 (отключён) | `__init__.py:68` |
| L3 | Coverage report игнорирует SHORT | `reporting.py:145-147` |
| L4 | Profit trigger state при рестарте | `reporting.py:52-66` |

## Приоритет на будущее

1. **M3** — двойной вход через лимитки (может стоить денег)
2. **M2** — DCA в обход circuit breaker (при убытках докупается)
3. **M4** — гонка pumps.json (сломает JUNK-защиту)
4. **M1** — bare except скрывает ошибки
5. **H6** — ссылки на доку (техдолг, не срочно)

Остальное — при рефакторинге или когда дойдут руки.
