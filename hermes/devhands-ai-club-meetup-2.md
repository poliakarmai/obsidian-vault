# Devhands AI Club — Митап №2: разбор для Hermes

**Источник:** https://habr.com/ru/articles/1053710/
**Дата:** 30 июня 2026
**Сообщество:** t.me/devhandsai

---

## 1. ACP как база для агентской автоматизации
**Алексей Самойлов, Techlead Fastronome**
📹 https://youtube.com/watch?v=HVrs3sIySac

### Эволюция: от IDE-плагина к протоколу
- Исторически агент был фичей внутри IDE (плагин) — человек пишет промпт → получает дифф
- Боль: каждый редактор должен отдельно интегрировать каждого нового агента
- Решение Zed (август 2025): агент = внешний процесс, IDE = клиент, ACP = протокол
- Октябрь 2025: JetBrains подхватывает ACP — registry агентов, MCP-форвардинг
- **Ключевая метаморфоза:** «любая программа может вертеть любым агентом»

### ACP ≠ A2A (важно!)
- **ACP** = Agent Client Protocol (client → agent)
- **MCP** = Model Context Protocol (agent → tools)  
- **A2A** = Agent-to-Agent (бывший Agent Communication Protocol)

### Жизненный цикл ACP-сессии
```
→ initialize (version + capabilities)
→ session/new (cwd + MCP servers)
→ session/prompt (долгий управляемый turn)
← session/update × N (plan/text/tool calls/diffs/usage/$$)
← result { stopReason }
```
**Важно:** `session/prompt` — это не «одно сообщение в чат», а долгий управляемый turn. Клиент видит события, approvals, tools, diffs и может **отменить выполнение**.

### Кто может быть клиентом
IDE, CI runner, чат-бот, workflow engine, control plane/harness, dump client

### Экосистема ACP
**Нативно:** OpenCode, Copilot, Cursor, Goose, **Hermes**, OpenClaw, Qwen Code, Kimi CLI, Mimo Code, Gemini CLI (помер)

**Через адаптеры:** Codex CLI, Claude Code, Pi, Antigravity CLI (coming soon)

### Оркестрация: Go-ADK + Norma Runtime
- **Go-ADK** (github.com/google/adk-go) — тяжеловес, платишь за токены
- **Решение Алексея:** ACPAgent-адаптер → любой ACP-агент становится агентом Go-ADK
- Использует **существующие подписки** (Codex, Gemini, ChatGPT) вместо оплаты токенов
- **Norma Runtime** (github.com/normahq/norma):
  - `norma pdca` — цикл Деминга (Plan-Do-Check-Act)
  - `norma goalkeeper` — аналог Reflexion loop
  - `norma planner` — декомпозиция задач (эпики → фичи → таски в Jira)
  - SequentialAgent, ParallelAgent — композиция агентов

### Пет-проекты → open source
| Проект | Суть |
|--------|------|
| **aida** | One-shot AI shell command runner |
| **codex-acp-bridge** | App-server → ACP мост |
| **relay** | Telegram Control Plane (аналог нашего Hermes!) |
| **balda** | Автономный worker: мессенджеры + шедулер + вебхуки + команда |
| **diffpal** | Open-source AI Code Review agent |

### Для Hermes
- ✅ Hermes уже в списке ACP-совместимых! Мы на передовой.
- 🔥 **Telegram Control Plane** — relay делает ровно то же что наш bridge. Мы конкуренты.
- 🔥 **ACPAgent-адаптер** — Pattern: оборачивать ACP-агентов в универсальный интерфейс. У нас delegate_task.
- 🔥 **Goalkeeper = Reflexion loop** — у нас cross-model-review, но не полноценный. Можно усилить.
- 📌 **ACPAgent + существующие подписки** — элегантный способ не платить за токены отдельно.
- 📌 **balda (автономный worker)** — аналог нашего cron + delegate. Интеграция с Teams интересна.

---

## 2. Системный дизайн через AI-скиллы и MCP
**Виталий Юшкевич, Lead engineer Pugofka**
📹 https://youtube.com/watch?v=RHfkGlp0f3c

### Проблема
- Задачу поняли неверно → хороший дизайн для неправильной задачи
- Наивный AI пропускает важное: класс задачи, ФТ/НФТ, сайзинг, скрытые допущения
- «ИИшка очень часто додумывает» — ловил много раз
- Система на 1K RPS vs 1M RPS — принципиально разная архитектура, AI это игнорирует

### Решение: Skill-flow с гейтами
Виталий сделал **публичный скилл** (доступен для тестирования). Архитектура:

```
Вход: описание задачи + контекст проекта
        ↓
  [REQUIREMENT GATE] ← режим брейншторминга
   • Вытаскивает ФТ, НФТ, числа
   • Ловит скрытые умолчания
   • Не даёт двигаться дальше без ответов
        ↓
  [RE-SIZING GATE]
   • Валидирует НФТ
   • Не тащить Kafka+ClickHouse для блога
        ↓
  [VERIFIER GATE]
   • Проверка требований
        ↓
  [DUAL-TRACK RESEARCH] — параллельно:
   Track A: Current Research (web, свежие источники)
   Track B: Internal Wiki (Karpathy-style LLM Wiki)
        ↓
  [MERGE + CONFLICT RESOLUTION]
   • Анализ совпадений/конфликтов
   • Авто-резолв, трейдофы где невозможно
        ↓
  [OUTPUT] C4 диаграммы, ADR, спецификации
```

### Ключевые фичи
- **Гейты** — не дают AI проскочить важные шаги
- **Karpathy Wiki** — внутренняя база знаний (книги, решения, трейдофы)
- **Dual-track** — веб-ресёрч + внутренние знания → мерж
- **Не заменяет спецификацию**, а делает граундинг (забрейнстормленная база)

### Результаты
- Менее опытные инженеры пускаются на сложное проектирование
- Количество упущенных требований **снизилось**
- Данных пока мало (внедрили недавно), но первые впечатления положительные

### Цитаты
- «AI без процесса может выдавать уверенную чушь, но ты не понимаешь»
- «Пропускаешь важные требования, потому что не хватает экспертизы»

### Для Hermes
- 🔥 **Гейты** — ровно то, что нам нужно для spec-driven-development! Сейчас у нас нет жёстких gate'ов.
- 🔥 **Dual-track research** — web + Obsidian vault. У нас Obsidian есть, можно добавить automatic web research.
- 🔥 **Karpathy Wiki** — аналог нашего Obsidian vault. Структура та же: перелинковка, знания, трейдофы.
- 🔥 **Re-sizing gate** — валидация НФТ. У нас нет этого в SDD. Критично для bybit-ws.
- 📌 Публичный скилл Виталия — можно изучить, адаптировать под Hermes.
- 📌 Не заменять spec, а делать граундинг — правильный подход.

---

## 3. AI в стартапе инфраструктурной платформы
**Георгий Меликов, founder Exordos (ex-VK Cloud)**

### Инструментарий
- Windsurf (ныне Devin) — топ IDE+агент, киллер-фича: автодополнение. НО ужасные квоты.
- VS Code + Cline/Continue.dev/KiloCode — для локальных моделей
- CLI (Claude/Codex/Qwen) — «стандарт де-факто»
- Локальные модели: Qwen 3.5-3.6, GLM 5.1+

### Железо
Consumer GPU (несколько) + AMD Ryzen AI Max+ PRO 395 + 128GB RAM (несколько)

### Ревью кода
- GitHub bots, долго на Gemini (депрекейтят)
- Слабое место — контекст (библиотеки, соседние зависимости)

### Тесты
- e2e > unit тесты
- CLI для всего — «ИИ его обожают»
- Документация = CLI help

### Бонус: AI не только для кода
Обзор рынка, экономика, юриспруденция, подбор названий.

### Для Hermes
- 🔥 **e2e > unit** — подтверждает наш подход. Стоит усилить e2e в Hermes.
- 🔥 **CLI как must-have** — у нас уже есть hermes CLI. Улучшать.
- 📌 Gemini deprecation — наш vision на Gemini тоже под вопросом.
- 📌 Контекст как слабое место — наша Obsidian-интеграция решает эту проблему.

---

## 4. Организация правил работы с проектами в Claude
**Денис Савицкий, dev lead DeltaSoft**

### Специфика
10 параллельных проектов, переключение контекста, большая кодовая база, чувствительные алгоритмы.

### Оптимизация токенов
- **caveman/ponytail** — ENG для CLI, экономия 25-50% токенов
- ENG vs RUS: https://habr.com/ru/companies/gptunnel/articles/986526/ (+50% к стоимости RUS)
- **CodeGraph** — индекс кода, быстрый поиск контекста задачи
- Prompt Rule: Task → Role → Context → Expectation

### Структура проекта
- `CLAUDE.md` — общий и проектные (аналог наших AGENTS.md)
- Отдельные сессии для работы
- `/init` — создаёт CLAUDE.md
- `/insights` — сводка сессии, проблемы, скелет навыков
- `/rename` + `--resume` — именованные сессии

### Скиллы
ansible-infra, codereview, git-split-commits, pr-description, rspec-test, server-triage, slack-deploy-notify, uptime-kuma

### Пайплайн сессии
1. `claude 'complete task and give'`
2. `/rename api-proxy-backend`
3. `claude --resume "api-proxy-backend"`
4. plan-mode для контроля и безопасности
5. `/init` → CLAUDE.md
6. `/insights` → анализ сессии

### Безопасность
- `/permissions` + `/allowed-tools`
- `~/.claude/settings.json` + `<project>/.claude/settings.json`

### Плагины
- **codegraph** — индекс + MCP
- **caveman** — экономия 50%+ токенов
- **security-guidance** — XSS, небезопасные паттерны
- **claude-remember** — память
- ❌ **Understand-Anything** — НЕ рекомендую (100k токенов, ничего полезного)

### Для Hermes
- 🔥 **CLAUDE.md = AGENTS.md** — у нас уже есть, но можно улучшить структуру
- 🔥 **/init + /insights** — аналог наших session-summarizer + obsidian-context
- 🔥 **caveman/ponytail** — стоит попробовать для экономии токенов в Hermes
- 📌 **CodeGraph** — индексация кода + MCP, можно интегрировать в Hermes
- 📌 **Именованные сессии** — у нас профили, но можно добавить sub-sessions
- 📌 **settings.json на проект** — у нас конфиги тенантов, но можно тоньше
- ⚠️ **Understand-Anything сливает токены** — подтверждает наш опыт

---

## 5. ИИ-агенты, прод и немного «извини»
**Ксения Погорельских, solo-фаундер Deploy-F**

Самый честный и полезный доклад — реальные факапы.

### Факап 1: Не вести память проекта
Агент постоянно забывает про Volume. Решение: ручная память из 10 строк ценнее всего, что нагенерит агент.

### Факап 2: Дать агенту сгенерировать память
«Сам во всём разберись, нагенери память, выстрой процесс по красоте» → агент стал тупить, генерировать мусор, думать что не готов.

### Факап 3: Не рассказать про бизнес и ЦА
Агент не знал позиционирование → UI стал перегружен ненужными подсказками. ЦА не хочет вникать, хочет чтобы работало.

### Факап 4: Большая задача без присмотра
В 3:51 ночи Opus: «а давай заодно сделаем кнопку пересборки?» Я: «но это же сложно». Opus: «да не, чё там, не ссы». Без комментариев.

### Факап 5: Надеяться на AI-ревью вёрстки
Opus 4.8: отлично. GPT-5.5: отлично. Fable 5.0: отлично. Вёрстка: кривая.

### Факап 6: Посадить 30 автономных агентов
10 тестовых стендов, доступы Codex, «пусть сами настроят». Задача: тестировать и багфиксить автономно. Результат: хаос.

### Выводы
- Доступы — только к песочнице
- 2 тестовых стенда для AI-тестировщиков
- Я остаюсь узким горлышком процесса
- **Значительно ускоряет, но НЕ делает полностью автономным**

### Для Hermes
- 🔥 **10 строк от себя > авто-память** — критично. Наш Obsidian-context правильный подход.
- 🔥 **30 агентов = хаос** — подтверждает: лимит делегатов (3 параллельно) оправдан.
- 🔥 **Sandbox-only** — наш skill-sandbox на Podman. Усиливать.
- 🔥 **Не доверять AI-ревью** — cross-model-review уже решает.
- 📌 Business-контекст для агентов — у нас user profile, но можно расширить.
- 📌 «Не ссы» от агента в 3:51 ночи — золото. safety-guard должен ловить такие порывы.

---

## 6. Пайплайн транскрибации 2000 часов лекций
**Максим Месилов, b24.io**

### Задача
Корпоративная LMS, 2000+ видеолекций на kinescope. Транскрипты, привязка фактов к кадрам, саммари, авто-тесты с открытыми вопросами.

### Типы саммаризации
Extractive, Abstractive, Hybrid. По длине, стилю, цели, источникам.

### Стек
Symfony + RoadRunner + Temporal + PostgreSQL

### AI-powered SDLC
- Спецификация → OpenSpec
- Написание кода 🥹
- Ревью результата
- Feedback loop для агента

### Скиллы: доменные, superpowers
MCP: gitlab, playwright, chrome, sentry

### Что сработало
- git-worktree
- make-файлы как entrypoint
- CLI-доступ к тулингу
- Сервисные операции через CLI
- Хуки агента для детерминизма
- Инфра как код
- На прод тоже можно пускать агента (коллеги спорят)

### Итоги
Сократили время доставки прототипа, дали больше функционала, поняли куда двигаться.

### Для Hermes
- 🔥 **Temporal для воркфлоу** — оркестрация пайплайнов. Мы используем cron + delegate, но Temporal надёжнее для сложных цепочек.
- 🔥 **Хуки агента для детерминизма** — у нас pre/post хуки в cron, можно расширить.
- 📌 **make-файлы как entrypoint** — у нас Makefile есть, но не везде.
- 📌 **OpenSpec для спецификаций** — аналог нашей spec-driven-development.
- 📌 **git-worktree** — для параллельной работы агентов над разными ветками.

---

## Что внедряем в Hermes

### 🔴 P0 — Сейчас
| # | Задача | Откуда | Статус |
|---|--------|--------|--------|
| 1 | Sandbox-only для делегатов (skill-sandbox обязателен) | Доклад 5 | ✅ |
| 2 | Запрет авто-памяти: только ручные 10 строк, не давать агенту генерить себе контекст | Доклад 5 | ✅ |
| 3 | Гейты в SDD: requirement gate → re-sizing → verifier (как у Виталия) | Доклад 2 | ✅ |
| 4 | Dual-track research: web search + Obsidian vault параллельно | Доклад 2 | ✅ |

### 🟡 P1 — На неделе
| # | Задача | Откуда | Статус |
|---|--------|--------|--------|
| 5 | Norma Runtime паттерн: pdca + goalkeeper + planner в Hermes | Доклад 1 | ✅ |
| 6 | e2e тесты для Hermes (не только unit) | Доклад 3 | ✅ |
| 7 | hermes CLI расширить (make everything CLI-accessible) | Доклад 3 | ✅ |
| 8 | ACPAgent-адаптер: универсальная обёртка для delegate_task | Доклад 1 | ✅ |

### 🟢 P2 — Когда время будет
| # | Задача | Откуда | Статус |
|---|--------|--------|--------|
| 9 | caveman/ponytail для English-сессий | Доклад 4 | ✅ |
| 10 | CodeGraph-подобная индексация через MCP | Доклад 4 | ✅ |
| 11 | Temporal для сложных пайплайнов | Доклад 6 | ✅ |
| 12 | git-worktree для параллельной работы агентов | Доклад 6 | ✅ |
| 13 | Business-контекст в профилях тенантов | Доклад 5 | ✅ |

### ⚪ P3 — Подумать
| # | Задача | Откуда | Статус |
|---|--------|--------|--------|
| 14 | Go-ADK интеграция | Доклад 1 | ⬜ defer |
| 15 | Karpathy Wiki для GSC | Доклад 2 | ✅ |

## Ссылки для изучения
- agentclientprotocol.com
- github.com/google/adk-go
- github.com/normahq/norma
- github.com/metalagman/aida
- github.com/normahq/relay — Telegram Control Plane
- github.com/colbymchenry/codegraph
- github.com/JuliusBrussee/caveman
- github.com/DietrichGebert/ponytail
- github.com/exordos — инфра-стартап
- t.me/devhandsai — сообщество
