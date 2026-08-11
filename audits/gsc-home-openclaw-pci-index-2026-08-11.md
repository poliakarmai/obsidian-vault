---
title: "GSC Audit: /home/openclaw/pci-index"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/pci-index

**Дата:** 11.08.2026 09:17  
**Путь:** `/home/openclaw/pci-index`  
**Всего находок:** 84  
**CRITICAL:** 0 | **HIGH:** 46 | **MEDIUM:** 6 | **LOW:** 19

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS025 | 38 |
| GS003 | 12 |
| GS018 | 8 |
| YAML-B39DC08C | 4 |
| GS014 | 3 |
| GS020 | 2 |
| GS022 | 2 |
| GS025-eval_usage | 2 |
| YAML-36ACF0AD | 2 |
| GS008 | 1 |
| GS000-LEGACY | 1 |
| Systemd: MemoryDenyWriteExecute= not set | 1 |
| Systemd: RestrictRealtime= not set | 1 |
| Systemd: RemoveIPC= not set | 1 |
| Systemd: LockPersonality= not set | 1 |
| Systemd: RestrictSUIDSGID= not set | 1 |
| GS002 | 1 |
| GS009 | 1 |
| GS016 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | dashboard.py | 334 |  |
| HIGH | GS025 | index_state.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-08.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-06-28.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-01.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-07.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-02.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-03.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-06.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-11.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-06-29.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-04.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-06-30.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-06-26.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-05.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-10.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-06-27.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | 2026-07-09.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | report.log | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260630T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260709T210001Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260704T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260707T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260627T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260701T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260708T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260625T210001Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260626T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260706T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260703T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260702T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260710T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260629T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260705T210003Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260628T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | index_state_20260711T210002Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS002 | public.pem | 0 | File public.pem has permissions -rw-r--r-- — readable by any |
| HIGH | GS016 | pci-bot.service | 11 | Writable script in user directory executed by cron — privile |
| HIGH | GS018 | pci_bot.py | 273 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | pci_bot.py | 655 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | nav.py | 143 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | portfolio.py | 27 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | trading.py | 310 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | trading.py | 369 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | trading.py | 370 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | trading.py | 397 | Float arithmetic for money leads to rounding errors exploita |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS025 | portfolio.py | 135 |
| M | GS025 | portfolio.py | 295 |
| H | GS025 | dashboard.py | 334 |
| M | GS020 | dashboard.py | 126 |
| L | GS003 | reset_genesis.py | 16 |
| L | GS003 | reset_genesis.py | 22 |
| L | GS003 | reset_genesis.py | 68 |
| L | GS003 | reset_genesis.py | 70 |
| L | GS003 | reset_genesis.py | 71 |
| L | GS003 | reset_genesis.py | 72 |
| L | GS003 | reset_genesis.py | 73 |
| L | GS003 | reset_genesis.py | 74 |
| L | GS003 | reset_genesis.py | 75 |
| L | GS003 | reset_genesis.py | 76 |
| L | GS003 | reset_genesis.py | 77 |
| L | GS003 | reset_genesis.py | 78 |
| L | GS008 | trading.py | 50 |
| i | GS020 |  | 126 |
| M | GS000-LEGACY | pci-bot.service | 10 |
| H | GS025 | index_state.json | 0 |
| H | GS025 | 2026-07-08.json | 0 |
| H | GS025 | 2026-06-28.json | 0 |
| H | GS025 | 2026-07-01.json | 0 |
| H | GS025 | 2026-07-07.json | 0 |
| H | GS025 | 2026-07-02.json | 0 |
| H | GS025 | 2026-07-03.json | 0 |
| H | GS025 | 2026-07-06.json | 0 |
| H | GS025 | 2026-07-11.json | 0 |
| H | GS025 | 2026-06-29.json | 0 |
| H | GS025 | 2026-07-04.json | 0 |
| H | GS025 | 2026-06-30.json | 0 |
| H | GS025 | 2026-06-26.json | 0 |
| H | GS025 | 2026-07-05.json | 0 |
| H | GS025 | 2026-07-10.json | 0 |
| H | GS025 | 2026-06-27.json | 0 |
| H | GS025 | 2026-07-09.json | 0 |
| H | GS025 | report.log | 0 |
| H | GS025 | index_state_20260630T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260709T210001Z_daily.json | 0 |
| H | GS025 | index_state_20260704T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260707T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260627T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260701T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260708T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260625T210001Z_daily.json | 0 |
| H | GS025 | index_state_20260626T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260706T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260703T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260702T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260710T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260629T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260705T210003Z_daily.json | 0 |
| H | GS025 | index_state_20260628T210002Z_daily.json | 0 |
| H | GS025 | index_state_20260711T210002Z_daily.json | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| H | GS002 | public.pem | 0 |
| s | GS009 |  | 0 |
| L | GS014 | pci-bot.env | 1 |
| M | GS014 | private.pem | 1 |
| M | GS014 | public.pem | 1 |
| H | GS016 | pci-bot.service | 11 |
| H | GS018 | pci_bot.py | 273 |
| H | GS018 | pci_bot.py | 655 |
| H | GS018 | nav.py | 143 |
| H | GS018 | portfolio.py | 27 |
| H | GS018 | trading.py | 310 |
| H | GS018 | trading.py | 369 |
| H | GS018 | trading.py | 370 |
| H | GS018 | trading.py | 397 |
| s | GS021 |  | 420 |
| r | GS022 |  | 708 |
| r | GS022 |  | 713 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | chart.umd.min.js | ? |
| ? | YAML-36ACF0AD | chart.umd.min.js | ? |
| ? | YAML-B39DC08C | pci_bot.py | ? |
| ? | YAML-B39DC08C | pci_bot.py | ? |
| ? | YAML-B39DC08C | pci_bot.py | ? |
| ? | YAML-B39DC08C | orchestrator.py | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:17:53.888773*