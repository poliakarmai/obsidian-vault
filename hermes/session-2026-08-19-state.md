---
status: active
as_of: 2026-08-19
---

# Состояние сессии 2026-08-19 (GSC precision-pass + фикс CI)

## Контекст

Репозиторий: `~/gsc`, ветка `master`. Два трека закрыты в этой сессии:
1. **Precision-pass детекторов** (GS020 XSS, GS021 CSRF/SSRF) по анти-галлюцинационным
   брифам, с ответами внешнего агента в строгом формате §7.
2. **Фикс битого пути gsc.py после packages split 0.5.2** (CI Calibration был красным 3 дня).

## Итог precision (главный прогресс)

- **Clean FP: 539 → 148** (общий по calibration-проектам).
- **recall сохранён:** `xss 2/2`, `sql_injection 2/3`, `command_injection 1/1`
  (дыры `hardcoded_secret 0/1`, `idor 0/1` — известные, не регрессия).
- Закрытые детекторы: GS000-LEGACY, GS020, GS021.
- **Очередь шума (дальше по убыванию):** GS037 path traversal (21) → GS003/GS022 (14/14).

## Запушенные коммиты сессии

| SHA | Что |
|---|---|
| `a520c2b` | fp_log (schema v33) + metrics dashboard |
| `df93085` | бриф GS021 (self-contained EN, anti-hallucination) |
| `9b382a4` | бриф GS020 (self-contained EN, anti-hallucination) |
| `849cfb8` | GS020 precision-pass (31→7 FP, recall 2/2) |
| `3d3597e` | GS021 precision-pass (39→0 FP, TP сохранён) |
| `1d4f3aa` | фикс GSC пути после packages split (CI Calibration зелёный) |

Всё запушено в `origin/master`. Тесты: **375 passed + 5 skipped**.

## Баг packages split 0.5.2 (исправлен, важно помнить)

- Коммит `e821e62` (17 авг) перенёс CLI в `gsc_cli/`, но `gsc_cli/gsc_external.py:36`
  остался с `GSC = Path(__file__).parent / "gsc.py"` → указывал на **несуществующий**
  `gsc_cli/gsc.py`. `gsc.py` — корневой shim (`→ gsc_cli.main`).
- Эффект: subprocess падал `FileNotFoundError`, голый `except` глотал → `raw_findings = 0`,
  Python-детекторы не запускались. `scan_multilang` маскировал для мультиязычных проектов,
  но flask-jwt-auth (чистый Python hardcoded JWT secret GS011/GS019) валился на
  `expect_blocking`. CI Calibration красный 08-17/18/19.
- **Фикс:** `GSC = Path(__file__).resolve().parent.parent / "gsc.py"`. Верифицирован:
  raw findings 0→35, CI run `32231488846` = success (13/13, Missed 0).

## Методология precision-pass (повторять так же)

1. **Бриф** — self-contained EN, полный embedded код детектора, §7 строгий формат ответа,
   §8 ожидаемые дельты. Явный запрет выдумывать `rule_id`/сигнатуры `load_patterns`/
   зеркала CVE. Кириллица только в SPDX.
2. **Приём ответа агента** — всегда критика → патчи → самостоятельная верификация
   (`py_compile` + калибровочные сканы + полный pytest). Агент НЕ видит регрессий recall.
3. **Precision-first, но НЕ ценой TP.** Обязательные positive/negative/FP fixtures +
   regression-тесты после каждого детектора. `xss 2/2` — жёсткий инвариант.
4. **Измерение:** `python3 scripts/gsc_precision_measure.py` (clean FP + recall),
   `python3 /tmp/gs0NN_verify.py` — скан по calibration-проектам.

## Уроки (подводные камни, не повторять)

- **Lead 3 GS020 (suppress `.innerHTML = <var>`)** откачен — потерял pygoat TP
  `li.innerHTML = data.logs[i]` (a9.js). `.innerHTML = <variable>` фундаментально
  двусмысленен, suppress только static string literals (через `_is_false_positive`).
- **Маркер-баг GS020:** `_REFLECTED_PATTERN_MARKERS` имел `f"`/`f'`, но f-string regex
  это `f["']` — ветка downgrade/suppress была мертва для f-string. Проверять маркеры
  против реального паттерна.
- **Off-by-one в window-логике:** `line_no` 1-indexed vs `lines[]` 0-indexed, и
  `range(0, 0, -1)` пуст. Тест на function-parameter guard.
- **Сужение SSRF f-string URL** требует taint token внутри `{...}` — иначе config-derived
  base URL даёт FP.

## Что осталось (для новой сессии)

- **Precision-очередь:** GS037 (21) → GS003/GS022 (14/14). Брифы по шаблону §7.
- **Хвосты ROADMAP:** полный packages split 0.5.3 (gsc_cloud) и 0.5.4/0.5.5 (dev-изоляция,
  shim cleanup); миграция 34 RU-брифов в EN; reconciliation/packages split/Registry;
  Proof Engine; Platform Play.
- **PoC-генерация локально зависает на LLM** (>400s на 5 PoC) — локальная сеть к DeepSeek;
  в CI работает (54s на 13 проектов). При локальной отладке `gsc_external.py scan`
  использовать `--scan-mode quick` или отключить LLM, иначе ждать долго.
