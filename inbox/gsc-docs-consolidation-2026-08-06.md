---
title: "GSC: консолидация документации в репо"
date: 2026-08-06
status: active
as_of: 2026-08-06
tags: [gsc, docs, consolidation, pr]
parent: [[inbox/gsc-critical-path-2026-08-06]]
---

# GSC: консолидация документации в репо

Три документа → PR → зелёный CI. Фиксируем базу для SaaS-трека.

## Структура после консолидации

```
gsc/
├── PROJECT.md              ← v1.0 (замена текущего)
├── GSC_APPLY_PLAN.md       ← 31 коммит v0.17→v0.26
├── GSC_SAAS_ROADMAP.md     ← стратегия S1–S4
├── docs/archive/
│   └── PROJECT_v0.16.md    ← архив старого
├── README.md, AGENTS.md, LICENSE
└── ... (код без изменений)
```

## Diff PROJECT.md v0.16 → v1.0

| Раздел | Было (v0.16) | Стало (v1.0) |
|---|---|---|
| Версии | 6 (v0.11–v0.16) | 16 (v0.11–v0.26) |
| Детекторов | 23 | 25 (+ GS025, GS028) |
| Уникальные фичи | 0 | 5 (PoC, AI-provenance, chains, mutations, invariants) |
| Calibration | 14/14 | 17/17 |
| Тесты | 8/8 | 67/67 |
| Rollout | plan Phase 0–5 | ✅ complete (blocking-standard) |
| Roadmap | warn-only | VSCode → Enterprise → SaaS |

## Коммит

```
docs: consolidate PROJECT.md v1.0 + apply plan + saas roadmap
```

## Чеклист

1. PROJECT.md → v1.0
2. Архив v0.16 → docs/archive/
3. GSC_APPLY_PLAN.md
4. GSC_SAAS_ROADMAP.md
5. Sanity: тесты 67/67, calibration 17/17, schema 23
6. git commit

## Мост к S1

После PR: код v0.26 production, доки зафиксированы, S1 спроектирован.
Старт S1 — вариант (a): Dockerfile + PgBackend (блоки 1–2 S1).
