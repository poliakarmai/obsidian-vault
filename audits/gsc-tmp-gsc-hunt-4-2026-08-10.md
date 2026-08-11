---
title: "GSC Audit: /tmp/gsc-hunt-4"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-4

**Дата:** 10.08.2026 07:10  
**Путь:** `/tmp/gsc-hunt-4`  
**Всего находок:** 806  
**CRITICAL:** 6 | **HIGH:** 113 | **MEDIUM:** 3 | **LOW:** 45

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS020 | 259 |
| GS022 | 134 |
| YAML-36ACF0AD | 103 |
| GS025-eval_usage | 102 |
| Rust: .clone() in hot path | 86 |
| GS012 | 38 |
| GS000-LEGACY | 24 |
| GS021 | 13 |
| GS036-redos | 11 |
| GS015 | 8 |
| GS003 | 7 |
| GS005 | 4 |
| GS025-insecure_random | 3 |
| GS010 | 2 |
| GS025 | 2 |
| GS001 | 1 |
| GS036-high_risk | 1 |
| GS037-debug_true | 1 |
| GS002 | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS019 | 1 |
| GS025-debug_mode | 1 |
| GS025-hardcoded_secret | 1 |
| YAML-ECB85AD8 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | bootstrap.min.js | 6 | OWASP A03: Injection |
| CRITICAL | GS005 | jquery-ui.min.js | 7 | OWASP A03: Injection |
| CRITICAL | GS005 | az.js | 5 | OWASP A03: Injection |
| CRITICAL | GS005 | bootstrap.min.js | 6 | OWASP A03: Injection |
| CRITICAL | GS001 | ckeditor.js | 1088 | Found: accessKey:"advAccessKey" |
| CRITICAL | GS019 | settings.py | 5 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | GS000-LEGACY | views.py | 41 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 69 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 70 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 115 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 152 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 24 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | managers.py | 16 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | forms.py | 63 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | forms.py | 66 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | forms.py | 85 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | forms.py | 88 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | common_views.py | 37 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | common_views.py | 40 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | common_views.py | 63 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | common_views.py | 66 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | common_views.py | 135 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | common_views.py | 146 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 94 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 248 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 308 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 386 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 537 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 612 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | settings.py | 7 | Match: DEBUG = True |
| HIGH | GS025 | docker-compose.prod.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | nginx.conf | 0 | File nginx.conf has permissions -rw-rw-r-- — readable by any |
| HIGH | GS011 | settings.py | 5 | Found JWT secret in code: 'g!y0otek...'. JWT secrets must be |
| HIGH | ? | bootstrap-datetimepicker.min.js | 1 | Clone in performance-critical code — consider references |
| HIGH | ? | bootstrap-datetimepicker.min.js | 2 | Clone in performance-critical code — consider references |
| HIGH | ? | moment.min.js | 1 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery-ui.min.js | 7 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery-ui.min.js | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery-ui.min.js | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery-ui.min.js | 12 | Clone in performance-critical code — consider references |
| HIGH | ? | fullcalendar.min.js | 6 | Clone in performance-critical code — consider references |
| HIGH | ? | fullcalendar.min.js | 7 | Clone in performance-critical code — consider references |
| HIGH | ? | fullcalendar.min.js | 8 | Clone in performance-critical code — consider references |
| HIGH | ? | fullcalendar.min.js | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | fullcalendar.min.js | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery.fancybox.min.js | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery-1.3.2.js | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | find.js | 7 | Clone in performance-critical code — consider references |
| HIGH | ? | anchor.js | 6 | Clone in performance-critical code — consider references |
| HIGH | ? | div.js | 3 | Clone in performance-critical code — consider references |
| HIGH | ? | plugin.js | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 313 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 358 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 427 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 437 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 789 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 928 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 929 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 999 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1109 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1122 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1125 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1126 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1266 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1269 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1272 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1278 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1279 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1308 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1358 | Clone in performance-critical code — consider references |
| HIGH | ? | ckeditor.js | 1369 | Clone in performance-critical code — consider references |
| HIGH | ? | raphael.min.js | 1 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery.dataTables.min.js | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery.dataTables.min.js | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | jquery.dataTables.min.js | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | datatables.min.js | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | datatables.min.js | 74 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | bootstrap.min.js | 6 |
| C | GS005 | jquery-ui.min.js | 7 |
| C | GS005 | az.js | 5 |
| C | GS005 | bootstrap.min.js | 6 |
| M | GS010 | views.py | 273 |
| M | GS010 | views.py | 337 |
| H | GS000-LEGACY | views.py | 41 |
| H | GS000-LEGACY | views.py | 69 |
| H | GS000-LEGACY | views.py | 70 |
| H | GS000-LEGACY | views.py | 115 |
| H | GS000-LEGACY | views.py | 152 |
| H | GS000-LEGACY | models.py | 24 |
| H | GS000-LEGACY | managers.py | 16 |
| H | GS000-LEGACY | forms.py | 63 |
| H | GS000-LEGACY | forms.py | 66 |
| H | GS000-LEGACY | forms.py | 85 |
| H | GS000-LEGACY | forms.py | 88 |
| H | GS000-LEGACY | common_views.py | 37 |
| H | GS000-LEGACY | common_views.py | 40 |
| H | GS000-LEGACY | common_views.py | 63 |
| H | GS000-LEGACY | common_views.py | 66 |
| H | GS000-LEGACY | common_views.py | 135 |
| H | GS000-LEGACY | common_views.py | 146 |
| H | GS000-LEGACY | models.py | 94 |
| H | GS000-LEGACY | views.py | 248 |
| H | GS000-LEGACY | views.py | 308 |
| H | GS000-LEGACY | views.py | 386 |
| H | GS000-LEGACY | views.py | 537 |
| H | GS000-LEGACY | views.py | 612 |
| M | GS025 | settings.py | 5 |
| C | GS001 | ckeditor.js | 1088 |
| L | GS003 | theia-sticky-sidebar.js | 37 |
| L | GS003 | plugin.js | 7 |
| L | GS003 | plugin.js | 7 |
| L | GS003 | plugin.js | 5 |
| L | GS003 | plugin.js | 1 |
| L | GS003 | datatables.min.js | 86 |
| L | GS003 | jquery.dataTables.min.js | 74 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | asgi.py | 16 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 16 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 71 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 2 |
| i | GS020 |  | 1 |
| i | GS020 |  | 12 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 120 |
| i | GS020 |  | 105 |
| i | GS020 |  | 105 |
| i | GS020 |  | 105 |
| i | GS020 |  | 105 |
| i | GS020 |  | 106 |
| i | GS020 |  | 106 |
| i | GS020 |  | 932 |
| i | GS020 |  | 513 |
| i | GS020 |  | 514 |
| i | GS020 |  | 637 |
| i | GS020 |  | 1182 |
| i | GS020 |  | 106 |
| i | GS020 |  | 375 |
| i | GS020 |  | 624 |
| i | GS020 |  | 730 |
| i | GS020 |  | 921 |
| i | GS020 |  | 971 |
| i | GS020 |  | 216 |
| i | GS020 |  | 370 |
| i | GS020 |  | 380 |
| i | GS020 |  | 382 |
| i | GS020 |  | 474 |
| i | GS020 |  | 476 |
| i | GS020 |  | 694 |
| i | GS020 |  | 695 |
| i | GS020 |  | 741 |
| i | GS020 |  | 749 |
| i | GS020 |  | 761 |
| i | GS020 |  | 763 |
| i | GS020 |  | 911 |
| i | GS020 |  | 922 |
| i | GS020 |  | 923 |
| i | GS020 |  | 923 |
| i | GS020 |  | 947 |
| i | GS020 |  | 985 |
| i | GS020 |  | 1034 |
| i | GS020 |  | 1035 |
| i | GS020 |  | 1037 |
| i | GS020 |  | 1046 |
| i | GS020 |  | 1065 |
| i | GS020 |  | 1122 |
| i | GS020 |  | 1137 |
| i | GS020 |  | 1148 |
| i | GS020 |  | 1149 |
| i | GS020 |  | 1149 |
| i | GS020 |  | 1150 |
| i | GS020 |  | 1150 |
| i | GS020 |  | 1158 |
| i | GS020 |  | 1159 |
| i | GS020 |  | 1160 |
| i | GS020 |  | 1163 |
| i | GS020 |  | 1165 |
| i | GS020 |  | 1181 |
| i | GS020 |  | 1183 |
| i | GS020 |  | 1187 |
| i | GS020 |  | 1187 |
| i | GS020 |  | 1191 |
| i | GS020 |  | 1199 |
| i | GS020 |  | 1199 |
| i | GS020 |  | 1199 |
| i | GS020 |  | 1200 |
| i | GS020 |  | 1203 |
| i | GS020 |  | 1212 |
| i | GS020 |  | 1213 |
| i | GS020 |  | 1213 |
| i | GS020 |  | 1254 |
| i | GS020 |  | 1255 |
| i | GS020 |  | 1320 |
| i | GS020 |  | 1322 |
| i | GS020 |  | 1325 |
| i | GS020 |  | 1342 |
| i | GS020 |  | 1367 |
| i | GS020 |  | 1446 |
| i | GS020 |  | 45 |
| i | GS020 |  | 43 |
| i | GS020 |  | 911 |
| i | GS020 |  | 2136 |
| i | GS020 |  | 2192 |
| i | GS020 |  | 2203 |
| i | GS020 |  | 2233 |
| i | GS020 |  | 3122 |
| i | GS020 |  | 4230 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 6 |
| i | GS020 |  | 7 |
| i | GS020 |  | 7 |
| i | GS020 |  | 9 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 6 |
| i | GS020 |  | 22 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 4 |
| i | GS020 |  | 10 |
| i | GS020 |  | 5 |
| i | GS020 |  | 5 |
| i | GS020 |  | 179 |
| i | GS020 |  | 179 |
| i | GS020 |  | 179 |
| i | GS020 |  | 198 |
| i | GS020 |  | 179 |
| i | GS020 |  | 8 |
| i | GS020 |  | 9 |
| i | GS020 |  | 78 |
| i | GS020 |  | 88 |
| i | GS020 |  | 88 |
| i | GS020 |  | 88 |
| i | GS020 |  | 88 |
| i | GS020 |  | 13 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 4 |
| i | GS020 |  | 2 |
| i | GS020 |  | 3 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 22 |
| i | GS020 |  | 24 |
| i | GS020 |  | 45 |
| i | GS020 |  | 58 |
| i | GS020 |  | 58 |
| i | GS020 |  | 45 |
| i | GS020 |  | 34 |
| i | GS020 |  | 36 |
| i | GS020 |  | 57 |
| i | GS020 |  | 70 |
| i | GS020 |  | 71 |
| i | GS020 |  | 57 |
| i | GS020 |  | 146 |
| i | GS020 |  | 155 |
| i | GS020 |  | 160 |
| i | GS020 |  | 145 |
| i | GS020 |  | 21 |
| i | GS020 |  | 3 |
| i | GS020 |  | 59 |
| i | GS020 |  | 31 |
| ? | GS036-redos | ckeditor.js | 29 |
| ? | GS036-redos | ckeditor.js | 100 |
| ? | GS036-redos | ckeditor.js | 339 |
| ? | GS036-redos | ckeditor.js | 359 |
| ? | GS036-redos | ckeditor.js | 671 |
| ? | GS036-redos | ckeditor.js | 697 |
| ? | GS036-high_risk | ckeditor.js | 1 |
| ? | GS036-redos | default.js | 19 |
| ? | GS036-redos | image.js | 5 |
| ? | GS036-redos | wsc.js | 7 |
| ? | GS036-redos | wsc.js | 9 |
| ? | GS036-redos | wsc.js | 43 |
| ? | GS037-debug_true | settings.py | 7 |
| H | GS000-LEGACY | settings.py | 7 |
| H | GS025 | docker-compose.prod.yml | 0 |
| H | GS002 | nginx.conf | 0 |
| s | GS009 |  | 0 |
| H | GS011 | settings.py | 5 |
| L | GS012 | forms.py | 66 |
| L | GS012 | forms.py | 88 |
| L | GS012 | common_views.py | 40 |
| L | GS012 | common_views.py | 66 |
| L | GS012 | common_views.py | 135 |
| L | GS012 | common_views.py | 146 |
| L | GS012 | views.py | 386 |
| L | GS012 | views.py | 537 |
| L | GS012 | views.py | 612 |
| L | GS012 | views.py | 69 |
| L | GS012 | views.py | 70 |
| L | GS012 | views.py | 115 |
| L | GS012 | views.py | 152 |
| L | GS012 | ckeditor.js | 956 |
| L | GS012 | ckeditor.js | 958 |
| L | GS012 | ckeditor.js | 958 |
| L | GS012 | ckeditor.js | 958 |
| L | GS012 | ckeditor.js | 960 |
| L | GS012 | ckeditor.js | 1320 |
| L | GS012 | ckeditor.js | 1322 |
| L | GS012 | ckeditor.js | 1327 |
| L | GS012 | ckeditor.js | 1329 |
| L | GS012 | ckeditor.js | 1330 |
| L | GS012 | ckeditor.js | 1434 |
| L | GS012 | ckeditor.js | 1436 |
| L | GS012 | ckeditor.js | 1436 |
| L | GS012 | ckeditor.js | 1436 |
| L | GS012 | ckeditor.js | 1440 |
| L | GS012 | plugin.js | 9 |
| L | GS012 | plugin.js | 10 |
| L | GS012 | plugin.js | 11 |
| L | GS012 | plugin.js | 6 |
| L | GS012 | plugin.js | 8 |
| L | GS012 | plugin.js | 8 |
| L | GS012 | plugin.js | 8 |
| L | GS012 | plugin.js | 8 |
| L | GS012 | jquery-1.3.2.js | 4100 |
| L | GS012 | jquery-1.3.2.js | 4143 |
| C | GS019 | settings.py | 5 |
| s | GS021 |  | 104 |
| s | GS021 |  | 2 |
| s | GS021 |  | 1 |
| s | GS021 |  | 7 |
| s | GS021 |  | 11 |
| s | GS021 |  | 2 |
| s | GS021 |  | 863 |
| s | GS021 |  | 953 |
| s | GS021 |  | 507 |
| s | GS021 |  | 6 |
| s | GS021 |  | 13 |
| s | GS021 |  | 2 |
| s | GS021 |  | 4 |
| r | GS022 |  | 194 |
| r | GS022 |  | 26 |
| r | GS022 |  | 34 |
| r | GS022 |  | 657 |
| r | GS022 |  | 29 |
| r | GS022 |  | 55 |
| r | GS022 |  | 85 |
| r | GS022 |  | 88 |
| r | GS022 |  | 99 |
| r | GS022 |  | 2 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 10 |
| r | GS022 |  | 12 |
| r | GS022 |  | 219 |
| r | GS022 |  | 260 |
| r | GS022 |  | 264 |
| r | GS022 |  | 265 |
| r | GS022 |  | 276 |
| r | GS022 |  | 276 |
| r | GS022 |  | 282 |
| r | GS022 |  | 534 |
| r | GS022 |  | 535 |
| r | GS022 |  | 571 |
| r | GS022 |  | 571 |
| r | GS022 |  | 573 |
| r | GS022 |  | 573 |
| r | GS022 |  | 574 |
| r | GS022 |  | 574 |
| r | GS022 |  | 693 |
| r | GS022 |  | 695 |
| r | GS022 |  | 778 |
| r | GS022 |  | 780 |
| r | GS022 |  | 864 |
| r | GS022 |  | 865 |
| r | GS022 |  | 957 |
| r | GS022 |  | 1008 |
| r | GS022 |  | 1008 |
| r | GS022 |  | 1025 |
| r | GS022 |  | 1025 |
| r | GS022 |  | 1081 |
| r | GS022 |  | 1081 |
| r | GS022 |  | 1130 |
| r | GS022 |  | 1130 |
| r | GS022 |  | 1165 |
| r | GS022 |  | 1165 |
| r | GS022 |  | 1174 |
| r | GS022 |  | 1174 |
| r | GS022 |  | 1175 |
| r | GS022 |  | 1175 |
| r | GS022 |  | 1175 |
| r | GS022 |  | 1176 |
| r | GS022 |  | 1176 |
| r | GS022 |  | 1176 |
| r | GS022 |  | 1188 |
| r | GS022 |  | 1189 |
| r | GS022 |  | 1189 |
| r | GS022 |  | 1200 |
| r | GS022 |  | 1201 |
| r | GS022 |  | 1201 |
| r | GS022 |  | 1202 |
| r | GS022 |  | 1398 |
| r | GS022 |  | 1444 |
| r | GS022 |  | 1446 |
| r | GS022 |  | 400 |
| r | GS022 |  | 507 |
| r | GS022 |  | 509 |
| r | GS022 |  | 5 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 3 |
| r | GS022 |  | 32 |
| r | GS022 |  | 1 |
| r | GS022 |  | 5 |
| r | GS022 |  | 5 |
| r | GS022 |  | 11 |
| r | GS022 |  | 5 |
| r | GS022 |  | 5 |
| r | GS022 |  | 8 |
| r | GS022 |  | 6 |
| r | GS022 |  | 10 |
| r | GS022 |  | 20 |
| r | GS022 |  | 50 |
| r | GS022 |  | 51 |
| r | GS022 |  | 51 |
| r | GS022 |  | 5 |
| r | GS022 |  | 5 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 7 |
| r | GS022 |  | 10 |
| r | GS022 |  | 11 |
| r | GS022 |  | 11 |
| r | GS022 |  | 12 |
| r | GS022 |  | 16 |
| r | GS022 |  | 17 |
| r | GS022 |  | 17 |
| r | GS022 |  | 18 |
| r | GS022 |  | 3 |
| r | GS022 |  | 3 |
| r | GS022 |  | 4 |
| r | GS022 |  | 4 |
| r | GS022 |  | 5 |
| r | GS022 |  | 5 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 7 |
| r | GS022 |  | 7 |
| r | GS022 |  | 7 |
| r | GS022 |  | 8 |
| r | GS022 |  | 8 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 3 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 108 |
| r | GS022 |  | 108 |
| r | GS022 |  | 120 |
| r | GS022 |  | 121 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | jquery.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | moment.min.js | ? |
| ? | YAML-36ACF0AD | dropzone.min.js | ? |
| ? | YAML-36ACF0AD | fullcalendar.min.js | ? |
| ? | YAML-36ACF0AD | fullcalendar.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | jquery-ui.min.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | ckeditor.js | ? |
| ? | YAML-36ACF0AD | plugin.js | ? |
| ? | YAML-36ACF0AD | plugin.js | ? |
| ? | YAML-36ACF0AD | plugin.js | ? |
| ? | YAML-36ACF0AD | link.js | ? |
| ? | YAML-36ACF0AD | common.js | ? |
| ? | YAML-36ACF0AD | image.js | ? |
| ? | YAML-36ACF0AD | tableCell.js | ? |
| ? | YAML-36ACF0AD | yui.js | ? |
| ? | YAML-36ACF0AD | yui.js | ? |
| ? | YAML-36ACF0AD | yui.js | ? |
| ? | YAML-36ACF0AD | yui.js | ? |
| ? | YAML-36ACF0AD | yui.js | ? |
| ? | YAML-36ACF0AD | yui.js | ? |
| ? | YAML-36ACF0AD | ciframe.html | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jquery-1.3.2.js | ? |
| ? | YAML-36ACF0AD | jush.js | ? |
| ? | YAML-36ACF0AD | jush.js | ? |
| ? | YAML-36ACF0AD | jush.js | ? |
| ? | YAML-36ACF0AD | jush.js | ? |
| ? | YAML-36ACF0AD | jush.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-36ACF0AD | jquery-3.2.1.min.js | ? |
| ? | YAML-ECB85AD8 | settings.py | ? |
| H | ? | bootstrap-datetimepicker.min.js | 1 |
| H | ? | bootstrap-datetimepicker.min.js | 2 |
| H | ? | moment.min.js | 1 |
| H | ? | jquery-ui.min.js | 7 |
| H | ? | jquery-ui.min.js | 9 |
| H | ? | jquery-ui.min.js | 10 |
| H | ? | jquery-ui.min.js | 12 |
| H | ? | fullcalendar.min.js | 6 |
| H | ? | fullcalendar.min.js | 7 |
| H | ? | fullcalendar.min.js | 8 |
| H | ? | fullcalendar.min.js | 9 |
| H | ? | fullcalendar.min.js | 10 |
| H | ? | jquery.fancybox.min.js | 11 |
| H | ? | jquery-1.3.2.js | 222 |
| H | ? | find.js | 7 |
| H | ? | anchor.js | 6 |
| H | ? | div.js | 3 |
| H | ? | plugin.js | 9 |
| H | ? | ckeditor.js | 113 |
| H | ? | ckeditor.js | 157 |
| H | ? | ckeditor.js | 158 |
| H | ? | ckeditor.js | 173 |
| H | ? | ckeditor.js | 174 |
| H | ? | ckeditor.js | 185 |
| H | ? | ckeditor.js | 186 |
| H | ? | ckeditor.js | 187 |
| H | ? | ckeditor.js | 190 |
| H | ? | ckeditor.js | 192 |
| H | ? | ckeditor.js | 194 |
| H | ? | ckeditor.js | 202 |
| H | ? | ckeditor.js | 205 |
| H | ? | ckeditor.js | 207 |
| H | ? | ckeditor.js | 208 |
| H | ? | ckeditor.js | 210 |
| H | ? | ckeditor.js | 285 |
| H | ? | ckeditor.js | 313 |
| H | ? | ckeditor.js | 358 |
| H | ? | ckeditor.js | 383 |
| H | ? | ckeditor.js | 386 |
| H | ? | ckeditor.js | 399 |
| H | ? | ckeditor.js | 423 |
| H | ? | ckeditor.js | 427 |
| H | ? | ckeditor.js | 433 |
| H | ? | ckeditor.js | 434 |
| H | ? | ckeditor.js | 435 |
| H | ? | ckeditor.js | 437 |
| H | ? | ckeditor.js | 438 |
| H | ? | ckeditor.js | 443 |
| H | ? | ckeditor.js | 445 |
| H | ? | ckeditor.js | 446 |
| H | ? | ckeditor.js | 447 |
| H | ? | ckeditor.js | 448 |
| H | ? | ckeditor.js | 449 |
| H | ? | ckeditor.js | 450 |
| H | ? | ckeditor.js | 457 |
| H | ? | ckeditor.js | 463 |
| H | ? | ckeditor.js | 488 |
| H | ? | ckeditor.js | 492 |
| H | ? | ckeditor.js | 496 |
| H | ? | ckeditor.js | 505 |
| H | ? | ckeditor.js | 509 |
| H | ? | ckeditor.js | 516 |
| H | ? | ckeditor.js | 538 |
| H | ? | ckeditor.js | 703 |
| H | ? | ckeditor.js | 789 |
| H | ? | ckeditor.js | 928 |
| H | ? | ckeditor.js | 929 |
| H | ? | ckeditor.js | 999 |
| H | ? | ckeditor.js | 1109 |
| H | ? | ckeditor.js | 1122 |
| H | ? | ckeditor.js | 1125 |
| H | ? | ckeditor.js | 1126 |
| H | ? | ckeditor.js | 1266 |
| H | ? | ckeditor.js | 1269 |
| H | ? | ckeditor.js | 1272 |
| H | ? | ckeditor.js | 1278 |
| H | ? | ckeditor.js | 1279 |
| H | ? | ckeditor.js | 1308 |
| H | ? | ckeditor.js | 1358 |
| H | ? | ckeditor.js | 1369 |
| H | ? | raphael.min.js | 1 |
| H | ? | jquery.dataTables.min.js | 57 |
| H | ? | jquery.dataTables.min.js | 61 |
| H | ? | jquery.dataTables.min.js | 62 |
| H | ? | datatables.min.js | 69 |
| H | ? | datatables.min.js | 74 |

---
*Сгенерировано GSC v0.6 · 2026-08-10T07:10:44.872817*