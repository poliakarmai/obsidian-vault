---
tags: [bybit-ws, roadmap, trading, architecture]
created: 2026-06-16
updated: 2026-06-16
version: "1.0"
---

# Bybit-ws — План развития

> **Версия монитора:** 3.10.1 | **Модулей:** 42 | **Стратегий:** 8
> **Дата:** 16 июня 2026 | **Рецензия:** внешний аудит плана (июнь 2026)

---

## Содержание

1. [Текущее состояние](#1-текущее-состояние)
2. [Фаза 1: Стабильность](#2-фаза-1-стабильность-) ✅
3. [Фаза 2: Надёжность](#3-фаза-2-надёжность)
4. [Фаза 3: Умный трейдинг](#4-фаза-3-умный-трейдинг)
5. [Фаза 4: Масштабирование](#5-фаза-4-масштабирование)
6. [Идеи](#6-идеи-бэклог)
7. [Замечания внешнего аудита](#7-замечания-внешнего-аудита)

---

## 1. Текущее состояние

### Архитектура

```
bybit-ws (systemd, цикл 30с)
├── core/                  ← планируется: main, config, rpc, api
├── strategies/            ← планируется: auto_entry, dca, bb_scalp, ...
├── risk/                  ← планируется: auto_sl, position_sizing, x10_limits
├── utils/                 ← планируется: file_utils, reporting, metrics
│
├── main.py           — главный цикл, оркестрация, risk limits
├── api.py            — REST API v5 (HMAC-SHA256), BB-данные
├── snapshot.py       — снепшоты позиций/ордеров + сравнение
├── auto_entry.py     — авто-вход LONG по 9-метричному скорингу
├── auto_short.py     — авто-SHORT (Tier A/B + JUNK-режим)
├── auto_sl.py        — авто-SL для позиций без стопа
├── auto_tp.py        — авто-TP (ретрей с backoff)
├── trailing_sl.py    — трейлинг-SL (только LONG)
├── junk_trail.py     — трейлинг-TP для JUNK-шортов
├── dca.py            — DCA-докупка (лесенка)
├── sl_reentry.py     — перезаход после SL
├── overbought.py     — сканер перегретых монет (BB > 75%)
├── pump_detect.py    — детектор пампов (24ч + недельные)
├── bb_scalp.py       — x10 BB Scalping M5
├── mean_revert.py    — x10 Mean Reversion Extreme
├── funding_entry.py  — x10 Funding Rate Momentum
├── atr_sizer.py      — x10 ATR Risk Sizing
├── x10_limits.py     — дневной лимит x10 убытков
├── position_sizing.py— динамическая маржа от % депозита
├── correlation.py    — корреляционная матрица позиций
├── regime.py         — классификация рыночного режима
├── funding_tracker.py— экстремальные ставки фондирования
├── rsi.py            — RSI-дивергенции
├── squeeze.py        — детектор BB-сжатия
├── health.py         — проверки здоровья
├── reporting.py      — сводки, трейд-журнал, аудит
├── metrics.py        — метрики SL/TP/entries
├── margin_alerts.py  — контроль маржи
├── cost_tracker.py   — учёт комиссий
├── cleanup.py        — снятие просроченных ордеров
├── recycle.py        — перевыставление TP
├── manual_positions.py— защита ручных позиций
├── config.py         — YAML-конфиг с ${ENV}-подстановкой
├── file_utils.py     — атомарная запись JSON
├── rpc.py            — HTTP-RPC (порт 8766)
└── dashboard.py      — SVG-дашборд
```

> ⚠️ **Техдолг:** 42 файла в плоской структуре. План: рефакторинг в пакеты `core/`, `strategies/`, `risk/`, `utils/` в Фазе 2.

### Цифры

| Метрика | Значение |
|---------|----------|
| Модулей | 42 |
| Стратегий | 8 (Grid LONG/SHORT, Junk, DCA, SL Re-entry, x10 × 3) |
| Память | ~27 MB |
| Цикл | 30 секунд |
| RPC порт | 8766 (localhost) |
| Стейт-файлов | ~15 JSON |
| Модульных тестов | 0 ❌ |
| Покрытие CI/CD | 0 ❌ |

### Что сделано (v3.10.1, 16 июня)

- ✅ Circuit breaker починен (был инвертирован — блокировал на прибыли)
- ✅ Hallucinated API-параметры в trading-stop убраны
- ✅ Watchdog crash fix (new_positions до определения)
- ✅ x10_limits undefined log_event → logging
- ✅ DCA уважает risk-лимиты (не докупается при превышении)
- ✅ auto_short проверяет pending лимитки (fetch_orders dedup)
- ✅ pumps.json атомарная запись (tmp + os.replace)
- ✅ Bare except:pass → log_event
- ✅ SHORT_ALERT_LAST persistent (JSON, выживает рестарты)
- ✅ SHORT_ALERT_COOLDOWN 1800 → 14400 (4 часа)

---

## 2. Фаза 1: Стабильность ✅

> **Срок:** 16 июня 2026
> **Статус:** завершена

Закрыты самые опасные баги из трёхэшелонного аудита. Детали — `bybit-ws-audit-backlog-2026-06-16.md`.

---

## 3. Фаза 2: Надёжность

> **Срок:** июль 2026
> **Цель:** техдолг, тесты, консистентность данных

### 3.1 Логирование — ротация и надёжность

**Проблема:** `events.log` и `alerts.log` пишутся через `log_event()` без ротации. При активном трейдинге файлы растут бесконтрольно. Для трейдинга логи — единственное доказательство при спорах с биржей.

**Решение:** `logging.handlers.RotatingFileHandler`:
```python
import logging
from logging.handlers import RotatingFileHandler

handler = RotatingFileHandler(
    EVENTS_LOG, maxBytes=10*1024*1024, backupCount=7
)
handler.setFormatter(logging.Formatter('%(asctime)s %(message)s'))
logger.addHandler(handler)
```

Параметры: 10 МБ × 7 файлов = 70 МБ истории. При споре с биржей — всегда есть логи за последнюю неделю.

### 3.2 Модульные тесты — smoke suite + property-based

**Проблема:** каждое изменение кода — риск сломать авто-входы или SL/TP. Сейчас проверка только «глазами по логам». Нужен минимальный набор тестов, который прогоняется перед коммитом.

**Что тестируем (smoke, 12-15 тестов):**

| # | Тест | Модуль | Что проверяет |
|---|------|--------|---------------|
| 1 | `test_circuit_breaker_blocks_on_loss` | main.py | При daily_pnl=-60 → blocked=True |
| 2 | `test_circuit_breaker_allows_on_profit` | main.py | При daily_pnl=+10 → blocked=False |
| 3 | `test_long_limit_blocks` | main.py | 13 LONG позиций → blocked=True |
| 4 | `test_sl_calculation_long` | auto_sl.py | SL = Lower BB × 0.93 |
| 5 | `test_junk_skip_sl` | auto_sl.py | JUNK-позиция → continue |
| 6 | `test_position_sizing_positive` | position_sizing.py | Депозит $500 → маржа > 0 |
| 7 | `test_trading_stop_body_valid` | api.py | Нет side/orderType/qty в trading-stop body |
| 8 | `test_order_dedup_blocks_duplicate` | auto_short.py | Pending Sell → пропуск |
| 9 | `test_atomic_write_no_corruption` | file_utils.py | tmp+replace → целостность |
| 10 | `test_x10_daily_limit_blocks` | x10_limits.py | 3 убыточных сделки → blocked |
| 11 | `test_funding_direction` | funding_entry.py | Отрицательный фондинг → бонус для LONG |
| 12 | `test_dca_respects_risk_limit` | main.py | При entry_blocked → DCA не вызывается |

**Инструменты:** `pytest` + `unittest.mock` для API-заглушек. Не нужен реальный Bybit.

**Property-based тестирование:** добавить `hypothesis` для проверки инвариантов:
```python
from hypothesis import given, strategies as st

@given(price=st.floats(min_value=0, max_value=1_000_000))
def test_sl_never_negative(price):
    """SL всегда положительный при любых входных данных."""
    sl = calculate_sl(price, 0.93)
    assert sl > 0

@given(margin=st.floats(min_value=-1000, max_value=0))
def test_margin_negative_raises(margin):
    """Отрицательная маржа должна вызывать ошибку."""
    with pytest.raises(ValueError):
        margin_for_strategy(margin, risk_pct=0.2)
```

**Интеграция:** pre-commit hook → `pytest tests/ -x --tb=short`. Property-based тесты в отдельной
директории `tests/property/` (медленнее, запускаются в CI, не в pre-commit).

### 3.3 SQLite вместо JSON-файлов

**Проблема:** 15 JSON-файлов состояния. Каждый пишется отдельно, нет транзакционности, гонки данных. При сбое между записью двух файлов — состояние рассогласовано.

**Решение:** одна SQLite база `~/.local/share/bybit-ws/state.db` с таблицами:

```sql
-- История сделок (аудит PnL, комиссии)
CREATE TABLE trade_history (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    symbol TEXT NOT NULL,
    side TEXT NOT NULL,           -- Buy/Sell
    strategy TEXT,                -- GRID_LONG, JUNK_SHORT, x10:scalp
    entry_price REAL,
    exit_price REAL,
    size REAL,
    pnl REAL,                    -- реализованный PnL
    fees REAL DEFAULT 0,         -- комиссии
    entry_at INTEGER,            -- unix timestamp входа
    closed_at INTEGER             -- unix timestamp закрытия
);
CREATE INDEX idx_trade_symbol ON trade_history(symbol);
CREATE INDEX idx_trade_closed ON trade_history(closed_at);

-- Открытые позиции (только активные)
CREATE TABLE positions (
    symbol TEXT PRIMARY KEY,
    side TEXT, entry REAL, mark REAL, size REAL,
    leverage REAL, stop_loss REAL, take_profit REAL,
    position_idx INTEGER, upnl REAL, liq_price REAL,
    updated_at INTEGER
);

-- SHORT-состояние
CREATE TABLE short_state (
    symbol TEXT PRIMARY KEY,
    last_short_ts INTEGER, entry_price REAL,
    qty REAL, bb_pct REAL, is_junk INTEGER,
    dca_level INTEGER DEFAULT 0
);

-- Памп-трекинг
CREATE TABLE pump_state (
    symbol TEXT PRIMARY KEY,
    first_seen_ts INTEGER, peak_price REAL,
    alerts TEXT, daily_pump INTEGER,
    weekly_pump INTEGER, short_entry_ts INTEGER
);

-- x10 лимиты
CREATE TABLE x10_limits (
    date TEXT, strategy TEXT,
    losses INTEGER DEFAULT 0, pnl REAL DEFAULT 0,
    stopped_at INTEGER,
    PRIMARY KEY (date, strategy)
);

-- Кулдауны
CREATE TABLE cooldowns (
    key TEXT PRIMARY KEY,
    until INTEGER
);

-- Алерт-дедупликация
CREATE TABLE alert_dedup (
    key TEXT PRIMARY KEY,
    last_at INTEGER
);
```

**Преимущества:**
- Атомарность: `BEGIN TRANSACTION` → commit/rollback
- Консистентность: нет частичных записей
- Запросы: `SELECT * FROM short_state WHERE is_junk=1` вместо grep по JSON
- WAL-режим: читатели не блокируют писателей

**План миграции:**
1. Добавить `state_db.py` с методами `get_*` / `set_*`
2. Перевести модули по одному, начиная с наименее критичных (alert_dedup, cooldowns)
3. Держать старые JSON как fallback на время перехода
4. Удалить JSON-чтение через 2 недели стабильной работы

### 3.3 RPC: CLI subprocess → прямые вызовы api.py

**Проблема:** RPC-сервер (`rpc.py`) для торговых операций использует `subprocess.run([BYBIT_CLI, 'raw', ...])`, а основной цикл — `api.bybit()`. Два пути аутентификации, разная обработка ошибок, гонка данных.

**Решение:** переписать `_handle_enter()`, `_handle_close()` и др. на прямые вызовы `api.bybit()` / `api.place_stop_loss()` / `api.place_take_profit()`.

**Конкретно:**

```python
# Было (rpc.py:716-726)
def _handle_enter(data):
    symbol = data['symbol']
    result = subprocess.run([BYBIT_CLI, 'raw', 'POST', '/v5/order/create', json.dumps(body)], ...)
    # парсим stdout

# Стало
def _handle_enter(data):
    from .api import bybit
    body = {...}
    result = bybit('POST', '/v5/order/create', body)
    # сразу dict, не надо парсить
```

**Затронутые эндпоинты RPC:**
- `POST /enter` → `api.bybit('POST', '/v5/order/create', ...)`
- `POST /close` → `api.bybit('POST', '/v5/order/create', ...)` (Market против позиции)
- `GET /positions` — уже через `fetch_positions()` ✅
- `GET /orders` — уже через `fetch_orders()` ✅
- `GET /health` — уже локальное ✅

### 3.4 Документирование API-вызовов

**Проблема:** в коде ноль ссылок на официальную документацию Bybit API v5. При изменении API непонятно, какой эндпоинт за что отвечает.

**Решение:** добавить docstring'и с URL'ами к каждой функции в `api.py`:

```python
def place_stop_loss(symbol, positionIdx, side, qty, stop_price):
    """Установить Stop-Loss через trading-stop.
    
    Bybit API v5: POST /v5/position/trading-stop
    Docs: https://bybit-exchange.github.io/docs/v5/position/trading-stop
    
    Валидные параметры: category, symbol, positionIdx, stopLoss, slTriggerBy
    НЕ передавать: side, orderType, qty, triggerBy — это параметры /v5/order/create
    """
```

Также `DESIGN.md` §3 дополнить таблицей всех API-вызовов со ссылками.

### 3.5 auto_tp/trailing_sl для SHORT

**Проблема:** `auto_tp.py` и `trailing_sl.py` фильтруют только `side == 'Buy'`. SHORT-позиции остаются без авто-TP и трейлинг-SL.

**auto_tp для SHORT:**

```python
# auto_tp.py — добавить ветку SHORT
if side == 'Buy' and size > 0:
    tp_price = upper_bb   # TP на Upper BB
    place_take_profit(...)
elif side == 'Sell' and size > 0:
    tp_price = lower_bb   # TP на Lower BB (ниже рынка = профит для шорта)
    place_take_profit(...)
```

**trailing_sl для SHORT:**

```python
# trailing_sl.py — добавить SHORT
if side == 'Buy':
    if mark > entry * 1.10:  # +10% профита
        new_sl = entry * 1.05  # зафиксировать +5%
elif side == 'Sell':
    if mark < entry * 0.90:  # +10% профита (цена упала)
        new_sl = entry * 0.95  # зафиксировать +5% (SL выше рынка)
```

### 3.7 Алертинг — мгновенные уведомления

**Проблема:** система управляет реальными деньгами, но критические события (Circuit Breaker, ошибки API, аномальная просадка) видны только при проверке логов.

**Решение:** вынести из бэклога в Фазу 2. Добавить каналы:
- **Telegram** (уже есть `@Gridbolbot`) — дополнить критическими алертами
- **Discord/Slack** webhook — для дублирования (resilience)

```python
def alert_critical(msg: str):
    """Критический алерт — во все каналы мгновенно."""
    alerts.append(msg)
    if ALERT_WEBHOOK_URL:
        requests.post(ALERT_WEBHOOK_URL, json={'content': msg}, timeout=5)
```

События для мгновенного алерта:
- Circuit Breaker сработал (max_daily_loss)
- Ошибка API (retCode != 0 на торговых операциях)
- Ликвидация позиции
- Маржа > 80%

### 3.8 Подготовка к asyncio: httpx + aiosqlite

**Проблема:** переход на asyncio в Фазе 4 затронет 70% кодовой базы. Чтобы снизить боль миграции, начинаем использовать асинхронные библиотеки уже сейчас.

**План:**
- `api.py`: заменить `requests` → `httpx` (имеет синхронный API, идентичный requests, но с async-двойником)
- `state_db.py`: использовать `aiosqlite` для SQLite-операций (совместим с синхронным кодом через `asyncio.run()`)
- Новый код в Фазе 2 пишем сразу на httpx/aiosqlite

### 3.9 RPC: импорт на уровне модуля

**Антипаттерн:** `from .api import bybit` внутри функции-обработчика создаёт циклические импорты и оверхед при каждом вызове.

**Правило:** все импорты — на уровне файла. Для RPC использовать внедрение через параметры конструктора:

```python
class RPCHandler:
    def __init__(self, api_client=None):
        self.api = api_client or bybit  # внедрение зависимости
```

**Проблема:** `reporting.py:check_strategy_compliance()` фильтрует `side != 'Buy'`. SHORT-позиции не аудируются — нет проверки что SL/TP на месте.

**Решение:** зеркальная проверка для SHORT:
- SL: выше входа на +5% (Tier A/B) или +7% (JUNK)
- TP: на Middle BB (ниже рынка)
- Для JUNK: проверять флаг `no_sl` и `max_hold_hours`

---

## 4. Фаза 3: Умный трейдинг

> **Срок:** август-сентябрь 2026
> **Цель:** фичи, повышающие профит и адаптивность

### 4.1 Trailing Stop для x10

**Суть:** x10 позиции волатильны. Сейчас SL фиксированный (3-5%). Когда цена идёт в нашу сторону, SL остаётся на месте — профит не защищён.

**Алгоритм:**

```
Для LONG x10:
  Если mark > entry * 1.05 (профит > 5%):
    new_sl = max(текущий SL, mark * 0.97)  # подтянуть до -3% от текущей
  Если mark > entry * 1.10 (профит > 10%):
    new_sl = mark * 0.98  # агрессивнее, -2%
  Если mark > entry * 1.20 (профит > 20%):
    new_sl = entry * 1.05  # безубыток + 5%

Для SHORT x10:
  Если mark < entry * 0.95:
    new_sl = min(текущий SL, mark * 1.03)
  ...
```

**Частота:** проверка каждый цикл (30с), но API-вызов только если SL реально сдвинулся более чем на 0.5%.

### 4.2 ML-скоринг — адаптивные веса метрик

**Проблема:** веса 9 метрик для LONG/SHORT захардкожены. Рынок меняется: в бычьем тренде BB% важнее, в боковике — RSI и squeeze. Фиксированные веса = упущенная прибыль.

**Решение:** простой ML без переобучения:

1. **Сбор данных:** для каждого входа записываем вектор метрик + исход (TP/SL/безубыток)
2. **Периодический пересчёт:** раз в неделю логистическая регрессия на новых данных
3. **Обновление весов:** плавное (EMA от старых весов, чтобы не дёргалось)
4. **A/B тест:** 50% входов по старым весам, 50% по новым → сравнить PnL через 2 недели

**Инструменты:** `sklearn.linear_model.LogisticRegression` (без GPU, без DL).

**⚠️ Стандартизация и валидация:**
- **StandardScaler** — логистическая регрессия чувствительна к масштабу признаков. Масштабировать перед обучением обязательно.
- **TimeSeriesSplit** вместо K-Fold — для временных рядов случайная кросс-валидация вызывает «утечку будущего» (data leakage). 5 фолдов по времени.
```python
from sklearn.preprocessing import StandardScaler
from sklearn.model_selection import TimeSeriesSplit

scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)
tscv = TimeSeriesSplit(n_splits=5)
for train_idx, test_idx in tscv.split(X_scaled):
    # train на более ранних данных, test на более поздних
```

**Метрики для модели:**
- BB% положение (D), BB% (W), BB% (M)
- RSI(14), RSI-дивергенция
- Объём 24ч (log), изменение за 24ч
- Фондинг, тренд фондинга (3 дня)
- BB squeeze (boolean)
- Дней падения подряд
- Tier монеты (one-hot)

**Целевая переменная:** `1` = TP сработал, `0` = SL сработал.

### 4.3 Авто-фандинг-ротация

**Суть:** когда ставка фондирования разворачивается, флипать позицию:
- LONG + отрицательный фондинг → получаешь выплаты ✅
- LONG + положительный фондинг → платишь ❌ → flip в SHORT

**Триггер:** фондинг сменил знак И держится > 2 часов в новом направлении.

**Исполнение:** Market-закрытие LONG + Market-открытие SHORT (или наоборот).

**Ограничения:**
- Только для Tier A/S монет (высокая ликвидность)
- Не чаще 1 флипа в сутки на монету
- Минимальный профит для флипа: позиция должна быть в плюсе

**⚠️ Математическое условие рентабельности флипа:**

Флип (Market-закрытие + Market-открытие) = двойная комиссия + двойной спред. Выгода от смены знака фондирования может быть мгновенно съедена.

```python
def flip_is_profitable(position, funding_rate, hours=24):
    \"\"\"Проверить что флип окупится за N часов.\"\"\"
    pos_value = position.size * position.mark
    flip_cost = pos_value * (TAKER_FEE * 2 + SLIPPAGE_BASE * 2)  # закрыть+открыть
    funding_gain = pos_value * abs(funding_rate) * (hours / 8)     # выплаты за N часов
    return funding_gain > flip_cost * 1.2  # запас 20%
```

### 4.4 Partial TP — гибкий сплит

**Сейчас:** жёстко 20% на Middle BB, 80% на Upper BB.
**Надо:** конфигурируемый сплит.

```yaml
strategy:
  long:
    tp_split:
      middle: 0.30    # 30% на Middle BB
      upper: 0.70     # 70% на Upper BB
```

Или даже 3 цели:

```yaml
    tp_split:
      target1: {pct: 0.25, level: "middle_bb"}
      target2: {pct: 0.35, level: "upper_bb"}
      target3: {pct: 0.40, level: "upper_bb * 1.05"}
```

### 4.5 Бэктестинг на исторических данных

**Суть:** прогнать стратегию на 6-12 месяцах исторических свечей без риска реальными деньгами.

**⚠️ Критически важно: реалистичная модель издержек с первого дня.**

Без точного учёта комиссий и проскальзывания бэктест покажет прибыль там, где реальность — убыток. Скальпинговые стратегии (M5) имеют маржинальность ниже 0.2%.

**Модель издержек:**
```python
TAKER_FEE = 0.00055        # 0.055% на Bybit
SLIPPAGE_BASE = 0.0005     # 0.05% база
SLIPPAGE_VOLATILITY = 0.001  # +0.1% при высокой волатильности

def apply_costs(price, side, volume_24h, atr):
    slippage = SLIPPAGE_BASE + (SLIPPAGE_VOLATILITY if atr/price > 0.05 else 0)
    if side == 'Buy':
        return price * (1 + TAKER_FEE + slippage)
    else:
        return price * (1 - TAKER_FEE - slippage)
```

Минимум: комиссия taker (0.055%) + база проскальзывания (0.05%) = 0.105% на сделку. Для входа+выхода = 0.21%.

**Архитектура:**

```
backtest.py:
  1. Загрузить Daily свечи для топ-50 монет (~5K запросов к Bybit API)
  2. Кэшировать в SQLite (bybit-ws/kline_cache.db)
  3. Симулятор цикла: подавать свечи по одной, вызывать те же auto_entry/auto_short
  4. Собирать метрики: winrate, avg PnL, max drawdown, Sharpe
  5. Сравнивать варианты стратегий (веса, пороги)
```

**Ограничения:** без реального исполнения ордеров — только сигналы. Не учитывает проскальзывание и комиссии (можно добавить -0.1% к каждому TP).

### 4.6 Paper-trading режим

**Суть:** параллельный «бумажный» счёт, который зеркалит реальные сигналы без отправки ордеров.

**Реализация:** `paper_trader.py` — класс с методами `place_order()`, `get_positions()` которые работают с виртуальным балансом вместо Bybit API.

```python
class PaperTrader:
    def __init__(self, initial_balance=1000):
        self.balance = initial_balance
        self.positions = {}
        self.orders = []
        self.trades = []
    
    def place_order(self, symbol, side, qty, price, order_type):
        # Создать виртуальный ордер
        # При fill — обновить баланс и позиции
    
    def get_positions(self):
        return self.positions
```

**Подключение:** флаг `paper_trading: true` в конфиге → все вызовы `api.bybit()` идут через `paper_trader`.

**⚠️ Эмуляция реальных условий:**
Без моделирования задержек и частичного исполнения paper-trading даст слишком оптимистичные результаты:
```python
import random, time

class PaperTrader:
    LATENCY_MS = (50, 200)       # задержка сети 50-200 мс
    PARTIAL_FILL_PROB = 0.05     # 5% шанс частичного исполнения

    def _simulate_latency(self):
        time.sleep(random.randint(*self.LATENCY_MS) / 1000)

    def _fill_order(self, order):
        self._simulate_latency()
        fill_qty = order.qty
        if random.random() < self.PARTIAL_FILL_PROB:
            fill_qty = order.qty * random.uniform(0.3, 0.9)  # частичное
        # применить комиссию + проскальзывание
        ...
```

---

## 5. Фаза 4: Масштабирование

> **Срок:** июнь-октябрь 2026
> **Цель:** расширение на другие биржи, мониторинг, архитектурные улучшения
> **Статус:** 6/8 задач завершено (июнь 2026)

### 5.1 WebSocket вместо REST polling ✅

**Реализовано:** `ws_client.py` — WebSocket-клиент к `wss://stream.bybit.com/v5/public/linear`.
Подписка на 50+ тикеров + kline D. Live-обновление BB и цен в in-memory кеше.
Авто-переподключение при обрыве. Запускается в фоновом потоке из main.py.

### 5.2 Дашборд ✅

**Реализовано:** `web/dashboard.html` v5.0 + `web/proxy_server.py` (порт 9999, systemd).
Показывает: риск-панель (daily PnL, margin, блокировка), equity/PnL, график за 24ч,
позиции с PnL, ордера TP/SL с фильтром, сигналы LONG/SHORT, алерты, uptime/WS-статус.
Прокси читает RPC-токен из state.db автоматически.

### 5.3 MTF-конфлюенс ✅ **ИСПРАВЛЕНО (18.06)**

**Реализовано:** `mtf_confirmation.py` — проверка D/W/M согласованности (≥2/3).
**Баг (исправлен):** импорт `gridsignal_scanner` заменён на `api.bybit` + inline `_fetch_candles`/`_calc_bb`. Модуль не работал в проде.
**Тесты:** 16/16 ✅
**Статус:** активно фильтрует LONG и SHORT входы.
`confluence_paper.py` — paper-трекинг эффективности конфлюенса.
Интегрировано в `auto_entry.py` через `_filter_by_mtf_confluence()`.

### 5.4 Алерты Telegram ✅

**Реализовано:** `alerts.py` → `hermes send --to telegram:Poliakarm`.
Алерты при входе/выходе в `rpc.py`, критические события в `main.py`.
Дедупликация: category-cooldown + normalized hash + SQLite persistent.

### 5.5 httpx вместо requests ✅

**Реализовано:** `api.py` мигрирован с `requests` на `httpx`.
Подготовка к полной asyncio-миграции. 45/45 тестов.

### 5.6 ATR-based риск-сайзинг ✅

**Реализовано:** `api.py:fetch_atr()` + `position_sizing.py:atr_margin()`.
Wilder's ATR(14), JSON-кеш на 4ч, авто-qty при qty=0 в place_entry.

### 5.7 asyncio вместо потоков 🔜

**Оценка:** 40-60 часов. Полная миграция main loop + RPC на asyncio.
Подготовка сделана (httpx, aiosqlite установлен).

### 5.8 Поддержка Binance/OKX 💡

**Оценка:** 60-80 часов. Абстракция биржи через ExchangeAdapter.

---

## 6. Фаза 5: AI/ML-усиление

> **Срок:** июнь-июль 2026
> **Цель:** глубокая ML-интеграция — от A/B-валидации до ансамбля нейросетей
> **Статус:** ✅ 6/6 задач завершено

### 6.1 ML Gate — RandomForest-фильтр ✅

**Реализовано:** `ml_scorer.py:ml_gate_pass()` — RandomForest (F1=0.921, Precision=0.853, Recall=1.000).
Порог 0.22. Ловит 29/30 TP, пропускает 5/240 ложных.
Интегрировано в `auto_entry.py` как обязательный фильтр перед входом.

### 6.2 Per-symbol авто-параметры ✅

**Реализовано:** `optimize_params.py` — 4320 бэктестов grid-search.
`per_symbol_optimal.json` для 22 тикеров: entry_discount 0.95, BB период 10-30, SL дисконт 0.90-0.93.
Интегрировано в `auto_entry.py` через `PER_SYMBOL_CONFIG`.

### 6.3 A/B-тестирование ML Gate 🔜

**Суть:** статистически проверить, реально ли ML Gate улучшает PnL.
Сейчас фильтр работает без baseline — неизвестно, не режет ли он хорошие входы.

**Реализация:**
- `ab_test.py` — модуль A/B-трекинга
- SQLite-таблица `ab_test` в state_db
- Сплит 50/50: группа A (ML Gate) vs группа B (без фильтра)
- Random assignment при каждом входе
- Метрики: winrate, avg PnL, max drawdown, Sharpe per group
- Статистический тест (t-test / Mann-Whitney) через 2 недели или 100+ сделок
- Отчёт: RPC-эндпоинт `/rpc/ab_test_report`

**Оценка:** 4-6 часов.

### 6.4 LSTM-классификатор рынка ✅

**Реализовано:** `lstm_regime.py` — 2-layer LSTM (64→32) на 30-дневных D-свечах BTC+ETH.
Forward-looking метки (lookahead 7 дней). 618 сэмплов, val_acc=60.5%.

**Суть:** заменить эвристический `regime.py` на LSTM-модель.
Рынок классифицируется по 5 режимам: TRENDING_UP, TRENDING_DOWN, RANGING, HIGH_VOL, LOW_VOL.
Параметры входа адаптируются под текущий режим.

**Признаки (последовательность):**
- Kline D × 30 дней: BB%, RSI(14), ATR(14)/price, объём
- Фондинг и его тренд (3 дня)
- BB squeeze (boolean)

**Архитектура:** 2-layer LSTM → Dense(64) → Dense(5) softmax.
PyTorch (без GPU). Обучение раз в неделю. Инференс — в цикле (раз в 4ч).

**Оценка:** 12-16 часов.

### 6.5 RL-оптимизатор входов ✅

**Реализовано:** `rl_env.py` + `rl_agent.py` — DQN (Stable-Baselines3).
Gym-среда на исторических D-свечах, 3 действия (SKIP/ENTER_LONG/WAIT).
13 признаков, обучение на BTC+ETH за 365 дней, 100K шагов.

**Суть:** RL-агент учится выбирать оптимальный момент входа.
Вместо «входить сразу при сигнале» — агент решает: ENTER / DELAY / SKIP.

**Состояние:** BB позиция, RSI, объём, фондинг, волатильность, MTF конфлюенс.
**Действия:** ENTER_LONG, ENTER_SHORT, WAIT, SKIP.
**Награда:** PnL сделки (TP +, SL −).
**Алгоритм:** DQN или PPO (Stable-Baselines3).

**Оценка:** 20-30 часов.

### 6.6 Ensemble моделей ✅

**Реализовано:** `ensemble.py` — взвешенное голосование RF+LSTM+RL.
Веса по умолчанию равные, порог 0.45. Авто-перераспределение при отказе модели.

**Суть:** объединить RF (6.1) + LSTM (6.4) + RL (6.5) в ансамбль.

**Варианты:**
1. **Voting:** каждый предиктор голосует Enter/Skip, большинство решает
2. **Stacking:** мета-модель (логистическая регрессия) на выходах трёх моделей
3. **Weighted:** веса адаптируются по исторической точности каждого предиктора

**Оценка:** 8-12 часов.

---

## 7. Идеи (бэклог)

| # | Идея | Сложность |
|---|------|-----------|
| 24 | Spot-поддержка (не только фьючерсы) | Средняя |
| 25 | Copy-trading: повторять сделки AI-агента | Высокая |
| 26 | TradingView-интеграция (webhook → сигнал) | Средняя |
| 27 | Optuna-оптимизация гиперпараметров | Средняя |
| 28 | Уведомления в Discord/Slack | Низкая |
| 29 | Мобильное PWA-приложение | Высокая |

---

## 8. Замечания внешнего аудита (июнь 2026)

> Краткий перечень критических замечаний и их статус в плане.

| # | Замечание | Статус |
|---|-----------|--------|
| 1 | Бэктестинг без комиссий/проскальзывания — фатальная ошибка | ✅ Добавлена модель издержек в §4.5 |
| 2 | Фандинг-ротация без расчёта рентабельности флипа | ✅ Добавлено мат. условие в §4.3 |
| 3 | Антипаттерн импорта в RPC | ✅ Правило в §3.9 |
| 4 | Плоская структура 42 модулей → рефакторинг в пакеты | ✅ План реорганизации в §1 |
| 5 | Логи без ротации | ✅ Добавлен RotatingFileHandler в §3.1 |
| 6 | SQLite без истории сделок | ✅ Добавлена trade_history в §3.3 |
| 7 | 12 smoke-тестов недостаточно для финтеха | ✅ Добавлен property-based testing в §3.2 |
| 8 | ML без масштабирования и TimeSeriesSplit | ✅ StandardScaler + TimeSeriesSplit в §4.2 |
| 9 | Paper-trading без эмуляции latency/partial fills | ✅ Добавлена эмуляция в §4.6 |
| 10 | WebSocket отложен на октябрь — риск rate-limits | ✅ Гибридный подход с Фазы 2 в §5.1 |
| 11 | Asyncio — рефакторинг 70% кода | ✅ httpx/aiosqlite с Фазы 2 в §3.8 |
| 12 | Алертинг в бэклоге вместо Фазы 2 | ✅ Перенесён в §3.7 |

### Приоритеты по итогам аудита

**🥇 Высокий (Фаза 2):** ротация логов, алертинг (Telegram/Discord), доработка SQLite (trade_history), импорт на уровне модуля.

**🥈 Средний (Фаза 2-3):** комиссии/проскальзывание в бэктестинге, рентабельность флипа, StandardScaler для ML.

**🥉 Стратегический:** httpx/aiosqlite с Фазы 2, гибридный WebSocket, рефакторинг в пакеты.

---

## 📊 Roadmap Summary

| Фаза | Срок | Пунктов | Статус |
|------|------|---------|--------|
| 1. Стабильность | Июнь 2026 | 6 | ✅ Завершена |
| 2. Надёжность | Июль 2026 | 9 (+3 от аудита) | ✅ Завершена |
| 3. Умный трейдинг | Август-сентябрь 2026 | 6 | ✅ Завершена |
| 4. Масштабирование | Октябрь 2026+ | 8 | ✅ 6/8 |
| 5. AI/ML-усиление | Июнь-июль 2026 | 6 | ✅ Завершена |
| Бэклог | — | 5 | 💡 Идеи |

---

## Связанные документы

- `DESIGN.md` — архитектура, API, конфиг, деплой
- `STRATEGIES.md` — описание всех торговых стратегий
- `bybit-ws-audit-backlog-2026-06-16.md` — находки аудита
- `bybit-ws-roadmap.md` — краткая дорожная карта
