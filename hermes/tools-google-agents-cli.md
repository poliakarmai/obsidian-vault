# Google Agents CLI

**Установлен:** 30.06.2026  
**Версия:** 0.6.1  
**Команда:** `uvx google-agents-cli setup`  
**Источник:** [github.com/google/agents-cli](https://github.com/google/agents-cli)

## Что это

CLI + 7 skills для coding agent'ов — полный цикл разработки ADK-агентов на Google Cloud.

## Установленные skills (`~/.agents/skills/`)

| Skill | Назначение |
|-------|-----------|
| `google-agents-cli-workflow` | Жизненный цикл: идея → код → деплой |
| `google-agents-cli-adk-code` | ADK Python API: агенты, tools, orchestration |
| `google-agents-cli-scaffold` | `create / enhance / upgrade` проектов |
| `google-agents-cli-eval` | Датасеты, метрики, прогоны |
| `google-agents-cli-deploy` | Agent Runtime, Cloud Run, GKE |
| `google-agents-cli-publish` | Регистрация в Gemini Enterprise |
| `google-agents-cli-observability` | Cloud Trace, логи |

## Команды CLI

```bash
agents-cli create <name> --adk    # Создать проект из шаблона
agents-cli install                 # Установить зависимости
agents-cli playground              # Локальный dev-сервер
agents-cli eval generate           # Сгенерировать eval-прогоны
agents-cli eval grade              # Оценить результаты
agents-cli scaffold enhance        # Добавить CI/CD
agents-cli deploy                  # Деплой
agents-cli login                   # Аутентификация GCP
```

## Ограничения

- **Нет GCP-креда** — `playground`, `deploy`, `publish` требуют `gcloud auth login`
- Scaffold + install работают локально без креда
- Eval'ы не тестировались (нужен работающий агент)

## Тестовый проект

`/tmp/test-rag-agent/test-rag-agent/` — создан через `agents-cli create --adk`, зависимости установлены.

## Статья-источник

[Agentic Engineering с нормальными инструментами](https://telegra.ph/Agentic-Engineering-s-normalnymi-instrumentami-Google-Agents-CLI-na-praktike-06-29) — Влад Смирнов
