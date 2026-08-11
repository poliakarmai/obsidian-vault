---
title: "GSC Audit: /tmp/gsc-learn/pip"
date: 2026-08-04
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pip

**Дата:** 04.08.2026 04:04  
**Путь:** `/tmp/gsc-learn/pip`  
**Всего находок:** 289  
**CRITICAL:** 4 | **HIGH:** 16 | **MEDIUM:** 246 | **LOW:** 19

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 215 |
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
| GS001 | 2 |
| CVE-2026-56233: Path traversal | 1 |
| CVE-2026-56413: Command injection | 1 |
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
| CRITICAL | GS001 | pyproject.toml | 216 | Found: "py310" |
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
| HIGH | ? | session.py | 292 |  |
| HIGH | ? | session.py | 303 |  |
| HIGH | ? | debug.py | 131 |  |
| HIGH | ? | base_command.py | 249 |  |
| HIGH | ? | base_command.py | 250 |  |
| HIGH | ? | session.py | 75 | Match:     ("*", "127.0.0.0/8", "*"), |
| HIGH | ? | .readthedocs-custom-redirects.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | configuration.py | 248 | Line 248: subprocess.check_call(f'{editor} "{fname}"', shell |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | noxfile.py | 154 |
| M | ? | search.py | 84 |
| M | ? | download.py | 143 |
| M | ? | install.py | 596 |
| M | ? | install.py | 685 |
| M | ? | install.py | 814 |
| M | ? | debug.py | 67 |
| M | ? | wheel.py | 161 |
| M | ? | wheel.py | 162 |
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
| M | ? | candidates.py | 299 |
| M | ? | candidates.py | 303 |
| M | ? | candidates.py | 307 |
| M | ? | candidates.py | 312 |
| M | ? | candidates.py | 313 |
| M | ? | factory.py | 262 |
| M | ? | factory.py | 272 |
| M | ? | factory.py | 277 |
| M | ? | factory.py | 377 |
| M | ? | factory.py | 556 |
| M | ? | factory.py | 668 |
| M | ? | factory.py | 790 |
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
| M | ? | pkg_resources.py | 114 |
| M | ? | exceptions.py | 97 |
| M | ? | exceptions.py | 99 |
| M | ? | exceptions.py | 810 |
| M | ? | exceptions.py | 977 |
| M | ? | session.py | 195 |
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
| M | ? | req_command.py | 175 |
| M | ? | command_context.py | 16 |
| M | ? | command_context.py | 26 |
| M | ? | index_command.py | 84 |
| M | ? | index_command.py | 96 |
| M | ? | index_command.py | 191 |
| M | ? | req_install.py | 83 |
| M | ? | req_install.py | 96 |
| M | ? | req_install.py | 230 |
| M | ? | req_install.py | 240 |
| M | ? | req_install.py | 254 |
| M | ? | req_install.py | 303 |
| M | ? | req_install.py | 325 |
| M | ? | req_install.py | 327 |
| M | ? | req_install.py | 367 |
| M | ? | req_install.py | 368 |
| M | ? | req_install.py | 369 |
| M | ? | req_install.py | 388 |
| M | ? | req_install.py | 458 |
| M | ? | req_install.py | 465 |
| M | ? | req_install.py | 472 |
| M | ? | req_install.py | 484 |
| M | ? | req_install.py | 524 |
| M | ? | req_install.py | 527 |
| M | ? | req_install.py | 565 |
| M | ? | req_install.py | 576 |
| M | ? | req_install.py | 616 |
| M | ? | req_install.py | 621 |
| M | ? | req_install.py | 644 |
| M | ? | req_install.py | 645 |
| M | ? | req_install.py | 652 |
| M | ? | req_install.py | 672 |
| M | ? | req_install.py | 685 |
| M | ? | req_install.py | 692 |
| M | ? | req_install.py | 702 |
| M | ? | req_install.py | 781 |
| M | ? | req_install.py | 791 |
| M | ? | req_install.py | 792 |
| M | ? | constructors.py | 88 |
| M | ? | constructors.py | 93 |
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
| M | ? | collector.py | 186 |
| M | ? | package_finder.py | 401 |
| M | ? | package_finder.py | 404 |
| M | ? | package_finder.py | 406 |
| M | ? | package_finder.py | 756 |
| M | ? | package_finder.py | 941 |
| M | ? | package_finder.py | 1010 |
| M | ? | package_finder.py | 1101 |
| M | ? | build_tracker.py | 38 |
| M | ? | build_tracker.py | 107 |
| M | ? | metadata_editable.py | 40 |
| M | ? | wheel_editable.py | 23 |
| M | ? | wheel.py | 23 |
| M | ? | wheel.py | 90 |
| M | ? | wheel.py | 636 |
| M | ? | prepare.py | 90 |
| M | ? | prepare.py | 177 |
| M | ? | prepare.py | 446 |
| M | ? | prepare.py | 520 |
| M | ? | prepare.py | 596 |
| M | ? | prepare.py | 626 |
| M | ? | prepare.py | 699 |
| M | ? | prepare.py | 705 |
| M | ? | prepare.py | 706 |
| M | ? | prepare.py | 707 |
| M | ? | prepare.py | 758 |
| M | ? | prepare.py | 815 |
| M | ? | prepare.py | 816 |
| M | ? | prepare.py | 845 |
| M | ? | prepare.py | 858 |
| M | ? | prepare.py | 880 |
| M | ? | prepare.py | 881 |
| M | ? | freeze.py | 167 |
| M | ? | installed.py | 24 |
| M | ? | sdist.py | 34 |
| M | ? | sdist.py | 72 |
| M | ? | sdist.py | 97 |
| M | ? | sdist.py | 98 |
| M | ? | sdist.py | 127 |
| M | ? | sdist.py | 137 |
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
| M | ? | wheel_builder.py | 230 |
| M | ? | wheel_builder.py | 248 |
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
| H | ? | session.py | 292 |
| H | ? | session.py | 303 |
| H | ? | debug.py | 131 |
| H | ? | base_command.py | 249 |
| H | ? | base_command.py | 250 |
| M | ? | misc.py | 508 |
| M | ? | misc.py | 511 |
| C | ? | configuration.py | 248 |
| M | ? | misc.py | 508 |
| M | ? | misc.py | 511 |
| C | GS001 | pyproject.toml | 216 |
| C | GS001 | auth.py | 486 |
| L | GS003 | autocompletion.py | 68 |
| L | GS003 | autocompletion.py | 76 |
| L | GS003 | autocompletion.py | 108 |
| L | GS003 | autocompletion.py | 114 |
| L | GS003 | autocompletion.py | 130 |
| L | GS003 | parser.py | 223 |
| L | GS003 | completion.py | 130 |
| L | GS003 | misc.py | 265 |
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
| H | ? | session.py | 75 |
| M | ? | noxfile.py | 61 |
| M | ? | noxfile.py | 201 |
| M | ? | pyproject.py | 23 |
| M | ? | pyproject.py | 59 |
| M | ? | factory.py | 760 |
| M | ? | factory.py | 763 |
| M | ? | factory.py | 765 |
| M | ? | exceptions.py | 215 |
| M | ? | exceptions.py | 223 |
| M | ? | exceptions.py | 232 |
| M | ? | exceptions.py | 241 |
| M | ? | exceptions.py | 1028 |
| M | ? | misc.py | 336 |
| M | ? | cmdoptions.py | 600 |
| M | ? | cmdoptions.py | 1065 |
| M | ? | constructors.py | 317 |
| M | ? | metadata_editable.py | 32 |
| M | ? | wheel_editable.py | 28 |
| M | ? | wheel.py | 28 |
| M | ? | metadata.py | 31 |
| M | ? | sdist.py | 114 |
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
*Сгенерировано GSC v0.6 · 2026-08-04T04:04:13.323402*