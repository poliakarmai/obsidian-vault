---
tags: [roadmap, orchestration, hermes]
updated: 2026-06-28
---

# Roadmap оркестрации Hermes

## ✅ Сделано

| Задача | Статус |
|--------|--------|
| Multi-tenant изоляция (8 тенантов) | ✅ |
| Baseline-скиллы для всех тенантов | ✅ |
| Gemini API для vision | ✅ |
| DSPy → DeepSeek training | ✅ |
| bybit-ws self-learning в main loop | ✅ |
| pump_state авто-очистка | ✅ |
| PR #52823 (macOS symlink fix) | 🟡 ждёт форк |

## ⬜ В плане

### Self-Evolution — авто-эволюция навыков (следующий уровень)

**Идея:** агент сам читает трассы ошибок (self_learn.jsonl, events.log), находит повторяющиеся сбои и предлагает правки в SKILL.md.

**Источник:** статья Влада Смирнова «Как AI-агенты учатся на практике» — Hermes Self-Evolution.

**Что нужно:**
- Накопить достаточно self_learn.jsonl (>100 записей)
- Фоновый агент (cron, раз в сутки) анализирует трассы
- Находит паттерны ошибок → предлагает diff в навык
- Человек ревьюит → применяет или отклоняет

**Метрики готовности:**
- ≥100 записей в self_learn.jsonl
- ≥30 закрытых сделок в post_trade_features.jsonl
- Стабильный поток ошибок для анализа

### DSPy → самообучение стратегий

- Сейчас: weekly-retrain (воскресенье 03:00)
- В плане: daily-retrain при >10 новых сделок
- Авто-подбор threshold для ML Gate

### OpenAI Agents SDK — интеграция

- Изучить возможность замены self-written loops на Agents SDK
- Handoff-ы между агентами (entry agent → risk agent → execution agent)

### AG-UI / Agent-User Interaction Protocol

- Сбор сигнала от пользователей (исправления агента человеком)
- Превращение исправлений в процедурную память
