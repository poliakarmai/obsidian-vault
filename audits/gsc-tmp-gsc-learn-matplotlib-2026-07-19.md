---
title: "GSC Audit: /tmp/gsc-learn/matplotlib"
date: 2026-07-19
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/matplotlib

**Дата:** 19.07.2026 04:02  
**Путь:** `/tmp/gsc-learn/matplotlib`  
**Всего находок:** 1025  
**CRITICAL:** 1 | **HIGH:** 88 | **MEDIUM:** 77 | **LOW:** 858

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 105 |
| Python: assert in production | 60 |
| CVE-2026-56233: Path traversal | 40 |
| GS012 | 34 |
| Python: File upload without content-type validation | 27 |
| Generic code smell #24 | 12 |
| Generic code smell #27 | 12 |
| Generic code smell #30 | 12 |
| Generic code smell #33 | 12 |
| Generic code smell #36 | 12 |
| Generic code smell #39 | 12 |
| Generic code smell #42 | 12 |
| Generic code smell #45 | 12 |
| Generic code smell #48 | 12 |
| Generic code smell #51 | 12 |
| Generic code smell #54 | 12 |
| Generic code smell #57 | 12 |
| Generic code smell #60 | 12 |
| Generic code smell #63 | 12 |
| Generic code smell #66 | 12 |
| Generic code smell #69 | 12 |
| Generic code smell #72 | 12 |
| Generic code smell #75 | 12 |
| Generic code smell #78 | 12 |
| Generic code smell #81 | 12 |
| Generic code smell #84 | 12 |
| Generic code smell #87 | 12 |
| Generic code smell #90 | 12 |
| Generic code smell #93 | 12 |
| Generic code smell #96 | 12 |
| Generic code smell #99 | 12 |
| Generic code smell #102 | 12 |
| Generic code smell #105 | 12 |
| Generic code smell #108 | 12 |
| Generic code smell #111 | 12 |
| Generic code smell #114 | 12 |
| Generic code smell #117 | 12 |
| Generic code smell #120 | 12 |
| Generic code smell #123 | 12 |
| Generic code smell #126 | 12 |
| Generic code smell #129 | 12 |
| Generic code smell #132 | 12 |
| Generic code smell #135 | 12 |
| Generic code smell #138 | 12 |
| Generic code smell #141 | 12 |
| Generic code smell #144 | 12 |
| Generic code smell #147 | 12 |
| Generic code smell #150 | 12 |
| Generic code smell #153 | 12 |
| Generic code smell #156 | 12 |
| Generic code smell #159 | 12 |
| Generic code smell #162 | 12 |
| Generic code smell #165 | 12 |
| Generic code smell #168 | 12 |
| Generic code smell #171 | 12 |
| Generic code smell #174 | 12 |
| Generic code smell #177 | 12 |
| Generic code smell #180 | 12 |
| Generic code smell #183 | 12 |
| Generic code smell #186 | 12 |
| Generic code smell #189 | 12 |
| Generic code smell #192 | 12 |
| Generic code smell #195 | 12 |
| Generic code smell #198 | 12 |
| GS008 | 11 |
| CVE-2026-37270: Hardcoded credential | 9 |
| Синхронный код в async | 7 |
| eval() or exec() usage | 5 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 4 |
| GS004 | 4 |
| GS001 | 1 |
| Хардкод IP адреса | 1 |
| Outdated dependency pattern | 1 |
| World-readable file: .meeseeksdev.yml (664) | 1 |
| World-readable file: environment.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: azure-pipelines.yml (664) | 1 |
| World-readable file: .yamllint.yml (664) | 1 |
| World-readable file: .appveyor.yml (664) | 1 |
| GS002 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | gh_api.py | 56 | Found: Password: ")

    auth_request = {
      " |
| HIGH | ? | image.py | 662 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | image.py | 1722 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | compare.py | 494 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | compare.py | 541 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | animation.py | 510 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | animation.py | 921 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | animation.py | 1322 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | animation.py | 1392 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _backend_pdf_ps.py | 133 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_pdf.py | 1629 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_svg.py | 975 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_svg.py | 986 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_pgf.py | 656 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 101 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 114 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 132 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 151 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 184 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 213 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 231 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 247 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 289 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_cairo.py | 300 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | backend_webagg_core.py | 282 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | colors.py | 1043 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | colors.py | 1679 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | colors.py | 2150 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | conf.py | 292 |  |
| HIGH | ? | conf.py | 305 |  |
| HIGH | ? | gallery_order.py | 21 |  |
| HIGH | ? | gallery_order.py | 22 |  |
| HIGH | ? | gallery_order.py | 23 |  |
| HIGH | ? | gallery_order.py | 24 |  |
| HIGH | ? | gallery_order.py | 26 |  |
| HIGH | ? | gallery_order.py | 28 |  |
| HIGH | ? | gallery_order.py | 29 |  |
| HIGH | ? | gallery_order.py | 30 |  |
| HIGH | ? | gallery_order.py | 32 |  |
| HIGH | ? | gallery_order.py | 33 |  |
| HIGH | ? | gallery_order.py | 35 |  |
| HIGH | ? | gallery_order.py | 36 |  |
| HIGH | ? | gallery_order.py | 38 |  |
| HIGH | ? | gallery_order.py | 39 |  |
| HIGH | ? | gallery_order.py | 40 |  |
| HIGH | ? | gallery_order.py | 41 |  |
| HIGH | ? | gallery_order.py | 43 |  |
| HIGH | ? | gallery_order.py | 44 |  |
| HIGH | ? | gallery_order.py | 45 |  |
| HIGH | ? | gallery_order.py | 46 |  |
| HIGH | ? | gallery_order.py | 48 |  |
| HIGH | ? | gallery_order.py | 50 |  |
| HIGH | ? | gallery_order.py | 51 |  |
| HIGH | ? | gallery_order.py | 55 |  |
| HIGH | ? | gallery_order.py | 56 |  |
| HIGH | ? | gallery_order.py | 57 |  |
| HIGH | ? | gallery_order.py | 59 |  |
| HIGH | ? | gallery_order.py | 63 |  |
| HIGH | ? | gallery_order.py | 64 |  |
| HIGH | ? | gallery_order.py | 65 |  |
| HIGH | ? | gallery_order.py | 66 |  |
| HIGH | ? | gallery_order.py | 67 |  |
| HIGH | ? | images.py | 51 |  |
| HIGH | ? | images.py | 188 |  |
| HIGH | ? | constrainedlayout_guide.py | 209 |  |
| HIGH | ? | constrainedlayout_guide.py | 231 |  |
| HIGH | ? | make_icons.py | 109 |  |
| HIGH | ? | cache_zenodo_svg.py | 168 |  |
| HIGH | ? | gh_api.py | 79 |  |
| HIGH | ? | gh_api.py | 107 |  |
| HIGH | ? | gh_api.py | 133 |  |
| HIGH | ? | gh_api.py | 275 |  |
| HIGH | ? | rcsetup.py | 1531 | Match:         default="127.0.0.1", |
| HIGH | ? | rcsetup.py | 821 | Match:     without using eval(). |
| HIGH | ? | qt_compat.py | 145 | Match:     obj.exec() if hasattr(obj, "exec") else obj.exec_ |
| HIGH | ? | _formlayout.py | 576 | Match:     _app.exec() |
| HIGH | ? | _formlayout.py | 582 | Match:     _app.exec() |
| HIGH | ? | _formlayout.py | 592 | Match:     _app.exec() |
| HIGH | ? | .meeseeksdev.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | environment.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | azure-pipelines.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .yamllint.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .appveyor.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | docutils.conf | 0 | File docutils.conf has permissions -rw-rw-r-- — readable by  |
| HIGH | GS004 | backend_qt.py | 480 | Line 480: qt_compat._exec(event_loop) |
| HIGH | GS004 | backend_qt.py | 661 | Line 661: qt_compat._exec(qapp) |
| HIGH | GS004 | qt_compat.py | 143 | Line 143: def _exec(obj): |
| HIGH | GS004 | triage_tests.py | 347 | Line 347: sys.exit(_exec(app)) |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| L | ? | widgets.py | 2085 |
| L | ? | widgets.py | 4411 |
| L | ? | animation.pyi | 163 |
| L | ? | figure.pyi | 131 |
| L | ? | backend_pdf.py | 1081 |
| L | ? | backend_pdf.py | 1082 |
| L | ? | backend_pdf.py | 1085 |
| L | ? | backend_pdf.py | 1347 |
| L | ? | backend_pdf.py | 1355 |
| L | ? | backend_pdf.py | 1357 |
| L | ? | backend_pdf.py | 1359 |
| L | ? | pyplot.py | 1704 |
| M | ? | cbook.py | 2106 |
| M | ? | cbook.py | 2107 |
| M | ? | cbook.py | 2108 |
| M | ? | transforms.py | 1556 |
| M | ? | decorators.py | 239 |
| M | ? | _triinterpolate.py | 1234 |
| M | ? | _triinterpolate.py | 1313 |
| M | ? | _triinterpolate.py | 1314 |
| M | ? | _triinterpolate.py | 1494 |
| M | ? | _triinterpolate.py | 1496 |
| M | ? | _triinterpolate.py | 1498 |
| M | ? | _triinterpolate.py | 1501 |
| M | ? | _triinterpolate.py | 1531 |
| M | ? | _triinterpolate.py | 1532 |
| M | ? | _triinterpolate.py | 1534 |
| M | ? | _triinterpolate.py | 1556 |
| M | ? | _triinterpolate.py | 1557 |
| M | ? | ticker.py | 2560 |
| M | ? | dviread.py | 213 |
| M | ? | dviread.py | 1117 |
| M | ? | _mathtext.py | 1764 |
| M | ? | _mathtext.py | 1827 |
| M | ? | _mathtext.py | 1859 |
| M | ? | legend.py | 982 |
| M | ? | legend.py | 1182 |
| M | ? | deprecation.py | 281 |
| M | ? | deprecation.py | 284 |
| M | ? | deprecation.py | 374 |
| M | ? | deprecation.py | 454 |
| M | ? | rcsetup.py | 953 |
| M | ? | spines.py | 126 |
| M | ? | spines.py | 309 |
| M | ? | spines.py | 377 |
| M | ? | backend_gtk4.py | 259 |
| M | ? | backend_pdf.py | 873 |
| M | ? | backend_pdf.py | 1551 |
| M | ? | backend_pdf.py | 2108 |
| M | ? | backend_pdf.py | 2111 |
| M | ? | backend_pdf.py | 2112 |
| M | ? | backend_pdf.py | 2113 |
| M | ? | backend_pdf.py | 2114 |
| M | ? | backend_pdf.py | 2115 |
| M | ? | backend_pdf.py | 2116 |
| M | ? | backend_pdf.py | 2271 |
| M | ? | backend_pdf.py | 2504 |
| M | ? | backend_webagg.py | 169 |
| M | ? | backend_ps.py | 861 |
| M | ? | backend_ps.py | 864 |
| M | ? | backend_ps.py | 865 |
| M | ? | backend_ps.py | 866 |
| M | ? | backend_ps.py | 867 |
| M | ? | backend_ps.py | 868 |
| M | ? | backend_ps.py | 869 |
| M | ? | backend_svg.py | 208 |
| M | ? | backend_svg.py | 209 |
| M | ? | backend_svg.py | 212 |
| M | ? | backend_webagg_core.py | 492 |
| M | ? | backend_webagg_core.py | 493 |
| M | ? | _formlayout.py | 110 |
| M | ? | _formlayout.py | 168 |
| H | ? | image.py | 662 |
| H | ? | image.py | 1722 |
| H | ? | compare.py | 494 |
| H | ? | compare.py | 541 |
| H | ? | animation.py | 510 |
| H | ? | animation.py | 921 |
| H | ? | animation.py | 1322 |
| H | ? | animation.py | 1392 |
| H | ? | _backend_pdf_ps.py | 133 |
| H | ? | backend_pdf.py | 1629 |
| H | ? | backend_svg.py | 975 |
| H | ? | backend_svg.py | 986 |
| H | ? | backend_pgf.py | 656 |
| H | ? | backend_cairo.py | 101 |
| H | ? | backend_cairo.py | 114 |
| H | ? | backend_cairo.py | 132 |
| H | ? | backend_cairo.py | 151 |
| H | ? | backend_cairo.py | 184 |
| H | ? | backend_cairo.py | 213 |
| H | ? | backend_cairo.py | 231 |
| H | ? | backend_cairo.py | 247 |
| H | ? | backend_cairo.py | 289 |
| H | ? | backend_cairo.py | 300 |
| H | ? | backend_webagg_core.py | 282 |
| H | ? | colors.py | 1043 |
| H | ? | colors.py | 1679 |
| H | ? | colors.py | 2150 |
| H | ? | conf.py | 292 |
| H | ? | conf.py | 305 |
| H | ? | gallery_order.py | 21 |
| H | ? | gallery_order.py | 22 |
| H | ? | gallery_order.py | 23 |
| H | ? | gallery_order.py | 24 |
| H | ? | gallery_order.py | 26 |
| H | ? | gallery_order.py | 28 |
| H | ? | gallery_order.py | 29 |
| H | ? | gallery_order.py | 30 |
| H | ? | gallery_order.py | 32 |
| H | ? | gallery_order.py | 33 |
| H | ? | gallery_order.py | 35 |
| H | ? | gallery_order.py | 36 |
| H | ? | gallery_order.py | 38 |
| H | ? | gallery_order.py | 39 |
| H | ? | gallery_order.py | 40 |
| H | ? | gallery_order.py | 41 |
| H | ? | gallery_order.py | 43 |
| H | ? | gallery_order.py | 44 |
| H | ? | gallery_order.py | 45 |
| H | ? | gallery_order.py | 46 |
| H | ? | gallery_order.py | 48 |
| H | ? | gallery_order.py | 50 |
| H | ? | gallery_order.py | 51 |
| H | ? | gallery_order.py | 55 |
| H | ? | gallery_order.py | 56 |
| H | ? | gallery_order.py | 57 |
| H | ? | gallery_order.py | 59 |
| H | ? | gallery_order.py | 63 |
| H | ? | gallery_order.py | 64 |
| H | ? | gallery_order.py | 65 |
| H | ? | gallery_order.py | 66 |
| H | ? | gallery_order.py | 67 |
| H | ? | images.py | 51 |
| H | ? | images.py | 188 |
| H | ? | constrainedlayout_guide.py | 209 |
| H | ? | constrainedlayout_guide.py | 231 |
| H | ? | make_icons.py | 109 |
| H | ? | cache_zenodo_svg.py | 168 |
| H | ? | gh_api.py | 79 |
| H | ? | gh_api.py | 107 |
| H | ? | gh_api.py | 133 |
| H | ? | gh_api.py | 275 |
| M | ? | cbook.py | 2366 |
| M | ? | backend_bases.py | 3302 |
| M | ? | backend_bases.py | 3304 |
| M | ? | backend_bases.py | 3328 |
| M | ? | backend_bases.py | 3330 |
| M | ? | animation.py | 525 |
| M | ? | animation.py | 526 |
| M | ? | animation.py | 659 |
| M | ? | animation.py | 660 |
| C | GS001 | gh_api.py | 56 |
| L | GS003 | check_version_number.py | 15 |
| L | GS003 | check_wheel_licenses.py | 24 |
| L | GS003 | export_sdist_name.py | 18 |
| L | GS003 | vendor_schemas.py | 36 |
| L | GS003 | vendor_schemas.py | 45 |
| L | GS003 | vendor_schemas.py | 47 |
| L | GS003 | conf.py | 33 |
| L | GS003 | conf.py | 64 |
| L | GS003 | conf.py | 74 |
| L | GS003 | conf.py | 175 |
| L | GS003 | conf.py | 176 |
| L | GS003 | math_symbol_table.py | 134 |
| L | GS003 | math_symbol_table.py | 144 |
| L | GS003 | math_symbol_table.py | 149 |
| L | GS003 | math_symbol_table.py | 152 |
| L | GS003 | images.py | 52 |
| L | GS003 | lifecycle.py | 79 |
| L | GS003 | lifecycle.py | 237 |
| L | GS003 | color_cycle.py | 39 |
| L | GS003 | autoscale.py | 42 |
| L | GS003 | autoscale.py | 153 |
| L | GS003 | autoscale.py | 155 |
| L | GS003 | autoscale.py | 170 |
| L | GS003 | autoscale.py | 201 |
| L | GS003 | autoscale.py | 202 |
| L | GS003 | autoscale.py | 203 |
| L | GS003 | autoscale.py | 204 |
| L | GS003 | axes_scales.py | 95 |
| L | GS003 | axes_scales.py | 192 |
| L | GS003 | axes_scales.py | 194 |
| L | GS003 | axes_scales.py | 201 |
| L | GS003 | axes_scales.py | 213 |
| L | GS003 | axes_scales.py | 215 |
| L | GS003 | axes_scales.py | 216 |
| L | GS003 | axes_scales.py | 217 |
| L | GS003 | axes_scales.py | 219 |
| L | GS003 | axes_scales.py | 220 |
| L | GS003 | axes_units.py | 279 |
| L | GS003 | mosaic.py | 98 |
| L | GS003 | colormap-manipulation.py | 46 |
| L | GS003 | colormap-manipulation.py | 59 |
| L | GS003 | colormap-manipulation.py | 61 |
| L | GS003 | colormap-manipulation.py | 62 |
| L | GS003 | colormap-manipulation.py | 67 |
| L | GS003 | colormap-manipulation.py | 78 |
| L | GS003 | colormap-manipulation.py | 80 |
| L | GS003 | customizing.py | 123 |
| L | GS003 | artist.py | 1893 |
| L | GS003 | artist.py | 1972 |
| L | GS003 | artist.py | 1974 |
| L | GS003 | backend_webagg.py | 57 |
| L | GS003 | backend_webagg.py | 59 |
| L | GS003 | backend_webagg.py | 277 |
| L | GS003 | backend_webagg.py | 293 |
| L | GS003 | _formlayout.py | 571 |
| L | GS003 | contour.py | 218 |
| L | GS003 | contour.py | 219 |
| L | GS003 | contour.py | 221 |
| L | GS003 | autoclose_prs.py | 41 |
| L | GS003 | autoclose_prs.py | 54 |
| L | GS003 | check_typehints.py | 149 |
| L | GS003 | check_typehints.py | 164 |
| L | GS003 | check_typehints.py | 205 |
| L | GS003 | check_typehints.py | 214 |
| L | GS003 | check_typehints.py | 223 |
| L | GS003 | check_typehints.py | 228 |
| L | GS003 | check_typehints.py | 237 |
| L | GS003 | check_typehints.py | 247 |
| L | GS003 | check_typehints.py | 259 |
| L | GS003 | check_typehints.py | 264 |
| L | GS003 | check_typehints.py | 273 |
| L | GS003 | check_typehints.py | 317 |
| L | GS003 | check_typehints.py | 318 |
| L | GS003 | gh_api.py | 14 |
| L | GS003 | gh_api.py | 51 |
| L | GS003 | gh_api.py | 106 |
| L | GS003 | gh_api.py | 130 |
| L | GS003 | gh_api.py | 132 |
| L | GS003 | gh_api.py | 186 |
| L | GS003 | github_stats.py | 214 |
| L | GS003 | github_stats.py | 286 |
| L | GS003 | memleak.py | 41 |
| L | GS003 | memleak.py | 45 |
| L | GS003 | memleak.py | 54 |
| L | GS003 | run_clang_tidy.py | 94 |
| L | GS003 | run_clang_tidy.py | 96 |
| L | GS003 | subset.py | 40 |
| L | GS003 | subset.py | 48 |
| L | GS003 | subset.py | 54 |
| L | GS003 | subset.py | 56 |
| L | GS003 | subset.py | 76 |
| L | GS003 | subset.py | 91 |
| L | GS003 | subset.py | 94 |
| L | GS003 | subset.py | 127 |
| L | GS003 | subset.py | 129 |
| L | GS003 | subset.py | 132 |
| L | GS003 | subset.py | 154 |
| L | GS003 | subset.py | 158 |
| L | GS003 | subset.py | 364 |
| L | GS003 | triage_tests.py | 192 |
| L | GS003 | triage_tests.py | 203 |
| L | GS003 | triage_tests.py | 319 |
| L | GS003 | triage_tests.py | 339 |
| L | GS003 | mpl.js | 594 |
| L | GS003 | mpl.js | 607 |
| L | GS008 | _animation_data.py | 2 |
| L | GS008 | _animation_data.py | 163 |
| L | GS008 | _animation_data.py | 193 |
| L | GS008 | _animation_data.py | 257 |
| L | GS008 | _color_data.py | 1 |
| L | GS008 | _color_data.py | 14 |
| L | GS008 | _color_data.py | 993 |
| L | GS008 | _backend_pdf_ps.py | 30 |
| L | GS008 | cbook.py | 1733 |
| L | GS008 | dates.py | 244 |
| L | GS008 | dates.py | 250 |
| H | ? | rcsetup.py | 1531 |
| M | ? | stubtest.py | 110 |
| H | ? | rcsetup.py | 821 |
| H | ? | qt_compat.py | 145 |
| H | ? | _formlayout.py | 576 |
| H | ? | _formlayout.py | 582 |
| H | ? | _formlayout.py | 592 |
| H | ? | .meeseeksdev.yml | 0 |
| H | ? | environment.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | azure-pipelines.yml | 0 |
| H | ? | .yamllint.yml | 0 |
| H | ? | .appveyor.yml | 0 |
| H | GS002 | docutils.conf | 0 |
| H | GS004 | backend_qt.py | 480 |
| H | GS004 | backend_qt.py | 661 |
| H | GS004 | qt_compat.py | 143 |
| H | GS004 | triage_tests.py | 347 |
| s | GS009 |  | 0 |
| L | GS012 | blitting.py | 223 |
| L | GS012 | animation.py | 145 |
| L | GS012 | animation.py | 921 |
| L | GS012 | backend_bases.py | 2808 |
| L | GS012 | _backend_tk.py | 474 |
| L | GS012 | _backend_tk.py | 632 |
| L | GS012 | _backend_tk.py | 646 |
| L | GS012 | backend_cairo.py | 101 |
| L | GS012 | backend_cairo.py | 114 |
| L | GS012 | backend_cairo.py | 132 |
| L | GS012 | backend_cairo.py | 151 |
| L | GS012 | backend_cairo.py | 184 |
| L | GS012 | backend_cairo.py | 213 |
| L | GS012 | backend_cairo.py | 231 |
| L | GS012 | backend_cairo.py | 247 |
| L | GS012 | backend_cairo.py | 289 |
| L | GS012 | backend_cairo.py | 300 |
| L | GS012 | backend_macosx.py | 57 |
| L | GS012 | backend_macosx.py | 98 |
| L | GS012 | backend_macosx.py | 159 |
| L | GS012 | backend_qt.py | 495 |
| L | GS012 | backend_qt.py | 562 |
| L | GS012 | figure.py | 3260 |
| L | GS012 | widgets.py | 2591 |
| L | GS012 | widgets.py | 2614 |
| L | GS012 | widgets.py | 2630 |
| L | GS012 | widgets.py | 2894 |
| L | GS012 | widgets.py | 2959 |
| L | GS012 | widgets.py | 3103 |
| L | GS012 | widgets.py | 3494 |
| L | GS012 | widgets.py | 3566 |
| L | GS012 | widgets.py | 3800 |
| L | GS012 | widgets.py | 4000 |
| L | GS012 | widgets.py | 4349 |
| M | ? | cbook.py | 2276 |
| M | ? | _internal_utils.py | 62 |
| M | ? | compare.py | 106 |
| M | ? | boilerplate.py | 394 |
| M | ? | stubtest.py | 107 |
| M | ? | run_clang_tidy.py | 70 |
| M | ? | run_clang_tidy.py | 77 |

---
*Сгенерировано GSC v0.6 · 2026-07-19T04:02:58.232473*