---
title: "GSC Audit: /tmp/gsc-learn/peewee"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/peewee

**Дата:** 05.08.2026 04:04  
**Путь:** `/tmp/gsc-learn/peewee`  
**Всего находок:** 223  
**CRITICAL:** 7 | **HIGH:** 40 | **MEDIUM:** 21 | **LOW:** 67

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS007 | 36 |
| GS020 | 25 |
| GS022 | 22 |
| GS021 | 17 |
| Rust: .clone() in hot path | 14 |
| Bare except: | 8 |
| Python: assert in production | 8 |
| GS003 | 7 |
| GS018 | 6 |
| GS005 | 5 |
| CVE-2026-37270: Hardcoded credential | 4 |
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
| CRITICAL | ? | shortcuts.py | 287 | Match: def resolve_multimodel_query(query, key='_model_ident |
| CRITICAL | ? | fields.py | 50 | Match:             return pickle.loads(value) |
| CRITICAL | GS005 | peewee.py | 4216 | Line 4216: cursor.execute('ATTACH DATABASE "%s" AS "%s"' % ( |
| CRITICAL | GS005 | peewee.py | 5032 | Line 5032: curs.execute('SET TRANSACTION ISOLATION LEVEL %s' |
| CRITICAL | GS005 | apsw_ext.py | 101 | Line 101: self.cursor().execute('begin %s;' % lock_type) |
| CRITICAL | GS005 | cockroachdb.py | 144 | Line 144: self.cursor().execute('SET TRANSACTION PRIORITY %s |
| CRITICAL | GS005 | pwasyncio.py | 848 | Line 848: await conn.execute('ATTACH DATABASE "%s" AS "%s"'  |
| HIGH | ? | peewee.py | 7796 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | signals.py | 71 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | .travis.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS007 | bench.py | 67 | Line 67: Register.insert_many(data, fields=[Register.value]) |
| HIGH | GS007 | bench.py | 70 | Line 70: def bulk_create(i): |
| HIGH | GS007 | bench.py | 73 | Line 73: Register.bulk_create(data, batch_size=100) |
| HIGH | GS007 | bench.py | 144 | Line 144: bulk_create() |
| HIGH | GS007 | peewee.py | 7766 | Line 7766: def insert_many(cls, rows, fields=None): |
| HIGH | GS007 | peewee.py | 7782 | Line 7782: .insert_many(rows=rows, fields=fields) |
| HIGH | GS007 | peewee.py | 7800 | Line 7800: def bulk_create(cls, model_list, batch_size=None) |
| HIGH | GS007 | peewee.py | 7828 | Line 7828: res = cls.insert_many(accum, fields=fields).execu |
| HIGH | GS007 | peewee.py | 7835 | Line 7835: def bulk_update(cls, model_list, fields, batch_si |
| HIGH | GS007 | peewee.py | 7837 | Line 7837: raise ValueError('bulk_update() is not supported  |
| HIGH | GS007 | peewee.py | 8855 | Line 8855: accessor.through_model.insert_many(inserts).execu |
| HIGH | GS007 | kv.py | 135 | Line 135: .insert_many(list(mapping.items()), |
| HIGH | GS007 | kv.py | 144 | Line 144: .insert_many(list(mapping.items()), |
| HIGH | GS014 | peewee.py | 4558 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | cockroachdb.py | 62 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | flask_utils.py | 99 | Database URL contains password in plaintext. Use environment |
| HIGH | GS018 | peewee.py | 4037 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | peewee.py | 4386 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | peewee.py | 5261 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | peewee.py | 5305 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | apsw_ext.py | 111 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | pwasyncio.py | 1143 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | ? | peewee.py | 796 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 803 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 915 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 1161 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 1191 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 1197 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 1963 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 2127 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 2575 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8444 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8702 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8705 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8710 | Clone in performance-critical code — consider references |
| HIGH | ? | peewee.py | 8738 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | apsw_ext.py | 50 |
| M | ? | sqlite_udf.py | 168 |
| M | ? | sqlite_udf.py | 238 |
| M | ? | sqlite_udf.py | 256 |
| M | ? | pool.py | 292 |
| M | ? | sqlite_ext.py | 652 |
| M | ? | sqlite_ext.py | 656 |
| M | ? | sqlcipher_ext.py | 75 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| L | ? | peewee.py | 133 |
| M | ? | peewee.py | 238 |
| M | ? | peewee.py | 245 |
| M | ? | flask_utils.py | 184 |
| M | ? | sqlite_changelog.py | 85 |
| M | ? | sqlite_changelog.py | 98 |
| M | ? | bench.py | 139 |
| M | ? | bench.py | 142 |
| M | ? | bench.py | 145 |
| H | ? | peewee.py | 7796 |
| H | ? | signals.py | 71 |
| M | ? | fields.py | 50 |
| M | ? | peewee.py | 4221 |
| M | ? | shortcuts.py | 287 |
| M | ? | sqlcipher_ext.py | 73 |
| M | ? | sqlcipher_ext.py | 92 |
| L | GS003 | bench.py | 38 |
| L | GS003 | reflection.py | 882 |
| L | GS003 | reflection.py | 895 |
| L | GS003 | reflection.py | 901 |
| L | GS003 | reflection.py | 918 |
| L | GS003 | reflection.py | 935 |
| L | GS003 | runtests.py | 123 |
| L | GS008 | postgres_ext.py | 51 |
| i | GS020 |  | 4 |
| i | GS020 |  | 9 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 3 |
| i | GS020 |  | 4 |
| i | GS020 |  | 3 |
| i | GS020 |  | 2 |
| i | GS020 |  | 3 |
| i | GS020 |  | 4 |
| i | GS020 |  | 509 |
| i | GS020 |  | 644 |
| C | ? | shortcuts.py | 287 |
| C | ? | fields.py | 50 |
| H | ? | .travis.yml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| C | GS005 | peewee.py | 4216 |
| C | GS005 | peewee.py | 5032 |
| C | GS005 | apsw_ext.py | 101 |
| C | GS005 | cockroachdb.py | 144 |
| C | GS005 | pwasyncio.py | 848 |
| H | GS007 | bench.py | 67 |
| H | GS007 | bench.py | 70 |
| H | GS007 | bench.py | 73 |
| H | GS007 | bench.py | 144 |
| I | GS007 | peewee.py | 4814 |
| I | GS007 | peewee.py | 4927 |
| I | GS007 | peewee.py | 4928 |
| I | GS007 | peewee.py | 5087 |
| I | GS007 | peewee.py | 5580 |
| I | GS007 | peewee.py | 5689 |
| I | GS007 | peewee.py | 5720 |
| I | GS007 | peewee.py | 7289 |
| I | GS007 | peewee.py | 7472 |
| I | GS007 | peewee.py | 7473 |
| I | GS007 | peewee.py | 7807 |
| I | GS007 | peewee.py | 7883 |
| I | GS007 | peewee.py | 7994 |
| I | GS007 | peewee.py | 8008 |
| I | GS007 | peewee.py | 8814 |
| I | GS007 | peewee.py | 4679 |
| I | GS007 | peewee.py | 4680 |
| H | GS007 | peewee.py | 7766 |
| H | GS007 | peewee.py | 7782 |
| H | GS007 | peewee.py | 7800 |
| H | GS007 | peewee.py | 7828 |
| H | GS007 | peewee.py | 7835 |
| H | GS007 | peewee.py | 7837 |
| H | GS007 | peewee.py | 8855 |
| I | GS007 | cockroachdb.py | 32 |
| I | GS007 | cysqlite_ext.py | 13 |
| H | GS007 | kv.py | 135 |
| H | GS007 | kv.py | 144 |
| I | GS007 | sqlite_ext.py | 24 |
| I | GS007 | sqlite_ext.py | 38 |
| I | GS007 | sqlite_ext.py | 40 |
| I | GS007 | sqlite_ext.py | 41 |
| s | GS009 |  | 0 |
| H | GS014 | peewee.py | 4558 |
| H | GS014 | cockroachdb.py | 62 |
| H | GS014 | flask_utils.py | 99 |
| H | GS018 | peewee.py | 4037 |
| H | GS018 | peewee.py | 4386 |
| H | GS018 | peewee.py | 5261 |
| H | GS018 | peewee.py | 5305 |
| H | GS018 | apsw_ext.py | 111 |
| H | GS018 | pwasyncio.py | 1143 |
| s | GS021 |  | 4 |
| s | GS021 |  | 44 |
| s | GS021 |  | 44 |
| s | GS021 |  | 49 |
| s | GS021 |  | 55 |
| s | GS021 |  | 55 |
| s | GS021 |  | 1164 |
| c | GS021 |  | 175 |
| c | GS021 |  | 200 |
| c | GS021 |  | 251 |
| c | GS021 |  | 266 |
| c | GS021 |  | 279 |
| c | GS021 |  | 143 |
| c | GS021 |  | 159 |
| c | GS021 |  | 207 |
| c | GS021 |  | 227 |
| s | GS021 |  | 256 |
| r | GS022 |  | 3 |
| r | GS022 |  | 8 |
| r | GS022 |  | 57 |
| r | GS022 |  | 1647 |
| r | GS022 |  | 1 |
| r | GS022 |  | 72 |
| r | GS022 |  | 76 |
| r | GS022 |  | 10 |
| r | GS022 |  | 183 |
| r | GS022 |  | 9 |
| r | GS022 |  | 25 |
| r | GS022 |  | 96 |
| r | GS022 |  | 26 |
| r | GS022 |  | 62 |
| r | GS022 |  | 63 |
| r | GS022 |  | 80 |
| r | GS022 |  | 106 |
| r | GS022 |  | 110 |
| r | GS022 |  | 118 |
| r | GS022 |  | 58 |
| r | GS022 |  | 145 |
| r | GS022 |  | 145 |
| H | ? | peewee.py | 796 |
| H | ? | peewee.py | 803 |
| H | ? | peewee.py | 915 |
| H | ? | peewee.py | 1161 |
| H | ? | peewee.py | 1191 |
| H | ? | peewee.py | 1197 |
| H | ? | peewee.py | 1963 |
| H | ? | peewee.py | 2127 |
| H | ? | peewee.py | 2575 |
| H | ? | peewee.py | 8444 |
| H | ? | peewee.py | 8702 |
| H | ? | peewee.py | 8705 |
| H | ? | peewee.py | 8710 |
| H | ? | peewee.py | 8738 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T04:04:40.935413*