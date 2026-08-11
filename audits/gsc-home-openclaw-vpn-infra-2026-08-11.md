---
title: "GSC Audit: /home/openclaw/vpn-infra"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/vpn-infra

**Дата:** 11.08.2026 09:05  
**Путь:** `/home/openclaw/vpn-infra`  
**Всего находок:** 39  
**CRITICAL:** 0 | **HIGH:** 11 | **MEDIUM:** 20 | **LOW:** 6

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Синхронный код в async | 17 |
| GS025 | 8 |
| GS018 | 3 |
| GS029 | 2 |
| GS000-LEGACY | 1 |
| Systemd: ProtectProc= not set | 1 |
| Systemd: MemoryDenyWriteExecute= not set | 1 |
| Systemd: RestrictRealtime= not set | 1 |
| Systemd: RemoveIPC= not set | 1 |
| Systemd: LockPersonality= not set | 1 |
| Systemd: RestrictSUIDSGID= not set | 1 |
| GS009 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS000-LEGACY | bot.py | 1185 | File upload without MIME-type validation → malicious file up |
| HIGH | GS025 | bot.py | 286 |  |
| HIGH | GS025 | vpn-watch.py | 148 |  |
| HIGH | GS025 | bot.py | 929 |  |
| HIGH | GS025 | bot.py | 964 |  |
| HIGH | GS025 | bot.py | 974 |  |
| HIGH | GS025 | admin_key.py | 160 |  |
| HIGH | GS025 | .mcp.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS018 | bot.py | 633 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | bot.py | 799 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | bot.py | 1862 | Float arithmetic for money leads to rounding errors exploita |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS000-LEGACY | bot.py | 1185 |
| H | GS025 | bot.py | 286 |
| H | GS025 | vpn-watch.py | 148 |
| H | GS025 | bot.py | 929 |
| H | GS025 | bot.py | 964 |
| H | GS025 | bot.py | 974 |
| H | GS025 | admin_key.py | 160 |
| M | GS025 | bot.py | 1278 |
| M | GS029 | bot.py | 1278 |
| M | GS029 | bot.py | 1837 |
| H | GS025 | .mcp.json | 0 |
| L | ? | vpn-core-xray.service | 0 |
| L | ? | vpn-core-xray.service | 0 |
| L | ? | vpn-core-xray.service | 0 |
| L | ? | vpn-core-xray.service | 0 |
| L | ? | vpn-core-xray.service | 0 |
| L | ? | vpn-core-xray.service | 0 |
| s | GS009 |  | 0 |
| H | GS018 | bot.py | 633 |
| H | GS018 | bot.py | 799 |
| H | GS018 | bot.py | 1862 |
| s | GS021 |  | 1028 |
| M | ? | vpn-watch.py | 29 |
| M | ? | bot.py | 873 |
| M | ? | bot.py | 929 |
| M | ? | bot.py | 959 |
| M | ? | bot.py | 964 |
| M | ? | bot.py | 974 |
| M | ? | bot.py | 999 |
| M | ? | bot.py | 1000 |
| M | ? | bot.py | 1120 |
| M | ? | bot.py | 1621 |
| M | ? | bot.py | 1696 |
| M | ? | bot.py | 2177 |
| M | ? | bot.py | 2521 |
| M | ? | bot.py | 2567 |
| M | ? | bot.py | 2596 |
| M | ? | admin_key.py | 148 |
| M | ? | admin_key.py | 160 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:05:43.410513*