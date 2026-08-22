---
status: active
as_of: 2026-08-21
---

# GSC Status 2026-08-21 — precision-hunt + 100-проектный benchmark

## Итог сессии (3 коммита, всё запушено)

| Коммит | Что |
|---|---|
| `3059552` | Фикс фейкового CVE — NVD-коллектор (`gsc_collect_light.py`) больше не генерит генерик-регексы из CVE-описаний, CVE → inactive refs (`active=0`, `cve-reference`). 25 CVE-паттернов деактивированы в БД. |
| `43af63a` | Benchmark 100 проектов — отчёты + скрипты + `benchmark/PRECISION_REPORT_100.md` + `.gitignore` (2.8 GB клонов не в git). |
| `ba4c2d0` | Фикс GS008 — голевой `\beval\(` seed закомментирован в `main.py:1575` + деактивированы `TS: eval() usage` и `eval() or exec() usage` в БД. |

## Benchmark: 100 реальных проектов (0.14.2 ✅)

- **64 831 находок**: 4 302 CRITICAL, 37 246 HIGH.
- **Recall 8/10** (пропущены: `aiohttp-security`, `cyberbro`).
- Чистых проектов: 42 без CRIT, 48 с CRIT (FP-шум).
- Артефакты: `benchmark/precision_report_ALL_100.json`, `precision_report_batch1..10.json`, `projects_100_ordered.json` (порядок от мелких к крупным).

## Precision-hunt (0.12.2 ✅, 0.12.3 ⏳)

**Топ FP-генераторы (до фикса):**

| Rule | CRIT | Статус |
|---|---|---|
| GS008 (голевой eval) | 2 508 (58%) | ✅ починен → **0** (next.js 2810→441 CRIT) |
| GS001 (creds/PAN) | 613 | не тронут |
| GS000-LEGACY | 505 + 26 678 HIGH | ⏳ **СЛЕДУЮЩИЙ** |
| GS005 (SQLi) | 211 | не тронут |

**Эффект GS008-фикса:** CRIT 4 302 → ~1 794 (−58%). Recall без регрессий (542 теста зелёные).

**Уроки (в скиллах):**
1. Голевой regex-паттерн на sink (`\beval\(`) = массовый FP. Refine до «sink + taint/контекст».
2. CVE-описание ≠ генерик-детектор. CVE — inactive reference, не код-паттерн.
3. Вторичный шум: `GS025-eval_usage` + `YAML-36ACF0AD` всё ещё флагают голый eval как HIGH (включая литеральный `eval("2+2")`) — рассмотреть при чистке HIGH-шума.

## Следующий шаг: GS000-LEGACY (0.12.3 data-quality)

505 CRIT + 26 678 HIGH находок без нормального `rule_id` → legacy-бакет. Гипотеза: пустые/заголовочные rule_id из legacy-паттернов (`check_source_driven`/`check_security` в `main.py`) и `_derive_rule_id` (маппит title-ключи → GS0XX; «command» не покрыт → GS000-LEGACY).

**Точки входа:**
- `gsc_cli/main.py`: `_derive_rule_id` (~477), `check_source_driven` (~599), `check_security` (~638), `load_patterns` (~1195).
- `gsc_core/gsc_blocking.py:43` — вес GS000-LEGACY.

После GS000-LEGACY → полный перегон benchmark → свежие precision-цифры.

## Как возобновить

```bash
cd ~/gsc
python3 -m pytest -q                              # 542 passed, 5 skipped
python3 scripts/gsc_benchmark_batch.py N          # перескан батча N (resumable)
python3 scripts/gsc_benchmark_all.py              # прогон батчей
python3 gsc.py scan <repo> --ci --json            # одиночный скан
python3 scripts/gsc_reconcile.py                  # сверка SSOT-чисел
```

Benchmark-сканер `scripts/gsc_benchmark_batch.py` — resumable (инкрементальное сохранение, resume по name). Таймаут 1800s/проект (крупные репо с тысячами находок медленные — ruff 404s, next.js 1243s).
