# Awesome AI OSINT

**Репозиторий:** [ubikron/Awesome-AI-OSINT](https://github.com/ubikron/Awesome-AI-OSINT)
**Дата:** 2026-06-14
⭐ 418 · 🍴 64

---

## Главная идея

Кураторский список инструментов, статей и видео по применению AI (ChatGPT, Claude, Grok) для OSINT-задач.

## Ключевые разделы

### Статьи
- Prompt Engineering для OSINT
- AI + OSINT: стратегии расследований
- Критика: «Ты не OSINT-аналитик, ты prompt monkey»

### Инструменты
- Lenso.ai — обратный поиск изображений
- Vehicle Identifier — определение авто по фото
- OSINT GPT (кастомные GPT от сообщества)
- ZoomEye GPT, CensysGPT, ShodanGPT — AI поверх поисковых движков

### MCP-серверы
- [OSINT Tools MCP Server](https://github.com/frishtik/osint-tools-mcp-server)

### Скиллы для OpenClaw / Claude Code
- OSINT Graph Analyzer
- Xint — X/Twitter intelligence
- OSINT Investigator
- Multi Search Engine
- Find People

## Применимость к Hermes

| Инструмент | Что можно сделать |
|-----------|-------------------|
| OSINT MCP Server | Подключить к Hermes как MCP-источник для разведки |
| OSINT Graph Analyzer | Анализ связей между крипто-адресами / инвесторами PCI |
| Lenso.ai | Поиск по логотипам проектов, проверка KYC |
| Xint | Мониторинг инфлюенсеров для CORE-монет |

## TODO

- [x] Подключить OSINT Tools MCP к Hermes ✅ (2026-06-14)
- [ ] Проверить OSINT Graph Analyzer для крипто-разведки
- [x] Создать скилл `osint-tools` для Hermes ✅ (2026-06-14)

## Установленный MCP-сервер

**Сервер:** `/opt/osint-tools/mcp-server/`
**Скилл Hermes:** `osint-tools` (категория: research)
**Конфиг:** `~/.hermes/config.yaml` → `mcp_servers.osint-tools`

Доступные инструменты через MCP:
- `sherlock_username_search` — поиск username по 399+ сайтам
- `holehe_email_search` — проверка email на 120+ платформах
- `maigret_username_search` — продвинутый поиск (3000+ сайтов)
- `theharvester_domain_search` — разведка по домену
- `spiderfoot_scan` — комплексный скан (5-30 мин)
- `ghunt_google_search` — информация о Google-аккаунте
- `blackbird_username_search` — быстрый поиск по 581 сайту

⚠️ После изменения конфига нужен **ребут Hermes**: `sudo systemctl restart hermes`
