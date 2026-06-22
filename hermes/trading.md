---
tags: [trading, bybit]
updated: 2026-06-19
---

# Трейдинг Bybit

## Пути (НЕ ИСКАТЬ КАЖДЫЙ РАЗ)

### Базы данных
- **SSOT (позиции/сделки):** `~/.local/share/bybit-ws/state.db` (SQLite, WAL)
- **Бумажная торговля:** `~/.local/share/bybit-ws/paper_state.db`
- **Бэкапы:** `~/.local/share/bybit-ws/backups/`

### Логи
- **События:** `~/.local/share/bybit-ws/events.log`
- **Алерты:** `~/.local/share/bybit-ws/alerts.log`

### Исполняемые файлы
- **MCP-сервер:** `~/.local/bin/bybit-mcp-server.py` (порт 8766 через RPC)
- **Сервис:** `bybit-ws-async` (НЕ `bybit-ws.service` — вырублен)
- **Репо:** `~/bybit-ws/` (ветка master)
- **Рабочая копия:** `~/.local/lib/bybit_ws/`
- **Синхронизация:** `cp ~/bybit-ws/bybit_ws/*.py ~/.local/lib/bybit_ws/ && systemctl --user restart bybit-ws-async`

### RPC
- URL: `http://127.0.0.1:8766`
- Auth: Bearer-токен из `kv_store.rpc_auth_token`
- Эндпоинты: `/rpc/metrics`, `/rpc/positions`, `/rpc/risk`, `/rpc/scan`, `/rpc/entry`, `/rpc/signals`, `/rpc/paths`, `/rpc/ml_toggle`

## Прогресс по фазам (19.06.2026)

| Фаза | Статус | Ключевые фичи |
|------|--------|--------------|
| 1 — Базовая | ✅ | Стабильность, мониторинг |
| 2 — SQLite + RPC | ✅ | SSOT, Prometheus /metrics |
| 3 — ML-скоринг | ✅ | RandomForest F1 0.69→0.921, Trailing x10, Partial TP, Фандинг-ротация |
| 4 — Масштабирование | ✅ | ATR risk-sizing, Multi-timeframe (D/W/M), Telegram-алерты, WebSocket, Дашборд v5.0 |
| 5 — ML | ✅ | RF Gate, LSTM (5 классов режима), RL (DQN), Ансамбль RF+LSTM+RL, A/B-тест, HMAC-подпись моделей |
| **6 — Мульти-биржа** | 🔄 | Binance Futures, OKX Futures, WebSocket real-time, унифицированный API-слой |
|| **6.3** — WebSocket full | ✅ | kline + position + execution + wallet + feature flag BYBIT_WS_FULL_ENABLED |
|| **6.4** — Push-уведомления | ✅ | ntfy (топик bybit-alerts-335c1721), CRITICAL/HIGH, без Telegram-дублей |
|| **6.7** — Глобальный risk-менеджмент | ✅ | circuit breaker, max_positions, correlation check |
|| **6.8** — Dry Spell Throttle | ✅ | 3 холостых SHORT-цикла → пропуск 30 мин, экономия ~80% BB-запросов |

## Аудит 18.06.2026
- 23 находки исправлены (7 CRITICAL + 12 HIGH + 4 MEDIUM)
- HMAC-подпись моделей → RCE-вектор закрыт
- Атомарный деплой с rollback
- RPC `/rpc/ml_toggle` — быстрый откат ML
- Watchdog с проверкой зависания цикла
- ML отключён (overfitting: F1=0.921 → F1_oos=0.368)

## Ключевые модули
- `main_async.py`, `api.py`, `rpc.py`, `state_db.py`
- `auto_entry.py`, `auto_short.py`, `auto_sl.py`, `auto_tp.py`
- `trailing_sl.py` (включая trailing_sl_x10)
- `ml_scorer.py`, `lstm_regime.py`, `rl_agent.py`, `ensemble.py`
- `correlation.py`, `position_sizing.py`, `x10_limits.py`
- `backtest.py`, `partial_tp.py`, `funding_rotation.py`
- Дашборд: `web/`, порт 9999

## Тесты
- 45/45 PASS (smoke)
- `test_modules.py`, `test_ml_smoke.py`

## Стратегии
- **Bollinger Grid LONG**: лимитки −3-5% ниже Lower BB, SL −7%, TP Middle/Upper
- **SHORT**: Tier A/B с SL+TP, Tier C/D шлак-режим
- **ONE_WAY исключения**: XRP, ONDO, WLFI, ENJ, ESPORTS, AVAX, APT, SUI
- **X10**: BB Scalp M5, Mean Revert, Funding Momentum, ATR Risk Sizing
- **MTF конфирмация**: D/W/M, ≥2/3
- **SHORT 9-metric scoring** + RL adversarial augmentation

## Правила
- **Протокол входа**: анализ → запрос подтверждения → исполнение
- «Бери X» = анализ (BB + Score) → показать → спросить → лимитка −5% Lower Daily
- Лимит позиций НЕ соблюдается (8-13 вместо 5). Не блокировать входы.
- Judge перед правками bybit-ws/скриптов/skill
- **auto_sl**: запрет перезатирания прибыльных SL, авто-безубыток при +10%

## API
- Bybit (bytick.com): торговые права, без Wallet
- Ключи в `~/.config/bybit-cli/config`

## Мониторинг
- **Watchdog cron `960fdc08de73`**: каждые 5 мин (было 30м), no_agent
- **Цикл 4**: ежедневно 09:00 MSK — анализ ошибок из логов

## Навигация
- AGENTS.md: `~/bybit-ws/AGENTS.md`
- ROADMAP: `~/bybit-ws/docs/ROADMAP.md`
- История: `~/bybit-ws/docs/history.md`
