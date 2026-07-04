---
tags: [tools, llm, self-hosted, webui]
created: 2026-06-30
status: idea
---

# Open WebUI

**Сайт:** https://openwebui.com
**GitHub:** https://github.com/open-webui/open-webui

Локальный ChatGPT-подобный интерфейс. Подключается к Ollama или OpenAI-совместимым API. Полностью самодостаточный.

## Фичи

- RAG (загрузка документов)
- Веб-поиск
- Мульти-пользовательский доступ с ролями
- Загрузка файлов
- Совместимость с OpenAI API

## Установка (одна команда)

```bash
docker run -d -p 3000:8080 \
  -v open-webui:/app/backend/data \
  -e OPENAI_API_BASE_URL=http://localhost:8888/v1 \
  -e OPENAI_API_KEY=not-needed \
  --name open-webui \
  ghcr.io/open-webui/open-webui:main
```

После запуска: http://localhost:3000

## Подключение к нашим API

| Бэкенд | URL |
|--------|-----|
| FreeLLMAPI | `http://localhost:8888/v1` |
| DeepSeek | `https://api.deepseek.com/v1` |

## Требования

- Docker
- ~500MB-1GB RAM
- Порт 3000

## Статус

⏳ Отложено. Поверхностно — Docker есть, памяти 2.1GB свободно, впритык.
