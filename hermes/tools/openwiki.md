# OpenWiki

**GitHub:** https://github.com/langchain-ai/openwiki (945 ⭐)
**Автор:** LangChain
**Лицензия:** MIT

CLI-инструмент для генерации wiki-документации репозитория. Решает проблему раздувания AGENTS.md/CLAUDE.md.

## Как работает

Вместо того чтобы пихать весь контекст проекта в AGENTS.md, OpenWiki:
- Создаёт папку `openwiki/` со структурированной документацией
- В AGENTS.md добавляет только короткую ссылку на вики
- Генерирует страницы: архитектура, CLI, операции, source map, правила работы с кодом

## Команды

```
npm install -g openwiki
openwiki --init          # первичная генерация
openwiki --update        # обновление по git diff
```

## Провайдеры

OpenRouter, Fireworks, Baseten, OpenAI, Anthropic
+ опционально LangSmith для трассировки

## GitHub Action

Встроенный action для ежедневного PR с обновлением документации.
Безопасный режим: обновления через PR → ревью как код → мёрж.

## Статус

Добавлено: 03.07.2026. Не тестировалось.
Кандидат на внедрение в: bybit-ws, hermes-trader, vpn-infra.
