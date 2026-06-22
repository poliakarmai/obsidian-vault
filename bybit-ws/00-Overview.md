---
tags: [bybit-ws, docs, trading]
updated: 2026-06-09
---

# bybit-ws — Карта документации

Репозиторий: https://github.com/poliakarmai/bybit-ws
Версия: v3.9 (код-ревью Manus AI внедрён)

## Документы

- [[bybit-ws-design|DESIGN.md]] — полная архитектура, стратегия, API, безопасность
- [[bybit-ws-strategies|STRATEGIES.md]] — 8 стратегий + roadmap
- [[bybit-ws-code-review|Код-ревью Manus AI]] — 09.06.2026, 8 страниц
- [[bybit-ws-errors|ERRORS.md]] — справочник ошибок

## Модули (v3.9)

| Файл | Назначение | Изменено в v3.9 |
|------|-----------|-----------------|
| api.py | API-запросы к Bybit | ✅ retry POST, openTime/margin |
| auto_sl.py | Авто-SL на позиции | ✅ BB-based вместо -7% |
| auto_short.py | Авто-SHORT | ✅ junk из strategy.junk |
| dca.py | DCA-лесенка | ✅ уровни из конфига, round |
| sl_reentry.py | Re-entry после SL | ✅ simple/ladder, конфиг |
| rpc.py | REST API сервер | ✅ CORS, RPC_TOKEN, polling |
| main.py | Главный цикл | ✅ sys.exit вместо os._exit |
| utils.py | Общие утилиты | 🆕 tier, lot_step, round_to_tick |

## Связанные заметки

- [[hermes/trading]] — трейдинг-инфра
- [[hermes/memory]] — техническая память
