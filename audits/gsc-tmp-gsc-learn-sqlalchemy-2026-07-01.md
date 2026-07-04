---
title: "GSC Audit: /tmp/gsc-learn/sqlalchemy"
date: 2026-07-01
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/sqlalchemy

**Дата:** 01.07.2026 04:08  
**Путь:** `/tmp/gsc-learn/sqlalchemy`  
**Всего находок:** 1422  
**CRITICAL:** 119 | **HIGH:** 70 | **MEDIUM:** 679 | **LOW:** 553

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 646 |
| GS003 | 86 |
| Hardcoded encryption key | 63 |
| GS008 | 36 |
| GS001 | 33 |
| Bare except: | 29 |
| GS004 | 21 |
| Хардкод IP адреса | 20 |
| GS012 | 18 |
| eval() or exec() usage | 13 |
| SQL injection risk: f-string in query | 9 |
| GS005 | 9 |
| GS014 | 9 |
| Generic code smell #24 | 7 |
| Generic code smell #27 | 7 |
| Generic code smell #30 | 7 |
| Generic code smell #33 | 7 |
| Generic code smell #36 | 7 |
| Generic code smell #39 | 7 |
| Generic code smell #42 | 7 |
| Generic code smell #45 | 7 |
| Generic code smell #48 | 7 |
| Generic code smell #51 | 7 |
| Generic code smell #54 | 7 |
| Generic code smell #57 | 7 |
| Generic code smell #60 | 7 |
| Generic code smell #63 | 7 |
| Generic code smell #66 | 7 |
| Generic code smell #69 | 7 |
| Generic code smell #72 | 7 |
| Generic code smell #75 | 7 |
| Generic code smell #78 | 7 |
| Generic code smell #81 | 7 |
| Generic code smell #84 | 7 |
| Generic code smell #87 | 7 |
| Generic code smell #90 | 7 |
| Generic code smell #93 | 7 |
| Generic code smell #96 | 7 |
| Generic code smell #99 | 7 |
| Generic code smell #102 | 7 |
| Generic code smell #105 | 7 |
| Generic code smell #108 | 7 |
| Generic code smell #111 | 7 |
| Generic code smell #114 | 7 |
| Generic code smell #117 | 7 |
| Generic code smell #120 | 7 |
| Generic code smell #123 | 7 |
| Generic code smell #126 | 7 |
| Generic code smell #129 | 7 |
| Generic code smell #132 | 7 |
| Generic code smell #135 | 7 |
| Generic code smell #138 | 7 |
| Generic code smell #141 | 7 |
| Generic code smell #144 | 7 |
| Generic code smell #147 | 7 |
| Generic code smell #150 | 7 |
| Generic code smell #153 | 7 |
| Generic code smell #156 | 7 |
| Generic code smell #159 | 7 |
| Generic code smell #162 | 7 |
| Generic code smell #165 | 7 |
| Generic code smell #168 | 7 |
| Generic code smell #171 | 7 |
| Generic code smell #174 | 7 |
| Generic code smell #177 | 7 |
| Generic code smell #180 | 7 |
| Generic code smell #183 | 7 |
| Generic code smell #186 | 7 |
| Generic code smell #189 | 7 |
| Generic code smell #192 | 7 |
| Generic code smell #195 | 7 |
| Generic code smell #198 | 7 |
| Postgres URL with password | 6 |
| pickle.load() — unsafe deserialization | 5 |
| Outdated dependency pattern | 2 |
| Синхронный код в async | 2 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | compiler.py | 5737 | OWASP A03: Injection |
| CRITICAL | ? | compiler.py | 6441 | OWASP A03: Injection |
| CRITICAL | ? | crud.py | 373 | OWASP A03: Injection |
| CRITICAL | ? | crud.py | 475 | OWASP A03: Injection |
| CRITICAL | ? | crud.py | 690 | OWASP A03: Injection |
| CRITICAL | ? | base.py | 1530 | OWASP A03: Injection |
| CRITICAL | ? | base.py | 1533 | OWASP A03: Injection |
| CRITICAL | ? | base.py | 2300 | OWASP A03: Injection |
| CRITICAL | ? | persistence.py | 1112 | OWASP A03: Injection |
| CRITICAL | GS001 | pyodbc.py | 80 | Found: password="tiger" |
| CRITICAL | GS001 | pyodbc.py | 215 | Found: password="tiger" |
| CRITICAL | GS001 | pyodbc.py | 245 | Found: password="tiger" |
| CRITICAL | GS001 | mysqldb.py | 204 | Found: password="passwd" |
| CRITICAL | GS001 | cx_oracle.py | 192 | Found: password="tiger" |
| CRITICAL | GS001 | cx_oracle.py | 236 | Found: password="tiger" |
| CRITICAL | GS001 | oracledb.py | 267 | Found: password="tiger" |
| CRITICAL | GS001 | oracledb.py | 309 | Found: password="tiger" |
| CRITICAL | GS001 | oracledb.py | 341 | Found: password="tiger" |
| CRITICAL | GS001 | psycopg.py | 21 | Found: postgresql://`` dialect
 |
| CRITICAL | GS001 | aiosqlite.py | 14 | Found: sqlite:///file_path
    :url: http |
| CRITICAL | GS001 | base.py | 226 | Found: sqlite:///myfile.db |
| CRITICAL | GS001 | base.py | 234 | Found: sqlite:///myfile.db |
| CRITICAL | GS001 | base.py | 243 | Found: sqlite:///myfile.db |
| CRITICAL | GS001 | base.py | 263 | Found: sqlite:///myfile.db |
| CRITICAL | GS001 | base.py | 283 | Found: sqlite:///myfile.db |
| CRITICAL | GS001 | base.py | 314 | Found: sqlite:///myfile.db |
| CRITICAL | GS001 | provision.py | 78 | Found: password="test" |
| CRITICAL | GS001 | pysqlite.py | 13 | Found: sqlite:///file_path
    :url: http |
| CRITICAL | GS001 | pysqlite.py | 41 | Found: sqlite:///path/to/databa |
| CRITICAL | GS001 | pysqlite.py | 47 | Found: sqlite:////path/to/databa |
| CRITICAL | GS001 | pysqlite.py | 56 | Found: sqlite:///:memory:``. It |
| CRITICAL | GS001 | pysqlite.py | 57 | Found: sqlite://`` and nothing el |
| CRITICAL | GS001 | pysqlite.py | 77 | Found: sqlite:///file:path/to/databa |
| CRITICAL | GS001 | pysqlite.py | 94 | Found: sqlite:///file:path/to/databa |
| CRITICAL | GS001 | pysqlite.py | 254 | Found: sqlite:///myfile.db |
| CRITICAL | GS001 | pysqlite.py | 380 | Found: sqlite:///./db_file |
| CRITICAL | GS001 | scoping.py | 822 | Found: sqlite:///leader.db |
| CRITICAL | GS001 | scoping.py | 824 | Found: sqlite:///follower1.db |
| CRITICAL | GS001 | scoping.py | 825 | Found: sqlite:///follower2.db |
| CRITICAL | GS001 | setup.cfg | 24 | Found: sqlite:///:memory:
 |
| CRITICAL | GS001 | setup.cfg | 25 | Found: sqlite:///:memory:
 |
| CRITICAL | GS001 | setup.cfg | 28 | Found: sqlite:///:memory:
 |
| CRITICAL | ? | associationproxy.py | 413 | Match:         self.key = "_%s_%s_%s" % ( |
| CRITICAL | ? | information_schema.py | 55 | Match:     Column("CATALOG_NAME", CoerceUnicode, key="catalo |
| CRITICAL | ? | information_schema.py | 56 | Match:     Column("SCHEMA_NAME", CoerceUnicode, key="schema_ |
| CRITICAL | ? | information_schema.py | 57 | Match:     Column("SCHEMA_OWNER", CoerceUnicode, key="schema |
| CRITICAL | ? | information_schema.py | 64 | Match:     Column("TABLE_CATALOG", CoerceUnicode, key="table |
| CRITICAL | ? | information_schema.py | 65 | Match:     Column("TABLE_SCHEMA", CoerceUnicode, key="table_ |
| CRITICAL | ? | information_schema.py | 66 | Match:     Column("TABLE_NAME", CoerceUnicode, key="table_na |
| CRITICAL | ? | information_schema.py | 67 | Match:     Column("TABLE_TYPE", CoerceUnicode, key="table_ty |
| CRITICAL | ? | information_schema.py | 74 | Match:     Column("TABLE_SCHEMA", CoerceUnicode, key="table_ |
| CRITICAL | ? | information_schema.py | 75 | Match:     Column("TABLE_NAME", CoerceUnicode, key="table_na |
| CRITICAL | ? | information_schema.py | 76 | Match:     Column("COLUMN_NAME", CoerceUnicode, key="column_ |
| CRITICAL | ? | information_schema.py | 77 | Match:     Column("IS_NULLABLE", Integer, key="is_nullable") |
| CRITICAL | ? | information_schema.py | 78 | Match:     Column("DATA_TYPE", String, key="data_type"), |
| CRITICAL | ? | information_schema.py | 79 | Match:     Column("ORDINAL_POSITION", Integer, key="ordinal_ |
| CRITICAL | ? | information_schema.py | 81 | Match:         "CHARACTER_MAXIMUM_LENGTH", Integer, key="cha |
| CRITICAL | ? | information_schema.py | 83 | Match:     Column("NUMERIC_PRECISION", Integer, key="numeric |
| CRITICAL | ? | information_schema.py | 84 | Match:     Column("NUMERIC_SCALE", Integer, key="numeric_sca |
| CRITICAL | ? | information_schema.py | 85 | Match:     Column("COLUMN_DEFAULT", Integer, key="column_def |
| CRITICAL | ? | information_schema.py | 86 | Match:     Column("COLLATION_NAME", String, key="collation_n |
| CRITICAL | ? | information_schema.py | 111 | Match:     Column("system_type_id", Integer, key="system_typ |
| CRITICAL | ? | information_schema.py | 112 | Match:     Column("user_type_id", Integer, key="user_type_id |
| CRITICAL | ? | information_schema.py | 113 | Match:     Column("schema_id", Integer, key="schema_id"), |
| CRITICAL | ? | information_schema.py | 114 | Match:     Column("max_length", Integer, key="max_length"), |
| CRITICAL | ? | information_schema.py | 115 | Match:     Column("precision", Integer, key="precision"), |
| CRITICAL | ? | information_schema.py | 117 | Match:     Column("collation_name", CoerceUnicode, key="coll |
| CRITICAL | ? | information_schema.py | 118 | Match:     Column("is_nullable", Boolean, key="is_nullable") |
| CRITICAL | ? | information_schema.py | 119 | Match:     Column("is_user_defined", Boolean, key="is_user_d |
| CRITICAL | ? | information_schema.py | 120 | Match:     Column("is_assembly_type", Boolean, key="is_assem |
| CRITICAL | ? | information_schema.py | 121 | Match:     Column("default_object_id", Integer, key="default |
| CRITICAL | ? | information_schema.py | 122 | Match:     Column("rule_object_id", Integer, key="rule_objec |
| CRITICAL | ? | information_schema.py | 123 | Match:     Column("is_table_type", Boolean, key="is_table_ty |
| CRITICAL | ? | information_schema.py | 130 | Match:     Column("TABLE_SCHEMA", CoerceUnicode, key="table_ |
| CRITICAL | ? | information_schema.py | 131 | Match:     Column("TABLE_NAME", CoerceUnicode, key="table_na |
| CRITICAL | ? | information_schema.py | 132 | Match:     Column("CONSTRAINT_NAME", CoerceUnicode, key="con |
| CRITICAL | ? | information_schema.py | 133 | Match:     Column("CONSTRAINT_TYPE", CoerceUnicode, key="con |
| CRITICAL | ? | information_schema.py | 151 | Match:     Column("TABLE_SCHEMA", CoerceUnicode, key="table_ |
| CRITICAL | ? | information_schema.py | 152 | Match:     Column("TABLE_NAME", CoerceUnicode, key="table_na |
| CRITICAL | ? | information_schema.py | 153 | Match:     Column("COLUMN_NAME", CoerceUnicode, key="column_ |
| CRITICAL | ? | information_schema.py | 154 | Match:     Column("CONSTRAINT_NAME", CoerceUnicode, key="con |
| CRITICAL | ? | information_schema.py | 161 | Match:     Column("TABLE_SCHEMA", CoerceUnicode, key="table_ |
| CRITICAL | ? | information_schema.py | 162 | Match:     Column("TABLE_NAME", CoerceUnicode, key="table_na |
| CRITICAL | ? | information_schema.py | 163 | Match:     Column("COLUMN_NAME", CoerceUnicode, key="column_ |
| CRITICAL | ? | information_schema.py | 164 | Match:     Column("CONSTRAINT_NAME", CoerceUnicode, key="con |
| CRITICAL | ? | information_schema.py | 165 | Match:     Column("CONSTRAINT_SCHEMA", CoerceUnicode, key="c |
| CRITICAL | ? | information_schema.py | 166 | Match:     Column("ORDINAL_POSITION", Integer, key="ordinal_ |
| CRITICAL | ? | information_schema.py | 173 | Match:     Column("CONSTRAINT_CATALOG", CoerceUnicode, key=" |
| CRITICAL | ? | information_schema.py | 174 | Match:     Column("CONSTRAINT_SCHEMA", CoerceUnicode, key="c |
| CRITICAL | ? | information_schema.py | 175 | Match:     Column("CONSTRAINT_NAME", CoerceUnicode, key="con |
| CRITICAL | ? | information_schema.py | 180 | Match:         key="unique_constraint_catalog", |
| CRITICAL | ? | information_schema.py | 185 | Match:         key="unique_constraint_schema", |
| CRITICAL | ? | information_schema.py | 188 | Match:         "UNIQUE_CONSTRAINT_NAME", CoerceUnicode, key= |
| CRITICAL | ? | information_schema.py | 190 | Match:     Column("MATCH_OPTION", String, key="match_option" |
| CRITICAL | ? | information_schema.py | 191 | Match:     Column("UPDATE_RULE", String, key="update_rule"), |
| CRITICAL | ? | information_schema.py | 192 | Match:     Column("DELETE_RULE", String, key="delete_rule"), |
| CRITICAL | ? | information_schema.py | 199 | Match:     Column("TABLE_CATALOG", CoerceUnicode, key="table |
| CRITICAL | ? | information_schema.py | 200 | Match:     Column("TABLE_SCHEMA", CoerceUnicode, key="table_ |
| CRITICAL | ? | information_schema.py | 201 | Match:     Column("TABLE_NAME", CoerceUnicode, key="table_na |
| CRITICAL | ? | information_schema.py | 202 | Match:     Column("VIEW_DEFINITION", CoerceUnicode, key="vie |
| CRITICAL | ? | information_schema.py | 203 | Match:     Column("CHECK_OPTION", String, key="check_option" |
| CRITICAL | ? | information_schema.py | 204 | Match:     Column("IS_UPDATABLE", String, key="is_updatable" |
| CRITICAL | ? | information_schema.py | 223 | Match:     Column("SEQUENCE_CATALOG", CoerceUnicode, key="se |
| CRITICAL | ? | information_schema.py | 224 | Match:     Column("SEQUENCE_SCHEMA", CoerceUnicode, key="seq |
| CRITICAL | ? | information_schema.py | 225 | Match:     Column("SEQUENCE_NAME", CoerceUnicode, key="seque |
| CRITICAL | ? | sqltypes.py | 1991 | Match:     ``pickle.dumps()`` to incoming objects, and ``pic |
| CRITICAL | ? | serializer.py | 149 | Match:                 cls = pickle.loads(b64decode(clsarg)) |
| CRITICAL | ? | serializer.py | 152 | Match:                 cls = pickle.loads(b64decode(args)) |
| CRITICAL | ? | serializer.py | 155 | Match:                 cls = pickle.loads(b64decode(args)) |
| CRITICAL | ? | serializer.py | 159 | Match:                 cls = pickle.loads(b64decode(mapper)) |
| CRITICAL | GS005 | base.py | 3270 | Line 3270: cursor.execute(f"SET TRANSACTION ISOLATION LEVEL  |
| CRITICAL | GS005 | base.py | 2852 | Line 2852: cursor.execute(f"SET SESSION TRANSACTION ISOLATIO |
| CRITICAL | GS005 | mysqldb.py | 179 | Line 179: cursor.execute("SET NAMES %s" % charset_name) |
| CRITICAL | GS005 | provision.py | 277 | Line 277: cursor.execute("ALTER SESSION SET CURRENT_SCHEMA=% |
| CRITICAL | GS005 | base.py | 364 | Line 364: cursor.execute("SET SESSION search_path='%s'" % sc |
| CRITICAL | GS005 | pg8000.py | 592 | Line 592: cursor.execute(f""" |
| CRITICAL | GS005 | provision.py | 89 | Line 89: cursor.execute("SET SESSION search_path='%s'" % sch |
| CRITICAL | GS005 | provision.py | 182 | Line 182: text(f"CREATE EXTENSION IF NOT EXISTS {extension}" |
| CRITICAL | GS005 | base.py | 3079 | Line 3079: cursor.execute("use %s" % shards[shard_id]) |
| HIGH | ? | engines.py | 33 | Redteam Kit |
| HIGH | ? | automap.py | 150 | Redteam Kit |
| HIGH | ? | automap.py | 180 | Redteam Kit |
| HIGH | ? | psycopg.py | 81 | Redteam Kit |
| HIGH | ? | psycopg.py | 103 | Redteam Kit |
| HIGH | ? | base.py | 195 | Redteam Kit |
| HIGH | ? | setup.cfg | 32 | Match: postgresql = postgresql+psycopg://scott:tiger@127.0.0 |
| HIGH | ? | setup.cfg | 33 | Match: psycopg2 = postgresql+psycopg2://scott:tiger@127.0.0. |
| HIGH | ? | setup.cfg | 34 | Match: psycopg = postgresql+psycopg://scott:tiger@127.0.0.1: |
| HIGH | ? | setup.cfg | 35 | Match: psycopg_async = postgresql+psycopg_async://scott:tige |
| HIGH | ? | setup.cfg | 36 | Match: asyncpg = postgresql+asyncpg://scott:tiger@127.0.0.1: |
| HIGH | ? | setup.cfg | 37 | Match: pg8000 = postgresql+pg8000://scott:tiger@127.0.0.1:54 |
| HIGH | ? | setup.cfg | 38 | Match: postgresql_psycopg2cffi = postgresql+psycopg2cffi://s |
| HIGH | ? | setup.cfg | 39 | Match: mysql = mysql+mysqldb://scott:tiger@127.0.0.1:3306/te |
| HIGH | ? | setup.cfg | 40 | Match: pymysql = mysql+pymysql://scott:tiger@127.0.0.1:3306/ |
| HIGH | ? | setup.cfg | 41 | Match: aiomysql = mysql+aiomysql://scott:tiger@127.0.0.1:330 |
| HIGH | ? | setup.cfg | 42 | Match: asyncmy = mysql+asyncmy://scott:tiger@127.0.0.1:3306/ |
| HIGH | ? | setup.cfg | 43 | Match: mariadb = mariadb+mysqldb://scott:tiger@127.0.0.1:330 |
| HIGH | ? | setup.cfg | 44 | Match: mariadb_connector = mariadb+mariadbconnector://scott: |
| HIGH | ? | setup.cfg | 45 | Match: mysql_connector = mariadb+mysqlconnector://scott:tige |
| HIGH | ? | setup.cfg | 50 | Match: docker_mssql = mssql+pyodbc://scott:tiger^5HHH@127.0. |
| HIGH | ? | setup.cfg | 55 | Match: docker_oracle = oracle+cx_oracle://scott:tiger@127.0. |
| HIGH | ? | psycopg2.py | 88 | Match:         "postgresql+psycopg2://scott:tiger@192.168.0. |
| HIGH | ? | pg8000.py | 58 | Match:         "postgresql+pg8000://scott:tiger@192.168.0.19 |
| HIGH | ? | pg8000.py | 72 | Match:         "postgresql+pg8000://scott:tiger@192.168.0.19 |
| HIGH | ? | pymysql.py | 35 | Match:         "mysql+pymysql://scott:tiger@192.168.0.134/te |
| HIGH | ? | lambdas.py | 1264 | Match:         exec(code, vars_, vars_) |
| HIGH | ? | langhelpers.py | 1039 | Match:         exec(py, env) |
| HIGH | ? | langhelpers.py | 2038 | Match:     exec(code, env) |
| HIGH | ? | typing.py | 265 | Match:             annotation = eval(expression, cls_namespa |
| HIGH | ? | typing.py | 267 | Match:             annotation = eval(expression, base_global |
| HIGH | ? | pytestplugin.py | 645 | Match:         exec(code, env) |
| HIGH | ? | _orm_constructors.py | 1172 | Match:          registry of tables.  The Python ``eval()`` f |
| HIGH | ? | _orm_constructors.py | 1408 | Match:          argument is interpreted using Python's ``eva |
| HIGH | ? | _orm_constructors.py | 1612 | Match:          argument is interpreted using Python's ``eva |
| HIGH | ? | _orm_constructors.py | 1709 | Match:          argument is interpreted using Python's ``eva |
| HIGH | ? | _orm_constructors.py | 1728 | Match:          argument is interpreted using Python's ``eva |
| HIGH | ? | _orm_constructors.py | 1770 | Match:          argument is interpreted using Python's ``eva |
| HIGH | ? | clsregistry.py | 592 | Match:                 x = eval(self.arg, globals(), self._d |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | base.py | 1857 | Line 1857: def pre_exec(self): |
| HIGH | GS004 | base.py | 1918 | Line 1918: def post_exec(self): |
| HIGH | GS004 | _mariadb_shim.py | 81 | Line 81: def post_exec(self) -> None: |
| HIGH | GS004 | mariadbconnector.py | 104 | Line 104: def post_exec(self) -> None: |
| HIGH | GS004 | base.py | 2078 | Line 2078: def pre_exec(self): |
| HIGH | GS004 | default.py | 1921 | Line 1921: def pre_exec(self): |
| HIGH | GS004 | default.py | 1929 | Line 1929: def post_exec(self): |
| HIGH | GS004 | interfaces.py | 3164 | Line 3164: def pre_exec(self) -> None: |
| HIGH | GS004 | interfaces.py | 3210 | Line 3210: def post_exec(self) -> None: |
| HIGH | GS004 | bulk_persistence.py | 694 | Line 694: def orm_pre_session_exec( |
| HIGH | GS004 | bulk_persistence.py | 1195 | Line 1195: def orm_pre_session_exec( |
| HIGH | GS004 | context.py | 295 | Line 295: def orm_pre_session_exec( |
| HIGH | GS004 | context.py | 345 | Line 345: def orm_pre_session_exec( |
| HIGH | GS004 | context.py | 506 | Line 506: def orm_pre_session_exec( |
| HIGH | GS004 | session.py | 4649 | Line 4649: self.dispatch.after_flush_postexec(self, flush_co |
| HIGH | GS004 | strategies.py | 2905 | Line 2905: def load_collection_from_joined_exec(state, dict_ |
| HIGH | GS004 | strategies.py | 2944 | Line 2944: def load_scalar_from_joined_exec(state, dict_, ro |
| HIGH | GS004 | lambdas.py | 1264 | Line 1264: exec(code, vars_, vars_) |
| HIGH | GS004 | pytestplugin.py | 645 | Line 645: exec(code, env) |
| HIGH | GS004 | langhelpers.py | 1039 | Line 1039: exec(py, env) |
| HIGH | GS004 | langhelpers.py | 2038 | Line 2038: exec(code, env) |
| HIGH | GS014 | base.py | 195 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | psycopg.py | 21 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | psycopg.py | 81 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | psycopg.py | 103 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | automap.py | 150 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | automap.py | 180 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | events.py | 76 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | provision.py | 126 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | engines.py | 33 | Database URL contains password in plaintext. Use environment |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | compiler.py | 5737 |
| C | ? | compiler.py | 6441 |
| C | ? | crud.py | 373 |
| C | ? | crud.py | 475 |
| C | ? | crud.py | 690 |
| C | ? | base.py | 1530 |
| C | ? | base.py | 1533 |
| C | ? | base.py | 2300 |
| C | ? | persistence.py | 1112 |
| M | ? | _result_cy.py | 552 |
| M | ? | _result_cy.py | 587 |
| M | ? | util.py | 135 |
| M | ? | provision.py | 56 |
| M | ? | _mariadb_shim.py | 269 |
| M | ? | mariadbconnector.py | 239 |
| M | ? | provision.py | 217 |
| M | ? | base.py | 2229 |
| M | ? | base.py | 2282 |
| M | ? | base.py | 108 |
| M | ? | base.py | 113 |
| M | ? | util.py | 172 |
| M | ? | requirements.py | 1168 |
| M | ? | attr.py | 456 |
| M | ? | attr.py | 501 |
| M | ? | langhelpers.py | 1940 |
| M | ? | langhelpers.py | 1995 |
| M | ? | loading.py | 146 |
| M | ? | loading.py | 170 |
| M | ? | state.py | 596 |
| M | ? | requirements.py | 1337 |
| M | ? | state_changes.py | 138 |
| M | ? | state_changes.py | 188 |
| M | ? | session.py | 1258 |
| M | ? | session.py | 1315 |
| M | ? | session.py | 1380 |
| M | ? | session.py | 2676 |
| M | ? | session.py | 4653 |
| M | ? | session.py | 4928 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | instrumentation.py | 549 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| L | ? | compiler.py | 165 |
| L | ? | selectable.py | 21 |
| L | ? | crud.py | 1515 |
| L | ? | type_api.py | 780 |
| L | ? | type_api.py | 826 |
| L | ? | instrumentation.py | 549 |
| L | ? | attributes.py | 2600 |
| M | ? | format_docs_code.py | 208 |
| M | ? | format_docs_code.py | 220 |
| M | ? | format_docs_code.py | 224 |
| M | ? | format_docs_code.py | 254 |
| M | ? | format_docs_code.py | 255 |
| M | ? | format_docs_code.py | 266 |
| M | ? | format_docs_code.py | 288 |
| M | ? | _row_cy.py | 194 |
| M | ? | _row_cy.py | 214 |
| M | ? | _result_cy.py | 238 |
| M | ? | _result_cy.py | 351 |
| M | ? | _result_cy.py | 352 |
| M | ? | _result_cy.py | 354 |
| M | ? | _result_cy.py | 471 |
| M | ? | _result_cy.py | 631 |
| M | ? | create.py | 722 |
| M | ? | result.py | 136 |
| M | ? | result.py | 282 |
| M | ? | result.py | 451 |
| M | ? | util.py | 141 |
| M | ? | util.py | 154 |
| M | ? | cursor.py | 265 |
| M | ? | cursor.py | 329 |
| M | ? | cursor.py | 334 |
| M | ? | cursor.py | 734 |
| M | ? | cursor.py | 808 |
| M | ? | cursor.py | 859 |
| M | ? | cursor.py | 933 |
| M | ? | cursor.py | 987 |
| M | ? | cursor.py | 1230 |
| M | ? | cursor.py | 1502 |
| M | ? | cursor.py | 1678 |
| M | ? | cursor.py | 1702 |
| M | ? | cursor.py | 2023 |
| M | ? | cursor.py | 2024 |
| M | ? | cursor.py | 2025 |
| M | ? | base.py | 644 |
| M | ? | base.py | 763 |
| M | ? | base.py | 1208 |
| M | ? | base.py | 1219 |
| M | ? | base.py | 1231 |
| M | ? | base.py | 2331 |
| M | ? | base.py | 2334 |
| M | ? | base.py | 2342 |
| M | ? | base.py | 2416 |
| M | ? | base.py | 2419 |
| M | ? | base.py | 2568 |
| M | ? | base.py | 2590 |
| M | ? | base.py | 2611 |
| M | ? | base.py | 2657 |
| M | ? | base.py | 2668 |
| M | ? | base.py | 2700 |
| M | ? | base.py | 2701 |
| M | ? | base.py | 2711 |
| M | ? | base.py | 2734 |
| M | ? | base.py | 2735 |
| M | ? | base.py | 2775 |
| M | ? | base.py | 2821 |
| M | ? | base.py | 2823 |
| M | ? | default.py | 926 |
| M | ? | default.py | 977 |
| M | ? | default.py | 984 |
| M | ? | default.py | 992 |
| M | ? | default.py | 993 |
| M | ? | default.py | 1136 |
| M | ? | default.py | 1145 |
| M | ? | default.py | 1486 |
| M | ? | default.py | 1496 |
| M | ? | default.py | 1625 |
| M | ? | default.py | 1747 |
| M | ? | default.py | 1797 |
| M | ? | default.py | 1803 |
| M | ? | default.py | 2098 |
| M | ? | default.py | 2120 |
| M | ? | default.py | 2152 |
| M | ? | default.py | 2425 |
| M | ? | default.py | 2426 |
| M | ? | default.py | 2430 |
| M | ? | default.py | 2442 |
| M | ? | automap.py | 669 |
| M | ? | compiler.py | 295 |
| M | ? | hybrid.py | 527 |
| M | ? | hybrid.py | 1089 |
| M | ? | hybrid.py | 1790 |
| M | ? | hybrid.py | 1797 |
| M | ? | mutable.py | 148 |
| M | ? | mutable.py | 323 |
| M | ? | associationproxy.py | 453 |
| M | ? | associationproxy.py | 893 |
| M | ? | associationproxy.py | 926 |
| M | ? | baked.py | 200 |
| M | ? | engine.py | 338 |
| M | ? | engine.py | 343 |
| M | ? | horizontal_shard.py | 116 |
| M | ? | horizontal_shard.py | 313 |
| M | ? | horizontal_shard.py | 318 |
| M | ? | horizontal_shard.py | 341 |
| M | ? | horizontal_shard.py | 351 |
| M | ? | horizontal_shard.py | 367 |
| M | ? | horizontal_shard.py | 446 |
| M | ? | events.py | 78 |
| M | ? | impl.py | 497 |
| M | ? | impl.py | 547 |
| M | ? | base.py | 866 |
| M | ? | base.py | 880 |
| M | ? | base.py | 938 |
| M | ? | base.py | 940 |
| M | ? | base.py | 943 |
| M | ? | base.py | 975 |
| M | ? | base.py | 982 |
| M | ? | base.py | 1275 |
| M | ? | base.py | 1278 |
| M | ? | base.py | 1491 |
| M | ? | sqltypes.py | 136 |
| M | ? | coercions.py | 417 |
| M | ? | coercions.py | 463 |
| M | ? | coercions.py | 715 |
| M | ? | coercions.py | 900 |
| M | ? | coercions.py | 1300 |
| M | ? | traversals.py | 359 |
| M | ? | traversals.py | 548 |
| M | ? | traversals.py | 549 |
| M | ? | traversals.py | 550 |
| M | ? | traversals.py | 553 |
| M | ? | _annotated_cols.py | 273 |
| M | ? | _annotated_cols.py | 390 |
| M | ? | compiler.py | 934 |
| M | ? | compiler.py | 939 |
| M | ? | compiler.py | 1530 |
| M | ? | compiler.py | 1534 |
| M | ? | compiler.py | 1719 |
| M | ? | compiler.py | 1720 |
| M | ? | compiler.py | 1721 |
| M | ? | compiler.py | 1726 |
| M | ? | compiler.py | 1747 |
| M | ? | compiler.py | 1778 |
| M | ? | compiler.py | 1779 |
| M | ? | compiler.py | 1824 |
| M | ? | compiler.py | 1921 |
| M | ? | compiler.py | 1932 |
| M | ? | compiler.py | 1961 |
| M | ? | compiler.py | 2208 |
| M | ? | compiler.py | 2260 |
| M | ? | compiler.py | 2320 |
| M | ? | compiler.py | 2324 |
| M | ? | compiler.py | 2402 |
| M | ? | compiler.py | 2406 |
| M | ? | compiler.py | 2412 |
| M | ? | compiler.py | 2723 |
| M | ? | compiler.py | 3454 |
| M | ? | compiler.py | 3524 |
| M | ? | compiler.py | 3913 |
| M | ? | compiler.py | 4246 |
| M | ? | compiler.py | 4267 |
| M | ? | compiler.py | 4316 |
| M | ? | compiler.py | 4317 |
| M | ? | compiler.py | 4406 |
| M | ? | compiler.py | 4480 |
| M | ? | compiler.py | 4662 |
| M | ? | compiler.py | 4757 |
| M | ? | compiler.py | 4777 |
| M | ? | compiler.py | 4885 |
| M | ? | compiler.py | 4985 |
| M | ? | compiler.py | 5331 |
| M | ? | compiler.py | 5758 |
| M | ? | compiler.py | 5891 |
| M | ? | compiler.py | 5962 |
| M | ? | compiler.py | 5971 |
| M | ? | compiler.py | 6050 |
| M | ? | compiler.py | 6250 |
| M | ? | compiler.py | 6299 |
| M | ? | compiler.py | 6573 |
| M | ? | compiler.py | 6706 |
| M | ? | compiler.py | 6860 |
| M | ? | compiler.py | 8118 |
| M | ? | compiler.py | 8148 |
| M | ? | compiler.py | 8202 |
| M | ? | compiler.py | 8214 |
| M | ? | compiler.py | 8257 |
| M | ? | selectable.py | 2157 |
| M | ? | selectable.py | 2466 |
| M | ? | selectable.py | 2472 |
| M | ? | selectable.py | 2514 |
| M | ? | selectable.py | 2538 |
| M | ? | elements.py | 329 |
| M | ? | elements.py | 532 |
| M | ? | elements.py | 1546 |
| M | ? | elements.py | 1743 |
| M | ? | elements.py | 1808 |
| M | ? | elements.py | 1809 |
| M | ? | elements.py | 3165 |
| M | ? | elements.py | 3290 |
| M | ? | elements.py | 3402 |
| M | ? | elements.py | 4134 |
| M | ? | elements.py | 4355 |
| M | ? | elements.py | 4416 |
| M | ? | elements.py | 5512 |
| M | ? | elements.py | 5524 |
| M | ? | elements.py | 5752 |
| M | ? | elements.py | 5883 |
| M | ? | crud.py | 169 |
| M | ? | crud.py | 236 |
| M | ? | crud.py | 252 |
| M | ? | crud.py | 297 |
| M | ? | crud.py | 371 |
| M | ? | crud.py | 394 |
| M | ? | crud.py | 623 |
| M | ? | crud.py | 652 |
| M | ? | crud.py | 728 |
| M | ? | crud.py | 1456 |
| M | ? | crud.py | 1577 |
| M | ? | cache_key.py | 167 |
| M | ? | cache_key.py | 173 |
| M | ? | cache_key.py | 388 |
| M | ? | lambdas.py | 408 |
| M | ? | lambdas.py | 451 |
| M | ? | lambdas.py | 594 |
| M | ? | schema.py | 2598 |
| M | ? | schema.py | 3427 |
| M | ? | schema.py | 3430 |
| M | ? | schema.py | 3453 |
| M | ? | schema.py | 3478 |
| M | ? | schema.py | 3553 |
| M | ? | schema.py | 3558 |
| M | ? | schema.py | 3572 |
| M | ? | schema.py | 3586 |
| M | ? | schema.py | 3680 |
| M | ? | schema.py | 4314 |
| M | ? | schema.py | 4404 |
| M | ? | schema.py | 6483 |
| M | ? | schema.py | 6660 |
| M | ? | util.py | 236 |
| M | ? | util.py | 423 |
| M | ? | util.py | 708 |
| M | ? | util.py | 876 |
| M | ? | util.py | 1210 |
| M | ? | util.py | 1220 |
| M | ? | util.py | 1349 |
| M | ? | util.py | 1474 |
| M | ? | dml.py | 256 |
| M | ? | dml.py | 267 |
| M | ? | dml.py | 351 |
| M | ? | dml.py | 384 |
| M | ? | base.py | 297 |
| M | ? | base.py | 1232 |
| M | ? | base.py | 1445 |
| M | ? | ddl.py | 140 |
| M | ? | ddl.py | 459 |
| M | ? | ddl.py | 1260 |
| M | ? | hybrid_three.py | 46 |
| M | ? | hybrid_three.py | 76 |
| M | ? | type_api.py | 210 |
| M | ? | type_api.py | 1042 |
| M | ? | type_api.py | 1813 |
| M | ? | type_api.py | 1821 |
| M | ? | types.py | 67 |
| M | ? | base.py | 2454 |
| M | ? | base.py | 3678 |
| M | ? | base.py | 3679 |
| M | ? | base.py | 5185 |
| M | ? | declared_attr_one.py | 55 |
| M | ? | declared_attr_one.py | 72 |
| M | ? | psycopg.py | 488 |
| M | ? | psycopg.py | 492 |
| M | ? | ranges.py | 622 |
| M | ? | named_types.py | 119 |
| M | ? | _mariadb_shim.py | 53 |
| M | ? | _mariadb_shim.py | 235 |
| M | ? | _mariadb_shim.py | 277 |
| M | ? | _mariadb_shim.py | 302 |
| M | ? | typed_queries.py | 369 |
| M | ? | enumerated.py | 91 |
| M | ? | enumerated.py | 216 |
| M | ? | enumerated.py | 218 |
| M | ? | declared_attr_three.py | 60 |
| M | ? | base.py | 1749 |
| M | ? | base.py | 1814 |
| M | ? | base.py | 1974 |
| M | ? | base.py | 2001 |
| M | ? | base.py | 3055 |
| M | ? | base.py | 3190 |
| M | ? | base.py | 3248 |
| M | ? | base.py | 3767 |
| M | ? | base.py | 3813 |
| M | ? | mapped_covariant.py | 65 |
| M | ? | mapped_covariant.py | 82 |
| M | ? | mariadbconnector.py | 110 |
| M | ? | mariadbconnector.py | 116 |
| M | ? | provision.py | 162 |
| M | ? | base.py | 3374 |
| M | ? | base.py | 3378 |
| M | ? | base.py | 3555 |
| M | ? | base.py | 3690 |
| M | ? | base.py | 3741 |
| M | ? | base.py | 1862 |
| M | ? | base.py | 1863 |
| M | ? | base.py | 1864 |
| M | ? | base.py | 1978 |
| M | ? | base.py | 1979 |
| M | ? | base.py | 1980 |
| M | ? | base.py | 2357 |
| M | ? | provision.py | 54 |
| M | ? | provision.py | 67 |
| M | ? | base.py | 831 |
| M | ? | base.py | 845 |
| M | ? | base.py | 2270 |
| M | ? | base.py | 2438 |
| M | ? | assertsql.py | 32 |
| M | ? | assertsql.py | 103 |
| M | ? | assertsql.py | 351 |
| M | ? | assertsql.py | 470 |
| M | ? | assertsql.py | 472 |
| M | ? | engines.py | 60 |
| M | ? | engines.py | 169 |
| M | ? | engines.py | 185 |
| M | ? | engines.py | 258 |
| M | ? | engines.py | 419 |
| M | ? | engines.py | 426 |
| M | ? | exclusions.py | 242 |
| M | ? | exclusions.py | 310 |
| M | ? | exclusions.py | 473 |
| M | ? | assertions.py | 196 |
| M | ? | assertions.py | 197 |
| M | ? | assertions.py | 255 |
| M | ? | assertions.py | 277 |
| M | ? | assertions.py | 287 |
| M | ? | assertions.py | 292 |
| M | ? | assertions.py | 297 |
| M | ? | assertions.py | 302 |
| M | ? | assertions.py | 306 |
| M | ? | assertions.py | 327 |
| M | ? | assertions.py | 332 |
| M | ? | assertions.py | 341 |
| M | ? | assertions.py | 346 |
| M | ? | assertions.py | 355 |
| M | ? | assertions.py | 369 |
| M | ? | assertions.py | 386 |
| M | ? | assertions.py | 482 |
| M | ? | assertions.py | 498 |
| M | ? | assertions.py | 677 |
| M | ? | assertions.py | 765 |
| M | ? | assertions.py | 790 |
| M | ? | assertions.py | 793 |
| M | ? | assertions.py | 801 |
| M | ? | assertions.py | 817 |
| M | ? | assertions.py | 822 |
| M | ? | assertions.py | 824 |
| M | ? | assertions.py | 827 |
| M | ? | orm.py | 119 |
| M | ? | orm.py | 175 |
| M | ? | sql.py | 87 |
| M | ? | sql.py | 329 |
| M | ? | sql.py | 334 |
| M | ? | sql.py | 340 |
| M | ? | sql.py | 351 |
| M | ? | sql.py | 355 |
| M | ? | sql.py | 378 |
| M | ? | sql.py | 380 |
| M | ? | base.py | 57 |
| M | ? | base.py | 237 |
| M | ? | base.py | 243 |
| M | ? | util.py | 191 |
| M | ? | util.py | 406 |
| M | ? | bootstrap.py | 38 |
| M | ? | bootstrap.py | 39 |
| M | ? | legacy.py | 103 |
| M | ? | legacy.py | 107 |
| M | ? | legacy.py | 235 |
| M | ? | registry.py | 194 |
| M | ? | base.py | 147 |
| M | ? | base.py | 195 |
| M | ? | base.py | 318 |
| M | ? | attr.py | 183 |
| M | ? | attr.py | 346 |
| M | ? | attr.py | 356 |
| M | ? | langhelpers.py | 157 |
| M | ? | langhelpers.py | 161 |
| M | ? | langhelpers.py | 166 |
| M | ? | langhelpers.py | 863 |
| M | ? | langhelpers.py | 1293 |
| M | ? | langhelpers.py | 1573 |
| M | ? | langhelpers.py | 1635 |
| M | ? | langhelpers.py | 1698 |
| M | ? | langhelpers.py | 2299 |
| M | ? | langhelpers.py | 2301 |
| M | ? | langhelpers.py | 2303 |
| M | ? | langhelpers.py | 2305 |
| M | ? | langhelpers.py | 2311 |
| M | ? | langhelpers.py | 2313 |
| M | ? | tool_support.py | 47 |
| M | ? | tool_support.py | 167 |
| M | ? | concurrency.py | 170 |
| M | ? | concurrency.py | 275 |
| M | ? | concurrency.py | 280 |
| M | ? | concurrency.py | 314 |
| M | ? | deprecations.py | 139 |
| M | ? | deprecations.py | 140 |
| M | ? | deprecations.py | 184 |
| M | ? | deprecations.py | 265 |
| M | ? | deprecations.py | 347 |
| M | ? | deprecations.py | 348 |
| M | ? | misc.py | 17 |
| M | ? | misc.py | 24 |
| M | ? | misc.py | 89 |
| M | ? | misc.py | 108 |
| M | ? | misc.py | 115 |
| M | ? | misc.py | 199 |
| M | ? | misc.py | 206 |
| M | ? | misc.py | 261 |
| M | ? | misc.py | 268 |
| M | ? | row.py | 14 |
| M | ? | row.py | 21 |
| M | ? | row.py | 74 |
| M | ? | row.py | 81 |
| M | ? | row.py | 109 |
| M | ? | row.py | 124 |
| M | ? | result.py | 27 |
| M | ? | result.py | 103 |
| M | ? | result.py | 240 |
| M | ? | result.py | 247 |
| M | ? | result.py | 249 |
| M | ? | result.py | 290 |
| M | ? | result.py | 292 |
| M | ? | result.py | 345 |
| M | ? | command.py | 179 |
| M | ? | command.py | 187 |
| M | ? | command.py | 191 |
| M | ? | instrumentation.py | 206 |
| M | ? | instrumentation.py | 474 |
| M | ? | instrumentation.py | 604 |
| M | ? | instrumentation.py | 605 |
| M | ? | instrumentation.py | 615 |
| M | ? | cache_key.py | 118 |
| M | ? | cache_key.py | 127 |
| M | ? | cache_key.py | 128 |
| M | ? | cache_key.py | 129 |
| M | ? | cache_key.py | 130 |
| M | ? | base.py | 65 |
| M | ? | loading.py | 556 |
| M | ? | loading.py | 1019 |
| M | ? | collections_.py | 15 |
| M | ? | collections_.py | 22 |
| M | ? | collections_.py | 188 |
| M | ? | collections_.py | 195 |
| M | ? | collections_.py | 444 |
| M | ? | collections_.py | 451 |
| M | ? | collections_.py | 502 |
| M | ? | collections_.py | 509 |
| M | ? | collections_.py | 525 |
| M | ? | many_table_reflection.py | 645 |
| M | ? | many_table_reflection.py | 646 |
| M | ? | strategy_options.py | 1072 |
| M | ? | strategy_options.py | 1161 |
| M | ? | strategy_options.py | 1373 |
| M | ? | strategy_options.py | 1375 |
| M | ? | strategy_options.py | 1388 |
| M | ? | strategy_options.py | 1402 |
| M | ? | strategy_options.py | 1409 |
| M | ? | strategy_options.py | 1442 |
| M | ? | strategy_options.py | 1445 |
| M | ? | strategy_options.py | 1448 |
| M | ? | strategy_options.py | 1461 |
| M | ? | strategy_options.py | 1474 |
| M | ? | strategy_options.py | 1770 |
| M | ? | strategy_options.py | 1812 |
| M | ? | strategy_options.py | 1813 |
| M | ? | strategy_options.py | 1814 |
| M | ? | strategy_options.py | 1910 |
| M | ? | strategy_options.py | 1929 |
| M | ? | strategy_options.py | 1956 |
| M | ? | strategy_options.py | 2008 |
| M | ? | strategy_options.py | 2034 |
| M | ? | strategy_options.py | 2037 |
| M | ? | strategy_options.py | 2079 |
| M | ? | strategy_options.py | 2102 |
| M | ? | strategy_options.py | 2131 |
| M | ? | strategy_options.py | 2202 |
| M | ? | strategy_options.py | 2356 |
| M | ? | attributes.py | 219 |
| M | ? | attributes.py | 337 |
| M | ? | attributes.py | 351 |
| M | ? | attributes.py | 401 |
| M | ? | attributes.py | 425 |
| M | ? | attributes.py | 981 |
| M | ? | attributes.py | 999 |
| M | ? | attributes.py | 1239 |
| M | ? | attributes.py | 1728 |
| M | ? | attributes.py | 1859 |
| M | ? | attributes.py | 1897 |
| M | ? | attributes.py | 1903 |
| M | ? | attributes.py | 1919 |
| M | ? | attributes.py | 1925 |
| M | ? | attributes.py | 2731 |
| M | ? | context.py | 245 |
| M | ? | context.py | 585 |
| M | ? | context.py | 801 |
| M | ? | context.py | 1398 |
| M | ? | context.py | 1563 |
| M | ? | context.py | 1564 |
| M | ? | context.py | 1590 |
| M | ? | context.py | 2021 |
| M | ? | context.py | 2085 |
| M | ? | context.py | 2414 |
| M | ? | context.py | 3426 |
| M | ? | strategies.py | 1823 |
| M | ? | strategies.py | 2059 |
| M | ? | strategies.py | 2413 |
| M | ? | strategies.py | 2532 |
| M | ? | strategies.py | 2622 |
| M | ? | strategies.py | 2625 |
| M | ? | strategies.py | 2703 |
| M | ? | strategies.py | 2725 |
| M | ? | clsregistry.py | 349 |
| M | ? | clsregistry.py | 376 |
| M | ? | clsregistry.py | 477 |
| M | ? | clsregistry.py | 547 |
| M | ? | clsregistry.py | 581 |
| M | ? | writeonly.py | 517 |
| M | ? | bulk_persistence.py | 239 |
| M | ? | bulk_persistence.py | 253 |
| M | ? | bulk_persistence.py | 443 |
| M | ? | bulk_persistence.py | 497 |
| M | ? | bulk_persistence.py | 724 |
| M | ? | bulk_persistence.py | 1217 |
| M | ? | bulk_persistence.py | 1309 |
| M | ? | bulk_persistence.py | 1310 |
| M | ? | bulk_persistence.py | 1640 |
| M | ? | bulk_persistence.py | 1654 |
| M | ? | bulk_persistence.py | 1655 |
| M | ? | state.py | 528 |
| M | ? | state.py | 914 |
| M | ? | path_registry.py | 289 |
| M | ? | path_registry.py | 313 |
| M | ? | path_registry.py | 391 |
| M | ? | path_registry.py | 462 |
| M | ? | path_registry.py | 490 |
| M | ? | path_registry.py | 619 |
| M | ? | path_registry.py | 646 |
| M | ? | persistence.py | 1218 |
| M | ? | unitofwork.py | 639 |
| M | ? | unitofwork.py | 676 |
| M | ? | descriptor_props.py | 912 |
| M | ? | descriptor_props.py | 966 |
| M | ? | identity.py | 151 |
| M | ? | identity.py | 162 |
| M | ? | identity.py | 183 |
| M | ? | identity.py | 241 |
| M | ? | identity.py | 266 |
| M | ? | identity.py | 282 |
| M | ? | exc.py | 195 |
| M | ? | util.py | 1009 |
| M | ? | util.py | 1077 |
| M | ? | util.py | 1172 |
| M | ? | util.py | 1199 |
| M | ? | util.py | 1255 |
| M | ? | util.py | 1413 |
| M | ? | util.py | 1460 |
| M | ? | util.py | 1493 |
| M | ? | util.py | 1862 |
| M | ? | util.py | 1882 |
| M | ? | util.py | 1935 |
| M | ? | util.py | 1965 |
| M | ? | util.py | 2128 |
| M | ? | mapper.py | 1178 |
| M | ? | mapper.py | 1179 |
| M | ? | mapper.py | 1198 |
| M | ? | mapper.py | 1199 |
| M | ? | mapper.py | 1213 |
| M | ? | mapper.py | 1314 |
| M | ? | mapper.py | 1369 |
| M | ? | mapper.py | 1379 |
| M | ? | mapper.py | 1380 |
| M | ? | mapper.py | 1381 |
| M | ? | mapper.py | 1450 |
| M | ? | mapper.py | 2247 |
| M | ? | mapper.py | 2251 |
| M | ? | mapper.py | 2385 |
| M | ? | mapper.py | 3677 |
| M | ? | mapper.py | 3678 |
| M | ? | mapper.py | 3679 |
| M | ? | mapper.py | 3767 |
| M | ? | mapper.py | 3811 |
| M | ? | mapper.py | 3876 |
| M | ? | decl_base.py | 195 |
| M | ? | decl_base.py | 608 |
| M | ? | decl_base.py | 1173 |
| M | ? | decl_base.py | 1203 |
| M | ? | decl_base.py | 1283 |
| M | ? | decl_base.py | 1305 |
| M | ? | decl_base.py | 1619 |
| M | ? | decl_base.py | 1718 |
| M | ? | decl_base.py | 1871 |
| M | ? | decl_base.py | 1895 |
| M | ? | decl_base.py | 1914 |
| M | ? | decl_base.py | 2091 |
| M | ? | state_changes.py | 83 |
| M | ? | state_changes.py | 180 |
| M | ? | base.py | 447 |
| M | ? | session.py | 967 |
| M | ? | session.py | 969 |
| M | ? | session.py | 1090 |
| M | ? | session.py | 1115 |
| M | ? | session.py | 1135 |
| M | ? | session.py | 1147 |
| M | ? | session.py | 1159 |
| M | ? | session.py | 1227 |
| M | ? | session.py | 1255 |
| M | ? | session.py | 1294 |
| M | ? | session.py | 1361 |
| M | ? | session.py | 3486 |
| M | ? | session.py | 3703 |
| M | ? | session.py | 3993 |
| M | ? | session.py | 4596 |
| M | ? | session.py | 4606 |
| M | ? | dependency.py | 136 |
| M | ? | dependency.py | 920 |
| M | ? | dependency.py | 927 |
| M | ? | decl_api.py | 301 |
| M | ? | decl_api.py | 1474 |
| M | ? | collections.py | 505 |
| M | ? | collections.py | 512 |
| M | ? | collections.py | 755 |
| M | ? | collections.py | 864 |
| M | ? | collections.py | 874 |
| M | ? | collections.py | 878 |
| M | ? | collections.py | 896 |
| M | ? | query.py | 668 |
| M | ? | query.py | 986 |
| M | ? | relationships.py | 2404 |
| M | ? | relationships.py | 2557 |
| M | ? | relationships.py | 2771 |
| M | ? | relationships.py | 2783 |
| M | ? | properties.py | 786 |
| M | ? | properties.py | 792 |
| M | ? | _concurrency_fixtures.py | 10 |
| M | ? | _concurrency_fixtures.py | 11 |
| M | ? | _concurrency_fixtures.py | 18 |
| M | ? | _concurrency_fixtures.py | 22 |
| M | ? | _concurrency_fixtures.py | 23 |
| M | ? | _concurrency_fixtures.py | 28 |
| M | ? | _concurrency_fixtures.py | 40 |
| M | ? | _concurrency_fixtures.py | 46 |
| M | ? | _concurrency_fixtures.py | 58 |
| M | ? | _concurrency_fixtures.py | 59 |
| M | ? | requirements.py | 1703 |
| M | ? | noxfile.py | 267 |
| H | ? | engines.py | 33 |
| H | ? | automap.py | 150 |
| H | ? | automap.py | 180 |
| H | ? | psycopg.py | 81 |
| H | ? | psycopg.py | 103 |
| H | ? | base.py | 195 |
| C | GS001 | pyodbc.py | 80 |
| C | GS001 | pyodbc.py | 215 |
| C | GS001 | pyodbc.py | 245 |
| C | GS001 | mysqldb.py | 204 |
| C | GS001 | cx_oracle.py | 192 |
| C | GS001 | cx_oracle.py | 236 |
| C | GS001 | oracledb.py | 267 |
| C | GS001 | oracledb.py | 309 |
| C | GS001 | oracledb.py | 341 |
| C | GS001 | psycopg.py | 21 |
| C | GS001 | aiosqlite.py | 14 |
| C | GS001 | base.py | 226 |
| C | GS001 | base.py | 234 |
| C | GS001 | base.py | 243 |
| C | GS001 | base.py | 263 |
| C | GS001 | base.py | 283 |
| C | GS001 | base.py | 314 |
| C | GS001 | provision.py | 78 |
| C | GS001 | pysqlite.py | 13 |
| C | GS001 | pysqlite.py | 41 |
| C | GS001 | pysqlite.py | 47 |
| C | GS001 | pysqlite.py | 56 |
| C | GS001 | pysqlite.py | 57 |
| C | GS001 | pysqlite.py | 77 |
| C | GS001 | pysqlite.py | 94 |
| C | GS001 | pysqlite.py | 254 |
| C | GS001 | pysqlite.py | 380 |
| C | GS001 | scoping.py | 822 |
| C | GS001 | scoping.py | 824 |
| C | GS001 | scoping.py | 825 |
| C | GS001 | setup.cfg | 24 |
| C | GS001 | setup.cfg | 25 |
| C | GS001 | setup.cfg | 28 |
| L | GS003 | base.py | 576 |
| L | GS003 | base.py | 584 |
| L | GS003 | base.py | 371 |
| L | GS003 | base.py | 977 |
| L | GS003 | cx_oracle.py | 210 |
| L | GS003 | cx_oracle.py | 261 |
| L | GS003 | oracledb.py | 281 |
| L | GS003 | oracledb.py | 325 |
| L | GS003 | base.py | 592 |
| L | GS003 | base.py | 601 |
| L | GS003 | base.py | 609 |
| L | GS003 | base.py | 1005 |
| L | GS003 | base.py | 1206 |
| L | GS003 | psycopg.py | 126 |
| L | GS003 | base.py | 350 |
| L | GS003 | base.py | 359 |
| L | GS003 | base.py | 367 |
| L | GS003 | pysqlite.py | 390 |
| L | GS003 | engine.py | 558 |
| L | GS003 | engine.py | 566 |
| L | GS003 | engine.py | 800 |
| L | GS003 | engine.py | 812 |
| L | GS003 | engine.py | 874 |
| L | GS003 | result.py | 199 |
| L | GS003 | session.py | 378 |
| L | GS003 | automap.py | 67 |
| L | GS003 | automap.py | 288 |
| L | GS003 | automap.py | 292 |
| L | GS003 | compiler.py | 37 |
| L | GS003 | compiler.py | 110 |
| L | GS003 | mutable.py | 240 |
| L | GS003 | context.py | 1271 |
| L | GS003 | context.py | 1272 |
| L | GS003 | context.py | 1275 |
| L | GS003 | context.py | 1276 |
| L | GS003 | context.py | 1277 |
| L | GS003 | context.py | 1279 |
| L | GS003 | context.py | 1280 |
| L | GS003 | events.py | 1542 |
| L | GS003 | events.py | 2417 |
| L | GS003 | events.py | 2444 |
| L | GS003 | events.py | 3266 |
| L | GS003 | util.py | 1609 |
| L | GS003 | _elements_constructors.py | 426 |
| L | GS003 | _elements_constructors.py | 611 |
| L | GS003 | _elements_constructors.py | 1812 |
| L | GS003 | _elements_constructors.py | 1900 |
| L | GS003 | elements.py | 298 |
| L | GS003 | elements.py | 2456 |
| L | GS003 | elements.py | 2465 |
| L | GS003 | functions.py | 961 |
| L | GS003 | functions.py | 1524 |
| L | GS003 | functions.py | 1543 |
| L | GS003 | selectable.py | 2673 |
| L | GS003 | visitors.py | 931 |
| L | GS003 | assertions.py | 488 |
| L | GS003 | assertions.py | 672 |
| L | GS003 | assertions.py | 839 |
| L | GS003 | exclusions.py | 172 |
| L | GS003 | plugin_base.py | 328 |
| L | GS003 | plugin_base.py | 330 |
| L | GS003 | pytestplugin.py | 162 |
| L | GS003 | pytestplugin.py | 164 |
| L | GS003 | profiling.py | 218 |
| L | GS003 | profiling.py | 296 |
| L | GS003 | profiling.py | 305 |
| L | GS003 | tool_support.py | 131 |
| L | GS003 | tool_support.py | 147 |
| L | GS003 | tool_support.py | 181 |
| L | GS003 | format_docs_code.py | 94 |
| L | GS003 | format_docs_code.py | 95 |
| L | GS003 | format_docs_code.py | 100 |
| L | GS003 | format_docs_code.py | 103 |
| L | GS003 | format_docs_code.py | 154 |
| L | GS003 | format_docs_code.py | 307 |
| L | GS003 | format_docs_code.py | 318 |
| L | GS003 | format_docs_code.py | 323 |
| L | GS003 | format_docs_code.py | 354 |
| L | GS003 | format_docs_code.py | 357 |
| L | GS003 | trace_orm_adapter.py | 88 |
| L | GS003 | trace_orm_adapter.py | 91 |
| L | GS003 | trace_orm_adapter.py | 104 |
| L | GS003 | trace_orm_adapter.py | 106 |
| L | GS003 | trace_orm_adapter.py | 112 |
| L | GS003 | trace_orm_adapter.py | 101 |
| L | GS003 | warn_tox.py | 2 |
| L | GS008 | base.py | 1025 |
| L | GS008 | base.py | 1026 |
| L | GS008 | base.py | 1027 |
| L | GS008 | base.py | 1030 |
| L | GS008 | base.py | 1031 |
| L | GS008 | reserved_words.py | 15 |
| L | GS008 | reserved_words.py | 291 |
| L | GS008 | types.py | 61 |
| L | GS008 | operators.py | 14 |
| L | GS008 | operators.py | 37 |
| L | GS008 | operators.py | 45 |
| L | GS008 | operators.py | 78 |
| L | GS008 | operators.py | 86 |
| L | GS008 | operators.py | 95 |
| L | GS008 | operators.py | 102 |
| L | GS008 | operators.py | 106 |
| L | GS008 | operators.py | 110 |
| L | GS008 | operators.py | 114 |
| L | GS008 | operators.py | 118 |
| L | GS008 | operators.py | 123 |
| L | GS008 | pg_catalog.py | 89 |
| L | GS008 | types.py | 32 |
| L | GS008 | types.py | 33 |
| L | GS008 | types.py | 34 |
| L | GS008 | cursor.py | 1234 |
| L | GS008 | cursor.py | 1322 |
| L | GS008 | base.py | 290 |
| L | GS008 | base.py | 292 |
| L | GS008 | base.py | 294 |
| L | GS008 | compiler.py | 256 |
| L | GS008 | traversals.py | 40 |
| L | GS008 | type_api.py | 79 |
| L | GS008 | provision.py | 30 |
| L | GS008 | cython.py | 19 |
| L | GS008 | cython.py | 34 |
| L | GS008 | typing.py | 709 |
| H | ? | setup.cfg | 32 |
| H | ? | setup.cfg | 33 |
| H | ? | setup.cfg | 34 |
| H | ? | setup.cfg | 35 |
| H | ? | setup.cfg | 36 |
| H | ? | setup.cfg | 37 |
| H | ? | setup.cfg | 38 |
| H | ? | setup.cfg | 39 |
| H | ? | setup.cfg | 40 |
| H | ? | setup.cfg | 41 |
| H | ? | setup.cfg | 42 |
| H | ? | setup.cfg | 43 |
| H | ? | setup.cfg | 44 |
| H | ? | setup.cfg | 45 |
| H | ? | setup.cfg | 50 |
| H | ? | setup.cfg | 55 |
| H | ? | psycopg2.py | 88 |
| H | ? | pg8000.py | 58 |
| H | ? | pg8000.py | 72 |
| H | ? | pymysql.py | 35 |
| C | ? | associationproxy.py | 413 |
| C | ? | information_schema.py | 55 |
| C | ? | information_schema.py | 56 |
| C | ? | information_schema.py | 57 |
| C | ? | information_schema.py | 64 |
| C | ? | information_schema.py | 65 |
| C | ? | information_schema.py | 66 |
| C | ? | information_schema.py | 67 |
| C | ? | information_schema.py | 74 |
| C | ? | information_schema.py | 75 |
| C | ? | information_schema.py | 76 |
| C | ? | information_schema.py | 77 |
| C | ? | information_schema.py | 78 |
| C | ? | information_schema.py | 79 |
| C | ? | information_schema.py | 81 |
| C | ? | information_schema.py | 83 |
| C | ? | information_schema.py | 84 |
| C | ? | information_schema.py | 85 |
| C | ? | information_schema.py | 86 |
| C | ? | information_schema.py | 111 |
| C | ? | information_schema.py | 112 |
| C | ? | information_schema.py | 113 |
| C | ? | information_schema.py | 114 |
| C | ? | information_schema.py | 115 |
| C | ? | information_schema.py | 117 |
| C | ? | information_schema.py | 118 |
| C | ? | information_schema.py | 119 |
| C | ? | information_schema.py | 120 |
| C | ? | information_schema.py | 121 |
| C | ? | information_schema.py | 122 |
| C | ? | information_schema.py | 123 |
| C | ? | information_schema.py | 130 |
| C | ? | information_schema.py | 131 |
| C | ? | information_schema.py | 132 |
| C | ? | information_schema.py | 133 |
| C | ? | information_schema.py | 151 |
| C | ? | information_schema.py | 152 |
| C | ? | information_schema.py | 153 |
| C | ? | information_schema.py | 154 |
| C | ? | information_schema.py | 161 |
| C | ? | information_schema.py | 162 |
| C | ? | information_schema.py | 163 |
| C | ? | information_schema.py | 164 |
| C | ? | information_schema.py | 165 |
| C | ? | information_schema.py | 166 |
| C | ? | information_schema.py | 173 |
| C | ? | information_schema.py | 174 |
| C | ? | information_schema.py | 175 |
| C | ? | information_schema.py | 180 |
| C | ? | information_schema.py | 185 |
| C | ? | information_schema.py | 188 |
| C | ? | information_schema.py | 190 |
| C | ? | information_schema.py | 191 |
| C | ? | information_schema.py | 192 |
| C | ? | information_schema.py | 199 |
| C | ? | information_schema.py | 200 |
| C | ? | information_schema.py | 201 |
| C | ? | information_schema.py | 202 |
| C | ? | information_schema.py | 203 |
| C | ? | information_schema.py | 204 |
| C | ? | information_schema.py | 223 |
| C | ? | information_schema.py | 224 |
| C | ? | information_schema.py | 225 |
| M | ? | noxfile.py | 116 |
| M | ? | tool_support.py | 46 |
| H | ? | lambdas.py | 1264 |
| H | ? | langhelpers.py | 1039 |
| H | ? | langhelpers.py | 2038 |
| H | ? | typing.py | 265 |
| H | ? | typing.py | 267 |
| H | ? | pytestplugin.py | 645 |
| H | ? | _orm_constructors.py | 1172 |
| H | ? | _orm_constructors.py | 1408 |
| H | ? | _orm_constructors.py | 1612 |
| H | ? | _orm_constructors.py | 1709 |
| H | ? | _orm_constructors.py | 1728 |
| H | ? | _orm_constructors.py | 1770 |
| H | ? | clsregistry.py | 592 |
| C | ? | sqltypes.py | 1991 |
| C | ? | serializer.py | 149 |
| C | ? | serializer.py | 152 |
| C | ? | serializer.py | 155 |
| C | ? | serializer.py | 159 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | GS004 | base.py | 1857 |
| H | GS004 | base.py | 1918 |
| H | GS004 | _mariadb_shim.py | 81 |
| H | GS004 | mariadbconnector.py | 104 |
| H | GS004 | base.py | 2078 |
| H | GS004 | default.py | 1921 |
| H | GS004 | default.py | 1929 |
| H | GS004 | interfaces.py | 3164 |
| H | GS004 | interfaces.py | 3210 |
| H | GS004 | bulk_persistence.py | 694 |
| H | GS004 | bulk_persistence.py | 1195 |
| H | GS004 | context.py | 295 |
| H | GS004 | context.py | 345 |
| H | GS004 | context.py | 506 |
| H | GS004 | session.py | 4649 |
| H | GS004 | strategies.py | 2905 |
| H | GS004 | strategies.py | 2944 |
| H | GS004 | lambdas.py | 1264 |
| H | GS004 | pytestplugin.py | 645 |
| H | GS004 | langhelpers.py | 1039 |
| H | GS004 | langhelpers.py | 2038 |
| C | GS005 | base.py | 3270 |
| C | GS005 | base.py | 2852 |
| C | GS005 | mysqldb.py | 179 |
| C | GS005 | provision.py | 277 |
| C | GS005 | base.py | 364 |
| C | GS005 | pg8000.py | 592 |
| C | GS005 | provision.py | 89 |
| C | GS005 | provision.py | 182 |
| C | GS005 | base.py | 3079 |
| s | GS009 |  | 0 |
| L | GS012 | dml.py | 51 |
| L | GS012 | base.py | 596 |
| L | GS012 | base.py | 354 |
| L | GS012 | dependency.py | 1236 |
| L | GS012 | persistence.py | 773 |
| L | GS012 | persistence.py | 1320 |
| L | GS012 | query.py | 3489 |
| L | GS012 | _elements_constructors.py | 586 |
| L | GS012 | dml.py | 489 |
| L | GS012 | dml.py | 754 |
| L | GS012 | dml.py | 1086 |
| L | GS012 | dml.py | 1102 |
| L | GS012 | dml.py | 1639 |
| L | GS012 | dml.py | 1687 |
| L | GS012 | selectable.py | 2897 |
| L | GS012 | selectable.py | 3301 |
| L | GS012 | sqltypes.py | 3043 |
| L | GS012 | typing.py | 106 |
| H | GS014 | base.py | 195 |
| H | GS014 | psycopg.py | 21 |
| H | GS014 | psycopg.py | 81 |
| H | GS014 | psycopg.py | 103 |
| H | GS014 | automap.py | 150 |
| H | GS014 | automap.py | 180 |
| H | GS014 | events.py | 76 |
| H | GS014 | provision.py | 126 |
| H | GS014 | engines.py | 33 |
| M | ? | command.py | 49 |
| M | ? | tool_support.py | 110 |

---
*Сгенерировано GSC v0.6 · 2026-07-01T04:08:31.048702*