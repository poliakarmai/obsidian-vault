---
tags: [bybit-ws, roadmap, trading, monitor]
created: 2026-06-16
updated: 2026-06-23
version: "2.0"
---

# Bybit-ws Monitor — Дорожная карта

> Версия монитора: 6.8 | Фаза: 6 (Мульти-биржа)

---

## ✅ Фаза 1-5: Сделано

| Фаза | Что | Статус |
|------|-----|--------|
| 1 | Базовая стабильность, мониторинг, circuit breaker | ✅ |
| 2 | SQLite SSOT + RPC + Prometheus /metrics | ✅ |
| 3 | ML-скоринг (RF F1 0.921), Trailing x10, Partial TP, Фандинг-ротация | ✅ |
| 4 | ATR risk-sizing, Multi-timeframe (D/W/M), Telegram-алерты, WS, Дашборд v5.0 | ✅ |
| 5 | RF Gate, LSTM (5 режимов), RL (DQN), Ансамбль, A/B-тест, HMAC-модели | ✅ |

## ✅ Фаза 6: Мульти-биржа (текущая)

| # | Что | Статус |
|---|-----|--------|
| 6.1 | Binance Futures REST | ✅ |
| 6.2 | OKX Futures REST | ✅ |
| 6.3 | WebSocket real-time (kline+position+execution+wallet) | ✅ |
| 6.4 | Push-уведомления (ntfy + Telegram fallback) | ✅ |
| 6.5 | Унифицированный API-слой (Bybit/Binance/OKX) | 🔄 |
| 6.6 | Кросс-биржевой арбитраж | 🔜 |
| 6.7 | Глобальный risk-менеджмент (circuit breaker, max_positions, correlation) | ✅ |
| 6.8 | Dry Spell Throttle (3 холостых → пропуск 30 мин) | ✅ |
| 6.9 | SHORT SL: +10% + задержка 20 мин | ✅ 23.06 |

## 🔜 Фаза 7: SHORT-стратегия (июль 2026)

| # | Что | Зачем |
|---|-----|-------|
| 7.1 | SHORT-сканер отдельный от LONG (не зеркало) | Разная динамика перегрева |
| 7.2 | SHORT ML Gate (отдельная модель) | LONG-модель не работает для SHORT |
| 7.3 | JUNK-режим v2: авто-определение пампа | Сейчас ручной порог 80% |
| 7.4 | SHORT x10 режим | Трейлинг SL для шлака |
| 7.5 | SHORT бэктестинг на истории | Валидация без риска |

## 🔮 Идеи (без сроков)

| # | Идея |
|---|------|
| 8.1 | Spot-поддержка |
| 8.2 | Copy-trading для AI-агентов |
| 8.3 | Интеграция с TradingView |
| 8.4 | Уведомления в Discord/Slack |
| 8.5 | Мобильное PWA-приложение |
| 8.6 | Prometheus/Grafana (продакшен-мониторинг) |

## 📊 Статистика

- **Модулей:** 45+ (.py файлов)
- **Тестов:** 24 (smoke + module + ML smoke)
- **RPC endpoints:** 12+
- **Cron-джобов:** 8 (dashboard, scan LONG, auto-entry, correlation, NL→SQL, extraction, rebuild-graph, backup)
- **Документация:** AGENTS.md + DESIGN.md + DESIGN-STRATEGIES.md + ROADMAP.md
