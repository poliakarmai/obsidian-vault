---
title: "GSC S2 — GitHub App + порт глубоких подсистем в PG"
date: 2026-08-06
status: draft
as_of: 2026-08-06
tags: [gsc, saas, s2, github-app, mutations, chains]
parent: [[inbox/gsc-s1-implementation-2026-08-06]]
---

# GSC S2 — GitHub App + глубокие подсистемы (v0.29)

Вход: S1 применён. S2 = онбординг через GitHub App + перенос
chains/mutations/overrides в облако. 8 коммитов. Тесты 74→82.

## Границы S2

| Входит | Не входит (S3) |
|---|---|
| GitHub App: installation, webhooks, токены | Web Dashboard |
| Авторегистрация репо и тенантов (PLG) | Stripe/биллинг |
| PR-скан по webhook | Метрики для продаж |
| /gsc-команды в облачных PR | SSO |
| Порт chains/mutations/overrides/published_comments в PG | |

## Блок 1/8. Схема S2

Новые таблицы: github_installs, chains, mutation_alerts, overrides,
published_comments, publication_events. ALTER для findings, repos, scans.
RLS + FORCE на все тенант-таблицы.

## Блок 2/8. Рефакторинг ядра: MutationMatcher

Чистый матчер без БД. Используется и SQLite-трекером, и cloud-инжестом.
Единственный коммит, трогающий production-код сканера.

## Блок 3/8. GitHub App auth

JWT (iat-60, exp+540) → installation token (кэш с margin 120s).
Приватный ключ только из env.

## Блок 4/8. Webhook-приёмник

Подпись по СЫРОМУ телу, dedup через Redis SETNX (X-GitHub-Delivery, TTL 24ч).
Порядок: подпись → dedup → бизнес-логика.

## Блок 5/8. Онбординг + scan jobs

PLG: установка App → авто-создание free-тенанта. synchronize → supersede
устаревших queued-сканов. is_fork из head/base full_name.

## Блок 6/8. GitHub worker + history ingest

Токен в $HOME/.netrc (не argv). Fork-safe: --no-llm. Мутации через
MutationMatcher против PG-истории (не эфемерный SQLite).

## Блок 7/8. /gsc-команды

Общий парсер gsc_pr_commands.py. Авторизация через author_association.
Override без причины → молча пропущен.

## Блок 8/8. Тесты S2 (+8 → 82/82)

| Тест | Что проверяет |
|---|---|
| test_webhook_signature | 4 ветки подписи |
| test_delivery_dedup | replay отбит |
| test_jwt_timing_bounds | iat/exp границы, RSA |
| test_installation_token_refresh_margin | кэш с запасом |
| test_install_auto_creates_tenant | PLG идемпотентно |
| test_fork_pr_job_flagged | is_fork = True |
| test_supersede_stale_queued_scans | synchronize dedup |
| test_gsc_command_tenant_scoped | вердикт tenant-scoped |

## Найденные баги S2 (9 шт.)

1. JWT с iat=now → iat = now - 60
2. Кэш без запаса → refresh margin 120s
3. Подпись по parsed JSON → сырое тело
4. Replay вебхуков → SETNX delivery
5. Установки без тенанта → авто free-тенант
6. synchronize плодил очередь → superseded
7. Токен в argv → $HOME/.netrc chmod 600
8. Эфемерный SQLite → MutationMatcher в PG
9. Импорт Actions-скрипта → общий парсер

## Чеклист и гейт

- 82/82 тестов
- 17/17 calibration после рефакторинга Блока 2
- Round-trip: install App → tenant → PR-скан → комментарий
- Fork PR: regex-only, без LLM/мутаций
- Подпись/dedup: отклонены
- Токены: netrc, не argv; кэш с margin
- /gsc: вердикт + override tenant-scoped
