# bybit-ws — статус на 29.06.2026 21:40

## Коммиты (6 шт, все запушены)
```
dbce633 fix: include unrealized PnL in daily loss (was only realized)
4c4f9f8 fix: sync blockers → run_in_thread + ab_status NoneType + port :8768
37ba6b4 fix: port :8768 (Hermes конфликт) + sync HTTP → run_in_thread
49314e7 fix: isinstance guard for ALL run_in_thread call sites (scan_unpack check)
2e2571d fix: isinstance guard for run_in_thread timeout sentinel (was 'object not iterable')
97e6295 fix(ensemble): add 'votes' key to details dict (ml_smoke test)
```

## Что исправлено
✅ not iterable — isinstance guard на 9 call sites
✅ ensemble votes — ml_smoke test pass
✅ port :8767→:8768 — конфликт с Hermes Gateway
✅ sync HTTP bybit() → run_in_thread
✅ ab_status NoneType → isinstance guard
✅ 6 sync-блокировок → run_in_thread helpers
✅ Daily PnL → включён unrealized PnL (был только realized)

## Что осталось на завтра
🔴 RPC /rpc/risk_full → тоже считает daily_loss из metrics.json без unrealized
🔴 TimeoutStopSec=5s в systemd unit
🟡 529 LOW в GSC (техдолг)
🟡 P/L ratio 0.29, disposition ×3.4 — стратегические вопросы

## Сервис
PID: 1979790
Active: running
WebSocket push: :8768 ✅
RPC: :8766 ✅

## Тесты
test_smoke.py: 45/45
test_modules.py: 28/28
test_ml_smoke.py: 3/3
test_regression.py: 95/95
scan_unpack.py: 0 issues
