---
title: "GSC: карта состояния и критический путь"
date: 2026-08-06
status: active
as_of: 2026-08-06
tags: [gsc, roadmap, planning]
parent: [[inbox/gsc-saas-strategy-2026-08-06]]
---

# GSC: карта состояния и критический путь

## Где мы сейчас

| Трек | Состояние | Что осталось |
|---|---|---|
| Ядро v0.11→v0.26 | ✅ production | ничего |
| Rollout Phase 0–5 | ✅ blocking-standard | наблюдение за первыми 2 неделями живых блокировок |
| Документация | ✅ написана | не зафиксирована в репозитории |
| SaaS-стратегия | ✅ расписана | S1 написан поблочно, но не применён |
| VSCode extension | ✅ план C1–C6 | scaffold кодом не собран |

Главный риск — не технический, а расползание: планов больше, чем рук.

## Критический путь (зависимости)

```
Консолидация доков в репо (½ дня, ни от чего не зависит)
        │
        ▼
Неделя наблюдения Phase 5 ──► S1: multi-tenant фундамент
(блок. FP-rate, overrides)      (блоки готовы — только применить)
                                    │
                                    ▼
                              S2: GitHub App + порт chains/mutations в PG
                                    │
                       ┌────────────┴────────────┐
                       ▼                         ▼
                 S3: Dashboard + Stripe    VSCode extension
                                           (цеплять уже к cloud API)
```

VSCode осознанно после S2: расширению нужен аккаунт и облачный API.

## Три горизонта

### Эта неделя (операционка + фиксация)
1. PR консолидации: PROJECT.md v1.0 + GSC_APPLY_PLAN.md + GSC_SAAS_ROADMAP.md в репозиторий
2. Наблюдение Phase 5: `gsc metrics --rollout` ежедневно, разбор override/bypass, FP-rate блокировок. Если FP-rate > 15% — тюнинг до S1.

### Этот месяц (стройка)
3. Применение S1 по готовым блокам: Dockerfile → PgBackend → схема → queue/worker → round-trip /api/v2

### Этот квартал (продукт)
4. S2 (GitHub App) → S3 (dashboard + биллинг) → публичная бета GSC Cloud
