# AgentsView — аналитика AI-кодинг-агентов

**Источник:** https://ai-uchi.ru/news/agentsview-analitika-kodiruyushchikh-agentov/
**Дата:** 2026-06-13

---

## Главная идея

Локальный open source бинарник для трекинга 20+ coding-агентов (Claude Code, Codex, Qwen Code, WorkBuddy и др.). Замена `ccusage` с ускорением ×100 за счёт SQLite-индексации вместо многократного парсинга JSONL.

## Ключевые фичи

- **Расходы** — сводка по токенам/деньгам с фильтрами по агенту/дате/модели
- **Сессии** — архетипы (quick/deep/marathon), пиковый контекст, инструменты на ход
- **Git-метрики** — коммиты, строки кода на доллар токенов
- **Веб-интерфейс** на `127.0.0.1:8080` + CLI
- **Local-first** — без облака, без регистрации

## Установка

```bash
curl -fsSL https://agentsview.io/install.sh | bash
agentsview serve  # http://127.0.0.1:8080
```

## Авторы

- **Kenn Software** (roborev, msgvault)
- **Уэс МакКинни** — создатель pandas, Ibis, сооснователь Apache Arrow
- 1100+ звёзд на GitHub

## Применимость к Hermes

| Концепция | У них | У нас |
|-----------|-------|-------|
| Аналитика агентов | SQLite-индексация сессий | delegate_task логи |
| Поддержка агентов | Claude Code, Codex, 20+ | Claude Code, Codex через delegate_task |
| Веб-интерфейс | Да | Дашборд Hermes |

**Вердикт:** пока не ставим, но держим в уме для будущей аналитики расходов на агентов.
