---
title: "GSC Audit: /tmp/gsc-learn/pip"
date: 2026-07-25
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pip

**Дата:** 25.07.2026 04:00  
**Путь:** `/tmp/gsc-learn/pip`  
**Всего находок:** 289  
**CRITICAL:** 3 | **HIGH:** 16 | **MEDIUM:** 247 | **LOW:** 19

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 216 |
| Outdated dependency pattern | 21 |
| GS003 | 9 |
| GS008 | 7 |
| Python: File upload without content-type validation | 6 |
| Синхронный код в async | 6 |
| GS015 | 3 |
| GS012 | 3 |
| CVE-2026-56219: Authentication bypass | 2 |
| CVE-2026-56233: Privilege escalation | 2 |
| CVE-2026-56318: Information disclosure | 2 |
| CVE-2026-37270: Hardcoded credential | 2 |
| CVE-2026-56233: Path traversal | 1 |
| CVE-2026-56413: Command injection | 1 |
| GS001 | 1 |
| Хардкод IP адреса | 1 |
| World-readable file: .readthedocs-custom-redirects.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| GS004 | 1 |
| GS005 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | configuration.py | 248 |  |
| CRITICAL | GS001 | auth.py | 486 | Found: Password: ")
        return username, password, True
 |
| CRITICAL | GS005 | exceptions.py | 1100 | Line 1100: message += Text(f" for {req}") |
| HIGH | ? | noxfile.py | 497 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | configuration.py | 274 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | package_finder.py | 230 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | wheel.py | 383 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | wheel.py | 605 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | link.py | 351 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | session.py | 320 |  |
| HIGH | ? | session.py | 331 |  |
| HIGH | ? | debug.py | 131 |  |
| HIGH | ? | base_command.py | 249 |  |
| HIGH | ? | base_command.py | 250 |  |
| HIGH | ? | session.py | 74 | Match:     ("*", "127.0.0.0/8", "*"), |
| HIGH | ? | .readthedocs-custom-redirects.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | configuration.py | 248 | Line 248: subprocess.check_call(f'{editor} "{fname}"', shell |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | noxfile.py | 154 |
| M | ? | search.py | 84 |
| M | ? | download.py | 142 |
| M | ? | install.py | 600 |
| M | ? | install.py | 689 |
| M | ? | install.py | 818 |
| M | ? | debug.py | 67 |
| M | ? | wheel.py | 159 |
| M | ? | wheel.py | 160 |
| M | ? | cache.py | 41 |
| M | ? | cache.py | 125 |
| M | ? | virtual.py | 89 |
| M | ? | _distutils.py | 67 |
| M | ? | _distutils.py | 72 |
| M | ? | _distutils.py | 73 |
| M | ? | requirements.py | 54 |
| M | ? | requirements.py | 88 |
| M | ? | requirements.py | 112 |
| M | ? | requirements.py | 119 |
| M | ? | requirements.py | 131 |
| M | ? | requirements.py | 209 |
| M | ? | candidates.py | 65 |
| M | ? | candidates.py | 93 |
| M | ? | candidates.py | 300 |
| M | ? | candidates.py | 304 |
| M | ? | candidates.py | 308 |
| M | ? | candidates.py | 313 |
| M | ? | candidates.py | 314 |
| M | ? | factory.py | 258 |
| M | ? | factory.py | 259 |
| M | ? | factory.py | 288 |
| M | ? | factory.py | 298 |
| M | ? | factory.py | 303 |
| M | ? | factory.py | 411 |
| M | ? | factory.py | 590 |
| M | ? | factory.py | 702 |
| M | ? | factory.py | 803 |
| M | ? | resolver.py | 60 |
| M | ? | resolver.py | 61 |
| M | ? | resolver.py | 210 |
| M | ? | resolver.py | 323 |
| M | ? | resolver.py | 134 |
| M | ? | resolver.py | 237 |
| M | ? | resolver.py | 315 |
| M | ? | resolver.py | 324 |
| M | ? | resolver.py | 422 |
| M | ? | resolver.py | 451 |
| M | ? | resolver.py | 536 |
| M | ? | resolver.py | 541 |
| M | ? | pkg_resources.py | 109 |
| M | ? | exceptions.py | 97 |
| M | ? | exceptions.py | 99 |
| M | ? | exceptions.py | 810 |
| M | ? | exceptions.py | 977 |
| M | ? | session.py | 223 |
| M | ? | cache.py | 58 |
| M | ? | lazy_wheel.py | 59 |
| M | ? | download.py | 193 |
| M | ? | download.py | 247 |
| M | ? | download.py | 328 |
| M | ? | download.py | 382 |
| M | ? | auth.py | 451 |
| M | ? | auth.py | 462 |
| M | ? | auth.py | 574 |
| M | ? | xmlrpc.py | 40 |
| M | ? | xmlrpc.py | 55 |
| M | ? | utils.py | 131 |
| M | ? | utils.py | 134 |
| M | ? | utils.py | 187 |
| M | ? | utils.py | 200 |
| M | ? | subversion.py | 66 |
| M | ? | subversion.py | 168 |
| M | ? | git.py | 225 |
| M | ? | git.py | 520 |
| M | ? | pylock.py | 38 |
| M | ? | pylock.py | 185 |
| M | ? | pylock.py | 229 |
| M | ? | subprocess.py | 150 |
| M | ? | subprocess.py | 151 |
| M | ? | subprocess.py | 165 |
| M | ? | subprocess.py | 188 |
| M | ? | filesystem.py | 25 |
| M | ? | temp_dir.py | 143 |
| M | ? | temp_dir.py | 148 |
| M | ? | urls.py | 26 |
| M | ? | unpacking.py | 349 |
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
| M | ? | progress_bars.py | 40 |
| M | ? | parser.py | 60 |
| M | ? | parser.py | 160 |
| M | ? | parser.py | 162 |
| M | ? | parser.py | 216 |
| M | ? | parser.py | 276 |
| M | ? | parser.py | 303 |
| M | ? | parser.py | 336 |
| M | ? | base_command.py | 93 |
| M | ? | base_command.py | 110 |
| M | ? | req_command.py | 101 |
| M | ? | req_command.py | 173 |
| M | ? | command_context.py | 16 |
| M | ? | command_context.py | 26 |
| M | ? | index_command.py | 84 |
| M | ? | index_command.py | 96 |
| M | ? | index_command.py | 190 |
| M | ? | req_install.py | 86 |
| M | ? | req_install.py | 100 |
| M | ? | req_install.py | 242 |
| M | ? | req_install.py | 252 |
| M | ? | req_install.py | 266 |
| M | ? | req_install.py | 315 |
| M | ? | req_install.py | 337 |
| M | ? | req_install.py | 339 |
| M | ? | req_install.py | 379 |
| M | ? | req_install.py | 380 |
| M | ? | req_install.py | 381 |
| M | ? | req_install.py | 400 |
| M | ? | req_install.py | 470 |
| M | ? | req_install.py | 477 |
| M | ? | req_install.py | 484 |
| M | ? | req_install.py | 496 |
| M | ? | req_install.py | 536 |
| M | ? | req_install.py | 539 |
| M | ? | req_install.py | 581 |
| M | ? | req_install.py | 592 |
| M | ? | req_install.py | 632 |
| M | ? | req_install.py | 637 |
| M | ? | req_install.py | 660 |
| M | ? | req_install.py | 661 |
| M | ? | req_install.py | 668 |
| M | ? | req_install.py | 688 |
| M | ? | req_install.py | 701 |
| M | ? | req_install.py | 708 |
| M | ? | req_install.py | 718 |
| M | ? | req_install.py | 797 |
| M | ? | req_install.py | 807 |
| M | ? | req_install.py | 808 |
| M | ? | constructors.py | 89 |
| M | ? | constructors.py | 94 |
| M | ? | req_uninstall.py | 73 |
| M | ? | req_uninstall.py | 539 |
| M | ? | req_file.py | 186 |
| M | ? | req_file.py | 509 |
| M | ? | req_file.py | 521 |
| M | ? | req_set.py | 41 |
| M | ? | req_set.py | 45 |
| M | ? | configuration.py | 131 |
| M | ? | configuration.py | 164 |
| M | ? | configuration.py | 185 |
| M | ? | configuration.py | 377 |
| M | ? | collector.py | 189 |
| M | ? | package_finder.py | 401 |
| M | ? | package_finder.py | 404 |
| M | ? | package_finder.py | 406 |
| M | ? | package_finder.py | 749 |
| M | ? | package_finder.py | 914 |
| M | ? | package_finder.py | 983 |
| M | ? | build_tracker.py | 38 |
| M | ? | build_tracker.py | 107 |
| M | ? | metadata_editable.py | 40 |
| M | ? | wheel_editable.py | 23 |
| M | ? | wheel.py | 23 |
| M | ? | wheel.py | 90 |
| M | ? | wheel.py | 636 |
| M | ? | prepare.py | 89 |
| M | ? | prepare.py | 176 |
| M | ? | prepare.py | 440 |
| M | ? | prepare.py | 514 |
| M | ? | prepare.py | 590 |
| M | ? | prepare.py | 620 |
| M | ? | prepare.py | 693 |
| M | ? | prepare.py | 699 |
| M | ? | prepare.py | 700 |
| M | ? | prepare.py | 701 |
| M | ? | prepare.py | 752 |
| M | ? | prepare.py | 808 |
| M | ? | prepare.py | 809 |
| M | ? | prepare.py | 838 |
| M | ? | prepare.py | 851 |
| M | ? | prepare.py | 872 |
| M | ? | prepare.py | 873 |
| M | ? | freeze.py | 167 |
| M | ? | installed.py | 24 |
| M | ? | sdist.py | 34 |
| M | ? | sdist.py | 69 |
| M | ? | sdist.py | 94 |
| M | ? | sdist.py | 95 |
| M | ? | sdist.py | 124 |
| M | ? | sdist.py | 134 |
| M | ? | wheel.py | 33 |
| M | ? | wheel.py | 34 |
| M | ? | wheel_builder.py | 59 |
| M | ? | wheel_builder.py | 60 |
| M | ? | wheel_builder.py | 62 |
| M | ? | wheel_builder.py | 67 |
| M | ? | wheel_builder.py | 84 |
| M | ? | wheel_builder.py | 161 |
| M | ? | wheel_builder.py | 162 |
| M | ? | wheel_builder.py | 163 |
| M | ? | wheel_builder.py | 229 |
| M | ? | wheel_builder.py | 247 |
| M | ? | installation_report.py | 16 |
| M | ? | link.py | 108 |
| M | ? | link.py | 144 |
| M | ? | __pip-runner__.py | 43 |
| M | ? | __pip-runner__.py | 49 |
| M | ? | update-rtd-redirects.py | 119 |
| H | ? | noxfile.py | 497 |
| H | ? | configuration.py | 274 |
| H | ? | package_finder.py | 230 |
| H | ? | wheel.py | 383 |
| H | ? | wheel.py | 605 |
| H | ? | link.py | 351 |
| H | ? | session.py | 320 |
| H | ? | session.py | 331 |
| H | ? | debug.py | 131 |
| H | ? | base_command.py | 249 |
| H | ? | base_command.py | 250 |
| M | ? | misc.py | 485 |
| M | ? | misc.py | 488 |
| C | ? | configuration.py | 248 |
| M | ? | misc.py | 485 |
| M | ? | misc.py | 488 |
| C | GS001 | auth.py | 486 |
| L | GS003 | autocompletion.py | 68 |
| L | GS003 | autocompletion.py | 76 |
| L | GS003 | autocompletion.py | 108 |
| L | GS003 | autocompletion.py | 114 |
| L | GS003 | autocompletion.py | 130 |
| L | GS003 | parser.py | 223 |
| L | GS003 | completion.py | 130 |
| L | GS003 | misc.py | 242 |
| L | GS003 | check_version.py | 38 |
| L | GS008 | status_codes.py | 1 |
| L | GS008 | status_codes.py | 2 |
| L | GS008 | status_codes.py | 3 |
| L | GS008 | status_codes.py | 4 |
| L | GS008 | status_codes.py | 6 |
| L | GS008 | status_codes.py | 7 |
| L | GS008 | hashes.py | 21 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | urls.py | 1 |
| H | ? | session.py | 74 |
| M | ? | noxfile.py | 61 |
| M | ? | noxfile.py | 201 |
| M | ? | pyproject.py | 23 |
| M | ? | pyproject.py | 59 |
| M | ? | factory.py | 773 |
| M | ? | factory.py | 776 |
| M | ? | factory.py | 778 |
| M | ? | exceptions.py | 215 |
| M | ? | exceptions.py | 223 |
| M | ? | exceptions.py | 232 |
| M | ? | exceptions.py | 241 |
| M | ? | exceptions.py | 1028 |
| M | ? | misc.py | 313 |
| M | ? | cmdoptions.py | 600 |
| M | ? | cmdoptions.py | 1028 |
| M | ? | constructors.py | 327 |
| M | ? | metadata_editable.py | 32 |
| M | ? | wheel_editable.py | 28 |
| M | ? | wheel.py | 28 |
| M | ? | metadata.py | 31 |
| M | ? | sdist.py | 111 |
| H | ? | .readthedocs-custom-redirects.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | GS004 | configuration.py | 248 |
| C | GS005 | exceptions.py | 1100 |
| s | GS009 |  | 0 |
| L | GS012 | configuration.py | 274 |
| L | GS012 | wheel.py | 383 |
| L | GS012 | wheel.py | 605 |
| M | ? | build-project.py | 25 |
| M | ? | build-project.py | 44 |
| M | ? | build-project.py | 58 |
| M | ? | auth.py | 138 |
| M | ? | auth.py | 171 |
| M | ? | main_parser.py | 102 |

---
*Сгенерировано GSC v0.6 · 2026-07-25T04:00:56.190223*