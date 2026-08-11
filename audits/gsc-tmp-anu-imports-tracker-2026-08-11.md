---
title: "GSC Audit: /tmp/anu-imports-tracker"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/anu-imports-tracker

**Дата:** 11.08.2026 06:20  
**Путь:** `/tmp/anu-imports-tracker`  
**Всего находок:** 686  
**CRITICAL:** 365 | **HIGH:** 14 | **MEDIUM:** 2 | **LOW:** 9

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS005 | 365 |
| GS020 | 96 |
| GS021 | 88 |
| GS007 | 67 |
| GS015 | 31 |
| GS022 | 9 |
| GS025 | 6 |
| GS003 | 6 |
| GS004 | 6 |
| GS008 | 3 |
| YAML-B39DC08C | 2 |
| GS000-LEGACY | 1 |
| GS029 | 1 |
| GS032-exfil_curl | 1 |
| GS009 | 1 |
| GS018 | 1 |
| GS019 | 1 |
| GS025-wildcard_bind | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | migrate_history.py | 69 | OWASP A03: Injection |
| CRITICAL | GS005 | migrate_history.py | 148 | OWASP A03: Injection |
| CRITICAL | GS005 | migrate_history.py | 159 | OWASP A03: Injection |
| CRITICAL | GS005 | migrate_history.py | 170 | OWASP A03: Injection |
| CRITICAL | GS005 | migrate_history.py | 180 | OWASP A03: Injection |
| CRITICAL | GS005 | migrate_history.py | 193 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8500 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8508 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8563 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8572 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8776 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8790 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8809 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8845 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8869 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8973 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8981 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 8988 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9007 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9113 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9124 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9186 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9191 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9322 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9354 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9368 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9373 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9433 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9522 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9565 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9572 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9585 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9719 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9756 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9760 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9766 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9771 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9800 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9831 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9838 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9845 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9846 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9874 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9878 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 9958 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10011 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10052 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10061 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10074 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10095 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10164 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10168 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10204 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10326 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10331 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10338 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10378 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10401 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10425 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10440 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10471 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10626 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10652 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10673 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10717 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10814 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10951 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10963 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 10985 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11093 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11126 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11135 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11158 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11185 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11225 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11263 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11381 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11458 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11483 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11486 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11543 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11551 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11575 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11614 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11621 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11627 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11685 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11706 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11716 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11721 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11728 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11770 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11775 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11780 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11876 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11892 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11898 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11919 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 11923 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17001 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17005 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17047 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17052 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17053 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17284 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17294 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17304 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 17311 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 18858 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 18879 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 18908 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 18924 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19040 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19054 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19076 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19095 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19322 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19329 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19341 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19347 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19431 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19441 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19877 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 19898 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 21847 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 21867 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 21883 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 21943 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 21956 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22050 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22605 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22618 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22639 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22657 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22828 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22838 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22850 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22861 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22872 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22910 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22933 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22942 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 22951 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 24581 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 24594 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 24609 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 24622 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 24862 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 24882 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 24888 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25047 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25056 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25067 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25074 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25117 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25125 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25135 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25143 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25176 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25182 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25193 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25198 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25227 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25737 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 25845 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27232 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27236 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27254 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27269 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27296 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27323 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27590 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27614 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27623 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27643 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27666 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27722 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27736 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27777 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 28265 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 28360 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 28368 | OWASP A03: Injection |
| CRITICAL | GS005 | app.py | 27006 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | migrate_history.py | 69 |  |
| CRITICAL | GS005 | migrate_history.py | 193 |  |
| CRITICAL | GS005 | app.py | 8500 |  |
| CRITICAL | GS005 | app.py | 8508 |  |
| CRITICAL | GS005 | app.py | 8563 |  |
| CRITICAL | GS005 | app.py | 8572 |  |
| CRITICAL | GS005 | app.py | 8776 |  |
| CRITICAL | GS005 | app.py | 8790 |  |
| CRITICAL | GS005 | app.py | 8809 |  |
| CRITICAL | GS005 | app.py | 8845 |  |
| CRITICAL | GS005 | app.py | 8869 |  |
| CRITICAL | GS005 | app.py | 8973 |  |
| CRITICAL | GS005 | app.py | 8981 |  |
| CRITICAL | GS005 | app.py | 8988 |  |
| CRITICAL | GS005 | app.py | 9007 |  |
| CRITICAL | GS005 | app.py | 9113 |  |
| CRITICAL | GS005 | app.py | 9124 |  |
| CRITICAL | GS005 | app.py | 9186 |  |
| CRITICAL | GS005 | app.py | 9191 |  |
| CRITICAL | GS005 | app.py | 9322 |  |
| CRITICAL | GS005 | app.py | 9354 |  |
| CRITICAL | GS005 | app.py | 9368 |  |
| CRITICAL | GS005 | app.py | 9373 |  |
| CRITICAL | GS005 | app.py | 9433 |  |
| CRITICAL | GS005 | app.py | 9522 |  |
| CRITICAL | GS005 | app.py | 9565 |  |
| CRITICAL | GS005 | app.py | 9572 |  |
| CRITICAL | GS005 | app.py | 9585 |  |
| CRITICAL | GS005 | app.py | 9719 |  |
| CRITICAL | GS005 | app.py | 9756 |  |
| CRITICAL | GS005 | app.py | 9760 |  |
| CRITICAL | GS005 | app.py | 9766 |  |
| CRITICAL | GS005 | app.py | 9771 |  |
| CRITICAL | GS005 | app.py | 9800 |  |
| CRITICAL | GS005 | app.py | 9831 |  |
| CRITICAL | GS005 | app.py | 9838 |  |
| CRITICAL | GS005 | app.py | 9845 |  |
| CRITICAL | GS005 | app.py | 9874 |  |
| CRITICAL | GS005 | app.py | 9878 |  |
| CRITICAL | GS005 | app.py | 9958 |  |
| CRITICAL | GS005 | app.py | 10011 |  |
| CRITICAL | GS005 | app.py | 10052 |  |
| CRITICAL | GS005 | app.py | 10061 |  |
| CRITICAL | GS005 | app.py | 10074 |  |
| CRITICAL | GS005 | app.py | 10095 |  |
| CRITICAL | GS005 | app.py | 10164 |  |
| CRITICAL | GS005 | app.py | 10204 |  |
| CRITICAL | GS005 | app.py | 10326 |  |
| CRITICAL | GS005 | app.py | 10331 |  |
| CRITICAL | GS005 | app.py | 10338 |  |
| CRITICAL | GS005 | app.py | 10378 |  |
| CRITICAL | GS005 | app.py | 10401 |  |
| CRITICAL | GS005 | app.py | 10425 |  |
| CRITICAL | GS005 | app.py | 10440 |  |
| CRITICAL | GS005 | app.py | 10471 |  |
| CRITICAL | GS005 | app.py | 10626 |  |
| CRITICAL | GS005 | app.py | 10652 |  |
| CRITICAL | GS005 | app.py | 10673 |  |
| CRITICAL | GS005 | app.py | 10717 |  |
| CRITICAL | GS005 | app.py | 10814 |  |
| CRITICAL | GS005 | app.py | 10951 |  |
| CRITICAL | GS005 | app.py | 10963 |  |
| CRITICAL | GS005 | app.py | 10985 |  |
| CRITICAL | GS005 | app.py | 11093 |  |
| CRITICAL | GS005 | app.py | 11126 |  |
| CRITICAL | GS005 | app.py | 11135 |  |
| CRITICAL | GS005 | app.py | 11158 |  |
| CRITICAL | GS005 | app.py | 11185 |  |
| CRITICAL | GS005 | app.py | 11225 |  |
| CRITICAL | GS005 | app.py | 11263 |  |
| CRITICAL | GS005 | app.py | 11381 |  |
| CRITICAL | GS005 | app.py | 11458 |  |
| CRITICAL | GS005 | app.py | 11483 |  |
| CRITICAL | GS005 | app.py | 11486 |  |
| CRITICAL | GS005 | app.py | 11543 |  |
| CRITICAL | GS005 | app.py | 11551 |  |
| CRITICAL | GS005 | app.py | 11575 |  |
| CRITICAL | GS005 | app.py | 11614 |  |
| CRITICAL | GS005 | app.py | 11621 |  |
| CRITICAL | GS005 | app.py | 11627 |  |
| CRITICAL | GS005 | app.py | 11685 |  |
| CRITICAL | GS005 | app.py | 11706 |  |
| CRITICAL | GS005 | app.py | 11716 |  |
| CRITICAL | GS005 | app.py | 11721 |  |
| CRITICAL | GS005 | app.py | 11728 |  |
| CRITICAL | GS005 | app.py | 11770 |  |
| CRITICAL | GS005 | app.py | 11775 |  |
| CRITICAL | GS005 | app.py | 11780 |  |
| CRITICAL | GS005 | app.py | 11876 |  |
| CRITICAL | GS005 | app.py | 11892 |  |
| CRITICAL | GS005 | app.py | 11898 |  |
| CRITICAL | GS005 | app.py | 11919 |  |
| CRITICAL | GS005 | app.py | 11923 |  |
| CRITICAL | GS005 | app.py | 17001 |  |
| CRITICAL | GS005 | app.py | 17005 |  |
| CRITICAL | GS005 | app.py | 17047 |  |
| CRITICAL | GS005 | app.py | 17052 |  |
| CRITICAL | GS005 | app.py | 17053 |  |
| CRITICAL | GS005 | app.py | 17284 |  |
| CRITICAL | GS005 | app.py | 17294 |  |
| CRITICAL | GS005 | app.py | 17304 |  |
| CRITICAL | GS005 | app.py | 17311 |  |
| CRITICAL | GS005 | app.py | 21847 |  |
| CRITICAL | GS005 | app.py | 21867 |  |
| CRITICAL | GS005 | app.py | 21883 |  |
| CRITICAL | GS005 | app.py | 21943 |  |
| CRITICAL | GS005 | app.py | 21956 |  |
| CRITICAL | GS005 | app.py | 22050 |  |
| CRITICAL | GS005 | app.py | 22605 |  |
| CRITICAL | GS005 | app.py | 22618 |  |
| CRITICAL | GS005 | app.py | 22828 |  |
| CRITICAL | GS005 | app.py | 22838 |  |
| CRITICAL | GS005 | app.py | 22850 |  |
| CRITICAL | GS005 | app.py | 22861 |  |
| CRITICAL | GS005 | app.py | 22872 |  |
| CRITICAL | GS005 | app.py | 22910 |  |
| CRITICAL | GS005 | app.py | 22933 |  |
| CRITICAL | GS005 | app.py | 22942 |  |
| CRITICAL | GS005 | app.py | 22951 |  |
| CRITICAL | GS005 | app.py | 24862 |  |
| CRITICAL | GS005 | app.py | 24882 |  |
| CRITICAL | GS005 | app.py | 24888 |  |
| CRITICAL | GS005 | app.py | 25047 |  |
| CRITICAL | GS005 | app.py | 25056 |  |
| CRITICAL | GS005 | app.py | 25067 |  |
| CRITICAL | GS005 | app.py | 25074 |  |
| CRITICAL | GS005 | app.py | 25117 |  |
| CRITICAL | GS005 | app.py | 25125 |  |
| CRITICAL | GS005 | app.py | 25135 |  |
| CRITICAL | GS005 | app.py | 25143 |  |
| CRITICAL | GS005 | app.py | 25176 |  |
| CRITICAL | GS005 | app.py | 25182 |  |
| CRITICAL | GS005 | app.py | 25193 |  |
| CRITICAL | GS005 | app.py | 25198 |  |
| CRITICAL | GS005 | app.py | 25227 |  |
| CRITICAL | GS005 | app.py | 25737 |  |
| CRITICAL | GS005 | app.py | 25845 |  |
| CRITICAL | GS005 | app.py | 27232 |  |
| CRITICAL | GS005 | app.py | 27254 |  |
| CRITICAL | GS005 | app.py | 27269 |  |
| CRITICAL | GS005 | app.py | 27296 |  |
| CRITICAL | GS005 | app.py | 27323 |  |
| CRITICAL | GS005 | app.py | 27590 |  |
| CRITICAL | GS005 | app.py | 27614 |  |
| CRITICAL | GS005 | app.py | 27623 |  |
| CRITICAL | GS005 | app.py | 27643 |  |
| CRITICAL | GS005 | app.py | 27666 |  |
| CRITICAL | GS005 | app.py | 27722 |  |
| CRITICAL | GS005 | app.py | 27736 |  |
| CRITICAL | GS005 | app.py | 27777 |  |
| CRITICAL | GS005 | app.py | 28265 |  |
| CRITICAL | GS005 | app.py | 28360 |  |
| CRITICAL | GS005 | app.py | 28368 |  |
| CRITICAL | GS005 | app.py | 8674 | Line 8674: cur.execute(f'ALTER TABLE {t} ADD COLUMN IF NOT E |
| CRITICAL | GS005 | app.py | 8685 | Line 8685: db.execute(f'ALTER TABLE {t} ADD COLUMN {c} {ctyp |
| CRITICAL | GS005 | app.py | 9565 | Line 9565: c2.execute(f"UPDATE horeca_accounts SET lat={ph}, |
| CRITICAL | GS005 | app.py | 9585 | Line 9585: c2.execute(f"UPDATE horeca_accounts SET lat={ph}, |
| CRITICAL | GS005 | app.py | 9756 | Line 9756: cur.execute(f"SELECT id FROM commission_programs  |
| CRITICAL | GS005 | app.py | 9760 | Line 9760: cur.execute(f"UPDATE commission_programs SET per_ |
| CRITICAL | GS005 | app.py | 9766 | Line 9766: cur.execute(f"INSERT INTO commission_programs (sk |
| CRITICAL | GS005 | app.py | 9771 | Line 9771: cur.execute(f"INSERT INTO commission_programs (sk |
| CRITICAL | GS005 | app.py | 9874 | Line 9874: cur.execute(f"UPDATE deals SET payment_status={ph |
| CRITICAL | GS005 | app.py | 9878 | Line 9878: cur.execute(f"UPDATE deals SET payment_status={ph |
| CRITICAL | GS005 | app.py | 9958 | Line 9958: cur.execute(f"DELETE FROM target_list_entries WHE |
| CRITICAL | GS005 | app.py | 10440 | Line 10440: cur.execute(f"UPDATE agco_licensees SET matched_ |
| CRITICAL | GS005 | app.py | 10626 | Line 10626: cur.execute(f"INSERT INTO system_heartbeat (job, |
| CRITICAL | GS005 | app.py | 11337 | Line 11337: cur.execute(f'''CREATE TABLE IF NOT EXISTS actio |
| CRITICAL | GS005 | app.py | 11483 | Line 11483: cur.execute(f"UPDATE action_queue SET status={ph |
| CRITICAL | GS005 | app.py | 11486 | Line 11486: cur.execute(f"UPDATE action_queue SET status={ph |
| CRITICAL | GS005 | app.py | 11543 | Line 11543: cur.execute(f"UPDATE stores SET rep='' WHERE COA |
| CRITICAL | GS005 | app.py | 11551 | Line 11551: c2 = db.execute(f"UPDATE stores SET rep='' WHERE |
| CRITICAL | GS005 | app.py | 11780 | Line 11780: cur.execute(f"UPDATE horeca_accounts SET last_vi |
| CRITICAL | GS005 | app.py | 11892 | Line 11892: cur.execute(f"UPDATE horeca_accounts SET {', '.j |
| CRITICAL | GS005 | app.py | 17001 | Line 17001: cur.execute(f"SELECT COUNT(*) FROM {tname}") |
| CRITICAL | GS005 | app.py | 17005 | Line 17005: row = db.execute(f"SELECT COUNT(*) FROM {tname}" |
| CRITICAL | GS005 | app.py | 17047 | Line 17047: cur.execute(f"SELECT * FROM {tname}") |
| CRITICAL | GS005 | app.py | 17052 | Line 17052: rows_raw = db.execute(f"SELECT * FROM {tname}"). |
| CRITICAL | GS005 | app.py | 17053 | Line 17053: cols = [d[0] for d in db.execute(f"SELECT * FROM |
| CRITICAL | GS005 | migrate_history.py | 193 | Line 193: c.execute(f'SELECT COUNT(*) FROM {t}') |
| CRITICAL | GS005 | sod_durability.py | 108 | Line 108: cur.execute(f""" |
| CRITICAL | GS005 | sod_durability.py | 127 | Line 127: cur.execute(f""" |
| CRITICAL | GS005 | sod_durability.py | 140 | Line 140: cur.execute(f""" |
| HIGH | GS000-LEGACY | app.py | 28208 | File upload without MIME-type validation → malicious file up |
| HIGH | GS025 | app.py | 12035 |  |
| HIGH | GS025 | app.py | 8395 |  |
| HIGH | GS025 | rpr_blitz_seed.json | 0 | Permissions 664 — should be 600 for sensitive files |
| HIGH | GS025 | railway.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | render.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | app.py | 22814 | Line 22814: def _exec(sql: str, params: tuple): |
| HIGH | GS004 | app.py | 22827 | Line 22827: rows = _exec( |
| HIGH | GS004 | app.py | 22837 | Line 22837: rows = _exec( |
| HIGH | GS004 | app.py | 22849 | Line 22849: rows = _exec( |
| HIGH | GS004 | app.py | 22860 | Line 22860: rows = _exec( |
| HIGH | GS004 | app.py | 22871 | Line 22871: rows = _exec( |
| HIGH | GS018 | app.py | 9744 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS019 | app.py | 3345 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | migrate_history.py | 69 |
| C | GS005 | migrate_history.py | 148 |
| C | GS005 | migrate_history.py | 159 |
| C | GS005 | migrate_history.py | 170 |
| C | GS005 | migrate_history.py | 180 |
| C | GS005 | migrate_history.py | 193 |
| C | GS005 | app.py | 8500 |
| C | GS005 | app.py | 8508 |
| C | GS005 | app.py | 8563 |
| C | GS005 | app.py | 8572 |
| C | GS005 | app.py | 8776 |
| C | GS005 | app.py | 8790 |
| C | GS005 | app.py | 8809 |
| C | GS005 | app.py | 8845 |
| C | GS005 | app.py | 8869 |
| C | GS005 | app.py | 8973 |
| C | GS005 | app.py | 8981 |
| C | GS005 | app.py | 8988 |
| C | GS005 | app.py | 9007 |
| C | GS005 | app.py | 9113 |
| C | GS005 | app.py | 9124 |
| C | GS005 | app.py | 9186 |
| C | GS005 | app.py | 9191 |
| C | GS005 | app.py | 9322 |
| C | GS005 | app.py | 9354 |
| C | GS005 | app.py | 9368 |
| C | GS005 | app.py | 9373 |
| C | GS005 | app.py | 9433 |
| C | GS005 | app.py | 9522 |
| C | GS005 | app.py | 9565 |
| C | GS005 | app.py | 9572 |
| C | GS005 | app.py | 9585 |
| C | GS005 | app.py | 9719 |
| C | GS005 | app.py | 9756 |
| C | GS005 | app.py | 9760 |
| C | GS005 | app.py | 9766 |
| C | GS005 | app.py | 9771 |
| C | GS005 | app.py | 9800 |
| C | GS005 | app.py | 9831 |
| C | GS005 | app.py | 9838 |
| C | GS005 | app.py | 9845 |
| C | GS005 | app.py | 9846 |
| C | GS005 | app.py | 9874 |
| C | GS005 | app.py | 9878 |
| C | GS005 | app.py | 9958 |
| C | GS005 | app.py | 10011 |
| C | GS005 | app.py | 10052 |
| C | GS005 | app.py | 10061 |
| C | GS005 | app.py | 10074 |
| C | GS005 | app.py | 10095 |
| C | GS005 | app.py | 10164 |
| C | GS005 | app.py | 10168 |
| C | GS005 | app.py | 10204 |
| C | GS005 | app.py | 10326 |
| C | GS005 | app.py | 10331 |
| C | GS005 | app.py | 10338 |
| C | GS005 | app.py | 10378 |
| C | GS005 | app.py | 10401 |
| C | GS005 | app.py | 10425 |
| C | GS005 | app.py | 10440 |
| C | GS005 | app.py | 10471 |
| C | GS005 | app.py | 10626 |
| C | GS005 | app.py | 10652 |
| C | GS005 | app.py | 10673 |
| C | GS005 | app.py | 10717 |
| C | GS005 | app.py | 10814 |
| C | GS005 | app.py | 10951 |
| C | GS005 | app.py | 10963 |
| C | GS005 | app.py | 10985 |
| C | GS005 | app.py | 11093 |
| C | GS005 | app.py | 11126 |
| C | GS005 | app.py | 11135 |
| C | GS005 | app.py | 11158 |
| C | GS005 | app.py | 11185 |
| C | GS005 | app.py | 11225 |
| C | GS005 | app.py | 11263 |
| C | GS005 | app.py | 11381 |
| C | GS005 | app.py | 11458 |
| C | GS005 | app.py | 11483 |
| C | GS005 | app.py | 11486 |
| C | GS005 | app.py | 11543 |
| C | GS005 | app.py | 11551 |
| C | GS005 | app.py | 11575 |
| C | GS005 | app.py | 11614 |
| C | GS005 | app.py | 11621 |
| C | GS005 | app.py | 11627 |
| C | GS005 | app.py | 11685 |
| C | GS005 | app.py | 11706 |
| C | GS005 | app.py | 11716 |
| C | GS005 | app.py | 11721 |
| C | GS005 | app.py | 11728 |
| C | GS005 | app.py | 11770 |
| C | GS005 | app.py | 11775 |
| C | GS005 | app.py | 11780 |
| C | GS005 | app.py | 11876 |
| C | GS005 | app.py | 11892 |
| C | GS005 | app.py | 11898 |
| C | GS005 | app.py | 11919 |
| C | GS005 | app.py | 11923 |
| C | GS005 | app.py | 17001 |
| C | GS005 | app.py | 17005 |
| C | GS005 | app.py | 17047 |
| C | GS005 | app.py | 17052 |
| C | GS005 | app.py | 17053 |
| C | GS005 | app.py | 17284 |
| C | GS005 | app.py | 17294 |
| C | GS005 | app.py | 17304 |
| C | GS005 | app.py | 17311 |
| C | GS005 | app.py | 18858 |
| C | GS005 | app.py | 18879 |
| C | GS005 | app.py | 18908 |
| C | GS005 | app.py | 18924 |
| C | GS005 | app.py | 19040 |
| C | GS005 | app.py | 19054 |
| C | GS005 | app.py | 19076 |
| C | GS005 | app.py | 19095 |
| C | GS005 | app.py | 19322 |
| C | GS005 | app.py | 19329 |
| C | GS005 | app.py | 19341 |
| C | GS005 | app.py | 19347 |
| C | GS005 | app.py | 19431 |
| C | GS005 | app.py | 19441 |
| C | GS005 | app.py | 19877 |
| C | GS005 | app.py | 19898 |
| C | GS005 | app.py | 21847 |
| C | GS005 | app.py | 21867 |
| C | GS005 | app.py | 21883 |
| C | GS005 | app.py | 21943 |
| C | GS005 | app.py | 21956 |
| C | GS005 | app.py | 22050 |
| C | GS005 | app.py | 22605 |
| C | GS005 | app.py | 22618 |
| C | GS005 | app.py | 22639 |
| C | GS005 | app.py | 22657 |
| C | GS005 | app.py | 22828 |
| C | GS005 | app.py | 22838 |
| C | GS005 | app.py | 22850 |
| C | GS005 | app.py | 22861 |
| C | GS005 | app.py | 22872 |
| C | GS005 | app.py | 22910 |
| C | GS005 | app.py | 22933 |
| C | GS005 | app.py | 22942 |
| C | GS005 | app.py | 22951 |
| C | GS005 | app.py | 24581 |
| C | GS005 | app.py | 24594 |
| C | GS005 | app.py | 24609 |
| C | GS005 | app.py | 24622 |
| C | GS005 | app.py | 24862 |
| C | GS005 | app.py | 24882 |
| C | GS005 | app.py | 24888 |
| C | GS005 | app.py | 25047 |
| C | GS005 | app.py | 25056 |
| C | GS005 | app.py | 25067 |
| C | GS005 | app.py | 25074 |
| C | GS005 | app.py | 25117 |
| C | GS005 | app.py | 25125 |
| C | GS005 | app.py | 25135 |
| C | GS005 | app.py | 25143 |
| C | GS005 | app.py | 25176 |
| C | GS005 | app.py | 25182 |
| C | GS005 | app.py | 25193 |
| C | GS005 | app.py | 25198 |
| C | GS005 | app.py | 25227 |
| C | GS005 | app.py | 25737 |
| C | GS005 | app.py | 25845 |
| C | GS005 | app.py | 27232 |
| C | GS005 | app.py | 27236 |
| C | GS005 | app.py | 27254 |
| C | GS005 | app.py | 27269 |
| C | GS005 | app.py | 27296 |
| C | GS005 | app.py | 27323 |
| C | GS005 | app.py | 27590 |
| C | GS005 | app.py | 27614 |
| C | GS005 | app.py | 27623 |
| C | GS005 | app.py | 27643 |
| C | GS005 | app.py | 27666 |
| C | GS005 | app.py | 27722 |
| C | GS005 | app.py | 27736 |
| C | GS005 | app.py | 27777 |
| C | GS005 | app.py | 28265 |
| C | GS005 | app.py | 28360 |
| C | GS005 | app.py | 28368 |
| C | GS005 | app.py | 27006 |
| H | GS000-LEGACY | app.py | 28208 |
| M | GS025 | app.py | 22568 |
| C | GS005 | migrate_history.py | 69 |
| C | GS005 | migrate_history.py | 193 |
| C | GS005 | app.py | 8500 |
| C | GS005 | app.py | 8508 |
| C | GS005 | app.py | 8563 |
| C | GS005 | app.py | 8572 |
| C | GS005 | app.py | 8776 |
| C | GS005 | app.py | 8790 |
| C | GS005 | app.py | 8809 |
| C | GS005 | app.py | 8845 |
| C | GS005 | app.py | 8869 |
| C | GS005 | app.py | 8973 |
| C | GS005 | app.py | 8981 |
| C | GS005 | app.py | 8988 |
| C | GS005 | app.py | 9007 |
| C | GS005 | app.py | 9113 |
| C | GS005 | app.py | 9124 |
| C | GS005 | app.py | 9186 |
| C | GS005 | app.py | 9191 |
| C | GS005 | app.py | 9322 |
| C | GS005 | app.py | 9354 |
| C | GS005 | app.py | 9368 |
| C | GS005 | app.py | 9373 |
| C | GS005 | app.py | 9433 |
| C | GS005 | app.py | 9522 |
| C | GS005 | app.py | 9565 |
| C | GS005 | app.py | 9572 |
| C | GS005 | app.py | 9585 |
| C | GS005 | app.py | 9719 |
| C | GS005 | app.py | 9756 |
| C | GS005 | app.py | 9760 |
| C | GS005 | app.py | 9766 |
| C | GS005 | app.py | 9771 |
| C | GS005 | app.py | 9800 |
| C | GS005 | app.py | 9831 |
| C | GS005 | app.py | 9838 |
| C | GS005 | app.py | 9845 |
| C | GS005 | app.py | 9874 |
| C | GS005 | app.py | 9878 |
| C | GS005 | app.py | 9958 |
| C | GS005 | app.py | 10011 |
| C | GS005 | app.py | 10052 |
| C | GS005 | app.py | 10061 |
| C | GS005 | app.py | 10074 |
| C | GS005 | app.py | 10095 |
| C | GS005 | app.py | 10164 |
| C | GS005 | app.py | 10204 |
| C | GS005 | app.py | 10326 |
| C | GS005 | app.py | 10331 |
| C | GS005 | app.py | 10338 |
| C | GS005 | app.py | 10378 |
| C | GS005 | app.py | 10401 |
| C | GS005 | app.py | 10425 |
| C | GS005 | app.py | 10440 |
| C | GS005 | app.py | 10471 |
| C | GS005 | app.py | 10626 |
| C | GS005 | app.py | 10652 |
| C | GS005 | app.py | 10673 |
| C | GS005 | app.py | 10717 |
| C | GS005 | app.py | 10814 |
| C | GS005 | app.py | 10951 |
| C | GS005 | app.py | 10963 |
| C | GS005 | app.py | 10985 |
| C | GS005 | app.py | 11093 |
| C | GS005 | app.py | 11126 |
| C | GS005 | app.py | 11135 |
| C | GS005 | app.py | 11158 |
| C | GS005 | app.py | 11185 |
| C | GS005 | app.py | 11225 |
| C | GS005 | app.py | 11263 |
| C | GS005 | app.py | 11381 |
| C | GS005 | app.py | 11458 |
| C | GS005 | app.py | 11483 |
| C | GS005 | app.py | 11486 |
| C | GS005 | app.py | 11543 |
| C | GS005 | app.py | 11551 |
| C | GS005 | app.py | 11575 |
| C | GS005 | app.py | 11614 |
| C | GS005 | app.py | 11621 |
| C | GS005 | app.py | 11627 |
| C | GS005 | app.py | 11685 |
| C | GS005 | app.py | 11706 |
| C | GS005 | app.py | 11716 |
| C | GS005 | app.py | 11721 |
| C | GS005 | app.py | 11728 |
| C | GS005 | app.py | 11770 |
| C | GS005 | app.py | 11775 |
| C | GS005 | app.py | 11780 |
| C | GS005 | app.py | 11876 |
| C | GS005 | app.py | 11892 |
| C | GS005 | app.py | 11898 |
| C | GS005 | app.py | 11919 |
| C | GS005 | app.py | 11923 |
| C | GS005 | app.py | 17001 |
| C | GS005 | app.py | 17005 |
| C | GS005 | app.py | 17047 |
| C | GS005 | app.py | 17052 |
| C | GS005 | app.py | 17053 |
| C | GS005 | app.py | 17284 |
| C | GS005 | app.py | 17294 |
| C | GS005 | app.py | 17304 |
| C | GS005 | app.py | 17311 |
| C | GS005 | app.py | 21847 |
| C | GS005 | app.py | 21867 |
| C | GS005 | app.py | 21883 |
| C | GS005 | app.py | 21943 |
| C | GS005 | app.py | 21956 |
| C | GS005 | app.py | 22050 |
| C | GS005 | app.py | 22605 |
| C | GS005 | app.py | 22618 |
| C | GS005 | app.py | 22828 |
| C | GS005 | app.py | 22838 |
| C | GS005 | app.py | 22850 |
| C | GS005 | app.py | 22861 |
| C | GS005 | app.py | 22872 |
| C | GS005 | app.py | 22910 |
| C | GS005 | app.py | 22933 |
| C | GS005 | app.py | 22942 |
| C | GS005 | app.py | 22951 |
| C | GS005 | app.py | 24862 |
| C | GS005 | app.py | 24882 |
| C | GS005 | app.py | 24888 |
| C | GS005 | app.py | 25047 |
| C | GS005 | app.py | 25056 |
| C | GS005 | app.py | 25067 |
| C | GS005 | app.py | 25074 |
| C | GS005 | app.py | 25117 |
| C | GS005 | app.py | 25125 |
| C | GS005 | app.py | 25135 |
| C | GS005 | app.py | 25143 |
| C | GS005 | app.py | 25176 |
| C | GS005 | app.py | 25182 |
| C | GS005 | app.py | 25193 |
| C | GS005 | app.py | 25198 |
| C | GS005 | app.py | 25227 |
| C | GS005 | app.py | 25737 |
| C | GS005 | app.py | 25845 |
| C | GS005 | app.py | 27232 |
| C | GS005 | app.py | 27254 |
| C | GS005 | app.py | 27269 |
| C | GS005 | app.py | 27296 |
| C | GS005 | app.py | 27323 |
| C | GS005 | app.py | 27590 |
| C | GS005 | app.py | 27614 |
| C | GS005 | app.py | 27623 |
| C | GS005 | app.py | 27643 |
| C | GS005 | app.py | 27666 |
| C | GS005 | app.py | 27722 |
| C | GS005 | app.py | 27736 |
| C | GS005 | app.py | 27777 |
| C | GS005 | app.py | 28265 |
| C | GS005 | app.py | 28360 |
| C | GS005 | app.py | 28368 |
| H | GS025 | app.py | 12035 |
| H | GS025 | app.py | 8395 |
| M | GS029 | app.py | 26843 |
| L | GS003 | seed_demo.py | 142 |
| L | GS003 | seed_demo.py | 144 |
| L | GS003 | seed_demo.py | 145 |
| L | GS003 | seed_demo.py | 146 |
| L | GS003 | seed_demo.py | 147 |
| L | GS003 | seed_demo.py | 148 |
| L | GS008 | app.py | 10868 |
| L | GS008 | app.py | 10869 |
| L | GS008 | sod_durability.py | 48 |
| I | GS015 | app.py | 190 |
| I | GS015 | app.py | 199 |
| I | GS015 | app.py | 1750 |
| I | GS015 | app.py | 1755 |
| I | GS015 | app.py | 1809 |
| I | GS015 | app.py | 1817 |
| I | GS015 | app.py | 1838 |
| I | GS015 | app.py | 1880 |
| I | GS015 | app.py | 1886 |
| I | GS015 | app.py | 1946 |
| I | GS015 | app.py | 190 |
| I | GS015 | app.py | 199 |
| I | GS015 | app.py | 1750 |
| I | GS015 | app.py | 1755 |
| I | GS015 | app.py | 1809 |
| I | GS015 | app.py | 1817 |
| I | GS015 | app.py | 1838 |
| I | GS015 | app.py | 1880 |
| I | GS015 | app.py | 1886 |
| I | GS015 | app.py | 1946 |
| I | GS015 | app.py | 190 |
| I | GS015 | app.py | 199 |
| I | GS015 | app.py | 1750 |
| I | GS015 | app.py | 1755 |
| I | GS015 | app.py | 1809 |
| I | GS015 | app.py | 1817 |
| I | GS015 | app.py | 1838 |
| I | GS015 | app.py | 1880 |
| I | GS015 | app.py | 1886 |
| I | GS015 | app.py | 1946 |
| I | GS015 | app.py | 54 |
| i | GS020 |  | 79 |
| i | GS020 |  | 106 |
| i | GS020 |  | 122 |
| i | GS020 |  | 130 |
| i | GS020 |  | 133 |
| i | GS020 |  | 165 |
| i | GS020 |  | 180 |
| i | GS020 |  | 191 |
| i | GS020 |  | 213 |
| i | GS020 |  | 229 |
| i | GS020 |  | 247 |
| i | GS020 |  | 256 |
| i | GS020 |  | 259 |
| i | GS020 |  | 280 |
| i | GS020 |  | 299 |
| i | GS020 |  | 316 |
| i | GS020 |  | 324 |
| i | GS020 |  | 361 |
| i | GS020 |  | 434 |
| i | GS020 |  | 482 |
| i | GS020 |  | 483 |
| i | GS020 |  | 523 |
| i | GS020 |  | 527 |
| i | GS020 |  | 541 |
| i | GS020 |  | 577 |
| i | GS020 |  | 635 |
| i | GS020 |  | 639 |
| i | GS020 |  | 673 |
| i | GS020 |  | 684 |
| i | GS020 |  | 724 |
| i | GS020 |  | 739 |
| i | GS020 |  | 748 |
| i | GS020 |  | 755 |
| i | GS020 |  | 763 |
| i | GS020 |  | 768 |
| i | GS020 |  | 789 |
| i | GS020 |  | 847 |
| i | GS020 |  | 869 |
| i | GS020 |  | 870 |
| i | GS020 |  | 871 |
| i | GS020 |  | 886 |
| i | GS020 |  | 892 |
| i | GS020 |  | 896 |
| i | GS020 |  | 940 |
| i | GS020 |  | 941 |
| i | GS020 |  | 950 |
| i | GS020 |  | 970 |
| i | GS020 |  | 1072 |
| i | GS020 |  | 1098 |
| i | GS020 |  | 1125 |
| i | GS020 |  | 1153 |
| i | GS020 |  | 1192 |
| i | GS020 |  | 1201 |
| i | GS020 |  | 1206 |
| i | GS020 |  | 1223 |
| i | GS020 |  | 1241 |
| i | GS020 |  | 1248 |
| i | GS020 |  | 1292 |
| i | GS020 |  | 1303 |
| i | GS020 |  | 1311 |
| i | GS020 |  | 1334 |
| i | GS020 |  | 1365 |
| i | GS020 |  | 1371 |
| i | GS020 |  | 1397 |
| i | GS020 |  | 1413 |
| i | GS020 |  | 1422 |
| i | GS020 |  | 1448 |
| i | GS020 |  | 1457 |
| i | GS020 |  | 1458 |
| i | GS020 |  | 1468 |
| i | GS020 |  | 1478 |
| i | GS020 |  | 1479 |
| i | GS020 |  | 1509 |
| i | GS020 |  | 1517 |
| i | GS020 |  | 1518 |
| i | GS020 |  | 1532 |
| i | GS020 |  | 1608 |
| i | GS020 |  | 1612 |
| i | GS020 |  | 1631 |
| i | GS020 |  | 1632 |
| i | GS020 |  | 1700 |
| i | GS020 |  | 1701 |
| i | GS020 |  | 1758 |
| i | GS020 |  | 190 |
| i | GS020 |  | 245 |
| i | GS020 |  | 280 |
| i | GS020 |  | 321 |
| i | GS020 |  | 541 |
| i | GS020 |  | 739 |
| i | GS020 |  | 775 |
| i | GS020 |  | 856 |
| i | GS020 |  | 984 |
| i | GS020 |  | 1037 |
| i | GS020 |  | 1583 |
| i | GS020 |  | 1590 |
| i | GS020 |  | 1658 |
| ? | GS032-exfil_curl | app.py | 12035 |
| H | GS025 | rpr_blitz_seed.json | 0 |
| H | GS025 | railway.json | 0 |
| H | GS025 | render.yaml | 0 |
| H | GS004 | app.py | 22814 |
| H | GS004 | app.py | 22827 |
| H | GS004 | app.py | 22837 |
| H | GS004 | app.py | 22849 |
| H | GS004 | app.py | 22860 |
| H | GS004 | app.py | 22871 |
| C | GS005 | app.py | 8674 |
| C | GS005 | app.py | 8685 |
| C | GS005 | app.py | 9565 |
| C | GS005 | app.py | 9585 |
| C | GS005 | app.py | 9756 |
| C | GS005 | app.py | 9760 |
| C | GS005 | app.py | 9766 |
| C | GS005 | app.py | 9771 |
| C | GS005 | app.py | 9874 |
| C | GS005 | app.py | 9878 |
| C | GS005 | app.py | 9958 |
| C | GS005 | app.py | 10440 |
| C | GS005 | app.py | 10626 |
| C | GS005 | app.py | 11337 |
| C | GS005 | app.py | 11483 |
| C | GS005 | app.py | 11486 |
| C | GS005 | app.py | 11543 |
| C | GS005 | app.py | 11551 |
| C | GS005 | app.py | 11780 |
| C | GS005 | app.py | 11892 |
| C | GS005 | app.py | 17001 |
| C | GS005 | app.py | 17005 |
| C | GS005 | app.py | 17047 |
| C | GS005 | app.py | 17052 |
| C | GS005 | app.py | 17053 |
| C | GS005 | migrate_history.py | 193 |
| C | GS005 | sod_durability.py | 108 |
| C | GS005 | sod_durability.py | 127 |
| C | GS005 | sod_durability.py | 140 |
| I | GS007 | app.py | 1200 |
| I | GS007 | app.py | 1203 |
| I | GS007 | app.py | 1213 |
| I | GS007 | app.py | 1220 |
| I | GS007 | app.py | 1233 |
| I | GS007 | app.py | 1251 |
| I | GS007 | app.py | 1258 |
| I | GS007 | app.py | 1273 |
| I | GS007 | app.py | 1287 |
| I | GS007 | app.py | 1311 |
| I | GS007 | app.py | 1321 |
| I | GS007 | app.py | 1345 |
| I | GS007 | app.py | 1356 |
| I | GS007 | app.py | 1370 |
| I | GS007 | app.py | 1403 |
| I | GS007 | app.py | 1423 |
| I | GS007 | app.py | 1436 |
| I | GS007 | app.py | 1445 |
| I | GS007 | app.py | 1455 |
| I | GS007 | app.py | 1532 |
| I | GS007 | app.py | 1557 |
| I | GS007 | app.py | 1578 |
| I | GS007 | app.py | 1594 |
| I | GS007 | app.py | 1611 |
| I | GS007 | app.py | 1625 |
| I | GS007 | app.py | 8626 |
| I | GS007 | app.py | 9652 |
| I | GS007 | app.py | 10581 |
| I | GS007 | app.py | 10877 |
| I | GS007 | app.py | 11335 |
| I | GS007 | app.py | 27126 |
| I | GS007 | app.py | 27411 |
| I | GS007 | app.py | 579 |
| I | GS007 | app.py | 602 |
| I | GS007 | app.py | 608 |
| I | GS007 | app.py | 621 |
| I | GS007 | app.py | 633 |
| I | GS007 | app.py | 644 |
| I | GS007 | app.py | 711 |
| I | GS007 | app.py | 722 |
| I | GS007 | app.py | 744 |
| I | GS007 | app.py | 760 |
| I | GS007 | app.py | 788 |
| I | GS007 | app.py | 816 |
| I | GS007 | app.py | 848 |
| I | GS007 | app.py | 861 |
| I | GS007 | app.py | 877 |
| I | GS007 | app.py | 918 |
| I | GS007 | app.py | 941 |
| I | GS007 | app.py | 957 |
| I | GS007 | app.py | 968 |
| I | GS007 | app.py | 980 |
| I | GS007 | app.py | 1049 |
| I | GS007 | app.py | 1077 |
| I | GS007 | app.py | 1100 |
| I | GS007 | app.py | 1118 |
| I | GS007 | app.py | 1143 |
| I | GS007 | app.py | 1167 |
| I | GS007 | app.py | 8626 |
| I | GS007 | app.py | 9652 |
| I | GS007 | app.py | 10581 |
| I | GS007 | app.py | 10877 |
| I | GS007 | app.py | 11335 |
| I | GS007 | app.py | 27126 |
| I | GS007 | app.py | 27411 |
| I | GS007 | sod_durability.py | 103 |
| I | GS007 | sod_durability.py | 103 |
| s | GS009 |  | 0 |
| H | GS018 | app.py | 9744 |
| H | GS019 | app.py | 3345 |
| c | GS021 |  | 199 |
| c | GS021 |  | 1886 |
| c | GS021 |  | 2125 |
| c | GS021 |  | 2134 |
| c | GS021 |  | 2170 |
| c | GS021 |  | 2418 |
| c | GS021 |  | 2961 |
| c | GS021 |  | 4860 |
| c | GS021 |  | 4948 |
| c | GS021 |  | 5072 |
| c | GS021 |  | 5098 |
| c | GS021 |  | 5963 |
| c | GS021 |  | 6212 |
| c | GS021 |  | 6469 |
| c | GS021 |  | 6847 |
| c | GS021 |  | 7340 |
| c | GS021 |  | 7580 |
| c | GS021 |  | 7943 |
| c | GS021 |  | 8006 |
| c | GS021 |  | 8129 |
| c | GS021 |  | 8366 |
| c | GS021 |  | 8831 |
| c | GS021 |  | 8856 |
| c | GS021 |  | 8915 |
| c | GS021 |  | 9041 |
| c | GS021 |  | 9383 |
| c | GS021 |  | 9508 |
| c | GS021 |  | 9593 |
| c | GS021 |  | 9736 |
| c | GS021 |  | 9781 |
| c | GS021 |  | 9862 |
| c | GS021 |  | 10022 |
| c | GS021 |  | 10037 |
| c | GS021 |  | 10359 |
| c | GS021 |  | 10828 |
| c | GS021 |  | 11050 |
| c | GS021 |  | 11079 |
| c | GS021 |  | 11104 |
| c | GS021 |  | 11143 |
| c | GS021 |  | 11438 |
| c | GS021 |  | 11471 |
| c | GS021 |  | 11527 |
| c | GS021 |  | 11591 |
| c | GS021 |  | 11758 |
| c | GS021 |  | 11826 |
| c | GS021 |  | 12243 |
| c | GS021 |  | 13584 |
| c | GS021 |  | 14594 |
| c | GS021 |  | 14877 |
| c | GS021 |  | 14959 |
| c | GS021 |  | 15062 |
| c | GS021 |  | 15241 |
| c | GS021 |  | 15476 |
| c | GS021 |  | 16823 |
| c | GS021 |  | 17230 |
| c | GS021 |  | 17254 |
| c | GS021 |  | 17582 |
| c | GS021 |  | 18409 |
| c | GS021 |  | 18417 |
| c | GS021 |  | 21567 |
| c | GS021 |  | 23093 |
| c | GS021 |  | 23149 |
| c | GS021 |  | 23291 |
| c | GS021 |  | 23553 |
| c | GS021 |  | 24837 |
| c | GS021 |  | 24908 |
| c | GS021 |  | 25024 |
| c | GS021 |  | 25097 |
| c | GS021 |  | 25156 |
| c | GS021 |  | 25318 |
| c | GS021 |  | 26091 |
| c | GS021 |  | 26405 |
| c | GS021 |  | 26596 |
| c | GS021 |  | 26729 |
| c | GS021 |  | 26757 |
| c | GS021 |  | 27898 |
| c | GS021 |  | 28229 |
| c | GS021 |  | 28300 |
| c | GS021 |  | 28417 |
| s | GS021 |  | 216 |
| s | GS021 |  | 217 |
| s | GS021 |  | 282 |
| s | GS021 |  | 286 |
| s | GS021 |  | 286 |
| s | GS021 |  | 346 |
| s | GS021 |  | 347 |
| s | GS021 |  | 348 |
| s | GS021 |  | 28999 |
| r | GS022 |  | 360 |
| r | GS022 |  | 361 |
| r | GS022 |  | 3773 |
| r | GS022 |  | 9269 |
| r | GS022 |  | 9487 |
| r | GS022 |  | 15276 |
| r | GS022 |  | 53 |
| r | GS022 |  | 92 |
| r | GS022 |  | 92 |
| ? | GS025-wildcard_bind |  | ? |
| ? | YAML-B39DC08C | app.py | ? |
| ? | YAML-B39DC08C | setup-everything.sh | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-11T06:20:32.180906*