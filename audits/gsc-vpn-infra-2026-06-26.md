---
title: "GSC Audit: vpn-infra"
date: 2026-06-26
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — vpn-infra

**Дата:** 26.06.2026 08:42  
**Путь:** `/opt/vpn-seller-bot`  
**Всего находок:** 49  
**CRITICAL:** 1 | **HIGH:** 7 | **MEDIUM:** 31 | **LOW:** 10

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Синхронный код в async | 31 |
| GS003 | 10 |
| Хардкод IP адреса | 5 |
| Python: File upload without content-type validation | 1 |
| Hardcoded encryption key | 1 |
| World-readable file: bot.db (644) | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | bot.py.bak.audit-20260611 | 1713 | Match:         msg_key = "lang_set_ru" if new_lang == "ru" e |
| HIGH | ? | bot.py | 1168 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | bot.py | 997 | Match: DNS = 1.1.1.1, 8.8.8.8 |
| HIGH | ? | bot.py | 1013 | Match: AllowedIPs = 0.0.0.0/0 |
| HIGH | ? | bot.py.bak.audit-20260611 | 173 | Match:     "proxy_access":         {"ru": "🔑 Твой MTProto пр |
| HIGH | ? | bot.py.bak.audit-20260611 | 934 | Match: DNS = 1.1.1.1, 8.8.8.8 |
| HIGH | ? | bot.py.bak.audit-20260611 | 950 | Match: AllowedIPs = 0.0.0.0/0 |
| HIGH | ? | bot.db | 0 | Permissions 644 — should be 600 for sensitive files |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | ? | bot.py | 1168 |
| L | GS003 | admin_key.py | 153 |
| L | GS003 | admin_key.py | 173 |
| L | GS003 | admin_key.py | 180 |
| L | GS003 | admin_key.py | 181 |
| L | GS003 | admin_key.py | 187 |
| L | GS003 | admin_key.py | 188 |
| L | GS003 | admin_key.py | 189 |
| L | GS003 | admin_key.py | 190 |
| L | GS003 | admin_key.py | 191 |
| L | GS003 | admin_key.py | 193 |
| H | ? | bot.py | 997 |
| H | ? | bot.py | 1013 |
| H | ? | bot.py.bak.audit-20260611 | 173 |
| H | ? | bot.py.bak.audit-20260611 | 934 |
| H | ? | bot.py.bak.audit-20260611 | 950 |
| C | ? | bot.py.bak.audit-20260611 | 1713 |
| H | ? | bot.db | 0 |
| M | ? | admin_key.py | 145 |
| M | ? | admin_key.py | 157 |
| M | ? | bot.py | 858 |
| M | ? | bot.py | 914 |
| M | ? | bot.py | 944 |
| M | ? | bot.py | 949 |
| M | ? | bot.py | 959 |
| M | ? | bot.py | 984 |
| M | ? | bot.py | 985 |
| M | ? | bot.py | 1103 |
| M | ? | bot.py | 1604 |
| M | ? | bot.py | 1679 |
| M | ? | bot.py | 2160 |
| M | ? | bot.py | 2504 |
| M | ? | bot.py | 2550 |
| M | ? | bot.py | 2579 |
| M | ? | bot.py.bak.audit-20260611 | 791 |
| M | ? | bot.py.bak.audit-20260611 | 847 |
| M | ? | bot.py.bak.audit-20260611 | 863 |
| M | ? | bot.py.bak.audit-20260611 | 883 |
| M | ? | bot.py.bak.audit-20260611 | 888 |
| M | ? | bot.py.bak.audit-20260611 | 898 |
| M | ? | bot.py.bak.audit-20260611 | 922 |
| M | ? | bot.py.bak.audit-20260611 | 923 |
| M | ? | bot.py.bak.audit-20260611 | 1040 |
| M | ? | bot.py.bak.audit-20260611 | 1495 |
| M | ? | bot.py.bak.audit-20260611 | 1572 |
| M | ? | bot.py.bak.audit-20260611 | 1998 |
| M | ? | bot.py.bak.audit-20260611 | 2305 |
| M | ? | bot.py.bak.audit-20260611 | 2351 |
| M | ? | bot.py.bak.audit-20260611 | 2380 |

---
*Сгенерировано GSC v0.6 · 2026-06-26T08:42:31.237411*