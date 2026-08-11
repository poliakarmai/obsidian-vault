---
title: "GSC Audit: /tmp/gsc-hunt-3"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-3

**Дата:** 10.08.2026 07:09  
**Путь:** `/tmp/gsc-hunt-3`  
**Всего находок:** 249  
**CRITICAL:** 14 | **HIGH:** 8 | **MEDIUM:** 10 | **LOW:** 26

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 119 |
| GS003 | 21 |
| GS034-token_collector | 17 |
| GS025-no_rate_limit_auth | 13 |
| GS021 | 12 |
| GS020 | 7 |
| GS015 | 6 |
| GS032-exfil_env_send | 6 |
| GS007 | 6 |
| GS005 | 5 |
| GS000-LEGACY | 5 |
| GS011 | 5 |
| TS: useEffect missing deps | 5 |
| GS025 | 3 |
| GS029 | 3 |
| GS001 | 3 |
| GS025-hardcoded_secret | 3 |
| GS019 | 2 |
| YAML-B39DC08C | 2 |
| GS036-dangerously_set_html | 1 |
| GS037-hardcoded_password | 1 |
| GS009 | 1 |
| GS025-eval_usage | 1 |
| GS025-insecure_random | 1 |
| YAML-36ACF0AD | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | seed.py | 48 | OWASP A03: Injection |
| CRITICAL | GS005 | seed.py | 48 |  |
| CRITICAL | GS001 | screenshots.mjs | 811 | Found: password: 'showcase-sync' |
| CRITICAL | GS001 | import_library.py | 192 | Found: sqlite:///{db_path} |
| CRITICAL | GS001 | seed_showcase.py | 234 | Found: sqlite:///{db_path} |
| CRITICAL | GS029 | outbound_notifications.py | 106 | Match:         msg_url = url.rstrip("/") + "/message?token=" |
| CRITICAL | GS005 | database.py | 79 | Line 79: conn.execute(text(f"DROP TRIGGER IF EXISTS {trig}") |
| CRITICAL | GS005 | database.py | 79 | Line 79: conn.execute(text(f"DROP TRIGGER IF EXISTS {trig}") |
| CRITICAL | GS005 | seed.py | 48 | Line 48: db.execute(text(f"DELETE FROM {table}")) |
| CRITICAL | GS007 | send_to_device.py | 474 | Line 474: @router.get("/admin/send-history", response_model= |
| CRITICAL | GS007 | users.py | 758 | Line 758: @router.delete("/admin/sync-status/{user_id}/{book |
| CRITICAL | GS007 | users.py | 786 | Line 786: @router.get("/admin/audit-logs") |
| CRITICAL | GS007 | wishlist.py | 365 | Line 365: @router.get("/admin/wishlist/matches", response_mo |
| CRITICAL | GS007 | wishlist.py | 396 | Line 396: @router.post("/admin/wishlist/{wish_id}/fulfill",  |
| HIGH | GS000-LEGACY | SearchBox.tsx | 53 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | theme.ts | 25 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | metadata.py | 438 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | fetch_seed_covers.py | 139 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | SearchBox.tsx | 99 | Match:                     <div className="search-result-exc |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS007 | tome_sync.py | 1308 | Line 1308: @router.get("/tome-sync/download/{book_id}/{file_ |
| HIGH | GS019 | auth.py | 72 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | seed.py | 48 |
| H | GS000-LEGACY | SearchBox.tsx | 53 |
| H | GS000-LEGACY | theme.ts | 25 |
| H | GS000-LEGACY | metadata.py | 438 |
| H | GS000-LEGACY | fetch_seed_covers.py | 139 |
| C | GS005 | seed.py | 48 |
| M | GS025 | outbound_notifications.py | 106 |
| M | GS025 | hardcover.py | 99 |
| M | GS029 | outbound_notifications.py | 106 |
| M | GS029 | hardcover.py | 99 |
| C | GS001 | screenshots.mjs | 811 |
| C | GS001 | import_library.py | 192 |
| C | GS001 | seed_showcase.py | 234 |
| L | GS003 | record-hero.mjs | 130 |
| L | GS003 | record-hero.mjs | 161 |
| L | GS003 | record-hero.mjs | 163 |
| L | GS003 | record-hero.mjs | 168 |
| L | GS003 | screenshots.mjs | 1102 |
| L | GS003 | screenshots.mjs | 1105 |
| L | GS003 | screenshots.mjs | 1111 |
| L | GS003 | screenshots.mjs | 1114 |
| L | GS003 | screenshots.mjs | 1121 |
| L | GS003 | shot-audit.mjs | 13 |
| L | GS003 | shot-audit.mjs | 21 |
| L | GS003 | shot-stats-refresh.mjs | 19 |
| L | GS003 | shot-ui-leftovers.mjs | 27 |
| L | GS003 | verify-statslab.mjs | 10 |
| L | GS003 | verify-statslab.mjs | 24 |
| L | GS003 | verify-statslab.mjs | 136 |
| L | GS003 | export-excalidraw.mjs | 50 |
| L | GS003 | generate-diagrams.mjs | 292 |
| L | GS003 | generate-diagrams.mjs | 294 |
| L | GS003 | render-og.mjs | 33 |
| L | GS003 | render-pwa-icons.mjs | 37 |
| I | GS015 | urls.py | 1 |
| I | GS015 | main.py | 815 |
| I | GS015 | main.py | 815 |
| I | GS015 | main.py | 815 |
| I | GS015 | main.py | 737 |
| I | GS015 | main.py | 826 |
| i | GS020 |  | 1290 |
| i | GS020 |  | 99 |
| i | GS020 |  | 4 |
| i | GS020 |  | 821 |
| i | GS020 |  | 446 |
| i | GS020 |  | 684 |
| i | GS020 |  | 8 |
| ? | GS032-exfil_env_send | helpers.ts | 31 |
| ? | GS032-exfil_env_send | helpers.ts | 39 |
| ? | GS032-exfil_env_send | tokens.ts | 3 |
| ? | GS032-exfil_env_send | tokens.ts | 26 |
| ? | GS032-exfil_env_send | tokens.ts | 30 |
| ? | GS032-exfil_env_send | tokens.ts | 34 |
| ? | GS034-token_collector | helpers.ts | 9 |
| ? | GS034-token_collector | record-hero.mjs | 12 |
| ? | GS034-token_collector | screenshots.mjs | 23 |
| ? | GS034-token_collector | screenshots.mjs | 24 |
| ? | GS034-token_collector | screenshots.mjs | 25 |
| ? | GS034-token_collector | screenshots.mjs | 26 |
| ? | GS034-token_collector | screenshots.mjs | 27 |
| ? | GS034-token_collector | screenshots.mjs | 28 |
| ? | GS034-token_collector | screenshots.mjs | 29 |
| ? | GS034-token_collector | screenshots.mjs | 38 |
| ? | GS034-token_collector | shot-audit.mjs | 2 |
| ? | GS034-token_collector | shot-stats-refresh.mjs | 3 |
| ? | GS034-token_collector | shot-ui-leftovers.mjs | 7 |
| ? | GS034-token_collector | verify-statslab.mjs | 5 |
| ? | GS034-token_collector | vite.config.ts | 95 |
| ? | GS034-token_collector | vite.config.ts | 98 |
| ? | GS034-token_collector | vite.config.ts | 102 |
| ? | GS036-dangerously_set_html | SearchBox.tsx | 99 |
| ? | GS037-hardcoded_password | seed.py | 36 |
| C | GS029 | outbound_notifications.py | 106 |
| H | GS000-LEGACY | SearchBox.tsx | 99 |
| H | GS025 | docker-compose.yml | 0 |
| C | GS005 | database.py | 79 |
| C | GS005 | database.py | 79 |
| C | GS005 | seed.py | 48 |
| C | GS007 | send_to_device.py | 474 |
| H | GS007 | tome_sync.py | 1308 |
| C | GS007 | users.py | 758 |
| C | GS007 | users.py | 786 |
| C | GS007 | wishlist.py | 365 |
| C | GS007 | wishlist.py | 396 |
| s | GS009 |  | 0 |
| L | GS011 | books.py | 2186 |
| L | GS011 | books.py | 2245 |
| L | GS011 | books.py | 2299 |
| L | GS011 | books.py | 2339 |
| L | GS011 | security.py | 38 |
| H | GS019 | auth.py | 72 |
| M | GS019 | auth.py | 137 |
| s | GS021 |  | 15 |
| s | GS021 |  | 20 |
| s | GS021 |  | 98 |
| s | GS021 |  | 102 |
| s | GS021 |  | 749 |
| s | GS021 |  | 1445 |
| s | GS021 |  | 36 |
| s | GS021 |  | 29 |
| s | GS021 |  | 51 |
| s | GS021 |  | 51 |
| s | GS021 |  | 58 |
| s | GS021 |  | 58 |
| r | GS022 |  | 27 |
| r | GS022 |  | 31 |
| r | GS022 |  | 32 |
| r | GS022 |  | 33 |
| r | GS022 |  | 34 |
| r | GS022 |  | 35 |
| r | GS022 |  | 36 |
| r | GS022 |  | 37 |
| r | GS022 |  | 38 |
| r | GS022 |  | 39 |
| r | GS022 |  | 40 |
| r | GS022 |  | 41 |
| r | GS022 |  | 42 |
| r | GS022 |  | 43 |
| r | GS022 |  | 44 |
| r | GS022 |  | 45 |
| r | GS022 |  | 46 |
| r | GS022 |  | 47 |
| r | GS022 |  | 204 |
| r | GS022 |  | 253 |
| r | GS022 |  | 889 |
| r | GS022 |  | 12 |
| r | GS022 |  | 40 |
| r | GS022 |  | 45 |
| r | GS022 |  | 81 |
| r | GS022 |  | 1430 |
| r | GS022 |  | 1450 |
| r | GS022 |  | 1474 |
| r | GS022 |  | 1512 |
| r | GS022 |  | 84 |
| r | GS022 |  | 41 |
| r | GS022 |  | 32 |
| r | GS022 |  | 36 |
| r | GS022 |  | 65 |
| r | GS022 |  | 91 |
| r | GS022 |  | 112 |
| r | GS022 |  | 136 |
| r | GS022 |  | 159 |
| r | GS022 |  | 185 |
| r | GS022 |  | 214 |
| r | GS022 |  | 240 |
| r | GS022 |  | 264 |
| r | GS022 |  | 298 |
| r | GS022 |  | 328 |
| r | GS022 |  | 351 |
| r | GS022 |  | 28 |
| r | GS022 |  | 20 |
| r | GS022 |  | 49 |
| r | GS022 |  | 129 |
| r | GS022 |  | 45 |
| r | GS022 |  | 72 |
| r | GS022 |  | 73 |
| r | GS022 |  | 90 |
| r | GS022 |  | 95 |
| r | GS022 |  | 112 |
| r | GS022 |  | 119 |
| r | GS022 |  | 182 |
| r | GS022 |  | 238 |
| r | GS022 |  | 239 |
| r | GS022 |  | 245 |
| r | GS022 |  | 37 |
| r | GS022 |  | 43 |
| r | GS022 |  | 154 |
| r | GS022 |  | 161 |
| r | GS022 |  | 1930 |
| r | GS022 |  | 1933 |
| r | GS022 |  | 583 |
| r | GS022 |  | 590 |
| r | GS022 |  | 135 |
| r | GS022 |  | 278 |
| r | GS022 |  | 288 |
| r | GS022 |  | 89 |
| r | GS022 |  | 313 |
| r | GS022 |  | 320 |
| r | GS022 |  | 498 |
| r | GS022 |  | 506 |
| r | GS022 |  | 537 |
| r | GS022 |  | 545 |
| r | GS022 |  | 1937 |
| r | GS022 |  | 1939 |
| r | GS022 |  | 330 |
| r | GS022 |  | 337 |
| r | GS022 |  | 173 |
| r | GS022 |  | 309 |
| r | GS022 |  | 356 |
| r | GS022 |  | 777 |
| r | GS022 |  | 852 |
| r | GS022 |  | 876 |
| r | GS022 |  | 877 |
| r | GS022 |  | 1084 |
| r | GS022 |  | 1165 |
| r | GS022 |  | 1214 |
| r | GS022 |  | 6 |
| r | GS022 |  | 7 |
| r | GS022 |  | 14 |
| r | GS022 |  | 61 |
| r | GS022 |  | 99 |
| r | GS022 |  | 102 |
| r | GS022 |  | 191 |
| r | GS022 |  | 192 |
| r | GS022 |  | 414 |
| r | GS022 |  | 455 |
| r | GS022 |  | 480 |
| r | GS022 |  | 526 |
| r | GS022 |  | 722 |
| r | GS022 |  | 730 |
| r | GS022 |  | 756 |
| r | GS022 |  | 783 |
| r | GS022 |  | 787 |
| r | GS022 |  | 799 |
| r | GS022 |  | 858 |
| r | GS022 |  | 864 |
| r | GS022 |  | 870 |
| r | GS022 |  | 902 |
| r | GS022 |  | 965 |
| r | GS022 |  | 990 |
| r | GS022 |  | 998 |
| r | GS022 |  | 1007 |
| r | GS022 |  | 69 |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | YAML-36ACF0AD | tome_sync.py | ? |
| ? | YAML-B39DC08C | fetch_seed_covers.py | ? |
| ? | YAML-B39DC08C | seed_showcase.py | ? |
| M | ? | NotificationChannels.tsx | 40 |
| M | ? | CoverAudit.tsx | 50 |
| M | ? | InstanceBackup.tsx | 25 |
| M | ? | ShareLinksOverview.tsx | 27 |
| M | ? | WishlistPage.tsx | 69 |

---
*Сгенерировано GSC v0.6 · 2026-08-10T07:09:04.280869*