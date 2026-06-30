---
tags: [roadmap, bybit-ws]
updated: 2026-06-30
---

# Roadmap bybit-ws

## ✅ ФАЗА 7 — ЗАВЕРШЕНА (27.06.2026)

| Задача | Статус | Результат |
|--------|--------|-----------|
| Graceful shutdown | ✅ v7.0 | `while not SHUTDOWN` + сигналы |
| apply_journal_insights | ✅ v7.0 → починен | был вызов без аргументов, исправлено в heavy_cycle_opt |
| Heavy cycle <30с | ✅ | 77s → 29.73s (asyncio.gather, 62% ускорение) |
| Backtesting framework | ✅ | Monte Carlo 10K + Sharpe + Sortino + Calmar + per-symbol |
| Kelly sizing | ✅ | f*=(p×b-q)/b, fractional 25%, per-symbol stats |
| Grafana dashboard | ✅ | 8 панелей: позиции, PnL, циклы, аптайм + 2 графика |

## ✅ ФАЗА 7.1 — СТАБИЛИЗАЦИЯ (28.06.2026)

| Задача | Статус |
|--------|--------|
| auto_tp: orders.values() → list/dict | ✅ |
| ab_status: NoneType check | ✅ |
| Self-learning в main loop (2880 циклов) | ✅ |
| pump_state авто-очистка | ✅ |
| gridsignal-bot: ALTER TABLE crash | ✅ |
| DSPy → DeepSeek | ✅ |
| pip-audit: per-package fix_versions | ✅ |
| PR #52823 (macOS symlink fix) | 🟡 ждёт форк |

## ✅ ФАЗА 7.2 — ЗАВЕРШЕНА (28.06.2026)

| Задача | Статус |
|--------|--------|
| BlackSwan multi-tier (3 уровня: -3%/-5%/-8%) | ✅ |
| Canary mode для self-learning (10% + auto-rollback) | ✅ |
| Paper Trading (PaperExchange + RPC) | ✅ |
| Structured Logging (JSON в events.jsonl) | ✅ |

## ✅ ФАЗА 7.3 — POST-TRADE + SELF-LEARN (30.06.2026)

| Задача | Статус |
|--------|--------|
| save_trade_features() hook при импорте истории Bybit | ✅ коммит 06c4482 |
| post_trade_features.jsonl наполняется реальными данными | ✅ |
| Кластерный анализ WR<40% → автоблок | ✅ (ждёт данных) |
| self_learn analyze() missing trades fix | ✅ (исправлено ранее) |
| Очистка диска (~2.5G) | ✅ |
| Telegram bridge восстановлен | ✅ |

## ⬜ ФАЗА 8 — ANDROID ПРИЛОЖЕНИЕ

### MVP (v8.0)
| Фича | Описание |
|------|---------|
| Дашборд | Позиции, PnL, SL/TP — live через RPC :8766 |
| Алерты | Пуш-уведомления: входы, TP, SL, пампы, circuit breaker |
| Управление | Закрыть позицию, подвинуть SL, поставить TP |
| Скан SHORT | Ручной запуск BB-скана из приложения |
| Мультисервер | Подключение к нескольким VPS |

### Что нужно для старта
- Защищённый API шлюз (RPC снаружи — дыра в безопасности)
- WebSocket эндпоинт для live-обновлений
- Push-сервер (Firebase или ntfy)

### Долгий срок
- Grafana HTTPS (нужен домен для Let's Encrypt)
- Multi-exchange (Binance, OKX)
- DQN → PPO
