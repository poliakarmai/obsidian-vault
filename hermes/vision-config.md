---
tags: [hermes, vision, config, credentials]
created: 2026-06-23
---

# Vision: Google AI Studio (прямой доступ)

**Настроено:** 23.06.2026

## Конфигурация

```yaml
auxiliary:
  vision:
    provider: custom:google
    model: gemini-2.5-flash
    base_url: https://generativelanguage.googleapis.com/v1beta/openai
    api_key: <в config.yaml>
    timeout: 120
```

## Почему напрямую а не через freellmapi

- FreeLLMAPI роутер не уважает запрошенную модель — шлёт по цепочке всех провайдеров
- OpenRouter free-модели вымерли (404)
- HF требует оплату (402)
- Google-ключей в базе freellmapi не было

Решение: Google AI Studio даёт OpenAI-совместимый эндпоинт. Подключили напрямую.

## Где прописано

- `/home/openclaw/.hermes/config.yaml` (главный)
- `/home/openclaw/.hermes/profiles/<tenant>/config.yaml` (все 12 тенантов)

## YouTube Fetcher

- Скрипт: `~/.local/share/youtube-fetcher/fetch_transcript.py`
- Репо: https://github.com/JimmySadek/youtube-fetcher-to-markdown
- Зависимости: yt-dlp, youtube-transcript-api (обе есть)
- Вывод: Markdown с YAML frontmatter, Obsidian-ready
- Использование: `python3 ~/.local/share/youtube-fetcher/fetch_transcript.py "URL" --force`
