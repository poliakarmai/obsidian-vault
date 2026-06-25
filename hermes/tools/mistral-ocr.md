---
tags: [ocr, mistral, ai, api, documents]
created: 2026-06-23
source: "Mistral AI"
model: "mistral-ocr / CX-9"
---

# Mistral OCR 4

API-based OCR от Mistral. 170 языков, bounding boxes, классификация блоков, confidence scores.

## Ключевые возможности

- Bounding boxes на уровне абзацев
- Классификация блоков (заголовок/текст/таблица/изображение)
- Confidence scores: per-word или per-page
- Извлечение таблиц
- Извлечение изображений
- Структурированный вывод: JSON Schema
- Header/footer extraction
- 170 языков

## Использование

```python
from mistralai.client import Mistral

with Mistral(api_key="...") as client:
    res = client.ocr.process(
        model="mistral-ocr",
        document={"type": "document_url", "document_url": "https://..."},
        include_blocks=True,
        confidence_scores_granularity="word",
    )
```

## Статус для нас

| Ресурс | Доступность |
|--------|------------|
| SDK | ✅ mistralai 2.4.8 |
| API key | ❌ нет |
| GPU | не нужен (API) |
| Цена | платно (per page) |

## Сравнение с аналогами

| Модель | Тип | GPU | Языки | Блоки | BBox |
|--------|-----|-----|-------|-------|------|
| **Mistral OCR** | API | ❌ | 170 | ✅ | ✅ |
| Baidu Unlimited OCR | open | ✅ | ? | ⬜ | ⬜ |
| Tesseract | open | ❌ | 100+ | ❌ | ✅ |
| PaddleOCR | open | ❌ | 80+ | ❌ | ✅ |

## Приоритет

🟡 Высокий — если добудем ключ. Идеально для дефектоскописта (ГОСТы со сложной вёрсткой) и D.V. (прайсы с таблицами).
