# Kaggle Day 4 — Observability & Evaluation

> Дата: 16.06.2026  
> Репозиторий: [ajmal-uk/5-Day-AI-Agents-Intensive-Course-with-Google](https://github.com/ajmal-uk/5-Day-AI-Agents-Intensive-Course-with-Google)  
> Локально: `~/obsidian-vault/hermes/kaggle-5day-agents/`

---

## 4a: Agent Observability

### Три столпа

| Столп | Вопрос | Аналог в Hermes |
|-------|--------|-----------------|
| **Logs** | Что произошло? | `events.log` (log_event) |
| **Traces** | Почему так вышло? | `session_search()` — сессии с tool calls |
| **Metrics** | Насколько хорошо? | Prometheus `/metrics` (частично) |

### Ключевая идея

Традиционный APM показывает 200 OK, а агент мог тихо вызвать не тот tool. Observability агентов — **семантическая**, не инфраструктурная.

### Спаны в трейсе (4 типа)

```
Tool-call spans:  имя инструмента, аргументы, вывод, latency, retries
Reasoning spans: план → действие → наблюдение → решение
State spans:     состояние до/после шага (контекст, память)
Memory spans:    чтение/запись, результаты поиска, свежесть
```

### Практика в ноутбуке

1. Создали агента `research_paper_finder` с намеренной ошибкой: `count_papers(papers: str)` вместо `List[str]`
2. Запустили `adk web --log_level DEBUG` — видно полные промпты, ответы LLM, вызовы tools
3. Через Web UI нашли ошибку: `TypeError: object of type 'str' has no len()`
4. Исправили сигнатуру — агент заработал

### Production logging

```python
# Встроенный CloudLogging (Vertex AI)
from google.adk.utils.log_entry import log_event

log_event(
    session=session,
    event_type="custom_metric",
    payload={"key": "value"}
)
```

---

## 4b: Agent Evaluation

### Observability vs Evaluation

```
Observability = РЕАКТИВНАЯ (после бага)
Evaluation    = ПРОАКТИВНАЯ (до бага)
```

### Формат eval case

```json
{
  "eval_id": "living_room_light_on",
  "conversation": [{
    "user_content": {"parts": [{"text": "Turn on the floor lamp"}]},
    "final_response": {"parts": [{"text": "Successfully set..."}]},
    "intermediate_data": {
      "tool_uses": [{
        "name": "set_device_status",
        "args": {"location": "living room", "device_id": "floor lamp", "status": "ON"}
      }]
    }
  }]
}
```

### Метрики оценки

| Метрика | Что меряет | Порог |
|---------|-----------|-------|
| `tool_trajectory_avg_score` | Правильные ли инструменты + аргументы | 1.0 (точное совпадение) |
| `response_match_score` | Совпадает ли текст ответа | 0.8 (80% similarity) |

### Диагностика отказов

| Tool | Response | Диагноз | Действие |
|------|----------|---------|----------|
| ❌ | ✅ | Тул не тот, но ответ норм | Чинить tool contract |
| ✅ | ❌ | Тул правильный, текст кривой | Чинить prompt/instruction |
| ❌ | ❌ | Глубокая логическая ошибка | Трассировка всей цепочки |

### CLI для regression testing

```bash
adk eval home_automation_agent \
  home_automation_agent/integration.evalset.json \
  --config_file_path=home_automation_agent/test_config.json \
  --print_detailed_results
```

---

## 🔥 User Simulation (самое мощное)

Вместо статичных eval cases — **LLM-симулятор пользователя**, который динамически генерирует запросы по `ConversationScenario`:

- Ты задаёшь **цель диалога** и **план беседы**
- Другой LLM играет роль пользователя, адаптируясь к ответам агента
- Ловит edge cases, которые статические тесты никогда не найдут

### Структура

```python
ConversationScenario(
    goal="User wants to control multiple smart devices",
    conversation_plan=[
        "Ask to turn on lights",
        "If agent succeeds, ask to turn off something else",
        "Deliberately use ambiguous device names",
        "Request a device that doesn't exist"
    ]
)
```

---

## 🎯 Что берём в Hermes

| Концепт | Статус | Приоритет |
|---------|--------|-----------|
| **User Simulation** | Отсутствует | 🔴 Высокий |
| **CI eval gate (adk eval)** | Частично (project-audit) | 🟡 Средний |
| **Trace visualisation** | session_search (текст) | 🟢 Низкий |
| **Safety + hallucination eval** | Отсутствует | 🟡 Средний |
| **Braintrust-style dashboard** | Отсутствует | 🟢 Низкий |

### Конкретный план

1. **User Simulation** — написать Hermes-совместимый симулятор пользователя:
   - `ConversationScenario` с целями и планом
   - Запуск второго агента (или DeepSeek) как «пользователя»
   - Автоматическая оценка качества ответов через LLM-as-judge
   
2. **Формат eval cases** — адаптировать `.evalset.json` формат для Hermes:
   - Сохранять сессии как eval cases
   - CLI-команда `hermes eval` для regression testing

---

## 📎 Файлы репозитория

```
kaggle-5day-agents/
├── Day1/
│   ├── day-1a-from-prompt-to-action.ipynb
│   └── day-1b-agent-architectures-eb9049.ipynb
├── Day2/
│   ├── day-2a-agent-tools.ipynb
│   └── day-2b-agent-tools-best-practices-2af7d1.ipynb
├── Day3/
│   ├── day-3a-agent-sessions (1).ipynb
│   └── day-3b-agent-memory.ipynb
├── Day4/
│   ├── day-4a-agent-observability.ipynb      ← этот конспект
│   ├── day-4b-agent-evaluation.ipynb         ← этот конспект
│   └── Agent Quality.pdf
├── Day5/
│   ├── day-5a-agent2agent-communication.ipynb
│   ├── day-5b-agent-deployment.ipynb
│   └── Prototype to Production.pdf
└── Readme.md
```
