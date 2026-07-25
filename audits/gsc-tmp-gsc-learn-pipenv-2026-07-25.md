---
title: "GSC Audit: /tmp/gsc-learn/pipenv"
date: 2026-07-25
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pipenv

**Дата:** 25.07.2026 04:02  
**Путь:** `/tmp/gsc-learn/pipenv`  
**Всего находок:** 771  
**CRITICAL:** 4 | **HIGH:** 24 | **MEDIUM:** 296 | **LOW:** 443

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 214 |
| GS003 | 127 |
| Outdated dependency pattern | 50 |
| Синхронный код в async | 21 |
| GS008 | 18 |
| Python: File upload without content-type validation | 6 |
| CVE-2026-37270: Hardcoded credential | 6 |
| Generic code smell #24 | 5 |
| Generic code smell #27 | 5 |
| Generic code smell #30 | 5 |
| Generic code smell #33 | 5 |
| Generic code smell #36 | 5 |
| Generic code smell #39 | 5 |
| Generic code smell #42 | 5 |
| Generic code smell #45 | 5 |
| Generic code smell #48 | 5 |
| Generic code smell #51 | 5 |
| Generic code smell #54 | 5 |
| Generic code smell #57 | 5 |
| Generic code smell #60 | 5 |
| Generic code smell #63 | 5 |
| Generic code smell #66 | 5 |
| Generic code smell #69 | 5 |
| Generic code smell #72 | 5 |
| Generic code smell #75 | 5 |
| Generic code smell #78 | 5 |
| Generic code smell #81 | 5 |
| Generic code smell #84 | 5 |
| Generic code smell #87 | 5 |
| Generic code smell #90 | 5 |
| Generic code smell #93 | 5 |
| Generic code smell #96 | 5 |
| Generic code smell #99 | 5 |
| Generic code smell #102 | 5 |
| Generic code smell #105 | 5 |
| Generic code smell #108 | 5 |
| Generic code smell #111 | 5 |
| Generic code smell #114 | 5 |
| Generic code smell #117 | 5 |
| Generic code smell #120 | 5 |
| Generic code smell #123 | 5 |
| Generic code smell #126 | 5 |
| Generic code smell #129 | 5 |
| Generic code smell #132 | 5 |
| Generic code smell #135 | 5 |
| Generic code smell #138 | 5 |
| Generic code smell #141 | 5 |
| Generic code smell #144 | 5 |
| Generic code smell #147 | 5 |
| Generic code smell #150 | 5 |
| Generic code smell #153 | 5 |
| Generic code smell #156 | 5 |
| Generic code smell #159 | 5 |
| Generic code smell #162 | 5 |
| Generic code smell #165 | 5 |
| Generic code smell #168 | 5 |
| Generic code smell #171 | 5 |
| Generic code smell #174 | 5 |
| Generic code smell #177 | 5 |
| Generic code smell #180 | 5 |
| Generic code smell #183 | 5 |
| Generic code smell #186 | 5 |
| Generic code smell #189 | 5 |
| Generic code smell #192 | 5 |
| Generic code smell #195 | 5 |
| Generic code smell #198 | 5 |
| CVE-2026-56318: Information disclosure | 5 |
| Хардкод IP адреса | 4 |
| GS004 | 4 |
| CVE-2026-56219: Authentication bypass | 3 |
| GS015 | 3 |
| GS012 | 3 |
| CVE-2026-56233: Privilege escalation | 2 |
| CVE-2026-56413: Command injection | 2 |
| eval() or exec() usage | 2 |
| CVE-2026-56233: Path traversal | 1 |
| GS001 | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS005 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | configuration.py | 247 |  |
| CRITICAL | ? | shell.py | 242 |  |
| CRITICAL | GS001 | auth.py | 471 | Found: Password: ")
        return username, password, True
 |
| CRITICAL | GS005 | exceptions.py | 968 | Line 968: message += Text(f" for {req}") |
| HIGH | ? | configuration.py | 273 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | package_finder.py | 248 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | wheel.py | 386 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | wheel.py | 608 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | link.py | 306 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | release.py | 153 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | session.py | 312 |  |
| HIGH | ? | session.py | 323 |  |
| HIGH | ? | internet.py | 24 |  |
| HIGH | ? | debug.py | 132 |  |
| HIGH | ? | base_command.py | 241 |  |
| HIGH | ? | base_command.py | 242 |  |
| HIGH | ? | Makefile | 183 | Match: 	pipenv run pypi-server run --server $(SERVER) -v --h |
| HIGH | ? | run-tests.bat | 6 | Match: cmd /c start pipenv run pypi-server run -v --host=0.0 |
| HIGH | ? | session.py | 71 | Match:     ("*", "127.0.0.0/8", "*"), |
| HIGH | ? | run-tests.sh | 61 | Match: pipenv run pypi-server run -v --host=0.0.0.0 --port=8 |
| HIGH | ? | environment.py | 782 | Match:                 exec(code, {"__file__": activate_this |
| HIGH | ? | virtualenv.py | 688 | Match:         exec(code, {"__file__": str(activate_path)}) |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | environment.py | 782 | Line 782: exec(code, {"__file__": activate_this}) |
| HIGH | GS004 | configuration.py | 247 | Line 247: subprocess.check_call(f'{editor} "{fname}"', shell |
| HIGH | GS004 | shell.py | 242 | Line 242: result = subprocess.run(cmd_string, shell=True, en |
| HIGH | GS004 | virtualenv.py | 688 | Line 688: exec(code, {"__file__": str(activate_path)}) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| L | ? | get-pipenv.py | 6025 |
| L | ? | get-pipenv.py | 12953 |
| L | ? | get-pipenv.py | 26113 |
| L | ? | get-pipenv.py | 26177 |
| L | ? | base.py | 32 |
| M | ? | build_env.py | 571 |
| M | ? | search.py | 84 |
| M | ? | download.py | 139 |
| M | ? | install.py | 596 |
| M | ? | install.py | 685 |
| M | ? | install.py | 814 |
| M | ? | debug.py | 68 |
| M | ? | wheel.py | 156 |
| M | ? | wheel.py | 157 |
| M | ? | cache.py | 41 |
| M | ? | cache.py | 125 |
| M | ? | _distutils.py | 82 |
| M | ? | _distutils.py | 87 |
| M | ? | _distutils.py | 88 |
| M | ? | requirements.py | 54 |
| M | ? | requirements.py | 88 |
| M | ? | requirements.py | 112 |
| M | ? | requirements.py | 119 |
| M | ? | requirements.py | 131 |
| M | ? | requirements.py | 209 |
| M | ? | candidates.py | 66 |
| M | ? | candidates.py | 94 |
| M | ? | candidates.py | 304 |
| M | ? | candidates.py | 308 |
| M | ? | candidates.py | 312 |
| M | ? | candidates.py | 317 |
| M | ? | candidates.py | 318 |
| M | ? | factory.py | 258 |
| M | ? | factory.py | 259 |
| M | ? | factory.py | 288 |
| M | ? | factory.py | 298 |
| M | ? | factory.py | 303 |
| M | ? | factory.py | 411 |
| M | ? | factory.py | 590 |
| M | ? | factory.py | 702 |
| M | ? | factory.py | 803 |
| M | ? | resolver.py | 59 |
| M | ? | resolver.py | 201 |
| M | ? | resolver.py | 314 |
| M | ? | resolver.py | 134 |
| M | ? | resolver.py | 237 |
| M | ? | resolver.py | 315 |
| M | ? | resolver.py | 324 |
| M | ? | resolver.py | 422 |
| M | ? | resolver.py | 451 |
| M | ? | resolver.py | 536 |
| M | ? | resolver.py | 541 |
| M | ? | pkg_resources.py | 109 |
| M | ? | exceptions.py | 95 |
| M | ? | exceptions.py | 97 |
| M | ? | exceptions.py | 678 |
| M | ? | exceptions.py | 845 |
| M | ? | session.py | 220 |
| M | ? | cache.py | 58 |
| M | ? | lazy_wheel.py | 59 |
| M | ? | download.py | 173 |
| M | ? | download.py | 225 |
| M | ? | download.py | 281 |
| M | ? | download.py | 335 |
| M | ? | auth.py | 436 |
| M | ? | auth.py | 447 |
| M | ? | auth.py | 557 |
| M | ? | xmlrpc.py | 40 |
| M | ? | xmlrpc.py | 55 |
| M | ? | subversion.py | 66 |
| M | ? | subversion.py | 168 |
| M | ? | git.py | 226 |
| M | ? | git.py | 517 |
| M | ? | pylock.py | 38 |
| M | ? | pylock.py | 173 |
| M | ? | pylock.py | 217 |
| M | ? | subprocess.py | 149 |
| M | ? | subprocess.py | 150 |
| M | ? | subprocess.py | 164 |
| M | ? | subprocess.py | 187 |
| M | ? | filesystem.py | 25 |
| M | ? | temp_dir.py | 144 |
| M | ? | temp_dir.py | 149 |
| M | ? | urls.py | 23 |
| M | ? | unpacking.py | 371 |
| M | ? | direct_url_helpers.py | 27 |
| M | ? | direct_url_helpers.py | 48 |
| M | ? | direct_url_helpers.py | 59 |
| M | ? | direct_url_helpers.py | 65 |
| M | ? | direct_url_helpers.py | 84 |
| M | ? | logging.py | 186 |
| M | ? | logging.py | 189 |
| M | ? | logging.py | 211 |
| M | ? | logging.py | 213 |
| M | ? | spinners.py | 60 |
| M | ? | spinners.py | 99 |
| M | ? | progress_bars.py | 38 |
| M | ? | parser.py | 60 |
| M | ? | parser.py | 160 |
| M | ? | parser.py | 162 |
| M | ? | parser.py | 216 |
| M | ? | parser.py | 276 |
| M | ? | parser.py | 303 |
| M | ? | parser.py | 336 |
| M | ? | base_command.py | 93 |
| M | ? | base_command.py | 110 |
| M | ? | req_command.py | 96 |
| M | ? | req_command.py | 168 |
| M | ? | command_context.py | 16 |
| M | ? | command_context.py | 26 |
| M | ? | index_command.py | 84 |
| M | ? | index_command.py | 96 |
| M | ? | index_command.py | 186 |
| M | ? | req_install.py | 87 |
| M | ? | req_install.py | 101 |
| M | ? | req_install.py | 241 |
| M | ? | req_install.py | 251 |
| M | ? | req_install.py | 265 |
| M | ? | req_install.py | 314 |
| M | ? | req_install.py | 336 |
| M | ? | req_install.py | 338 |
| M | ? | req_install.py | 378 |
| M | ? | req_install.py | 379 |
| M | ? | req_install.py | 380 |
| M | ? | req_install.py | 399 |
| M | ? | req_install.py | 469 |
| M | ? | req_install.py | 476 |
| M | ? | req_install.py | 483 |
| M | ? | req_install.py | 495 |
| M | ? | req_install.py | 525 |
| M | ? | req_install.py | 528 |
| M | ? | req_install.py | 570 |
| M | ? | req_install.py | 581 |
| M | ? | req_install.py | 621 |
| M | ? | req_install.py | 626 |
| M | ? | req_install.py | 649 |
| M | ? | req_install.py | 650 |
| M | ? | req_install.py | 657 |
| M | ? | req_install.py | 677 |
| M | ? | req_install.py | 690 |
| M | ? | req_install.py | 697 |
| M | ? | req_install.py | 707 |
| M | ? | req_install.py | 778 |
| M | ? | req_install.py | 808 |
| M | ? | req_install.py | 809 |
| M | ? | constructors.py | 89 |
| M | ? | constructors.py | 94 |
| M | ? | req_uninstall.py | 73 |
| M | ? | req_uninstall.py | 534 |
| M | ? | req_file.py | 186 |
| M | ? | req_file.py | 507 |
| M | ? | req_file.py | 519 |
| M | ? | req_set.py | 41 |
| M | ? | req_set.py | 45 |
| M | ? | configuration.py | 132 |
| M | ? | configuration.py | 165 |
| M | ? | configuration.py | 186 |
| M | ? | configuration.py | 378 |
| M | ? | collector.py | 184 |
| M | ? | package_finder.py | 419 |
| M | ? | package_finder.py | 422 |
| M | ? | package_finder.py | 424 |
| M | ? | package_finder.py | 795 |
| M | ? | package_finder.py | 961 |
| M | ? | package_finder.py | 1031 |
| M | ? | build_tracker.py | 38 |
| M | ? | build_tracker.py | 107 |
| M | ? | metadata_editable.py | 40 |
| M | ? | wheel_editable.py | 23 |
| M | ? | wheel.py | 23 |
| M | ? | wheel.py | 91 |
| M | ? | wheel.py | 639 |
| M | ? | prepare.py | 85 |
| M | ? | prepare.py | 172 |
| M | ? | prepare.py | 324 |
| M | ? | prepare.py | 398 |
| M | ? | prepare.py | 474 |
| M | ? | prepare.py | 504 |
| M | ? | prepare.py | 577 |
| M | ? | prepare.py | 583 |
| M | ? | prepare.py | 584 |
| M | ? | prepare.py | 585 |
| M | ? | prepare.py | 636 |
| M | ? | prepare.py | 671 |
| M | ? | prepare.py | 672 |
| M | ? | prepare.py | 701 |
| M | ? | prepare.py | 714 |
| M | ? | prepare.py | 735 |
| M | ? | prepare.py | 736 |
| M | ? | freeze.py | 167 |
| M | ? | installed.py | 24 |
| M | ? | sdist.py | 29 |
| M | ? | sdist.py | 63 |
| M | ? | sdist.py | 79 |
| M | ? | sdist.py | 105 |
| M | ? | sdist.py | 115 |
| M | ? | wheel.py | 33 |
| M | ? | wheel.py | 34 |
| M | ? | wheel_builder.py | 56 |
| M | ? | wheel_builder.py | 57 |
| M | ? | wheel_builder.py | 59 |
| M | ? | wheel_builder.py | 64 |
| M | ? | wheel_builder.py | 81 |
| M | ? | wheel_builder.py | 158 |
| M | ? | wheel_builder.py | 159 |
| M | ? | wheel_builder.py | 160 |
| M | ? | wheel_builder.py | 226 |
| M | ? | wheel_builder.py | 244 |
| M | ? | installation_report.py | 16 |
| M | ? | link.py | 65 |
| M | ? | link.py | 101 |
| M | ? | link.py | 436 |
| M | ? | __pip-runner__.py | 43 |
| M | ? | __pip-runner__.py | 49 |
| M | ? | virtualenv.py | 462 |
| M | ? | fileutils.py | 39 |
| M | ? | requirementslib.py | 84 |
| M | ? | toml.py | 66 |
| M | ? | project.py | 851 |
| H | ? | configuration.py | 273 |
| H | ? | package_finder.py | 248 |
| H | ? | wheel.py | 386 |
| H | ? | wheel.py | 608 |
| H | ? | link.py | 306 |
| H | ? | release.py | 153 |
| H | ? | session.py | 312 |
| H | ? | session.py | 323 |
| H | ? | internet.py | 24 |
| H | ? | debug.py | 132 |
| H | ? | base_command.py | 241 |
| H | ? | base_command.py | 242 |
| M | ? | misc.py | 469 |
| M | ? | misc.py | 472 |
| M | ? | requirements.py | 44 |
| M | ? | requirements.py | 49 |
| M | ? | requirements.py | 52 |
| C | ? | configuration.py | 247 |
| C | ? | shell.py | 242 |
| M | ? | misc.py | 469 |
| M | ? | misc.py | 472 |
| M | ? | requirements.py | 44 |
| M | ? | requirements.py | 49 |
| M | ? | requirements.py | 52 |
| M | ? | project.py | 937 |
| C | GS001 | auth.py | 471 |
| L | GS003 | benchmark.py | 224 |
| L | GS003 | benchmark.py | 250 |
| L | GS003 | benchmark.py | 254 |
| L | GS003 | benchmark.py | 256 |
| L | GS003 | benchmark.py | 258 |
| L | GS003 | benchmark.py | 260 |
| L | GS003 | benchmark.py | 262 |
| L | GS003 | benchmark.py | 282 |
| L | GS003 | benchmark.py | 285 |
| L | GS003 | benchmark.py | 289 |
| L | GS003 | benchmark.py | 291 |
| L | GS003 | benchmark.py | 299 |
| L | GS003 | benchmark.py | 300 |
| L | GS003 | benchmark.py | 302 |
| L | GS003 | benchmark.py | 304 |
| L | GS003 | benchmark.py | 306 |
| L | GS003 | benchmark.py | 308 |
| L | GS003 | benchmark.py | 313 |
| L | GS003 | benchmark.py | 317 |
| L | GS003 | benchmark.py | 333 |
| L | GS003 | benchmark.py | 337 |
| L | GS003 | benchmark.py | 342 |
| L | GS003 | benchmark.py | 351 |
| L | GS003 | benchmark.py | 365 |
| L | GS003 | benchmark.py | 368 |
| L | GS003 | benchmark.py | 370 |
| L | GS003 | benchmark.py | 372 |
| L | GS003 | benchmark.py | 376 |
| L | GS003 | benchmark.py | 383 |
| L | GS003 | benchmark.py | 388 |
| L | GS003 | benchmark.py | 392 |
| L | GS003 | benchmark.py | 396 |
| L | GS003 | benchmark.py | 400 |
| L | GS003 | benchmark.py | 402 |
| L | GS003 | benchmark.py | 406 |
| L | GS003 | benchmark.py | 408 |
| L | GS003 | benchmark.py | 412 |
| L | GS003 | benchmark.py | 416 |
| L | GS003 | benchmark.py | 420 |
| L | GS003 | benchmark.py | 424 |
| L | GS003 | benchmark.py | 443 |
| L | GS003 | benchmark.py | 473 |
| L | GS003 | benchmark.py | 489 |
| L | GS003 | benchmark.py | 527 |
| L | GS003 | benchmark.py | 528 |
| L | GS003 | benchmark.py | 529 |
| L | GS003 | benchmark.py | 546 |
| L | GS003 | benchmark.py | 547 |
| L | GS003 | benchmark.py | 549 |
| L | GS003 | benchmark.py | 551 |
| L | GS003 | benchmark.py | 552 |
| L | GS003 | benchmark.py | 613 |
| L | GS003 | get-pipenv.py | 35 |
| L | GS003 | command.py | 273 |
| L | GS003 | command.py | 665 |
| L | GS003 | command.py | 780 |
| L | GS003 | exceptions.py | 26 |
| L | GS003 | help.py | 11 |
| L | GS003 | help.py | 12 |
| L | GS003 | help.py | 13 |
| L | GS003 | help.py | 14 |
| L | GS003 | help.py | 15 |
| L | GS003 | help.py | 16 |
| L | GS003 | help.py | 17 |
| L | GS003 | help.py | 18 |
| L | GS003 | help.py | 19 |
| L | GS003 | help.py | 20 |
| L | GS003 | help.py | 24 |
| L | GS003 | help.py | 26 |
| L | GS003 | help.py | 29 |
| L | GS003 | help.py | 31 |
| L | GS003 | help.py | 35 |
| L | GS003 | help.py | 36 |
| L | GS003 | help.py | 38 |
| L | GS003 | help.py | 39 |
| L | GS003 | help.py | 40 |
| L | GS003 | help.py | 42 |
| L | GS003 | help.py | 43 |
| L | GS003 | help.py | 44 |
| L | GS003 | help.py | 45 |
| L | GS003 | help.py | 47 |
| L | GS003 | help.py | 48 |
| L | GS003 | help.py | 49 |
| L | GS003 | help.py | 50 |
| L | GS003 | help.py | 53 |
| L | GS003 | help.py | 54 |
| L | GS003 | help.py | 55 |
| L | GS003 | help.py | 56 |
| L | GS003 | help.py | 59 |
| L | GS003 | help.py | 60 |
| L | GS003 | help.py | 61 |
| L | GS003 | help.py | 62 |
| L | GS003 | help.py | 63 |
| L | GS003 | help.py | 65 |
| L | GS003 | help.py | 66 |
| L | GS003 | help.py | 67 |
| L | GS003 | help.py | 69 |
| L | GS003 | help.py | 70 |
| L | GS003 | help.py | 71 |
| L | GS003 | help.py | 73 |
| L | GS003 | help.py | 74 |
| L | GS003 | help.py | 75 |
| L | GS003 | help.py | 76 |
| L | GS003 | help.py | 78 |
| L | GS003 | help.py | 79 |
| L | GS003 | help.py | 80 |
| L | GS003 | autocompletion.py | 65 |
| L | GS003 | autocompletion.py | 73 |
| L | GS003 | autocompletion.py | 105 |
| L | GS003 | autocompletion.py | 111 |
| L | GS003 | autocompletion.py | 127 |
| L | GS003 | parser.py | 223 |
| L | GS003 | completion.py | 130 |
| L | GS003 | misc.py | 226 |
| L | GS003 | pep508checker.py | 39 |
| L | GS003 | requirements.py | 51 |
| L | GS003 | requirements.py | 95 |
| L | GS003 | requirements.py | 122 |
| L | GS003 | requirements.py | 145 |
| L | GS003 | exceptions.py | 20 |
| L | GS003 | exceptions.py | 54 |
| L | GS003 | exceptions.py | 72 |
| L | GS003 | exceptions.py | 90 |
| L | GS003 | release.py | 21 |
| L | GS003 | release.py | 153 |
| L | GS003 | release.py | 157 |
| L | GS003 | release.py | 288 |
| L | GS008 | command.py | 22 |
| L | GS008 | command.py | 32 |
| L | GS008 | environments.py | 77 |
| L | GS008 | environments.py | 517 |
| L | GS008 | environments.py | 518 |
| L | GS008 | status_codes.py | 1 |
| L | GS008 | status_codes.py | 2 |
| L | GS008 | status_codes.py | 3 |
| L | GS008 | status_codes.py | 4 |
| L | GS008 | status_codes.py | 6 |
| L | GS008 | hashes.py | 21 |
| L | GS008 | constants.py | 2 |
| L | GS008 | constants.py | 3 |
| L | GS008 | constants.py | 4 |
| L | GS008 | constants.py | 5 |
| L | GS008 | constants.py | 29 |
| L | GS008 | constants.py | 39 |
| L | GS008 | constants.py | 50 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | urls.py | 1 |
| H | ? | Makefile | 183 |
| H | ? | run-tests.bat | 6 |
| H | ? | session.py | 71 |
| H | ? | run-tests.sh | 61 |
| M | ? | benchmark.py | 312 |
| M | ? | benchmark.py | 313 |
| M | ? | benchmark.py | 314 |
| M | ? | benchmark.py | 391 |
| M | ? | benchmark.py | 394 |
| M | ? | benchmark.py | 592 |
| M | ? | pyproject.py | 23 |
| M | ? | pyproject.py | 59 |
| M | ? | factory.py | 773 |
| M | ? | factory.py | 776 |
| M | ? | factory.py | 778 |
| M | ? | exceptions.py | 213 |
| M | ? | exceptions.py | 221 |
| M | ? | exceptions.py | 230 |
| M | ? | exceptions.py | 239 |
| M | ? | exceptions.py | 896 |
| M | ? | misc.py | 297 |
| M | ? | cmdoptions.py | 556 |
| M | ? | cmdoptions.py | 976 |
| M | ? | cmdoptions.py | 979 |
| M | ? | cmdoptions.py | 980 |
| M | ? | cmdoptions.py | 995 |
| M | ? | cmdoptions.py | 996 |
| M | ? | cmdoptions.py | 997 |
| M | ? | constructors.py | 334 |
| M | ? | metadata_editable.py | 32 |
| M | ? | wheel_editable.py | 28 |
| M | ? | wheel.py | 28 |
| M | ? | metadata.py | 31 |
| M | ? | sdist.py | 92 |
| M | ? | install.py | 567 |
| M | ? | exceptions.py | 389 |
| M | ? | exceptions.py | 390 |
| M | ? | pylock.py | 286 |
| M | ? | pylock.py | 297 |
| M | ? | pylock.py | 373 |
| M | ? | shell.py | 176 |
| M | ? | shell.py | 181 |
| M | ? | shell.py | 185 |
| M | ? | pipfile.py | 97 |
| M | ? | pipfile.py | 117 |
| M | ? | dependencies.py | 1043 |
| M | ? | resolver.py | 1538 |
| M | ? | resolver.py | 1539 |
| M | ? | constants.py | 36 |
| M | ? | command.py | 551 |
| M | ? | command.py | 553 |
| M | ? | command.py | 620 |
| M | ? | options.py | 262 |
| M | ? | options.py | 814 |
| H | ? | environment.py | 782 |
| H | ? | virtualenv.py | 688 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | environment.py | 782 |
| H | GS004 | configuration.py | 247 |
| H | GS004 | shell.py | 242 |
| H | GS004 | virtualenv.py | 688 |
| C | GS005 | exceptions.py | 968 |
| s | GS009 |  | 0 |
| L | GS012 | configuration.py | 273 |
| L | GS012 | wheel.py | 386 |
| L | GS012 | wheel.py | 608 |
| M | ? | benchmark.py | 353 |
| M | ? | benchmark.py | 429 |
| M | ? | auth.py | 140 |
| M | ? | auth.py | 156 |
| M | ? | main_parser.py | 103 |
| M | ? | audit.py | 28 |
| M | ? | audit.py | 261 |
| M | ? | shell.py | 186 |
| M | ? | shell.py | 192 |
| M | ? | shell.py | 196 |
| M | ? | shell.py | 202 |
| M | ? | shell.py | 208 |
| M | ? | shell.py | 242 |
| M | ? | scan.py | 234 |
| M | ? | scan.py | 288 |
| M | ? | check.py | 152 |
| M | ? | check.py | 210 |
| M | ? | processes.py | 76 |
| M | ? | funktools.py | 193 |
| M | ? | funktools.py | 216 |
| M | ? | funktools.py | 338 |

---
*Сгенерировано GSC v0.6 · 2026-07-25T04:02:18.932462*