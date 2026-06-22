# Kaggle Day 5 — Production Deployment & A2A

> Дата: 16.06.2026  
> Репозиторий: `~/obsidian-vault/hermes/kaggle-5day-agents/Day5/`

---

## 5a: Agent2Agent (A2A) Protocol

### Проблема

- Один агент не может всё
- Разные команды делают разных агентов
- Нужен стандартный протокол для меж-агентной коммуникации

### Решение: A2A Protocol

Открытый стандарт (`a2a-protocol.org`), который позволяет агентам:
- 🌐 Общаться через сеть (HTTP)
- 🔧 Использовать возможности друг друга как tools
- 🌍 Работать cross-framework и cross-language
- 📋 Иметь формальные контракты (agent cards)

### Agent Card

Автогенерируемый JSON-манифест агента по пути `/.well-known/agent-card.json`:

```json
{
  "name": "product_catalog_agent",
  "description": "External vendor's product catalog agent",
  "url": "http://localhost:8001",
  "skills": [
    {
      "name": "get_product_info",
      "description": "Get product information",
      "input_schema": {...},
      "output_schema": {...}
    }
  ]
}
```

### Архитектура

```
┌──────────────────────┐           ┌──────────────────────┐
│ Customer Support     │  ─A2A──▶  │ Product Catalog      │
│ Agent (Consumer)     │           │ Agent (Vendor)       │
│ localhost:8000       │           │ localhost:8001       │
└──────────────────────┘           └──────────────────────┘
```

### A2A vs Sub-agents

| Фактор | A2A | Sub-agents |
|--------|-----|------------|
| **Где агент** | Внешний сервис | Внутри кодовой базы |
| **Владелец** | Другая команда | Твоя команда |
| **Сеть** | Разные машины | Тот же процесс |
| **Задержка** | Терпима | Минимальная |
| **Пример** | Внешний каталог товаров | Внутренняя обработка заказа |

### Ключевые примитивы

```python
# Expose agent
from google.adk.a2a.utils.agent_to_a2a import to_a2a
app = to_a2a(agent, port=8001)

# Consume remote agent
from google.adk.agents.remote_a2a_agent import RemoteA2aAgent
remote_agent = RemoteA2aAgent(
    name="product_catalog_agent",
    agent_card="http://localhost:8001/.well-known/agent-card.json"
)

# Use as sub-agent
root_agent.sub_agents = [remote_agent]
```

### Что это даёт

1. **Прозрачность** — потребитель не знает, что агент удалённый
2. **Стандарт** — любой A2A-совместимый агент работает
3. **Простота** — одна строка для интеграции
4. **Разделение зон ответственности** — vendor ↔ consumer

---

## 5b: Deploy to Vertex AI Agent Engine

### Структура артефакта

```
sample_agent/
├── agent.py                  # Логика агента
├── requirements.txt          # Зависимости
├── .env                      # GOOGLE_CLOUD_LOCATION, GOOGLE_GENAI_USE_VERTEXAI
└── .agent_engine_config.json # min/max instances, CPU, RAM
```

### Конфигурация деплоя

```json
{
    "min_instances": 0,
    "max_instances": 1,
    "resource_limits": {"cpu": "1", "memory": "1Gi"}
}
```

### Деплой одной командой

```bash
adk deploy agent_engine \
  --project=$PROJECT_ID \
  --region=$REGION \
  sample_agent \
  --agent_engine_config_file=sample_agent/.agent_engine_config.json
```

### Платформы (Google Cloud)

| Платформа | Для чего |
|-----------|----------|
| **Agent Engine** | Managed, auto-scale, специально для агентов |
| **Cloud Run** | Serverless, быстро стартовать |
| **GKE** | Полный контроль, сложные multi-agent системы |

### Memory Bank (долговременная память)

В отличие от **сессионной памяти** (забывается при завершении сессии), Memory Bank сохраняет факты между сессиями:

| Session Memory | Memory Bank |
|---------------|-------------|
| Одна беседа | Все беседы |
| Забывает при закрытии | Помнит всегда |
| «Что я сейчас сказал?» | «Какой мой любимый город?» |

Как работает:
1. Агент использует memory tools во время диалога
2. Agent Engine экстрактирует ключевые факты после беседы
3. Следующая сессия автоматически подгружает эти факты

---

## 🎯 Что берём в Hermes

| Концепт Kaggle | Аналог в Hermes | Что улучшить |
|----------------|-----------------|-------------|
| **A2A Protocol** | `delegate_task()` + MCP | Стандартизировать контракты (agent cards) |
| **Agent Card** | Описание в MCP server | Автогенерировать манифесты для тенантов |
| **Agent Engine** | systemd + cron + systemd-linger | Уже хорошо, но нет auto-scale |
| **Memory Bank** | SQLite сессии + Obsidian vault | ✅ Фактически есть |
| **adk deploy** | systemd unit + git push | Можем сделать `hermes deploy` |

### Что реально стоит внедрить

1. **A2A-подобный протокол** — стандартизировать меж-агентное общение:
   - Agent cards для каждого тенанта
   - HTTP API для remote agent consumption
   - Уже есть фундамент: `delegate_task` + MCP

2. **User Simulation** — из Day 4, самое важное (см. отдельный конспект)

3. **`hermes deploy`** — CLI-команда для деплоя тенантов как systemd-юнитов с авто-конфигурацией

---

## 📊 Сводка всего курса (5 дней)

| День | Тема | Ключевой навык |
|------|------|----------------|
| 1 | Основы | Создание первого агента с tools + instructions |
| 2 | Инструменты | Custom tools, MCP, лучшие практики |
| 3 | Сессии и память | Управление контекстом и долговременная память |
| 4 | Observability + Eval | Мониторинг агентов и измерение качества |
| 5 | Production | Деплой в облако и A2A коммуникация |
