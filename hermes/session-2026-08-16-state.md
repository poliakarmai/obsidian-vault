---
status: active
as_of: 2026-08-16
---

# Состояние сессии 2026-08-16

## Сделано (16.08)

### 1. COWUSDT TP-ордер обнулялся 🔴 (деньги)
- Баг: `auto_tp.py` `rounding = 0 if pos_size >= 10 else 1` → `round(uncovered*split, 1)`
  давал `0.0` / меньше `qtyStep` для мелких SHORT → Bybit отклонял
  `orderQty will be truncated to zero` → позиция без TP, только SL. 6 фейлов 03:03–03:29.
- Фикс: `_round_qty()` округляет **вниз** к `qtyStep` из `_get_lot_step(sym)`,
  при `qty < qtyStep` логирует и пропускает уровень (не шлёт нулевой ордер).
- Коммит `91f0c74`, deploy (canary 8/8, smoke 52/52), push `origin main`.

### 2. Vietnam Guide Bot — голые traceback на сетевых сбросах 🟡
- 388×/сут `No error handlers are registered` (Connection reset, httpx.ReadError).
- Фикс: `on_error` + `app.add_error_handler` — httpx/NetworkError → warning, остальное → error.
- Коммит `cc789f0`, restart (getMe 200 OK), push `origin master`.

### 3. DeepSeek stream stale 🔴 (инфра) — РАЗОБРАН, фикс применён
- Симптом: 172×/24ч, stream умирает на context 283K–367K, `Stream stale 600s`.
- **Root cause:** Hermes registry считает `deepseek-v4-pro` = **1_000_000** токенов
  (`model_metadata.py:269`), `compression.threshold` 0.5 → компакция на **500K**.
  Контекст 327K < 500K → компакция НЕ срабатывала, контекст рос бесконтрольно.
  DeepSeek API реально умирает уже на ~283K.
- Фикс: `compression.threshold` 0.5 → **0.2** (компакция на ~200K),
  `compression.target_ratio` 0.2 → **0.15** (сильнее сжатие).
- ⚠️ **НУЖЕН РЕСТАРТ `hermes-gateway.service`** — подхватит конфиг + сбросит текущий 327K контекст.
  Пользователь рестартанёт сам.

## Осталось (TODO)
- [ ] Рестарт `hermes-gateway` (пользователь сам).
- [ ] Обновить skill `system-improvement-loop` → `references/deepseek-stream-stale.md`
      (статус `resolved` устарел — паттерн снова active, теперь есть точный root cause).

## Ключевые durable-факты
- `deepseek-v4-pro` в Hermes registry = 1M контекст → threshold 0.2 = 200K компакция (безопасно, API умирает ~283K).
- `auto_tp.py`: qty через `_round_qty()`/`qtyStep`, хардкод `rounding` убран.
- Vietnam Guide Bot: глобальный `on_error` handler в `bot.py`.
