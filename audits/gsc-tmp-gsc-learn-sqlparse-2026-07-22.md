---
title: "GSC Audit: /tmp/gsc-learn/sqlparse"
date: 2026-07-22
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/sqlparse

**Дата:** 22.07.2026 04:03  
**Путь:** `/tmp/gsc-learn/sqlparse`  
**Всего находок:** 22  
**CRITICAL:** 5 | **HIGH:** 2 | **MEDIUM:** 1 | **LOW:** 13

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 8 |
| GS003 | 5 |
| SQL injection risk: f-string in query | 2 |
| CVE-2026-55721: SQL injection | 2 |
| Python: assert in production | 1 |
| Python: raw string concatenation in SQL | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| World-readable file: .pre-commit-hooks.yaml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | bench_grouping.py | 52 | OWASP A03: Injection |
| CRITICAL | ? | bench_grouping.py | 58 | OWASP A03: Injection |
| CRITICAL | ? | bench_grouping.py | 43 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | bench_grouping.py | 52 |  |
| CRITICAL | ? | bench_grouping.py | 58 |  |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-hooks.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | bench_grouping.py | 52 |
| C | ? | bench_grouping.py | 58 |
| M | ? | sql.py | 241 |
| C | ? | bench_grouping.py | 43 |
| C | ? | bench_grouping.py | 52 |
| C | ? | bench_grouping.py | 58 |
| L | GS003 | bench_grouping.py | 37 |
| L | GS003 | bench_grouping.py | 41 |
| L | GS003 | bench_grouping.py | 47 |
| L | GS003 | bench_grouping.py | 55 |
| L | GS003 | sql.py | 197 |
| L | GS008 | keywords.py | 675 |
| L | GS008 | keywords.py | 725 |
| L | GS008 | keywords.py | 834 |
| L | GS008 | keywords.py | 839 |
| L | GS008 | keywords.py | 887 |
| L | GS008 | keywords.py | 971 |
| L | GS008 | keywords.py | 976 |
| L | GS008 | keywords.py | 993 |
| H | ? | .readthedocs.yaml | 0 |
| H | ? | .pre-commit-hooks.yaml | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-22T04:03:44.532465*