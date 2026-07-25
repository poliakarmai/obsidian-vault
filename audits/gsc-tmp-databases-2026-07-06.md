---
title: "GSC Audit: /tmp/databases"
date: 2026-07-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/databases

**Дата:** 06.07.2026 09:10  
**Путь:** `/tmp/databases`  
**Всего находок:** 93  
**CRITICAL:** 9 | **HIGH:** 1 | **MEDIUM:** 82 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 81 |
| GS005 | 8 |
| CVE-2026-56318: Information disclosure | 1 |
| Hardcoded encryption key | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | core.py | 607 | Match:             return self.replace(password="********"). |
| CRITICAL | GS005 | aiopg.py | 276 | Line 276: await cursor.execute(f"SAVEPOINT {self._savepoint_ |
| CRITICAL | GS005 | aiopg.py | 287 | Line 287: await cursor.execute(f"RELEASE SAVEPOINT {self._sa |
| CRITICAL | GS005 | aiopg.py | 298 | Line 298: await cursor.execute(f"ROLLBACK TO SAVEPOINT {self |
| CRITICAL | GS005 | asyncmy.py | 270 | Line 270: await cursor.execute(f"SAVEPOINT {self._savepoint_ |
| CRITICAL | GS005 | asyncmy.py | 281 | Line 281: await cursor.execute(f"RELEASE SAVEPOINT {self._sa |
| CRITICAL | GS005 | mysql.py | 267 | Line 267: await cursor.execute(f"SAVEPOINT {self._savepoint_ |
| CRITICAL | GS005 | mysql.py | 278 | Line 278: await cursor.execute(f"RELEASE SAVEPOINT {self._sa |
| CRITICAL | GS005 | mysql.py | 289 | Line 289: await cursor.execute(f"ROLLBACK TO SAVEPOINT {self |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | postgres.py | 65 |
| M | ? | postgres.py | 77 |
| M | ? | postgres.py | 92 |
| M | ? | postgres.py | 93 |
| M | ? | postgres.py | 97 |
| M | ? | postgres.py | 98 |
| M | ? | postgres.py | 103 |
| M | ? | postgres.py | 111 |
| M | ? | postgres.py | 139 |
| M | ? | postgres.py | 144 |
| M | ? | postgres.py | 155 |
| M | ? | postgres.py | 196 |
| M | ? | postgres.py | 208 |
| M | ? | postgres.py | 213 |
| M | ? | postgres.py | 217 |
| M | ? | aiopg.py | 78 |
| M | ? | aiopg.py | 90 |
| M | ? | aiopg.py | 111 |
| M | ? | aiopg.py | 112 |
| M | ? | aiopg.py | 116 |
| M | ? | aiopg.py | 117 |
| M | ? | aiopg.py | 122 |
| M | ? | aiopg.py | 146 |
| M | ? | aiopg.py | 168 |
| M | ? | aiopg.py | 178 |
| M | ? | aiopg.py | 190 |
| M | ? | aiopg.py | 254 |
| M | ? | aiopg.py | 267 |
| M | ? | aiopg.py | 281 |
| M | ? | aiopg.py | 292 |
| M | ? | asyncmy.py | 67 |
| M | ? | asyncmy.py | 80 |
| M | ? | asyncmy.py | 101 |
| M | ? | asyncmy.py | 102 |
| M | ? | asyncmy.py | 106 |
| M | ? | asyncmy.py | 107 |
| M | ? | asyncmy.py | 112 |
| M | ? | asyncmy.py | 138 |
| M | ? | asyncmy.py | 160 |
| M | ? | asyncmy.py | 172 |
| M | ? | asyncmy.py | 184 |
| M | ? | asyncmy.py | 248 |
| M | ? | asyncmy.py | 261 |
| M | ? | asyncmy.py | 275 |
| M | ? | asyncmy.py | 286 |
| M | ? | sqlite.py | 84 |
| M | ? | sqlite.py | 88 |
| M | ? | sqlite.py | 93 |
| M | ? | sqlite.py | 113 |
| M | ? | sqlite.py | 132 |
| M | ? | sqlite.py | 141 |
| M | ? | sqlite.py | 148 |
| M | ? | sqlite.py | 214 |
| M | ? | sqlite.py | 227 |
| M | ? | sqlite.py | 241 |
| M | ? | sqlite.py | 252 |
| M | ? | mysql.py | 67 |
| M | ? | mysql.py | 80 |
| M | ? | mysql.py | 101 |
| M | ? | mysql.py | 102 |
| M | ? | mysql.py | 106 |
| M | ? | mysql.py | 107 |
| M | ? | mysql.py | 112 |
| M | ? | mysql.py | 135 |
| M | ? | mysql.py | 157 |
| M | ? | mysql.py | 169 |
| M | ? | mysql.py | 181 |
| M | ? | mysql.py | 245 |
| M | ? | mysql.py | 258 |
| M | ? | mysql.py | 272 |
| M | ? | mysql.py | 283 |
| M | ? | core.py | 72 |
| M | ? | core.py | 119 |
| M | ? | core.py | 120 |
| M | ? | core.py | 138 |
| M | ? | core.py | 139 |
| M | ? | core.py | 277 |
| M | ? | core.py | 462 |
| M | ? | core.py | 464 |
| M | ? | core.py | 471 |
| M | ? | core.py | 473 |
| M | ? | core.py | 607 |
| C | ? | core.py | 607 |
| H | ? | mkdocs.yml | 0 |
| C | GS005 | aiopg.py | 276 |
| C | GS005 | aiopg.py | 287 |
| C | GS005 | aiopg.py | 298 |
| C | GS005 | asyncmy.py | 270 |
| C | GS005 | asyncmy.py | 281 |
| C | GS005 | mysql.py | 267 |
| C | GS005 | mysql.py | 278 |
| C | GS005 | mysql.py | 289 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-06T09:10:46.407506*