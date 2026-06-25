---
tags: [ocr, baidu, ai, pdf, tools]
created: 2026-06-23
updated: 2026-06-23
source: "https://github.com/baidu/Unlimited-OCR"
huggingface: "baidu/Unlimited-OCR"
paper: "https://arxiv.org/abs/2606.23050"
stars: 2207
likes: 362
downloads: 8396
---

# Baidu Unlimited OCR

**One-shot long-horizon parsing.** Считывает весь документ целиком, не по частям.

## Ключевые факты

- Релиз: **23 июня 2026** (сегодня)
- На базе DeepSeek-OCR, улучшенная версия
- `transformers` + CUDA 12.9 + torch 2.10
- Два режима: `gundam` (640px, crop) и `base` (1024px, без crop)
- `infer_multi()` — multi-page PDF

## API

```python
model = AutoModel.from_pretrained("baidu/Unlimited-OCR", trust_remote_code=True)

# Одна страница
model.infer(tokenizer, prompt="<image>document parsing.", image_file="page.jpg")

# Много страниц (PDF)
model.infer_multi(tokenizer, prompt="<image>Multi page parsing.", 
                  image_files=["p1.png","p2.png","p3.png"])
```

## Статус для нас

| Ресурс | Доступность |
|--------|------------|
| GitHub | ✅ репо открыт |
| HuggingFace | ✅ модель загружена |
| GPU (локально) | ❌ нет CUDA |
| HF Inference API | ❌ не поднято |
| ModelScope | ✅ доступно |
| CPU fallback | ❌ не предусмотрен |

## План действий

1. 🔴 Сейчас — наблюдать, модель свежая
2. 🟡 Дождаться HF Inference API или Replicate
3. 🟡 Или арендовать GPU (RunPod/Modal) для разовых прогонов
4. 🟢 Когда заработает — сразу в дефектоскопист (ГОСТы) и D.V. (прайсы)

## Ссылки

- GitHub: https://github.com/baidu/Unlimited-OCR
- HF: https://huggingface.co/baidu/Unlimited-OCR
- Paper: https://arxiv.org/abs/2606.23050
- ModelScope: https://modelscope.cn/models/PaddlePaddle/Unlimited-OCR
