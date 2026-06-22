---
tags: [ai-agent, yagni, minimal-code, claude-code, codex, plugin, benchmarking]
created: 2026-06-15
---

# Ponytail — заставь AI-агента писать минимальный код

**Автор:** [DietrichGebert](https://github.com/DietrichGebert)
**Репозиторий:** https://github.com/DietrichGebert/ponytail
**⭐ 9.1k** звёзд, 387 форков, MIT, v4.4.0 (15.06.2026)
**Слоган:** *He says nothing. He writes one line. It works.*

---

## Главная идея

Ponytail — это skill для AI-агентов, заставляющий их думать как самый ленивый сеньор-разработчик: «лучший код — тот, который ты не написал».

**Результаты бенчмарков:** 80-94% меньше кода, 3-6× быстрее, 47-77% дешевле.

## Как работает: 6-ступенчатая лестница

Перед тем как писать код, агент проверяет каждую ступень:

1. Это вообще нужно? → нет: пропустить (YAGNI)
2. Есть в stdlib? → использовать
3. Нативная фича платформы? → использовать
4. Уже установленная зависимость? → использовать
5. Одна строка? → одна строка
6. **Только тогда:** минимально рабочий код

Безопасность, валидация, доступность — не режутся.

## Поддержка платформ

| Платформа | Способ установки |
|---|---|
| **Claude Code** | `/plugin marketplace add DietrichGebert/ponytail` |
| **Codex** | `codex plugin marketplace add DietrichGebert/ponytail codex` |
| **OpenCode** | Плагин `.opencode/plugins/ponytail.mjs` |
| **Gemini CLI** | `gemini extensions install https://github.com/DietrichGebert/ponytail` |
| Cursor/Windsurf/Cline/Copilot | Копировать `.cursor/rules/`, `.windsurf/rules/` и т.д. |
| **Kiro** | Скопировать `.kiro/steering/ponytail.md` |
| **Pi agent harness** | `pi install git:github.com/DietrichGebert/ponytail` |

## Команды

| Команда | Назначение |
|---|---|
| `/ponytail [lite\|full\|ultra\|off]` | Уровень интенсивности |
| `/ponytail-review` | Ревью диффа на переинженеринг |
| `/ponytail-audit` | Аудит всего репозитория |
| `/ponytail-debt` | Собрать отложенные «ponytail:» комментарии в ledger |

## Применимость к Hermes

| Концепция | У них | У нас |
|---|---|---|
| YAGNI-фильтр | 6-ступенчатая лестница | Скилл `ponytail` уже установлен |
| Бенчмарки | promptfoo eval, 10 прогонов | Можно адаптировать для оценки качества |
| ponytail-review | Проверка диффа | Прямо в пайплайнコード-ревью |
| ponytail-debt | Отложенные улучшения | Может помочь с tracking технического долга |
| Мульти-агент | Claude Code, Codex, Gemini, OpenCode | У нас Hermes — нужна адаптация под AGENTS.md |

## Оценка

- **Практическая ценность:** очень высокая — напрямую экономит токены и время
- **Уже используем:** скилл `ponytail` в Hermes — надо сверить с актуальной версией репозитория
- **Что можно украсть:** команды review/audit/debt — отличный апгрейд для нашего скилла

---

**Связанные заметки:** [[Оркестрация-Hermes]]
