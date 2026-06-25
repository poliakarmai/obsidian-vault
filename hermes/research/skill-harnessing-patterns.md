# Skill Harnessing — Architectural Patterns for Agent Skills

**Источник:** arXiv, 23.06.2026

## Суть

Метод skill harnessing: 10 архитектурных паттернов + 4-слойная эталонная архитектура для превращения статических навыков LLM-агентов в контролируемые, воспроизводимые действия в рантайме.

## 4 слоя ответственности

1. **Supply Chain** — откуда берутся скиллы (создание, импорт, каталог)
2. **Mediation** — выбор и адаптация скилла под контекст
3. **Execution Control** — безопасное исполнение с проверками
4. **Evidence & Feedback** — аудит-трейл, улики, обратная связь

## Соответствие Hermes

| Слой | Hermes-реализация |
|------|-------------------|
| Supply Chain | `skill-sync`, `user-skills`, 4-stage review (validate→security→judge→adversarial) |
| Mediation | `using-hermes-skills` (progressive disclosure router), `tenant_prefix` |
| Execution Control | `disabled_toolsets`, `safety-guard`, `invariant-check`, skill sandbox |
| Evidence & Feedback | `audit-trail`, `tenant-audit`, `session_search`, `vault-vs-reality-check` |

## Ключевое

Наш 4-stage review pipeline (validate→security→judge→adversarial) — это реализация их Supply Chain + Execution Control. Не хватает формализации Evidence & Feedback как отдельного слоя.

## Тэги

#ии #исследование #llmagents #architecturalpatterns #skill-harnessing
