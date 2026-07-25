---
title: "GSC Audit: /tmp/gsc-learn/ruff"
date: 2026-07-23
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/ruff

**Дата:** 23.07.2026 04:05  
**Путь:** `/tmp/gsc-learn/ruff`  
**Всего находок:** 4567  
**CRITICAL:** 253 | **HIGH:** 1544 | **MEDIUM:** 1145 | **LOW:** 1596

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 1438 |
| Python: assert in production | 736 |
| GS003 | 292 |
| Bare except: | 176 |
| Синхронный код в async | 134 |
| chmod: World-readable configs | 114 |
| GS001 | 48 |
| CVE-2026-37270: Hardcoded credential | 44 |
| Хардкод IP адреса | 37 |
| SQL injection risk: f-string in query | 30 |
| Hardcoded encryption key | 29 |
| CVE-2026-55223: Insecure deserialization | 28 |
| GS015 | 28 |
| Generic code smell #24 | 22 |
| Generic code smell #27 | 22 |
| Generic code smell #30 | 22 |
| Generic code smell #33 | 22 |
| Generic code smell #36 | 22 |
| Generic code smell #39 | 22 |
| Generic code smell #42 | 22 |
| Generic code smell #45 | 22 |
| Generic code smell #48 | 22 |
| Generic code smell #51 | 22 |
| Generic code smell #54 | 22 |
| Generic code smell #57 | 22 |
| Generic code smell #60 | 22 |
| Generic code smell #63 | 22 |
| Generic code smell #66 | 22 |
| Generic code smell #69 | 22 |
| Generic code smell #72 | 22 |
| Generic code smell #75 | 22 |
| Generic code smell #78 | 22 |
| Generic code smell #81 | 22 |
| Generic code smell #84 | 22 |
| Generic code smell #87 | 22 |
| Generic code smell #90 | 22 |
| Generic code smell #93 | 22 |
| Generic code smell #96 | 22 |
| Generic code smell #99 | 22 |
| Generic code smell #102 | 22 |
| Generic code smell #105 | 22 |
| Generic code smell #108 | 22 |
| Generic code smell #111 | 22 |
| Generic code smell #114 | 22 |
| Generic code smell #117 | 22 |
| Generic code smell #120 | 22 |
| Generic code smell #123 | 22 |
| Generic code smell #126 | 22 |
| Generic code smell #129 | 22 |
| Generic code smell #132 | 22 |
| Generic code smell #135 | 22 |
| Generic code smell #138 | 22 |
| Generic code smell #141 | 22 |
| Generic code smell #144 | 22 |
| Generic code smell #147 | 22 |
| Generic code smell #150 | 22 |
| Generic code smell #153 | 22 |
| Generic code smell #156 | 22 |
| Generic code smell #159 | 22 |
| Generic code smell #162 | 22 |
| Generic code smell #165 | 22 |
| Generic code smell #168 | 22 |
| Generic code smell #171 | 22 |
| Generic code smell #174 | 22 |
| Generic code smell #177 | 22 |
| Generic code smell #180 | 22 |
| Generic code smell #183 | 22 |
| Generic code smell #186 | 22 |
| Generic code smell #189 | 22 |
| Generic code smell #192 | 22 |
| Generic code smell #195 | 22 |
| Generic code smell #198 | 22 |
| CVE-2026-56219: Authentication bypass | 19 |
| CVE-2026-56413: Command injection | 19 |
| CVE-2026-56318: Information disclosure | 15 |
| eval() or exec() usage | 14 |
| Outdated dependency pattern | 11 |
| TS: Hardcoded API key | 10 |
| CVE-2026-56233: Path traversal | 8 |
| TS: any type escape hatch | 7 |
| Python: raw string concatenation in SQL | 6 |
| GS008 | 6 |
| CVE-2026-55721: SQL injection | 4 |
| GS004 | 4 |
| Weak password validation | 2 |
| TS: console.log in production | 1 |
| Python: File upload without content-type validation | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: ty.schema.json (664) | 1 |
| World-readable file: ruff.schema.json (664) | 1 |
| World-readable file: .markdownlint.yaml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: mkdocs.template.yml (664) | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 33 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 43 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 51 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 60 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 86 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 96 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 104 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 113 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 128 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 138 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 146 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 155 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 170 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 180 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 188 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 197 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 463 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 472 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 482 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 491 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 590 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 598 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 604 | OWASP A03: Injection |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 612 | OWASP A03: Injection |
| CRITICAL | ? | S608.py | 6 | OWASP A03: Injection |
| CRITICAL | ? | S608.py | 12 | OWASP A03: Injection |
| CRITICAL | ? | S608.py | 17 | OWASP A03: Injection |
| CRITICAL | ? | S608.py | 22 | OWASP A03: Injection |
| CRITICAL | ? | S608.py | 136 | OWASP A03: Injection |
| CRITICAL | ? | S608.py | 140 | OWASP A03: Injection |
| CRITICAL | ? | S608.py | 3 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | S608.py | 4 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | S608.py | 9 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | S608.py | 10 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | S608.py | 15 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | S608.py | 20 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | S608.py | 6 |  |
| CRITICAL | ? | S608.py | 12 |  |
| CRITICAL | ? | S608.py | 17 |  |
| CRITICAL | ? | S608.py | 22 |  |
| CRITICAL | ? | S605.py | 8 |  |
| CRITICAL | ? | S605.py | 26 |  |
| CRITICAL | ? | S605.py | 27 |  |
| CRITICAL | ? | S605.py | 28 |  |
| CRITICAL | ? | S609.py | 5 |  |
| CRITICAL | ? | S609.py | 6 |  |
| CRITICAL | ? | S609.py | 8 |  |
| CRITICAL | ? | S607.py | 9 |  |
| CRITICAL | ? | S607.py | 40 |  |
| CRITICAL | ? | S607.py | 41 |  |
| CRITICAL | ? | S607.py | 42 |  |
| CRITICAL | ? | S607.py | 43 |  |
| CRITICAL | ? | S607.py | 44 |  |
| CRITICAL | ? | subprocess_run_without_check.py | 5 |  |
| CRITICAL | ? | subprocess_run_without_check.py | 15 |  |
| CRITICAL | ? | subprocess_run_without_check.py | 16 |  |
| CRITICAL | ? | ASYNC22x.py | 32 |  |
| CRITICAL | ? | ASYNC22x.py | 35 |  |
| CRITICAL | ? | setup_primer_project.py | 142 |  |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 8 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 11 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 18 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 21 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 22 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 28 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 30 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 32 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 40 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 41 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 50 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 51 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 61 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 66 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 76 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 85 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 88 | Found: PASSWORD = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 95 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 98 | Found: PASSWORD = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 99 | Found: PassWord = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 105 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 107 | Found: PASSWORD = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 109 | Found: PassWord = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 117 | Found: PASSWORD = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 118 | Found: PassWord = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 127 | Found: PASSWORD = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 128 | Found: PassWord = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 137 | Found: PassWord = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 244 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 252 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 255 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 261 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 264 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 265 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 271 | Found: password = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 273 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 275 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 283 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 284 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 293 | Found: passwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 294 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 304 | Found: pwd = "s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S106_S106.py.snap | 8 | Found: password="s3cr3t" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 7 | Found: password="default" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 15 | Found: password="posonly" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 23 | Found: password="kwonly" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 31 | Found: password="kwonly" |
| CRITICAL | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 39 | Found: password="kwonly" |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 12 | Match: 8 | os.chmod("/etc/passwd", 0o664)  # OK (stable); Er |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 21 | Match: 8 | os.chmod("/etc/passwd", 0o664)  # OK (stable); Er |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 22 | Match: 9 | os.chmod("/etc/passwd", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 25 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 29 | Match:  8 | os.chmod("/etc/passwd", 0o664)  # OK (stable); E |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 30 | Match:  9 | os.chmod("/etc/passwd", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 33 | Match: 11 | os.chmod("/etc/passwd", 0o776)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 39 | Match:  8 | os.chmod("/etc/passwd", 0o664)  # OK (stable); E |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 40 | Match:  9 | os.chmod("/etc/passwd", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 43 | Match: 11 | os.chmod("/etc/passwd", 0o776)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 47 | Match: S103 `os.chmod` setting a permissive mask `0o776` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 50 | Match:  9 | os.chmod("/etc/passwd", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 52 | Match: 11 | os.chmod("/etc/passwd", 0o776)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 58 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 61 | Match: 11 | os.chmod("/etc/passwd", 0o776)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 65 | Match: 14 | os.chmod("/etc/hosts", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 69 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 74 | Match: 14 | os.chmod("/etc/hosts", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 80 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 84 | Match: 14 | os.chmod("/etc/hosts", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 88 | Match: 17 | os.chmod(keyfile, 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 91 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 96 | Match: 17 | os.chmod(keyfile, 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 102 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 106 | Match: 17 | os.chmod(keyfile, 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 113 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 116 | Match: 17 | os.chmod(keyfile, 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 165 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 169 | Match: 31 |     os.chmod(path, mode | 0o777)  # Error (stati |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 175 | Match: S103 `os.chmod` setting a permissive mask `0o777` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 178 | Match: 36 | os.chmod("/etc/secrets.txt", 0o777777 & 0o700)   |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 179 | Match: 37 | os.chmod("/etc/secrets.txt", 0o777777 & 0o777)   |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 181 | Match: 38 | os.chmod("/etc/passwd", 0o200000)  # Error (bit  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 187 | Match: 36 | os.chmod("/etc/secrets.txt", 0o777777 & 0o700)   |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 188 | Match: 37 | os.chmod("/etc/secrets.txt", 0o777777 & 0o777)   |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 189 | Match: 38 | os.chmod("/etc/passwd", 0o200000)  # Error (bit  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 198 | Match: 38 | os.chmod("/etc/passwd", 0o200000)  # Error (bit  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 203 | Match: 42 | os.chmod("/etc/passwd", 99999999999999999999999  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 211 | Match: 42 | os.chmod("/etc/passwd", 99999999999999999999999  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 214 | Match: 44 | os.chmod("/tmp/x", 18446744073709551616 ^ 184467 |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 13 | Match: S103 `os.chmod` setting a permissive mask `0o664` on  |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 18 | Match:  8 | os.chmod("/etc/passwd", 0o664)  # OK (stable); E |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 20 | Match:  9 | os.chmod("/etc/passwd", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 29 | Match: 11 | os.chmod("/etc/passwd", 0o776)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 33 | Match: 14 | os.chmod("/etc/hosts", 0o777)  # Error |
| CRITICAL | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1008 | Match: 186 | os.chmod(_AttrHolder.fd, 0o644)    # Suppressed |
| CRITICAL | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1009 | Match: 187 | os.chmod(_AttrHolder.name, 0o644)  # Diagnostic |
| CRITICAL | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1018 | Match: 187 | os.chmod(_AttrHolder.fd, 0o644)    # Suppressed |
| CRITICAL | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1019 | Match:     - os.chmod(_AttrHolder.name, 0o644)  # Diagnostic |
| CRITICAL | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1020 | Match: 188 + pathlib.Path(_AttrHolder.name).chmod(0o644)  #  |
| CRITICAL | ? | ruff_linter__rules__flake8_use_pathlib__tests__full_name.py.snap | 635 | Match: 186 | os.chmod(_AttrHolder.fd, 0o644)    # Suppressed |
| CRITICAL | ? | ruff_linter__rules__flake8_use_pathlib__tests__full_name.py.snap | 636 | Match: 187 | os.chmod(_AttrHolder.name, 0o644)  # Diagnostic |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 9 | Match: 6 | os.chmod("foo", 444)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 11 | Match: 7 | os.chmod("foo", 0o444)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 12 | Match: 8 | os.chmod("foo", 7777)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 19 | Match:   - os.chmod("foo", 444)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 20 | Match: 6 + os.chmod("foo", 0o444)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 21 | Match: 7 | os.chmod("foo", 0o444)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 28 | Match:  6 | os.chmod("foo", 444)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 29 | Match:  7 | os.chmod("foo", 0o444)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 30 | Match:  8 | os.chmod("foo", 7777)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 41 | Match:  7 | os.chmod("foo", 0o444)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 42 | Match:  8 | os.chmod("foo", 7777)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 53 | Match:  8 | os.chmod("foo", 7777)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 107 | Match: 18 | os.lchmod("foo", 755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 109 | Match: 19 | os.lchmod("foo", 0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 116 | Match:    - os.lchmod("foo", 755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 117 | Match: 18 + os.lchmod("foo", 0o755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 118 | Match: 19 | os.lchmod("foo", 0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 125 | Match: 19 | os.lchmod("foo", 0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 227 | Match: 36 | Path("bar").chmod(755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 229 | Match: 37 | Path("bar").chmod(0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 236 | Match:    - Path("bar").chmod(755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 237 | Match: 36 + Path("bar").chmod(0o755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 238 | Match: 37 | Path("bar").chmod(0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 246 | Match: 40 | path.chmod(755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 248 | Match: 41 | path.chmod(0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 255 | Match:    - path.chmod(755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 256 | Match: 40 + path.chmod(0o755)  # Error |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 257 | Match: 41 | path.chmod(0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 264 | Match: 41 | path.chmod(0o755)  # OK |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 326 | Match: 52 | os.fchmod(0, 256)  # 0o400 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 328 | Match: 53 | os.fchmod(0, 493)  # 0o755 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 335 | Match:    - os.fchmod(0, 256)  # 0o400 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 337 | Match: 53 | os.fchmod(0, 493)  # 0o755 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 344 | Match: 52 | os.fchmod(0, 256)  # 0o400 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 345 | Match: 53 | os.fchmod(0, 493)  # 0o755 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 354 | Match: 52 | os.fchmod(0, 256)  # 0o400 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 355 | Match:    - os.fchmod(0, 493)  # 0o755 |
| CRITICAL | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 356 | Match: 53 + os.fchmod(0, 0o755)  # 0o755 |
| CRITICAL | ? | S103.py | 8 | Match: os.chmod("/etc/passwd", 0o664)  # OK (stable); Error  |
| CRITICAL | ? | S103.py | 9 | Match: os.chmod("/etc/passwd", 0o777)  # Error |
| CRITICAL | ? | S103.py | 11 | Match: os.chmod("/etc/passwd", 0o776)  # Error |
| CRITICAL | ? | S103.py | 14 | Match: os.chmod("/etc/hosts", 0o777)  # Error |
| CRITICAL | ? | S103.py | 17 | Match: os.chmod(keyfile, 0o777)  # Error |
| CRITICAL | ? | S103.py | 31 | Match:     os.chmod(path, mode | 0o777)  # Error (statically |
| CRITICAL | ? | S103.py | 36 | Match: os.chmod("/etc/secrets.txt", 0o777777 & 0o700)  # OK  |
| CRITICAL | ? | S103.py | 37 | Match: os.chmod("/etc/secrets.txt", 0o777777 & 0o777)  # Err |
| CRITICAL | ? | S103.py | 38 | Match: os.chmod("/etc/passwd", 0o200000)  # Error (bit outsi |
| CRITICAL | ? | S103.py | 42 | Match: os.chmod("/etc/passwd", 99999999999999999999999 | 0o7 |
| CRITICAL | ? | S103.py | 44 | Match: os.chmod("/tmp/x", 18446744073709551616 ^ 18446744073 |
| CRITICAL | ? | full_name.py | 186 | Match: os.chmod(_AttrHolder.fd, 0o644)    # Suppressed: reso |
| CRITICAL | ? | full_name.py | 187 | Match: os.chmod(_AttrHolder.name, 0o644)  # Diagnostic + fix |
| CRITICAL | ? | RUF064.py | 6 | Match: os.chmod("foo", 444)  # Error |
| CRITICAL | ? | RUF064.py | 7 | Match: os.chmod("foo", 0o444)  # OK |
| CRITICAL | ? | RUF064.py | 8 | Match: os.chmod("foo", 7777)  # Error |
| CRITICAL | ? | RUF064.py | 18 | Match: os.lchmod("foo", 755)  # Error |
| CRITICAL | ? | RUF064.py | 19 | Match: os.lchmod("foo", 0o755)  # OK |
| CRITICAL | ? | RUF064.py | 36 | Match: Path("bar").chmod(755)  # Error |
| CRITICAL | ? | RUF064.py | 37 | Match: Path("bar").chmod(0o755)  # OK |
| CRITICAL | ? | RUF064.py | 40 | Match: path.chmod(755)  # Error |
| CRITICAL | ? | RUF064.py | 41 | Match: path.chmod(0o755)  # OK |
| CRITICAL | ? | RUF064.py | 52 | Match: os.fchmod(0, 256)  # 0o400 |
| CRITICAL | ? | RUF064.py | 53 | Match: os.fchmod(0, 493)  # 0o755 |
| CRITICAL | ? | ruff_linter__rules__pylint__tests__PLE1507_invalid_envvar_value.py.snap | 19 | Match: 6 | os.getenv(key="testingAgain") |
| CRITICAL | ? | ruff_linter__rules__pylint__tests__PLE1507_invalid_envvar_value.py.snap | 29 | Match:  6 | os.getenv(key="testingAgain") |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 189 | Match: 79 |     bash_command="{{ ti.xcom_pull(task_ids='task |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 196 | Match:    -     bash_command="{{ ti.xcom_pull(task_ids='task |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 207 | Match: 85 |     bash_command="{{ ti.xcom_pull(task_ids=['tas |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 214 | Match:    -     bash_command="{{ ti.xcom_pull(task_ids=['tas |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 225 | Match: 91 |     bash_command='{{ task_instance.xcom_pull(tas |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 232 | Match:    -     bash_command='{{ task_instance.xcom_pull(tas |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 243 | Match: 97 |     bash_command="{{ ti.xcom_pull(key='return_va |
| CRITICAL | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 250 | Match:    -     bash_command="{{ ti.xcom_pull(key='return_va |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 451 | Match:             parse_xcom_pull_template("{{ ti.xcom_pull |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 460 | Match:                 r#"{{ ti.xcom_pull(task_ids='my_task' |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 470 | Match:                 "{{ ti.xcom_pull(task_ids=['my_task'] |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 479 | Match:             parse_xcom_pull_template("{{ ti.xcom_pull |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 487 | Match:             parse_xcom_pull_template("{{ ti.xcom_pull |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 511 | Match:             parse_xcom_pull_template("{{ ti.xcom_pull |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 520 | Match:                 "{{ ti.xcom_pull(key='return_value',  |
| CRITICAL | ? | xcom_pull_in_template_string.rs | 529 | Match:             parse_xcom_pull_template("{{ ti.xcom_pull |
| CRITICAL | ? | magic_value_comparison.py | 66 | Match: input_password = "password" |
| CRITICAL | ? | AIR201.py | 79 | Match:     bash_command="{{ ti.xcom_pull(task_ids='task_1',  |
| CRITICAL | ? | AIR201.py | 85 | Match:     bash_command="{{ ti.xcom_pull(task_ids=['task_1'] |
| CRITICAL | ? | AIR201.py | 91 | Match:     bash_command='{{ task_instance.xcom_pull(task_ids |
| CRITICAL | ? | AIR201.py | 97 | Match:     bash_command="{{ ti.xcom_pull(key='return_value', |
| CRITICAL | ? | AIR201.py | 180 | Match:     bash_command="{{ ti.xcom_pull(task_ids=['task_1'] |
| CRITICAL | ? | AIR201.py | 186 | Match:     bash_command="{{ ti.xcom_pull(task_ids='task_1',  |
| CRITICAL | ? | AIR301_args.py | 335 | Match:     source_s3_key="s3://bucket/key", |
| CRITICAL | ? | AIR301_args.py | 336 | Match:     dest_s3_key="s3://bucket_2/key_2", |
| CRITICAL | ? | AIR301_args.py | 344 | Match:     source_s3_key="s3://bucket/key", |
| CRITICAL | ? | AIR301_args.py | 345 | Match:     dest_s3_key="s3://bucket_2/key_2", |
| CRITICAL | ? | FAST002_1.py | 20 | Match: def handler3(echo: str = Query("123", min_length=3, m |
| CRITICAL | ? | FAST002_2.py | 54 | Match:     param: str = Query(..., description="Test", min_l |
| CRITICAL | ? | S301.py | 3 | Match: pickle.loads() |
| HIGH | ? | Editor.tsx | 360 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | Editor.tsx | 539 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | Editor.tsx | 544 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | Editor.tsx | 549 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | Editor.tsx | 329 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | settings.ts | 4 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | SettingsEditor.tsx | 127 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | DJ012.py | 103 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | S501.py | 5 |  |
| HIGH | ? | S501.py | 7 |  |
| HIGH | ? | S501.py | 9 |  |
| HIGH | ? | S501.py | 11 |  |
| HIGH | ? | S501.py | 13 |  |
| HIGH | ? | S501.py | 15 |  |
| HIGH | ? | S501.py | 17 |  |
| HIGH | ? | S501.py | 19 |  |
| HIGH | ? | S501.py | 22 |  |
| HIGH | ? | S501.py | 24 |  |
| HIGH | ? | S501.py | 26 |  |
| HIGH | ? | S501.py | 28 |  |
| HIGH | ? | S501.py | 30 |  |
| HIGH | ? | S501.py | 32 |  |
| HIGH | ? | S501.py | 34 |  |
| HIGH | ? | S501.py | 36 |  |
| HIGH | ? | S501.py | 38 |  |
| HIGH | ? | S501.py | 40 |  |
| HIGH | ? | S501.py | 42 |  |
| HIGH | ? | preview_long_strings.py | 213 |  |
| HIGH | ? | long_strings_flag_disabled.py | 268 |  |
| HIGH | ? | E402_4.py | 5 |  |
| HIGH | ? | S202.py | 51 |  |
| HIGH | ? | S202.py | 54 |  |
| HIGH | ? | py_path_1.py | 3 |  |
| HIGH | ? | tool.py | 66 |  |
| HIGH | ? | update_schemastore.py | 102 |  |
| HIGH | ? | split_empty_brackets.py | 77 | Match:     f"http://127.0.0.1:{self.port}{path}", method=met |
| HIGH | ? | split_empty_brackets.py | 81 | Match:     f"http://127.0.0.1:{self.port}{path}", method=met |
| HIGH | ? | split_empty_brackets.py | 85 | Match:     f"http://127.0.0.1:{self.port}{path}", method=met |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 8 | Match:  9 | "0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 10 | Match: 10 | '0.0.0.0' |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 11 | Match: 11 | f"0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 18 | Match:  9 | "0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 19 | Match: 10 | '0.0.0.0' |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 21 | Match: 11 | f"0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 27 | Match:  9 | "0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 28 | Match: 10 | '0.0.0.0' |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 29 | Match: 11 | f"0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 37 | Match: 15 | func("0.0.0.0") |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 45 | Match: 19 |     x = "0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 54 | Match: 24 | "0.0.0.0" f"0.0.0.0{expr}0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 64 | Match: 24 | "0.0.0.0" f"0.0.0.0{expr}0.0.0.0" |
| HIGH | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 74 | Match: 24 | "0.0.0.0" f"0.0.0.0{expr}0.0.0.0" |
| HIGH | ? | hardcoded_bind_all_interfaces.rs | 44 | Match:             if value == "0.0.0.0" { |
| HIGH | ? | hardcoded_bind_all_interfaces.rs | 52 | Match:                         if &**literal == "0.0.0.0" { |
| HIGH | ? | hardcoded_bind_all_interfaces.rs | 58 | Match:                             if &**literal == "0.0.0.0 |
| HIGH | ? | S104.py | 9 | Match: "0.0.0.0" |
| HIGH | ? | S104.py | 10 | Match: '0.0.0.0' |
| HIGH | ? | S104.py | 11 | Match: f"0.0.0.0" |
| HIGH | ? | S104.py | 15 | Match: func("0.0.0.0") |
| HIGH | ? | S104.py | 19 | Match:     x = "0.0.0.0" |
| HIGH | ? | S104.py | 24 | Match: "0.0.0.0" f"0.0.0.0{expr}0.0.0.0" |
| HIGH | ? | S104.py | 27 | Match: t"0.0.0.0" |
| HIGH | ? | S104.py | 28 | Match: t"0.0.0.0" t"0.0.0.0{expr}0.0.0.0" |
| HIGH | ? | S104.py | 29 | Match: t"0.0.0.0" t"0.0.0.0{expr}0.0.0.0" t"0.0.0.0{expr}0.0 |
| HIGH | ? | v1.json | 4 | Match:   "logoSvg": "<svg xmlns=\"http://www.w3.org/2000/svg |
| HIGH | ? | v0.json | 4 | Match:   "logoSvg": "<svg xmlns=\"http://www.w3.org/2000/svg |
| HIGH | ? | projects.py | 363 | Match:             "types-protobuf==5.29.1.20250403", |
| HIGH | ? | projects.py | 364 | Match:             "types-setuptools==79.0.0.20250422", |
| HIGH | ? | projects.py | 371 | Match:             "types-openpyxl==3.1.5.20250919", |
| HIGH | ? | projects.py | 372 | Match:             "types-python-dateutil==2.9.0.20251008", |
| HIGH | ? | Icons.tsx | 225 | Match:         d="M9.86 2A2.86 2.86 0 0 0 7 4.86v1.68h4.29c. |
| HIGH | ? | Icons.tsx | 229 | Match:         d="M17.959 7v2.68a2.85 2.85 0 0 1-2.85 2.859H |
| HIGH | ? | function.py | 17 | Match:   exec("new-style exec", {}, {}) |
| HIGH | ? | fmtonoff.py | 26 | Match:   exec('new-style exec', {}, {}) |
| HIGH | ? | S102.py | 3 | Match:     exec('x = 2') |
| HIGH | ? | S102.py | 5 | Match: exec('y = 3') |
| HIGH | ? | S102.py | 11 | Match:     exec('')  # Error |
| HIGH | ? | S102.py | 15 | Match:     exec('')  # No error |
| HIGH | ? | S307.py | 3 | Match: print(eval("1+1"))  # S307 |
| HIGH | ? | S307.py | 4 | Match: print(eval("os.getcwd()"))  # S307 |
| HIGH | ? | S307.py | 8 | Match:     def eval(self): |
| HIGH | ? | S307.py | 12 | Match:         self.eval()  # OK |
| HIGH | ? | RUF028.py | 103 | Match:     assert eval(test_input) == expected |
| HIGH | ? | B007.py | 47 | Match:     print(FMT.format(foo=foo, bar=eval("bar"))) |
| HIGH | ? | decorator_expression_eval_hack_py38.py | 2 | Match: @eval("buttons[0].clicked.connect") |
| HIGH | ? | generate_builtin_modules.py | 52 | Match:     return set(eval(run(command_2))) |
| HIGH | ? | setupMonaco.tsx | 296 | Match:         token: "builtinConstant", |
| HIGH | ? | setupMonaco.tsx | 315 | Match:         token: "function", |
| HIGH | ? | setupMonaco.tsx | 319 | Match:         token: "decorator", |
| HIGH | ? | setupMonaco.tsx | 577 | Match:         token: "identifier", |
| HIGH | ? | setupMonaco.tsx | 585 | Match:         token: "builtinConstant", |
| HIGH | ? | setupMonaco.tsx | 593 | Match:         token: "delimiter", |
| HIGH | ? | setupMonaco.tsx | 601 | Match:         token: "variable", |
| HIGH | ? | setupMonaco.tsx | 605 | Match:         token: "parameter", |
| HIGH | ? | setupMonaco.tsx | 612 | Match:         token: "function", |
| HIGH | ? | setupMonaco.tsx | 616 | Match:         token: "decorator", |
| HIGH | ? | ty.schema.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | ruff.schema.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .markdownlint.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | mkdocs.template.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | check.py | 552 | Line 552: proc = await create_subprocess_exec( |
| HIGH | GS004 | format.py | 256 | Line 256: proc = await create_subprocess_exec( |
| HIGH | GS004 | check_ecosystem.py | 197 | Line 197: proc = await create_subprocess_exec( |
| HIGH | GS004 | setup_primer_project.py | 142 | Line 142: subprocess.run(install_cmd, cwd=target_dir, shell= |
| HIGH | ? | version.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 521 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 735 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 806 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1579 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2023 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2331 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2408 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2445 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2529 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 3059 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_ty_cli_reference.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_rules_table.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_ty_options.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | main.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_options.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | format_dev.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | format_dev.rs | 821 | Clone in performance-critical code — consider references |
| HIGH | ? | panic.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | vendored.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | source.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | source.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | source.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1811 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2599 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2608 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2614 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2624 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2630 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2636 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2642 | Clone in performance-critical code — consider references |
| HIGH | ? | render.rs | 2648 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | cancellation.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | files.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | files.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | files.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | file_root.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | ignore.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | ignore.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 596 | Clone in performance-critical code — consider references |
| HIGH | ? | memory_fs.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | os.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | os.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | os.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | os.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | parallel.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 427 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2020 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2029 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2037 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2038 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2145 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2167 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2287 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 2292 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration_file.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration_file.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration_file.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | watcher.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | changes.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | changes.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | changes.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | changes.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | files.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | walk.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | walk.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 618 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 682 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 810 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 821 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 943 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 947 | Clone in performance-critical code — consider references |
| HIGH | ? | symbols.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | symbols.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | symbols.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | symbols.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | symbols.rs | 777 | Clone in performance-critical code — consider references |
| HIGH | ? | symbols.rs | 1060 | Clone in performance-critical code — consider references |
| HIGH | ? | hints.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | rst.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | rst.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | google.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | google.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | google.rs | 850 | Clone in performance-critical code — consider references |
| HIGH | ? | completion.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | completion.rs | 2077 | Clone in performance-critical code — consider references |
| HIGH | ? | completion.rs | 11046 | Clone in performance-critical code — consider references |
| HIGH | ? | docstring.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | references.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | references.rs | 561 | Clone in performance-critical code — consider references |
| HIGH | ? | outgoing_calls.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | incoming_calls.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | incoming_calls.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | incoming_calls.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | inlay_hints.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | inlay_hints.rs | 739 | Clone in performance-critical code — consider references |
| HIGH | ? | inlay_hints.rs | 881 | Clone in performance-critical code — consider references |
| HIGH | ? | inlay_hints.rs | 8517 | Clone in performance-critical code — consider references |
| HIGH | ? | inlay_hints.rs | 8519 | Clone in performance-critical code — consider references |
| HIGH | ? | goto.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 646 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 668 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | tokenizer.rs | 925 | Clone in performance-critical code — consider references |
| HIGH | ? | tokenizer.rs | 975 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | fix.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | fix.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | text_document.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | traits.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | did_close.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | did_change_watched_files.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | did_change_watched_files.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | did_open_notebook.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | did_open.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | did_open.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | execute_command.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | execute_command.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | execute_command.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action_resolve.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action_resolve.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action_resolve.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action_resolve.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | api.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | api.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | pool.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 755 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 757 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 792 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 795 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | client.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | client.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 288 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_settings.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_settings.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_settings.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_settings.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_settings.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_settings.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_settings.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | request_queue.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | lint.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | lint.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | lint.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | lint.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | lint.rs | 466 | Clone in performance-critical code — consider references |
| HIGH | ? | lint.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | semantic_model.rs | 459 | Clone in performance-critical code — consider references |
| HIGH | ? | semantic_model.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 6255 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 8051 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 8791 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 583 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 2071 | Clone in performance-critical code — consider references |
| HIGH | ? | pydantic.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | pydantic.rs | 817 | Clone in performance-critical code — consider references |
| HIGH | ? | pydantic.rs | 856 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 1622 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 1834 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 1835 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 1903 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 2085 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 2215 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 3847 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 3855 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4245 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4252 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4258 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4264 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4265 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4301 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4318 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4402 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4408 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4414 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4419 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 4420 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | bind.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | bind.rs | 3318 | Clone in performance-critical code — consider references |
| HIGH | ? | bind.rs | 6877 | Clone in performance-critical code — consider references |
| HIGH | ? | bind.rs | 6972 | Clone in performance-critical code — consider references |
| HIGH | ? | bind.rs | 6973 | Clone in performance-critical code — consider references |
| HIGH | ? | bind.rs | 6974 | Clone in performance-critical code — consider references |
| HIGH | ? | bind.rs | 7571 | Clone in performance-critical code — consider references |
| HIGH | ? | constructor.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 915 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 918 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 969 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 1219 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 840 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 846 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 876 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 906 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1054 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1269 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1334 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1377 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1395 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1396 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1527 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1528 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1602 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1851 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 1903 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2159 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2220 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2441 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2442 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2478 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2503 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2542 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 2712 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3084 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3281 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3282 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3454 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3455 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3469 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3757 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3768 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3887 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 3908 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4195 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4227 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4239 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4250 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4262 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4390 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4435 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4442 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4469 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4472 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4476 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4479 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4483 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4488 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4492 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4536 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4771 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4783 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4797 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4807 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4809 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4988 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 4991 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5062 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5072 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5082 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5088 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5112 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5116 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5120 | Clone in performance-critical code — consider references |
| HIGH | ? | signatures.rs | 5122 | Clone in performance-critical code — consider references |
| HIGH | ? | class.rs | 1353 | Clone in performance-critical code — consider references |
| HIGH | ? | class.rs | 2185 | Clone in performance-critical code — consider references |
| HIGH | ? | relation_error.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | ide_support.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | ide_support.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | ide_support.rs | 822 | Clone in performance-critical code — consider references |
| HIGH | ? | ide_support.rs | 2099 | Clone in performance-critical code — consider references |
| HIGH | ? | known_instance.rs | 711 | Clone in performance-critical code — consider references |
| HIGH | ? | known_instance.rs | 745 | Clone in performance-critical code — consider references |
| HIGH | ? | class_base.rs | 475 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 1105 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 1803 | Clone in performance-critical code — consider references |
| HIGH | ? | relation.rs | 880 | Clone in performance-critical code — consider references |
| HIGH | ? | match_pattern.rs | 862 | Clone in performance-critical code — consider references |
| HIGH | ? | match_pattern.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | callable.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | callable.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | callable.rs | 737 | Clone in performance-critical code — consider references |
| HIGH | ? | callable.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | dict.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | static_class.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | static_class.rs | 839 | Clone in performance-critical code — consider references |
| HIGH | ? | static_class.rs | 850 | Clone in performance-critical code — consider references |
| HIGH | ? | static_class.rs | 857 | Clone in performance-critical code — consider references |
| HIGH | ? | static_class.rs | 1077 | Clone in performance-critical code — consider references |
| HIGH | ? | static_class.rs | 1094 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | overloaded_function.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_call.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | type_call.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | type_call.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | imports.rs | 418 | Clone in performance-critical code — consider references |
| HIGH | ? | imports.rs | 576 | Clone in performance-critical code — consider references |
| HIGH | ? | new_class.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | named_tuple.rs | 534 | Clone in performance-critical code — consider references |
| HIGH | ? | named_tuple.rs | 683 | Clone in performance-critical code — consider references |
| HIGH | ? | typevar.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | typevar.rs | 1001 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 604 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5043 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5132 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5134 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5155 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5211 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5294 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5313 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5314 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5364 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5365 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5368 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5373 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5397 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 5457 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 6099 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7039 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7147 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7171 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7869 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7886 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7902 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7907 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 7918 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 8013 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 9010 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 9928 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 11188 | Clone in performance-critical code — consider references |
| HIGH | ? | unused_bindings.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | unreachable_code.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 654 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 889 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 971 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 974 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 976 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 982 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 985 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1025 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1034 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1044 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1053 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1069 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1083 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1093 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1096 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1099 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1112 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1141 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1297 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1300 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1309 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1315 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1329 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1352 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1369 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1398 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1404 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1407 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1430 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1435 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1624 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1679 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1680 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1693 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1715 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1763 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1780 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1786 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1845 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 1996 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2017 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2027 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2038 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2062 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2141 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2148 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2163 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2274 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2283 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2467 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2523 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2534 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2557 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 2583 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 3025 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 3065 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 3080 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 3311 | Clone in performance-critical code — consider references |
| HIGH | ? | constraints.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | constraints.rs | 3179 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 1362 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 1556 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 1567 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 1574 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 1658 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 2024 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 2029 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 2061 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 2172 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 2199 | Clone in performance-critical code — consider references |
| HIGH | ? | static_literal.rs | 2319 | Clone in performance-critical code — consider references |
| HIGH | ? | dynamic_literal.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | enum_literal.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | named_tuple.rs | 610 | Clone in performance-critical code — consider references |
| HIGH | ? | tuple.rs | 848 | Clone in performance-critical code — consider references |
| HIGH | ? | tuple.rs | 2936 | Clone in performance-critical code — consider references |
| HIGH | ? | tuple.rs | 2975 | Clone in performance-critical code — consider references |
| HIGH | ? | generics.rs | 1055 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 719 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 1091 | Clone in performance-critical code — consider references |
| HIGH | ? | function.rs | 2591 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1265 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1339 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1340 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1348 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1349 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1447 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclic.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclic.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclic.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclic.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclic.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclic.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 732 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 733 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 744 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 745 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 855 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 1893 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 1902 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 3360 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 3510 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 3532 | Clone in performance-critical code — consider references |
| HIGH | ? | narrow.rs | 3869 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 775 | Clone in performance-critical code — consider references |
| HIGH | ? | enums.rs | 806 | Clone in performance-critical code — consider references |
| HIGH | ? | bound_super.rs | 929 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 578 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 737 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 747 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 769 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 823 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 836 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 888 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 1587 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 1730 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 1762 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 1930 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 1990 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2084 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2108 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2113 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2167 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2467 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2530 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2578 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2726 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2785 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2789 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2810 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2933 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2936 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2971 | Clone in performance-critical code — consider references |
| HIGH | ? | typed_dict.rs | 2973 | Clone in performance-critical code — consider references |
| HIGH | ? | set_theoretic.rs | 805 | Clone in performance-critical code — consider references |
| HIGH | ? | set_theoretic.rs | 814 | Clone in performance-critical code — consider references |
| HIGH | ? | list_members.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | list_members.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | list_members.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | list_members.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | list_members.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | list_members.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | protocol_class.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | protocol_class.rs | 431 | Clone in performance-critical code — consider references |
| HIGH | ? | protocol_class.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | protocol_class.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | protocol_class.rs | 628 | Clone in performance-critical code — consider references |
| HIGH | ? | protocol_class.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | protocol_class.rs | 3074 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | subscript.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | reachability.rs | 313 | Clone in performance-critical code — consider references |
| HIGH | ? | reachability.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | reachability.rs | 1096 | Clone in performance-critical code — consider references |
| HIGH | ? | reachability.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | reachability.rs | 1254 | Clone in performance-critical code — consider references |
| HIGH | ? | reachability.rs | 1267 | Clone in performance-critical code — consider references |
| HIGH | ? | reachability.rs | 1270 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | document.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | document.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | buffer.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | format_extensions.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | parameters.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | except_handler_except_handler.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | arguments.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolated_string_element.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | match_case.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | comprehension.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | alias.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | with_item.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_lambda.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_lambda.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 362 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_generator.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_list.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_if.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_dict_comp.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_attribute.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_unary_op.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_subscript.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_slice.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_list_comp.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_named.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_dict.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_dict.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_like.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | binary_like.rs | 853 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_starred.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_set_comp.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_tuple.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_call.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | expr_set.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | type_params.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_match_or.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_arguments.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_arguments.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_match_mapping.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_match_star.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_match_sequence.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_match_class.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | pattern_match_as.rs | 21 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | implicit.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | docstring.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | docstring.rs | 532 | Clone in performance-critical code — consider references |
| HIGH | ? | normalize.rs | 711 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | node_key.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_ann_assign.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_with.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_class_def.rs | 29 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_import_from.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_assign.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_assign.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_if.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_if.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | suite.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | suite.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | suite.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | suite.rs | 835 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_match.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | clause.rs | 766 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_try.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_function_def.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_function_def.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_for.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | stmt_while.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | formatter.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | formatter.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | formatter.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | formatter.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | formatter.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | ty_walltime.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | ty_walltime.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | module_resolution.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | ty.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | ty.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | ty.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | ty.rs | 1802 | Clone in performance-critical code — consider references |
| HIGH | ? | lexer.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | lexer.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | lexer.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | lexer.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | lexer.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 1922 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 1923 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2136 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2145 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2327 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2423 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2442 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2555 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2574 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2615 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2616 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2665 | Clone in performance-critical code — consider references |
| HIGH | ? | use_def.rs | 2984 | Clone in performance-critical code — consider references |
| HIGH | ? | program.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | program.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | program.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | loop_bindings_visitor.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | re_exports.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | place.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | place.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | platform.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | scope.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | member.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | member.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | definition.rs | 984 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 702 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 715 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1015 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1070 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1181 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1689 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 1802 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2100 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2118 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2144 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2147 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2358 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2481 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2491 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2503 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2530 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2549 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2570 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2824 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2866 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2874 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 2901 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 3044 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 3115 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 3224 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 3787 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 3881 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 3907 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 3994 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 4037 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 4049 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 4088 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 4671 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 4718 | Clone in performance-critical code — consider references |
| HIGH | ? | builder.rs | 4739 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 592 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 602 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 896 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 1030 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 1057 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 750 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 1311 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 1322 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 1325 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 1327 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 1331 | Clone in performance-critical code — consider references |
| HIGH | ? | format.rs | 1338 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | analyze_graph.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 739 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 786 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1418 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1421 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1424 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1427 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1433 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1445 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1453 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1454 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1462 | Clone in performance-critical code — consider references |
| HIGH | ? | args.rs | 1483 | Clone in performance-critical code — consider references |
| HIGH | ? | tokens.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1696 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1716 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1926 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1934 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1938 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1944 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1949 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1978 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 1996 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 2034 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 2071 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 1220 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 1312 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 2889 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 2891 | Clone in performance-critical code — consider references |
| HIGH | ? | nodes.rs | 2896 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1686 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 584 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 585 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 600 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 732 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 872 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 981 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1112 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1147 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1148 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1229 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1233 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1354 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1626 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1709 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1713 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1715 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1723 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1865 | Clone in performance-critical code — consider references |
| HIGH | ? | session.rs | 1868 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | system.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | document.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | did_change_watched_files.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | did_open_notebook.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | did_change_workspace_folders.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostics.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostics.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | code_action.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace_diagnostic.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace_diagnostic.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace_diagnostic.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace_diagnostic.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | completion.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | rename.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | api.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | api.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | api.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | api.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | api.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy_work_done_progress.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy_work_done_progress.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy_work_done_progress.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy_work_done_progress.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy_work_done_progress.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy_work_done_progress.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | lazy_work_done_progress.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | pool.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | main_loop.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | client.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | client.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | client.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | request_queue.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | main.rs | 526 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | notebook.rs | 825 | Clone in performance-critical code — consider references |
| HIGH | ? | config.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 430 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | test.rs | 495 | Clone in performance-critical code — consider references |
| HIGH | ? | violation.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | linter.rs | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2729 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3436 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3505 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3760 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3772 | Clone in performance-critical code — consider references |
| HIGH | ? | definition.rs | 786 | Clone in performance-critical code — consider references |
| HIGH | ? | definition.rs | 813 | Clone in performance-critical code — consider references |
| HIGH | ? | definition.rs | 903 | Clone in performance-critical code — consider references |
| HIGH | ? | definition.rs | 938 | Clone in performance-critical code — consider references |
| HIGH | ? | repeated_append.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | repeated_append.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | repeated_append.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | print_empty_string.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | delete_full_slice.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | verbose_decimal_constructor.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | verbose_decimal_constructor.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_starmap.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | slice_copy.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_enumerate.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | bit_count.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | check_and_remove_from_set.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | check_and_remove_from_set.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | literal_comparisons.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 180 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | lambda_assignment.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | compound_statements.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | suspicious_function_call.rs | 1019 | Clone in performance-critical code — consider references |
| HIGH | ? | redundant_numeric_union.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | redundant_numeric_union.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | duplicate_union_member.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | duplicate_union_member.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | duplicate_union_member.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_literal_union.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_literal_union.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | redundant_none_literal.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | redundant_none_literal.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | redundant_none_literal.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_type_union.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_type_union.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_type_union.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | duplicate_literal_member.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | duplicate_literal_member.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | duplicate_literal_member.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 485 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 688 | Clone in performance-critical code — consider references |
| HIGH | ? | categorize.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | normalize.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | normalize.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | normalize.rs | 100 | Clone in performance-critical code — consider references |
| HIGH | ? | multiple_starts_ends_with.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | numpy_2_0_deprecation.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | needless_bool.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | needless_bool.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | needless_bool.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | needless_bool.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | needless_bool.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | needless_bool.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | needless_bool.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | fix_with.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_bool_op.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_bool_op.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | zip_dict_keys_and_values.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | collapsible_if.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | collapsible_if.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | collapsible_if.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_dict_get.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | yoda_conditions.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | yoda_conditions.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | yoda_conditions.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | yoda_conditions.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_expr.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_expr.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | reimplemented_builtin.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | suppressible_exception.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_ifexp.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_ifexp.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_ifexp.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_ifexp.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_ifexp.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | if_else_block_instead_of_if_exp.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_unary_op.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_unary_op.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_unary_op.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_unary_op.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | ast_unary_op.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | deprecated_mock_import.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | deprecated_mock_import.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | deprecated_mock_import.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | deprecated_mock_import.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | deprecated_mock_import.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | deprecated_mock_import.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_default_type_args.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_default_type_args.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_default_type_args.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_default_type_args.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | use_pep604_annotation.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | convert_typed_dict_functional_to_class.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | convert_typed_dict_functional_to_class.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | convert_typed_dict_functional_to_class.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | timeout_error_alias.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | convert_named_tuple_functional_to_class.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | convert_named_tuple_functional_to_class.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | convert_named_tuple_functional_to_class.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | os_error_alias.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | format_literals.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | format_literals.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | format_literals.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | format_literals.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | outdated_version_block.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | implicit.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | implicit.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | none_not_at_end_of_union.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | never_union.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | implicit_optional.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | implicit_optional.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_regular_expression.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable_fromkeys_value.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable_fromkeys_value.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | mutable_fromkeys_value.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | legacy_form_pytest_raises.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | legacy_form_pytest_raises.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | legacy_form_pytest_raises.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | legacy_form_pytest_raises.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | legacy_form_pytest_raises.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | legacy_form_pytest_raises.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | collection_literal_concatenation.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | collection_literal_concatenation.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | collection_literal_concatenation.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | collection_literal_concatenation.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | collection_literal_concatenation.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | collection_literal_concatenation.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | sort_dunder_slots.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | explicit_f_string_type_conversion.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | explicit_f_string_type_conversion.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | assert_with_print_message.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | assert_with_print_message.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | assert_with_print_message.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | assert_with_print_message.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | assert_with_print_message.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_nested_literal.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_nested_literal.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 517 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 633 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 697 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 749 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 759 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 789 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 790 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 882 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 887 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 902 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 905 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 908 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 923 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 950 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 951 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 952 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 953 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 958 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 961 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 965 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 989 | Clone in performance-critical code — consider references |
| HIGH | ? | fixes.rs | 991 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_dict_comprehension_for_iterable.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_dict_comprehension_for_iterable.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | unused_import.rs | 480 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 714 | Clone in performance-critical code — consider references |
| HIGH | ? | strings.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | redefined_while_unused.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | cformat.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | banned_api.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | banned_api.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | banned_api.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | relative_imports.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | nested_min_max.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | nested_min_max.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | nested_min_max.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | manual_import_from.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | repeated_equality_comparison.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | modified_iterating_set.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | unnecessary_dunder_call.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | no_method_decorator.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | redeclared_assigned_name.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | len_test.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | xcom_pull_in_template_string.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | moved_to_provider_in_3.rs | 1199 | Clone in performance-critical code — consider references |
| HIGH | ? | moved_in_3_1.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | moved_in_3_1.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | suggested_to_move_to_provider_in_3.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | suggested_to_update_3_0.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | suggested_to_update_3_0.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | removal_in_3.rs | 1079 | Clone in performance-critical code — consider references |
| HIGH | ? | removal_in_3.rs | 1095 | Clone in performance-critical code — consider references |
| HIGH | ? | static_join_to_fstring.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 7 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | setattr_with_constant.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | setattr_with_constant.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | unused_loop_control_variable.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | delattr_with_constant.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | assert_false.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | blank_before_after_class.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | capitalized.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | indent.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | runtime_import_in_type_checking_block.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | runtime_import_in_type_checking_block.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | type_alias_quotes.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | typing_only_runtime_import.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | parametrize.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | parametrize.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | unittest_assert.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | unittest_assert.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | unittest_assert.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | unittest_assert.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | unittest_assert.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | unittest_assert.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | unittest_assert.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | assertion.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | assertion.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | unconventional_import_alias.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | codemods.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | codemods.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_set.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 431 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 899 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 920 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 928 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 935 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 982 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 983 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 1001 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 1009 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 3040 | Clone in performance-critical code — consider references |
| HIGH | ? | suppression.rs | 3067 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_selector.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_selector.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | source_kind.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 821 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_table.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | helpers.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostic.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 797 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 891 | Clone in performance-critical code — consider references |
| HIGH | ? | parser.rs | 900 | Clone in performance-critical code — consider references |
| HIGH | ? | matcher.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | matcher.rs | 417 | Clone in performance-critical code — consider references |
| HIGH | ? | matcher.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | matcher.rs | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | matcher.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 1249 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 1256 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 1500 | Clone in performance-critical code — consider references |
| HIGH | ? | options.rs | 3055 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 2266 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 2275 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 2285 | Clone in performance-critical code — consider references |
| HIGH | ? | configuration.rs | 2289 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 919 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 976 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 977 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 1287 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 2604 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 2647 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 2669 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 2770 | Clone in performance-critical code — consider references |
| HIGH | ? | resolve.rs | 3302 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 979 | Clone in performance-critical code — consider references |
| HIGH | ? | module_name.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | db.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 686 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 905 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 942 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 1106 | Clone in performance-critical code — consider references |
| HIGH | ? | path.rs | 1118 | Clone in performance-critical code — consider references |
| HIGH | ? | module.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | module.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | module.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | module.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | visibility.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | display_list.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | display_list.rs | 1420 | Clone in performance-critical code — consider references |
| HIGH | ? | display_list.rs | 1428 | Clone in performance-critical code — consider references |
| HIGH | ? | display_list.rs | 1482 | Clone in performance-critical code — consider references |
| HIGH | ? | display_list.rs | 1523 | Clone in performance-critical code — consider references |
| HIGH | ? | env_vars.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | env_vars.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | map_codes.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | map_codes.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | map_codes.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_namespace.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_namespace.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_namespace.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | config.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | config.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | rule_code_prefix.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | cache_key.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | recovery.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | interpolated_string.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | indentation.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | semantic_errors.rs | 2248 | Clone in performance-critical code — consider references |
| HIGH | ? | semantic_errors.rs | 2339 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_formatter_idempotency.rs | 19 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_formatter_idempotency.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | ty_check_invalid_syntax.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | ty_check_invalid_syntax.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_formatter_validity.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | ruff_formatter_validity.rs | 64 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 33 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 43 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 51 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 60 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 86 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 96 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 104 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 113 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 128 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 138 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 146 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 155 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 170 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 180 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 188 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 197 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 463 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 472 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 482 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 491 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 590 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 598 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 604 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S608_S608.py.snap | 612 |
| C | ? | S608.py | 6 |
| C | ? | S608.py | 12 |
| C | ? | S608.py | 17 |
| C | ? | S608.py | 22 |
| C | ? | S608.py | 136 |
| C | ? | S608.py | 140 |
| M | ? | 62_try_except_double_nested_inside_if_else.py | 5 |
| M | ? | 62_try_except_double_nested_inside_if_else.py | 7 |
| M | ? | 60_try_except_bare.py | 3 |
| M | ? | 67_with_inside_try_finally_preceding_terminal_except.py | 5 |
| M | ? | 62_try_except_break.py | 5 |
| M | ? | 15_while_break_non_exit.py | 4 |
| M | ? | or_else.py | 25 |
| M | ? | compound_one_liners.py | 36 |
| M | ? | compound_one_liners.py | 124 |
| M | ? | blank_line_after_nested_stub_class.pyi | 164 |
| M | ? | try.py | 3 |
| M | ? | try.py | 58 |
| M | ? | try.py | 70 |
| M | ? | try.py | 112 |
| M | ? | try.py | 127 |
| M | ? | try.py | 135 |
| M | ? | ellipsis.pyi | 86 |
| M | ? | ellipsis.pyi | 94 |
| M | ? | ellipsis.pyi | 103 |
| M | ? | allow_empty_first_line.py | 35 |
| M | ? | pep_654.py.expect | 18 |
| M | ? | remove_except_types_parens_pre_py314.py | 5 |
| M | ? | pep_654.py | 18 |
| M | ? | allow_empty_first_line.py.expect | 35 |
| M | ? | pep_654_style.py | 18 |
| M | ? | remove_except_types_parens_pre_py314.py.expect | 5 |
| M | ? | pep_654_style.py.expect | 18 |
| M | ? | remove_except_types_parens.py | 5 |
| M | ? | remove_except_types_parens.py.expect | 5 |
| M | ? | except_handler.rs | 31 |
| M | ? | ruff_linter__rules__perflint__tests__PERF203_PERF203.py.snap | 9 |
| M | ? | ruff_linter__rules__pycodestyle__tests__E722_E722.py.snap | 9 |
| M | ? | ruff_linter__rules__pycodestyle__tests__E722_E722.py.snap | 20 |
| M | ? | ruff_linter__rules__pycodestyle__tests__E722_E722.py.snap | 31 |
| M | ? | mod.rs | 4 |
| M | ? | mod.rs | 1 |
| M | ? | ruff_linter__rules__flake8_bandit__tests__S112_S112.py.snap | 21 |
| M | ? | ruff_linter__rules__flake8_bandit__tests__S110_S110.py.snap | 21 |
| M | ? | ruff_linter__rules__flake8_bandit__tests__S110_typed.snap | 21 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 183 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 200 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 207 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 216 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 224 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 233 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 240 |
| M | ? | ruff_linter__rules__eradicate__tests__ERA001_ERA001.py.snap | 249 |
| M | ? | detection.rs | 206 |
| M | ? | detection.rs | 212 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G201.py.snap | 8 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G201.py.snap | 19 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G201.py.snap | 30 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G201.py.snap | 41 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G202.py.snap | 8 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G202.py.snap | 19 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G202.py.snap | 30 |
| M | ? | ruff_linter__rules__flake8_logging_format__tests__G202.py.snap | 41 |
| M | ? | ruff_linter__rules__tryceratops__tests__useless-try-except_TRY203.py.snap | 34 |
| M | ? | mod.rs | 8 |
| M | ? | ruff_linter__rules__flake8_simplify__tests__SIM105_SIM105_0.py.snap | 89 |
| M | ? | ruff_linter__rules__flake8_simplify__tests__SIM105_SIM105_0.py.snap | 104 |
| M | ? | ruff_linter__rules__ruff__tests__RUF047_RUF047_try.py.snap | 7 |
| M | ? | ruff_linter__rules__ruff__tests__RUF047_RUF047_try.py.snap | 24 |
| M | ? | mod.rs | 1865 |
| M | ? | mod.rs | 2167 |
| M | ? | mod.rs | 2183 |
| M | ? | mod.rs | 2201 |
| M | ? | mod.rs | 2219 |
| M | ? | mod.rs | 2707 |
| M | ? | mod.rs | 2719 |
| M | ? | ruff_linter__rules__pyflakes__tests__F707_F707.py.snap | 9 |
| M | ? | ruff_linter__rules__pyflakes__tests__F707_F707.py.snap | 20 |
| M | ? | ruff_linter__rules__pyflakes__tests__F707_F707.py.snap | 31 |
| M | ? | ruff_linter__rules__pyflakes__tests__F811_F811_8.py.snap | 12 |
| M | ? | ruff_linter__rules__pyflakes__tests__F811_F811_8.py.snap | 19 |
| M | ? | ruff_linter__rules__pylint__tests__PLW0129_assert_on_string_literal.py.snap | 19 |
| M | ? | ruff_linter__rules__pylint__tests__PLW0129_assert_on_string_literal.py.snap | 27 |
| M | ? | ruff_linter__rules__pylint__tests__PLE0704_misplaced_bare_raise.py.snap | 71 |
| M | ? | ruff_linter__rules__pylint__tests__PLE0704_misplaced_bare_raise.py.snap | 82 |
| M | ? | too_many_branches.rs | 349 |
| M | ? | too_many_branches.rs | 362 |
| M | ? | too_many_branches.rs | 390 |
| M | ? | too_many_branches.rs | 392 |
| M | ? | helpers.rs | 678 |
| M | ? | helpers.rs | 680 |
| M | ? | mod.rs | 25 |
| M | ? | ruff_linter__rules__flake8_pytest_style__tests__PT031.snap | 84 |
| M | ? | ruff_linter__rules__flake8_pytest_style__tests__PT012.snap | 84 |
| M | ? | mod.rs | 394 |
| M | ? | codes.rs | 411 |
| M | ? | PERF203.py | 5 |
| M | ? | PERF203.py | 12 |
| M | ? | PERF203.py | 20 |
| M | ? | PERF203.py | 30 |
| M | ? | PERF203.py | 38 |
| M | ? | PERF203.py | 48 |
| M | ? | auto_return_type.py | 115 |
| M | ? | auto_return_type.py | 122 |
| M | ? | auto_return_type.py | 131 |
| M | ? | auto_return_type.py | 140 |
| M | ? | auto_return_type.py | 190 |
| M | ? | auto_return_type.py | 197 |
| M | ? | auto_return_type.py | 251 |
| M | ? | auto_return_type.py | 258 |
| M | ? | auto_return_type.py | 293 |
| M | ? | E721.py | 67 |
| M | ? | E721.py | 74 |
| M | ? | E721.py | 79 |
| M | ? | E721.py | 85 |
| M | ? | E722.py | 4 |
| M | ? | E722.py | 11 |
| M | ? | E722.py | 16 |
| M | ? | E722.py | 22 |
| M | ? | E30.py | 347 |
| M | ? | S110.py | 8 |
| M | ? | S112.py | 9 |
| M | ? | RET502.py | 38 |
| M | ? | try.py | 16 |
| M | ? | try.py | 22 |
| M | ? | try.py | 54 |
| M | ? | try.py | 62 |
| M | ? | try.py | 69 |
| M | ? | try.py | 130 |
| M | ? | G201.py | 7 |
| M | ? | G201.py | 12 |
| M | ? | G201.py | 18 |
| M | ? | G201.py | 27 |
| M | ? | G201.py | 32 |
| M | ? | G201.py | 38 |
| M | ? | G202.py | 7 |
| M | ? | G202.py | 12 |
| M | ? | G202.py | 18 |
| M | ? | G202.py | 27 |
| M | ? | G202.py | 32 |
| M | ? | G202.py | 38 |
| M | ? | TRY203.py | 25 |
| M | ? | SIM107.py | 6 |
| M | ? | SIM107.py | 18 |
| M | ? | SIM113.py | 107 |
| M | ? | SIM105_0.py | 27 |
| M | ? | UP041.py | 56 |
| M | ? | UP024_0.py | 78 |
| M | ? | RUF047_try.py | 5 |
| M | ? | RUF047_try.py | 15 |
| M | ? | RUF047_try.py | 23 |
| M | ? | RUF047_try.py | 34 |
| M | ? | RUF047_try.py | 54 |
| M | ? | RUF047_try.py | 63 |
| M | ? | RUF047_try.py | 70 |
| M | ? | DOC501_numpy.py | 77 |
| M | ? | DOC501_google.py | 64 |
| M | ? | F811_8.py | 6 |
| M | ? | F811_9.py | 5 |
| M | ? | F811_11.py | 7 |
| M | ? | F707.py | 3 |
| M | ? | F707.py | 10 |
| M | ? | F707.py | 19 |
| M | ? | F707.py | 28 |
| M | ? | F707.py | 35 |
| M | ? | F811_10.py | 6 |
| M | ? | misplaced_bare_raise.py | 56 |
| M | ? | misplaced_bare_raise.py | 62 |
| M | ? | misplaced_bare_raise.py | 68 |
| M | ? | assert_on_string_literal.py | 13 |
| M | ? | PT012.py | 74 |
| M | ? | PT031.py | 74 |
| M | ? | try.py | 3 |
| M | ? | try.py | 17 |
| M | ? | try.py | 24 |
| M | ? | try.py | 31 |
| M | ? | lazy_import_invalid_context_py315.py | 4 |
| M | ? | try_stmt_mixed_except_kind.py | 3 |
| M | ? | try_stmt_mixed_except_kind.py | 11 |
| M | ? | try_stmt_mixed_except_kind.py | 15 |
| M | ? | try_stmt_mixed_except_kind.py | 17 |
| M | ? | try_stmt_misspelled_except.py | 10 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| L | ? | type_alias.py | 28 |
| L | ? | dataset.py | 499 |
| L | ? | dataset.py | 899 |
| L | ? | dataset.py | 920 |
| L | ? | dataset.py | 1000 |
| L | ? | PYI063.pyi | 26 |
| L | ? | RUF053.py | 26 |
| L | ? | RUF053.py | 27 |
| L | ? | RUF053.py | 28 |
| L | ? | RUF053.py | 33 |
| L | ? | RUF053.py | 38 |
| L | ? | RUF053.py | 61 |
| L | ? | RUF053.py | 66 |
| L | ? | missing_maxsplit_arg.py | 141 |
| L | ? | missing_maxsplit_arg.py | 143 |
| L | ? | missing_maxsplit_arg.py | 173 |
| L | ? | missing_maxsplit_arg.py | 174 |
| L | ? | missing_maxsplit_arg.py | 184 |
| L | ? | missing_maxsplit_arg.py | 187 |
| L | ? | missing_maxsplit_arg.py | 189 |
| L | ? | add_rule.py | 119 |
| L | ? | add_plugin.py | 131 |
| H | ? | Editor.tsx | 360 |
| H | ? | Editor.tsx | 539 |
| H | ? | Editor.tsx | 544 |
| H | ? | Editor.tsx | 549 |
| H | ? | Editor.tsx | 329 |
| H | ? | settings.ts | 4 |
| H | ? | SettingsEditor.tsx | 127 |
| M | ? | SettingsEditor.tsx | 95 |
| M | ? | pandas_html.py | 999 |
| M | ? | mdtest.py | 136 |
| M | ? | 64_assert.py | 1 |
| M | ? | 64_assert.py | 2 |
| M | ? | abstract_methods_cycle_regression.py | 9 |
| M | ? | 88_regression_issue_17792.py | 15 |
| M | ? | classliteral_decorators_cycle.py | 21 |
| M | ? | 67_with_multi_exit.py | 5 |
| M | ? | cyclic_lambdas.py | 13 |
| M | ? | fstring.py | 590 |
| M | ? | fstring.py | 594 |
| M | ? | fstring.py | 597 |
| M | ? | fstring.py | 599 |
| M | ? | fstring.py | 602 |
| M | ? | fstring.py | 604 |
| M | ? | fstring.py | 608 |
| M | ? | compare.py | 128 |
| M | ? | join_implicit_concatenated_string.py | 217 |
| M | ? | join_implicit_concatenated_string.py | 220 |
| M | ? | join_implicit_concatenated_string.py | 223 |
| M | ? | join_implicit_concatenated_string.py | 226 |
| M | ? | join_implicit_concatenated_string.py | 229 |
| M | ? | join_implicit_concatenated_string.py | 232 |
| M | ? | join_implicit_concatenated_string.py | 235 |
| M | ? | join_implicit_concatenated_string.py | 358 |
| M | ? | join_implicit_concatenated_string.py | 362 |
| M | ? | join_implicit_concatenated_string.py | 366 |
| M | ? | join_implicit_concatenated_string.py | 370 |
| M | ? | tstring.py | 571 |
| M | ? | tstring.py | 575 |
| M | ? | tstring.py | 578 |
| M | ? | tstring.py | 580 |
| M | ? | tstring.py | 583 |
| M | ? | tstring.py | 585 |
| M | ? | tstring.py | 589 |
| M | ? | named_expr.py | 61 |
| M | ? | opening_parentheses_comment_empty.py | 22 |
| M | ? | opening_parentheses_comment_value.py | 22 |
| M | ? | assert.py | 1 |
| M | ? | assert.py | 2 |
| M | ? | assert.py | 3 |
| M | ? | assert.py | 4 |
| M | ? | assert.py | 6 |
| M | ? | assert.py | 12 |
| M | ? | assert.py | 23 |
| M | ? | assert.py | 33 |
| M | ? | assert.py | 47 |
| M | ? | assert.py | 61 |
| M | ? | assert.py | 73 |
| M | ? | assert.py | 88 |
| M | ? | assert.py | 103 |
| M | ? | assert.py | 115 |
| M | ? | assert.py | 127 |
| M | ? | assert.py | 142 |
| M | ? | assert.py | 158 |
| M | ? | assert.py | 162 |
| M | ? | composition_no_trailing_comma.py | 62 |
| M | ? | composition_no_trailing_comma.py | 74 |
| M | ? | composition_no_trailing_comma.py | 86 |
| M | ? | composition_no_trailing_comma.py | 99 |
| M | ? | composition_no_trailing_comma.py | 113 |
| M | ? | composition_no_trailing_comma.py | 127 |
| M | ? | composition_no_trailing_comma.py | 141 |
| M | ? | collections.py | 40 |
| M | ? | preview_long_strings__edge_case.py | 32 |
| M | ? | preview_long_strings__edge_case.py | 33 |
| M | ? | preview_long_strings__edge_case.py | 34 |
| M | ? | function.py | 33 |
| M | ? | function.py | 36 |
| M | ? | preview_multiline_strings.py | 159 |
| M | ? | preview_multiline_strings.py | 162 |
| M | ? | preview_long_strings.py | 143 |
| M | ? | preview_long_strings.py | 145 |
| M | ? | preview_long_strings.py | 147 |
| M | ? | preview_long_strings.py | 149 |
| M | ? | torture.py | 3 |
| M | ? | torture.py | 26 |
| M | ? | expression.py | 186 |
| M | ? | composition.py | 62 |
| M | ? | composition.py | 74 |
| M | ? | composition.py | 86 |
| M | ? | composition.py | 99 |
| M | ? | composition.py | 113 |
| M | ? | composition.py | 127 |
| M | ? | composition.py | 141 |
| M | ? | tuple_with_stmt.py | 30 |
| M | ? | trailing_commas_in_leading_parts.py | 23 |
| M | ? | trailing_commas_in_leading_parts.py | 29 |
| M | ? | empty_lines.py | 20 |
| M | ? | empty_lines.py | 73 |
| M | ? | fmtonoff2.py | 31 |
| M | ? | pattern_matching_extras.py | 34 |
| M | ? | pattern_matching_extras.py | 36 |
| M | ? | pep_572_remove_parens.py | 21 |
| M | ? | long_strings_flag_disabled.py | 170 |
| M | ? | long_strings_flag_disabled.py | 174 |
| M | ? | long_strings_flag_disabled.py | 180 |
| M | ? | long_strings_flag_disabled.py | 185 |
| M | ? | fmtonoff.py | 43 |
| M | ? | types.py | 765 |
| M | ? | types.py | 781 |
| M | ? | types.py | 813 |
| M | ? | types.py | 829 |
| M | ? | dataset.py | 77 |
| M | ? | dataset.py | 78 |
| M | ? | dataset.py | 79 |
| M | ? | dataset.py | 80 |
| M | ? | dataset.py | 88 |
| M | ? | dataset.py | 89 |
| M | ? | dataset.py | 91 |
| M | ? | dataset.py | 92 |
| M | ? | dataset.py | 93 |
| M | ? | dataset.py | 94 |
| M | ? | dataset.py | 95 |
| M | ? | dataset.py | 97 |
| M | ? | dataset.py | 98 |
| M | ? | dataset.py | 99 |
| M | ? | dataset.py | 100 |
| M | ? | dataset.py | 104 |
| M | ? | dataset.py | 109 |
| M | ? | dataset.py | 110 |
| M | ? | dataset.py | 111 |
| M | ? | dataset.py | 112 |
| M | ? | dataset.py | 115 |
| M | ? | dataset.py | 118 |
| M | ? | dataset.py | 119 |
| M | ? | dataset.py | 120 |
| M | ? | dataset.py | 121 |
| M | ? | dataset.py | 126 |
| M | ? | dataset.py | 127 |
| M | ? | dataset.py | 128 |
| M | ? | dataset.py | 129 |
| M | ? | dataset.py | 137 |
| M | ? | dataset.py | 138 |
| M | ? | dataset.py | 139 |
| M | ? | dataset.py | 162 |
| M | ? | dataset.py | 163 |
| M | ? | dataset.py | 166 |
| M | ? | dataset.py | 192 |
| M | ? | dataset.py | 193 |
| M | ? | dataset.py | 195 |
| M | ? | dataset.py | 198 |
| M | ? | dataset.py | 206 |
| M | ? | dataset.py | 207 |
| M | ? | dataset.py | 210 |
| M | ? | dataset.py | 211 |
| M | ? | dataset.py | 215 |
| M | ? | dataset.py | 216 |
| M | ? | dataset.py | 220 |
| M | ? | dataset.py | 221 |
| M | ? | dataset.py | 224 |
| M | ? | dataset.py | 225 |
| M | ? | dataset.py | 265 |
| M | ? | dataset.py | 266 |
| M | ? | dataset.py | 267 |
| M | ? | dataset.py | 268 |
| M | ? | dataset.py | 269 |
| M | ? | dataset.py | 273 |
| M | ? | dataset.py | 274 |
| M | ? | dataset.py | 279 |
| M | ? | dataset.py | 283 |
| M | ? | dataset.py | 291 |
| M | ? | dataset.py | 310 |
| M | ? | dataset.py | 311 |
| M | ? | dataset.py | 325 |
| M | ? | dataset.py | 326 |
| M | ? | dataset.py | 330 |
| M | ? | dataset.py | 331 |
| M | ? | dataset.py | 334 |
| M | ? | dataset.py | 337 |
| M | ? | dataset.py | 340 |
| M | ? | dataset.py | 354 |
| M | ? | dataset.py | 357 |
| M | ? | dataset.py | 360 |
| M | ? | dataset.py | 377 |
| M | ? | dataset.py | 414 |
| M | ? | dataset.py | 417 |
| M | ? | dataset.py | 418 |
| M | ? | dataset.py | 419 |
| M | ? | dataset.py | 421 |
| M | ? | dataset.py | 425 |
| M | ? | dataset.py | 428 |
| M | ? | dataset.py | 429 |
| M | ? | dataset.py | 430 |
| M | ? | dataset.py | 431 |
| M | ? | dataset.py | 435 |
| M | ? | dataset.py | 438 |
| M | ? | dataset.py | 439 |
| M | ? | dataset.py | 440 |
| M | ? | dataset.py | 441 |
| M | ? | dataset.py | 460 |
| M | ? | dataset.py | 477 |
| M | ? | dataset.py | 478 |
| M | ? | dataset.py | 479 |
| M | ? | dataset.py | 484 |
| M | ? | dataset.py | 485 |
| M | ? | dataset.py | 486 |
| M | ? | dataset.py | 505 |
| M | ? | dataset.py | 506 |
| M | ? | dataset.py | 507 |
| M | ? | dataset.py | 508 |
| M | ? | dataset.py | 522 |
| M | ? | dataset.py | 523 |
| M | ? | dataset.py | 524 |
| M | ? | dataset.py | 525 |
| M | ? | dataset.py | 541 |
| M | ? | dataset.py | 558 |
| M | ? | dataset.py | 559 |
| M | ? | dataset.py | 585 |
| M | ? | dataset.py | 599 |
| M | ? | dataset.py | 603 |
| M | ? | dataset.py | 604 |
| M | ? | dataset.py | 607 |
| M | ? | dataset.py | 619 |
| M | ? | dataset.py | 633 |
| M | ? | dataset.py | 634 |
| M | ? | dataset.py | 635 |
| M | ? | dataset.py | 636 |
| M | ? | dataset.py | 640 |
| M | ? | dataset.py | 651 |
| M | ? | dataset.py | 665 |
| M | ? | dataset.py | 666 |
| M | ? | dataset.py | 667 |
| M | ? | dataset.py | 668 |
| M | ? | dataset.py | 669 |
| M | ? | dataset.py | 670 |
| M | ? | dataset.py | 680 |
| M | ? | dataset.py | 703 |
| M | ? | dataset.py | 716 |
| M | ? | dataset.py | 727 |
| M | ? | dataset.py | 733 |
| M | ? | dataset.py | 760 |
| M | ? | dataset.py | 761 |
| M | ? | dataset.py | 773 |
| M | ? | dataset.py | 779 |
| M | ? | dataset.py | 788 |
| M | ? | dataset.py | 801 |
| M | ? | dataset.py | 802 |
| M | ? | dataset.py | 803 |
| M | ? | dataset.py | 804 |
| M | ? | dataset.py | 810 |
| M | ? | dataset.py | 823 |
| M | ? | dataset.py | 837 |
| M | ? | dataset.py | 842 |
| M | ? | dataset.py | 843 |
| M | ? | dataset.py | 845 |
| M | ? | dataset.py | 846 |
| M | ? | dataset.py | 850 |
| M | ? | dataset.py | 851 |
| M | ? | dataset.py | 852 |
| M | ? | dataset.py | 857 |
| M | ? | dataset.py | 858 |
| M | ? | dataset.py | 860 |
| M | ? | dataset.py | 861 |
| M | ? | dataset.py | 862 |
| M | ? | dataset.py | 866 |
| M | ? | dataset.py | 867 |
| M | ? | dataset.py | 868 |
| M | ? | dataset.py | 869 |
| M | ? | dataset.py | 870 |
| M | ? | dataset.py | 872 |
| M | ? | dataset.py | 873 |
| M | ? | dataset.py | 874 |
| M | ? | dataset.py | 885 |
| M | ? | dataset.py | 886 |
| M | ? | dataset.py | 891 |
| M | ? | dataset.py | 892 |
| M | ? | dataset.py | 902 |
| M | ? | dataset.py | 903 |
| M | ? | dataset.py | 904 |
| M | ? | dataset.py | 905 |
| M | ? | dataset.py | 909 |
| M | ? | dataset.py | 910 |
| M | ? | dataset.py | 911 |
| M | ? | dataset.py | 918 |
| M | ? | dataset.py | 924 |
| M | ? | dataset.py | 925 |
| M | ? | dataset.py | 926 |
| M | ? | dataset.py | 927 |
| M | ? | dataset.py | 928 |
| M | ? | dataset.py | 945 |
| M | ? | dataset.py | 946 |
| M | ? | dataset.py | 947 |
| M | ? | dataset.py | 953 |
| M | ? | dataset.py | 954 |
| M | ? | dataset.py | 971 |
| M | ? | dataset.py | 972 |
| M | ? | dataset.py | 976 |
| M | ? | dataset.py | 982 |
| M | ? | dataset.py | 983 |
| M | ? | dataset.py | 989 |
| M | ? | dataset.py | 992 |
| M | ? | dataset.py | 998 |
| M | ? | dataset.py | 999 |
| M | ? | dataset.py | 1000 |
| M | ? | dataset.py | 1006 |
| M | ? | dataset.py | 1007 |
| M | ? | dataset.py | 1008 |
| M | ? | dataset.py | 1011 |
| M | ? | dataset.py | 1012 |
| M | ? | dataset.py | 1013 |
| M | ? | dataset.py | 1016 |
| M | ? | dataset.py | 1017 |
| M | ? | dataset.py | 1018 |
| M | ? | dataset.py | 1024 |
| M | ? | dataset.py | 1025 |
| M | ? | dataset.py | 1028 |
| M | ? | dataset.py | 1032 |
| M | ? | dataset.py | 1033 |
| M | ? | dataset.py | 1047 |
| M | ? | dataset.py | 1048 |
| M | ? | dataset.py | 1061 |
| M | ? | dataset.py | 1065 |
| M | ? | dataset.py | 1067 |
| M | ? | dataset.py | 1069 |
| M | ? | dataset.py | 1073 |
| M | ? | dataset.py | 1077 |
| M | ? | dataset.py | 1108 |
| M | ? | dataset.py | 1109 |
| M | ? | dataset.py | 1110 |
| M | ? | dataset.py | 1111 |
| M | ? | dataset.py | 1112 |
| M | ? | dataset.py | 1119 |
| M | ? | dataset.py | 1120 |
| M | ? | dataset.py | 1121 |
| M | ? | dataset.py | 1122 |
| M | ? | dataset.py | 1123 |
| M | ? | dataset.py | 1124 |
| M | ? | dataset.py | 1125 |
| M | ? | dataset.py | 1126 |
| M | ? | dataset.py | 1132 |
| M | ? | dataset.py | 1133 |
| M | ? | dataset.py | 1137 |
| M | ? | dataset.py | 1138 |
| M | ? | dataset.py | 1142 |
| M | ? | dataset.py | 1143 |
| M | ? | dataset.py | 1163 |
| M | ? | dataset.py | 1164 |
| M | ? | dataset.py | 1165 |
| M | ? | dataset.py | 1170 |
| M | ? | dataset.py | 1173 |
| M | ? | dataset.py | 1174 |
| M | ? | dataset.py | 1181 |
| M | ? | dataset.py | 1204 |
| M | ? | dataset.py | 1205 |
| M | ? | dataset.py | 1208 |
| M | ? | dataset.py | 1209 |
| M | ? | dataset.py | 1210 |
| M | ? | dataset.py | 1215 |
| M | ? | dataset.py | 1218 |
| M | ? | dataset.py | 1219 |
| M | ? | dataset.py | 1224 |
| M | ? | dataset.py | 1225 |
| M | ? | dataset.py | 1228 |
| M | ? | dataset.py | 1229 |
| M | ? | dataset.py | 1248 |
| M | ? | dataset.py | 1249 |
| M | ? | dataset.py | 1266 |
| M | ? | dataset.py | 1274 |
| M | ? | dataset.py | 1275 |
| M | ? | dataset.py | 1276 |
| M | ? | dataset.py | 1277 |
| M | ? | dataset.py | 1278 |
| M | ? | dataset.py | 1279 |
| M | ? | dataset.py | 1287 |
| M | ? | dataset.py | 1288 |
| M | ? | dataset.py | 1289 |
| M | ? | dataset.py | 1290 |
| M | ? | dataset.py | 1291 |
| M | ? | dataset.py | 1292 |
| M | ? | dataset.py | 1293 |
| M | ? | dataset.py | 1294 |
| M | ? | dataset.py | 1302 |
| M | ? | dataset.py | 1303 |
| M | ? | dataset.py | 1304 |
| M | ? | dataset.py | 1305 |
| M | ? | dataset.py | 1306 |
| M | ? | dataset.py | 1307 |
| M | ? | dataset.py | 1308 |
| M | ? | dataset.py | 1309 |
| M | ? | dataset.py | 1325 |
| M | ? | dataset.py | 1333 |
| M | ? | dataset.py | 1334 |
| M | ? | dataset.py | 1345 |
| M | ? | dataset.py | 1346 |
| M | ? | dataset.py | 1347 |
| M | ? | dataset.py | 1351 |
| M | ? | dataset.py | 1352 |
| M | ? | dataset.py | 1354 |
| M | ? | dataset.py | 1355 |
| M | ? | dataset.py | 1356 |
| M | ? | dataset.py | 1360 |
| M | ? | dataset.py | 1361 |
| M | ? | dataset.py | 1362 |
| M | ? | dataset.py | 1374 |
| M | ? | dataset.py | 1375 |
| M | ? | dataset.py | 1376 |
| M | ? | dataset.py | 1381 |
| M | ? | dataset.py | 1383 |
| M | ? | dataset.py | 1387 |
| M | ? | dataset.py | 1389 |
| M | ? | dataset.py | 1390 |
| M | ? | dataset.py | 1391 |
| M | ? | dataset.py | 1398 |
| M | ? | dataset.py | 1399 |
| M | ? | dataset.py | 1409 |
| M | ? | dataset.py | 1410 |
| M | ? | dataset.py | 1411 |
| M | ? | dataset.py | 1412 |
| M | ? | dataset.py | 1413 |
| M | ? | dataset.py | 1414 |
| M | ? | dataset.py | 1424 |
| M | ? | dataset.py | 1425 |
| M | ? | dataset.py | 1426 |
| M | ? | dataset.py | 1427 |
| M | ? | dataset.py | 1428 |
| M | ? | dataset.py | 1429 |
| M | ? | dataset.py | 1430 |
| M | ? | dataset.py | 1440 |
| M | ? | dataset.py | 1441 |
| M | ? | dataset.py | 1442 |
| M | ? | dataset.py | 1452 |
| M | ? | dataset.py | 1453 |
| M | ? | dataset.py | 1454 |
| M | ? | dataset.py | 1455 |
| M | ? | dataset.py | 1463 |
| M | ? | dataset.py | 1477 |
| M | ? | dataset.py | 1485 |
| M | ? | dataset.py | 1494 |
| M | ? | dataset.py | 1513 |
| M | ? | dataset.py | 1531 |
| M | ? | dataset.py | 1532 |
| M | ? | dataset.py | 1549 |
| M | ? | dataset.py | 1561 |
| M | ? | dataset.py | 1562 |
| M | ? | dataset.py | 1563 |
| M | ? | dataset.py | 1564 |
| M | ? | dataset.py | 1568 |
| M | ? | dataset.py | 1569 |
| M | ? | dataset.py | 1570 |
| M | ? | dataset.py | 1571 |
| M | ? | dataset.py | 1577 |
| M | ? | dataset.py | 1578 |
| M | ? | dataset.py | 1579 |
| M | ? | dataset.py | 1584 |
| M | ? | dataset.py | 1587 |
| M | ? | dataset.py | 1606 |
| M | ? | dataset.py | 1607 |
| M | ? | dataset.py | 1608 |
| M | ? | dataset.py | 1611 |
| M | ? | dataset.py | 1612 |
| M | ? | FURB118.py | 134 |
| M | ? | N802.py | 41 |
| M | ? | E721.py | 21 |
| M | ? | E721.py | 23 |
| M | ? | E721.py | 25 |
| M | ? | E721.py | 27 |
| M | ? | E721.py | 29 |
| M | ? | E721.py | 31 |
| M | ? | E721.py | 33 |
| M | ? | E721.py | 35 |
| M | ? | E721.py | 37 |
| M | ? | E721.py | 39 |
| M | ? | E721.py | 41 |
| M | ? | E711.py | 51 |
| M | ? | E711.py | 52 |
| M | ? | E711.py | 53 |
| M | ? | E711.py | 55 |
| M | ? | E714.py | 36 |
| M | ? | E714.py | 37 |
| M | ? | E714.py | 38 |
| M | ? | E714.py | 39 |
| M | ? | E713.py | 36 |
| M | ? | E713.py | 37 |
| M | ? | E713.py | 38 |
| M | ? | E713.py | 39 |
| M | ? | E713.py | 40 |
| M | ? | E712.py | 53 |
| M | ? | E712.py | 54 |
| M | ? | E712.py | 55 |
| M | ? | S101.py | 1 |
| M | ? | S101.py | 6 |
| M | ? | S101.py | 7 |
| M | ? | S101.py | 13 |
| M | ? | RET503.py | 109 |
| M | ? | try.py | 67 |
| M | ? | try.py | 81 |
| M | ? | try.py | 113 |
| M | ? | assert.py | 2 |
| M | ? | assert.py | 5 |
| M | ? | assert.py | 8 |
| M | ? | assert.py | 11 |
| M | ? | assert.py | 15 |
| M | ? | assert.py | 16 |
| M | ? | assert.py | 17 |
| M | ? | assert.py | 21 |
| M | ? | assert.py | 27 |
| M | ? | assert.py | 36 |
| M | ? | for.py | 65 |
| M | ? | if.py | 128 |
| M | ? | PGH005_0.py | 4 |
| M | ? | PGH005_0.py | 5 |
| M | ? | PGH005_0.py | 6 |
| M | ? | PGH005_0.py | 7 |
| M | ? | PGH005_0.py | 25 |
| M | ? | PGH005_0.py | 26 |
| M | ? | PGH005_0.py | 36 |
| M | ? | PGH005_0.py | 37 |
| M | ? | PGH005_0.py | 38 |
| M | ? | PGH005_0.py | 39 |
| M | ? | PGH005_0.py | 45 |
| M | ? | PGH005_0.py | 59 |
| M | ? | SIM222.py | 104 |
| M | ? | SIM223.py | 99 |
| M | ? | UP003.py | 14 |
| M | ? | RUF040.py | 3 |
| M | ? | RUF040.py | 5 |
| M | ? | RUF018.py | 2 |
| M | ? | RUF018.py | 3 |
| M | ? | RUF018.py | 16 |
| M | ? | RUF018.py | 17 |
| M | ? | RUF018.py | 20 |
| M | ? | confusables.py | 55 |
| M | ? | RUF021.py | 38 |
| M | ? | RUF021.py | 114 |
| M | ? | RUF056.py | 131 |
| M | ? | RUF061_raises.py | 36 |
| M | ? | RUF030.py | 6 |
| M | ? | RUF030.py | 11 |
| M | ? | RUF030.py | 16 |
| M | ? | RUF030.py | 21 |
| M | ? | RUF030.py | 26 |
| M | ? | RUF030.py | 31 |
| M | ? | RUF030.py | 36 |
| M | ? | RUF030.py | 41 |
| M | ? | RUF030.py | 46 |
| M | ? | RUF030.py | 51 |
| M | ? | RUF030.py | 56 |
| M | ? | RUF030.py | 61 |
| M | ? | RUF030.py | 66 |
| M | ? | RUF030.py | 71 |
| M | ? | RUF030.py | 76 |
| M | ? | RUF030.py | 83 |
| M | ? | RUF030.py | 88 |
| M | ? | RUF030.py | 93 |
| M | ? | RUF030.py | 101 |
| M | ? | RUF030.py | 108 |
| M | ? | RUF028.py | 103 |
| M | ? | RUF069.py | 12 |
| M | ? | RUF069.py | 24 |
| M | ? | RUF069.py | 25 |
| M | ? | RUF069.py | 26 |
| M | ? | RUF069.py | 27 |
| M | ? | RUF069.py | 28 |
| M | ? | RUF069.py | 29 |
| M | ? | RUF069.py | 30 |
| M | ? | RUF069.py | 35 |
| M | ? | RUF069.py | 36 |
| M | ? | RUF069.py | 39 |
| M | ? | RUF069.py | 44 |
| M | ? | RUF069.py | 46 |
| M | ? | RUF069.py | 48 |
| M | ? | RUF069.py | 56 |
| M | ? | RUF069.py | 58 |
| M | ? | RUF069.py | 60 |
| M | ? | RUF069.py | 62 |
| M | ? | RUF069.py | 64 |
| M | ? | RUF069.py | 70 |
| M | ? | RUF069.py | 77 |
| M | ? | RUF069.py | 79 |
| M | ? | RUF069.py | 85 |
| M | ? | RUF069.py | 87 |
| M | ? | RUF059_0.py | 59 |
| M | ? | COM81.py | 189 |
| M | ? | COM81.py | 193 |
| M | ? | COM81.py | 646 |
| M | ? | C419.py | 68 |
| M | ? | F631.py | 1 |
| M | ? | F631.py | 2 |
| M | ? | F631.py | 3 |
| M | ? | F631.py | 4 |
| M | ? | F821_25.py | 5 |
| M | ? | F841_0.py | 59 |
| M | ? | nan_comparison.py | 98 |
| M | ? | nan_comparison.py | 99 |
| M | ? | len_as_condition.py | 73 |
| M | ? | len_as_condition.py | 90 |
| M | ? | len_as_condition.py | 93 |
| M | ? | len_as_condition.py | 96 |
| M | ? | len_as_condition.py | 99 |
| M | ? | len_as_condition.py | 102 |
| M | ? | len_as_condition.py | 122 |
| M | ? | len_as_condition.py | 123 |
| M | ? | len_as_condition.py | 124 |
| M | ? | len_as_condition.py | 125 |
| M | ? | len_as_condition.py | 126 |
| M | ? | len_as_condition.py | 127 |
| M | ? | len_as_condition.py | 129 |
| M | ? | len_as_condition.py | 130 |
| M | ? | len_as_condition.py | 171 |
| M | ? | len_as_condition.py | 172 |
| M | ? | len_as_condition.py | 175 |
| M | ? | len_as_condition.py | 176 |
| M | ? | len_as_condition.py | 177 |
| M | ? | unnecessary_dict_index_lookup.py | 11 |
| M | ? | unnecessary_dict_index_lookup.py | 18 |
| M | ? | unnecessary_dict_index_lookup.py | 23 |
| M | ? | unnecessary_dict_index_lookup.py | 29 |
| M | ? | unnecessary_dict_index_lookup.py | 40 |
| M | ? | unnecessary_dunder_call.py | 131 |
| M | ? | unnecessary_list_index_lookup.py | 14 |
| M | ? | unnecessary_list_index_lookup.py | 19 |
| M | ? | unnecessary_list_index_lookup.py | 27 |
| M | ? | unexpected_special_method_signature.py | 77 |
| M | ? | unexpected_special_method_signature.py | 80 |
| M | ? | unexpected_special_method_signature.py | 83 |
| M | ? | unexpected_special_method_signature.py | 86 |
| M | ? | unexpected_special_method_signature.py | 89 |
| M | ? | unexpected_special_method_signature.py | 92 |
| M | ? | unexpected_special_method_signature.py | 95 |
| M | ? | unexpected_special_method_signature.py | 98 |
| M | ? | unexpected_special_method_signature.py | 101 |
| M | ? | unexpected_special_method_signature.py | 104 |
| M | ? | unexpected_special_method_signature.py | 107 |
| M | ? | unexpected_special_method_signature.py | 110 |
| M | ? | assert_on_string_literal.py | 3 |
| M | ? | assert_on_string_literal.py | 8 |
| M | ? | assert_on_string_literal.py | 12 |
| M | ? | assert_on_string_literal.py | 14 |
| M | ? | assert_on_string_literal.py | 17 |
| M | ? | assert_on_string_literal.py | 18 |
| M | ? | assert_on_string_literal.py | 19 |
| M | ? | assert_on_string_literal.py | 20 |
| M | ? | assert_on_string_literal.py | 21 |
| M | ? | assert_on_string_literal.py | 22 |
| M | ? | assert_on_string_literal.py | 23 |
| M | ? | assert_on_string_literal.py | 24 |
| M | ? | assert_on_string_literal.py | 29 |
| M | ? | assert_on_string_literal.py | 30 |
| M | ? | assert_on_string_literal.py | 31 |
| M | ? | B015.py | 1 |
| M | ? | B015.py | 5 |
| M | ? | B015.py | 15 |
| M | ? | B009_B010.py | 58 |
| M | ? | B004.py | 45 |
| M | ? | B004.py | 46 |
| M | ? | B004.py | 53 |
| M | ? | B004.py | 54 |
| M | ? | B023.py | 70 |
| M | ? | B904.py | 15 |
| M | ? | B904.py | 92 |
| M | ? | B011.py | 7 |
| M | ? | B011.py | 8 |
| M | ? | B011.py | 9 |
| M | ? | B011.py | 10 |
| M | ? | PT018.py | 5 |
| M | ? | PT018.py | 6 |
| M | ? | PT018.py | 7 |
| M | ? | PT018.py | 8 |
| M | ? | PT018.py | 9 |
| M | ? | PT018.py | 10 |
| M | ? | PT018.py | 14 |
| M | ? | PT018.py | 15 |
| M | ? | PT018.py | 16 |
| M | ? | PT018.py | 17 |
| M | ? | PT018.py | 18 |
| M | ? | PT018.py | 19 |
| M | ? | PT018.py | 20 |
| M | ? | PT018.py | 21 |
| M | ? | PT015.py | 5 |
| M | ? | PT015.py | 9 |
| M | ? | PT015.py | 10 |
| M | ? | PT015.py | 11 |
| M | ? | PT015.py | 12 |
| M | ? | PT015.py | 13 |
| M | ? | PT015.py | 14 |
| M | ? | PT015.py | 15 |
| M | ? | PT015.py | 16 |
| M | ? | PT015.py | 17 |
| M | ? | PT015.py | 18 |
| M | ? | PT015.py | 19 |
| M | ? | PT015.py | 20 |
| M | ? | PT015.py | 21 |
| M | ? | PT015.py | 22 |
| M | ? | PT015.py | 23 |
| M | ? | PT015.py | 24 |
| M | ? | PT015.py | 25 |
| M | ? | PT015.py | 29 |
| M | ? | PT015.py | 30 |
| M | ? | PT015.py | 31 |
| M | ? | PT015.py | 32 |
| M | ? | PT015.py | 33 |
| M | ? | PT017.py | 12 |
| M | ? | PT017.py | 19 |
| M | ? | PT009.py | 6 |
| M | ? | PT012.py | 89 |
| M | ? | PT012.py | 97 |
| M | ? | PT031.py | 89 |
| M | ? | PT031.py | 97 |
| M | ? | assert.py | 1 |
| M | ? | assert.py | 2 |
| M | ? | assert.py | 3 |
| M | ? | assert.py | 4 |
| M | ? | assert.py | 5 |
| M | ? | assert.py | 6 |
| M | ? | assert.py | 8 |
| M | ? | assert.py | 9 |
| M | ? | assert.py | 10 |
| M | ? | assert.py | 11 |
| M | ? | assert_invalid_test_expr.py | 1 |
| M | ? | assert_invalid_test_expr.py | 2 |
| M | ? | assert_invalid_test_expr.py | 3 |
| M | ? | assert_invalid_test_expr.py | 4 |
| M | ? | assert_empty_msg.py | 1 |
| M | ? | assert_invalid_msg_expr.py | 1 |
| M | ? | assert_invalid_msg_expr.py | 2 |
| M | ? | assert_invalid_msg_expr.py | 3 |
| M | ? | assert_invalid_msg_expr.py | 4 |
| M | ? | memory_report.py | 503 |
| M | ? | check_ecosystem.py | 108 |
| M | ? | check_ecosystem.py | 259 |
| M | ? | check_ecosystem.py | 260 |
| M | ? | check_ecosystem.py | 311 |
| M | ? | check_ecosystem.py | 327 |
| M | ? | conformance.py | 483 |
| M | ? | conformance.py | 885 |
| M | ? | lsp_client.py | 124 |
| M | ? | tool.py | 21 |
| M | ? | tool.py | 69 |
| M | ? | setup_primer_project.py | 73 |
| M | ? | setup_primer_project.py | 138 |
| M | ? | update_ambiguous_characters.py | 66 |
| M | ? | main.py | 110 |
| M | ? | main.py | 111 |
| M | ? | fuzz.py | 205 |
| M | ? | fuzz.py | 437 |
| C | ? | S608.py | 3 |
| C | ? | S608.py | 4 |
| C | ? | S608.py | 9 |
| C | ? | S608.py | 10 |
| C | ? | S608.py | 15 |
| C | ? | S608.py | 20 |
| H | ? | DJ012.py | 103 |
| M | ? | preview_multiline_strings.py | 42 |
| M | ? | preview_multiline_strings.py | 46 |
| M | ? | S301.py | 3 |
| M | ? | S301.py | 7 |
| M | ? | S301.py | 8 |
| M | ? | S506.py | 10 |
| M | ? | S506.py | 13 |
| M | ? | S506.py | 16 |
| M | ? | S506.py | 24 |
| M | ? | S506.py | 27 |
| M | ? | S506.py | 28 |
| M | ? | S506.py | 29 |
| M | ? | S506.py | 30 |
| M | ? | S506.py | 31 |
| M | ? | S506.py | 32 |
| M | ? | S506.py | 33 |
| M | ? | S506.py | 34 |
| M | ? | S506.py | 35 |
| M | ? | S506.py | 36 |
| M | ? | S506.py | 37 |
| M | ? | S506.py | 38 |
| M | ? | S506.py | 41 |
| M | ? | S506.py | 42 |
| M | ? | S506.py | 43 |
| M | ? | S506.py | 44 |
| M | ? | S506.py | 46 |
| M | ? | S506.py | 48 |
| M | ? | S506.py | 50 |
| C | ? | S608.py | 6 |
| C | ? | S608.py | 12 |
| C | ? | S608.py | 17 |
| C | ? | S608.py | 22 |
| H | ? | S501.py | 5 |
| H | ? | S501.py | 7 |
| H | ? | S501.py | 9 |
| H | ? | S501.py | 11 |
| H | ? | S501.py | 13 |
| H | ? | S501.py | 15 |
| H | ? | S501.py | 17 |
| H | ? | S501.py | 19 |
| H | ? | S501.py | 22 |
| H | ? | S501.py | 24 |
| H | ? | S501.py | 26 |
| H | ? | S501.py | 28 |
| H | ? | S501.py | 30 |
| H | ? | S501.py | 32 |
| H | ? | S501.py | 34 |
| H | ? | S501.py | 36 |
| H | ? | S501.py | 38 |
| H | ? | S501.py | 40 |
| H | ? | S501.py | 42 |
| H | ? | preview_long_strings.py | 213 |
| H | ? | long_strings_flag_disabled.py | 268 |
| H | ? | E402_4.py | 5 |
| H | ? | S202.py | 51 |
| H | ? | S202.py | 54 |
| H | ? | py_path_1.py | 3 |
| H | ? | tool.py | 66 |
| H | ? | update_schemastore.py | 102 |
| M | ? | S105.py | 7 |
| M | ? | S105.py | 13 |
| M | ? | S105.py | 18 |
| M | ? | S105.py | 20 |
| M | ? | S105.py | 39 |
| M | ? | S105.py | 43 |
| M | ? | S105.py | 48 |
| M | ? | S107.py | 5 |
| M | ? | S107.py | 13 |
| M | ? | S107.py | 21 |
| M | ? | S107.py | 29 |
| M | ? | S107.py | 33 |
| M | ? | S106.py | 10 |
| M | ? | S106.py | 14 |
| M | ? | magic_value_comparison.py | 66 |
| C | ? | S605.py | 8 |
| C | ? | S605.py | 26 |
| C | ? | S605.py | 27 |
| C | ? | S605.py | 28 |
| C | ? | S609.py | 5 |
| C | ? | S609.py | 6 |
| C | ? | S609.py | 8 |
| C | ? | S607.py | 9 |
| C | ? | S607.py | 40 |
| C | ? | S607.py | 41 |
| C | ? | S607.py | 42 |
| C | ? | S607.py | 43 |
| C | ? | S607.py | 44 |
| C | ? | subprocess_run_without_check.py | 5 |
| C | ? | subprocess_run_without_check.py | 15 |
| C | ? | subprocess_run_without_check.py | 16 |
| C | ? | ASYNC22x.py | 32 |
| C | ? | ASYNC22x.py | 35 |
| C | ? | setup_primer_project.py | 142 |
| M | ? | E22.py | 146 |
| M | ? | S105.py | 7 |
| M | ? | S105.py | 13 |
| M | ? | S105.py | 17 |
| M | ? | S105.py | 18 |
| M | ? | S105.py | 20 |
| M | ? | S105.py | 39 |
| M | ? | S105.py | 43 |
| M | ? | S105.py | 47 |
| M | ? | S105.py | 48 |
| M | ? | S107.py | 5 |
| M | ? | S107.py | 13 |
| M | ? | S107.py | 21 |
| M | ? | S107.py | 29 |
| M | ? | S107.py | 33 |
| M | ? | S106.py | 10 |
| M | ? | S106.py | 14 |
| M | ? | RUF056.py | 87 |
| M | ? | RUF056.py | 88 |
| M | ? | RUF056.py | 167 |
| M | ? | RUF056.py | 168 |
| M | ? | RUF056.py | 170 |
| M | ? | RUF056.py | 171 |
| M | ? | RUF056.py | 176 |
| M | ? | RUF056.py | 181 |
| M | ? | RUF024.py | 37 |
| M | ? | F523.py | 37 |
| M | ? | invalid_envvar_value.py | 6 |
| M | ? | invalid_envvar_value.py | 9 |
| M | ? | invalid_envvar_value.py | 11 |
| M | ? | magic_value_comparison.py | 66 |
| M | ? | AIR201.py | 79 |
| M | ? | AIR201.py | 85 |
| M | ? | AIR201.py | 91 |
| M | ? | AIR201.py | 97 |
| M | ? | AIR201.py | 150 |
| M | ? | AIR201.py | 180 |
| M | ? | AIR201.py | 186 |
| M | ? | AIR301_args.py | 115 |
| M | ? | AIR301_args.py | 118 |
| M | ? | AIR301_args.py | 335 |
| M | ? | AIR301_args.py | 336 |
| M | ? | AIR301_args.py | 344 |
| M | ? | AIR301_args.py | 345 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 8 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 11 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 18 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 21 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 22 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 28 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 30 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 32 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 40 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 41 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 50 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 51 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 61 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 66 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 76 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 85 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 88 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 95 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 98 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 99 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 105 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 107 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 109 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 117 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 118 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 127 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 128 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 137 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 244 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 252 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 255 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 261 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 264 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 265 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 271 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 273 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 275 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 283 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 284 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 293 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 294 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S105_S105.py.snap | 304 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S106_S106.py.snap | 8 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 7 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 15 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 23 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 31 |
| C | GS001 | ruff_linter__rules__flake8_bandit__tests__S107_S107.py.snap | 39 |
| L | GS003 | generate.py | 48 |
| L | GS003 | starred_starred_expression.py | 1 |
| L | GS003 | starred_starred_expression.py | 3 |
| L | GS003 | match.py | 174 |
| L | GS003 | match.py | 179 |
| L | GS003 | match.py | 340 |
| L | GS003 | try.py | 60 |
| L | GS003 | try.py | 62 |
| L | GS003 | try.py | 67 |
| L | GS003 | try.py | 69 |
| L | GS003 | type.py | 70 |
| L | GS003 | while.py | 11 |
| L | GS003 | while.py | 14 |
| L | GS003 | main.py | 2 |
| L | GS003 | main.py | 2 |
| L | GS003 | mdtest.py | 100 |
| L | GS003 | mdtest.py | 228 |
| L | GS003 | mdtest.py | 361 |
| L | GS003 | 93_deadcode.py | 3 |
| L | GS003 | 95_annotation_global.py | 3 |
| L | GS003 | 95_annotation_global_simple.py | 3 |
| L | GS003 | 96_debug.py | 2 |
| L | GS003 | fuzz.py | 147 |
| L | GS003 | fuzz.py | 162 |
| L | GS003 | fuzz.py | 164 |
| L | GS003 | fuzz.py | 165 |
| L | GS003 | fuzz.py | 166 |
| L | GS003 | fuzz.py | 225 |
| L | GS003 | fuzz.py | 245 |
| L | GS003 | fuzz.py | 246 |
| L | GS003 | fuzz.py | 254 |
| L | GS003 | fuzz.py | 276 |
| L | GS003 | fuzz.py | 277 |
| L | GS003 | fuzz.py | 280 |
| L | GS003 | fuzz.py | 408 |
| L | GS003 | fuzz.py | 416 |
| L | GS003 | fuzz.py | 434 |
| L | GS003 | cli.py | 29 |
| L | GS003 | cli.py | 53 |
| L | GS003 | cli.py | 68 |
| L | GS003 | cli.py | 25 |
| L | GS003 | main.py | 88 |
| L | GS003 | main.py | 92 |
| L | GS003 | main.py | 94 |
| L | GS003 | check_docs_formatted.py | 212 |
| L | GS003 | check_docs_formatted.py | 217 |
| L | GS003 | check_docs_formatted.py | 231 |
| L | GS003 | check_docs_formatted.py | 240 |
| L | GS003 | check_docs_formatted.py | 251 |
| L | GS003 | check_docs_formatted.py | 253 |
| L | GS003 | check_docs_formatted.py | 303 |
| L | GS003 | check_docs_formatted.py | 312 |
| L | GS003 | check_docs_formatted.py | 323 |
| L | GS003 | check_docs_formatted.py | 331 |
| L | GS003 | check_docs_formatted.py | 332 |
| L | GS003 | check_docs_formatted.py | 333 |
| L | GS003 | check_docs_formatted.py | 344 |
| L | GS003 | check_docs_formatted.py | 364 |
| L | GS003 | check_docs_formatted.py | 367 |
| L | GS003 | check_docs_formatted.py | 370 |
| L | GS003 | check_docs_formatted.py | 371 |
| L | GS003 | check_docs_formatted.py | 372 |
| L | GS003 | check_docs_formatted.py | 375 |
| L | GS003 | check_docs_formatted.py | 376 |
| L | GS003 | check_docs_formatted.py | 377 |
| L | GS003 | check_docs_formatted.py | 378 |
| L | GS003 | check_docs_formatted.py | 379 |
| L | GS003 | check_docs_formatted.py | 380 |
| L | GS003 | check_docs_formatted.py | 381 |
| L | GS003 | check_docs_formatted.py | 383 |
| L | GS003 | check_docs_formatted.py | 386 |
| L | GS003 | check_docs_formatted.py | 387 |
| L | GS003 | check_docs_formatted.py | 391 |
| L | GS003 | check_ecosystem.py | 393 |
| L | GS003 | check_ecosystem.py | 397 |
| L | GS003 | check_ecosystem.py | 399 |
| L | GS003 | check_ecosystem.py | 404 |
| L | GS003 | check_ecosystem.py | 406 |
| L | GS003 | check_ecosystem.py | 410 |
| L | GS003 | check_ecosystem.py | 411 |
| L | GS003 | check_ecosystem.py | 412 |
| L | GS003 | check_ecosystem.py | 414 |
| L | GS003 | check_ecosystem.py | 415 |
| L | GS003 | check_ecosystem.py | 416 |
| L | GS003 | check_ecosystem.py | 418 |
| L | GS003 | check_ecosystem.py | 419 |
| L | GS003 | check_ecosystem.py | 422 |
| L | GS003 | check_ecosystem.py | 423 |
| L | GS003 | check_ecosystem.py | 424 |
| L | GS003 | check_ecosystem.py | 428 |
| L | GS003 | check_ecosystem.py | 433 |
| L | GS003 | check_ecosystem.py | 438 |
| L | GS003 | check_ecosystem.py | 439 |
| L | GS003 | check_ecosystem.py | 440 |
| L | GS003 | check_ecosystem.py | 442 |
| L | GS003 | check_ecosystem.py | 443 |
| L | GS003 | check_ecosystem.py | 474 |
| L | GS003 | check_ecosystem.py | 475 |
| L | GS003 | check_ecosystem.py | 476 |
| L | GS003 | check_ecosystem.py | 477 |
| L | GS003 | check_ecosystem.py | 483 |
| L | GS003 | collect_ty_ecosystem_run_metadata.py | 355 |
| L | GS003 | collect_ty_ecosystem_run_metadata.py | 359 |
| L | GS003 | conformance.py | 1112 |
| L | GS003 | conformance.py | 1113 |
| L | GS003 | conformance.py | 1115 |
| L | GS003 | ecosystem_all_check.py | 76 |
| L | GS003 | generate-crate-readmes.py | 157 |
| L | GS003 | generate-crate-readmes.py | 184 |
| L | GS003 | generate_builtin_modules.py | 29 |
| L | GS003 | generate_builtin_modules.py | 30 |
| L | GS003 | generate_builtin_modules.py | 58 |
| L | GS003 | generate_builtin_modules.py | 87 |
| L | GS003 | generate_builtin_modules.py | 91 |
| L | GS003 | generate_builtin_modules.py | 92 |
| L | GS003 | generate_builtin_modules.py | 93 |
| L | GS003 | generate_builtin_modules.py | 101 |
| L | GS003 | generate_builtin_modules.py | 103 |
| L | GS003 | generate_builtin_modules.py | 106 |
| L | GS003 | generate_builtin_modules.py | 107 |
| L | GS003 | generate_builtin_modules.py | 108 |
| L | GS003 | generate_builtin_modules.py | 109 |
| L | GS003 | memory_report.py | 258 |
| L | GS003 | memory_report.py | 260 |
| L | GS003 | memory_report.py | 280 |
| L | GS003 | memory_report.py | 340 |
| L | GS003 | memory_report.py | 355 |
| L | GS003 | memory_report.py | 365 |
| L | GS003 | memory_report.py | 366 |
| L | GS003 | memory_report.py | 368 |
| L | GS003 | memory_report.py | 378 |
| L | GS003 | memory_report.py | 380 |
| L | GS003 | memory_report.py | 381 |
| L | GS003 | memory_report.py | 410 |
| L | GS003 | memory_report.py | 411 |
| L | GS003 | memory_report.py | 413 |
| L | GS003 | publish-crates.py | 105 |
| L | GS003 | publish-crates.py | 128 |
| L | GS003 | publish-crates.py | 130 |
| L | GS003 | publish-crates.py | 133 |
| L | GS003 | setup-crates-io-publish.py | 186 |
| L | GS003 | setup-crates-io-publish.py | 250 |
| L | GS003 | setup-crates-io-publish.py | 256 |
| L | GS003 | setup-crates-io-publish.py | 263 |
| L | GS003 | setup-crates-io-publish.py | 268 |
| L | GS003 | setup-crates-io-publish.py | 305 |
| L | GS003 | setup-crates-io-publish.py | 313 |
| L | GS003 | setup-crates-io-publish.py | 317 |
| L | GS003 | setup-crates-io-publish.py | 322 |
| L | GS003 | setup-crates-io-publish.py | 336 |
| L | GS003 | setup-crates-io-publish.py | 356 |
| L | GS003 | setup-crates-io-publish.py | 384 |
| L | GS003 | setup-crates-io-publish.py | 386 |
| L | GS003 | setup-crates-io-publish.py | 391 |
| L | GS003 | setup-crates-io-publish.py | 399 |
| L | GS003 | setup-crates-io-publish.py | 401 |
| L | GS003 | setup-crates-io-publish.py | 404 |
| L | GS003 | setup-crates-io-publish.py | 413 |
| L | GS003 | setup-crates-io-publish.py | 421 |
| L | GS003 | setup-crates-io-publish.py | 428 |
| L | GS003 | setup-crates-io-publish.py | 431 |
| L | GS003 | setup-crates-io-publish.py | 438 |
| L | GS003 | setup-crates-io-publish.py | 450 |
| L | GS003 | setup_primer_project.py | 47 |
| L | GS003 | setup_primer_project.py | 48 |
| L | GS003 | setup_primer_project.py | 50 |
| L | GS003 | setup_primer_project.py | 111 |
| L | GS003 | setup_primer_project.py | 115 |
| L | GS003 | setup_primer_project.py | 125 |
| L | GS003 | setup_primer_project.py | 140 |
| L | GS003 | setup_primer_project.py | 147 |
| L | GS003 | setup_primer_project.py | 149 |
| L | GS003 | setup_primer_project.py | 151 |
| L | GS003 | setup_primer_project.py | 152 |
| L | GS003 | setup_primer_project.py | 153 |
| L | GS003 | setup_primer_project.py | 155 |
| L | GS003 | run.py | 143 |
| L | GS003 | run.py | 168 |
| L | GS003 | run.py | 169 |
| L | GS003 | run.py | 172 |
| L | GS003 | run.py | 173 |
| L | GS003 | run.py | 175 |
| L | GS003 | run.py | 176 |
| L | GS003 | snapshot.py | 97 |
| L | GS003 | snapshot.py | 98 |
| L | GS003 | snapshot.py | 99 |
| L | GS003 | snapshot.py | 100 |
| L | GS003 | snapshot.py | 101 |
| L | GS003 | snapshot.py | 115 |
| L | GS003 | snapshot.py | 117 |
| L | GS003 | snapshot.py | 119 |
| L | GS003 | snapshot.py | 121 |
| L | GS003 | snapshot.py | 122 |
| L | GS003 | snapshot.py | 126 |
| L | GS003 | snapshot.py | 129 |
| L | GS003 | snapshot.py | 132 |
| L | GS003 | snapshot.py | 136 |
| L | GS003 | update_ambiguous_characters.py | 86 |
| L | GS003 | update_ambiguous_characters.py | 93 |
| L | GS003 | update_ambiguous_characters.py | 98 |
| L | GS003 | update_ambiguous_characters.py | 100 |
| L | GS003 | update_schemastore.py | 138 |
| L | GS003 | lib.rs | 213 |
| L | GS003 | lib.rs | 238 |
| L | GS003 | build.rs | 17 |
| L | GS003 | build.rs | 28 |
| L | GS003 | build.rs | 41 |
| L | GS003 | build.rs | 60 |
| L | GS003 | build.rs | 61 |
| L | GS003 | build.rs | 62 |
| L | GS003 | build.rs | 68 |
| L | GS003 | build.rs | 73 |
| L | GS003 | config.rs | 15 |
| L | GS003 | config.rs | 19 |
| L | GS003 | config.rs | 33 |
| L | GS003 | lib.rs | 147 |
| L | GS003 | lib.rs | 366 |
| L | GS003 | generate_cli_help.rs | 100 |
| L | GS003 | generate_docs.rs | 150 |
| L | GS003 | generate_docs.rs | 190 |
| L | GS003 | generate_docs.rs | 219 |
| L | GS003 | generate_json_schema.rs | 29 |
| L | GS003 | generate_json_schema.rs | 34 |
| L | GS003 | generate_json_schema.rs | 43 |
| L | GS003 | generate_json_schema.rs | 45 |
| L | GS003 | generate_ty_cli_reference.rs | 30 |
| L | GS003 | generate_ty_cli_reference.rs | 35 |
| L | GS003 | generate_ty_cli_reference.rs | 53 |
| L | GS003 | generate_ty_cli_reference.rs | 55 |
| L | GS003 | generate_ty_cli_reference.rs | 60 |
| L | GS003 | generate_ty_env_vars_reference.rs | 35 |
| L | GS003 | generate_ty_env_vars_reference.rs | 40 |
| L | GS003 | generate_ty_env_vars_reference.rs | 68 |
| L | GS003 | generate_ty_env_vars_reference.rs | 70 |
| L | GS003 | generate_ty_env_vars_reference.rs | 75 |
| L | GS003 | generate_ty_options.rs | 42 |
| L | GS003 | generate_ty_options.rs | 47 |
| L | GS003 | generate_ty_options.rs | 56 |
| L | GS003 | generate_ty_options.rs | 58 |
| L | GS003 | generate_ty_rules.rs | 30 |
| L | GS003 | generate_ty_rules.rs | 35 |
| L | GS003 | generate_ty_rules.rs | 44 |
| L | GS003 | generate_ty_rules.rs | 46 |
| L | GS003 | generate_ty_schema.rs | 29 |
| L | GS003 | generate_ty_schema.rs | 34 |
| L | GS003 | generate_ty_schema.rs | 43 |
| L | GS003 | generate_ty_schema.rs | 45 |
| L | GS003 | main.rs | 100 |
| L | GS003 | main.rs | 102 |
| L | GS003 | print_ast.rs | 29 |
| L | GS003 | print_cst.rs | 19 |
| L | GS003 | print_tokens.rs | 29 |
| L | GS003 | round_trip.rs | 21 |
| L | GS003 | round_trip.rs | 24 |
| L | GS003 | macros.rs | 106 |
| L | GS003 | linter.rs | 686 |
| L | GS003 | linter.rs | 696 |
| L | GS003 | linter.rs | 724 |
| L | GS003 | linter.rs | 734 |
| L | GS003 | logging.rs | 86 |
| L | GS003 | cli.rs | 77 |
| L | GS003 | cli.rs | 83 |
| L | GS003 | cli.rs | 86 |
| L | GS003 | cli.rs | 102 |
| L | GS003 | logging.rs | 39 |
| L | GS003 | build.rs | 31 |
| L | GS003 | build.rs | 41 |
| L | GS003 | build.rs | 49 |
| L | GS003 | build.rs | 62 |
| L | GS003 | build.rs | 75 |
| L | GS003 | build.rs | 95 |
| L | GS003 | build.rs | 96 |
| L | GS003 | build.rs | 97 |
| L | GS003 | build.rs | 105 |
| L | GS003 | build.rs | 111 |
| L | GS003 | main.rs | 106 |
| L | GS003 | main.rs | 115 |
| L | GS003 | docstring.rs | 1023 |
| L | GS003 | docstring.rs | 1035 |
| L | GS003 | docstring.rs | 1069 |
| L | GS003 | docstring.rs | 1081 |
| L | GS003 | property_tests.rs | 51 |
| L | GS003 | property_tests.rs | 52 |
| L | GS003 | property_tests.rs | 68 |
| L | GS003 | property_tests.rs | 69 |
| L | GS003 | logging.rs | 41 |
| L | GS003 | build.rs | 69 |
| L | GS003 | build.rs | 81 |
| L | GS003 | build.rs | 88 |
| L | GS003 | build.rs | 26 |
| L | GS003 | build.rs | 39 |
| L | GS003 | build.rs | 62 |
| L | GS008 | _re.py | 19 |
| L | GS008 | sub2.py | 1 |
| L | GS008 | 03_dict_literal_large.py | 1 |
| L | GS008 | check.py | 54 |
| L | GS008 | defaults.py | 15 |
| L | GS008 | main.py | 23 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| H | ? | split_empty_brackets.py | 77 |
| H | ? | split_empty_brackets.py | 81 |
| H | ? | split_empty_brackets.py | 85 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 8 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 10 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 11 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 18 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 19 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 21 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 27 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 28 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 29 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 37 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 45 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 54 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 64 |
| H | ? | ruff_linter__rules__flake8_bandit__tests__S104_S104.py.snap | 74 |
| H | ? | hardcoded_bind_all_interfaces.rs | 44 |
| H | ? | hardcoded_bind_all_interfaces.rs | 52 |
| H | ? | hardcoded_bind_all_interfaces.rs | 58 |
| H | ? | S104.py | 9 |
| H | ? | S104.py | 10 |
| H | ? | S104.py | 11 |
| H | ? | S104.py | 15 |
| H | ? | S104.py | 19 |
| H | ? | S104.py | 24 |
| H | ? | S104.py | 27 |
| H | ? | S104.py | 28 |
| H | ? | S104.py | 29 |
| H | ? | v1.json | 4 |
| H | ? | v0.json | 4 |
| H | ? | projects.py | 363 |
| H | ? | projects.py | 364 |
| H | ? | projects.py | 371 |
| H | ? | projects.py | 372 |
| H | ? | Icons.tsx | 225 |
| H | ? | Icons.tsx | 229 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 12 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 21 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 22 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 25 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 29 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 30 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 33 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 39 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 40 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 43 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 47 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 50 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 52 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 58 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 61 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 65 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 69 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 74 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 80 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 84 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 88 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 91 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 96 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 102 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 106 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 113 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 116 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 165 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 169 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 175 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 178 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 179 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 181 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 187 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 188 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 189 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 198 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 203 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 211 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__S103_S103.py.snap | 214 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 13 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 18 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 20 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 29 |
| C | ? | ruff_linter__rules__flake8_bandit__tests__preview__S103_S103.py.snap | 33 |
| C | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1008 |
| C | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1009 |
| C | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1018 |
| C | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1019 |
| C | ? | ruff_linter__rules__flake8_use_pathlib__tests__preview_full_name.py.snap | 1020 |
| C | ? | ruff_linter__rules__flake8_use_pathlib__tests__full_name.py.snap | 635 |
| C | ? | ruff_linter__rules__flake8_use_pathlib__tests__full_name.py.snap | 636 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 9 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 11 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 12 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 19 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 20 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 21 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 28 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 29 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 30 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 41 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 42 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 53 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 107 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 109 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 116 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 117 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 118 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 125 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 227 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 229 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 236 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 237 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 238 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 246 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 248 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 255 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 256 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 257 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 264 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 326 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 328 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 335 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 337 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 344 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 345 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 354 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 355 |
| C | ? | ruff_linter__rules__ruff__tests__RUF064_RUF064.py.snap | 356 |
| C | ? | S103.py | 8 |
| C | ? | S103.py | 9 |
| C | ? | S103.py | 11 |
| C | ? | S103.py | 14 |
| C | ? | S103.py | 17 |
| C | ? | S103.py | 31 |
| C | ? | S103.py | 36 |
| C | ? | S103.py | 37 |
| C | ? | S103.py | 38 |
| C | ? | S103.py | 42 |
| C | ? | S103.py | 44 |
| C | ? | full_name.py | 186 |
| C | ? | full_name.py | 187 |
| C | ? | RUF064.py | 6 |
| C | ? | RUF064.py | 7 |
| C | ? | RUF064.py | 8 |
| C | ? | RUF064.py | 18 |
| C | ? | RUF064.py | 19 |
| C | ? | RUF064.py | 36 |
| C | ? | RUF064.py | 37 |
| C | ? | RUF064.py | 40 |
| C | ? | RUF064.py | 41 |
| C | ? | RUF064.py | 52 |
| C | ? | RUF064.py | 53 |
| C | ? | ruff_linter__rules__pylint__tests__PLE1507_invalid_envvar_value.py.snap | 19 |
| C | ? | ruff_linter__rules__pylint__tests__PLE1507_invalid_envvar_value.py.snap | 29 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 189 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 196 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 207 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 214 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 225 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 232 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 243 |
| C | ? | ruff_linter__rules__airflow__tests__AIR201_AIR201.py.snap | 250 |
| C | ? | xcom_pull_in_template_string.rs | 451 |
| C | ? | xcom_pull_in_template_string.rs | 460 |
| C | ? | xcom_pull_in_template_string.rs | 470 |
| C | ? | xcom_pull_in_template_string.rs | 479 |
| C | ? | xcom_pull_in_template_string.rs | 487 |
| C | ? | xcom_pull_in_template_string.rs | 511 |
| C | ? | xcom_pull_in_template_string.rs | 520 |
| C | ? | xcom_pull_in_template_string.rs | 529 |
| C | ? | magic_value_comparison.py | 66 |
| C | ? | AIR201.py | 79 |
| C | ? | AIR201.py | 85 |
| C | ? | AIR201.py | 91 |
| C | ? | AIR201.py | 97 |
| C | ? | AIR201.py | 180 |
| C | ? | AIR201.py | 186 |
| C | ? | AIR301_args.py | 335 |
| C | ? | AIR301_args.py | 336 |
| C | ? | AIR301_args.py | 344 |
| C | ? | AIR301_args.py | 345 |
| M | ? | FURB103_0.py | 158 |
| M | ? | check_ecosystem.py | 308 |
| M | ? | check_ecosystem.py | 329 |
| M | ? | ecosystem_all_check.py | 41 |
| M | ? | projects.py | 139 |
| M | ? | projects.py | 163 |
| M | ? | projects.py | 219 |
| M | ? | projects.py | 266 |
| M | ? | projects.py | 286 |
| M | ? | collect_ty_ecosystem_run_metadata.py | 289 |
| M | ? | projects.py | 100 |
| C | ? | FAST002_1.py | 20 |
| C | ? | FAST002_2.py | 54 |
| H | ? | function.py | 17 |
| H | ? | fmtonoff.py | 26 |
| H | ? | S102.py | 3 |
| H | ? | S102.py | 5 |
| H | ? | S102.py | 11 |
| H | ? | S102.py | 15 |
| H | ? | S307.py | 3 |
| H | ? | S307.py | 4 |
| H | ? | S307.py | 8 |
| H | ? | S307.py | 12 |
| H | ? | RUF028.py | 103 |
| H | ? | B007.py | 47 |
| H | ? | decorator_expression_eval_hack_py38.py | 2 |
| H | ? | generate_builtin_modules.py | 52 |
| C | ? | S301.py | 3 |
| H | ? | setupMonaco.tsx | 296 |
| H | ? | setupMonaco.tsx | 315 |
| H | ? | setupMonaco.tsx | 319 |
| H | ? | setupMonaco.tsx | 577 |
| H | ? | setupMonaco.tsx | 585 |
| H | ? | setupMonaco.tsx | 593 |
| H | ? | setupMonaco.tsx | 601 |
| H | ? | setupMonaco.tsx | 605 |
| H | ? | setupMonaco.tsx | 612 |
| H | ? | setupMonaco.tsx | 616 |
| H | ? | ty.schema.json | 0 |
| H | ? | ruff.schema.json | 0 |
| H | ? | .markdownlint.yaml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | mkdocs.template.yml | 0 |
| H | ? | mkdocs.yml | 0 |
| H | GS004 | check.py | 552 |
| H | GS004 | format.py | 256 |
| H | GS004 | check_ecosystem.py | 197 |
| H | GS004 | setup_primer_project.py | 142 |
| s | GS009 |  | 0 |
| M | ? | mdtest.py | 139 |
| M | ? | ruff_linter__rules__flake8_bandit__tests__S607_S607.py.snap | 8 |
| M | ? | ruff_linter__rules__flake8_bandit__tests__S607_S607.py.snap | 18 |
| M | ? | ruff_linter__rules__flake8_bandit__tests__S607_S607.py.snap | 250 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 12 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 28 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 31 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 36 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 37 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 45 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 47 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 50 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 55 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 56 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 64 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 66 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 72 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 76 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 88 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 94 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 98 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 110 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 139 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 150 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 168 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 174 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 183 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 189 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP022.py.snap | 198 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 8 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 10 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 16 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 17 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 18 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 25 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 26 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 32 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 33 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 34 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 41 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 42 |
| M | ? | ruff_linter__rules__pyupgrade__tests__UP021.py.snap | 50 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 4 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 8 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 10 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 11 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 16 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 17 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 18 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 22 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 26 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 27 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 29 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 34 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 35 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 36 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 37 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 41 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 44 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 45 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 46 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 60 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 65 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 73 |
| M | ? | ruff_linter__rules__pylint__tests__PLW1510_subprocess_run_without_check.py.snap | 74 |
| M | ? | subprocess_run_without_check.rs | 62 |
| M | ? | ruff_linter__rules__flake8_async__tests__ASYNC221_ASYNC22x.py.snap | 8 |
| M | ? | ruff_linter__rules__flake8_async__tests__ASYNC221_ASYNC22x.py.snap | 47 |
| M | ? | ruff_linter__rules__flake8_async__tests__ASYNC221_ASYNC22x.py.snap | 56 |
| M | ? | ruff_linter__rules__flake8_async__tests__ASYNC221_ASYNC22x.py.snap | 66 |
| M | ? | S607.py | 8 |
| M | ? | S607.py | 49 |
| M | ? | UP022.py | 6 |
| M | ? | UP022.py | 8 |
| M | ? | UP022.py | 10 |
| M | ? | UP022.py | 14 |
| M | ? | UP022.py | 18 |
| M | ? | UP022.py | 29 |
| M | ? | UP022.py | 38 |
| M | ? | UP022.py | 42 |
| M | ? | UP022.py | 46 |
| M | ? | UP022.py | 52 |
| M | ? | UP021.py | 5 |
| M | ? | UP021.py | 6 |
| M | ? | UP021.py | 10 |
| M | ? | subprocess_run_without_check.py | 4 |
| M | ? | subprocess_run_without_check.py | 5 |
| M | ? | subprocess_run_without_check.py | 6 |
| M | ? | subprocess_run_without_check.py | 10 |
| M | ? | subprocess_run_without_check.py | 13 |
| M | ? | subprocess_run_without_check.py | 14 |
| M | ? | subprocess_run_without_check.py | 15 |
| M | ? | subprocess_run_without_check.py | 16 |
| M | ? | subprocess_run_without_check.py | 17 |
| M | ? | subprocess_run_without_check.py | 18 |
| M | ? | ASYNC22x.py | 8 |
| M | ? | ASYNC22x.py | 38 |
| M | ? | memory_report.py | 262 |
| M | ? | memory_report.py | 282 |
| M | ? | generate_builtin_modules.py | 22 |
| M | ? | generate_builtin_modules.py | 112 |
| M | ? | setup-crates-io-publish.py | 60 |
| M | ? | setup-crates-io-publish.py | 174 |
| M | ? | ecosystem_all_check.py | 61 |
| M | ? | bump-workspace-crate-versions.py | 56 |
| M | ? | conformance.py | 497 |
| M | ? | projects.py | 47 |
| M | ? | projects.py | 60 |
| M | ? | projects.py | 69 |
| M | ? | projects.py | 86 |
| M | ? | venv.py | 52 |
| M | ? | venv.py | 93 |
| M | ? | snapshot.py | 70 |
| M | ? | snapshot.py | 80 |
| M | ? | collect_ty_ecosystem_run_metadata.py | 36 |
| M | ? | check_docs_formatted.py | 149 |
| M | ? | generate-crate-readmes.py | 80 |
| M | ? | generate-crate-readmes.py | 188 |
| M | ? | publish-crates.py | 45 |
| M | ? | publish-crates.py | 136 |
| M | ? | setup_primer_project.py | 112 |
| M | ? | setup_primer_project.py | 116 |
| M | ? | setup_primer_project.py | 117 |
| M | ? | setup_primer_project.py | 126 |
| M | ? | setup_primer_project.py | 142 |
| M | ? | setup_primer_project.py | 148 |
| M | ? | generate_mkdocs.py | 177 |
| M | ? | add_rule.py | 158 |
| M | ? | fuzz.py | 59 |
| M | ? | fuzz.py | 77 |
| M | ? | fuzz.py | 386 |
| M | ? | fuzz.py | 396 |
| M | ? | fuzz.py | 432 |
| M | ? | __main__.py | 17 |
| H | ? | version.rs | 77 |
| H | ? | lib.rs | 129 |
| H | ? | lib.rs | 157 |
| H | ? | lib.rs | 299 |
| H | ? | lib.rs | 314 |
| H | ? | lib.rs | 342 |
| H | ? | lib.rs | 343 |
| H | ? | lib.rs | 349 |
| H | ? | lib.rs | 521 |
| H | ? | lib.rs | 163 |
| H | ? | lib.rs | 723 |
| H | ? | lib.rs | 735 |
| H | ? | lib.rs | 763 |
| H | ? | lib.rs | 806 |
| H | ? | lib.rs | 1579 |
| H | ? | lib.rs | 2023 |
| H | ? | lib.rs | 2331 |
| H | ? | lib.rs | 2408 |
| H | ? | lib.rs | 2445 |
| H | ? | lib.rs | 2529 |
| H | ? | lib.rs | 3059 |
| H | ? | lib.rs | 122 |
| H | ? | generate_ty_cli_reference.rs | 122 |
| H | ? | generate_rules_table.rs | 225 |
| H | ? | generate_ty_options.rs | 109 |
| H | ? | main.rs | 117 |
| H | ? | generate_options.rs | 65 |
| H | ? | format_dev.rs | 582 |
| H | ? | format_dev.rs | 821 |
| H | ? | panic.rs | 204 |
| H | ? | vendored.rs | 187 |
| H | ? | source.rs | 22 |
| H | ? | source.rs | 109 |
| H | ? | source.rs | 120 |
| H | ? | mod.rs | 294 |
| H | ? | mod.rs | 1201 |
| H | ? | mod.rs | 1811 |
| H | ? | render.rs | 467 |
| H | ? | render.rs | 2599 |
| H | ? | render.rs | 2608 |
| H | ? | render.rs | 2614 |
| H | ? | render.rs | 2624 |
| H | ? | render.rs | 2630 |
| H | ? | render.rs | 2636 |
| H | ? | render.rs | 2642 |
| H | ? | render.rs | 2648 |
| H | ? | parsed.rs | 141 |
| H | ? | parsed.rs | 147 |
| H | ? | cancellation.rs | 31 |
| H | ? | files.rs | 134 |
| H | ? | files.rs | 481 |
| H | ? | files.rs | 807 |
| H | ? | file_root.rs | 86 |
| H | ? | test.rs | 34 |
| H | ? | test.rs | 35 |
| H | ? | test.rs | 170 |
| H | ? | test.rs | 179 |
| H | ? | test.rs | 203 |
| H | ? | test.rs | 391 |
| H | ? | test.rs | 426 |
| H | ? | test.rs | 444 |
| H | ? | ignore.rs | 177 |
| H | ? | ignore.rs | 190 |
| H | ? | memory_fs.rs | 57 |
| H | ? | memory_fs.rs | 273 |
| H | ? | memory_fs.rs | 344 |
| H | ? | memory_fs.rs | 352 |
| H | ? | memory_fs.rs | 388 |
| H | ? | memory_fs.rs | 488 |
| H | ? | memory_fs.rs | 596 |
| H | ? | memory_fs.rs | 705 |
| H | ? | os.rs | 222 |
| H | ? | os.rs | 240 |
| H | ? | os.rs | 454 |
| H | ? | os.rs | 464 |
| H | ? | lib.rs | 140 |
| H | ? | parallel.rs | 61 |
| H | ? | metadata.rs | 84 |
| H | ? | metadata.rs | 87 |
| H | ? | metadata.rs | 188 |
| H | ? | metadata.rs | 207 |
| H | ? | metadata.rs | 427 |
| H | ? | options.rs | 116 |
| H | ? | options.rs | 117 |
| H | ? | options.rs | 197 |
| H | ? | options.rs | 565 |
| H | ? | options.rs | 671 |
| H | ? | options.rs | 672 |
| H | ? | options.rs | 2020 |
| H | ? | options.rs | 2029 |
| H | ? | options.rs | 2037 |
| H | ? | options.rs | 2038 |
| H | ? | options.rs | 2145 |
| H | ? | options.rs | 2167 |
| H | ? | options.rs | 2287 |
| H | ? | options.rs | 2292 |
| H | ? | settings.rs | 50 |
| H | ? | settings.rs | 218 |
| H | ? | settings.rs | 221 |
| H | ? | settings.rs | 229 |
| H | ? | settings.rs | 230 |
| H | ? | pyproject.rs | 92 |
| H | ? | pyproject.rs | 142 |
| H | ? | configuration_file.rs | 24 |
| H | ? | configuration_file.rs | 28 |
| H | ? | configuration_file.rs | 58 |
| H | ? | watcher.rs | 83 |
| H | ? | changes.rs | 140 |
| H | ? | changes.rs | 170 |
| H | ? | changes.rs | 194 |
| H | ? | changes.rs | 195 |
| H | ? | exclude.rs | 237 |
| H | ? | files.rs | 331 |
| H | ? | walk.rs | 276 |
| H | ? | walk.rs | 286 |
| H | ? | db.rs | 572 |
| H | ? | db.rs | 618 |
| H | ? | db.rs | 675 |
| H | ? | db.rs | 682 |
| H | ? | db.rs | 810 |
| H | ? | db.rs | 821 |
| H | ? | lib.rs | 204 |
| H | ? | lib.rs | 205 |
| H | ? | lib.rs | 662 |
| H | ? | lib.rs | 943 |
| H | ? | lib.rs | 947 |
| H | ? | symbols.rs | 180 |
| H | ? | symbols.rs | 234 |
| H | ? | symbols.rs | 279 |
| H | ? | symbols.rs | 299 |
| H | ? | symbols.rs | 777 |
| H | ? | symbols.rs | 1060 |
| H | ? | hints.rs | 61 |
| H | ? | rst.rs | 254 |
| H | ? | rst.rs | 348 |
| H | ? | google.rs | 117 |
| H | ? | google.rs | 207 |
| H | ? | google.rs | 850 |
| H | ? | completion.rs | 492 |
| H | ? | completion.rs | 2077 |
| H | ? | completion.rs | 11046 |
| H | ? | docstring.rs | 79 |
| H | ? | references.rs | 413 |
| H | ? | references.rs | 561 |
| H | ? | outgoing_calls.rs | 314 |
| H | ? | incoming_calls.rs | 406 |
| H | ? | incoming_calls.rs | 421 |
| H | ? | incoming_calls.rs | 522 |
| H | ? | inlay_hints.rs | 65 |
| H | ? | inlay_hints.rs | 739 |
| H | ? | inlay_hints.rs | 881 |
| H | ? | inlay_hints.rs | 8517 |
| H | ? | inlay_hints.rs | 8519 |
| H | ? | goto.rs | 442 |
| H | ? | lib.rs | 461 |
| H | ? | lib.rs | 646 |
| H | ? | lib.rs | 667 |
| H | ? | lib.rs | 668 |
| H | ? | lib.rs | 77 |
| H | ? | lib.rs | 314 |
| H | ? | cursor.rs | 31 |
| H | ? | cursor.rs | 47 |
| H | ? | cursor.rs | 53 |
| H | ? | cursor.rs | 61 |
| H | ? | cursor.rs | 103 |
| H | ? | cursor.rs | 116 |
| H | ? | tokenizer.rs | 925 |
| H | ? | tokenizer.rs | 975 |
| H | ? | session.rs | 100 |
| H | ? | server.rs | 80 |
| H | ? | server.rs | 110 |
| H | ? | server.rs | 130 |
| H | ? | server.rs | 131 |
| H | ? | fix.rs | 96 |
| H | ? | fix.rs | 126 |
| H | ? | notebook.rs | 90 |
| H | ? | notebook.rs | 154 |
| H | ? | notebook.rs | 228 |
| H | ? | notebook.rs | 276 |
| H | ? | notebook.rs | 290 |
| H | ? | text_document.rs | 105 |
| H | ? | traits.rs | 107 |
| H | ? | did_close.rs | 23 |
| H | ? | did_change_watched_files.rs | 30 |
| H | ? | did_change_watched_files.rs | 39 |
| H | ? | did_open_notebook.rs | 39 |
| H | ? | did_open.rs | 30 |
| H | ? | did_open.rs | 35 |
| H | ? | code_action.rs | 61 |
| H | ? | code_action.rs | 140 |
| H | ? | code_action.rs | 142 |
| H | ? | code_action.rs | 149 |
| H | ? | code_action.rs | 163 |
| H | ? | code_action.rs | 179 |
| H | ? | format.rs | 57 |
| H | ? | execute_command.rs | 85 |
| H | ? | execute_command.rs | 193 |
| H | ? | execute_command.rs | 209 |
| H | ? | code_action_resolve.rs | 28 |
| H | ? | code_action_resolve.rs | 35 |
| H | ? | code_action_resolve.rs | 57 |
| H | ? | code_action_resolve.rs | 147 |
| H | ? | api.rs | 48 |
| H | ? | api.rs | 254 |
| H | ? | pool.rs | 66 |
| H | ? | main_loop.rs | 20 |
| H | ? | main_loop.rs | 21 |
| H | ? | main_loop.rs | 34 |
| H | ? | main_loop.rs | 35 |
| H | ? | main_loop.rs | 43 |
| H | ? | options.rs | 135 |
| H | ? | options.rs | 755 |
| H | ? | options.rs | 757 |
| H | ? | options.rs | 792 |
| H | ? | options.rs | 795 |
| H | ? | settings.rs | 39 |
| H | ? | settings.rs | 60 |
| H | ? | client.rs | 139 |
| H | ? | client.rs | 141 |
| H | ? | index.rs | 161 |
| H | ? | index.rs | 209 |
| H | ? | index.rs | 288 |
| H | ? | index.rs | 308 |
| H | ? | index.rs | 341 |
| H | ? | index.rs | 435 |
| H | ? | index.rs | 504 |
| H | ? | index.rs | 509 |
| H | ? | index.rs | 548 |
| H | ? | index.rs | 552 |
| H | ? | index.rs | 553 |
| H | ? | index.rs | 662 |
| H | ? | index.rs | 665 |
| H | ? | ruff_settings.rs | 138 |
| H | ? | ruff_settings.rs | 305 |
| H | ? | ruff_settings.rs | 307 |
| H | ? | ruff_settings.rs | 308 |
| H | ? | ruff_settings.rs | 393 |
| H | ? | ruff_settings.rs | 397 |
| H | ? | ruff_settings.rs | 423 |
| H | ? | request_queue.rs | 155 |
| H | ? | lint.rs | 183 |
| H | ? | lint.rs | 210 |
| H | ? | lint.rs | 324 |
| H | ? | lint.rs | 461 |
| H | ? | lint.rs | 466 |
| H | ? | lint.rs | 528 |
| H | ? | semantic_model.rs | 459 |
| H | ? | semantic_model.rs | 460 |
| H | ? | types.rs | 6255 |
| H | ? | types.rs | 8051 |
| H | ? | types.rs | 8791 |
| H | ? | fixes.rs | 170 |
| H | ? | fixes.rs | 583 |
| H | ? | fixes.rs | 615 |
| H | ? | fixes.rs | 636 |
| H | ? | fixes.rs | 2071 |
| H | ? | pydantic.rs | 269 |
| H | ? | pydantic.rs | 817 |
| H | ? | pydantic.rs | 856 |
| H | ? | diagnostic.rs | 1622 |
| H | ? | diagnostic.rs | 1834 |
| H | ? | diagnostic.rs | 1835 |
| H | ? | diagnostic.rs | 1903 |
| H | ? | diagnostic.rs | 2085 |
| H | ? | diagnostic.rs | 2215 |
| H | ? | diagnostic.rs | 3847 |
| H | ? | diagnostic.rs | 3855 |
| H | ? | diagnostic.rs | 4245 |
| H | ? | diagnostic.rs | 4252 |
| H | ? | diagnostic.rs | 4258 |
| H | ? | diagnostic.rs | 4264 |
| H | ? | diagnostic.rs | 4265 |
| H | ? | diagnostic.rs | 4301 |
| H | ? | diagnostic.rs | 4318 |
| H | ? | diagnostic.rs | 4402 |
| H | ? | diagnostic.rs | 4408 |
| H | ? | diagnostic.rs | 4414 |
| H | ? | diagnostic.rs | 4419 |
| H | ? | diagnostic.rs | 4420 |
| H | ? | arguments.rs | 284 |
| H | ? | arguments.rs | 405 |
| H | ? | bind.rs | 263 |
| H | ? | bind.rs | 3318 |
| H | ? | bind.rs | 6877 |
| H | ? | bind.rs | 6972 |
| H | ? | bind.rs | 6973 |
| H | ? | bind.rs | 6974 |
| H | ? | bind.rs | 7571 |
| H | ? | constructor.rs | 380 |
| H | ? | enums.rs | 319 |
| H | ? | enums.rs | 324 |
| H | ? | enums.rs | 700 |
| H | ? | enums.rs | 915 |
| H | ? | enums.rs | 918 |
| H | ? | enums.rs | 969 |
| H | ? | enums.rs | 1092 |
| H | ? | enums.rs | 1219 |
| H | ? | signatures.rs | 125 |
| H | ? | signatures.rs | 224 |
| H | ? | signatures.rs | 244 |
| H | ? | signatures.rs | 270 |
| H | ? | signatures.rs | 840 |
| H | ? | signatures.rs | 846 |
| H | ? | signatures.rs | 876 |
| H | ? | signatures.rs | 906 |
| H | ? | signatures.rs | 1054 |
| H | ? | signatures.rs | 1269 |
| H | ? | signatures.rs | 1334 |
| H | ? | signatures.rs | 1377 |
| H | ? | signatures.rs | 1395 |
| H | ? | signatures.rs | 1396 |
| H | ? | signatures.rs | 1527 |
| H | ? | signatures.rs | 1528 |
| H | ? | signatures.rs | 1602 |
| H | ? | signatures.rs | 1851 |
| H | ? | signatures.rs | 1903 |
| H | ? | signatures.rs | 2159 |
| H | ? | signatures.rs | 2220 |
| H | ? | signatures.rs | 2441 |
| H | ? | signatures.rs | 2442 |
| H | ? | signatures.rs | 2478 |
| H | ? | signatures.rs | 2503 |
| H | ? | signatures.rs | 2542 |
| H | ? | signatures.rs | 2712 |
| H | ? | signatures.rs | 3084 |
| H | ? | signatures.rs | 3281 |
| H | ? | signatures.rs | 3282 |
| H | ? | signatures.rs | 3454 |
| H | ? | signatures.rs | 3455 |
| H | ? | signatures.rs | 3469 |
| H | ? | signatures.rs | 3757 |
| H | ? | signatures.rs | 3768 |
| H | ? | signatures.rs | 3887 |
| H | ? | signatures.rs | 3908 |
| H | ? | signatures.rs | 4195 |
| H | ? | signatures.rs | 4227 |
| H | ? | signatures.rs | 4239 |
| H | ? | signatures.rs | 4250 |
| H | ? | signatures.rs | 4262 |
| H | ? | signatures.rs | 4390 |
| H | ? | signatures.rs | 4435 |
| H | ? | signatures.rs | 4442 |
| H | ? | signatures.rs | 4469 |
| H | ? | signatures.rs | 4472 |
| H | ? | signatures.rs | 4476 |
| H | ? | signatures.rs | 4479 |
| H | ? | signatures.rs | 4483 |
| H | ? | signatures.rs | 4488 |
| H | ? | signatures.rs | 4492 |
| H | ? | signatures.rs | 4536 |
| H | ? | signatures.rs | 4771 |
| H | ? | signatures.rs | 4783 |
| H | ? | signatures.rs | 4797 |
| H | ? | signatures.rs | 4807 |
| H | ? | signatures.rs | 4809 |
| H | ? | signatures.rs | 4988 |
| H | ? | signatures.rs | 4991 |
| H | ? | signatures.rs | 5062 |
| H | ? | signatures.rs | 5072 |
| H | ? | signatures.rs | 5082 |
| H | ? | signatures.rs | 5088 |
| H | ? | signatures.rs | 5112 |
| H | ? | signatures.rs | 5116 |
| H | ? | signatures.rs | 5120 |
| H | ? | signatures.rs | 5122 |
| H | ? | class.rs | 1353 |
| H | ? | class.rs | 2185 |
| H | ? | relation_error.rs | 24 |
| H | ? | ide_support.rs | 614 |
| H | ? | ide_support.rs | 717 |
| H | ? | ide_support.rs | 822 |
| H | ? | ide_support.rs | 2099 |
| H | ? | known_instance.rs | 711 |
| H | ? | known_instance.rs | 745 |
| H | ? | class_base.rs | 475 |
| H | ? | overrides.rs | 178 |
| H | ? | overrides.rs | 214 |
| H | ? | overrides.rs | 770 |
| H | ? | overrides.rs | 1105 |
| H | ? | overrides.rs | 1803 |
| H | ? | relation.rs | 880 |
| H | ? | match_pattern.rs | 862 |
| H | ? | match_pattern.rs | 873 |
| H | ? | callable.rs | 166 |
| H | ? | callable.rs | 187 |
| H | ? | callable.rs | 737 |
| H | ? | callable.rs | 738 |
| H | ? | dict.rs | 96 |
| H | ? | static_class.rs | 137 |
| H | ? | static_class.rs | 839 |
| H | ? | static_class.rs | 850 |
| H | ? | static_class.rs | 857 |
| H | ? | static_class.rs | 1077 |
| H | ? | static_class.rs | 1094 |
| H | ? | function.rs | 206 |
| H | ? | function.rs | 229 |
| H | ? | function.rs | 240 |
| H | ? | overloaded_function.rs | 301 |
| H | ? | typed_dict.rs | 121 |
| H | ? | enum_call.rs | 588 |
| H | ? | type_call.rs | 167 |
| H | ? | type_call.rs | 245 |
| H | ? | imports.rs | 418 |
| H | ? | imports.rs | 576 |
| H | ? | new_class.rs | 124 |
| H | ? | named_tuple.rs | 534 |
| H | ? | named_tuple.rs | 683 |
| H | ? | typevar.rs | 120 |
| H | ? | typevar.rs | 1001 |
| H | ? | builder.rs | 604 |
| H | ? | builder.rs | 680 |
| H | ? | builder.rs | 718 |
| H | ? | builder.rs | 752 |
| H | ? | builder.rs | 5043 |
| H | ? | builder.rs | 5132 |
| H | ? | builder.rs | 5134 |
| H | ? | builder.rs | 5155 |
| H | ? | builder.rs | 5211 |
| H | ? | builder.rs | 5294 |
| H | ? | builder.rs | 5313 |
| H | ? | builder.rs | 5314 |
| H | ? | builder.rs | 5364 |
| H | ? | builder.rs | 5365 |
| H | ? | builder.rs | 5368 |
| H | ? | builder.rs | 5373 |
| H | ? | builder.rs | 5397 |
| H | ? | builder.rs | 5457 |
| H | ? | builder.rs | 6099 |
| H | ? | builder.rs | 7039 |
| H | ? | builder.rs | 7147 |
| H | ? | builder.rs | 7171 |
| H | ? | builder.rs | 7869 |
| H | ? | builder.rs | 7886 |
| H | ? | builder.rs | 7902 |
| H | ? | builder.rs | 7907 |
| H | ? | builder.rs | 7918 |
| H | ? | builder.rs | 8013 |
| H | ? | builder.rs | 9010 |
| H | ? | builder.rs | 9928 |
| H | ? | builder.rs | 11188 |
| H | ? | unused_bindings.rs | 176 |
| H | ? | unreachable_code.rs | 138 |
| H | ? | display.rs | 138 |
| H | ? | display.rs | 146 |
| H | ? | display.rs | 162 |
| H | ? | display.rs | 170 |
| H | ? | display.rs | 178 |
| H | ? | display.rs | 184 |
| H | ? | display.rs | 188 |
| H | ? | display.rs | 205 |
| H | ? | display.rs | 654 |
| H | ? | display.rs | 885 |
| H | ? | display.rs | 889 |
| H | ? | display.rs | 971 |
| H | ? | display.rs | 974 |
| H | ? | display.rs | 976 |
| H | ? | display.rs | 982 |
| H | ? | display.rs | 985 |
| H | ? | display.rs | 1025 |
| H | ? | display.rs | 1034 |
| H | ? | display.rs | 1044 |
| H | ? | display.rs | 1053 |
| H | ? | display.rs | 1069 |
| H | ? | display.rs | 1083 |
| H | ? | display.rs | 1093 |
| H | ? | display.rs | 1096 |
| H | ? | display.rs | 1099 |
| H | ? | display.rs | 1112 |
| H | ? | display.rs | 1141 |
| H | ? | display.rs | 1297 |
| H | ? | display.rs | 1300 |
| H | ? | display.rs | 1309 |
| H | ? | display.rs | 1315 |
| H | ? | display.rs | 1329 |
| H | ? | display.rs | 1352 |
| H | ? | display.rs | 1369 |
| H | ? | display.rs | 1398 |
| H | ? | display.rs | 1404 |
| H | ? | display.rs | 1407 |
| H | ? | display.rs | 1430 |
| H | ? | display.rs | 1435 |
| H | ? | display.rs | 1624 |
| H | ? | display.rs | 1679 |
| H | ? | display.rs | 1680 |
| H | ? | display.rs | 1693 |
| H | ? | display.rs | 1715 |
| H | ? | display.rs | 1763 |
| H | ? | display.rs | 1780 |
| H | ? | display.rs | 1786 |
| H | ? | display.rs | 1845 |
| H | ? | display.rs | 1996 |
| H | ? | display.rs | 2017 |
| H | ? | display.rs | 2027 |
| H | ? | display.rs | 2038 |
| H | ? | display.rs | 2062 |
| H | ? | display.rs | 2141 |
| H | ? | display.rs | 2148 |
| H | ? | display.rs | 2163 |
| H | ? | display.rs | 2274 |
| H | ? | display.rs | 2283 |
| H | ? | display.rs | 2467 |
| H | ? | display.rs | 2523 |
| H | ? | display.rs | 2534 |
| H | ? | display.rs | 2557 |
| H | ? | display.rs | 2583 |
| H | ? | display.rs | 3025 |
| H | ? | display.rs | 3065 |
| H | ? | display.rs | 3080 |
| H | ? | display.rs | 3311 |
| H | ? | constraints.rs | 299 |
| H | ? | constraints.rs | 3179 |
| H | ? | static_literal.rs | 1362 |
| H | ? | static_literal.rs | 1556 |
| H | ? | static_literal.rs | 1567 |
| H | ? | static_literal.rs | 1574 |
| H | ? | static_literal.rs | 1658 |
| H | ? | static_literal.rs | 2024 |
| H | ? | static_literal.rs | 2029 |
| H | ? | static_literal.rs | 2061 |
| H | ? | static_literal.rs | 2172 |
| H | ? | static_literal.rs | 2199 |
| H | ? | static_literal.rs | 2319 |
| H | ? | dynamic_literal.rs | 551 |
| H | ? | enum_literal.rs | 40 |
| H | ? | typed_dict.rs | 155 |
| H | ? | typed_dict.rs | 163 |
| H | ? | typed_dict.rs | 166 |
| H | ? | typed_dict.rs | 172 |
| H | ? | typed_dict.rs | 487 |
| H | ? | named_tuple.rs | 610 |
| H | ? | tuple.rs | 848 |
| H | ? | tuple.rs | 2936 |
| H | ? | tuple.rs | 2975 |
| H | ? | generics.rs | 1055 |
| H | ? | function.rs | 700 |
| H | ? | function.rs | 716 |
| H | ? | function.rs | 717 |
| H | ? | function.rs | 718 |
| H | ? | function.rs | 719 |
| H | ? | function.rs | 1091 |
| H | ? | function.rs | 2591 |
| H | ? | builder.rs | 1265 |
| H | ? | builder.rs | 1339 |
| H | ? | builder.rs | 1340 |
| H | ? | builder.rs | 1348 |
| H | ? | builder.rs | 1349 |
| H | ? | builder.rs | 1447 |
| H | ? | cyclic.rs | 369 |
| H | ? | cyclic.rs | 400 |
| H | ? | cyclic.rs | 405 |
| H | ? | cyclic.rs | 428 |
| H | ? | cyclic.rs | 440 |
| H | ? | cyclic.rs | 651 |
| H | ? | narrow.rs | 732 |
| H | ? | narrow.rs | 733 |
| H | ? | narrow.rs | 744 |
| H | ? | narrow.rs | 745 |
| H | ? | narrow.rs | 855 |
| H | ? | narrow.rs | 1893 |
| H | ? | narrow.rs | 1902 |
| H | ? | narrow.rs | 3360 |
| H | ? | narrow.rs | 3510 |
| H | ? | narrow.rs | 3532 |
| H | ? | narrow.rs | 3869 |
| H | ? | enums.rs | 37 |
| H | ? | enums.rs | 775 |
| H | ? | enums.rs | 806 |
| H | ? | bound_super.rs | 929 |
| H | ? | typed_dict.rs | 514 |
| H | ? | typed_dict.rs | 578 |
| H | ? | typed_dict.rs | 595 |
| H | ? | typed_dict.rs | 599 |
| H | ? | typed_dict.rs | 737 |
| H | ? | typed_dict.rs | 747 |
| H | ? | typed_dict.rs | 769 |
| H | ? | typed_dict.rs | 823 |
| H | ? | typed_dict.rs | 836 |
| H | ? | typed_dict.rs | 888 |
| H | ? | typed_dict.rs | 1587 |
| H | ? | typed_dict.rs | 1730 |
| H | ? | typed_dict.rs | 1762 |
| H | ? | typed_dict.rs | 1930 |
| H | ? | typed_dict.rs | 1990 |
| H | ? | typed_dict.rs | 2084 |
| H | ? | typed_dict.rs | 2108 |
| H | ? | typed_dict.rs | 2113 |
| H | ? | typed_dict.rs | 2167 |
| H | ? | typed_dict.rs | 2467 |
| H | ? | typed_dict.rs | 2530 |
| H | ? | typed_dict.rs | 2578 |
| H | ? | typed_dict.rs | 2726 |
| H | ? | typed_dict.rs | 2785 |
| H | ? | typed_dict.rs | 2789 |
| H | ? | typed_dict.rs | 2810 |
| H | ? | typed_dict.rs | 2933 |
| H | ? | typed_dict.rs | 2936 |
| H | ? | typed_dict.rs | 2971 |
| H | ? | typed_dict.rs | 2973 |
| H | ? | set_theoretic.rs | 805 |
| H | ? | set_theoretic.rs | 814 |
| H | ? | list_members.rs | 49 |
| H | ? | list_members.rs | 69 |
| H | ? | list_members.rs | 104 |
| H | ? | list_members.rs | 120 |
| H | ? | list_members.rs | 426 |
| H | ? | list_members.rs | 435 |
| H | ? | protocol_class.rs | 92 |
| H | ? | protocol_class.rs | 431 |
| H | ? | protocol_class.rs | 433 |
| H | ? | protocol_class.rs | 461 |
| H | ? | protocol_class.rs | 628 |
| H | ? | protocol_class.rs | 649 |
| H | ? | protocol_class.rs | 3074 |
| H | ? | subscript.rs | 237 |
| H | ? | subscript.rs | 238 |
| H | ? | subscript.rs | 239 |
| H | ? | subscript.rs | 240 |
| H | ? | subscript.rs | 241 |
| H | ? | subscript.rs | 249 |
| H | ? | subscript.rs | 250 |
| H | ? | subscript.rs | 251 |
| H | ? | subscript.rs | 252 |
| H | ? | subscript.rs | 260 |
| H | ? | subscript.rs | 261 |
| H | ? | subscript.rs | 262 |
| H | ? | subscript.rs | 263 |
| H | ? | subscript.rs | 265 |
| H | ? | subscript.rs | 266 |
| H | ? | subscript.rs | 267 |
| H | ? | subscript.rs | 268 |
| H | ? | subscript.rs | 277 |
| H | ? | subscript.rs | 278 |
| H | ? | subscript.rs | 279 |
| H | ? | subscript.rs | 281 |
| H | ? | subscript.rs | 282 |
| H | ? | subscript.rs | 283 |
| H | ? | db.rs | 71 |
| H | ? | db.rs | 79 |
| H | ? | db.rs | 178 |
| H | ? | reachability.rs | 313 |
| H | ? | reachability.rs | 354 |
| H | ? | reachability.rs | 1096 |
| H | ? | reachability.rs | 1103 |
| H | ? | reachability.rs | 1254 |
| H | ? | reachability.rs | 1267 |
| H | ? | reachability.rs | 1270 |
| H | ? | lib.rs | 189 |
| H | ? | document.rs | 302 |
| H | ? | document.rs | 387 |
| H | ? | buffer.rs | 382 |
| H | ? | buffer.rs | 451 |
| H | ? | buffer.rs | 458 |
| H | ? | buffer.rs | 461 |
| H | ? | buffer.rs | 481 |
| H | ? | format_extensions.rs | 163 |
| H | ? | parameters.rs | 62 |
| H | ? | except_handler_except_handler.rs | 52 |
| H | ? | arguments.rs | 32 |
| H | ? | arguments.rs | 88 |
| H | ? | interpolated_string_element.rs | 157 |
| H | ? | match_case.rs | 35 |
| H | ? | comprehension.rs | 62 |
| H | ? | alias.rs | 21 |
| H | ? | with_item.rs | 100 |
| H | ? | expr_lambda.rs | 29 |
| H | ? | expr_lambda.rs | 269 |
| H | ? | mod.rs | 121 |
| H | ? | mod.rs | 362 |
| H | ? | expr_generator.rs | 52 |
| H | ? | expr_list.rs | 23 |
| H | ? | expr_if.rs | 54 |
| H | ? | expr_dict_comp.rs | 23 |
| H | ? | expr_attribute.rs | 77 |
| H | ? | expr_unary_op.rs | 32 |
| H | ? | expr_subscript.rs | 38 |
| H | ? | expr_slice.rs | 39 |
| H | ? | expr_list_comp.rs | 26 |
| H | ? | expr_named.rs | 24 |
| H | ? | expr_dict.rs | 22 |
| H | ? | expr_dict.rs | 128 |
| H | ? | binary_like.rs | 269 |
| H | ? | binary_like.rs | 853 |
| H | ? | expr_starred.rs | 22 |
| H | ? | expr_set_comp.rs | 26 |
| H | ? | expr_tuple.rs | 123 |
| H | ? | expr_call.rs | 33 |
| H | ? | expr_set.rs | 27 |
| H | ? | type_params.rs | 22 |
| H | ? | mod.rs | 66 |
| H | ? | pattern_match_or.rs | 24 |
| H | ? | pattern_arguments.rs | 21 |
| H | ? | pattern_arguments.rs | 64 |
| H | ? | pattern_match_mapping.rs | 29 |
| H | ? | pattern_match_star.rs | 16 |
| H | ? | pattern_match_sequence.rs | 23 |
| H | ? | pattern_match_class.rs | 21 |
| H | ? | pattern_match_as.rs | 21 |
| H | ? | verbatim.rs | 69 |
| H | ? | verbatim.rs | 121 |
| H | ? | verbatim.rs | 274 |
| H | ? | verbatim.rs | 462 |
| H | ? | implicit.rs | 84 |
| H | ? | docstring.rs | 188 |
| H | ? | docstring.rs | 532 |
| H | ? | normalize.rs | 711 |
| H | ? | format.rs | 57 |
| H | ? | format.rs | 215 |
| H | ? | node_key.rs | 90 |
| H | ? | stmt_ann_assign.rs | 25 |
| H | ? | stmt_with.rs | 35 |
| H | ? | stmt_class_def.rs | 29 |
| H | ? | stmt_import_from.rs | 67 |
| H | ? | stmt_assign.rs | 297 |
| H | ? | stmt_assign.rs | 577 |
| H | ? | stmt_if.rs | 24 |
| H | ? | stmt_if.rs | 72 |
| H | ? | suite.rs | 104 |
| H | ? | suite.rs | 115 |
| H | ? | suite.rs | 224 |
| H | ? | suite.rs | 835 |
| H | ? | stmt_match.rs | 23 |
| H | ? | clause.rs | 766 |
| H | ? | stmt_try.rs | 72 |
| H | ? | stmt_function_def.rs | 24 |
| H | ? | stmt_function_def.rs | 107 |
| H | ? | stmt_for.rs | 42 |
| H | ? | stmt_while.rs | 24 |
| H | ? | lib.rs | 58 |
| H | ? | lib.rs | 186 |
| H | ? | lib.rs | 324 |
| H | ? | formatter.rs | 33 |
| H | ? | formatter.rs | 34 |
| H | ? | formatter.rs | 35 |
| H | ? | formatter.rs | 36 |
| H | ? | formatter.rs | 37 |
| H | ? | parser.rs | 30 |
| H | ? | parser.rs | 31 |
| H | ? | parser.rs | 32 |
| H | ? | parser.rs | 33 |
| H | ? | parser.rs | 34 |
| H | ? | linter.rs | 57 |
| H | ? | linter.rs | 58 |
| H | ? | linter.rs | 59 |
| H | ? | linter.rs | 60 |
| H | ? | linter.rs | 61 |
| H | ? | linter.rs | 80 |
| H | ? | ty_walltime.rs | 33 |
| H | ? | ty_walltime.rs | 41 |
| H | ? | module_resolution.rs | 46 |
| H | ? | ty.rs | 77 |
| H | ? | ty.rs | 167 |
| H | ? | ty.rs | 246 |
| H | ? | ty.rs | 1802 |
| H | ? | lexer.rs | 31 |
| H | ? | lexer.rs | 32 |
| H | ? | lexer.rs | 33 |
| H | ? | lexer.rs | 34 |
| H | ? | lexer.rs | 35 |
| H | ? | use_def.rs | 1922 |
| H | ? | use_def.rs | 1923 |
| H | ? | use_def.rs | 2136 |
| H | ? | use_def.rs | 2145 |
| H | ? | use_def.rs | 2327 |
| H | ? | use_def.rs | 2423 |
| H | ? | use_def.rs | 2442 |
| H | ? | use_def.rs | 2555 |
| H | ? | use_def.rs | 2574 |
| H | ? | use_def.rs | 2615 |
| H | ? | use_def.rs | 2616 |
| H | ? | use_def.rs | 2665 |
| H | ? | use_def.rs | 2984 |
| H | ? | program.rs | 84 |
| H | ? | program.rs | 85 |
| H | ? | program.rs | 86 |
| H | ? | loop_bindings_visitor.rs | 111 |
| H | ? | loop_bindings_visitor.rs | 122 |
| H | ? | loop_bindings_visitor.rs | 130 |
| H | ? | loop_bindings_visitor.rs | 136 |
| H | ? | loop_bindings_visitor.rs | 141 |
| H | ? | loop_bindings_visitor.rs | 176 |
| H | ? | loop_bindings_visitor.rs | 182 |
| H | ? | loop_bindings_visitor.rs | 188 |
| H | ? | re_exports.rs | 91 |
| H | ? | place.rs | 53 |
| H | ? | place.rs | 78 |
| H | ? | platform.rs | 28 |
| H | ? | scope.rs | 156 |
| H | ? | member.rs | 221 |
| H | ? | member.rs | 306 |
| H | ? | db.rs | 57 |
| H | ? | definition.rs | 984 |
| H | ? | builder.rs | 662 |
| H | ? | builder.rs | 702 |
| H | ? | builder.rs | 715 |
| H | ? | builder.rs | 1015 |
| H | ? | builder.rs | 1070 |
| H | ? | builder.rs | 1181 |
| H | ? | builder.rs | 1689 |
| H | ? | builder.rs | 1802 |
| H | ? | builder.rs | 2100 |
| H | ? | builder.rs | 2118 |
| H | ? | builder.rs | 2144 |
| H | ? | builder.rs | 2147 |
| H | ? | builder.rs | 2358 |
| H | ? | builder.rs | 2481 |
| H | ? | builder.rs | 2491 |
| H | ? | builder.rs | 2503 |
| H | ? | builder.rs | 2530 |
| H | ? | builder.rs | 2549 |
| H | ? | builder.rs | 2570 |
| H | ? | builder.rs | 2824 |
| H | ? | builder.rs | 2866 |
| H | ? | builder.rs | 2874 |
| H | ? | builder.rs | 2901 |
| H | ? | builder.rs | 3044 |
| H | ? | builder.rs | 3115 |
| H | ? | builder.rs | 3224 |
| H | ? | builder.rs | 3787 |
| H | ? | builder.rs | 3881 |
| H | ? | builder.rs | 3907 |
| H | ? | builder.rs | 3994 |
| H | ? | builder.rs | 4037 |
| H | ? | builder.rs | 4049 |
| H | ? | builder.rs | 4088 |
| H | ? | builder.rs | 4671 |
| H | ? | builder.rs | 4718 |
| H | ? | builder.rs | 4739 |
| H | ? | cache.rs | 546 |
| H | ? | cache.rs | 592 |
| H | ? | cache.rs | 602 |
| H | ? | cache.rs | 896 |
| H | ? | cache.rs | 1030 |
| H | ? | cache.rs | 1057 |
| H | ? | format.rs | 174 |
| H | ? | format.rs | 373 |
| H | ? | format.rs | 434 |
| H | ? | format.rs | 489 |
| H | ? | format.rs | 750 |
| H | ? | format.rs | 1311 |
| H | ? | format.rs | 1322 |
| H | ? | format.rs | 1325 |
| H | ? | format.rs | 1327 |
| H | ? | format.rs | 1331 |
| H | ? | format.rs | 1338 |
| H | ? | check.rs | 130 |
| H | ? | analyze_graph.rs | 34 |
| H | ? | analyze_graph.rs | 86 |
| H | ? | analyze_graph.rs | 119 |
| H | ? | analyze_graph.rs | 161 |
| H | ? | analyze_graph.rs | 162 |
| H | ? | analyze_graph.rs | 163 |
| H | ? | analyze_graph.rs | 164 |
| H | ? | analyze_graph.rs | 248 |
| H | ? | analyze_graph.rs | 281 |
| H | ? | args.rs | 739 |
| H | ? | args.rs | 786 |
| H | ? | args.rs | 1418 |
| H | ? | args.rs | 1421 |
| H | ? | args.rs | 1424 |
| H | ? | args.rs | 1427 |
| H | ? | args.rs | 1433 |
| H | ? | args.rs | 1445 |
| H | ? | args.rs | 1453 |
| H | ? | args.rs | 1454 |
| H | ? | args.rs | 1462 |
| H | ? | args.rs | 1483 |
| H | ? | tokens.rs | 380 |
| H | ? | helpers.rs | 1696 |
| H | ? | helpers.rs | 1716 |
| H | ? | helpers.rs | 1926 |
| H | ? | helpers.rs | 1934 |
| H | ? | helpers.rs | 1938 |
| H | ? | helpers.rs | 1944 |
| H | ? | helpers.rs | 1949 |
| H | ? | helpers.rs | 1978 |
| H | ? | helpers.rs | 1996 |
| H | ? | helpers.rs | 2034 |
| H | ? | helpers.rs | 2071 |
| H | ? | nodes.rs | 1220 |
| H | ? | nodes.rs | 1312 |
| H | ? | nodes.rs | 2889 |
| H | ? | nodes.rs | 2891 |
| H | ? | nodes.rs | 2896 |
| H | ? | lib.rs | 139 |
| H | ? | lib.rs | 199 |
| H | ? | lib.rs | 1686 |
| H | ? | session.rs | 364 |
| H | ? | session.rs | 504 |
| H | ? | session.rs | 544 |
| H | ? | session.rs | 584 |
| H | ? | session.rs | 585 |
| H | ? | session.rs | 591 |
| H | ? | session.rs | 600 |
| H | ? | session.rs | 608 |
| H | ? | session.rs | 611 |
| H | ? | session.rs | 649 |
| H | ? | session.rs | 706 |
| H | ? | session.rs | 723 |
| H | ? | session.rs | 732 |
| H | ? | session.rs | 872 |
| H | ? | session.rs | 981 |
| H | ? | session.rs | 1112 |
| H | ? | session.rs | 1147 |
| H | ? | session.rs | 1148 |
| H | ? | session.rs | 1229 |
| H | ? | session.rs | 1233 |
| H | ? | session.rs | 1354 |
| H | ? | session.rs | 1626 |
| H | ? | session.rs | 1709 |
| H | ? | session.rs | 1713 |
| H | ? | session.rs | 1715 |
| H | ? | session.rs | 1723 |
| H | ? | session.rs | 1865 |
| H | ? | session.rs | 1868 |
| H | ? | server.rs | 100 |
| H | ? | server.rs | 164 |
| H | ? | server.rs | 165 |
| H | ? | system.rs | 283 |
| H | ? | range.rs | 42 |
| H | ? | range.rs | 204 |
| H | ? | range.rs | 319 |
| H | ? | notebook.rs | 53 |
| H | ? | notebook.rs | 115 |
| H | ? | notebook.rs | 140 |
| H | ? | notebook.rs | 151 |
| H | ? | document.rs | 96 |
| H | ? | did_change_watched_files.rs | 79 |
| H | ? | did_open_notebook.rs | 43 |
| H | ? | did_change_workspace_folders.rs | 39 |
| H | ? | diagnostics.rs | 116 |
| H | ? | diagnostics.rs | 266 |
| H | ? | code_action.rs | 77 |
| H | ? | code_action.rs | 106 |
| H | ? | workspace_diagnostic.rs | 152 |
| H | ? | workspace_diagnostic.rs | 180 |
| H | ? | workspace_diagnostic.rs | 349 |
| H | ? | workspace_diagnostic.rs | 630 |
| H | ? | completion.rs | 101 |
| H | ? | rename.rs | 64 |
| H | ? | api.rs | 31 |
| H | ? | api.rs | 253 |
| H | ? | api.rs | 301 |
| H | ? | api.rs | 333 |
| H | ? | api.rs | 388 |
| H | ? | lazy_work_done_progress.rs | 57 |
| H | ? | lazy_work_done_progress.rs | 72 |
| H | ? | lazy_work_done_progress.rs | 82 |
| H | ? | lazy_work_done_progress.rs | 87 |
| H | ? | lazy_work_done_progress.rs | 90 |
| H | ? | lazy_work_done_progress.rs | 129 |
| H | ? | lazy_work_done_progress.rs | 160 |
| H | ? | pool.rs | 62 |
| H | ? | main_loop.rs | 18 |
| H | ? | main_loop.rs | 19 |
| H | ? | main_loop.rs | 30 |
| H | ? | main_loop.rs | 31 |
| H | ? | main_loop.rs | 45 |
| H | ? | client.rs | 87 |
| H | ? | client.rs | 144 |
| H | ? | client.rs | 146 |
| H | ? | index.rs | 131 |
| H | ? | index.rs | 180 |
| H | ? | index.rs | 208 |
| H | ? | index.rs | 219 |
| H | ? | request_queue.rs | 154 |
| H | ? | main.rs | 526 |
| H | ? | notebook.rs | 158 |
| H | ? | notebook.rs | 175 |
| H | ? | notebook.rs | 825 |
| H | ? | config.rs | 57 |
| H | ? | db.rs | 44 |
| H | ? | db.rs | 164 |
| H | ? | db.rs | 527 |
| H | ? | db.rs | 547 |
| H | ? | lib.rs | 132 |
| H | ? | lib.rs | 233 |
| H | ? | lib.rs | 293 |
| H | ? | test.rs | 115 |
| H | ? | test.rs | 116 |
| H | ? | test.rs | 294 |
| H | ? | test.rs | 430 |
| H | ? | test.rs | 436 |
| H | ? | test.rs | 444 |
| H | ? | test.rs | 458 |
| H | ? | test.rs | 495 |
| H | ? | violation.rs | 78 |
| H | ? | linter.rs | 522 |
| H | ? | linter.rs | 525 |
| H | ? | linter.rs | 530 |
| H | ? | mod.rs | 2729 |
| H | ? | mod.rs | 3436 |
| H | ? | mod.rs | 3505 |
| H | ? | mod.rs | 3760 |
| H | ? | mod.rs | 3772 |
| H | ? | definition.rs | 786 |
| H | ? | definition.rs | 813 |
| H | ? | definition.rs | 903 |
| H | ? | definition.rs | 938 |
| H | ? | repeated_append.rs | 101 |
| H | ? | repeated_append.rs | 339 |
| H | ? | repeated_append.rs | 352 |
| H | ? | print_empty_string.rs | 233 |
| H | ? | delete_full_slice.rs | 74 |
| H | ? | verbose_decimal_constructor.rs | 154 |
| H | ? | verbose_decimal_constructor.rs | 200 |
| H | ? | reimplemented_starmap.rs | 322 |
| H | ? | slice_copy.rs | 70 |
| H | ? | unnecessary_enumerate.rs | 191 |
| H | ? | bit_count.rs | 191 |
| H | ? | check_and_remove_from_set.rs | 185 |
| H | ? | check_and_remove_from_set.rs | 195 |
| H | ? | helpers.rs | 68 |
| H | ? | literal_comparisons.rs | 424 |
| H | ? | lambda_assignment.rs | 171 |
| H | ? | lambda_assignment.rs | 180 |
| H | ? | lambda_assignment.rs | 215 |
| H | ? | lambda_assignment.rs | 216 |
| H | ? | lambda_assignment.rs | 218 |
| H | ? | lambda_assignment.rs | 229 |
| H | ? | lambda_assignment.rs | 230 |
| H | ? | lambda_assignment.rs | 232 |
| H | ? | compound_statements.rs | 165 |
| H | ? | suspicious_function_call.rs | 1019 |
| H | ? | redundant_numeric_union.rs | 340 |
| H | ? | redundant_numeric_union.rs | 345 |
| H | ? | duplicate_union_member.rs | 153 |
| H | ? | duplicate_union_member.rs | 182 |
| H | ? | duplicate_union_member.rs | 187 |
| H | ? | unnecessary_literal_union.rs | 140 |
| H | ? | unnecessary_literal_union.rs | 164 |
| H | ? | redundant_none_literal.rs | 136 |
| H | ? | redundant_none_literal.rs | 215 |
| H | ? | redundant_none_literal.rs | 228 |
| H | ? | unnecessary_type_union.rs | 122 |
| H | ? | unnecessary_type_union.rs | 166 |
| H | ? | unnecessary_type_union.rs | 201 |
| H | ? | duplicate_literal_member.rs | 91 |
| H | ? | duplicate_literal_member.rs | 101 |
| H | ? | duplicate_literal_member.rs | 115 |
| H | ? | settings.rs | 25 |
| H | ? | categorize.rs | 321 |
| H | ? | categorize.rs | 485 |
| H | ? | categorize.rs | 519 |
| H | ? | categorize.rs | 551 |
| H | ? | categorize.rs | 582 |
| H | ? | categorize.rs | 613 |
| H | ? | categorize.rs | 644 |
| H | ? | categorize.rs | 688 |
| H | ? | categorize.rs | 703 |
| H | ? | normalize.rs | 91 |
| H | ? | normalize.rs | 97 |
| H | ? | normalize.rs | 100 |
| H | ? | multiple_starts_ends_with.rs | 222 |
| H | ? | numpy_2_0_deprecation.rs | 84 |
| H | ? | needless_bool.rs | 234 |
| H | ? | needless_bool.rs | 257 |
| H | ? | needless_bool.rs | 258 |
| H | ? | needless_bool.rs | 266 |
| H | ? | needless_bool.rs | 274 |
| H | ? | needless_bool.rs | 286 |
| H | ? | needless_bool.rs | 303 |
| H | ? | fix_with.rs | 74 |
| H | ? | ast_bool_op.rs | 541 |
| H | ? | ast_bool_op.rs | 564 |
| H | ? | zip_dict_keys_and_values.rs | 124 |
| H | ? | collapsible_if.rs | 391 |
| H | ? | collapsible_if.rs | 396 |
| H | ? | collapsible_if.rs | 400 |
| H | ? | if_else_block_instead_of_dict_get.rs | 195 |
| H | ? | if_else_block_instead_of_dict_get.rs | 196 |
| H | ? | if_else_block_instead_of_dict_get.rs | 198 |
| H | ? | if_else_block_instead_of_dict_get.rs | 215 |
| H | ? | if_else_block_instead_of_dict_get.rs | 237 |
| H | ? | if_else_block_instead_of_dict_get.rs | 304 |
| H | ? | if_else_block_instead_of_dict_get.rs | 305 |
| H | ? | if_else_block_instead_of_dict_get.rs | 307 |
| H | ? | if_else_block_instead_of_dict_get.rs | 329 |
| H | ? | yoda_conditions.rs | 146 |
| H | ? | yoda_conditions.rs | 149 |
| H | ? | yoda_conditions.rs | 155 |
| H | ? | yoda_conditions.rs | 232 |
| H | ? | ast_expr.rs | 230 |
| H | ? | ast_expr.rs | 311 |
| H | ? | reimplemented_builtin.rs | 127 |
| H | ? | reimplemented_builtin.rs | 150 |
| H | ? | reimplemented_builtin.rs | 173 |
| H | ? | reimplemented_builtin.rs | 175 |
| H | ? | reimplemented_builtin.rs | 183 |
| H | ? | reimplemented_builtin.rs | 192 |
| H | ? | reimplemented_builtin.rs | 223 |
| H | ? | reimplemented_builtin.rs | 411 |
| H | ? | reimplemented_builtin.rs | 413 |
| H | ? | reimplemented_builtin.rs | 414 |
| H | ? | suppressible_exception.rs | 145 |
| H | ? | ast_ifexp.rs | 194 |
| H | ? | ast_ifexp.rs | 226 |
| H | ? | ast_ifexp.rs | 275 |
| H | ? | ast_ifexp.rs | 276 |
| H | ? | ast_ifexp.rs | 277 |
| H | ? | if_else_block_instead_of_if_exp.rs | 242 |
| H | ? | if_else_block_instead_of_if_exp.rs | 271 |
| H | ? | if_else_block_instead_of_if_exp.rs | 272 |
| H | ? | if_else_block_instead_of_if_exp.rs | 273 |
| H | ? | if_else_block_instead_of_if_exp.rs | 278 |
| H | ? | if_else_block_instead_of_if_exp.rs | 289 |
| H | ? | if_else_block_instead_of_if_exp.rs | 294 |
| H | ? | if_else_block_instead_of_if_exp.rs | 306 |
| H | ? | if_else_block_instead_of_if_exp.rs | 312 |
| H | ? | ast_unary_op.rs | 188 |
| H | ? | ast_unary_op.rs | 190 |
| H | ? | ast_unary_op.rs | 244 |
| H | ? | ast_unary_op.rs | 246 |
| H | ? | ast_unary_op.rs | 295 |
| H | ? | deprecated_mock_import.rs | 81 |
| H | ? | deprecated_mock_import.rs | 90 |
| H | ? | deprecated_mock_import.rs | 99 |
| H | ? | deprecated_mock_import.rs | 165 |
| H | ? | deprecated_mock_import.rs | 223 |
| H | ? | deprecated_mock_import.rs | 328 |
| H | ? | unnecessary_default_type_args.rs | 123 |
| H | ? | unnecessary_default_type_args.rs | 125 |
| H | ? | unnecessary_default_type_args.rs | 199 |
| H | ? | unnecessary_default_type_args.rs | 210 |
| H | ? | use_pep604_annotation.rs | 386 |
| H | ? | convert_typed_dict_functional_to_class.rs | 160 |
| H | ? | convert_typed_dict_functional_to_class.rs | 179 |
| H | ? | convert_typed_dict_functional_to_class.rs | 181 |
| H | ? | timeout_error_alias.rs | 133 |
| H | ? | mod.rs | 144 |
| H | ? | mod.rs | 151 |
| H | ? | mod.rs | 156 |
| H | ? | convert_named_tuple_functional_to_class.rs | 175 |
| H | ? | convert_named_tuple_functional_to_class.rs | 228 |
| H | ? | convert_named_tuple_functional_to_class.rs | 239 |
| H | ? | os_error_alias.rs | 120 |
| H | ? | format_literals.rs | 188 |
| H | ? | format_literals.rs | 189 |
| H | ? | format_literals.rs | 193 |
| H | ? | format_literals.rs | 194 |
| H | ? | outdated_version_block.rs | 449 |
| H | ? | implicit.rs | 247 |
| H | ? | implicit.rs | 253 |
| H | ? | none_not_at_end_of_union.rs | 181 |
| H | ? | never_union.rs | 187 |
| H | ? | implicit_optional.rs | 143 |
| H | ? | implicit_optional.rs | 174 |
| H | ? | unnecessary_regular_expression.rs | 134 |
| H | ? | unnecessary_regular_expression.rs | 289 |
| H | ? | unnecessary_regular_expression.rs | 291 |
| H | ? | unnecessary_regular_expression.rs | 304 |
| H | ? | unnecessary_regular_expression.rs | 308 |
| H | ? | unnecessary_regular_expression.rs | 333 |
| H | ? | unnecessary_regular_expression.rs | 335 |
| H | ? | unnecessary_regular_expression.rs | 345 |
| H | ? | mutable_fromkeys_value.rs | 115 |
| H | ? | mutable_fromkeys_value.rs | 116 |
| H | ? | mutable_fromkeys_value.rs | 125 |
| H | ? | legacy_form_pytest_raises.rs | 245 |
| H | ? | legacy_form_pytest_raises.rs | 246 |
| H | ? | legacy_form_pytest_raises.rs | 252 |
| H | ? | legacy_form_pytest_raises.rs | 264 |
| H | ? | legacy_form_pytest_raises.rs | 274 |
| H | ? | legacy_form_pytest_raises.rs | 306 |
| H | ? | collection_literal_concatenation.rs | 79 |
| H | ? | collection_literal_concatenation.rs | 115 |
| H | ? | collection_literal_concatenation.rs | 117 |
| H | ? | collection_literal_concatenation.rs | 123 |
| H | ? | collection_literal_concatenation.rs | 125 |
| H | ? | collection_literal_concatenation.rs | 210 |
| H | ? | sort_dunder_slots.rs | 160 |
| H | ? | explicit_f_string_type_conversion.rs | 162 |
| H | ? | explicit_f_string_type_conversion.rs | 165 |
| H | ? | assert_with_print_message.rs | 69 |
| H | ? | assert_with_print_message.rs | 116 |
| H | ? | assert_with_print_message.rs | 130 |
| H | ? | assert_with_print_message.rs | 155 |
| H | ? | assert_with_print_message.rs | 240 |
| H | ? | unnecessary_nested_literal.rs | 115 |
| H | ? | unnecessary_nested_literal.rs | 125 |
| H | ? | fixes.rs | 58 |
| H | ? | fixes.rs | 65 |
| H | ? | fixes.rs | 66 |
| H | ? | fixes.rs | 69 |
| H | ? | fixes.rs | 72 |
| H | ? | fixes.rs | 121 |
| H | ? | fixes.rs | 128 |
| H | ? | fixes.rs | 129 |
| H | ? | fixes.rs | 134 |
| H | ? | fixes.rs | 137 |
| H | ? | fixes.rs | 139 |
| H | ? | fixes.rs | 140 |
| H | ? | fixes.rs | 184 |
| H | ? | fixes.rs | 185 |
| H | ? | fixes.rs | 186 |
| H | ? | fixes.rs | 202 |
| H | ? | fixes.rs | 205 |
| H | ? | fixes.rs | 267 |
| H | ? | fixes.rs | 268 |
| H | ? | fixes.rs | 279 |
| H | ? | fixes.rs | 287 |
| H | ? | fixes.rs | 401 |
| H | ? | fixes.rs | 434 |
| H | ? | fixes.rs | 452 |
| H | ? | fixes.rs | 468 |
| H | ? | fixes.rs | 484 |
| H | ? | fixes.rs | 515 |
| H | ? | fixes.rs | 517 |
| H | ? | fixes.rs | 518 |
| H | ? | fixes.rs | 519 |
| H | ? | fixes.rs | 520 |
| H | ? | fixes.rs | 552 |
| H | ? | fixes.rs | 554 |
| H | ? | fixes.rs | 589 |
| H | ? | fixes.rs | 611 |
| H | ? | fixes.rs | 633 |
| H | ? | fixes.rs | 697 |
| H | ? | fixes.rs | 703 |
| H | ? | fixes.rs | 716 |
| H | ? | fixes.rs | 741 |
| H | ? | fixes.rs | 749 |
| H | ? | fixes.rs | 759 |
| H | ? | fixes.rs | 789 |
| H | ? | fixes.rs | 790 |
| H | ? | fixes.rs | 882 |
| H | ? | fixes.rs | 887 |
| H | ? | fixes.rs | 902 |
| H | ? | fixes.rs | 905 |
| H | ? | fixes.rs | 908 |
| H | ? | fixes.rs | 923 |
| H | ? | fixes.rs | 950 |
| H | ? | fixes.rs | 951 |
| H | ? | fixes.rs | 952 |
| H | ? | fixes.rs | 953 |
| H | ? | fixes.rs | 958 |
| H | ? | fixes.rs | 961 |
| H | ? | fixes.rs | 965 |
| H | ? | fixes.rs | 989 |
| H | ? | fixes.rs | 991 |
| H | ? | unnecessary_dict_comprehension_for_iterable.rs | 208 |
| H | ? | unnecessary_dict_comprehension_for_iterable.rs | 213 |
| H | ? | unused_import.rs | 480 |
| H | ? | strings.rs | 714 |
| H | ? | strings.rs | 837 |
| H | ? | redefined_while_unused.rs | 293 |
| H | ? | cformat.rs | 34 |
| H | ? | banned_api.rs | 50 |
| H | ? | banned_api.rs | 77 |
| H | ? | banned_api.rs | 78 |
| H | ? | relative_imports.rs | 110 |
| H | ? | nested_min_max.rs | 148 |
| H | ? | nested_min_max.rs | 161 |
| H | ? | nested_min_max.rs | 203 |
| H | ? | manual_import_from.rs | 92 |
| H | ? | repeated_equality_comparison.rs | 203 |
| H | ? | modified_iterating_set.rs | 103 |
| H | ? | unnecessary_dunder_call.rs | 92 |
| H | ? | no_method_decorator.rs | 138 |
| H | ? | redeclared_assigned_name.rs | 87 |
| H | ? | len_test.rs | 113 |
| H | ? | xcom_pull_in_template_string.rs | 110 |
| H | ? | moved_to_provider_in_3.rs | 1199 |
| H | ? | moved_in_3_1.rs | 246 |
| H | ? | moved_in_3_1.rs | 262 |
| H | ? | suggested_to_move_to_provider_in_3.rs | 325 |
| H | ? | suggested_to_update_3_0.rs | 372 |
| H | ? | suggested_to_update_3_0.rs | 386 |
| H | ? | removal_in_3.rs | 1079 |
| H | ? | removal_in_3.rs | 1095 |
| H | ? | static_join_to_fstring.rs | 197 |
| H | ? | helpers.rs | 7 |
| H | ? | helpers.rs | 68 |
| H | ? | setattr_with_constant.rs | 74 |
| H | ? | setattr_with_constant.rs | 80 |
| H | ? | unused_loop_control_variable.rs | 136 |
| H | ? | delattr_with_constant.rs | 118 |
| H | ? | assert_false.rs | 66 |
| H | ? | blank_before_after_class.rs | 238 |
| H | ? | capitalized.rs | 101 |
| H | ? | indent.rs | 269 |
| H | ? | helpers.rs | 67 |
| H | ? | runtime_import_in_type_checking_block.rs | 224 |
| H | ? | runtime_import_in_type_checking_block.rs | 255 |
| H | ? | type_alias_quotes.rs | 191 |
| H | ? | typing_only_runtime_import.rs | 423 |
| H | ? | helpers.rs | 422 |
| H | ? | helpers.rs | 483 |
| H | ? | parametrize.rs | 439 |
| H | ? | parametrize.rs | 484 |
| H | ? | unittest_assert.rs | 166 |
| H | ? | unittest_assert.rs | 167 |
| H | ? | unittest_assert.rs | 175 |
| H | ? | unittest_assert.rs | 177 |
| H | ? | unittest_assert.rs | 297 |
| H | ? | unittest_assert.rs | 395 |
| H | ? | unittest_assert.rs | 444 |
| H | ? | assertion.rs | 707 |
| H | ? | assertion.rs | 710 |
| H | ? | unconventional_import_alias.rs | 81 |
| H | ? | codemods.rs | 83 |
| H | ? | codemods.rs | 154 |
| H | ? | mod.rs | 496 |
| H | ? | mod.rs | 254 |
| H | ? | mod.rs | 286 |
| H | ? | rule_set.rs | 286 |
| H | ? | suppression.rs | 431 |
| H | ? | suppression.rs | 482 |
| H | ? | suppression.rs | 483 |
| H | ? | suppression.rs | 899 |
| H | ? | suppression.rs | 920 |
| H | ? | suppression.rs | 928 |
| H | ? | suppression.rs | 935 |
| H | ? | suppression.rs | 982 |
| H | ? | suppression.rs | 983 |
| H | ? | suppression.rs | 1001 |
| H | ? | suppression.rs | 1009 |
| H | ? | suppression.rs | 3040 |
| H | ? | suppression.rs | 3067 |
| H | ? | rule_selector.rs | 76 |
| H | ? | rule_selector.rs | 274 |
| H | ? | source_kind.rs | 92 |
| H | ? | types.rs | 277 |
| H | ? | mod.rs | 821 |
| H | ? | rule_table.rs | 84 |
| H | ? | helpers.rs | 24 |
| H | ? | helpers.rs | 70 |
| H | ? | helpers.rs | 73 |
| H | ? | diagnostic.rs | 110 |
| H | ? | parser.rs | 797 |
| H | ? | parser.rs | 798 |
| H | ? | parser.rs | 891 |
| H | ? | parser.rs | 900 |
| H | ? | matcher.rs | 36 |
| H | ? | matcher.rs | 417 |
| H | ? | matcher.rs | 424 |
| H | ? | matcher.rs | 438 |
| H | ? | matcher.rs | 507 |
| H | ? | lib.rs | 731 |
| H | ? | options.rs | 1249 |
| H | ? | options.rs | 1256 |
| H | ? | options.rs | 1500 |
| H | ? | options.rs | 3055 |
| H | ? | configuration.rs | 238 |
| H | ? | configuration.rs | 241 |
| H | ? | configuration.rs | 277 |
| H | ? | configuration.rs | 323 |
| H | ? | configuration.rs | 375 |
| H | ? | configuration.rs | 2266 |
| H | ? | configuration.rs | 2275 |
| H | ? | configuration.rs | 2285 |
| H | ? | configuration.rs | 2289 |
| H | ? | pyproject.rs | 441 |
| H | ? | resolve.rs | 391 |
| H | ? | resolve.rs | 678 |
| H | ? | resolve.rs | 693 |
| H | ? | resolve.rs | 919 |
| H | ? | resolve.rs | 976 |
| H | ? | resolve.rs | 977 |
| H | ? | resolve.rs | 1287 |
| H | ? | resolve.rs | 2604 |
| H | ? | resolve.rs | 2647 |
| H | ? | resolve.rs | 2669 |
| H | ? | resolve.rs | 2770 |
| H | ? | resolve.rs | 3302 |
| H | ? | list.rs | 16 |
| H | ? | list.rs | 32 |
| H | ? | list.rs | 184 |
| H | ? | list.rs | 256 |
| H | ? | list.rs | 979 |
| H | ? | module_name.rs | 302 |
| H | ? | testing.rs | 247 |
| H | ? | testing.rs | 249 |
| H | ? | testing.rs | 314 |
| H | ? | testing.rs | 315 |
| H | ? | db.rs | 43 |
| H | ? | db.rs | 51 |
| H | ? | path.rs | 315 |
| H | ? | path.rs | 330 |
| H | ? | path.rs | 582 |
| H | ? | path.rs | 638 |
| H | ? | path.rs | 686 |
| H | ? | path.rs | 905 |
| H | ? | path.rs | 942 |
| H | ? | path.rs | 1106 |
| H | ? | path.rs | 1118 |
| H | ? | module.rs | 197 |
| H | ? | module.rs | 210 |
| H | ? | module.rs | 231 |
| H | ? | module.rs | 247 |
| H | ? | lib.rs | 212 |
| H | ? | lib.rs | 213 |
| H | ? | lib.rs | 232 |
| H | ? | lib.rs | 233 |
| H | ? | visibility.rs | 87 |
| H | ? | display_list.rs | 464 |
| H | ? | display_list.rs | 1420 |
| H | ? | display_list.rs | 1428 |
| H | ? | display_list.rs | 1482 |
| H | ? | display_list.rs | 1523 |
| H | ? | env_vars.rs | 32 |
| H | ? | env_vars.rs | 44 |
| H | ? | map_codes.rs | 72 |
| H | ? | map_codes.rs | 224 |
| H | ? | map_codes.rs | 500 |
| H | ? | rule_namespace.rs | 47 |
| H | ? | rule_namespace.rs | 80 |
| H | ? | rule_namespace.rs | 81 |
| H | ? | config.rs | 48 |
| H | ? | config.rs | 349 |
| H | ? | rule_code_prefix.rs | 22 |
| H | ? | cache_key.rs | 18 |
| H | ? | lib.rs | 85 |
| H | ? | lib.rs | 91 |
| H | ? | lib.rs | 120 |
| H | ? | mod.rs | 54 |
| H | ? | mod.rs | 58 |
| H | ? | recovery.rs | 77 |
| H | ? | recovery.rs | 98 |
| H | ? | recovery.rs | 102 |
| H | ? | recovery.rs | 113 |
| H | ? | recovery.rs | 128 |
| H | ? | recovery.rs | 140 |
| H | ? | recovery.rs | 187 |
| H | ? | recovery.rs | 200 |
| H | ? | interpolated_string.rs | 148 |
| H | ? | cursor.rs | 43 |
| H | ? | cursor.rs | 49 |
| H | ? | cursor.rs | 114 |
| H | ? | cursor.rs | 125 |
| H | ? | indentation.rs | 131 |
| H | ? | semantic_errors.rs | 2248 |
| H | ? | semantic_errors.rs | 2339 |
| H | ? | lib.rs | 338 |
| H | ? | ruff_formatter_idempotency.rs | 19 |
| H | ? | ruff_formatter_idempotency.rs | 23 |
| H | ? | ty_check_invalid_syntax.rs | 53 |
| H | ? | ty_check_invalid_syntax.rs | 135 |
| H | ? | ruff_formatter_validity.rs | 55 |
| H | ? | ruff_formatter_validity.rs | 64 |

---
*Сгенерировано GSC v0.6 · 2026-07-23T04:05:17.811055*