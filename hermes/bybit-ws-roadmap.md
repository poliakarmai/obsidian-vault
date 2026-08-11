---
tags: [roadmap, bybit-ws]
updated: 2026-08-08
---

# Roadmap bybit-ws

> Актуально на 08.08.2026. Синхронизировано с `~/bybit-ws/docs/ROADMAP.md`.

## ✅ ФАЗА 1–7 — ЗАВЕРШЕНЫ (07.06 – 28.06.2026)

Базовая архитектура, ML-скоринг, LSTM-режимы, RPC, дашборд, алерты, self-learning.

## ✅ ФАЗА 8.0–8.2 — ЗАВЕРШЕНЫ (01–04.08.2026)

| Подфаза | Что сделано |
|---------|------------|
| 8.0 | Документация, Paper Trade, веб-дашборд, Graphify-рефакторинг, лицензия AGPL-3.0 |
| 8.1 | LSTM World Model (33.1%), Anti-ludomania, REGIME_AUTO, адаптивный TP/SL, BlackSwan v2, MTF-дыра, SL floor 2→5% |
| 8.2 | Systemd hardening (MemoryDenyWriteExecute, HMAC mismatch, TimeoutStopSec), MTF-скидка TRENDING_DOWN |

## ✅ ФАЗА 9 — SHORT-оптимизация (08.08.2026)

| Задача | Статус |
|--------|--------|
| Time-based SL: закрытие убыточных SHORT >12ч | ✅ `check_short_time_sl()` в основном цикле |
| Junk ужесточение: max_loss 15→10%, max_hold 48→24ч | ✅ |
| Исключение imported-сделок из self-learn | ✅ `WHERE strategy != 'imported'` |
| Анализ: без STGUSDT SHORT +$146 | ✅ |
| World Model качество: 22.3% → 33.1% | ✅ 400 эпох, λ=0.01 |

## ⬜ ФАЗА 10 — ANDROID ПРИЛОЖЕНИЕ

### Сделано
| Компонент | Статус |
|-----------|--------|
| Код приложения (Kotlin/Compose, 25 файлов, 1277 строк) | ✅ |
| 5 экранов: Dashboard, Detail, Scan, Alerts, Settings | ✅ |
| Серверная часть: JWT auth, nginx :4444→:8766, /set-tp, /generate-jwt | ✅ |
| Спецификация: `docs/android/SPEC.md` | ✅ |

### Осталось
- Сборка APK (нужен Android SDK + Gradle)
- Global Kill-Switch из приложения
- Установка на телефон

## 📋 ДОЛГИЙ СРОК

| Задача | Приоритет |
|--------|-----------|
| Multi-exchange (Binance, OKX) | 🟡 |
| ExchangeAdapter — абстракция бирж | 📋 pre-req |
| DQN → PPO (RL-агент) | 🟢 |
| Feature Store / Data Pipeline для RL | 📋 pre-req |
| Grafana HTTPS (нужен домен) | 🟢 |

## История фаз

| Фаза | Дата |
|------|------|
| 1 — Базовая | 07.06.2026 |
| 2 — SQLite + RPC | 16.06.2026 |
| 3 — ML-скоринг | 17.06.2026 |
| 4 — Алерты + Дашборд + MTF | 18.06.2026 |
| 5 — DSPy + A/B + LSTM + RL | 18.06.2026 |
| 6 — WebSocket + Risk + Push | 21.06.2026 |
| 7 — Graceful shutdown + Kelly | 27.06.2026 |
| 7.1 — Стабилизация | 28.06.2026 |
| 8.0 — Документация + Paper Trade | 02.08.2026 |
| 8.1 — World Model + Anti-ludomania | 04.08.2026 |
| 8.2 — Systemd Hardening | 04.08.2026 |
| 9 — SHORT-оптимизация | 08.08.2026 |
| 10 — Android ⬜ | — |
