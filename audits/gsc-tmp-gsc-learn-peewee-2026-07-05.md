---
title: "GSC Audit: /tmp/gsc-learn/peewee"
date: 2026-07-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/peewee

**Дата:** 05.07.2026 04:00  
**Путь:** `/tmp/gsc-learn/peewee`  
**Всего находок:** 112  
**CRITICAL:** 7 | **HIGH:** 19 | **MEDIUM:** 18 | **LOW:** 67

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 12 |
| Bare except: | 9 |
| Python: assert in production | 8 |
| GS003 | 7 |
| GS005 | 5 |
| GS014 | 3 |
| Python: File upload without content-type validation | 2 |
| Generic code smell #24 | 1 |
| Generic code smell #27 | 1 |
| Generic code smell #30 | 1 |
| Generic code smell #33 | 1 |
| Generic code smell #36 | 1 |
| Generic code smell #39 | 1 |
| Generic code smell #42 | 1 |
| Generic code smell #45 | 1 |
| Generic code smell #48 | 1 |
| Generic code smell #51 | 1 |
| Generic code smell #54 | 1 |
| Generic code smell #57 | 1 |
| Generic code smell #60 | 1 |
| Generic code smell #63 | 1 |
| Generic code smell #66 | 1 |
| Generic code smell #69 | 1 |
| Generic code smell #72 | 1 |
| Generic code smell #75 | 1 |
| Generic code smell #78 | 1 |
| Generic code smell #81 | 1 |
| Generic code smell #84 | 1 |
| Generic code smell #87 | 1 |
| Generic code smell #90 | 1 |
| Generic code smell #93 | 1 |
| Generic code smell #96 | 1 |
| Generic code smell #99 | 1 |
| Generic code smell #102 | 1 |
| Generic code smell #105 | 1 |
| Generic code smell #108 | 1 |
| Generic code smell #111 | 1 |
| Generic code smell #114 | 1 |
| Generic code smell #117 | 1 |
| Generic code smell #120 | 1 |
| Generic code smell #123 | 1 |
| Generic code smell #126 | 1 |
| Generic code smell #129 | 1 |
| Generic code smell #132 | 1 |
| Generic code smell #135 | 1 |
| Generic code smell #138 | 1 |
| Generic code smell #141 | 1 |
| Generic code smell #144 | 1 |
| Generic code smell #147 | 1 |
| Generic code smell #150 | 1 |
| Generic code smell #153 | 1 |
| Generic code smell #156 | 1 |
| Generic code smell #159 | 1 |
| Generic code smell #162 | 1 |
| Generic code smell #165 | 1 |
| Generic code smell #168 | 1 |
| Generic code smell #171 | 1 |
| Generic code smell #174 | 1 |
| Generic code smell #177 | 1 |
| Generic code smell #180 | 1 |
| Generic code smell #183 | 1 |
| Generic code smell #186 | 1 |
| Generic code smell #189 | 1 |
| Generic code smell #192 | 1 |
| Generic code smell #195 | 1 |
| Generic code smell #198 | 1 |
| CVE-2026-55223: Insecure deserialization | 1 |
| GS008 | 1 |
| Hardcoded encryption key | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: .travis.yml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | shortcuts.py | 286 | Match: def resolve_multimodel_query(query, key='_model_ident |
| CRITICAL | ? | fields.py | 49 | Match:             return pickle.loads(value) |
| CRITICAL | GS005 | peewee.py | 4061 | Line 4061: cursor.execute('ATTACH DATABASE "%s" AS "%s"' % ( |
| CRITICAL | GS005 | peewee.py | 4865 | Line 4865: curs.execute('SET TRANSACTION ISOLATION LEVEL %s' |
| CRITICAL | GS005 | apsw_ext.py | 110 | Line 110: self.cursor().execute('begin %s;' % lock_type) |
| CRITICAL | GS005 | cockroachdb.py | 150 | Line 150: self.cursor().execute('SET TRANSACTION PRIORITY %s |
| CRITICAL | GS005 | pwasyncio.py | 781 | Line 781: await conn.execute('ATTACH DATABASE "%s" AS "%s"'  |
| HIGH | ? | signals.py | 71 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | peewee.py | 7656 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | .travis.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS014 | peewee.py | 4410 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | cockroachdb.py | 68 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | flask_utils.py | 111 | Database URL contains password in plaintext. Use environment |
| HIGH | ? | peewee.py | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 764 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 1145 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 1150 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 1917 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 2080 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 2463 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8308 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8554 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8557 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8562 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8591 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | sqlcipher_ext.py | 75 |
| M | ? | sqlite_ext.py | 655 |
| M | ? | sqlite_ext.py | 659 |
| M | ? | pool.py | 257 |
| M | ? | pool.py | 282 |
| M | ? | sqlite_udf.py | 174 |
| M | ? | sqlite_udf.py | 244 |
| M | ? | sqlite_udf.py | 262 |
| M | ? | apsw_ext.py | 52 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| L | ? | peewee.py | 132 |
| M | ? | bench.py | 139 |
| M | ? | bench.py | 142 |
| M | ? | bench.py | 145 |
| M | ? | sqlite_changelog.py | 85 |
| M | ? | sqlite_changelog.py | 98 |
| M | ? | flask_utils.py | 196 |
| M | ? | peewee.py | 242 |
| M | ? | peewee.py | 249 |
| H | ? | signals.py | 71 |
| H | ? | peewee.py | 7656 |
| M | ? | fields.py | 49 |
| L | GS003 | bench.py | 38 |
| L | GS003 | reflection.py | 892 |
| L | GS003 | reflection.py | 905 |
| L | GS003 | reflection.py | 911 |
| L | GS003 | reflection.py | 928 |
| L | GS003 | reflection.py | 945 |
| L | GS003 | runtests.py | 123 |
| L | GS008 | postgres_ext.py | 52 |
| C | ? | shortcuts.py | 286 |
| C | ? | fields.py | 49 |
| H | ? | .travis.yml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| C | GS005 | peewee.py | 4061 |
| C | GS005 | peewee.py | 4865 |
| C | GS005 | apsw_ext.py | 110 |
| C | GS005 | cockroachdb.py | 150 |
| C | GS005 | pwasyncio.py | 781 |
| s | GS009 |  | 0 |
| H | GS014 | peewee.py | 4410 |
| H | GS014 | cockroachdb.py | 68 |
| H | GS014 | flask_utils.py | 111 |
| H | ? | peewee.py | 757 |
| H | ? | peewee.py | 764 |
| H | ? | peewee.py | 1145 |
| H | ? | peewee.py | 1150 |
| H | ? | peewee.py | 1917 |
| H | ? | peewee.py | 2080 |
| H | ? | peewee.py | 2463 |
| H | ? | peewee.py | 8308 |
| H | ? | peewee.py | 8554 |
| H | ? | peewee.py | 8557 |
| H | ? | peewee.py | 8562 |
| H | ? | peewee.py | 8591 |

---
*Сгенерировано GSC v0.6 · 2026-07-05T04:00:39.951808*