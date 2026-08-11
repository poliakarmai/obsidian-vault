---
title: "GSC S1 — Multi-tenant фундамент: блочная подача"
date: 2026-08-06
status: draft
as_of: 2026-08-06
tags: [gsc, saas, s1, multi-tenant, implementation]
parent: [[inbox/gsc-saas-strategy-2026-08-06]]
---

# GSC S1 — Multi-tenant фундамент (v0.27)

Граница этапа: переносим в облако пайплайн сканирования + изоляцию + metering.
Глубокие подсистемы (chains, mutations, overrides, invariants) → S2 вместе с GitHub App.

**Входное состояние:** v0.26, production, тесты 67/67, schema 23 (SQLite). Внутренний инстанс не трогаем.

## Блок 0/9. Состав S1 и принцип совместимости

```
Внутренний контур (не меняется):          GSC Cloud (S1, новое):
  gsc API v1 (порт 8766, sync)              cloud_api: /api/v2/* (async)
  gsc_db.py → SQLite                        PgBackend → PostgreSQL + RLS
  workflows v0.22–v0.26                     queue (Redis) → worker (CLI в subprocess)
```

Ядро сканера не меняется — worker вызывает его как subprocess.

## Блок 1/9. Docker-образ сканера

**Файл:** `~/gsc/Dockerfile`
- `python:3.11-slim`, non-root (user gsc)
- `GSC_DB_PATH=/tmp/gsc/worker.db` — эфемерный том
- Секреты только через runtime env
- Внутренние тесты в образе: `docker run image python3 tests/test_corpus.py`

## Блок 2/9. PgBackend: абстракция БД

**Файл:** `~/gsc/gsc_db_backend.py`
- `SqliteBackend` — внутренний контур (tenant_id=0)
- `PgBackend` — cloud, требует tenant_id, выставляет `SET app.tenant_id`
- Конвертер `?` → `%s` с учётом кавычек (не ломает литералы)

Патч `gsc_db.py`: `GSC_DB_PATH` из env.

## Блок 3/9. Multi-tenant схема PostgreSQL

**Файл:** `~/gsc/cloud/schema_s1.sql`
- `tenants`, `api_keys`, `repos`, `scans`, `findings`, `verdicts`, `usage`
- RLS-политики на findings/verdicts/scans (роль `gsc_app`, не superuser)
- Chains/mutations/overrides сознательно отсутствуют (S2)

## Блок 4/9. API-ключи и tenant middleware

**Файл:** `~/gsc/cloud/auth.py`
- `generate_api_key()` → `gsc_` + `token_urlsafe(32)`
- Хранится только sha256-хэш; raw показывается один раз
- `auth_tenant()`: lookup по префиксу + `hmac.compare_digest`

## Блок 5/9. Очередь и worker

**Файлы:** `~/gsc/cloud/queue.py`, `~/gsc/cloud/worker.py`
- Redis-очередь (`gsc:scans`), BRPOP
- Worker: `validate_target()` (только `https://github.com`) → subprocess с эфемерным HOME → инжест в PG → удаление временного каталога
- timeout=900 на subprocess; exit 0/1 = успех, 2 = error

## Блок 6/9. REST API v2 (async, multi-tenant)

**Файл:** `~/gsc/cloud/api.py`
- `/api/v2/scan` (POST) → 202 с scan_id
- `/api/v2/scans/{id}` (GET) → статус + findings
- `/api/v2/verdicts` (POST) → tp/fp/fixed
- Отдельное пространство `/api/v2` — v1 не трогаем
- 402 при превышении квоты до enqueue

## Блок 7/9. Metering и квоты

**Файл:** `~/gsc/cloud/store.py`
- `check_quota()`: сверка с `usage.scans` за месяц
- `meter()`: upsert в `usage` по факту скана
- Патч сканера: `report["usage"] = {"llm_calls": ..., "poc_generated": ..., "chains_composed": ...}`

## Блок 8/9. Тесты (+7 → 74/74)

| Тест | Что проверяет |
|---|---|
| `test_q_to_pg_placeholder_conversion` | Литерал `?` в кавычках не конвертируется |
| `test_pg_backend_requires_tenant` | PgBackend без tenant_id → ValueError |
| `test_api_key_hash_roundtrip` | Хэш + отозванный ключ |
| `test_target_validation_blocks_ssrf` | SSRF: http, IP, поддомен-трюк, file:// |
| `test_quota_returns_402` | 51-й скан free-плана → 402 |
| `test_cross_tenant_isolation` | RLS + фильтр (требует PG в CI) |
| `test_worker_treats_blocking_exit_as_success` | Exit 1 ≠ ошибка |

## Блок 9/9. Деплой MVP + чеклист

**Файл:** `~/gsc/cloud/docker-compose.yml`
- postgres:16-alpine + redis:7-alpine + api + 2 workers

### Гейт завершения S1

| Критерий | Цель |
|---|---|
| Тесты | 74/74 (включая PG-изоляцию) |
| Round-trip | scan → 202 → done → findings в PG |
| Изоляция | cross-tenant read = 404/пусто |
| Квота | 402 на 51-м скане free-плана |
| SSRF | все non-github target'ы отклонены |
| Внутренний production | 17/17 calibration, workflows без изменений |
| Секреты | 0 секретов в образе |

## Найденные баги S1

| # | Блок | Баг | Исправление |
|---|---|---|---|
| 1 | 2 | Наивный replace ?→%s ломал литералы | Конвертер с учётом кавычек + тест |
| 2 | 4 | API-ключи открытым текстом | Только sha256, raw разово |
| 3 | 4 | Timing-сигнал при проверке ключа | prefix lookup + hmac.compare_digest |
| 4 | 5 | SSRF: worker клонировал произвольный target | Allowlist только github.com |
| 5 | 5 | Exit 1 (blocking) = ошибка | 0/1 = успех, 2 = error |
| 6 | 6 | Async-перестройка v1 ломала контур | Отдельное /api/v2 |
| 7 | 9 | RLS молча не работает под superuser | Роль gsc_app + FORCE RLS |
