---
created: 2026-06-29
severity: CRITICAL
incident: gateway-indentationerror-20260629
---

# Защита hermes-agent репо

## Инцидент

29.06.2026 — gateway не стартовал 56 минут (09:22–10:18):
1. Агент сделал `git checkout main` + `git reset HEAD` в `~/.hermes/hermes-agent/`
2. Файл `gateway/run.py:15367` получил `IndentationError: unexpected indent`
3. Gateway попал в crash loop (systemd Restart=on-failure)
4. Починилось только когда `git pull --ff-only origin main` притянул свежую версию

## Правило

**НИКОГДА не делать git-операции в `~/.hermes/hermes-agent/` без явной команды пользователя.**

Это работающий код gateway. Любое изменение — риск обвала.

## Защита

- Скилл `safety-guard` содержит секцию «Hermes Agent Repo — НЕ ТРОГАТЬ»
- `patch`/`write_file` на файлы hermes-agent требуют явного подтверждения
- `git checkout`/`git reset`/`git pull` в этом репо — только по команде
