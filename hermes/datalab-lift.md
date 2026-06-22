# Datalab Lift — 9B structured extraction

**Дата:** 2026-06-20
**Источник:** https://www.datalab.to/blog/introducing-lift
**GitHub:** https://github.com/datalab-to/lift
**HF:** https://huggingface.co/datalab-to/lift

---

## Что это

**Lift** — open-weights (Apache 2.0) 9B vision-модель от Datalab (авторы marker, surya, chandra) для извлечения структурированных данных из PDF и изображений.

**Принцип:** кидаешь PDF/изображение + JSON Schema → получаешь строго валидный JSON. Schema-constrained decoding гарантирует, что модель **не сгенерирует** поле вне схемы.

## Бенчмарки

| Модель | Точность (field accuracy) | Скорость |
|---|---|---|
| **Lift** | **90.2%** | **9.5s медиана** |
| Gemini 3.5 Flash | 91.3% | ~30s |
| NuExtract3 (open) | 81.5% | — |
| Datalab API (hosted) | выше за счёт verification | дольше |

Вывод: Lift — **всего -1.1% от Gemini, но в 3× быстрее** и open-source.

## Как использовать

```bash
pip install lift-pdf[hf]    # HF-режим (загрузка весов локально)
pip install lift-pdf[vllm]  # vLLM-сервер (быстрее, нужен GPU)
```

```python
from lift.model import InferenceManager
model = InferenceManager(method="hf")

result = model.extract(
    "invoice.pdf",
    schema={"type": "object", "properties": {
        "invoice_number": {"type": "string"},
        "total": {"type": "number"}
    }}
)
# → {"invoice_number": "INV-2024-001", "total": 1500.00}
```

CLI:
```bash
lift "документ.pdf" --schema schema.json
```

## Feature highlights

- **Schema-constrained decoding** — не парсишь «почти JSON», всегда валидный вывод
- **PDF и изображения** — работает напрямую, не нужен предварительный OCR
- **Мультистраничные PDF** — `page_range="0-5"` лимит по страницам
- **InferenceManager** — переиспользование модели в памяти
- **vLLM / SGLang / Docker** — любые инференс-бэкенды
- **Лицензия:** Apache 2.0 для некоммерческого использования. Коммерция — отдельная лицензия.

## Применимость к нашим задачам

| Задача | Документы | Схема | Сложность |
|---|---|---|---|
| **Gazprom: акты осмотра** | PDF трубопроводов | дата, объект, давление, толщина, заключение | средняя |
| **Сертификаты / паспорта** | PDF оборудования | номер, дата, стандарт, параметры | низкая |
| **ОСК / коррозия** | Табличные отчёты | массив измерений с локациями | высокая |
| **СМКТО / DLA** | Протоколы диагностики | тип, глубина, координаты, заключение | высокая |

## План внедрения

1. **Фаза 0 — тест через hosted API** (Datalab Playground) на 5-10 реальных документах
2. **Фаза 1 — если ок:** поднять vLLM на RunPod (~$0.5/ч) с моделью `datalab-to/lift`
3. **Фаза 2 — интеграция в hermes-пайплайн:** `ocr-rag` скилл → добавить Lift как extraction-бэкенд
4. **Фаза 3 — поток:** cron-джоба на batch-обработку Gazprom-документов

## Ограничения

- **Нужен GPU.** 9B модель — CPU-инференс возможен, но медленный (минуты вместо секунд)
- **Schema quality matters.** Чем точнее схема — тем лучше extraction. Нужно инвестировать время в схемы под каждый тип документа
- **Не 100% точность.** ~90% — значит 1 из 10 полей может быть с ошибкой. Для критичных данных нужна верификация
- **Коммерческая лицензия.** Для использования в продукте нужна отдельная лицензия Datalab

## Ссылки

- [[hermes/00-Index|Hermes Index]]
- [[ocr-rag]] — текущий OCR-стек
- [[gazprom-work]] — документация Газпром
