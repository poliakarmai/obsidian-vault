---
title: "GSC → SaaS: стратегия и архитектура перехода"
date: 2026-08-06
status: draft
as_of: 2026-08-06
tags: [gsc, saas, architecture, strategy]
---

# GSC → SaaS: стратегия и архитектура перехода

Проект уже на ~70% готов к SaaS-ификации. Ядро проектировалось правильно.

## 1. Аудит: что уже есть и почему это SaaS-активы

| Актив (сейчас) | Ценность для SaaS |
|---|---|
| Сканер = stateless CLI с JSON/SARIF выходом | Готовый container worker: образ запускается, сканирует, умирает. Ничего не переписывать |
| REST API v0.16 (/api/v1/scan, x-api-key) | Зародыш control plane — уже есть контракт |
| finding_key + feedback loop | Готовая модель per-tenant обучения — каждый клиент делает сканер тише для себя |
| Profiles (LLM 10/20/50) | Готовая основа тарифных лимитов |
| Self-learning + авто-деактивация | Главный moat: «сканер, который учится на ваших вердиктах» — этого нет у Snyk/Semgrep как сервис |
| SARIF + GitHub Adapter | Экосистема интеграций из коробки |
| Хранятся findings/snippets, а не код | Privacy-преимущество: «мы не храним ваш код» |
| 400K находок в SQLite | Доказательство масштаба модели данных |

Вывод: переписывать нечего. Нужно добавить multi-tenant обвязку вокруг существующего ядра.

## 2. Позиционирование и рынок

**ICP:** команды 5–50 разработчиков без AppSec-инженера.

| Конкурент | Их слабость | Наш ответ |
|---|---|---|
| Semgrep Cloud | Статичные правила, шум | Self-learning: правила отключаются по вердиктам клиента |
| Snyk | Дорого, фокус на зависимостях | Дешевле + SAST + PoC-доказательства |
| GitHub Advanced Security | $49/committer, только CodeQL-паттерны | Attack chains + PoC + AI-code scanner |
| CodeQL | Сложно настроить | 0 конфигурации: GitHub App → 2 клика |

**Уникальное предложение:**
> «Сканер, который доказывает уязвимости эксплойтами и учится на ваших ответах — через месяц он молчит там, где другие кричат».

**Сетевой эффект:** глобальный кэш ревалидации по fingerprint'ам — находка, подтверждённая как FP у одного клиента, гасится у всех.

## 3. Целевая архитектура (GSC Cloud)

```
Разработчик ─────────┐
Sec-инженер ─────────┤
                     ▼
       ┌─────────────────────────────┐
       │  Web Dashboard (Next.js)    │
       │  находки, цепочки, PoC,     │
       │  политики, биллинг          │
       └──────────────┬──────────────┘
                      │ OIDC / API key
       ┌──────────────▼──────────────┐
       │  Control Plane (FastAPI)    │◄──── GitHub App
       │  v0.16 API → multi-tenant:  │      (webhooks, checks,
       │  authn/z, квоты, metering   │       installation)
       └──────────────┬──────────────┘
                      │ enqueue
       ┌──────────────▼──────────────┐
       │  Queue (Redis / SQS)        │
       └──────────────┬──────────────┘
       ┌──────────────┼──────────────┐
       ▼              ▼              ▼
┌─────────────┐ ┌─────────────┐ ┌──────────────────┐
│ Scan Worker │ │ Scan Worker │ │ LLM Gateway      │
│ (Docker,    │ │  ...        │ │ бюджет/тенант,   │
│ эфемерный)  │ │             │ │ глоб. кэш по fp  │
└──────┬──────┘ └─────────────┘ └──────────────────┘
       │ findings JSON/SARIF (код НЕ сохраняется)
┌──────▼────────────────────────────────────────────┐
│ PostgreSQL: tenants | repos | scans | findings |  │
│ verdicts | policies | usage   (tenant_id + RLS)   │
└───────────────────────────────────────────────────┘
```

**Принципы:**
1. Worker эфемерный: клонирует → сканирует → том удаляется
2. LLM Gateway: единый бюджет + глобальный кэш. Экономия 40–60%
3. GitHub App вместо PAT

## 4. Модель данных (multi-tenant)

```
tenants      (id, name, plan, stripe_customer_id, llm_budget_month, created_at)
memberships  (tenant_id, user_id, role)              -- owner|security|developer
github_installs (tenant_id, installation_id, org)
repos        (id, tenant_id, gh_repo_id, name, policy_json)
scans        (id, tenant_id, repo_id, profile, mode, status, ...)
findings     (tenant_id, scan_id, finding_key, rule_id, severity, confidence, ...)
verdicts     (tenant_id, finding_key, actor, verdict, reason, source)
chains       (tenant_id, chain_key, finding_keys, severity, confidence)
overrides    (tenant_id, repo_id, pr_number, finding_key, actor, reason)
usage        (tenant_id, period, scans, llm_calls, poc_generated)
```

PostgreSQL с row-level isolation (tenant_id + RLS).

## 5. Поэтапный план S1–S4

| Этап | Содержание | Оценка | Версии |
|---|---|---|---|
| **S1. Фундамент** | Docker-образ сканера; PgBackend; tenants/repos/scans; API key; очередь + 1 worker | 3–4 нед | v0.27–v0.28 |
| **S2. Onboarding** | GitHub App (install, webhooks, checks); автозапуск на PR; /gsc-команды | 3 нед | v0.29 |
| **S3. Продукт** | Web Dashboard; Stripe + metering; тарифные лимиты | 4–5 нед | v0.30 |
| **S4. Доверие и рост** | SOC 2 Type I; DPA; audit log; SSO; GitHub Marketplace; VSCode extension | 6–8 нед | Cloud 1.0 |

**Параллельно:** VSCode extension по готовому плану.

## 6. Тарифы

| План | Цена | Лимиты | Фичи |
|---|---|---|---|
| **Free** | $0 | 3 репо, 50 сканов/мес | regex-детекторы, SARIF, 1 пользователь |
| **Team** | $29/польз/мес | 20 репо, 500 сканов | + LLM, PoC, цепочки, PR-комментарии |
| **Business** | $49/польз/мес | безлимит репо | + инварианты, мутации, SSO, audit log |
| **Enterprise** | custom | — | + hybrid-агент, SLA, SOC 2 report |

## 7. Безопасность и compliance

1. «Мы не храним ваш код» — findings/snippets только
2. Изоляция: tenant_id + PostgreSQL RLS
3. Redaction audit v0.15 на всех выходах
4. SOC 2 Type I на этапе S4
5. Hybrid-режим для Enterprise

## 8. Первые шаги — этот месяц

- [ ] Dockerfile сканера: gsc external-scan → report.json
- [ ] 12-factor аудит: конфиг из env, секреты вне кода, structured logs
- [ ] gsc_db.py: интерфейс DbBackend + PgBackend, миграция schema 23 → PG
- [ ] Таблицы tenants/repos/scans + API key middleware
- [ ] Очередь: Redis + один worker
- [ ] Лендинг + waitlist + домен (gsc.dev / gscsec.io)
- [ ] Черновик GitHub App (manifest + webhook-заглушка)

## 9. Риски и митигация

| Риск | Митигация |
|---|---|
| LLM-расходы при росте | Кэш по fingerprint, квоты, regex-first |
| Доверие к облаку (код!) | Не храним код + SOC 2 + hybrid |
| Semgrep/Snyk задавят | Ниша self-learning + PoC, PLG free-tier |
| Расползание скоупа | S1–S2 без дашборда, дашборд только в S3 |
| Multi-tenant утечка | RLS + интеграционные тесты в calibration-стиле |

**Итог:** GSC → SaaS не перезапуском, а наращиванием обвязки вокруг ядра. Уникальность полностью переносится и усиливается сетевым эффектом глобального кэша вердиктов.
