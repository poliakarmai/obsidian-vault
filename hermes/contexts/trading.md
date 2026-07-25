# Трейдинг-контекст

> Загружать при входе в trading-режим (позиции, ордера, анализ)

## MCP-инструменты Bybit

`scan_market` → `get_risk_status` → `get_positions` → `place_entry`

| Инструмент | Назначение |
|-----------|-----------|
| `scan_market(mode, interval)` | Скан Bollinger Grid |
| `get_positions()` | Позиции + PnL |
| `get_metrics()` | TP/SL/входы за день |
| `get_risk_status()` | Лимиты + CB |
| `place_entry(symbol, side, qty)` | Вход |
| `get_journal()` | Журнал (FIFO, bias) |

## Чек-лист перед входом

- [ ] `get_risk_status()` — не заблокирован
- [ ] `scan_market` — сигнал есть
- [ ] `get_positions()` — не дублируем, лимит 12 поз
- [ ] SL в рынке (ATR-based)
- [ ] `trading-discipline` skill загружен

## Пути

- SSOT: `~/.local/share/bybit-ws/state.db`
- Логи: `~/.local/share/bybit-ws/events.log`
- RPC: `http://127.0.0.1:8766`
- Репо: `~/bybit-ws/`
- Сервис: `systemctl --user status bybit-ws-async`

## Лимиты

- Max позиций: 12
- Max дневной убыток: -$50
- Max маржа: $300
- Плечо: 10x (SHORT кроме ONE_WAY)
- Размер: $15/3x, x10=$10
