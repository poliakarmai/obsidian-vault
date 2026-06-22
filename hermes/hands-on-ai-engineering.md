# Hands-On AI Engineering — выжимка

> Источник: [Sumanth077/Hands-On-AI-Engineering](https://github.com/Sumanth077/Hands-On-AI-Engineering)
> Лицензия: MIT
> Дата: 12.06.2026

## 🔥 Что взяли для Hermes

### 1. Finagent — MCP-сервер для финансового анализа
**Стек:** Gemini 2.5 Flash + yfinance + FastMCP

**Архитектура:**
```
User Query → Query Parser Agent → Market Analyst Agent → Structured Report
```

**MCP-инструменты:** `analyze_stock`, `execute_code`, `get_news`

**Паттерн для нас:** замена Gemini на DeepSeek + доработка под крипту. MCP-сервер уже умеем делать (bybit-ws MCP).

### 2. Stock Portfolio Analyst — DeepSeek + Agno
**Стек:** DeepSeek-V4-Flash (NVIDIA API) + Agno framework + YFinance + DuckDuckGo + Gradio

**Ключевой паттерн:** streaming analysis — отчёт стримится в UI по мере генерации

**Инструкция агента (из agent.py):**
- 6 шагов: fetch → calculate → portfolio metrics → news → verify → risk flags
- Структурированный вывод: Summary → Holdings → Performers → Risk → Rebalancing → News
- Правило: «Always fetch live data — never estimate prices»

### 3. Eagle Eye — PR Review через Telegram
**Стек:** OpenClaw + MiniMax M2.7 + GitHub MCP + Telegram

**Паттерн SOUL.md:** ядро агента — markdown-файл с идентичностью, тоном, критериями ревью и workflow. Прямой аналог наших скиллов.

**Workflow:** PR URL → fetch diff → analyze → draft review → ждать approve → пост

**Шкала severity:** 🔴 Critical → 🟠 Warning → 🟡 Suggestion → 🔵 Nitpick

**Рейтинг:** ✅ Approved / ✅ Approved w/ suggestions / 🔄 Request changes / ❌ Blocked

### 4. Daily AI News Digest — паттерн для crypto-дайджеста
**Стек:** 92 RSS-фида + MiniMax M2.7 + Telegram

**Паплайн:**
```
92 RSS feeds → fetch_rss → filter 24h → LLM scoring → top 3 → summarise → categorise → Telegram
```

**SKILL.md формат:**
```yaml
name: daily-ai-news-digest
trigger: "0 8 * * *"
metadata: {openclaw: {requires: {env: [...], bins: [...]}}}
```

**Для нас:** заменить RSS на crypto-источники (CoinDesk, CoinTelegraph, Twitter) → crypto-daily-digest скилл.

### 5. Marketing Strategy Agent — мультиагентный пайплайн
**Стек:** DeepSeek-V4-Flash (Orq.ai) + Serper + Gradio

**3 агента последовательно:**
```
Market Analyst (Serper search) → Strategy Officer (positioning) → Creative Director (copy)
```

**Паттерн для нас:** sequential agent pipeline — один строит на выходе другого. Можно адаптировать для trading (Analyst → Strategy → Execution).

---

## Что можно внедрить прямо сейчас

| Проект | Паттерн | Куда |
|--------|---------|------|
| finagent | MCP-сервер для финансов | Доработать bybit-ws MCP |
| stock_portfolio_analyst | Streaming analysis + Agno | Для портфельного дашборда |
| eagle_eye | SOUL.md + approve flow | Уже используем скиллы |
| daily-news-digest | RSS → scoring → Telegram | crypto-daily-digest |
| marketing_strategy_agent | 3-agent sequential pipeline | Для trading-решений |

## Технические детали

### finagent — код
- `main.py`: FastMCP сервер, один тул `analyze_stock(query: str)`
- `financial_agents.py`: Query Parser → Market Analyst, yfinance для данных
- Gemini 2.5 Flash, заменить на DeepSeek

### stock_portfolio_analyst — код
- `agent.py`: Agno Agent + OpenAILike (DeepSeek через NVIDIA) + YFinance + DuckDuckGo + Calculator
- `app.py`: Gradio UI, стриминг, таблица портфеля
- Зависимости: `agno`, `yfinance`, `duckduckgo-search`, `gradio`

### eagle_eye — SOUL.md
- Идентичность, тон, критерии ревью, workflow — всё в одном markdown
- Telegram-триггер, GitHub MCP, MiniMax M2.7
- Прямой аналог наших скиллов, но компактнее

### daily-news-digest — SKILL.md + skill.py
- SKILL.md: name, description, trigger (cron), metadata, pipeline diagram, env vars
- skill.py: fetch → score → top 3 → summarise → categorise → Telegram
- 92 фида, MiniMax M2.7, Telegram Markdown
