---
title: "GSC Audit: /tmp/gsc-learn/rich"
date: 2026-07-30
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/rich

**Дата:** 30.07.2026 04:10  
**Путь:** `/tmp/gsc-learn/rich`  
**Всего находок:** 123  
**CRITICAL:** 7 | **HIGH:** 10 | **MEDIUM:** 50 | **LOW:** 52

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 48 |
| GS003 | 34 |
| GS008 | 18 |
| GS005 | 7 |
| Хардкод IP адреса | 5 |
| GS007 | 3 |
| Bare except: | 2 |
| CVE-2026-56233: Path traversal | 1 |
| World-readable file: faq.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| World-readable file: asv.conf.json (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | box.py | 470 | Line 470: table.title = Text(f"box.{box_name}", style="magen |
| CRITICAL | GS005 | color.py | 614 | Line 614: table.add_row(color_cell, f"{color_number}", Text( |
| CRITICAL | GS005 | color.py | 618 | Line 618: color_cell, str(color_number), Text(f'"{name}"'),  |
| CRITICAL | GS005 | progress.py | 754 | Line 754: return Text(f"{data_speed:.1f}{suffix} it/s", styl |
| CRITICAL | GS005 | progress.py | 923 | Line 923: return Text(f"{data_speed}/s", style="progress.dat |
| CRITICAL | GS005 | prompt.py | 160 | Line 160: return Text(f"({default})", "prompt.default") |
| CRITICAL | GS005 | prompt.py | 356 | Line 356: return Text(f"({yes})" if default else f"({no})",  |
| HIGH | ? | make_width_tables.py | 14 |  |
| HIGH | ? | highlighter.py | 228 | Match:         "127.0.1.1 bar 192.168.1.4 2001:0db8:85a3:000 |
| HIGH | ? | logging.py | 264 | Match:     log.info("Listening on http://127.0.0.1:8080") |
| HIGH | ? | poetry.lock | 92 | Match: typing-extensions = {version = ">=3.10.0.0", markers  |
| HIGH | ? | poetry.lock | 430 | Match: qa = ["flake8 (==5.0.4)", "mypy (==0.971)", "types-se |
| HIGH | ? | poetry.lock | 609 | Match: qa = ["flake8 (==5.0.4)", "mypy (==0.971)", "types-se |
| HIGH | ? | faq.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | asv.conf.json | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | traceback.py | 319 |
| M | ? | logging.py | 298 |
| M | ? | color.py | 365 |
| M | ? | color.py | 368 |
| M | ? | color.py | 371 |
| M | ? | color.py | 374 |
| M | ? | color.py | 377 |
| M | ? | color.py | 493 |
| M | ? | color.py | 499 |
| M | ? | color.py | 504 |
| M | ? | color.py | 508 |
| M | ? | color.py | 520 |
| M | ? | color.py | 546 |
| M | ? | color.py | 549 |
| M | ? | color.py | 557 |
| M | ? | color.py | 560 |
| M | ? | color.py | 573 |
| M | ? | prompt.py | 222 |
| M | ? | pretty.py | 198 |
| M | ? | pretty.py | 203 |
| M | ? | pretty.py | 516 |
| M | ? | pretty.py | 522 |
| M | ? | pretty.py | 524 |
| M | ? | syntax.py | 510 |
| M | ? | live.py | 71 |
| M | ? | _win32_console.py | 435 |
| M | ? | _win32_console.py | 436 |
| M | ? | _win32_console.py | 565 |
| M | ? | markdown.py | 279 |
| M | ? | markdown.py | 291 |
| M | ? | markdown.py | 303 |
| M | ? | markdown.py | 326 |
| M | ? | markdown.py | 353 |
| M | ? | markdown.py | 632 |
| M | ? | segment.py | 168 |
| M | ? | progress.py | 1091 |
| M | ? | text.py | 907 |
| M | ? | text.py | 924 |
| M | ? | text.py | 940 |
| M | ? | text.py | 1079 |
| M | ? | _pick.py | 13 |
| M | ? | _ratio.py | 123 |
| M | ? | console.py | 1143 |
| M | ? | console.py | 1939 |
| M | ? | console.py | 2204 |
| M | ? | console.py | 2268 |
| M | ? | traceback.py | 342 |
| M | ? | traceback.py | 798 |
| M | ? | logging.py | 148 |
| M | ? | logging.py | 149 |
| H | ? | make_width_tables.py | 14 |
| L | GS003 | _ratio.py | 153 |
| L | GS003 | _timer.py | 19 |
| L | GS003 | _win32_console.py | 661 |
| L | GS003 | _windows.py | 69 |
| L | GS003 | _windows.py | 71 |
| L | GS003 | _wrap.py | 86 |
| L | GS003 | abc.py | 25 |
| L | GS003 | abc.py | 26 |
| L | GS003 | abc.py | 32 |
| L | GS003 | abc.py | 33 |
| L | GS003 | ansi.py | 236 |
| L | GS003 | default_styles.py | 196 |
| L | GS003 | markup.py | 250 |
| L | GS003 | padding.py | 140 |
| L | GS003 | pretty.py | 1009 |
| L | GS003 | pretty.py | 1015 |
| L | GS003 | prompt.py | 376 |
| L | GS003 | prompt.py | 377 |
| L | GS003 | prompt.py | 386 |
| L | GS003 | prompt.py | 387 |
| L | GS003 | prompt.py | 390 |
| L | GS003 | prompt.py | 397 |
| L | GS003 | prompt.py | 400 |
| L | GS003 | scope.py | 78 |
| L | GS003 | scope.py | 89 |
| L | GS003 | scope.py | 92 |
| L | GS003 | styled.py | 42 |
| L | GS003 | theme.py | 116 |
| L | GS003 | traceback.py | 906 |
| L | GS003 | make_emoji.py | 4 |
| L | GS003 | profile_divide.py | 14 |
| L | GS003 | profile_pretty.py | 20 |
| L | GS003 | profile_pretty.py | 21 |
| L | GS003 | profile_pretty.py | 23 |
| L | GS008 | snippets.py | 1 |
| L | GS008 | _emoji_codes.py | 1 |
| L | GS008 | _export_format.py | 1 |
| L | GS008 | _export_format.py | 20 |
| L | GS008 | _palettes.py | 5 |
| L | GS008 | _palettes.py | 27 |
| L | GS008 | _palettes.py | 50 |
| L | GS008 | _spinners.py | 22 |
| L | GS008 | _versions.py | 1 |
| L | GS008 | _win32_console.py | 24 |
| L | GS008 | syntax.py | 59 |
| L | GS008 | terminal_theme.py | 32 |
| L | GS008 | terminal_theme.py | 57 |
| L | GS008 | terminal_theme.py | 81 |
| L | GS008 | terminal_theme.py | 105 |
| L | GS008 | terminal_theme.py | 130 |
| L | GS008 | themes.py | 5 |
| L | GS008 | traceback.py | 50 |
| H | ? | highlighter.py | 228 |
| H | ? | logging.py | 264 |
| H | ? | poetry.lock | 92 |
| H | ? | poetry.lock | 430 |
| H | ? | poetry.lock | 609 |
| H | ? | faq.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | ? | asv.conf.json | 0 |
| C | GS005 | box.py | 470 |
| C | GS005 | color.py | 614 |
| C | GS005 | color.py | 618 |
| C | GS005 | progress.py | 754 |
| C | GS005 | progress.py | 923 |
| C | GS005 | prompt.py | 160 |
| C | GS005 | prompt.py | 356 |
| I | GS007 | __main__.py | 23 |
| I | GS007 | cells.py | 338 |
| I | GS007 | palette.py | 89 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-30T04:10:03.282928*