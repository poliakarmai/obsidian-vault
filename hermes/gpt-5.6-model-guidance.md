# GPT-5.6 — Полный конспект (OpenAI Docs)

> Источники:
> - https://developers.openai.com/api/docs/guides/latest-model (Model Guidance)
> - https://developers.openai.com/api/docs/guides/reasoning (Reasoning Models)
> - https://community.openai.com/t/introducing-gpt-5-6-series-sol-terra-and-luna/1384931
> - https://o-mega.ai/articles/openai-gpt-5-6-practical-guide-july-2026
> Дата: 10 июля 2026

---

## Модельная линейка

| Модель | Назначение | Алиас | Цена (вход/выход $/M tok) |
|--------|-----------|-------|---------------------------|
| **GPT-5.6 Sol** | Флагман: frontier reasoning, long-horizon агенты | `gpt-5.6` (по умолчанию) | $5/$30 |
| **GPT-5.6 Terra** | Баланс: GPT-5.5-уровень, 2× дешевле | `gpt-5.6-terra` | $2.50/$15 |
| **GPT-5.6 Luna** | Эффектив: high-volume, макс скорость | `gpt-5.6-luna` | $1/$6 |

**Ключевой принцип миграции:** не просто сменить slug модели. Начать с текущих настроек reasoning, затем протестировать на уровень ниже.

---

## Что нового в GPT-5.6

### Programmatic Tool Calling (PTC)
- Модель пишет JavaScript → вызывает eligible tools → обрабатывает результаты в рантайме
- **Когда использовать:** bounded workflows — фильтрация, join, ранжирование, агрегация
- **Когда НЕ использовать:** один вызов, малые результаты, каждое изменение требует fresh model judgment, approval-действия
- Шаблон промпта:
```xml
<tool_orchestration>
Use Programmatic Tool Calling for [bounded stage] using only [eligible tools].
Run independent calls concurrently when safe.
Process and reduce the intermediate results, then emit exactly [output schema].
Stop when [condition] is met. Retry transient failures at most [R] times.
Use direct tool calls for [semantic judgment, approval, or final validation].
</tool_orchestration>
```

### Multi-agent (beta)
- Один инстанс GPT-5.6 координирует суб-агентов параллельно
- Responses API, beta

### Explicit Prompt Caching
- Ручная маркировка кешируемых префиксов через `prompt_cache_options.mode: "explicit"`
- Запись кеша: **1.25×** от uncached input rate
- Чтение кеша: со скидкой
- TTL через `prompt_cache_options.ttl` (замена `prompt_cache_retention`)

### Persisted Reasoning
- Переиспользование reasoning между ходами через `reasoning.context`:
  - `auto` — дефолт модели
  - `current_turn` — только текущий ход
  - `all_turns` — рендерит reasoning из предыдущих ходов
- Для `store: false` / Zero Data Retention: `include: ["reasoning.encrypted_content"]`

### Max Reasoning Effort + Pro Mode
- **Efforts:** `none` → `low` → `medium` → `high` → `xhigh` → `max`
- **Pro mode** (`reasoning.mode: "pro"`) — больше модельной работы перед финальным ответом
- Mode и effort **независимы**
- Pro mode биллится по стандартным тарифам модели
- **Включать в API, не в промпте**

### Другие улучшения
- Токен-эффективность: frontier performance с меньшим числом токенов
- Frontend: лучше вёрстка, визуальная иерархия, дизайн
- Intent understanding: лучше угадывает цель без пошаговых инструкций
- Original image detail: сохраняет исходные размеры изображений

---

## Reasoning: полное руководство

### Уровни effort

| Effort | Для чего | Примеры |
|--------|----------|---------|
| `none` | Latency-critical, без reasoning | Voice, классификация, быстрый retrieval |
| `low` | Эффективный reasoning, небольшой latency | Data analysis, drafting, coding, support |
| `medium` | Баланс качество/скорость **(дефолт)** | Agentic coding, research, spreadsheets |
| `high` | Сложные задачи, качество > скорость | Complex debugging, long-horizon research |
| `xhigh` | Глубокий research, async workflows | Security review, enterprise productivity |
| `max` | Максимальное качество | Только когда xhigh недостаточно |

### GPT-5.6: дефолтный effort = medium (оба режима)

### Pro mode
```bash
curl https://api.openai.com/v1/responses \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-5.6",
    "reasoning": {"mode": "pro", "effort": "medium"},
    "input": "..."
  }'
```
- Больше model work → один финальный ответ
- Выше latency, агрегирует токены
- **Выбирать на основе тестов, не предположений**

### Persisted reasoning
```python
# all_turns: рендерит reasoning из предыдущих ответов
first = client.responses.create(
    model="gpt-5.6",
    input="Inspect this repo and find the bug.",
    reasoning={"context": "current_turn"},
)
second = client.responses.create(
    model="gpt-5.6",
    previous_response_id=first.id,
    input="Now patch the bug.",
    reasoning={"context": "all_turns"},
)
```

### Контроль costs
- `max_output_tokens` лимитирует reasoning + output токены
- Резервировать ≥25,000 токенов для reasoning при старте
- Проверять `response.status == "incomplete"` и `incomplete_details.reason == "max_output_tokens"`

---

## Промптинг: лучшие практики (GPT-5.6)

### 1. Короче = лучше
Внутренние тесты OpenAI:
- **+10–15% качества** при замене длинных промптов на минимальные
- **-41–66% токенов**
- **-33–67% стоимости**

> «Многие старые инструкции в харнессах стали дефолтным поведением модели. Фокусируйтесь только на том, что модель НЕ делает сама.»

### 2. Автономия и разрешения — компактно
```
Для «ответь/объясни/проверь» → инспектируй, докладывай, НЕ внедряй.
Для «измени/построй/почини» → делай in-scope локально, валидируй без спроса.
Подтверждение для: внешних записей, деструктивных действий, покупок.
```
**Не повторяй** «спроси сначала» — вызывает лишние permission checks.

### 3. Стиль: приоритизация, не «будь кратким»
GPT-5.6 УЖЕ сжат. «Будь кратким» может заставить модель ВЫБРОСИТЬ контент.

✅ Правильно:
```
Начни с вывода. Приложи доказательства, оговорки, следующее действие.
Опусти вторичные детали и повторения.
```

❌ Неправильно:
```
Будь кратким. Используй минимум текста.
```

### 4. Легковесная структура
Лёгкий outline под задачу, не глобальный шаблон. Узкие ограничения — только если тесты доказывают.

### 5. Тон (warmth)
✅ Конкретно:
```
Будь прямым и тактичным. Отмечай friction когда релевантно.
Избегай шаблонных утешений.
```

❌ Не надо:
```
Будь дружелюбным и тёплым.
```

### 6. Pro mode — в API, не в промпте
Не проси модель «думать усерднее» или «использовать pro mode». Включай `reasoning.mode: "pro"` в API.

---

## Миграция: чеклист

1. **Выбрать модель:** `gpt-5.6` (Sol) / `gpt-5.6-terra` / `gpt-5.6-luna`
2. **Responses API** для reasoning и tool calling
3. **`reasoning.effort`** явно: сохранить baseline, тестировать на уровень ниже
4. **Persisted reasoning:** `all_turns` если цели стабильны
5. **Prompt caching:** `explicit` для избежания лишних cache writes (1.25×)
6. **PTC:** добавить `programmatic_tool_calling` tool + `allowed_callers`
7. **Бенчмарк:** task success, полнота, evidence, total tokens, latency, cost

---

## Что применимо к Hermes

### Системный промпт → сократить
- Убрать дублирующиеся инструкции
- Один блок автономии без повторов
- Лёгкий outline вместо шаблона

### Стиль → приоритизация
- «Начни с вывода» вместо «будь кратким»
- Конкретный тон вместо «будь дружелюбным»

### Tool calling
- PTC для batch-операций в перспективе
- Описания тулов: точные типы возврата и ошибок

### Кеширование + reasoning
- Explicit caching для длинных системных промптов
- `all_turns` для persisted reasoning в cron и сессиях

### Safeguards
- GPT-5.6 имеет real-time классификаторы безопасности (cyber + bio)
- Могут блокировать легитимные запросы (code review, security research)
- Рекомендуется `safety_identifier` для end-user приложений
