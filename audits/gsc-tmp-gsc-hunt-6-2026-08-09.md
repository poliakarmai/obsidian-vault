---
title: "GSC Audit: /tmp/gsc-hunt-6"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-6

**Дата:** 09.08.2026 09:53  
**Путь:** `/tmp/gsc-hunt-6`  
**Всего находок:** 215  
**CRITICAL:** 74 | **HIGH:** 8 | **MEDIUM:** 14 | **LOW:** 4

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS020 | 75 |
| GS005 | 73 |
| GS021 | 15 |
| GS022 | 10 |
| GS025 | 8 |
| GS018 | 5 |
| GS015 | 4 |
| GS004 | 4 |
| GS007 | 4 |
| GS003 | 3 |
| Синхронный код в async | 3 |
| GS029 | 2 |
| GS025-no_rate_limit_auth | 2 |
| GS037-hardcoded_password | 1 |
| GS009 | 1 |
| GS017 | 1 |
| GS019 | 1 |
| GS025-wildcard_bind | 1 |
| GS025-eval_usage | 1 |
| YAML-36ACF0AD | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | day_tracks.py | 50 | OWASP A03: Injection |
| CRITICAL | GS005 | day_tracks.py | 77 | OWASP A03: Injection |
| CRITICAL | GS005 | day_tracks.py | 111 | OWASP A03: Injection |
| CRITICAL | GS005 | exporter.py | 704 | OWASP A03: Injection |
| CRITICAL | GS005 | exporter.py | 927 | OWASP A03: Injection |
| CRITICAL | GS005 | scanner.py | 244 | OWASP A03: Injection |
| CRITICAL | GS005 | triage.py | 128 | OWASP A03: Injection |
| CRITICAL | GS005 | triage.py | 133 | OWASP A03: Injection |
| CRITICAL | GS005 | triage.py | 206 | OWASP A03: Injection |
| CRITICAL | GS005 | triage.py | 210 | OWASP A03: Injection |
| CRITICAL | GS005 | triage.py | 355 | OWASP A03: Injection |
| CRITICAL | GS005 | retention.py | 466 | OWASP A03: Injection |
| CRITICAL | GS005 | retention.py | 567 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 348 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 528 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 803 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 819 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 840 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 874 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 878 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 891 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 910 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 933 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 955 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 988 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 1012 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 1032 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 1036 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 1058 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 1077 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 1098 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 1110 | OWASP A03: Injection |
| CRITICAL | GS005 | exports.py | 183 | OWASP A03: Injection |
| CRITICAL | GS005 | archive.py | 126 | OWASP A03: Injection |
| CRITICAL | GS005 | archive.py | 384 | OWASP A03: Injection |
| CRITICAL | GS005 | archive.py | 804 | OWASP A03: Injection |
| CRITICAL | GS005 | queue.py | 315 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | day_tracks.py | 50 |  |
| CRITICAL | GS005 | day_tracks.py | 77 |  |
| CRITICAL | GS005 | day_tracks.py | 111 |  |
| CRITICAL | GS005 | exporter.py | 704 |  |
| CRITICAL | GS005 | exporter.py | 927 |  |
| CRITICAL | GS005 | triage.py | 128 |  |
| CRITICAL | GS005 | triage.py | 133 |  |
| CRITICAL | GS005 | triage.py | 206 |  |
| CRITICAL | GS005 | triage.py | 210 |  |
| CRITICAL | GS005 | triage.py | 355 |  |
| CRITICAL | GS005 | retention.py | 466 |  |
| CRITICAL | GS005 | retention.py | 567 |  |
| CRITICAL | GS005 | queue.py | 348 |  |
| CRITICAL | GS005 | queue.py | 528 |  |
| CRITICAL | GS005 | queue.py | 803 |  |
| CRITICAL | GS005 | queue.py | 819 |  |
| CRITICAL | GS005 | queue.py | 840 |  |
| CRITICAL | GS005 | queue.py | 874 |  |
| CRITICAL | GS005 | queue.py | 878 |  |
| CRITICAL | GS005 | queue.py | 891 |  |
| CRITICAL | GS005 | queue.py | 910 |  |
| CRITICAL | GS005 | queue.py | 933 |  |
| CRITICAL | GS005 | queue.py | 955 |  |
| CRITICAL | GS005 | queue.py | 988 |  |
| CRITICAL | GS005 | queue.py | 1012 |  |
| CRITICAL | GS005 | queue.py | 1032 |  |
| CRITICAL | GS005 | queue.py | 1036 |  |
| CRITICAL | GS005 | queue.py | 1058 |  |
| CRITICAL | GS005 | queue.py | 1077 |  |
| CRITICAL | GS005 | queue.py | 1098 |  |
| CRITICAL | GS005 | queue.py | 1110 |  |
| CRITICAL | GS005 | exports.py | 183 |  |
| CRITICAL | GS005 | archive.py | 126 |  |
| CRITICAL | GS005 | archive.py | 384 |  |
| CRITICAL | GS005 | archive.py | 804 |  |
| CRITICAL | GS029 | app.js | 5085 | Match:                data-key="${escHtml(s.key)}" data-cmd= |
| CRITICAL | GS029 | app.js | 5096 | Match:       <select id="${id}" data-cam-control data-key="$ |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | durations.py | 149 | Line 149: proc = await asyncio.create_subprocess_exec( |
| HIGH | GS004 | exporter.py | 1436 | Line 1436: proc = await asyncio.create_subprocess_exec( |
| HIGH | GS004 | exporter.py | 1457 | Line 1457: proc = await asyncio.create_subprocess_exec( |
| HIGH | GS004 | thumbs.py | 125 | Line 125: proc = await asyncio.create_subprocess_exec( |
| HIGH | GS017 | hub.py | 274 | Password length = 1 chars. |
| HIGH | GS018 | exporter.py | 628 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | sync_worker.py | 484 | Cancel/refund function lacks state check. Risk: refund after |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | day_tracks.py | 50 |
| C | GS005 | day_tracks.py | 77 |
| C | GS005 | day_tracks.py | 111 |
| C | GS005 | exporter.py | 704 |
| C | GS005 | exporter.py | 927 |
| C | GS005 | scanner.py | 244 |
| C | GS005 | triage.py | 128 |
| C | GS005 | triage.py | 133 |
| C | GS005 | triage.py | 206 |
| C | GS005 | triage.py | 210 |
| C | GS005 | triage.py | 355 |
| C | GS005 | retention.py | 466 |
| C | GS005 | retention.py | 567 |
| C | GS005 | queue.py | 348 |
| C | GS005 | queue.py | 528 |
| C | GS005 | queue.py | 803 |
| C | GS005 | queue.py | 819 |
| C | GS005 | queue.py | 840 |
| C | GS005 | queue.py | 874 |
| C | GS005 | queue.py | 878 |
| C | GS005 | queue.py | 891 |
| C | GS005 | queue.py | 910 |
| C | GS005 | queue.py | 933 |
| C | GS005 | queue.py | 955 |
| C | GS005 | queue.py | 988 |
| C | GS005 | queue.py | 1012 |
| C | GS005 | queue.py | 1032 |
| C | GS005 | queue.py | 1036 |
| C | GS005 | queue.py | 1058 |
| C | GS005 | queue.py | 1077 |
| C | GS005 | queue.py | 1098 |
| C | GS005 | queue.py | 1110 |
| C | GS005 | exports.py | 183 |
| C | GS005 | archive.py | 126 |
| C | GS005 | archive.py | 384 |
| C | GS005 | archive.py | 804 |
| M | GS018 | exporter.py | 1525 |
| M | GS018 | exporter.py | 1550 |
| M | GS018 | log_store.py | 149 |
| C | GS005 | queue.py | 315 |
| M | GS025 | triage.py | 98 |
| M | GS025 | triage.py | 150 |
| M | GS025 | triage.py | 156 |
| M | GS025 | triage.py | 271 |
| M | GS025 | sync_worker.py | 944 |
| M | GS025 | archive.py | 1194 |
| M | GS025 | archive.py | 1293 |
| C | GS005 | day_tracks.py | 50 |
| C | GS005 | day_tracks.py | 77 |
| C | GS005 | day_tracks.py | 111 |
| C | GS005 | exporter.py | 704 |
| C | GS005 | exporter.py | 927 |
| L | GS005 | scanner.py | 244 |
| C | GS005 | triage.py | 128 |
| C | GS005 | triage.py | 133 |
| C | GS005 | triage.py | 206 |
| C | GS005 | triage.py | 210 |
| C | GS005 | triage.py | 355 |
| C | GS005 | retention.py | 466 |
| C | GS005 | retention.py | 567 |
| C | GS005 | queue.py | 348 |
| C | GS005 | queue.py | 528 |
| C | GS005 | queue.py | 803 |
| C | GS005 | queue.py | 819 |
| C | GS005 | queue.py | 840 |
| C | GS005 | queue.py | 874 |
| C | GS005 | queue.py | 878 |
| C | GS005 | queue.py | 891 |
| C | GS005 | queue.py | 910 |
| C | GS005 | queue.py | 933 |
| C | GS005 | queue.py | 955 |
| C | GS005 | queue.py | 988 |
| C | GS005 | queue.py | 1012 |
| C | GS005 | queue.py | 1032 |
| C | GS005 | queue.py | 1036 |
| C | GS005 | queue.py | 1058 |
| C | GS005 | queue.py | 1077 |
| C | GS005 | queue.py | 1098 |
| C | GS005 | queue.py | 1110 |
| C | GS005 | exports.py | 183 |
| C | GS005 | archive.py | 126 |
| C | GS005 | archive.py | 384 |
| C | GS005 | archive.py | 804 |
| L | GS003 | log_store.py | 113 |
| L | GS003 | log_store.py | 196 |
| L | GS003 | log_store.py | 209 |
| I | GS015 | app.py | 457 |
| I | GS015 | app.py | 457 |
| I | GS015 | app.py | 457 |
| I | GS015 | app.py | 407 |
| i | GS020 |  | 184 |
| i | GS020 |  | 205 |
| i | GS020 |  | 208 |
| i | GS020 |  | 216 |
| i | GS020 |  | 452 |
| i | GS020 |  | 463 |
| i | GS020 |  | 698 |
| i | GS020 |  | 700 |
| i | GS020 |  | 1155 |
| i | GS020 |  | 453 |
| i | GS020 |  | 553 |
| i | GS020 |  | 588 |
| i | GS020 |  | 651 |
| i | GS020 |  | 653 |
| i | GS020 |  | 670 |
| i | GS020 |  | 721 |
| i | GS020 |  | 780 |
| i | GS020 |  | 799 |
| i | GS020 |  | 1007 |
| i | GS020 |  | 1025 |
| i | GS020 |  | 1095 |
| i | GS020 |  | 1142 |
| i | GS020 |  | 1478 |
| i | GS020 |  | 1829 |
| i | GS020 |  | 2197 |
| i | GS020 |  | 2199 |
| i | GS020 |  | 2205 |
| i | GS020 |  | 2317 |
| i | GS020 |  | 2394 |
| i | GS020 |  | 2420 |
| i | GS020 |  | 2488 |
| i | GS020 |  | 2517 |
| i | GS020 |  | 2616 |
| i | GS020 |  | 2618 |
| i | GS020 |  | 2694 |
| i | GS020 |  | 2741 |
| i | GS020 |  | 2760 |
| i | GS020 |  | 2790 |
| i | GS020 |  | 2831 |
| i | GS020 |  | 2852 |
| i | GS020 |  | 2877 |
| i | GS020 |  | 3215 |
| i | GS020 |  | 3423 |
| i | GS020 |  | 3499 |
| i | GS020 |  | 3576 |
| i | GS020 |  | 3610 |
| i | GS020 |  | 4081 |
| i | GS020 |  | 4094 |
| i | GS020 |  | 4197 |
| i | GS020 |  | 4346 |
| i | GS020 |  | 4390 |
| i | GS020 |  | 4405 |
| i | GS020 |  | 4467 |
| i | GS020 |  | 4987 |
| i | GS020 |  | 4988 |
| i | GS020 |  | 5014 |
| i | GS020 |  | 5039 |
| i | GS020 |  | 5116 |
| i | GS020 |  | 780 |
| i | GS020 |  | 1126 |
| i | GS020 |  | 1451 |
| i | GS020 |  | 1457 |
| i | GS020 |  | 1831 |
| i | GS020 |  | 1833 |
| i | GS020 |  | 2243 |
| i | GS020 |  | 2254 |
| i | GS020 |  | 2394 |
| i | GS020 |  | 2421 |
| i | GS020 |  | 2638 |
| i | GS020 |  | 2647 |
| i | GS020 |  | 3577 |
| i | GS020 |  | 5070 |
| i | GS020 |  | 5081 |
| i | GS020 |  | 5093 |
| i | GS020 |  | 484 |
| ? | GS037-hardcoded_password | settings_schema.py | 247 |
| C | GS029 | app.js | 5085 |
| C | GS029 | app.js | 5096 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS004 | durations.py | 149 |
| H | GS004 | exporter.py | 1436 |
| H | GS004 | exporter.py | 1457 |
| H | GS004 | thumbs.py | 125 |
| I | GS007 | db.py | 97 |
| I | GS007 | db.py | 122 |
| I | GS007 | db.py | 149 |
| I | GS007 | db.py | 189 |
| s | GS009 |  | 0 |
| H | GS017 | hub.py | 274 |
| H | GS018 | exporter.py | 628 |
| H | GS018 | sync_worker.py | 484 |
| M | GS019 | settings.py | 142 |
| s | GS021 |  | 47 |
| s | GS021 |  | 54 |
| s | GS021 |  | 84 |
| s | GS021 |  | 230 |
| s | GS021 |  | 116 |
| s | GS021 |  | 146 |
| s | GS021 |  | 5 |
| s | GS021 |  | 15 |
| s | GS021 |  | 5 |
| s | GS021 |  | 255 |
| s | GS021 |  | 254 |
| s | GS021 |  | 684 |
| s | GS021 |  | 1040 |
| s | GS021 |  | 1085 |
| s | GS021 |  | 180 |
| r | GS022 |  | 267 |
| r | GS022 |  | 278 |
| r | GS022 |  | 2146 |
| r | GS022 |  | 225 |
| r | GS022 |  | 266 |
| r | GS022 |  | 321 |
| r | GS022 |  | 608 |
| r | GS022 |  | 623 |
| r | GS022 |  | 15 |
| r | GS022 |  | 29 |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | app.js | ? |
| M | ? | exporter.py | 266 |
| M | ? | exporter.py | 316 |
| M | ? | exporter.py | 339 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T09:53:34.613690*