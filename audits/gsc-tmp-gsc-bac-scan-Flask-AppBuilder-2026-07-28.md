---
title: "GSC Audit: /tmp/gsc-bac-scan/Flask-AppBuilder"
date: 2026-07-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-bac-scan/Flask-AppBuilder

**Дата:** 28.07.2026 19:19  
**Путь:** `/tmp/gsc-bac-scan/Flask-AppBuilder`  
**Всего находок:** 137  
**CRITICAL:** 5 | **HIGH:** 19 | **MEDIUM:** 15 | **LOW:** 97

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 80 |
| GS003 | 12 |
| GS011 | 6 |
| Хардкод IP адреса | 5 |
| CVE-2026-54696: Buffer overflow | 4 |
| GS004 | 4 |
| Python: File upload without content-type validation | 3 |
| Open redirect: user-supplied URL | 3 |
| CVE-2026-56318: Information disclosure | 3 |
| GS001 | 3 |
| Python: assert in production | 2 |
| CVE-2026-37270: Hardcoded credential | 2 |
| Rust: .clone() in hot path | 2 |
| SQL injection risk: f-string in query | 1 |
| Bare except: | 1 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 1 |
| World-readable file: .env (664) | 1 |
| World-readable file: docker-compose.yml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS005 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | swagger-ui-bundle.js | 2 | OWASP A03: Injection |
| CRITICAL | GS001 | swagger-ui-bundle.js | 2 | Found: Password:"),X?He.createElement(" |
| CRITICAL | GS001 | swagger-ui-bundle.js | 2 | Found: password:"),we?He.createElement(" |
| CRITICAL | GS001 | swagger-ui-bundle.js | 2 | Found: Password:"),s?He.createElement(" |
| CRITICAL | GS005 | migrate_db_1.3.py | 92 | Line 92: conn.execute("alter sequence %s rename to %s;" % (s |
| HIGH | ? | filemanager.py | 72 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | filemanager.py | 181 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | filemanager.py | 216 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 52 |  |
| HIGH | ? | swagger-ui-bundle.js | 2 | Match: !function webpackUniversalModuleDefinition(i,s){"obje |
| HIGH | ? | google_charts.js | 38 | Match:                         compressed:"build/yuiloader/y |
| HIGH | ? | google_charts.js | 39 | Match:                     "1.7.0.0":{uncompressed:"prototyp |
| HIGH | ? | tox.ini | 22 | Match:     SQLALCHEMY_DATABASE_URI = mysql://mysqluser:mysql |
| HIGH | ? | tox.ini | 32 | Match:     SQLALCHEMY_DATABASE_URI = postgresql+psycopg2://p |
| HIGH | ? | .env | 0 | Permissions 664 — should be 600 |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | cli.py | 417 | Line 417: os.popen( |
| HIGH | GS004 | cli.py | 423 | Line 423: os.popen("pybabel update -N -i {0} -d {1}".format( |
| HIGH | GS004 | cli.py | 438 | Line 438: os.popen("pybabel compile -f -d {0}".format(target |
| HIGH | GS004 | create_release.py | 60 | Line 60: output = subprocess.check_output( |
| HIGH | GS011 | config.py | 5 | Found JWT secret in code: '\2\1this...'. JWT secrets must be |
| HIGH | ? | swagger-ui-bundle.js | 2 | Clone in performance-critical code — consider references |
| HIGH | ? | ab_actions.js | 74 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | swagger-ui-bundle.js | 2 |
| M | ? | hash_db_password.py | 12 |
| M | ? | manager.py | 1083 |
| M | ? | manager.py | 1181 |
| H | ? | filemanager.py | 72 |
| H | ? | filemanager.py | 181 |
| H | ? | filemanager.py | 216 |
| M | ? | views.py | 623 |
| M | ? | views.py | 647 |
| M | ? | views.py | 813 |
| M | ? | views.py | 381 |
| M | ? | baseviews.py | 1045 |
| M | ? | baseviews.py | 1225 |
| M | ? | baseviews.py | 1315 |
| H | ? | utils.py | 52 |
| M | ? | config.py | 5 |
| M | ? | manager.py | 2260 |
| M | ? | registerviews.py | 102 |
| M | ? | manager.py | 2260 |
| M | ? | registerviews.py | 102 |
| C | GS001 | swagger-ui-bundle.js | 2 |
| C | GS001 | swagger-ui-bundle.js | 2 |
| C | GS001 | swagger-ui-bundle.js | 2 |
| L | GS003 | convert.py | 101 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS003 | swagger-ui-bundle.js | 2 |
| L | GS008 | config.py | 4 |
| L | GS008 | config.py | 7 |
| L | GS008 | config.py | 16 |
| L | GS008 | config.py | 19 |
| L | GS008 | config.py | 22 |
| L | GS008 | config.py | 23 |
| L | GS008 | config.py | 25 |
| L | GS008 | config.py | 27 |
| L | GS008 | config.py | 37 |
| L | GS008 | config.py | 38 |
| L | GS008 | config.py | 40 |
| L | GS008 | config.py | 41 |
| L | GS008 | config.py | 42 |
| L | GS008 | config.py | 43 |
| L | GS008 | const.py | 20 |
| L | GS008 | const.py | 22 |
| L | GS008 | const.py | 23 |
| L | GS008 | const.py | 25 |
| L | GS008 | const.py | 27 |
| L | GS008 | const.py | 29 |
| L | GS008 | const.py | 31 |
| L | GS008 | const.py | 33 |
| L | GS008 | const.py | 35 |
| L | GS008 | const.py | 37 |
| L | GS008 | const.py | 39 |
| L | GS008 | const.py | 42 |
| L | GS008 | const.py | 43 |
| L | GS008 | const.py | 44 |
| L | GS008 | const.py | 45 |
| L | GS008 | const.py | 46 |
| L | GS008 | const.py | 48 |
| L | GS008 | const.py | 50 |
| L | GS008 | const.py | 52 |
| L | GS008 | const.py | 54 |
| L | GS008 | const.py | 56 |
| L | GS008 | const.py | 58 |
| L | GS008 | const.py | 62 |
| L | GS008 | const.py | 64 |
| L | GS008 | const.py | 66 |
| L | GS008 | const.py | 68 |
| L | GS008 | const.py | 70 |
| L | GS008 | const.py | 72 |
| L | GS008 | const.py | 74 |
| L | GS008 | const.py | 77 |
| L | GS008 | const.py | 80 |
| L | GS008 | const.py | 82 |
| L | GS008 | const.py | 83 |
| L | GS008 | const.py | 84 |
| L | GS008 | const.py | 86 |
| L | GS008 | const.py | 88 |
| L | GS008 | const.py | 90 |
| L | GS008 | const.py | 92 |
| L | GS008 | const.py | 94 |
| L | GS008 | const.py | 96 |
| L | GS008 | const.py | 98 |
| L | GS008 | const.py | 100 |
| L | GS008 | const.py | 102 |
| L | GS008 | const.py | 104 |
| L | GS008 | const.py | 106 |
| L | GS008 | const.py | 109 |
| L | GS008 | const.py | 111 |
| L | GS008 | const.py | 113 |
| L | GS008 | const.py | 118 |
| L | GS008 | const.py | 120 |
| L | GS008 | const.py | 123 |
| L | GS008 | const.py | 125 |
| L | GS008 | const.py | 127 |
| L | GS008 | const.py | 129 |
| L | GS008 | const.py | 131 |
| L | GS008 | const.py | 134 |
| L | GS008 | const.py | 138 |
| L | GS008 | const.py | 142 |
| L | GS008 | const.py | 145 |
| L | GS008 | const.py | 146 |
| L | GS008 | const.py | 147 |
| L | GS008 | const.py | 148 |
| L | GS008 | const.py | 149 |
| L | GS008 | const.py | 156 |
| L | GS008 | const.py | 157 |
| L | GS008 | const.py | 158 |
| H | ? | swagger-ui-bundle.js | 2 |
| H | ? | google_charts.js | 38 |
| H | ? | google_charts.js | 39 |
| H | ? | tox.ini | 22 |
| H | ? | tox.ini | 32 |
| H | ? | .env | 0 |
| H | ? | docker-compose.yml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | cli.py | 417 |
| H | GS004 | cli.py | 423 |
| H | GS004 | cli.py | 438 |
| H | GS004 | create_release.py | 60 |
| C | GS005 | migrate_db_1.3.py | 92 |
| s | GS009 |  | 0 |
| H | GS011 | config.py | 5 |
| L | GS011 | manager.py | 780 |
| L | GS011 | manager.py | 790 |
| L | GS011 | manager.py | 804 |
| L | GS011 | manager.py | 810 |
| L | GS011 | views.py | 756 |
| H | ? | swagger-ui-bundle.js | 2 |
| H | ? | ab_actions.js | 74 |

---
*Сгенерировано GSC v0.6 · 2026-07-28T19:19:44.330123*