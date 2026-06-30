# bybit-ws — статус на 30.06.2026 12:45

## Коммиты (2 шт, все запушены)
```
894d4c9 fix: main_async traceback [:500] + run_in_thread logging + push_notifier title sanitize
06c4482 fix: post_trade save_trade_features hook при импорте закрытых сделок Bybit
```

## Что сделано 30.06
✅ post_trade_features.jsonl — теперь наполняется реальными данными (save_trade_features hook)
✅ Кластерный анализ WR<40% → автоблок (ждёт накопления данных)
✅ self_learn analyze() missing trades — исправлено в 894d4c9
✅ Telegram bridge восстановлен (PID 2050044)
✅ Диск почищен (~2.5G: /tmp, uv cache, pip cache, audio cache, events.log)
✅ Документация обновлена: AGENTS.md, README, roadmap

## Трейдинг за 28-30.06
📊 21 сделка, PnL +$12.34
📊 Авто-входов нет (все закрытия — bybit_history)
🟡 12 позиций LONG, unrealized PnL -$156.75
🟡 P/L ratio 0.29, disposition ×3.39 — стратегические проблемы

## Сервис
PID: 2056095
Active: running (~33 мин)
RAM: 45MB
RPC :8766 ✅
WS push :8768 🔴 (не отвечает — известная проблема)

## Тесты
test_smoke.py: 11/11
test_modules.py: 5/5

## Состояние самообучения
self_learn.jsonl: 1 запись (28.06)
post_trade_features.jsonl: будет наполняться при след. закрытии
canary_state.json: активно (min_score 19, sl_pct 6.0)
