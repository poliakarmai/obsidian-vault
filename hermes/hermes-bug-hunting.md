---
title: "Проект БАГИ — охота за багами в Hermes Agent"
created: 2026-06-26
tags: [hermes, bugs, contributions, open-source]
status: active
---

# Проект «БАГИ» — контрибьюции в Hermes Agent

## Идея

Вместо сдачи формальных сертификатов — находим и чиним реальные баги в [Hermes Agent](https://github.com/NousResearch/hermes-agent). Каждый принятый PR = строка в списке контрибьюторов топового AI-проекта (13K+ звёзд).

**Почему это круче сертификатов:**
- Публичный и верифицируемый вклад на GitHub
- Реальный код в реальном проекте
- Вес в сообществе AI-разработки
- Строчка в резюме: «Contributor to Hermes Agent (Nous Research)»

## Процесс

1. Мониторим [issues](https://github.com/NousResearch/hermes-agent/issues) — ищем `bug` + `good first issue`
2. Воспроизводим баг локально
3. Пишем фикс
4. Гоняем тесты
5. Открываем PR через GitHub CLI

## Найденные и починенные баги

| # | Issue | Описание | PR | Статус |
|---|-------|----------|-----|--------|
| 1 | [#52823](https://github.com/NousResearch/hermes-agent/issues/52823) | macOS: нелокальные бэкенды ломают пути через симлинк `/home` → `/System/Volumes/Data/home` | `fix/non-local-path-resolution` | 🟡 коммит готов, ждём API rate limit |

## Бэклог

- [ ] Добить PR #52823 (форк + пуш)
- [ ] Issue [#52694](https://github.com/NousResearch/hermes-agent/issues/52694) — Background process notifications misinterpreted as user messages
- [ ] Issue [#52492](https://github.com/NousResearch/hermes-agent/issues/52492) — 400 'gpt-5.3-codex' model not supported
- [ ] Мониторить новые issues с label `bug`

## Инструменты

- GitHub CLI: `gh` (настроен, токен активен)
- Форк: `poliakarmai/hermes-agent` (нужно создать когда API отлимитится)
- Локальный клон: `/tmp/hermes-agent-pr`
- Патч первого фикса: `/tmp/certs/fix-52823.patch`

## Команда для PR

```bash
cd /tmp/hermes-agent-pr
gh repo fork --remote-name origin-fork
git push origin-fork fix/non-local-path-resolution
gh pr create --repo NousResearch/hermes-agent \
  --title "fix: skip symlink resolution for non-local terminal backends" \
  --body-file /tmp/certs/pr-body-52823.md
```
