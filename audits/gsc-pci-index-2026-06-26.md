---
title: "GSC Audit: pci-index"
date: 2026-06-26
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — pci-index

**Дата:** 26.06.2026 08:42  
**Путь:** `/home/openclaw/pci-index`  
**Всего находок:** 150  
**CRITICAL:** 0 | **HIGH:** 3 | **MEDIUM:** 1 | **LOW:** 146

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 141 |
| Systemd: EnvironmentFile without quotes → word splitting | 1 |
| World-readable file: index_state.json (664) | 1 |
| World-readable file: index_state_20260625T210001Z_daily.json (664) | 1 |
| Systemd: MemoryDenyWriteExecute= not set | 1 |
| Systemd: RestrictRealtime= not set | 1 |
| Systemd: RemoveIPC= not set | 1 |
| Systemd: LockPersonality= not set | 1 |
| Systemd: RestrictSUIDSGID= not set | 1 |
| GS002 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | index_state.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | ? | index_state_20260625T210001Z_daily.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS002 | public.pem | 0 | File public.pem has permissions -rw-r--r-- — readable by any |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS003 | pci_bot.py | 52 |
| L | GS003 | pci_bot.py | 741 |
| L | GS003 | pci_bot.py | 746 |
| L | GS003 | pci_bot.py | 748 |
| L | GS003 | pci_bot.py | 797 |
| L | GS003 | pci_bot.py | 804 |
| L | GS003 | pci_bot.py | 805 |
| L | GS003 | pci_bot.py | 806 |
| L | GS003 | pci_bot.py | 817 |
| L | GS003 | pci_bot.py | 819 |
| L | GS003 | pci_bot.py | 820 |
| L | GS003 | pci_bot.py | 836 |
| L | GS003 | pci_bot.py | 837 |
| L | GS003 | pci_bot.py | 838 |
| L | GS003 | pci_bot.py | 841 |
| L | GS003 | pci_bot.py | 843 |
| L | GS003 | pci_bot.py | 844 |
| L | GS003 | pci_bot.py | 847 |
| L | GS003 | pci_bot.py | 850 |
| L | GS003 | pci_bot.py | 853 |
| L | GS003 | pci_bot.py | 854 |
| L | GS003 | pci_bot.py | 855 |
| L | GS003 | pci_bot.py | 856 |
| L | GS003 | pci_bot.py | 859 |
| L | GS003 | pci_bot.py | 863 |
| L | GS003 | dashboard.py | 420 |
| L | GS003 | dashboard.py | 421 |
| L | GS003 | dashboard.py | 425 |
| L | GS003 | dashboard.py | 442 |
| L | GS003 | dashboard.py | 446 |
| L | GS003 | dashboard.py | 447 |
| L | GS003 | dip_buy.py | 135 |
| L | GS003 | dip_buy.py | 301 |
| L | GS003 | dip_buy.py | 306 |
| L | GS003 | dip_buy.py | 311 |
| L | GS003 | dip_buy.py | 319 |
| L | GS003 | dip_buy.py | 322 |
| L | GS003 | dip_buy.py | 326 |
| L | GS003 | dip_buy.py | 329 |
| L | GS003 | dip_buy.py | 331 |
| L | GS003 | dip_buy.py | 335 |
| L | GS003 | dip_buy.py | 336 |
| L | GS003 | dip_buy.py | 338 |
| L | GS003 | investors.py | 211 |
| L | GS003 | investors.py | 216 |
| L | GS003 | investors.py | 217 |
| L | GS003 | investors.py | 219 |
| L | GS003 | investors.py | 221 |
| L | GS003 | investors.py | 222 |
| L | GS003 | investors.py | 224 |
| L | GS003 | nav.py | 45 |
| L | GS003 | nav.py | 55 |
| L | GS003 | nav.py | 60 |
| L | GS003 | nav.py | 427 |
| L | GS003 | nav.py | 429 |
| L | GS003 | nav.py | 430 |
| L | GS003 | nav.py | 431 |
| L | GS003 | nav.py | 436 |
| L | GS003 | nav.py | 438 |
| L | GS003 | nav.py | 443 |
| L | GS003 | nav.py | 445 |
| L | GS003 | nav.py | 447 |
| L | GS003 | nav.py | 448 |
| L | GS003 | nav.py | 450 |
| L | GS003 | orchestrator.py | 139 |
| L | GS003 | orchestrator.py | 157 |
| L | GS003 | orchestrator.py | 158 |
| L | GS003 | portfolio.py | 172 |
| L | GS003 | portfolio.py | 276 |
| L | GS003 | portfolio.py | 281 |
| L | GS003 | portfolio.py | 288 |
| L | GS003 | portfolio.py | 293 |
| L | GS003 | portfolio.py | 297 |
| L | GS003 | portfolio.py | 299 |
| L | GS003 | portfolio.py | 301 |
| L | GS003 | portfolio.py | 311 |
| L | GS003 | portfolio.py | 313 |
| L | GS003 | portfolio.py | 315 |
| L | GS003 | portfolio.py | 316 |
| L | GS003 | portfolio.py | 318 |
| L | GS003 | price_feed.py | 35 |
| L | GS003 | price_feed.py | 54 |
| L | GS003 | price_feed.py | 88 |
| L | GS003 | price_feed.py | 90 |
| L | GS003 | price_feed.py | 91 |
| L | GS003 | price_feed.py | 92 |
| L | GS003 | reconcile.py | 192 |
| L | GS003 | reconcile.py | 312 |
| L | GS003 | reconcile.py | 313 |
| L | GS003 | reconcile.py | 314 |
| L | GS003 | reconcile.py | 318 |
| L | GS003 | reconcile.py | 319 |
| L | GS003 | reconcile.py | 320 |
| L | GS003 | reconcile.py | 323 |
| L | GS003 | reconcile.py | 326 |
| L | GS003 | reconcile.py | 327 |
| L | GS003 | reconcile.py | 328 |
| L | GS003 | reconcile.py | 329 |
| L | GS003 | reconcile.py | 330 |
| L | GS003 | reconcile.py | 331 |
| L | GS003 | reconcile.py | 332 |
| L | GS003 | reconcile.py | 333 |
| L | GS003 | reconcile.py | 334 |
| L | GS003 | reconcile.py | 337 |
| L | GS003 | reconcile.py | 338 |
| L | GS003 | reporting.py | 421 |
| L | GS003 | reporting.py | 423 |
| L | GS003 | reporting.py | 425 |
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
| L | GS003 | trading.py | 154 |
| L | GS003 | trading.py | 289 |
| L | GS003 | trading.py | 450 |
| L | GS003 | trading.py | 468 |
| L | GS003 | trading.py | 470 |
| L | GS003 | trading.py | 669 |
| L | GS003 | trading.py | 671 |
| L | GS003 | trading.py | 673 |
| L | GS003 | trading.py | 676 |
| L | GS003 | trading.py | 681 |
| L | GS003 | trading.py | 686 |
| L | GS003 | trading.py | 694 |
| L | GS003 | trading.py | 700 |
| L | GS003 | trading.py | 703 |
| L | GS003 | trading.py | 707 |
| L | GS003 | trading.py | 708 |
| L | GS003 | trading.py | 709 |
| L | GS003 | trading.py | 711 |
| L | GS003 | trading.py | 713 |
| L | GS003 | trading.py | 714 |
| L | GS003 | trading.py | 716 |
| M | ? | pci-bot.service | 10 |
| H | ? | index_state.json | 0 |
| H | ? | index_state_20260625T210001Z_daily.json | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| L | ? | pci-bot.service | 0 |
| H | GS002 | public.pem | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-26T08:42:30.066288*