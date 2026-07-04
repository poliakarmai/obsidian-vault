
---

## PPT-Master (июнь 2026)

**Репозиторий:** `~/ppt-master/` (клон `github.com/hugohe3/ppt-master`, v2.11.0, MIT)  
**Автор:** Hugo He (Китай, CPA/CPV/консультант по инвестициям)  
**Назначение:** AI-генерируемые нативные PPTX из любого документа

**Вход:** PDF, DOCX, XLSX, Markdown, URL, PPTX  
**Выход:** Редактируемый `.pptx` с DrawingML-шейпами, анимациями, аудионаррацией speaker notes

**Установка:** `~/ppt-master/.venv/` (Python 3.11, все зависимости)  
**Активация:** `source ~/ppt-master/.venv/bin/activate`

**Конвертеры источников:**
- `pdf_to_md.py` → PDF → Markdown (PyMuPDF)
- `doc_to_md.py` → DOCX/HTML/EPUB → MD (mammoth)
- `excel_to_md.py` → XLSX → MD (openpyxl)
- `web_to_md.py` → URL → MD (requests+bs4)
- `ppt_to_md.py` → PPTX → MD

**Работает как skill** для: Claude Code, Cursor, VS Code + Copilot, Codebuddy  
**Стоимость:** ~$0.08/колода (только токены LLM)  
**Ключевая фишка:** не картинки слайдов, а нативные объекты PowerPoint


## Supermemory (28K ⭐)

Локальный memory-движок для AI-агентов. Graph engine + embeddings + извлечение фактов + user profiles.

- Запуск: `npx supermemory local` или `supermemory-server`
- Модели: OpenAI, Anthropic, Gemini, Groq, Ollama (офлайн)
- Интеграции: Claude Code, Cursor, Codex, Hermes, LangChain, Vercel AI SDK
- Хранение: `$SUPERMEMORY_DATA_DIR` или `./supermemory/`
- Конфиг: `~/.supermemory/env`
- GitHub: https://github.com/supermemoryai/supermemory
- Статус: установлен 02.07.2026, не интегрирован

Потенциал: замена BM25-поиска на семантический, авто-факты из сессий, граф знаний.

## Claude Video Watch (02.07.2026)

Видео Ромарая: «Как заставить Claude смотреть видео в YouTube за тебя»
https://youtu.be/So3srrfKiWg

**Суть:** Claude Code может не просто читать транскрипцию, а РЕАЛЬНО смотреть видео:
- Разбирает на скриншоты по тайм-кодам
- Видит интерфейс, действия на экране, детали
- Связывает визуал с транскрипцией
- Готовит план доработок, находит баги

**Инструменты (бесплатные):**
- Команда `/watch` — ссылка на YouTube → полный разбор
- Три open-source пакета для обработки видео
- Работает с YouTube, записями созвонов, обычными видеофайлами

**Use cases:**
- Разбор скринкастов с багами → авто-фиксы
- Просмотр обучающих видео → конспект без просмотра
- Созвоны с клиентами → Claude смотрит и формирует задачи

**Статус:** не интегрировано. Потенциал: Hermes + Claude Code + video watch.

## Студенческие подписки — агрегатор халявы (02.07.2026)

Китайский сайт-агрегатор студенческих скидок/подписок/льгот. Есть инструкции как получить .edu почту не будучи студентом.

**Что даёт студенческая почта:**
- GitHub Student Developer Pack
- JetBrains (все IDE бесплатно)
- Microsoft Office, Azure, GitHub Copilot
- Adobe CC (скидка), Notion, Canva
- Облачные сервисы, AI-инструменты
- MATLAB, Shodan, Goodnotes, iLovePDF

**На сайте:** 30+ карточек сервисов с инструкциями. Теги: «Популярные предложения», «Обязательно для офисной работы», «Академические исследования», «Доступно облачная», «Китайский ИИ».

**Как получить .edu:**
- Через некоторые зарубежные вузы с открытой регистрацией
- Инструкции на сайте (нужен перевод страницы)
- Student Beans, Student App Centre — агрегаторы скидок

**Статус:** не использовано. Можно разово получить .edu и активировать подписки.
