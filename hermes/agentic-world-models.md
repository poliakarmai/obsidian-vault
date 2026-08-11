---
tags: [ai, research, world-models, agents, bybit-ws]
created: 2026-08-03
source: "https://cameronrwolfe.substack.com/p/agentic-world-models"
---

# Agentic World Models — применение в наших проектах

## Источник
Cameron R. Wolfe, Ph.D. — «Agentic World Models» (Deep Learning Focus), 20.07.2026.

## Ключевая идея
RL для агентов даёт разреженный сигнал (outcome reward), но каждая траектория богата информацией —
action → observation от среды. Добавление world modeling objective (предсказание observation-токенов)
даёт плотный сигнал, улучшает обучение и обобщение.

## Ключевые papers
- **ECHO** (Anthropic, 2026): гибрид GRPO + cross-entropy на observation-токенах. Pass rate ×2, обучение в 1.5-2.3× быстрее.
- **True Agents Model the World** [2]: та же архитектура, детальный empirical analysis.

## Наша реализация

### 1. bybit-ws: Multi-task LSTM с World Model
Файл: `bybit-ws/lstm_world_model.py`

```
LSTM(64) → LSTM(32) ─┬── Dense(32) → Dense(5) softmax  (режим)
                      └── Dense(32) → Dense(5) linear   (OHLCV t+1)

Loss = L_regime + 0.05 · L_world
```

Каждая свеча → training sample. Даже убыточные периоды дают градиент.

### 2. Hermes: Tool Call World Model
Файл: `.hermes/scripts/tool_world_model.py`

Предиктор latency/success/cost для tool calls. Оркестратор может решать
делегировать или нет на основе предсказаний.

## Статус
- bybit-ws: модель реализована, обучение на BTC+ETH (365 дней)
- Hermes: скрипт готов, ждёт интеграции в оркестратор (cron для сбора, predict перед delegate_task)
