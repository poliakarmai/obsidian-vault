---
tags: [tools, youtube, markdown, obsidian, howto]
created: 2026-06-23
source: https://github.com/JimmySadek/youtube-fetcher-to-markdown
---

# YouTube → Markdown: инструкция

## Установка

```bash
# Зависимости уже есть:
pip3 install yt-dlp youtube-transcript-api

# Скрипт:
~/.local/share/youtube-fetcher/fetch_transcript.py
```

## Использование

```bash
# Базовая команда (авто-язык)
python3 ~/.local/share/youtube-fetcher/fetch_transcript.py "URL" --force

# С указанием языка
python3 ~/.local/share/youtube-fetcher/fetch_transcript.py "URL" --force --lang ru

# Вывести в stdout (для AI-обработки)
python3 ~/.local/share/youtube-fetcher/fetch_transcript.py "URL" --force --stdout
```

## Выход

Файлы сохраняются в `~/yt_transcripts/` с именем `YYYY-MM-DD_slug_[VIDEO_ID].md`.

Формат: YAML frontmatter + таблица метаданных + описание + транскрипт.

## Что внутри

- **yt-dlp** — метаданные (название, канал, длительность, описание, главы)
- **youtube-transcript-api** — транскрипт/субтитры (авто-генерированные или ручные)

## Тест

```
URL: https://youtu.be/oFkldYJGKvI
Результат: ✅ 380 строк, русский авто-транскрипт, 24KB
Файл: ~/yt_transcripts/2026-06-23_блокада-началась..._[oFkldYJGKvI].md
```
