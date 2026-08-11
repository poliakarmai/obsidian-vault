---
title: "GSC Audit: /tmp/gsc-learn/hypothesis"
date: 2026-07-31
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/hypothesis

**Дата:** 31.07.2026 04:01  
**Путь:** `/tmp/gsc-learn/hypothesis`  
**Всего находок:** 853  
**CRITICAL:** 2 | **HIGH:** 51 | **MEDIUM:** 493 | **LOW:** 304

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 471 |
| GS003 | 40 |
| GS008 | 28 |
| Хардкод IP адреса | 25 |
| CVE-2026-54696: Buffer overflow | 12 |
| Python: File upload without content-type validation | 10 |
| CVE-2026-56233: Path traversal | 7 |
| CVE-2026-37270: Hardcoded credential | 6 |
| GS004 | 5 |
| Generic code smell #24 | 4 |
| Generic code smell #27 | 4 |
| Generic code smell #30 | 4 |
| Generic code smell #33 | 4 |
| Generic code smell #36 | 4 |
| Generic code smell #39 | 4 |
| Generic code smell #42 | 4 |
| Generic code smell #45 | 4 |
| Generic code smell #48 | 4 |
| Generic code smell #51 | 4 |
| Generic code smell #54 | 4 |
| Generic code smell #57 | 4 |
| Generic code smell #60 | 4 |
| Generic code smell #63 | 4 |
| Generic code smell #66 | 4 |
| Generic code smell #69 | 4 |
| Generic code smell #72 | 4 |
| Generic code smell #75 | 4 |
| Generic code smell #78 | 4 |
| Generic code smell #81 | 4 |
| Generic code smell #84 | 4 |
| Generic code smell #87 | 4 |
| Generic code smell #90 | 4 |
| Generic code smell #93 | 4 |
| Generic code smell #96 | 4 |
| Generic code smell #99 | 4 |
| Generic code smell #102 | 4 |
| Generic code smell #105 | 4 |
| Generic code smell #108 | 4 |
| Generic code smell #111 | 4 |
| Generic code smell #114 | 4 |
| Generic code smell #117 | 4 |
| Generic code smell #120 | 4 |
| Generic code smell #123 | 4 |
| Generic code smell #126 | 4 |
| Generic code smell #129 | 4 |
| Generic code smell #132 | 4 |
| Generic code smell #135 | 4 |
| Generic code smell #138 | 4 |
| Generic code smell #141 | 4 |
| Generic code smell #144 | 4 |
| Generic code smell #147 | 4 |
| Generic code smell #150 | 4 |
| Generic code smell #153 | 4 |
| Generic code smell #156 | 4 |
| Generic code smell #159 | 4 |
| Generic code smell #162 | 4 |
| Generic code smell #165 | 4 |
| Generic code smell #168 | 4 |
| Generic code smell #171 | 4 |
| Generic code smell #174 | 4 |
| Generic code smell #177 | 4 |
| Generic code smell #180 | 4 |
| Generic code smell #183 | 4 |
| Generic code smell #186 | 4 |
| Generic code smell #189 | 4 |
| Generic code smell #192 | 4 |
| Generic code smell #195 | 4 |
| Generic code smell #198 | 4 |
| eval() or exec() usage | 3 |
| Синхронный код в async | 3 |
| GS007 | 2 |
| CVE-2026-56413: Command injection | 1 |
| Hardcoded encryption key | 1 |
| Outdated dependency pattern | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | installers.py | 94 |  |
| CRITICAL | ? | regex.py | 67 | Match:     st.builds(dict), key="hypothesis.regex.group_cach |
| HIGH | ? | engine.py | 924 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | redis.py | 117 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | core.py | 2363 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | database.py | 266 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | database.py | 269 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | database.py | 499 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | database.py | 534 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | database.py | 542 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | database.py | 548 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | database.py | 797 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | ghostwriter.py | 718 |  |
| HIGH | ? | pelicanconf.py | 42 |  |
| HIGH | ? | pelicanconf.py | 43 |  |
| HIGH | ? | pelicanconf.py | 44 |  |
| HIGH | ? | pelicanconf.py | 47 |  |
| HIGH | ? | pelicanconf.py | 48 |  |
| HIGH | ? | pelicanconf.py | 49 |  |
| HIGH | ? | ipaddress.py | 23 | Match:     "0.0.0.0/8", |
| HIGH | ? | ipaddress.py | 24 | Match:     "10.0.0.0/8", |
| HIGH | ? | ipaddress.py | 25 | Match:     "100.64.0.0/10", |
| HIGH | ? | ipaddress.py | 26 | Match:     "127.0.0.0/8", |
| HIGH | ? | ipaddress.py | 27 | Match:     "169.254.0.0/16", |
| HIGH | ? | ipaddress.py | 28 | Match:     "172.16.0.0/12", |
| HIGH | ? | ipaddress.py | 29 | Match:     "192.0.0.0/24", |
| HIGH | ? | ipaddress.py | 30 | Match:     "192.0.0.0/29", |
| HIGH | ? | ipaddress.py | 31 | Match:     "192.0.0.8/32", |
| HIGH | ? | ipaddress.py | 32 | Match:     "192.0.0.9/32", |
| HIGH | ? | ipaddress.py | 33 | Match:     "192.0.0.10/32", |
| HIGH | ? | ipaddress.py | 34 | Match:     "192.0.0.170/32", |
| HIGH | ? | ipaddress.py | 35 | Match:     "192.0.0.171/32", |
| HIGH | ? | ipaddress.py | 36 | Match:     "192.0.2.0/24", |
| HIGH | ? | ipaddress.py | 37 | Match:     "192.31.196.0/24", |
| HIGH | ? | ipaddress.py | 38 | Match:     "192.52.193.0/24", |
| HIGH | ? | ipaddress.py | 39 | Match:     "192.88.99.0/24", |
| HIGH | ? | ipaddress.py | 40 | Match:     "192.168.0.0/16", |
| HIGH | ? | ipaddress.py | 41 | Match:     "192.175.48.0/24", |
| HIGH | ? | ipaddress.py | 42 | Match:     "198.18.0.0/15", |
| HIGH | ? | ipaddress.py | 43 | Match:     "198.51.100.0/24", |
| HIGH | ? | ipaddress.py | 44 | Match:     "203.0.113.0/24", |
| HIGH | ? | ipaddress.py | 45 | Match:     "240.0.0.0/4", |
| HIGH | ? | ipaddress.py | 46 | Match:     "255.255.255.255/32", |
| HIGH | ? | ipaddress.py | 85 | Match:     ``"127.0.0.0/24"`` or ``"2001:db8::/32"``.  As we |
| HIGH | ? | reflection.py | 358 | Match:     exec(source, result.__dict__) |
| HIGH | ? | lambda_sources.py | 253 | Match:         compiled = eval(source, f_globals) |
| HIGH | ? | lambda_sources.py | 286 | Match:         exec(exec_str, f_globals) |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | lambda_sources.py | 286 | Line 286: exec(exec_str, f_globals) |
| HIGH | GS004 | reflection.py | 358 | Line 358: exec(source, result.__dict__) |
| HIGH | GS004 | installers.py | 66 | Line 66: subprocess.check_call( |
| HIGH | GS004 | installers.py | 94 | Line 94: subprocess.check_call("mkdir -p ~/.local/bin", shel |
| HIGH | GS004 | installers.py | 98 | Line 98: subprocess.check_call( |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| L | ? | ghostwriter.py | 1106 |
| L | ? | ghostwriter.py | 1108 |
| L | ? | strategies.py | 305 |
| L | ? | strategies.py | 396 |
| M | ? | graph.py | 53 |
| M | ? | graph.py | 56 |
| M | ? | validate_branch_check.py | 36 |
| M | ? | compat.py | 221 |
| M | ? | cache.py | 95 |
| M | ? | cache.py | 129 |
| M | ? | cache.py | 135 |
| M | ? | cache.py | 205 |
| M | ? | cache.py | 207 |
| M | ? | cache.py | 210 |
| M | ? | cache.py | 223 |
| M | ? | cache.py | 224 |
| M | ? | cache.py | 255 |
| M | ? | cache.py | 314 |
| M | ? | scrutineer.py | 202 |
| M | ? | scrutineer.py | 212 |
| M | ? | statistics.py | 29 |
| M | ? | statistics.py | 230 |
| M | ? | floats.py | 29 |
| M | ? | floats.py | 46 |
| M | ? | floats.py | 108 |
| M | ? | floats.py | 109 |
| M | ? | pareto.py | 73 |
| M | ? | pareto.py | 77 |
| M | ? | pareto.py | 156 |
| M | ? | pareto.py | 158 |
| M | ? | pareto.py | 172 |
| M | ? | pareto.py | 203 |
| M | ? | pareto.py | 303 |
| M | ? | pareto.py | 323 |
| M | ? | pareto.py | 329 |
| M | ? | datatree.py | 69 |
| M | ? | datatree.py | 96 |
| M | ? | datatree.py | 100 |
| M | ? | datatree.py | 120 |
| M | ? | datatree.py | 213 |
| M | ? | datatree.py | 433 |
| M | ? | datatree.py | 453 |
| M | ? | datatree.py | 475 |
| M | ? | datatree.py | 522 |
| M | ? | datatree.py | 710 |
| M | ? | datatree.py | 715 |
| M | ? | datatree.py | 721 |
| M | ? | datatree.py | 768 |
| M | ? | datatree.py | 772 |
| M | ? | datatree.py | 808 |
| M | ? | datatree.py | 868 |
| M | ? | datatree.py | 896 |
| M | ? | datatree.py | 940 |
| M | ? | datatree.py | 982 |
| M | ? | datatree.py | 1041 |
| M | ? | datatree.py | 1066 |
| M | ? | datatree.py | 1068 |
| M | ? | datatree.py | 1101 |
| M | ? | datatree.py | 1105 |
| M | ? | datatree.py | 1112 |
| M | ? | datatree.py | 1189 |
| M | ? | datatree.py | 1191 |
| M | ? | data.py | 277 |
| M | ? | data.py | 336 |
| M | ? | data.py | 649 |
| M | ? | data.py | 675 |
| M | ? | data.py | 841 |
| M | ? | data.py | 882 |
| M | ? | data.py | 883 |
| M | ? | data.py | 884 |
| M | ? | data.py | 888 |
| M | ? | data.py | 891 |
| M | ? | data.py | 894 |
| M | ? | data.py | 896 |
| M | ? | data.py | 922 |
| M | ? | data.py | 923 |
| M | ? | data.py | 924 |
| M | ? | data.py | 937 |
| M | ? | data.py | 938 |
| M | ? | data.py | 962 |
| M | ? | data.py | 963 |
| M | ? | data.py | 965 |
| M | ? | data.py | 985 |
| M | ? | data.py | 986 |
| M | ? | data.py | 1000 |
| M | ? | data.py | 1001 |
| M | ? | data.py | 1053 |
| M | ? | data.py | 1055 |
| M | ? | data.py | 1061 |
| M | ? | data.py | 1065 |
| M | ? | data.py | 1139 |
| M | ? | data.py | 1160 |
| M | ? | data.py | 1204 |
| M | ? | data.py | 1218 |
| M | ? | data.py | 1269 |
| M | ? | data.py | 1309 |
| M | ? | data.py | 1349 |
| M | ? | floats.py | 104 |
| M | ? | floats.py | 111 |
| M | ? | floats.py | 142 |
| M | ? | floats.py | 159 |
| M | ? | floats.py | 177 |
| M | ? | floats.py | 185 |
| M | ? | floats.py | 195 |
| M | ? | floats.py | 208 |
| M | ? | collection.py | 47 |
| M | ? | floats.py | 60 |
| M | ? | integer.py | 38 |
| M | ? | ordering.py | 37 |
| M | ? | ordering.py | 38 |
| M | ? | ordering.py | 82 |
| M | ? | choicetree.py | 72 |
| M | ? | choicetree.py | 78 |
| M | ? | choicetree.py | 92 |
| M | ? | choicetree.py | 99 |
| M | ? | choicetree.py | 106 |
| M | ? | choicetree.py | 110 |
| M | ? | choicetree.py | 135 |
| M | ? | junkdrawer.py | 57 |
| M | ? | junkdrawer.py | 158 |
| M | ? | junkdrawer.py | 166 |
| M | ? | junkdrawer.py | 269 |
| M | ? | junkdrawer.py | 273 |
| M | ? | junkdrawer.py | 340 |
| M | ? | junkdrawer.py | 348 |
| M | ? | junkdrawer.py | 355 |
| M | ? | junkdrawer.py | 388 |
| M | ? | choice.py | 81 |
| M | ? | choice.py | 101 |
| M | ? | choice.py | 185 |
| M | ? | choice.py | 298 |
| M | ? | choice.py | 374 |
| M | ? | choice.py | 375 |
| M | ? | choice.py | 376 |
| M | ? | choice.py | 428 |
| M | ? | choice.py | 455 |
| M | ? | choice.py | 456 |
| M | ? | choice.py | 457 |
| M | ? | choice.py | 481 |
| M | ? | choice.py | 484 |
| M | ? | choice.py | 580 |
| M | ? | optimiser.py | 67 |
| M | ? | optimiser.py | 75 |
| M | ? | optimiser.py | 105 |
| M | ? | optimiser.py | 127 |
| M | ? | optimiser.py | 133 |
| M | ? | optimiser.py | 136 |
| M | ? | optimiser.py | 146 |
| M | ? | optimiser.py | 147 |
| M | ? | optimiser.py | 178 |
| M | ? | providers.py | 161 |
| M | ? | providers.py | 187 |
| M | ? | providers.py | 648 |
| M | ? | providers.py | 776 |
| M | ? | providers.py | 777 |
| M | ? | providers.py | 784 |
| M | ? | providers.py | 822 |
| M | ? | providers.py | 839 |
| M | ? | providers.py | 851 |
| M | ? | providers.py | 855 |
| M | ? | providers.py | 856 |
| M | ? | providers.py | 883 |
| M | ? | providers.py | 901 |
| M | ? | providers.py | 958 |
| M | ? | providers.py | 969 |
| M | ? | providers.py | 1023 |
| M | ? | providers.py | 1024 |
| M | ? | providers.py | 1035 |
| M | ? | providers.py | 1069 |
| M | ? | providers.py | 1070 |
| M | ? | providers.py | 1077 |
| M | ? | providers.py | 1098 |
| M | ? | providers.py | 1164 |
| M | ? | providers.py | 1173 |
| M | ? | providers.py | 1176 |
| M | ? | providers.py | 1258 |
| M | ? | utils.py | 157 |
| M | ? | utils.py | 158 |
| M | ? | utils.py | 159 |
| M | ? | utils.py | 179 |
| M | ? | utils.py | 180 |
| M | ? | utils.py | 181 |
| M | ? | utils.py | 244 |
| M | ? | utils.py | 254 |
| M | ? | utils.py | 257 |
| M | ? | utils.py | 283 |
| M | ? | utils.py | 284 |
| M | ? | utils.py | 323 |
| M | ? | utils.py | 347 |
| M | ? | utils.py | 366 |
| M | ? | utils.py | 371 |
| M | ? | utils.py | 373 |
| M | ? | utils.py | 391 |
| M | ? | utils.py | 397 |
| M | ? | utils.py | 398 |
| M | ? | provider_conformance.py | 134 |
| M | ? | provider_conformance.py | 135 |
| M | ? | provider_conformance.py | 295 |
| M | ? | provider_conformance.py | 414 |
| M | ? | provider_conformance.py | 415 |
| M | ? | provider_conformance.py | 481 |
| M | ? | provider_conformance.py | 487 |
| M | ? | provider_conformance.py | 496 |
| M | ? | engine.py | 609 |
| M | ? | engine.py | 658 |
| M | ? | engine.py | 672 |
| M | ? | engine.py | 714 |
| M | ? | engine.py | 808 |
| M | ? | engine.py | 815 |
| M | ? | engine.py | 962 |
| M | ? | engine.py | 969 |
| M | ? | engine.py | 971 |
| M | ? | engine.py | 1073 |
| M | ? | engine.py | 1085 |
| M | ? | engine.py | 1146 |
| M | ? | engine.py | 1147 |
| M | ? | engine.py | 1148 |
| M | ? | engine.py | 1168 |
| M | ? | engine.py | 1172 |
| M | ? | engine.py | 1285 |
| M | ? | engine.py | 1307 |
| M | ? | engine.py | 1491 |
| M | ? | engine.py | 1614 |
| M | ? | shrinker.py | 319 |
| M | ? | shrinker.py | 596 |
| M | ? | shrinker.py | 597 |
| M | ? | shrinker.py | 649 |
| M | ? | shrinker.py | 657 |
| M | ? | shrinker.py | 757 |
| M | ? | shrinker.py | 841 |
| M | ? | shrinker.py | 1032 |
| M | ? | shrinker.py | 1033 |
| M | ? | shrinker.py | 1034 |
| M | ? | shrinker.py | 1092 |
| M | ? | shrinker.py | 1136 |
| M | ? | shrinker.py | 1139 |
| M | ? | shrinker.py | 1147 |
| M | ? | shrinker.py | 1149 |
| M | ? | shrinker.py | 1156 |
| M | ? | shrinker.py | 1648 |
| M | ? | shrinker.py | 1680 |
| M | ? | shrinker.py | 1798 |
| M | ? | observability.py | 139 |
| M | ? | observability.py | 224 |
| M | ? | observability.py | 420 |
| M | ? | reflection.py | 236 |
| M | ? | reflection.py | 357 |
| M | ? | validation.py | 23 |
| M | ? | validation.py | 33 |
| M | ? | filtering.py | 145 |
| M | ? | filtering.py | 163 |
| M | ? | filtering.py | 240 |
| M | ? | filtering.py | 248 |
| M | ? | filtering.py | 299 |
| M | ? | entropy.py | 51 |
| M | ? | entropy.py | 177 |
| M | ? | entropy.py | 178 |
| M | ? | entropy.py | 188 |
| M | ? | intervalsets.py | 52 |
| M | ? | intervalsets.py | 90 |
| M | ? | intervalsets.py | 96 |
| M | ? | intervalsets.py | 143 |
| M | ? | intervalsets.py | 180 |
| M | ? | intervalsets.py | 197 |
| M | ? | intervalsets.py | 199 |
| M | ? | intervalsets.py | 250 |
| M | ? | intervalsets.py | 287 |
| M | ? | intervalsets.py | 288 |
| M | ? | intervalsets.py | 296 |
| M | ? | intervalsets.py | 304 |
| M | ? | intervalsets.py | 308 |
| M | ? | intervalsets.py | 309 |
| M | ? | charmap.py | 136 |
| M | ? | charmap.py | 137 |
| M | ? | charmap.py | 138 |
| M | ? | charmap.py | 140 |
| M | ? | charmap.py | 147 |
| M | ? | charmap.py | 270 |
| M | ? | charmap.py | 277 |
| M | ? | escalation.py | 35 |
| M | ? | escalation.py | 72 |
| M | ? | lambda_sources.py | 318 |
| M | ? | reporting.py | 40 |
| M | ? | reporting.py | 60 |
| M | ? | impl.py | 228 |
| M | ? | impl.py | 673 |
| M | ? | dateutil.py | 36 |
| M | ? | dateutil.py | 63 |
| M | ? | _array_helpers.py | 328 |
| M | ? | _array_helpers.py | 406 |
| M | ? | _array_helpers.py | 576 |
| M | ? | _array_helpers.py | 577 |
| M | ? | _array_helpers.py | 629 |
| M | ? | _array_helpers.py | 630 |
| M | ? | _array_helpers.py | 631 |
| M | ? | ghostwriter.py | 547 |
| M | ? | ghostwriter.py | 584 |
| M | ? | ghostwriter.py | 586 |
| M | ? | ghostwriter.py | 587 |
| M | ? | ghostwriter.py | 939 |
| M | ? | lark.py | 72 |
| M | ? | lark.py | 101 |
| M | ? | lark.py | 196 |
| M | ? | redis.py | 88 |
| M | ? | redis.py | 89 |
| M | ? | redis.py | 135 |
| M | ? | numpy.py | 66 |
| M | ? | numpy.py | 170 |
| M | ? | numpy.py | 448 |
| M | ? | array_api.py | 63 |
| M | ? | array_api.py | 65 |
| M | ? | array_api.py | 232 |
| M | ? | array_api.py | 233 |
| M | ? | array_api.py | 250 |
| M | ? | array_api.py | 255 |
| M | ? | array_api.py | 325 |
| M | ? | array_api.py | 562 |
| M | ? | array_api.py | 583 |
| M | ? | _fields.py | 63 |
| M | ? | _fields.py | 411 |
| M | ? | _patching.py | 302 |
| M | ? | _patching.py | 336 |
| M | ? | deprecation.py | 22 |
| M | ? | core.py | 540 |
| M | ? | core.py | 548 |
| M | ? | core.py | 553 |
| M | ? | core.py | 583 |
| M | ? | core.py | 689 |
| M | ? | core.py | 915 |
| M | ? | core.py | 1196 |
| M | ? | core.py | 1310 |
| M | ? | core.py | 1525 |
| M | ? | core.py | 1526 |
| M | ? | core.py | 1666 |
| M | ? | core.py | 2001 |
| M | ? | core.py | 2194 |
| M | ? | core.py | 2243 |
| M | ? | core.py | 2315 |
| M | ? | core.py | 2316 |
| M | ? | core.py | 2339 |
| M | ? | core.py | 2387 |
| M | ? | errors.py | 93 |
| M | ? | _settings.py | 127 |
| M | ? | _settings.py | 546 |
| M | ? | _settings.py | 548 |
| M | ? | _settings.py | 841 |
| M | ? | _settings.py | 1198 |
| M | ? | _settings.py | 1224 |
| M | ? | _settings.py | 1240 |
| M | ? | _settings.py | 1246 |
| M | ? | strings.py | 84 |
| M | ? | strings.py | 99 |
| M | ? | collections.py | 170 |
| M | ? | collections.py | 208 |
| M | ? | collections.py | 238 |
| M | ? | collections.py | 288 |
| M | ? | collections.py | 321 |
| M | ? | collections.py | 327 |
| M | ? | collections.py | 333 |
| M | ? | collections.py | 362 |
| M | ? | numbers.py | 54 |
| M | ? | numbers.py | 55 |
| M | ? | numbers.py | 56 |
| M | ? | numbers.py | 162 |
| M | ? | numbers.py | 163 |
| M | ? | numbers.py | 361 |
| M | ? | numbers.py | 364 |
| M | ? | numbers.py | 390 |
| M | ? | numbers.py | 391 |
| M | ? | numbers.py | 392 |
| M | ? | numbers.py | 396 |
| M | ? | numbers.py | 404 |
| M | ? | numbers.py | 405 |
| M | ? | numbers.py | 406 |
| M | ? | numbers.py | 410 |
| M | ? | numbers.py | 495 |
| M | ? | numbers.py | 496 |
| M | ? | types.py | 290 |
| M | ? | types.py | 344 |
| M | ? | types.py | 382 |
| M | ? | types.py | 383 |
| M | ? | types.py | 580 |
| M | ? | types.py | 1280 |
| M | ? | types.py | 1281 |
| M | ? | lazy.py | 49 |
| M | ? | lazy.py | 63 |
| M | ? | lazy.py | 124 |
| M | ? | lazy.py | 147 |
| M | ? | regex.py | 282 |
| M | ? | regex.py | 288 |
| M | ? | regex.py | 473 |
| M | ? | regex.py | 523 |
| M | ? | datetime.py | 185 |
| M | ? | datetime.py | 204 |
| M | ? | datetime.py | 205 |
| M | ? | datetime.py | 206 |
| M | ? | datetime.py | 254 |
| M | ? | datetime.py | 255 |
| M | ? | datetime.py | 261 |
| M | ? | datetime.py | 275 |
| M | ? | datetime.py | 278 |
| M | ? | datetime.py | 279 |
| M | ? | datetime.py | 280 |
| M | ? | datetime.py | 649 |
| M | ? | datetime.py | 650 |
| M | ? | datetime.py | 651 |
| M | ? | datetime.py | 706 |
| M | ? | datetime.py | 707 |
| M | ? | datetime.py | 708 |
| M | ? | datetime.py | 747 |
| M | ? | core.py | 1726 |
| M | ? | core.py | 1727 |
| M | ? | core.py | 1791 |
| M | ? | core.py | 1804 |
| M | ? | core.py | 1822 |
| M | ? | core.py | 2101 |
| M | ? | utils.py | 150 |
| M | ? | recursive.py | 68 |
| M | ? | strategies.py | 109 |
| M | ? | strategies.py | 178 |
| M | ? | strategies.py | 198 |
| M | ? | strategies.py | 596 |
| M | ? | strategies.py | 723 |
| M | ? | strategies.py | 742 |
| M | ? | strategies.py | 788 |
| M | ? | strategies.py | 1146 |
| M | ? | strategies.py | 1147 |
| M | ? | strategies.py | 1261 |
| M | ? | attrs.py | 69 |
| M | ? | attrs.py | 104 |
| M | ? | attrs.py | 184 |
| M | ? | control.py | 267 |
| M | ? | control.py | 287 |
| M | ? | provisional.py | 43 |
| M | ? | stateful.py | 371 |
| M | ? | stateful.py | 1066 |
| M | ? | stateful.py | 1072 |
| M | ? | stateful.py | 1209 |
| M | ? | database.py | 528 |
| M | ? | database.py | 599 |
| M | ? | database.py | 602 |
| M | ? | database.py | 632 |
| M | ? | database.py | 633 |
| M | ? | database.py | 643 |
| M | ? | database.py | 644 |
| M | ? | database.py | 645 |
| M | ? | database.py | 681 |
| M | ? | database.py | 722 |
| M | ? | database.py | 776 |
| M | ? | database.py | 946 |
| M | ? | database.py | 1143 |
| M | ? | database.py | 1144 |
| M | ? | database.py | 1237 |
| M | ? | database.py | 1292 |
| M | ? | database.py | 1326 |
| M | ? | database.py | 1333 |
| M | ? | _hypothesis_pytestplugin.py | 58 |
| M | ? | pelicanconf.py | 86 |
| M | ? | release.py | 39 |
| M | ? | release.py | 169 |
| M | ? | release.py | 173 |
| M | ? | release.py | 174 |
| M | ? | release.py | 175 |
| M | ? | release.py | 176 |
| M | ? | release.py | 181 |
| M | ? | release.py | 275 |
| M | ? | release.py | 278 |
| M | ? | release.py | 279 |
| M | ? | release.py | 289 |
| M | ? | cargo.py | 26 |
| M | ? | installers.py | 58 |
| M | ? | git.py | 21 |
| M | ? | git.py | 41 |
| M | ? | git.py | 84 |
| M | ? | git.py | 95 |
| H | ? | engine.py | 924 |
| H | ? | redis.py | 117 |
| H | ? | core.py | 2363 |
| H | ? | database.py | 266 |
| H | ? | database.py | 269 |
| H | ? | database.py | 499 |
| H | ? | database.py | 534 |
| H | ? | database.py | 542 |
| H | ? | database.py | 548 |
| H | ? | database.py | 797 |
| M | ? | engine.py | 1346 |
| M | ? | engine.py | 1506 |
| M | ? | engine.py | 1569 |
| M | ? | statistics.py | 31 |
| M | ? | statistics.py | 127 |
| M | ? | core.py | 1511 |
| M | ? | stateful.py | 217 |
| M | ? | stateful.py | 219 |
| M | ? | stateful.py | 449 |
| M | ? | stateful.py | 761 |
| M | ? | stateful.py | 892 |
| M | ? | stateful.py | 973 |
| H | ? | ghostwriter.py | 718 |
| H | ? | pelicanconf.py | 42 |
| H | ? | pelicanconf.py | 43 |
| H | ? | pelicanconf.py | 44 |
| H | ? | pelicanconf.py | 47 |
| H | ? | pelicanconf.py | 48 |
| H | ? | pelicanconf.py | 49 |
| C | ? | installers.py | 94 |
| M | ? | regex.py | 67 |
| M | ? | core.py | 2277 |
| M | ? | core.py | 2278 |
| M | ? | strategies.py | 110 |
| M | ? | strategies.py | 112 |
| M | ? | _hypothesis_pytestplugin.py | 36 |
| L | GS003 | graph.py | 82 |
| L | GS003 | validate_branch_check.py | 27 |
| L | GS003 | validate_branch_check.py | 45 |
| L | GS003 | validate_branch_check.py | 48 |
| L | GS003 | validate_branch_check.py | 49 |
| L | GS003 | validate_branch_check.py | 51 |
| L | GS003 | validate_branch_check.py | 53 |
| L | GS003 | validate_branch_check.py | 54 |
| L | GS003 | validate_branch_check.py | 56 |
| L | GS003 | validate_branch_check.py | 59 |
| L | GS003 | _hypothesis_ftz_detector.py | 159 |
| L | GS003 | cli.py | 212 |
| L | GS003 | cli.py | 213 |
| L | GS003 | cli.py | 229 |
| L | GS003 | cli.py | 331 |
| L | GS003 | cli.py | 338 |
| L | GS003 | cli.py | 339 |
| L | GS003 | common.py | 80 |
| L | GS003 | reporting.py | 22 |
| L | GS003 | reporting.py | 24 |
| L | GS003 | tool-hash.py | 17 |
| L | GS003 | __main__.py | 82 |
| L | GS003 | __main__.py | 132 |
| L | GS003 | __main__.py | 133 |
| L | GS003 | __main__.py | 143 |
| L | GS003 | __main__.py | 144 |
| L | GS003 | __main__.py | 159 |
| L | GS003 | __main__.py | 165 |
| L | GS003 | __main__.py | 168 |
| L | GS003 | __main__.py | 173 |
| L | GS003 | __main__.py | 176 |
| L | GS003 | __main__.py | 179 |
| L | GS003 | __main__.py | 186 |
| L | GS003 | __main__.py | 1135 |
| L | GS003 | __main__.py | 1140 |
| L | GS003 | __main__.py | 1154 |
| L | GS003 | __main__.py | 1162 |
| L | GS003 | scripts.py | 35 |
| L | GS003 | prism.js | 7 |
| L | GS003 | prism.js | 7 |
| L | GS008 | compat.py | 76 |
| L | GS008 | compat.py | 77 |
| L | GS008 | compat.py | 78 |
| L | GS008 | compat.py | 80 |
| L | GS008 | floats.py | 79 |
| L | GS008 | floats.py | 105 |
| L | GS008 | floats.py | 107 |
| L | GS008 | regex.py | 48 |
| L | GS008 | git.py | 32 |
| L | GS008 | release.py | 31 |
| L | GS008 | release.py | 32 |
| L | GS008 | pelicanconf.py | 11 |
| L | GS008 | pelicanconf.py | 11 |
| L | GS008 | pelicanconf.py | 12 |
| L | GS008 | pelicanconf.py | 16 |
| L | GS008 | pelicanconf.py | 20 |
| L | GS008 | pelicanconf.py | 21 |
| L | GS008 | pelicanconf.py | 22 |
| L | GS008 | pelicanconf.py | 23 |
| L | GS008 | pelicanconf.py | 24 |
| L | GS008 | pelicanconf.py | 27 |
| L | GS008 | pelicanconf.py | 28 |
| L | GS008 | pelicanconf.py | 29 |
| L | GS008 | pelicanconf.py | 32 |
| L | GS008 | pelicanconf.py | 35 |
| L | GS008 | pelicanconf.py | 39 |
| L | GS008 | pelicanconf.py | 53 |
| L | GS008 | pelicanconf.py | 88 |
| H | ? | ipaddress.py | 23 |
| H | ? | ipaddress.py | 24 |
| H | ? | ipaddress.py | 25 |
| H | ? | ipaddress.py | 26 |
| H | ? | ipaddress.py | 27 |
| H | ? | ipaddress.py | 28 |
| H | ? | ipaddress.py | 29 |
| H | ? | ipaddress.py | 30 |
| H | ? | ipaddress.py | 31 |
| H | ? | ipaddress.py | 32 |
| H | ? | ipaddress.py | 33 |
| H | ? | ipaddress.py | 34 |
| H | ? | ipaddress.py | 35 |
| H | ? | ipaddress.py | 36 |
| H | ? | ipaddress.py | 37 |
| H | ? | ipaddress.py | 38 |
| H | ? | ipaddress.py | 39 |
| H | ? | ipaddress.py | 40 |
| H | ? | ipaddress.py | 41 |
| H | ? | ipaddress.py | 42 |
| H | ? | ipaddress.py | 43 |
| H | ? | ipaddress.py | 44 |
| H | ? | ipaddress.py | 45 |
| H | ? | ipaddress.py | 46 |
| H | ? | ipaddress.py | 85 |
| C | ? | regex.py | 67 |
| M | ? | release.py | 240 |
| H | ? | reflection.py | 358 |
| H | ? | lambda_sources.py | 253 |
| H | ? | lambda_sources.py | 286 |
| H | ? | .readthedocs.yml | 0 |
| H | GS004 | lambda_sources.py | 286 |
| H | GS004 | reflection.py | 358 |
| H | GS004 | installers.py | 66 |
| H | GS004 | installers.py | 94 |
| H | GS004 | installers.py | 98 |
| I | GS007 | _hypothesis_ftz_detector.py | 37 |
| I | GS007 | shrinker.py | 561 |
| s | GS009 |  | 0 |
| M | ? | scrutineer.py | 312 |
| M | ? | __main__.py | 124 |
| M | ? | __main__.py | 136 |

---
*Сгенерировано GSC v0.6 · 2026-07-31T04:01:25.355525*