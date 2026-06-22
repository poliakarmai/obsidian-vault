# Crypto Agent — MCP-сервер крипто-анализа

> Адаптирован из finagent (Hands-On AI Engineering)
> DeepSeek + bybit-ws RPC вместо Gemini + yfinance
> Дата: 12.06.2026

## Архитектура

```
User NL Query → Query Parser (DeepSeek) → Market Analyst (DeepSeek) + bybit-ws RPC → Structured Report
```

## MCP тулы

- `analyze_portfolio(query)` — анализ позиций через DeepSeek
- `health_check()` — статус bybit-ws + позиции

## Файлы

- `~/.hermes/scripts/crypto-agent/server.py` — MCP-сервер
- Venv: `/tmp/crypto-agent/`

## Запуск

```bash
/tmp/crypto-agent/bin/python3 ~/.hermes/scripts/crypto-agent/server.py
```

## Примеры запросов

- «Какие позиции самые рискованные?»
- «Что делать с MOVE?»
- «Дай рекомендации по стоп-лоссам»
- «Какие позиции пора фиксировать?»
