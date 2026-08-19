---
status: active
as_of: 2026-08-19
---

# GSC — Git Security Checker

AppSec-платформа Алексея. Самообучающийся security-сканер: 42 детектора
(38 registry + 4 движка: Secrets/SCA/IaC/Invariants), SQLite schema 33,
цикл detect → prove → fix → verify → heal → predict.

- **Репо:** `~/gsc` (GitHub `poliakarmai/gsc`, ветка `master`)
- **SSOT чисел:** `python3 gsc_meta.py` (v1.3.0, schema 33, 147 модулей)
- **Сверка:** `python3 scripts/gsc_reconcile.py`

## Статус (2026-08-19)

- **Precision-pass активен.** Clean FP **539 → 148** на calibration-проектах; recall
  `xss 2/2`/`sql_injection 2/3`/`command_injection 1/1` сохранён. Закрыты GS000-LEGACY,
  GS020 (XSS), GS021 (CSRF/SSRF). Очередь: GS037 (21) → GS003/GS022 (14/14).
- **fp_log (schema v33)** + `scripts/gsc_metrics_dashboard.py` (Precision/FP-rate/TP-rate,
  fallback из `findings.status`). Precision ≈ 0.74 из status-fallback.
- **CI Calibration зелёный** (13/13) после фикса битого пути gsc.py (packages split 0.5.2).
- Фазы Ф1–Ф7 + S1 (PostgreSQL) закрыты. Packages split 0.5.1/0.5.2 done; 0.5.3+ остаётся.

## Ключевые факты

- Push — только по явной команде; по умолчанию commit без push.
- Judge (`/home/openclaw/.local/bin/judge`) перед коммитом, домен «GSC (НЕ bybit-ws)».
- **Брифы детекторов** (`docs/DETECTOR_BRIEF_GS0NN.md`) — EN, self-contained, полный
  embedded код, §7 строгий формат ответа, анти-галлюцинационные guardrails.
- **Код/коммиты/доки GSC — только английский**; кириллица только в SPDX-строке копирайта.
- Лицензия: Apache 2.0 + Commercial dual.
- `gsc.py` — корневой shim (`→ gsc_cli.main`); после packages split пути резолвить
  относительно корня, а не `gsc_cli/`.
