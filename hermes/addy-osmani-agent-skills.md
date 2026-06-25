---
tags: [agent-skills, claude-code, cursor, workflow, engineering]
created: 2026-06-23
source: https://github.com/addyosmani/agent-skills
author: Addy Osmani
stars: 65733
---

# Addy Osmani: Agent Skills

Production-grade engineering skills for AI coding agents. 65K+ ⭐.

## Пайплайн

```
  DEFINE          PLAN           BUILD          VERIFY         REVIEW          SHIP
 ┌──────┐      ┌──────┐      ┌──────┐      ┌──────┐      ┌──────┐      ┌──────┐
 │ Idea │ ───▶ │ Spec │ ───▶ │ Code │ ───▶ │ Test │ ───▶ │  QA  │ ───▶ │  Go  │
 │Refine│      │  PRD │      │ Impl │      │Debug │      │ Gate │      │ Live │
 └──────┘      └──────┘      └──────┘      └──────┘      └──────┘      └──────┘
  /spec          /plan          /build        /test         /review       /ship
```

## 23 скилла

### Фаза DEFINE
- `interview-me` — интервью пользователя
- `idea-refine` — дивергентное/конвергентное мышление

### Фаза PLAN
- `spec-driven-development` — PRD перед кодом
- `planning-and-task-breakdown` — атомарные задачи

### Фаза BUILD
- `incremental-implementation` — по кускам
- `source-driven-development` — документированный код
- `api-and-interface-design`
- `frontend-ui-engineering`
- `context-engineering` — управление контекстом
- `doubt-driven-development` — адверсариальная проверка решений

### Фаза VERIFY
- `test-driven-development` — RED-GREEN-REFACTOR
- `browser-testing-with-devtools`
- `debugging-and-error-recovery`

### Фаза REVIEW
- `code-review-and-quality`
- `code-simplification` — ясность > хитрость
- `security-and-hardening` — OWASP Top 10
- `performance-optimization`

### Фаза SHIP
- `shipping-and-launch`
- `ci-cd-and-automation`
- `git-workflow-and-versioning`
- `deprecation-and-migration`
- `documentation-and-adrs`
- `observability-and-instrumentation`

### Мета
- `using-agent-skills` — роутер скиллов

## Сравнение с Hermes

| Скилл | У Addy | У нас | Статус |
|-------|--------|-------|--------|
| spec-driven-development | ✅ | ✅ | Есть |
| test-driven-development | ✅ | ✅ | Есть |
| source-driven-development | ✅ | ✅ | Есть |
| code-review | ✅ | ✅ | requesting-code-review |
| security-and-hardening | ✅ | ✅ | Есть |
| code-simplification | ✅ | ✅ | simplify-code |
| planning | ✅ | ✅ | plan |
| context-engineering | ✅ | ✅ | stay-within-limits |
| idea-refine | ✅ | ❌ | **Интересно** |
| doubt-driven-development | ✅ | 🟡 | adversarial-review (слабее) |
| interview-me | ✅ | 🟡 | clarify (проще) |
| using-agent-skills | ✅ | ✅ | using-hermes-skills |

## Что можно забрать

1. **doubt-driven-development** — свежий контекст, bias to disprove. Мощнее нашего adversarial-review
2. **idea-refine** — структурированный brainstorming: дивергентно → кластеризация → one-pager
3. **incremental-implementation** — one slice at a time, каждый коммит атомарный
