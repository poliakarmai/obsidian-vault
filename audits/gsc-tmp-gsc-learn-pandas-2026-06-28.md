---
title: "GSC Audit: /tmp/gsc-learn/pandas"
date: 2026-06-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pandas

**Дата:** 28.06.2026 04:01  
**Путь:** `/tmp/gsc-learn/pandas`  
**Всего находок:** 2257  
**CRITICAL:** 9 | **HIGH:** 1265 | **MEDIUM:** 434 | **LOW:** 549

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Хардкод IP адреса | 1244 |
| Python: assert in production | 413 |
| GS003 | 18 |
| Bare except: | 17 |
| eval() or exec() usage | 13 |
| Generic code smell #24 | 9 |
| Generic code smell #27 | 9 |
| Generic code smell #30 | 9 |
| Generic code smell #33 | 9 |
| Generic code smell #36 | 9 |
| Generic code smell #39 | 9 |
| Generic code smell #42 | 9 |
| Generic code smell #45 | 9 |
| Generic code smell #48 | 9 |
| Generic code smell #51 | 9 |
| Generic code smell #54 | 9 |
| Generic code smell #57 | 9 |
| Generic code smell #60 | 9 |
| Generic code smell #63 | 9 |
| Generic code smell #66 | 9 |
| Generic code smell #69 | 9 |
| Generic code smell #72 | 9 |
| Generic code smell #75 | 9 |
| Generic code smell #78 | 9 |
| Generic code smell #81 | 9 |
| Generic code smell #84 | 9 |
| Generic code smell #87 | 9 |
| Generic code smell #90 | 9 |
| Generic code smell #93 | 9 |
| Generic code smell #96 | 9 |
| Generic code smell #99 | 9 |
| Generic code smell #102 | 9 |
| Generic code smell #105 | 9 |
| Generic code smell #108 | 9 |
| Generic code smell #111 | 9 |
| Generic code smell #114 | 9 |
| Generic code smell #117 | 9 |
| Generic code smell #120 | 9 |
| Generic code smell #123 | 9 |
| Generic code smell #126 | 9 |
| Generic code smell #129 | 9 |
| Generic code smell #132 | 9 |
| Generic code smell #135 | 9 |
| Generic code smell #138 | 9 |
| Generic code smell #141 | 9 |
| Generic code smell #144 | 9 |
| Generic code smell #147 | 9 |
| Generic code smell #150 | 9 |
| Generic code smell #153 | 9 |
| Generic code smell #156 | 9 |
| Generic code smell #159 | 9 |
| Generic code smell #162 | 9 |
| Generic code smell #165 | 9 |
| Generic code smell #168 | 9 |
| Generic code smell #171 | 9 |
| Generic code smell #174 | 9 |
| Generic code smell #177 | 9 |
| Generic code smell #180 | 9 |
| Generic code smell #183 | 9 |
| Generic code smell #186 | 9 |
| Generic code smell #189 | 9 |
| Generic code smell #192 | 9 |
| Generic code smell #195 | 9 |
| Generic code smell #198 | 9 |
| SQL injection risk: f-string in query | 6 |
| Python: File upload without content-type validation | 4 |
| Outdated dependency pattern | 3 |
| Hardcoded encryption key | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: environment.yml (664) | 1 |
| World-readable file: pyright_reportGeneralTypeIssues.json (664) | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| GS005 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | sql.py | 2246 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2248 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2460 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2610 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 26 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 75 | OWASP A03: Injection |
| CRITICAL | ? | hashing.py | 45 | Match: _default_hash_key = "0123456789123456" |
| CRITICAL | ? | pickle.py | 240 | Match:                 return pickle.load(handles.handle) |
| CRITICAL | GS005 | sql.py | 2460 | Line 2460: self.execute(f"DELETE FROM {quoted_table_name}"). |
| HIGH | ? | format.py | 1023 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _openpyxl.py | 109 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _odswriter.py | 92 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | excel.py | 83 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | pixi.lock | 17 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 132 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 370 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 485 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 941 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1019 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1254 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1332 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1549 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1800 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1860 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1907 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2022 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2255 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2336 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2451 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2683 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2868 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3051 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3133 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3257 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3440 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3522 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3643 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3807 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3911 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4026 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4263 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4378 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4833 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4910 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 5145 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 5222 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 5439 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 5619 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 5853 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6160 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6221 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6393 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6454 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6607 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6912 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 7015 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 7122 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 7378 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 7487 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 7955 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8262 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8559 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8647 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8752 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8999 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9104 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9564 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9642 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9871 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9949 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10160 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10454 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10530 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10592 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10715 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10974 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11097 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11589 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11676 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11926 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12013 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12243 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12342 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12465 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12724 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12847 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13339 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13426 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13676 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13763 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13993 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14092 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14215 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14472 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14595 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15084 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15172 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15420 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15508 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15736 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16065 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16151 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16225 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16345 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16607 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16727 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17226 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17312 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17564 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17650 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17882 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18207 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18292 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18367 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18483 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18725 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18737 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18738 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18739 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18740 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18758 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18874 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19115 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19127 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19128 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19129 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19130 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19264 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19276 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19277 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19278 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19279 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19402 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19482 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19615 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19627 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19628 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19629 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19630 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19753 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19833 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19965 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19976 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19977 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19978 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19979 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20084 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20323 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 20334 | Match:     - alsa-lib >=1.2.16.1,<1.3.0a0 |
| HIGH | ? | pixi.lock | 20381 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20382 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20383 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 20384 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20385 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20391 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 20399 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20400 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20401 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20402 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20403 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 20409 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 20417 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20424 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20432 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20440 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20454 | Match:     - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20466 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20473 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20479 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 20488 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20494 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 20502 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20503 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20504 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 20511 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 20521 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20522 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 20523 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20529 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20538 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 20539 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20540 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20541 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20547 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20555 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20556 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20557 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 20558 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20564 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20572 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20573 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20575 | Match:   - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 20580 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20589 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20590 | Match:   - s2n >=1.7.4,<1.7.5.0a0 |
| HIGH | ? | pixi.lock | 20591 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20597 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20605 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20606 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20607 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20613 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 20622 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20623 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20624 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20630 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 20639 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20640 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 20642 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20643 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 20644 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20645 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20651 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 20659 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 20660 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20661 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20662 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20663 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20664 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 20671 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 20678 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20684 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 20693 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20699 | Match:     - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 20706 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20712 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 20721 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20727 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 20735 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 20736 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20737 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20738 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 20739 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20740 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20741 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 20742 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 20743 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 20750 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20760 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 20761 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 20762 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20763 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20764 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 20765 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20766 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20767 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 20768 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20774 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 20782 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20783 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 20784 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 20785 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20805 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20806 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 20809 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 20831 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 20839 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 20848 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 20856 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 20857 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 20865 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 20873 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 20884 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 20892 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 20893 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 20894 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 20902 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 20961 | Match:   - binutils_impl_linux-64 >=2.45.1,<2.45.2.0a0 |
| HIGH | ? | pixi.lock | 21475 | Match:   - gcc_impl_linux-64 >=14.3.0,<14.3.1.0a0 |
| HIGH | ? | pixi.lock | 22649 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 22836 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 22844 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 22845 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 22846 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 22847 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 22848 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 22849 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 23020 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 23179 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 23192 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 23195 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 23200 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 23223 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23225 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23226 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23227 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23228 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23239 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23243 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23262 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23264 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23265 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23266 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23267 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23278 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23282 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23301 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23303 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23304 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23305 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23306 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23317 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23321 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23340 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23342 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23343 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23344 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23345 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23356 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23360 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23597 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23617 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23637 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23657 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23671 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 24060 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 24310 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 24333 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24395 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 24419 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24444 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24472 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 24484 | Match:     - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 24694 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 24723 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24768 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 24785 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 24802 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 24819 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 24903 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 24921 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25037 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 25112 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 25121 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 25129 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 25139 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25706 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 25720 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 25736 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 25750 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 25764 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 26662 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 26673 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 26688 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 26696 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 27234 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 28513 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 29013 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 29027 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 29089 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 29174 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 29411 | Match:     - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 29426 | Match:     - s2n >=1.7.4,<1.7.5.0a0 |
| HIGH | ? | pixi.lock | 30534 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 30606 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 30622 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 30640 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 30656 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 30827 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 30837 | Match:     - alsa-lib >=1.2.16.1,<1.3.0a0 |
| HIGH | ? | pixi.lock | 30882 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 30883 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 30884 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 30885 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 30886 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 30892 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 30899 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 30900 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 30901 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 30902 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 30903 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 30909 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 30916 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 30923 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 30930 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 30938 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 30951 | Match:     - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 30963 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 30970 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 30976 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 30984 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 30990 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 30997 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 30998 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 30999 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 31006 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 31015 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31016 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 31017 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31023 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31031 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31032 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31033 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 31034 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31040 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31047 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31048 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31049 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 31050 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31056 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31063 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31064 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31066 | Match:   - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 31071 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31079 | Match:   - s2n >=1.7.4,<1.7.5.0a0 |
| HIGH | ? | pixi.lock | 31080 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31081 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31087 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31094 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31095 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31096 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31102 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 31110 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31111 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31112 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31118 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 31126 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31127 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31128 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 31129 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 31130 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31132 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31138 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 31145 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 31146 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31147 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31148 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31149 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31150 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 31157 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 31164 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31170 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 31178 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31184 | Match:     - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 31191 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31197 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 31205 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31211 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 31218 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 31219 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31220 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31221 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 31222 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31223 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31224 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 31225 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 31226 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 31233 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31242 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31243 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 31244 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 31245 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31246 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31247 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 31248 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31249 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 31250 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31256 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 31263 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31264 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 31265 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 31266 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31287 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 31288 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 31289 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31310 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 31317 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 31326 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 31333 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 31334 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 31342 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 31349 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 31360 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 31367 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 31368 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 31369 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 31377 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 31433 | Match:   - binutils_impl_linux-aarch64 >=2.45.1,<2.45.2.0a0 |
| HIGH | ? | pixi.lock | 31964 | Match:   - gcc_impl_linux-aarch64 >=14.3.0,<14.3.1.0a0 |
| HIGH | ? | pixi.lock | 33103 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 33286 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 33293 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 33294 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 33295 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 33296 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 33297 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 33298 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 33460 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 33619 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 33632 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 33635 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 33640 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 33662 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 33664 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 33665 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 33666 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 33667 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 33678 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 33682 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 33700 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 33702 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 33703 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 33704 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 33705 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 33716 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 33720 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 33738 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 33740 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 33741 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 33742 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 33743 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 33754 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 33758 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 33776 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 33778 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 33779 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 33780 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 33781 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 33792 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 33796 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34020 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34039 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34058 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34077 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34091 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 34459 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 34700 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 34722 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34782 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 34805 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34829 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34856 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 34867 | Match:     - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 35063 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 35091 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35134 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 35150 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 35166 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 35182 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 35261 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 35278 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35376 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 35468 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 35477 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 35484 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 35494 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36037 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 36051 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 36066 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 36080 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 36094 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 36971 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 36982 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 36993 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 37004 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 37536 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 38756 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 39216 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 39230 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 39291 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 39365 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 39608 | Match:     - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 39622 | Match:     - s2n >=1.7.4,<1.7.5.0a0 |
| HIGH | ? | pixi.lock | 40665 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 40734 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 40750 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 40768 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 40784 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 40825 | Match:   - libadbc-driver-postgresql >=1.11.0,<1.11.1.0a0 |
| HIGH | ? | pixi.lock | 40842 | Match:   - libadbc-driver-postgresql >=1.2.0,<1.2.1.0a0 |
| HIGH | ? | pixi.lock | 40857 | Match:   - libadbc-driver-postgresql >=1.8.0,<1.8.1.0a0 |
| HIGH | ? | pixi.lock | 40872 | Match:   - libadbc-driver-sqlite >=1.11.0,<1.11.1.0a0 |
| HIGH | ? | pixi.lock | 40889 | Match:   - libadbc-driver-sqlite >=1.2.0,<1.2.1.0a0 |
| HIGH | ? | pixi.lock | 40904 | Match:   - libadbc-driver-sqlite >=1.3.0,<1.3.1.0a0 |
| HIGH | ? | pixi.lock | 41539 | Match:   - dask-core >=2026.6.0,<2026.6.1.0a0 |
| HIGH | ? | pixi.lock | 41540 | Match:   - distributed >=2026.6.0,<2026.6.1.0a0 |
| HIGH | ? | pixi.lock | 41618 | Match:   - dask-core >=2026.6.0,<2026.6.1.0a0 |
| HIGH | ? | pixi.lock | 41898 | Match:   - typing_extensions >=3.10.0.2 |
| HIGH | ? | pixi.lock | 42332 | Match:   - importlib-resources >=7.1.0,<7.1.1.0a0 |
| HIGH | ? | pixi.lock | 43491 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 44411 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 44878 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 44888 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 44898 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 44908 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 45457 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45458 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 45459 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45460 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45461 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45467 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 45475 | Match:   - aws-c-sdkutils >=0.2.4,<0.2.5.0a0 |
| HIGH | ? | pixi.lock | 45476 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45477 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45478 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45479 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45484 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 45492 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45493 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45494 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 45495 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 45496 | Match:   - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 45501 | Match:     - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45509 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45515 | Match:     - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45523 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45529 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45541 | Match:     - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45554 | Match:     - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45562 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45567 | Match:     - aws-c-compression >=0.3.0,<0.3.1.0a0 |
| HIGH | ? | pixi.lock | 45575 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45581 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 45589 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45590 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 45591 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 45597 | Match:     - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 45606 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 45607 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45608 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45614 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 45622 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45623 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45624 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 45625 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45631 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45639 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45640 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45641 | Match:   - aws-c-compression >=0.3.0,<0.3.1.0a0 |
| HIGH | ? | pixi.lock | 45642 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 45647 | Match:     - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 45655 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45656 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45661 | Match:     - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 45669 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45670 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45676 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45684 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45685 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 45686 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 45691 | Match:     - aws-c-mqtt >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45699 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45700 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45701 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45706 | Match:     - aws-c-mqtt >=0.15.2,<0.15.3.0a0 |
| HIGH | ? | pixi.lock | 45714 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45715 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45716 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45722 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 45730 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 45731 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 45732 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45733 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45734 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45735 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45740 | Match:     - aws-c-s3 >=0.12.5,<0.12.6.0a0 |
| HIGH | ? | pixi.lock | 45748 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 45749 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45750 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45751 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45752 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45753 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 45759 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 45767 | Match:   - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45768 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45769 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45770 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 45771 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 45772 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 45777 | Match:     - aws-c-s3 >=0.7.9,<0.7.10.0a0 |
| HIGH | ? | pixi.lock | 45785 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45790 | Match:     - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 45798 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45803 | Match:     - aws-c-sdkutils >=0.2.4,<0.2.5.0a0 |
| HIGH | ? | pixi.lock | 45811 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45817 | Match:     - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 45825 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45831 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 45839 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45844 | Match:     - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 45852 | Match:   - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45853 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 45854 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45855 | Match:   - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 45856 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 45857 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 45858 | Match:   - aws-c-mqtt >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45859 | Match:   - aws-c-s3 >=0.7.9,<0.7.10.0a0 |
| HIGH | ? | pixi.lock | 45860 | Match:   - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 45866 | Match:     - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 45875 | Match:   - aws-c-s3 >=0.12.5,<0.12.6.0a0 |
| HIGH | ? | pixi.lock | 45876 | Match:   - aws-c-mqtt >=0.15.2,<0.15.3.0a0 |
| HIGH | ? | pixi.lock | 45877 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45878 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45879 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45880 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 45881 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 45882 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45883 | Match:   - aws-c-sdkutils >=0.2.4,<0.2.5.0a0 |
| HIGH | ? | pixi.lock | 45888 | Match:     - aws-crt-cpp >=0.40.0,<0.40.1.0a0 |
| HIGH | ? | pixi.lock | 45897 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 45898 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45899 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 45900 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 45901 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 45902 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 45903 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 45904 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 45905 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 45911 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 45919 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 45920 | Match:   - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 45921 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 45922 | Match:   - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 45941 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45943 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 45944 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 45958 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 45960 | Match:   - aws-crt-cpp >=0.40.0,<0.40.1.0a0 |
| HIGH | ? | pixi.lock | 45961 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 45983 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 45991 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 45999 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 46007 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 46008 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 46015 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 46023 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 46033 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 46041 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 46042 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 46043 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 46050 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 47810 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 47818 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 47819 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 47820 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47821 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47822 | Match:   - aws-c-s3 >=0.12.5,<0.12.6.0a0 |
| HIGH | ? | pixi.lock | 47823 | Match:   - aws-c-sdkutils >=0.2.4,<0.2.5.0a0 |
| HIGH | ? | pixi.lock | 47843 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 47844 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 47845 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47846 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47847 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 47848 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 47981 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 48033 | Match:   - tapi >=1600.0.11.8,<1601.0a0 |
| HIGH | ? | pixi.lock | 48172 | Match:   - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 48187 | Match:   - orc >=2.0.3,<2.0.4.0a0 |
| HIGH | ? | pixi.lock | 48208 | Match:   - aws-crt-cpp >=0.40.0,<0.40.1.0a0 |
| HIGH | ? | pixi.lock | 48210 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 48211 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 48212 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 48213 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 48224 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48227 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 48247 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 48249 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 48250 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 48251 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 48252 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 48263 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48266 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 48285 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 48287 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 48288 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 48289 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 48290 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 48301 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48304 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 48323 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 48325 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 48326 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 48327 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 48328 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 48339 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48342 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 48383 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48403 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48422 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48441 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48460 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48482 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48503 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48524 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48566 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48588 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48609 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48630 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48649 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 48666 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 48704 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 48724 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48744 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48763 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48782 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 48795 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 49045 | Match:   - libcxx-headers >=19.1.7,<19.1.8.0a0 |
| HIGH | ? | pixi.lock | 49057 | Match:   - libcxx-headers >=21.1.8,<21.1.9.0a0 |
| HIGH | ? | pixi.lock | 49112 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 49234 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 49256 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49316 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 49339 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49363 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49415 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-6 |
| HIGH | ? | pixi.lock | 49426 | Match:     - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 49648 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 49666 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49709 | Match:   - libthrift >=0.21.0,<0.21.1.0a0 |
| HIGH | ? | pixi.lock | 49729 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49730 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 49750 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49751 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 49770 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49771 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 49790 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49791 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 49857 | Match:     - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 49874 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49950 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 50000 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 50007 | Match:     - libthrift >=0.21.0,<0.21.1.0a0 |
| HIGH | ? | pixi.lock | 50016 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 50024 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 50536 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 50549 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 50564 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 50577 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 50590 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 51421 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 51431 | Match:     - orc >=2.0.3,<2.0.4.0a0 |
| HIGH | ? | pixi.lock | 51441 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51453 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 52998 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 54022 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-6 |
| HIGH | ? | pixi.lock | 54358 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 54427 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 54442 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 54459 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 54474 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 54684 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 54685 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 54686 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54687 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 54688 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 54694 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 54702 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 54703 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54704 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 54705 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 54706 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 54711 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 54719 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54725 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 54733 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54739 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 54752 | Match:     - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54764 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54772 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54777 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 54785 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54791 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 54799 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54800 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 54801 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 54807 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 54816 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 54817 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 54818 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54824 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 54832 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 54833 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 54834 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54835 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 54841 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 54849 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 54850 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54851 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 54852 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 54857 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 54865 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 54866 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54871 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 54879 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54880 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 54886 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 54894 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54895 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 54896 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 54901 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 54909 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54910 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 54911 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 54917 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 54925 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54926 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 54927 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 54928 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 54929 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 54930 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 54936 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 54944 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 54945 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 54946 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54947 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 54948 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 54949 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 54954 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 54962 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54967 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 54975 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 54981 | Match:     - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 54989 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 54994 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 55002 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 55008 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 55016 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 55017 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 55018 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 55019 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 55020 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 55021 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 55022 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 55023 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 55024 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 55030 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 55039 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 55040 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 55041 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 55042 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 55043 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 55044 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 55045 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 55046 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 55047 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 55053 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 55061 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 55062 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 55063 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 55064 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 55082 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 55083 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 55086 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 55107 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 55115 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 55123 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 55131 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 55132 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 55139 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 55147 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 55157 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 55165 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 55166 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 55167 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 55174 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 57009 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 57017 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 57018 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 57019 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 57020 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 57021 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 57022 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 57159 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 57224 | Match:   - tapi >=1600.0.11.8,<1601.0a0 |
| HIGH | ? | pixi.lock | 57363 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 57375 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 57377 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 57382 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 57404 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 57406 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 57407 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 57408 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 57409 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 57420 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57423 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 57442 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 57444 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 57445 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 57446 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 57447 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 57458 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57461 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 57480 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 57482 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 57483 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 57484 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 57485 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 57496 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57499 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 57518 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 57520 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 57521 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 57522 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 57523 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 57534 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57537 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 57563 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57582 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57601 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57620 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57639 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57660 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57681 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57702 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57727 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57748 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57769 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57790 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57810 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57829 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57848 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57867 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 57880 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 58129 | Match:   - libcxx-headers >=19.1.7,<19.1.8.0a0 |
| HIGH | ? | pixi.lock | 58185 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 58307 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 58329 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58388 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 58411 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58435 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58487 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-a |
| HIGH | ? | pixi.lock | 58498 | Match:     - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 58718 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 58736 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58782 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58783 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 58802 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58803 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 58822 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58823 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 58842 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 58843 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 58909 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 58926 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59001 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 59049 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 59056 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 59065 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 59073 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 59597 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 59610 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 59625 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 59638 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 59651 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 60511 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 60521 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 60534 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60543 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 61061 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 62089 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 63123 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-a |
| HIGH | ? | pixi.lock | 63476 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 63546 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 63562 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 63580 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 63596 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 63817 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 63818 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 63819 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 63820 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 63821 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 63827 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 63834 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 63835 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 63836 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 63837 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 63838 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 63846 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 63853 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 63862 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 63869 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 63878 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 63893 | Match:     - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 63907 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 63914 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 63922 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 63932 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 63938 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 63945 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 63946 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 63947 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 63955 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 63965 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 63966 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 63967 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 63973 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 63983 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 63984 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 63985 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 63986 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 63992 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 63999 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 64000 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64001 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 64002 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 64010 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 64017 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 64018 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64026 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 64036 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 64037 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 64043 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 64050 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64051 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 64052 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 64060 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 64070 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 64071 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 64072 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 64078 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 64088 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 64089 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 64090 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 64091 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 64092 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 64093 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 64099 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 64106 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 64107 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 64108 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64109 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 64110 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 64111 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 64119 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 64126 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64134 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 64144 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 64150 | Match:     - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 64157 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64165 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 64175 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 64181 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 64188 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 64189 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 64190 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64191 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 64192 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 64193 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 64194 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 64195 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 64196 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 64204 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 64214 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 64215 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 64216 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 64217 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 64218 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 64219 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 64220 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 64221 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 64222 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 64228 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 64235 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 64236 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 64237 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 64238 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 64257 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 64258 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 64260 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 64280 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 64287 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 64296 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 64303 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 64304 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 64313 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 64320 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 64329 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 64336 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 64337 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 64338 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 64347 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 64912 | Match:   - gcc_impl_win-64 >=15.2.0,<15.2.1.0a0 |
| HIGH | ? | pixi.lock | 66080 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 66087 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 66088 | Match:   - aws-c-common >=0.14.0,<0.14.1.0a0 |
| HIGH | ? | pixi.lock | 66089 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66090 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66091 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 66092 | Match:   - aws-c-sdkutils >=0.2.5,<0.2.6.0a0 |
| HIGH | ? | pixi.lock | 66246 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 66405 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66417 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 66419 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 66424 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 66448 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66450 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66451 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 66452 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66453 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 66463 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 66466 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 66487 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66489 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66490 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 66491 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66492 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 66502 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 66505 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 66526 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66528 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66529 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 66530 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66531 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 66541 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 66544 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 66565 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66567 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66568 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 66569 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66570 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 66580 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 66583 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 66821 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 66841 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 66861 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 66881 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 67155 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 67309 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 67331 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 67391 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 67415 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 67440 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 67472 | Match:     - libhwloc >=2.13.0,<2.13.1.0a0 |
| HIGH | ? | pixi.lock | 67513 | Match: - conda: https://conda.anaconda.org/conda-forge/win-6 |
| HIGH | ? | pixi.lock | 67526 | Match:     - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 67622 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 67651 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 67668 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 67685 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 67702 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 67776 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 67794 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 67864 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 67915 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 67925 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 67932 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 67943 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 68560 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 68574 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 68590 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 68604 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 68618 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 69473 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 69486 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 69501 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69509 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 70065 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 71265 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 71696 | Match:   - zeromq >=4.3.5,<4.3.6.0a0 |
| HIGH | ? | pixi.lock | 71791 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72327 | Match:   - libhwloc >=2.13.0,<2.13.1.0a0 |
| HIGH | ? | pixi.lock | 72775 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 72782 | Match:     - zeromq >=4.3.5,<4.3.6.0a0 |
| HIGH | ? | pixi.lock | 72851 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 72871 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 72893 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 72913 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | eval_performance.py | 20 | Match:                 f"df.eval(s, engine={engine!r})", |
| HIGH | ? | eval_performance.py | 107 | Match:     plot_perf(ev, engines, "DataFrame.eval()", filena |
| HIGH | ? | eval.py | 179 | Match: def eval( |
| HIGH | ? | ops.py | 430 | Match:                 res = eval(self, local_dict=env, engi |
| HIGH | ? | frame.py | 5232 | Match:         >>> df.eval("A + B") |
| HIGH | ? | frame.py | 5243 | Match:         >>> df.eval("D = A + B") |
| HIGH | ? | frame.py | 5260 | Match:         >>> df.eval( |
| HIGH | ? | frame.py | 5276 | Match:         >>> df.eval("B * `C&C`") |
| HIGH | ? | frame.py | 5288 | Match:         >>> df.eval("@local_var * A") |
| HIGH | ? | eval.py | 25 | Match:         pd.eval("self.df + self.df2 + self.df3 + self |
| HIGH | ? | eval.py | 28 | Match:         pd.eval( |
| HIGH | ? | eval.py | 34 | Match:         pd.eval("self.df < self.df2 < self.df3 < self |
| HIGH | ? | eval.py | 37 | Match:         pd.eval("self.df * self.df2 * self.df3 * self |
| HIGH | ? | environment.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | pyright_reportGeneralTypeIssues.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | sql.py | 2246 |
| C | ? | sql.py | 2248 |
| C | ? | sql.py | 2460 |
| C | ? | sql.py | 2610 |
| C | ? | sql.py | 26 |
| C | ? | sql.py | 75 |
| M | ? | hashtable_class_helper.pxi.in | 235 |
| M | ? | hashtable_class_helper.pxi.in | 309 |
| M | ? | groupby.pyx | 1607 |
| M | ? | parsers.pyx | 303 |
| M | ? | parsers.pyx | 306 |
| M | ? | tzconversion.pyx | 454 |
| M | ? | period.pyx | 1102 |
| M | ? | util.pxd | 41 |
| M | ? | util.pxd | 48 |
| M | ? | util.pxd | 118 |
| M | ? | util.pxd | 122 |
| M | ? | np_datetime.pxd | 68 |
| M | ? | strptime.pyx | 265 |
| M | ? | timedeltas.pyx | 327 |
| M | ? | parsing.pyx | 1097 |
| M | ? | np_datetime.pyx | 282 |
| M | ? | np_datetime.pyx | 318 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | groupby.py | 1573 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | groupby.py | 1573 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | groupby.py | 1573 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| L | ? | numba.pyi | 22 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | groupby.py | 1573 |
| L | ? | datetimes.py | 1158 |
| L | ? | merge.py | 1610 |
| L | ? | array.py | 1288 |
| L | ? | masked.py | 878 |
| L | ? | managers.py | 1320 |
| M | ? | validate_min_versions_in_sync.py | 115 |
| M | ? | validate_min_versions_in_sync.py | 135 |
| M | ? | check_test_naming.py | 122 |
| M | ? | groupby.py | 80 |
| M | ? | converter.py | 1125 |
| M | ? | core.py | 292 |
| M | ? | timeseries.py | 280 |
| M | ? | hist.py | 281 |
| M | ? | hist.py | 378 |
| M | ? | boxplot.py | 60 |
| M | ? | frequencies.py | 480 |
| M | ? | frequencies.py | 627 |
| M | ? | pandas_web.py | 405 |
| M | ? | groupby.py | 834 |
| M | ? | groupby.py | 1491 |
| M | ? | groupby.py | 1501 |
| M | ? | groupby.py | 1582 |
| M | ? | groupby.py | 1744 |
| M | ? | groupby.py | 1969 |
| M | ? | groupby.py | 1970 |
| M | ? | groupby.py | 5693 |
| M | ? | groupby.py | 5741 |
| M | ? | groupby.py | 5784 |
| M | ? | generic.py | 478 |
| M | ? | generic.py | 588 |
| M | ? | generic.py | 788 |
| M | ? | generic.py | 2800 |
| M | ? | generic.py | 4252 |
| M | ? | apply.py | 255 |
| M | ? | apply.py | 337 |
| M | ? | apply.py | 392 |
| M | ? | apply.py | 757 |
| M | ? | apply.py | 800 |
| M | ? | apply.py | 809 |
| M | ? | apply.py | 810 |
| M | ? | apply.py | 868 |
| M | ? | apply.py | 1124 |
| M | ? | apply.py | 1215 |
| M | ? | apply.py | 1252 |
| M | ? | apply.py | 1427 |
| M | ? | apply.py | 1667 |
| M | ? | apply.py | 1791 |
| M | ? | apply.py | 1948 |
| M | ? | apply.py | 2154 |
| M | ? | apply.py | 2155 |
| M | ? | accessor.py | 278 |
| M | ? | ops.py | 527 |
| M | ? | ops.py | 552 |
| M | ? | ops.py | 556 |
| M | ? | ops.py | 620 |
| M | ? | ops.py | 1014 |
| M | ? | ops.py | 1287 |
| M | ? | numba_.py | 109 |
| M | ? | numba_.py | 166 |
| M | ? | grouper.py | 347 |
| M | ? | grouper.py | 367 |
| M | ? | grouper.py | 508 |
| M | ? | grouper.py | 861 |
| M | ? | nanops.py | 359 |
| M | ? | nanops.py | 417 |
| M | ? | nanops.py | 1681 |
| M | ? | sorting.py | 505 |
| M | ? | from_dataframe.py | 328 |
| M | ? | from_dataframe.py | 332 |
| M | ? | from_dataframe.py | 510 |
| M | ? | array_ops.py | 378 |
| M | ? | array_ops.py | 384 |
| M | ? | numeric.py | 312 |
| M | ? | datetimes.py | 219 |
| M | ? | datetimes.py | 225 |
| M | ? | datetimelike.py | 1306 |
| M | ? | datetimelike.py | 1315 |
| M | ? | datetimelike.py | 1316 |
| M | ? | datetimelike.py | 1350 |
| M | ? | multi.py | 1606 |
| M | ? | multi.py | 1681 |
| M | ? | range.py | 251 |
| M | ? | range.py | 1089 |
| M | ? | timedeltas.py | 305 |
| M | ? | timedeltas.py | 348 |
| M | ? | cast.py | 1014 |
| M | ? | cast.py | 1053 |
| M | ? | cast.py | 1070 |
| M | ? | cast.py | 1513 |
| M | ? | dtypes.py | 2447 |
| M | ? | datetimes.py | 99 |
| M | ? | period.py | 536 |
| M | ? | base.py | 667 |
| M | ? | base.py | 745 |
| M | ? | base.py | 3876 |
| M | ? | base.py | 4691 |
| M | ? | base.py | 4863 |
| M | ? | base.py | 4941 |
| M | ? | base.py | 5040 |
| M | ? | base.py | 5041 |
| M | ? | base.py | 5107 |
| M | ? | base.py | 7223 |
| M | ? | common.py | 120 |
| M | ? | common.py | 284 |
| M | ? | extensions.py | 90 |
| M | ? | extensions.py | 103 |
| M | ? | extensions.py | 120 |
| M | ? | extensions.py | 121 |
| M | ? | extensions.py | 136 |
| M | ? | extensions.py | 145 |
| M | ? | extensions.py | 146 |
| M | ? | extensions.py | 154 |
| M | ? | extensions.py | 166 |
| M | ? | extensions.py | 167 |
| M | ? | extensions.py | 168 |
| M | ? | extension.py | 175 |
| M | ? | missing.py | 260 |
| M | ? | hashing.py | 79 |
| M | ? | sample.py | 109 |
| M | ? | sample.py | 158 |
| M | ? | describe.py | 379 |
| M | ? | merge.py | 1279 |
| M | ? | merge.py | 1393 |
| M | ? | merge.py | 1528 |
| M | ? | merge.py | 2057 |
| M | ? | merge.py | 2641 |
| M | ? | merge.py | 2903 |
| M | ? | merge.py | 2904 |
| M | ? | merge.py | 2984 |
| M | ? | merge.py | 2988 |
| M | ? | merge.py | 3025 |
| M | ? | merge.py | 3026 |
| M | ? | pivot.py | 490 |
| M | ? | pivot.py | 563 |
| M | ? | pivot.py | 700 |
| M | ? | reshape.py | 438 |
| M | ? | reshape.py | 552 |
| M | ? | reshape.py | 620 |
| M | ? | reshape.py | 836 |
| M | ? | reshape.py | 1028 |
| M | ? | reshape.py | 1093 |
| M | ? | extension_types.py | 66 |
| M | ? | array.py | 500 |
| M | ? | array.py | 2069 |
| M | ? | array.py | 2081 |
| M | ? | categorical.py | 1638 |
| M | ? | categorical.py | 1990 |
| M | ? | categorical.py | 2367 |
| M | ? | categorical.py | 2593 |
| M | ? | categorical.py | 2876 |
| M | ? | numeric.py | 212 |
| M | ? | _mixins.py | 191 |
| M | ? | datetimelike.py | 1076 |
| M | ? | datetimelike.py | 1297 |
| M | ? | datetimelike.py | 1313 |
| M | ? | datetimelike.py | 1690 |
| M | ? | boolean.py | 390 |
| M | ? | boolean.py | 394 |
| M | ? | interval.py | 1688 |
| M | ? | interval.py | 1692 |
| M | ? | interval.py | 1722 |
| M | ? | interval.py | 1726 |
| M | ? | interval.py | 1869 |
| M | ? | interval.py | 1873 |
| M | ? | interval.py | 1878 |
| M | ? | array.py | 2065 |
| M | ? | string_arrow.py | 172 |
| M | ? | string_arrow.py | 237 |
| M | ? | string_.py | 767 |
| M | ? | timedeltas.py | 240 |
| M | ? | timedeltas.py | 241 |
| M | ? | timedeltas.py | 242 |
| M | ? | timedeltas.py | 243 |
| M | ? | timedeltas.py | 438 |
| M | ? | timedeltas.py | 635 |
| M | ? | timedeltas.py | 1073 |
| M | ? | timedeltas.py | 1154 |
| M | ? | timedeltas.py | 1155 |
| M | ? | _ranges.py | 202 |
| M | ? | _ranges.py | 235 |
| M | ? | _ranges.py | 248 |
| M | ? | _ranges.py | 269 |
| M | ? | _ranges.py | 278 |
| M | ? | datetimes.py | 307 |
| M | ? | datetimes.py | 308 |
| M | ? | datetimes.py | 310 |
| M | ? | datetimes.py | 311 |
| M | ? | datetimes.py | 315 |
| M | ? | datetimes.py | 794 |
| M | ? | period.py | 261 |
| M | ? | period.py | 983 |
| M | ? | period.py | 1193 |
| M | ? | period.py | 1200 |
| M | ? | period.py | 1290 |
| M | ? | masked.py | 1442 |
| M | ? | base.py | 3041 |
| M | ? | scope.py | 236 |
| M | ? | scope.py | 326 |
| M | ? | scope.py | 328 |
| M | ? | expr.py | 136 |
| M | ? | expr.py | 170 |
| M | ? | expr.py | 258 |
| M | ? | pytables.py | 108 |
| M | ? | pytables.py | 665 |
| M | ? | expressions.py | 268 |
| M | ? | blocks.py | 362 |
| M | ? | blocks.py | 400 |
| M | ? | blocks.py | 424 |
| M | ? | blocks.py | 872 |
| M | ? | blocks.py | 1050 |
| M | ? | blocks.py | 1051 |
| M | ? | blocks.py | 1197 |
| M | ? | blocks.py | 1258 |
| M | ? | blocks.py | 1259 |
| M | ? | blocks.py | 1558 |
| M | ? | blocks.py | 1559 |
| M | ? | blocks.py | 2058 |
| M | ? | blocks.py | 2065 |
| M | ? | blocks.py | 2417 |
| M | ? | ops.py | 124 |
| M | ? | ops.py | 131 |
| M | ? | ops.py | 133 |
| M | ? | ops.py | 140 |
| M | ? | ops.py | 144 |
| M | ? | managers.py | 258 |
| M | ? | managers.py | 420 |
| M | ? | managers.py | 506 |
| M | ? | managers.py | 507 |
| M | ? | managers.py | 849 |
| M | ? | managers.py | 1045 |
| M | ? | managers.py | 1704 |
| M | ? | managers.py | 1747 |
| M | ? | managers.py | 1748 |
| M | ? | managers.py | 1792 |
| M | ? | managers.py | 2064 |
| M | ? | managers.py | 2065 |
| M | ? | managers.py | 2571 |
| M | ? | resample.py | 242 |
| M | ? | resample.py | 525 |
| M | ? | resample.py | 527 |
| M | ? | resample.py | 2019 |
| M | ? | resample.py | 2022 |
| M | ? | resample.py | 2092 |
| M | ? | resample.py | 2141 |
| M | ? | resample.py | 3045 |
| M | ? | arraylike.py | 522 |
| M | ? | generic.py | 533 |
| M | ? | generic.py | 5758 |
| M | ? | generic.py | 6094 |
| M | ? | generic.py | 10809 |
| M | ? | generic.py | 10840 |
| M | ? | generic.py | 11720 |
| M | ? | generic.py | 11831 |
| M | ? | series.py | 1241 |
| M | ? | series.py | 4663 |
| M | ? | series.py | 4717 |
| M | ? | series.py | 7272 |
| M | ? | series.py | 7273 |
| M | ? | objects.py | 190 |
| M | ? | objects.py | 615 |
| M | ? | rolling.py | 3541 |
| M | ? | indexing.py | 976 |
| M | ? | indexing.py | 985 |
| M | ? | indexing.py | 986 |
| M | ? | indexing.py | 1125 |
| M | ? | indexing.py | 2587 |
| M | ? | indexing.py | 3296 |
| M | ? | construction.py | 395 |
| M | ? | _warnings.py | 267 |
| M | ? | asserters.py | 834 |
| M | ? | asserters.py | 835 |
| M | ? | asserters.py | 883 |
| M | ? | asserters.py | 891 |
| M | ? | asserters.py | 1065 |
| M | ? | asserters.py | 1088 |
| M | ? | asserters.py | 1364 |
| M | ? | asserters.py | 1374 |
| M | ? | asserters.py | 1412 |
| M | ? | asserters.py | 1413 |
| M | ? | asserters.py | 1470 |
| M | ? | asserters.py | 1488 |
| M | ? | asserters.py | 1489 |
| M | ? | asserters.py | 1491 |
| M | ? | asserters.py | 1509 |
| M | ? | asserters.py | 1510 |
| M | ? | asserters.py | 1530 |
| M | ? | asserters.py | 1548 |
| M | ? | asserters.py | 1590 |
| M | ? | asserters.py | 1592 |
| M | ? | _optional.py | 148 |
| M | ? | config.py | 405 |
| M | ? | config.py | 756 |
| M | ? | _print_versions.py | 141 |
| M | ? | _print_versions.py | 146 |
| M | ? | sas7bdat.py | 340 |
| M | ? | sas7bdat.py | 355 |
| M | ? | sas7bdat.py | 375 |
| M | ? | stata.py | 1483 |
| M | ? | stata.py | 1527 |
| M | ? | stata.py | 1695 |
| M | ? | stata.py | 2540 |
| M | ? | stata.py | 2955 |
| M | ? | stata.py | 3519 |
| M | ? | csvs.py | 222 |
| M | ? | csvs.py | 238 |
| M | ? | format.py | 667 |
| M | ? | format.py | 692 |
| M | ? | format.py | 1026 |
| M | ? | format.py | 1311 |
| M | ? | html.py | 491 |
| M | ? | xml.py | 544 |
| M | ? | string.py | 133 |
| M | ? | css.py | 319 |
| M | ? | excel.py | 361 |
| M | ? | _base.py | 840 |
| M | ? | _base.py | 851 |
| M | ? | _base.py | 858 |
| M | ? | _base.py | 881 |
| M | ? | _base.py | 886 |
| M | ? | _base.py | 913 |
| M | ? | _base.py | 1209 |
| M | ? | _base.py | 1491 |
| M | ? | _base.py | 1650 |
| M | ? | _odswriter.py | 118 |
| M | ? | _util.py | 81 |
| M | ? | _util.py | 293 |
| M | ? | _util.py | 296 |
| M | ? | parquet.py | 537 |
| M | ? | sql.py | 352 |
| M | ? | sql.py | 494 |
| M | ? | sql.py | 699 |
| M | ? | sql.py | 1073 |
| M | ? | sql.py | 1309 |
| M | ? | html.py | 998 |
| M | ? | c_parser_wrapper.py | 133 |
| M | ? | c_parser_wrapper.py | 171 |
| M | ? | c_parser_wrapper.py | 190 |
| M | ? | c_parser_wrapper.py | 225 |
| M | ? | c_parser_wrapper.py | 309 |
| M | ? | base_parser.py | 314 |
| M | ? | base_parser.py | 355 |
| M | ? | python_parser.py | 144 |
| M | ? | python_parser.py | 997 |
| M | ? | python_parser.py | 1257 |
| M | ? | python_parser.py | 1362 |
| M | ? | python_parser.py | 1367 |
| M | ? | pytables.py | 655 |
| M | ? | pytables.py | 755 |
| M | ? | pytables.py | 1910 |
| M | ? | pytables.py | 1911 |
| M | ? | pytables.py | 1970 |
| M | ? | pytables.py | 1971 |
| M | ? | pytables.py | 1995 |
| M | ? | pytables.py | 1996 |
| M | ? | pytables.py | 2002 |
| M | ? | pytables.py | 2240 |
| M | ? | pytables.py | 2394 |
| M | ? | pytables.py | 2398 |
| M | ? | pytables.py | 2431 |
| M | ? | pytables.py | 2639 |
| M | ? | pytables.py | 2640 |
| M | ? | pytables.py | 2694 |
| M | ? | pytables.py | 2940 |
| M | ? | pytables.py | 3029 |
| M | ? | pytables.py | 3030 |
| M | ? | pytables.py | 3151 |
| M | ? | pytables.py | 3161 |
| M | ? | pytables.py | 3172 |
| M | ? | pytables.py | 3180 |
| M | ? | pytables.py | 3266 |
| M | ? | pytables.py | 3328 |
| M | ? | pytables.py | 3329 |
| M | ? | pytables.py | 3330 |
| M | ? | pytables.py | 3526 |
| M | ? | pytables.py | 4226 |
| M | ? | pytables.py | 4419 |
| M | ? | pytables.py | 4691 |
| M | ? | pytables.py | 4751 |
| M | ? | pytables.py | 4754 |
| M | ? | pytables.py | 4952 |
| M | ? | pytables.py | 4965 |
| M | ? | pytables.py | 5238 |
| M | ? | pytables.py | 5412 |
| M | ? | pytables.py | 5472 |
| M | ? | pytables.py | 5525 |
| M | ? | pytables.py | 5552 |
| M | ? | pytables.py | 5603 |
| M | ? | pytables.py | 5645 |
| M | ? | pytables.py | 5713 |
| M | ? | pytables.py | 5726 |
| M | ? | pytables.py | 5821 |
| M | ? | pytables.py | 5822 |
| M | ? | pytables.py | 6013 |
| M | ? | common.py | 135 |
| M | ? | common.py | 421 |
| M | ? | common.py | 881 |
| M | ? | common.py | 887 |
| M | ? | common.py | 928 |
| M | ? | common.py | 987 |
| M | ? | common.py | 1171 |
| M | ? | common.py | 1337 |
| M | ? | orc.py | 242 |
| M | ? | orc.py | 256 |
| M | ? | take.py | 193 |
| M | ? | take.py | 194 |
| M | ? | take.py | 195 |
| M | ? | quantile.py | 85 |
| M | ? | quantile.py | 93 |
| M | ? | quantile.py | 203 |
| M | ? | algorithms.py | 496 |
| M | ? | algorithms.py | 1105 |
| M | ? | gil.py | 60 |
| M | ? | gil.py | 63 |
| M | ? | index_cached_properties.py | 50 |
| M | ? | indexing.py | 130 |
| M | ? | indexing.py | 135 |
| M | ? | indexing_engines.py | 89 |
| M | ? | indexing_engines.py | 147 |
| H | ? | format.py | 1023 |
| H | ? | _openpyxl.py | 109 |
| H | ? | _odswriter.py | 92 |
| H | ? | excel.py | 83 |
| L | GS003 | eval_performance.py | 58 |
| L | GS003 | announce.py | 167 |
| L | GS003 | generate_version.py | 66 |
| L | GS003 | config.py | 340 |
| L | GS003 | _base.py | 763 |
| L | GS003 | sas7bdat.py | 508 |
| L | GS003 | _print_versions.py | 152 |
| L | GS003 | _print_versions.py | 153 |
| L | GS003 | _print_versions.py | 155 |
| L | GS003 | _print_versions.py | 156 |
| L | GS003 | _print_versions.py | 158 |
| L | GS003 | _tester.py | 56 |
| L | GS003 | check_test_naming.py | 86 |
| L | GS003 | check_test_naming.py | 92 |
| L | GS003 | check_test_naming.py | 132 |
| L | GS003 | run_vulture.py | 18 |
| L | GS003 | validate_rst_title_capitalization.py | 272 |
| L | GS003 | validate_unwanted_patterns.py | 537 |
| H | ? | pixi.lock | 17 |
| H | ? | pixi.lock | 132 |
| H | ? | pixi.lock | 370 |
| H | ? | pixi.lock | 485 |
| H | ? | pixi.lock | 941 |
| H | ? | pixi.lock | 1019 |
| H | ? | pixi.lock | 1254 |
| H | ? | pixi.lock | 1332 |
| H | ? | pixi.lock | 1549 |
| H | ? | pixi.lock | 1800 |
| H | ? | pixi.lock | 1860 |
| H | ? | pixi.lock | 1907 |
| H | ? | pixi.lock | 2022 |
| H | ? | pixi.lock | 2255 |
| H | ? | pixi.lock | 2336 |
| H | ? | pixi.lock | 2451 |
| H | ? | pixi.lock | 2683 |
| H | ? | pixi.lock | 2868 |
| H | ? | pixi.lock | 3051 |
| H | ? | pixi.lock | 3133 |
| H | ? | pixi.lock | 3257 |
| H | ? | pixi.lock | 3440 |
| H | ? | pixi.lock | 3522 |
| H | ? | pixi.lock | 3643 |
| H | ? | pixi.lock | 3807 |
| H | ? | pixi.lock | 3911 |
| H | ? | pixi.lock | 4026 |
| H | ? | pixi.lock | 4263 |
| H | ? | pixi.lock | 4378 |
| H | ? | pixi.lock | 4833 |
| H | ? | pixi.lock | 4910 |
| H | ? | pixi.lock | 5145 |
| H | ? | pixi.lock | 5222 |
| H | ? | pixi.lock | 5439 |
| H | ? | pixi.lock | 5619 |
| H | ? | pixi.lock | 5853 |
| H | ? | pixi.lock | 6160 |
| H | ? | pixi.lock | 6221 |
| H | ? | pixi.lock | 6393 |
| H | ? | pixi.lock | 6454 |
| H | ? | pixi.lock | 6607 |
| H | ? | pixi.lock | 6912 |
| H | ? | pixi.lock | 7015 |
| H | ? | pixi.lock | 7122 |
| H | ? | pixi.lock | 7378 |
| H | ? | pixi.lock | 7487 |
| H | ? | pixi.lock | 7955 |
| H | ? | pixi.lock | 8262 |
| H | ? | pixi.lock | 8559 |
| H | ? | pixi.lock | 8647 |
| H | ? | pixi.lock | 8752 |
| H | ? | pixi.lock | 8999 |
| H | ? | pixi.lock | 9104 |
| H | ? | pixi.lock | 9564 |
| H | ? | pixi.lock | 9642 |
| H | ? | pixi.lock | 9871 |
| H | ? | pixi.lock | 9949 |
| H | ? | pixi.lock | 10160 |
| H | ? | pixi.lock | 10454 |
| H | ? | pixi.lock | 10530 |
| H | ? | pixi.lock | 10592 |
| H | ? | pixi.lock | 10715 |
| H | ? | pixi.lock | 10974 |
| H | ? | pixi.lock | 11097 |
| H | ? | pixi.lock | 11589 |
| H | ? | pixi.lock | 11676 |
| H | ? | pixi.lock | 11926 |
| H | ? | pixi.lock | 12013 |
| H | ? | pixi.lock | 12243 |
| H | ? | pixi.lock | 12342 |
| H | ? | pixi.lock | 12465 |
| H | ? | pixi.lock | 12724 |
| H | ? | pixi.lock | 12847 |
| H | ? | pixi.lock | 13339 |
| H | ? | pixi.lock | 13426 |
| H | ? | pixi.lock | 13676 |
| H | ? | pixi.lock | 13763 |
| H | ? | pixi.lock | 13993 |
| H | ? | pixi.lock | 14092 |
| H | ? | pixi.lock | 14215 |
| H | ? | pixi.lock | 14472 |
| H | ? | pixi.lock | 14595 |
| H | ? | pixi.lock | 15084 |
| H | ? | pixi.lock | 15172 |
| H | ? | pixi.lock | 15420 |
| H | ? | pixi.lock | 15508 |
| H | ? | pixi.lock | 15736 |
| H | ? | pixi.lock | 16065 |
| H | ? | pixi.lock | 16151 |
| H | ? | pixi.lock | 16225 |
| H | ? | pixi.lock | 16345 |
| H | ? | pixi.lock | 16607 |
| H | ? | pixi.lock | 16727 |
| H | ? | pixi.lock | 17226 |
| H | ? | pixi.lock | 17312 |
| H | ? | pixi.lock | 17564 |
| H | ? | pixi.lock | 17650 |
| H | ? | pixi.lock | 17882 |
| H | ? | pixi.lock | 18207 |
| H | ? | pixi.lock | 18292 |
| H | ? | pixi.lock | 18367 |
| H | ? | pixi.lock | 18483 |
| H | ? | pixi.lock | 18725 |
| H | ? | pixi.lock | 18737 |
| H | ? | pixi.lock | 18738 |
| H | ? | pixi.lock | 18739 |
| H | ? | pixi.lock | 18740 |
| H | ? | pixi.lock | 18758 |
| H | ? | pixi.lock | 18874 |
| H | ? | pixi.lock | 19115 |
| H | ? | pixi.lock | 19127 |
| H | ? | pixi.lock | 19128 |
| H | ? | pixi.lock | 19129 |
| H | ? | pixi.lock | 19130 |
| H | ? | pixi.lock | 19264 |
| H | ? | pixi.lock | 19276 |
| H | ? | pixi.lock | 19277 |
| H | ? | pixi.lock | 19278 |
| H | ? | pixi.lock | 19279 |
| H | ? | pixi.lock | 19402 |
| H | ? | pixi.lock | 19482 |
| H | ? | pixi.lock | 19615 |
| H | ? | pixi.lock | 19627 |
| H | ? | pixi.lock | 19628 |
| H | ? | pixi.lock | 19629 |
| H | ? | pixi.lock | 19630 |
| H | ? | pixi.lock | 19753 |
| H | ? | pixi.lock | 19833 |
| H | ? | pixi.lock | 19965 |
| H | ? | pixi.lock | 19976 |
| H | ? | pixi.lock | 19977 |
| H | ? | pixi.lock | 19978 |
| H | ? | pixi.lock | 19979 |
| H | ? | pixi.lock | 20084 |
| H | ? | pixi.lock | 20323 |
| H | ? | pixi.lock | 20334 |
| H | ? | pixi.lock | 20381 |
| H | ? | pixi.lock | 20382 |
| H | ? | pixi.lock | 20383 |
| H | ? | pixi.lock | 20384 |
| H | ? | pixi.lock | 20385 |
| H | ? | pixi.lock | 20391 |
| H | ? | pixi.lock | 20399 |
| H | ? | pixi.lock | 20400 |
| H | ? | pixi.lock | 20401 |
| H | ? | pixi.lock | 20402 |
| H | ? | pixi.lock | 20403 |
| H | ? | pixi.lock | 20409 |
| H | ? | pixi.lock | 20417 |
| H | ? | pixi.lock | 20424 |
| H | ? | pixi.lock | 20432 |
| H | ? | pixi.lock | 20440 |
| H | ? | pixi.lock | 20454 |
| H | ? | pixi.lock | 20466 |
| H | ? | pixi.lock | 20473 |
| H | ? | pixi.lock | 20479 |
| H | ? | pixi.lock | 20488 |
| H | ? | pixi.lock | 20494 |
| H | ? | pixi.lock | 20502 |
| H | ? | pixi.lock | 20503 |
| H | ? | pixi.lock | 20504 |
| H | ? | pixi.lock | 20511 |
| H | ? | pixi.lock | 20521 |
| H | ? | pixi.lock | 20522 |
| H | ? | pixi.lock | 20523 |
| H | ? | pixi.lock | 20529 |
| H | ? | pixi.lock | 20538 |
| H | ? | pixi.lock | 20539 |
| H | ? | pixi.lock | 20540 |
| H | ? | pixi.lock | 20541 |
| H | ? | pixi.lock | 20547 |
| H | ? | pixi.lock | 20555 |
| H | ? | pixi.lock | 20556 |
| H | ? | pixi.lock | 20557 |
| H | ? | pixi.lock | 20558 |
| H | ? | pixi.lock | 20564 |
| H | ? | pixi.lock | 20572 |
| H | ? | pixi.lock | 20573 |
| H | ? | pixi.lock | 20575 |
| H | ? | pixi.lock | 20580 |
| H | ? | pixi.lock | 20589 |
| H | ? | pixi.lock | 20590 |
| H | ? | pixi.lock | 20591 |
| H | ? | pixi.lock | 20597 |
| H | ? | pixi.lock | 20605 |
| H | ? | pixi.lock | 20606 |
| H | ? | pixi.lock | 20607 |
| H | ? | pixi.lock | 20613 |
| H | ? | pixi.lock | 20622 |
| H | ? | pixi.lock | 20623 |
| H | ? | pixi.lock | 20624 |
| H | ? | pixi.lock | 20630 |
| H | ? | pixi.lock | 20639 |
| H | ? | pixi.lock | 20640 |
| H | ? | pixi.lock | 20642 |
| H | ? | pixi.lock | 20643 |
| H | ? | pixi.lock | 20644 |
| H | ? | pixi.lock | 20645 |
| H | ? | pixi.lock | 20651 |
| H | ? | pixi.lock | 20659 |
| H | ? | pixi.lock | 20660 |
| H | ? | pixi.lock | 20661 |
| H | ? | pixi.lock | 20662 |
| H | ? | pixi.lock | 20663 |
| H | ? | pixi.lock | 20664 |
| H | ? | pixi.lock | 20671 |
| H | ? | pixi.lock | 20678 |
| H | ? | pixi.lock | 20684 |
| H | ? | pixi.lock | 20693 |
| H | ? | pixi.lock | 20699 |
| H | ? | pixi.lock | 20706 |
| H | ? | pixi.lock | 20712 |
| H | ? | pixi.lock | 20721 |
| H | ? | pixi.lock | 20727 |
| H | ? | pixi.lock | 20735 |
| H | ? | pixi.lock | 20736 |
| H | ? | pixi.lock | 20737 |
| H | ? | pixi.lock | 20738 |
| H | ? | pixi.lock | 20739 |
| H | ? | pixi.lock | 20740 |
| H | ? | pixi.lock | 20741 |
| H | ? | pixi.lock | 20742 |
| H | ? | pixi.lock | 20743 |
| H | ? | pixi.lock | 20750 |
| H | ? | pixi.lock | 20760 |
| H | ? | pixi.lock | 20761 |
| H | ? | pixi.lock | 20762 |
| H | ? | pixi.lock | 20763 |
| H | ? | pixi.lock | 20764 |
| H | ? | pixi.lock | 20765 |
| H | ? | pixi.lock | 20766 |
| H | ? | pixi.lock | 20767 |
| H | ? | pixi.lock | 20768 |
| H | ? | pixi.lock | 20774 |
| H | ? | pixi.lock | 20782 |
| H | ? | pixi.lock | 20783 |
| H | ? | pixi.lock | 20784 |
| H | ? | pixi.lock | 20785 |
| H | ? | pixi.lock | 20805 |
| H | ? | pixi.lock | 20806 |
| H | ? | pixi.lock | 20809 |
| H | ? | pixi.lock | 20831 |
| H | ? | pixi.lock | 20839 |
| H | ? | pixi.lock | 20848 |
| H | ? | pixi.lock | 20856 |
| H | ? | pixi.lock | 20857 |
| H | ? | pixi.lock | 20865 |
| H | ? | pixi.lock | 20873 |
| H | ? | pixi.lock | 20884 |
| H | ? | pixi.lock | 20892 |
| H | ? | pixi.lock | 20893 |
| H | ? | pixi.lock | 20894 |
| H | ? | pixi.lock | 20902 |
| H | ? | pixi.lock | 20961 |
| H | ? | pixi.lock | 21475 |
| H | ? | pixi.lock | 22649 |
| H | ? | pixi.lock | 22836 |
| H | ? | pixi.lock | 22844 |
| H | ? | pixi.lock | 22845 |
| H | ? | pixi.lock | 22846 |
| H | ? | pixi.lock | 22847 |
| H | ? | pixi.lock | 22848 |
| H | ? | pixi.lock | 22849 |
| H | ? | pixi.lock | 23020 |
| H | ? | pixi.lock | 23179 |
| H | ? | pixi.lock | 23192 |
| H | ? | pixi.lock | 23195 |
| H | ? | pixi.lock | 23200 |
| H | ? | pixi.lock | 23223 |
| H | ? | pixi.lock | 23225 |
| H | ? | pixi.lock | 23226 |
| H | ? | pixi.lock | 23227 |
| H | ? | pixi.lock | 23228 |
| H | ? | pixi.lock | 23239 |
| H | ? | pixi.lock | 23243 |
| H | ? | pixi.lock | 23262 |
| H | ? | pixi.lock | 23264 |
| H | ? | pixi.lock | 23265 |
| H | ? | pixi.lock | 23266 |
| H | ? | pixi.lock | 23267 |
| H | ? | pixi.lock | 23278 |
| H | ? | pixi.lock | 23282 |
| H | ? | pixi.lock | 23301 |
| H | ? | pixi.lock | 23303 |
| H | ? | pixi.lock | 23304 |
| H | ? | pixi.lock | 23305 |
| H | ? | pixi.lock | 23306 |
| H | ? | pixi.lock | 23317 |
| H | ? | pixi.lock | 23321 |
| H | ? | pixi.lock | 23340 |
| H | ? | pixi.lock | 23342 |
| H | ? | pixi.lock | 23343 |
| H | ? | pixi.lock | 23344 |
| H | ? | pixi.lock | 23345 |
| H | ? | pixi.lock | 23356 |
| H | ? | pixi.lock | 23360 |
| H | ? | pixi.lock | 23597 |
| H | ? | pixi.lock | 23617 |
| H | ? | pixi.lock | 23637 |
| H | ? | pixi.lock | 23657 |
| H | ? | pixi.lock | 23671 |
| H | ? | pixi.lock | 24060 |
| H | ? | pixi.lock | 24310 |
| H | ? | pixi.lock | 24333 |
| H | ? | pixi.lock | 24395 |
| H | ? | pixi.lock | 24419 |
| H | ? | pixi.lock | 24444 |
| H | ? | pixi.lock | 24472 |
| H | ? | pixi.lock | 24484 |
| H | ? | pixi.lock | 24694 |
| H | ? | pixi.lock | 24723 |
| H | ? | pixi.lock | 24768 |
| H | ? | pixi.lock | 24785 |
| H | ? | pixi.lock | 24802 |
| H | ? | pixi.lock | 24819 |
| H | ? | pixi.lock | 24903 |
| H | ? | pixi.lock | 24921 |
| H | ? | pixi.lock | 25037 |
| H | ? | pixi.lock | 25112 |
| H | ? | pixi.lock | 25121 |
| H | ? | pixi.lock | 25129 |
| H | ? | pixi.lock | 25139 |
| H | ? | pixi.lock | 25706 |
| H | ? | pixi.lock | 25720 |
| H | ? | pixi.lock | 25736 |
| H | ? | pixi.lock | 25750 |
| H | ? | pixi.lock | 25764 |
| H | ? | pixi.lock | 26662 |
| H | ? | pixi.lock | 26673 |
| H | ? | pixi.lock | 26688 |
| H | ? | pixi.lock | 26696 |
| H | ? | pixi.lock | 27234 |
| H | ? | pixi.lock | 28513 |
| H | ? | pixi.lock | 29013 |
| H | ? | pixi.lock | 29027 |
| H | ? | pixi.lock | 29089 |
| H | ? | pixi.lock | 29174 |
| H | ? | pixi.lock | 29411 |
| H | ? | pixi.lock | 29426 |
| H | ? | pixi.lock | 30534 |
| H | ? | pixi.lock | 30606 |
| H | ? | pixi.lock | 30622 |
| H | ? | pixi.lock | 30640 |
| H | ? | pixi.lock | 30656 |
| H | ? | pixi.lock | 30827 |
| H | ? | pixi.lock | 30837 |
| H | ? | pixi.lock | 30882 |
| H | ? | pixi.lock | 30883 |
| H | ? | pixi.lock | 30884 |
| H | ? | pixi.lock | 30885 |
| H | ? | pixi.lock | 30886 |
| H | ? | pixi.lock | 30892 |
| H | ? | pixi.lock | 30899 |
| H | ? | pixi.lock | 30900 |
| H | ? | pixi.lock | 30901 |
| H | ? | pixi.lock | 30902 |
| H | ? | pixi.lock | 30903 |
| H | ? | pixi.lock | 30909 |
| H | ? | pixi.lock | 30916 |
| H | ? | pixi.lock | 30923 |
| H | ? | pixi.lock | 30930 |
| H | ? | pixi.lock | 30938 |
| H | ? | pixi.lock | 30951 |
| H | ? | pixi.lock | 30963 |
| H | ? | pixi.lock | 30970 |
| H | ? | pixi.lock | 30976 |
| H | ? | pixi.lock | 30984 |
| H | ? | pixi.lock | 30990 |
| H | ? | pixi.lock | 30997 |
| H | ? | pixi.lock | 30998 |
| H | ? | pixi.lock | 30999 |
| H | ? | pixi.lock | 31006 |
| H | ? | pixi.lock | 31015 |
| H | ? | pixi.lock | 31016 |
| H | ? | pixi.lock | 31017 |
| H | ? | pixi.lock | 31023 |
| H | ? | pixi.lock | 31031 |
| H | ? | pixi.lock | 31032 |
| H | ? | pixi.lock | 31033 |
| H | ? | pixi.lock | 31034 |
| H | ? | pixi.lock | 31040 |
| H | ? | pixi.lock | 31047 |
| H | ? | pixi.lock | 31048 |
| H | ? | pixi.lock | 31049 |
| H | ? | pixi.lock | 31050 |
| H | ? | pixi.lock | 31056 |
| H | ? | pixi.lock | 31063 |
| H | ? | pixi.lock | 31064 |
| H | ? | pixi.lock | 31066 |
| H | ? | pixi.lock | 31071 |
| H | ? | pixi.lock | 31079 |
| H | ? | pixi.lock | 31080 |
| H | ? | pixi.lock | 31081 |
| H | ? | pixi.lock | 31087 |
| H | ? | pixi.lock | 31094 |
| H | ? | pixi.lock | 31095 |
| H | ? | pixi.lock | 31096 |
| H | ? | pixi.lock | 31102 |
| H | ? | pixi.lock | 31110 |
| H | ? | pixi.lock | 31111 |
| H | ? | pixi.lock | 31112 |
| H | ? | pixi.lock | 31118 |
| H | ? | pixi.lock | 31126 |
| H | ? | pixi.lock | 31127 |
| H | ? | pixi.lock | 31128 |
| H | ? | pixi.lock | 31129 |
| H | ? | pixi.lock | 31130 |
| H | ? | pixi.lock | 31132 |
| H | ? | pixi.lock | 31138 |
| H | ? | pixi.lock | 31145 |
| H | ? | pixi.lock | 31146 |
| H | ? | pixi.lock | 31147 |
| H | ? | pixi.lock | 31148 |
| H | ? | pixi.lock | 31149 |
| H | ? | pixi.lock | 31150 |
| H | ? | pixi.lock | 31157 |
| H | ? | pixi.lock | 31164 |
| H | ? | pixi.lock | 31170 |
| H | ? | pixi.lock | 31178 |
| H | ? | pixi.lock | 31184 |
| H | ? | pixi.lock | 31191 |
| H | ? | pixi.lock | 31197 |
| H | ? | pixi.lock | 31205 |
| H | ? | pixi.lock | 31211 |
| H | ? | pixi.lock | 31218 |
| H | ? | pixi.lock | 31219 |
| H | ? | pixi.lock | 31220 |
| H | ? | pixi.lock | 31221 |
| H | ? | pixi.lock | 31222 |
| H | ? | pixi.lock | 31223 |
| H | ? | pixi.lock | 31224 |
| H | ? | pixi.lock | 31225 |
| H | ? | pixi.lock | 31226 |
| H | ? | pixi.lock | 31233 |
| H | ? | pixi.lock | 31242 |
| H | ? | pixi.lock | 31243 |
| H | ? | pixi.lock | 31244 |
| H | ? | pixi.lock | 31245 |
| H | ? | pixi.lock | 31246 |
| H | ? | pixi.lock | 31247 |
| H | ? | pixi.lock | 31248 |
| H | ? | pixi.lock | 31249 |
| H | ? | pixi.lock | 31250 |
| H | ? | pixi.lock | 31256 |
| H | ? | pixi.lock | 31263 |
| H | ? | pixi.lock | 31264 |
| H | ? | pixi.lock | 31265 |
| H | ? | pixi.lock | 31266 |
| H | ? | pixi.lock | 31287 |
| H | ? | pixi.lock | 31288 |
| H | ? | pixi.lock | 31289 |
| H | ? | pixi.lock | 31310 |
| H | ? | pixi.lock | 31317 |
| H | ? | pixi.lock | 31326 |
| H | ? | pixi.lock | 31333 |
| H | ? | pixi.lock | 31334 |
| H | ? | pixi.lock | 31342 |
| H | ? | pixi.lock | 31349 |
| H | ? | pixi.lock | 31360 |
| H | ? | pixi.lock | 31367 |
| H | ? | pixi.lock | 31368 |
| H | ? | pixi.lock | 31369 |
| H | ? | pixi.lock | 31377 |
| H | ? | pixi.lock | 31433 |
| H | ? | pixi.lock | 31964 |
| H | ? | pixi.lock | 33103 |
| H | ? | pixi.lock | 33286 |
| H | ? | pixi.lock | 33293 |
| H | ? | pixi.lock | 33294 |
| H | ? | pixi.lock | 33295 |
| H | ? | pixi.lock | 33296 |
| H | ? | pixi.lock | 33297 |
| H | ? | pixi.lock | 33298 |
| H | ? | pixi.lock | 33460 |
| H | ? | pixi.lock | 33619 |
| H | ? | pixi.lock | 33632 |
| H | ? | pixi.lock | 33635 |
| H | ? | pixi.lock | 33640 |
| H | ? | pixi.lock | 33662 |
| H | ? | pixi.lock | 33664 |
| H | ? | pixi.lock | 33665 |
| H | ? | pixi.lock | 33666 |
| H | ? | pixi.lock | 33667 |
| H | ? | pixi.lock | 33678 |
| H | ? | pixi.lock | 33682 |
| H | ? | pixi.lock | 33700 |
| H | ? | pixi.lock | 33702 |
| H | ? | pixi.lock | 33703 |
| H | ? | pixi.lock | 33704 |
| H | ? | pixi.lock | 33705 |
| H | ? | pixi.lock | 33716 |
| H | ? | pixi.lock | 33720 |
| H | ? | pixi.lock | 33738 |
| H | ? | pixi.lock | 33740 |
| H | ? | pixi.lock | 33741 |
| H | ? | pixi.lock | 33742 |
| H | ? | pixi.lock | 33743 |
| H | ? | pixi.lock | 33754 |
| H | ? | pixi.lock | 33758 |
| H | ? | pixi.lock | 33776 |
| H | ? | pixi.lock | 33778 |
| H | ? | pixi.lock | 33779 |
| H | ? | pixi.lock | 33780 |
| H | ? | pixi.lock | 33781 |
| H | ? | pixi.lock | 33792 |
| H | ? | pixi.lock | 33796 |
| H | ? | pixi.lock | 34020 |
| H | ? | pixi.lock | 34039 |
| H | ? | pixi.lock | 34058 |
| H | ? | pixi.lock | 34077 |
| H | ? | pixi.lock | 34091 |
| H | ? | pixi.lock | 34459 |
| H | ? | pixi.lock | 34700 |
| H | ? | pixi.lock | 34722 |
| H | ? | pixi.lock | 34782 |
| H | ? | pixi.lock | 34805 |
| H | ? | pixi.lock | 34829 |
| H | ? | pixi.lock | 34856 |
| H | ? | pixi.lock | 34867 |
| H | ? | pixi.lock | 35063 |
| H | ? | pixi.lock | 35091 |
| H | ? | pixi.lock | 35134 |
| H | ? | pixi.lock | 35150 |
| H | ? | pixi.lock | 35166 |
| H | ? | pixi.lock | 35182 |
| H | ? | pixi.lock | 35261 |
| H | ? | pixi.lock | 35278 |
| H | ? | pixi.lock | 35376 |
| H | ? | pixi.lock | 35468 |
| H | ? | pixi.lock | 35477 |
| H | ? | pixi.lock | 35484 |
| H | ? | pixi.lock | 35494 |
| H | ? | pixi.lock | 36037 |
| H | ? | pixi.lock | 36051 |
| H | ? | pixi.lock | 36066 |
| H | ? | pixi.lock | 36080 |
| H | ? | pixi.lock | 36094 |
| H | ? | pixi.lock | 36971 |
| H | ? | pixi.lock | 36982 |
| H | ? | pixi.lock | 36993 |
| H | ? | pixi.lock | 37004 |
| H | ? | pixi.lock | 37536 |
| H | ? | pixi.lock | 38756 |
| H | ? | pixi.lock | 39216 |
| H | ? | pixi.lock | 39230 |
| H | ? | pixi.lock | 39291 |
| H | ? | pixi.lock | 39365 |
| H | ? | pixi.lock | 39608 |
| H | ? | pixi.lock | 39622 |
| H | ? | pixi.lock | 40665 |
| H | ? | pixi.lock | 40734 |
| H | ? | pixi.lock | 40750 |
| H | ? | pixi.lock | 40768 |
| H | ? | pixi.lock | 40784 |
| H | ? | pixi.lock | 40825 |
| H | ? | pixi.lock | 40842 |
| H | ? | pixi.lock | 40857 |
| H | ? | pixi.lock | 40872 |
| H | ? | pixi.lock | 40889 |
| H | ? | pixi.lock | 40904 |
| H | ? | pixi.lock | 41539 |
| H | ? | pixi.lock | 41540 |
| H | ? | pixi.lock | 41618 |
| H | ? | pixi.lock | 41898 |
| H | ? | pixi.lock | 42332 |
| H | ? | pixi.lock | 43491 |
| H | ? | pixi.lock | 44411 |
| H | ? | pixi.lock | 44878 |
| H | ? | pixi.lock | 44888 |
| H | ? | pixi.lock | 44898 |
| H | ? | pixi.lock | 44908 |
| H | ? | pixi.lock | 45457 |
| H | ? | pixi.lock | 45458 |
| H | ? | pixi.lock | 45459 |
| H | ? | pixi.lock | 45460 |
| H | ? | pixi.lock | 45461 |
| H | ? | pixi.lock | 45467 |
| H | ? | pixi.lock | 45475 |
| H | ? | pixi.lock | 45476 |
| H | ? | pixi.lock | 45477 |
| H | ? | pixi.lock | 45478 |
| H | ? | pixi.lock | 45479 |
| H | ? | pixi.lock | 45484 |
| H | ? | pixi.lock | 45492 |
| H | ? | pixi.lock | 45493 |
| H | ? | pixi.lock | 45494 |
| H | ? | pixi.lock | 45495 |
| H | ? | pixi.lock | 45496 |
| H | ? | pixi.lock | 45501 |
| H | ? | pixi.lock | 45509 |
| H | ? | pixi.lock | 45515 |
| H | ? | pixi.lock | 45523 |
| H | ? | pixi.lock | 45529 |
| H | ? | pixi.lock | 45541 |
| H | ? | pixi.lock | 45554 |
| H | ? | pixi.lock | 45562 |
| H | ? | pixi.lock | 45567 |
| H | ? | pixi.lock | 45575 |
| H | ? | pixi.lock | 45581 |
| H | ? | pixi.lock | 45589 |
| H | ? | pixi.lock | 45590 |
| H | ? | pixi.lock | 45591 |
| H | ? | pixi.lock | 45597 |
| H | ? | pixi.lock | 45606 |
| H | ? | pixi.lock | 45607 |
| H | ? | pixi.lock | 45608 |
| H | ? | pixi.lock | 45614 |
| H | ? | pixi.lock | 45622 |
| H | ? | pixi.lock | 45623 |
| H | ? | pixi.lock | 45624 |
| H | ? | pixi.lock | 45625 |
| H | ? | pixi.lock | 45631 |
| H | ? | pixi.lock | 45639 |
| H | ? | pixi.lock | 45640 |
| H | ? | pixi.lock | 45641 |
| H | ? | pixi.lock | 45642 |
| H | ? | pixi.lock | 45647 |
| H | ? | pixi.lock | 45655 |
| H | ? | pixi.lock | 45656 |
| H | ? | pixi.lock | 45661 |
| H | ? | pixi.lock | 45669 |
| H | ? | pixi.lock | 45670 |
| H | ? | pixi.lock | 45676 |
| H | ? | pixi.lock | 45684 |
| H | ? | pixi.lock | 45685 |
| H | ? | pixi.lock | 45686 |
| H | ? | pixi.lock | 45691 |
| H | ? | pixi.lock | 45699 |
| H | ? | pixi.lock | 45700 |
| H | ? | pixi.lock | 45701 |
| H | ? | pixi.lock | 45706 |
| H | ? | pixi.lock | 45714 |
| H | ? | pixi.lock | 45715 |
| H | ? | pixi.lock | 45716 |
| H | ? | pixi.lock | 45722 |
| H | ? | pixi.lock | 45730 |
| H | ? | pixi.lock | 45731 |
| H | ? | pixi.lock | 45732 |
| H | ? | pixi.lock | 45733 |
| H | ? | pixi.lock | 45734 |
| H | ? | pixi.lock | 45735 |
| H | ? | pixi.lock | 45740 |
| H | ? | pixi.lock | 45748 |
| H | ? | pixi.lock | 45749 |
| H | ? | pixi.lock | 45750 |
| H | ? | pixi.lock | 45751 |
| H | ? | pixi.lock | 45752 |
| H | ? | pixi.lock | 45753 |
| H | ? | pixi.lock | 45759 |
| H | ? | pixi.lock | 45767 |
| H | ? | pixi.lock | 45768 |
| H | ? | pixi.lock | 45769 |
| H | ? | pixi.lock | 45770 |
| H | ? | pixi.lock | 45771 |
| H | ? | pixi.lock | 45772 |
| H | ? | pixi.lock | 45777 |
| H | ? | pixi.lock | 45785 |
| H | ? | pixi.lock | 45790 |
| H | ? | pixi.lock | 45798 |
| H | ? | pixi.lock | 45803 |
| H | ? | pixi.lock | 45811 |
| H | ? | pixi.lock | 45817 |
| H | ? | pixi.lock | 45825 |
| H | ? | pixi.lock | 45831 |
| H | ? | pixi.lock | 45839 |
| H | ? | pixi.lock | 45844 |
| H | ? | pixi.lock | 45852 |
| H | ? | pixi.lock | 45853 |
| H | ? | pixi.lock | 45854 |
| H | ? | pixi.lock | 45855 |
| H | ? | pixi.lock | 45856 |
| H | ? | pixi.lock | 45857 |
| H | ? | pixi.lock | 45858 |
| H | ? | pixi.lock | 45859 |
| H | ? | pixi.lock | 45860 |
| H | ? | pixi.lock | 45866 |
| H | ? | pixi.lock | 45875 |
| H | ? | pixi.lock | 45876 |
| H | ? | pixi.lock | 45877 |
| H | ? | pixi.lock | 45878 |
| H | ? | pixi.lock | 45879 |
| H | ? | pixi.lock | 45880 |
| H | ? | pixi.lock | 45881 |
| H | ? | pixi.lock | 45882 |
| H | ? | pixi.lock | 45883 |
| H | ? | pixi.lock | 45888 |
| H | ? | pixi.lock | 45897 |
| H | ? | pixi.lock | 45898 |
| H | ? | pixi.lock | 45899 |
| H | ? | pixi.lock | 45900 |
| H | ? | pixi.lock | 45901 |
| H | ? | pixi.lock | 45902 |
| H | ? | pixi.lock | 45903 |
| H | ? | pixi.lock | 45904 |
| H | ? | pixi.lock | 45905 |
| H | ? | pixi.lock | 45911 |
| H | ? | pixi.lock | 45919 |
| H | ? | pixi.lock | 45920 |
| H | ? | pixi.lock | 45921 |
| H | ? | pixi.lock | 45922 |
| H | ? | pixi.lock | 45941 |
| H | ? | pixi.lock | 45943 |
| H | ? | pixi.lock | 45944 |
| H | ? | pixi.lock | 45958 |
| H | ? | pixi.lock | 45960 |
| H | ? | pixi.lock | 45961 |
| H | ? | pixi.lock | 45983 |
| H | ? | pixi.lock | 45991 |
| H | ? | pixi.lock | 45999 |
| H | ? | pixi.lock | 46007 |
| H | ? | pixi.lock | 46008 |
| H | ? | pixi.lock | 46015 |
| H | ? | pixi.lock | 46023 |
| H | ? | pixi.lock | 46033 |
| H | ? | pixi.lock | 46041 |
| H | ? | pixi.lock | 46042 |
| H | ? | pixi.lock | 46043 |
| H | ? | pixi.lock | 46050 |
| H | ? | pixi.lock | 47810 |
| H | ? | pixi.lock | 47818 |
| H | ? | pixi.lock | 47819 |
| H | ? | pixi.lock | 47820 |
| H | ? | pixi.lock | 47821 |
| H | ? | pixi.lock | 47822 |
| H | ? | pixi.lock | 47823 |
| H | ? | pixi.lock | 47843 |
| H | ? | pixi.lock | 47844 |
| H | ? | pixi.lock | 47845 |
| H | ? | pixi.lock | 47846 |
| H | ? | pixi.lock | 47847 |
| H | ? | pixi.lock | 47848 |
| H | ? | pixi.lock | 47981 |
| H | ? | pixi.lock | 48033 |
| H | ? | pixi.lock | 48172 |
| H | ? | pixi.lock | 48187 |
| H | ? | pixi.lock | 48208 |
| H | ? | pixi.lock | 48210 |
| H | ? | pixi.lock | 48211 |
| H | ? | pixi.lock | 48212 |
| H | ? | pixi.lock | 48213 |
| H | ? | pixi.lock | 48224 |
| H | ? | pixi.lock | 48227 |
| H | ? | pixi.lock | 48247 |
| H | ? | pixi.lock | 48249 |
| H | ? | pixi.lock | 48250 |
| H | ? | pixi.lock | 48251 |
| H | ? | pixi.lock | 48252 |
| H | ? | pixi.lock | 48263 |
| H | ? | pixi.lock | 48266 |
| H | ? | pixi.lock | 48285 |
| H | ? | pixi.lock | 48287 |
| H | ? | pixi.lock | 48288 |
| H | ? | pixi.lock | 48289 |
| H | ? | pixi.lock | 48290 |
| H | ? | pixi.lock | 48301 |
| H | ? | pixi.lock | 48304 |
| H | ? | pixi.lock | 48323 |
| H | ? | pixi.lock | 48325 |
| H | ? | pixi.lock | 48326 |
| H | ? | pixi.lock | 48327 |
| H | ? | pixi.lock | 48328 |
| H | ? | pixi.lock | 48339 |
| H | ? | pixi.lock | 48342 |
| H | ? | pixi.lock | 48383 |
| H | ? | pixi.lock | 48403 |
| H | ? | pixi.lock | 48422 |
| H | ? | pixi.lock | 48441 |
| H | ? | pixi.lock | 48460 |
| H | ? | pixi.lock | 48482 |
| H | ? | pixi.lock | 48503 |
| H | ? | pixi.lock | 48524 |
| H | ? | pixi.lock | 48566 |
| H | ? | pixi.lock | 48588 |
| H | ? | pixi.lock | 48609 |
| H | ? | pixi.lock | 48630 |
| H | ? | pixi.lock | 48649 |
| H | ? | pixi.lock | 48666 |
| H | ? | pixi.lock | 48704 |
| H | ? | pixi.lock | 48724 |
| H | ? | pixi.lock | 48744 |
| H | ? | pixi.lock | 48763 |
| H | ? | pixi.lock | 48782 |
| H | ? | pixi.lock | 48795 |
| H | ? | pixi.lock | 49045 |
| H | ? | pixi.lock | 49057 |
| H | ? | pixi.lock | 49112 |
| H | ? | pixi.lock | 49234 |
| H | ? | pixi.lock | 49256 |
| H | ? | pixi.lock | 49316 |
| H | ? | pixi.lock | 49339 |
| H | ? | pixi.lock | 49363 |
| H | ? | pixi.lock | 49415 |
| H | ? | pixi.lock | 49426 |
| H | ? | pixi.lock | 49648 |
| H | ? | pixi.lock | 49666 |
| H | ? | pixi.lock | 49709 |
| H | ? | pixi.lock | 49729 |
| H | ? | pixi.lock | 49730 |
| H | ? | pixi.lock | 49750 |
| H | ? | pixi.lock | 49751 |
| H | ? | pixi.lock | 49770 |
| H | ? | pixi.lock | 49771 |
| H | ? | pixi.lock | 49790 |
| H | ? | pixi.lock | 49791 |
| H | ? | pixi.lock | 49857 |
| H | ? | pixi.lock | 49874 |
| H | ? | pixi.lock | 49950 |
| H | ? | pixi.lock | 50000 |
| H | ? | pixi.lock | 50007 |
| H | ? | pixi.lock | 50016 |
| H | ? | pixi.lock | 50024 |
| H | ? | pixi.lock | 50536 |
| H | ? | pixi.lock | 50549 |
| H | ? | pixi.lock | 50564 |
| H | ? | pixi.lock | 50577 |
| H | ? | pixi.lock | 50590 |
| H | ? | pixi.lock | 51421 |
| H | ? | pixi.lock | 51431 |
| H | ? | pixi.lock | 51441 |
| H | ? | pixi.lock | 51453 |
| H | ? | pixi.lock | 52998 |
| H | ? | pixi.lock | 54022 |
| H | ? | pixi.lock | 54358 |
| H | ? | pixi.lock | 54427 |
| H | ? | pixi.lock | 54442 |
| H | ? | pixi.lock | 54459 |
| H | ? | pixi.lock | 54474 |
| H | ? | pixi.lock | 54684 |
| H | ? | pixi.lock | 54685 |
| H | ? | pixi.lock | 54686 |
| H | ? | pixi.lock | 54687 |
| H | ? | pixi.lock | 54688 |
| H | ? | pixi.lock | 54694 |
| H | ? | pixi.lock | 54702 |
| H | ? | pixi.lock | 54703 |
| H | ? | pixi.lock | 54704 |
| H | ? | pixi.lock | 54705 |
| H | ? | pixi.lock | 54706 |
| H | ? | pixi.lock | 54711 |
| H | ? | pixi.lock | 54719 |
| H | ? | pixi.lock | 54725 |
| H | ? | pixi.lock | 54733 |
| H | ? | pixi.lock | 54739 |
| H | ? | pixi.lock | 54752 |
| H | ? | pixi.lock | 54764 |
| H | ? | pixi.lock | 54772 |
| H | ? | pixi.lock | 54777 |
| H | ? | pixi.lock | 54785 |
| H | ? | pixi.lock | 54791 |
| H | ? | pixi.lock | 54799 |
| H | ? | pixi.lock | 54800 |
| H | ? | pixi.lock | 54801 |
| H | ? | pixi.lock | 54807 |
| H | ? | pixi.lock | 54816 |
| H | ? | pixi.lock | 54817 |
| H | ? | pixi.lock | 54818 |
| H | ? | pixi.lock | 54824 |
| H | ? | pixi.lock | 54832 |
| H | ? | pixi.lock | 54833 |
| H | ? | pixi.lock | 54834 |
| H | ? | pixi.lock | 54835 |
| H | ? | pixi.lock | 54841 |
| H | ? | pixi.lock | 54849 |
| H | ? | pixi.lock | 54850 |
| H | ? | pixi.lock | 54851 |
| H | ? | pixi.lock | 54852 |
| H | ? | pixi.lock | 54857 |
| H | ? | pixi.lock | 54865 |
| H | ? | pixi.lock | 54866 |
| H | ? | pixi.lock | 54871 |
| H | ? | pixi.lock | 54879 |
| H | ? | pixi.lock | 54880 |
| H | ? | pixi.lock | 54886 |
| H | ? | pixi.lock | 54894 |
| H | ? | pixi.lock | 54895 |
| H | ? | pixi.lock | 54896 |
| H | ? | pixi.lock | 54901 |
| H | ? | pixi.lock | 54909 |
| H | ? | pixi.lock | 54910 |
| H | ? | pixi.lock | 54911 |
| H | ? | pixi.lock | 54917 |
| H | ? | pixi.lock | 54925 |
| H | ? | pixi.lock | 54926 |
| H | ? | pixi.lock | 54927 |
| H | ? | pixi.lock | 54928 |
| H | ? | pixi.lock | 54929 |
| H | ? | pixi.lock | 54930 |
| H | ? | pixi.lock | 54936 |
| H | ? | pixi.lock | 54944 |
| H | ? | pixi.lock | 54945 |
| H | ? | pixi.lock | 54946 |
| H | ? | pixi.lock | 54947 |
| H | ? | pixi.lock | 54948 |
| H | ? | pixi.lock | 54949 |
| H | ? | pixi.lock | 54954 |
| H | ? | pixi.lock | 54962 |
| H | ? | pixi.lock | 54967 |
| H | ? | pixi.lock | 54975 |
| H | ? | pixi.lock | 54981 |
| H | ? | pixi.lock | 54989 |
| H | ? | pixi.lock | 54994 |
| H | ? | pixi.lock | 55002 |
| H | ? | pixi.lock | 55008 |
| H | ? | pixi.lock | 55016 |
| H | ? | pixi.lock | 55017 |
| H | ? | pixi.lock | 55018 |
| H | ? | pixi.lock | 55019 |
| H | ? | pixi.lock | 55020 |
| H | ? | pixi.lock | 55021 |
| H | ? | pixi.lock | 55022 |
| H | ? | pixi.lock | 55023 |
| H | ? | pixi.lock | 55024 |
| H | ? | pixi.lock | 55030 |
| H | ? | pixi.lock | 55039 |
| H | ? | pixi.lock | 55040 |
| H | ? | pixi.lock | 55041 |
| H | ? | pixi.lock | 55042 |
| H | ? | pixi.lock | 55043 |
| H | ? | pixi.lock | 55044 |
| H | ? | pixi.lock | 55045 |
| H | ? | pixi.lock | 55046 |
| H | ? | pixi.lock | 55047 |
| H | ? | pixi.lock | 55053 |
| H | ? | pixi.lock | 55061 |
| H | ? | pixi.lock | 55062 |
| H | ? | pixi.lock | 55063 |
| H | ? | pixi.lock | 55064 |
| H | ? | pixi.lock | 55082 |
| H | ? | pixi.lock | 55083 |
| H | ? | pixi.lock | 55086 |
| H | ? | pixi.lock | 55107 |
| H | ? | pixi.lock | 55115 |
| H | ? | pixi.lock | 55123 |
| H | ? | pixi.lock | 55131 |
| H | ? | pixi.lock | 55132 |
| H | ? | pixi.lock | 55139 |
| H | ? | pixi.lock | 55147 |
| H | ? | pixi.lock | 55157 |
| H | ? | pixi.lock | 55165 |
| H | ? | pixi.lock | 55166 |
| H | ? | pixi.lock | 55167 |
| H | ? | pixi.lock | 55174 |
| H | ? | pixi.lock | 57009 |
| H | ? | pixi.lock | 57017 |
| H | ? | pixi.lock | 57018 |
| H | ? | pixi.lock | 57019 |
| H | ? | pixi.lock | 57020 |
| H | ? | pixi.lock | 57021 |
| H | ? | pixi.lock | 57022 |
| H | ? | pixi.lock | 57159 |
| H | ? | pixi.lock | 57224 |
| H | ? | pixi.lock | 57363 |
| H | ? | pixi.lock | 57375 |
| H | ? | pixi.lock | 57377 |
| H | ? | pixi.lock | 57382 |
| H | ? | pixi.lock | 57404 |
| H | ? | pixi.lock | 57406 |
| H | ? | pixi.lock | 57407 |
| H | ? | pixi.lock | 57408 |
| H | ? | pixi.lock | 57409 |
| H | ? | pixi.lock | 57420 |
| H | ? | pixi.lock | 57423 |
| H | ? | pixi.lock | 57442 |
| H | ? | pixi.lock | 57444 |
| H | ? | pixi.lock | 57445 |
| H | ? | pixi.lock | 57446 |
| H | ? | pixi.lock | 57447 |
| H | ? | pixi.lock | 57458 |
| H | ? | pixi.lock | 57461 |
| H | ? | pixi.lock | 57480 |
| H | ? | pixi.lock | 57482 |
| H | ? | pixi.lock | 57483 |
| H | ? | pixi.lock | 57484 |
| H | ? | pixi.lock | 57485 |
| H | ? | pixi.lock | 57496 |
| H | ? | pixi.lock | 57499 |
| H | ? | pixi.lock | 57518 |
| H | ? | pixi.lock | 57520 |
| H | ? | pixi.lock | 57521 |
| H | ? | pixi.lock | 57522 |
| H | ? | pixi.lock | 57523 |
| H | ? | pixi.lock | 57534 |
| H | ? | pixi.lock | 57537 |
| H | ? | pixi.lock | 57563 |
| H | ? | pixi.lock | 57582 |
| H | ? | pixi.lock | 57601 |
| H | ? | pixi.lock | 57620 |
| H | ? | pixi.lock | 57639 |
| H | ? | pixi.lock | 57660 |
| H | ? | pixi.lock | 57681 |
| H | ? | pixi.lock | 57702 |
| H | ? | pixi.lock | 57727 |
| H | ? | pixi.lock | 57748 |
| H | ? | pixi.lock | 57769 |
| H | ? | pixi.lock | 57790 |
| H | ? | pixi.lock | 57810 |
| H | ? | pixi.lock | 57829 |
| H | ? | pixi.lock | 57848 |
| H | ? | pixi.lock | 57867 |
| H | ? | pixi.lock | 57880 |
| H | ? | pixi.lock | 58129 |
| H | ? | pixi.lock | 58185 |
| H | ? | pixi.lock | 58307 |
| H | ? | pixi.lock | 58329 |
| H | ? | pixi.lock | 58388 |
| H | ? | pixi.lock | 58411 |
| H | ? | pixi.lock | 58435 |
| H | ? | pixi.lock | 58487 |
| H | ? | pixi.lock | 58498 |
| H | ? | pixi.lock | 58718 |
| H | ? | pixi.lock | 58736 |
| H | ? | pixi.lock | 58782 |
| H | ? | pixi.lock | 58783 |
| H | ? | pixi.lock | 58802 |
| H | ? | pixi.lock | 58803 |
| H | ? | pixi.lock | 58822 |
| H | ? | pixi.lock | 58823 |
| H | ? | pixi.lock | 58842 |
| H | ? | pixi.lock | 58843 |
| H | ? | pixi.lock | 58909 |
| H | ? | pixi.lock | 58926 |
| H | ? | pixi.lock | 59001 |
| H | ? | pixi.lock | 59049 |
| H | ? | pixi.lock | 59056 |
| H | ? | pixi.lock | 59065 |
| H | ? | pixi.lock | 59073 |
| H | ? | pixi.lock | 59597 |
| H | ? | pixi.lock | 59610 |
| H | ? | pixi.lock | 59625 |
| H | ? | pixi.lock | 59638 |
| H | ? | pixi.lock | 59651 |
| H | ? | pixi.lock | 60511 |
| H | ? | pixi.lock | 60521 |
| H | ? | pixi.lock | 60534 |
| H | ? | pixi.lock | 60543 |
| H | ? | pixi.lock | 61061 |
| H | ? | pixi.lock | 62089 |
| H | ? | pixi.lock | 63123 |
| H | ? | pixi.lock | 63476 |
| H | ? | pixi.lock | 63546 |
| H | ? | pixi.lock | 63562 |
| H | ? | pixi.lock | 63580 |
| H | ? | pixi.lock | 63596 |
| H | ? | pixi.lock | 63817 |
| H | ? | pixi.lock | 63818 |
| H | ? | pixi.lock | 63819 |
| H | ? | pixi.lock | 63820 |
| H | ? | pixi.lock | 63821 |
| H | ? | pixi.lock | 63827 |
| H | ? | pixi.lock | 63834 |
| H | ? | pixi.lock | 63835 |
| H | ? | pixi.lock | 63836 |
| H | ? | pixi.lock | 63837 |
| H | ? | pixi.lock | 63838 |
| H | ? | pixi.lock | 63846 |
| H | ? | pixi.lock | 63853 |
| H | ? | pixi.lock | 63862 |
| H | ? | pixi.lock | 63869 |
| H | ? | pixi.lock | 63878 |
| H | ? | pixi.lock | 63893 |
| H | ? | pixi.lock | 63907 |
| H | ? | pixi.lock | 63914 |
| H | ? | pixi.lock | 63922 |
| H | ? | pixi.lock | 63932 |
| H | ? | pixi.lock | 63938 |
| H | ? | pixi.lock | 63945 |
| H | ? | pixi.lock | 63946 |
| H | ? | pixi.lock | 63947 |
| H | ? | pixi.lock | 63955 |
| H | ? | pixi.lock | 63965 |
| H | ? | pixi.lock | 63966 |
| H | ? | pixi.lock | 63967 |
| H | ? | pixi.lock | 63973 |
| H | ? | pixi.lock | 63983 |
| H | ? | pixi.lock | 63984 |
| H | ? | pixi.lock | 63985 |
| H | ? | pixi.lock | 63986 |
| H | ? | pixi.lock | 63992 |
| H | ? | pixi.lock | 63999 |
| H | ? | pixi.lock | 64000 |
| H | ? | pixi.lock | 64001 |
| H | ? | pixi.lock | 64002 |
| H | ? | pixi.lock | 64010 |
| H | ? | pixi.lock | 64017 |
| H | ? | pixi.lock | 64018 |
| H | ? | pixi.lock | 64026 |
| H | ? | pixi.lock | 64036 |
| H | ? | pixi.lock | 64037 |
| H | ? | pixi.lock | 64043 |
| H | ? | pixi.lock | 64050 |
| H | ? | pixi.lock | 64051 |
| H | ? | pixi.lock | 64052 |
| H | ? | pixi.lock | 64060 |
| H | ? | pixi.lock | 64070 |
| H | ? | pixi.lock | 64071 |
| H | ? | pixi.lock | 64072 |
| H | ? | pixi.lock | 64078 |
| H | ? | pixi.lock | 64088 |
| H | ? | pixi.lock | 64089 |
| H | ? | pixi.lock | 64090 |
| H | ? | pixi.lock | 64091 |
| H | ? | pixi.lock | 64092 |
| H | ? | pixi.lock | 64093 |
| H | ? | pixi.lock | 64099 |
| H | ? | pixi.lock | 64106 |
| H | ? | pixi.lock | 64107 |
| H | ? | pixi.lock | 64108 |
| H | ? | pixi.lock | 64109 |
| H | ? | pixi.lock | 64110 |
| H | ? | pixi.lock | 64111 |
| H | ? | pixi.lock | 64119 |
| H | ? | pixi.lock | 64126 |
| H | ? | pixi.lock | 64134 |
| H | ? | pixi.lock | 64144 |
| H | ? | pixi.lock | 64150 |
| H | ? | pixi.lock | 64157 |
| H | ? | pixi.lock | 64165 |
| H | ? | pixi.lock | 64175 |
| H | ? | pixi.lock | 64181 |
| H | ? | pixi.lock | 64188 |
| H | ? | pixi.lock | 64189 |
| H | ? | pixi.lock | 64190 |
| H | ? | pixi.lock | 64191 |
| H | ? | pixi.lock | 64192 |
| H | ? | pixi.lock | 64193 |
| H | ? | pixi.lock | 64194 |
| H | ? | pixi.lock | 64195 |
| H | ? | pixi.lock | 64196 |
| H | ? | pixi.lock | 64204 |
| H | ? | pixi.lock | 64214 |
| H | ? | pixi.lock | 64215 |
| H | ? | pixi.lock | 64216 |
| H | ? | pixi.lock | 64217 |
| H | ? | pixi.lock | 64218 |
| H | ? | pixi.lock | 64219 |
| H | ? | pixi.lock | 64220 |
| H | ? | pixi.lock | 64221 |
| H | ? | pixi.lock | 64222 |
| H | ? | pixi.lock | 64228 |
| H | ? | pixi.lock | 64235 |
| H | ? | pixi.lock | 64236 |
| H | ? | pixi.lock | 64237 |
| H | ? | pixi.lock | 64238 |
| H | ? | pixi.lock | 64257 |
| H | ? | pixi.lock | 64258 |
| H | ? | pixi.lock | 64260 |
| H | ? | pixi.lock | 64280 |
| H | ? | pixi.lock | 64287 |
| H | ? | pixi.lock | 64296 |
| H | ? | pixi.lock | 64303 |
| H | ? | pixi.lock | 64304 |
| H | ? | pixi.lock | 64313 |
| H | ? | pixi.lock | 64320 |
| H | ? | pixi.lock | 64329 |
| H | ? | pixi.lock | 64336 |
| H | ? | pixi.lock | 64337 |
| H | ? | pixi.lock | 64338 |
| H | ? | pixi.lock | 64347 |
| H | ? | pixi.lock | 64912 |
| H | ? | pixi.lock | 66080 |
| H | ? | pixi.lock | 66087 |
| H | ? | pixi.lock | 66088 |
| H | ? | pixi.lock | 66089 |
| H | ? | pixi.lock | 66090 |
| H | ? | pixi.lock | 66091 |
| H | ? | pixi.lock | 66092 |
| H | ? | pixi.lock | 66246 |
| H | ? | pixi.lock | 66405 |
| H | ? | pixi.lock | 66417 |
| H | ? | pixi.lock | 66419 |
| H | ? | pixi.lock | 66424 |
| H | ? | pixi.lock | 66448 |
| H | ? | pixi.lock | 66450 |
| H | ? | pixi.lock | 66451 |
| H | ? | pixi.lock | 66452 |
| H | ? | pixi.lock | 66453 |
| H | ? | pixi.lock | 66463 |
| H | ? | pixi.lock | 66466 |
| H | ? | pixi.lock | 66487 |
| H | ? | pixi.lock | 66489 |
| H | ? | pixi.lock | 66490 |
| H | ? | pixi.lock | 66491 |
| H | ? | pixi.lock | 66492 |
| H | ? | pixi.lock | 66502 |
| H | ? | pixi.lock | 66505 |
| H | ? | pixi.lock | 66526 |
| H | ? | pixi.lock | 66528 |
| H | ? | pixi.lock | 66529 |
| H | ? | pixi.lock | 66530 |
| H | ? | pixi.lock | 66531 |
| H | ? | pixi.lock | 66541 |
| H | ? | pixi.lock | 66544 |
| H | ? | pixi.lock | 66565 |
| H | ? | pixi.lock | 66567 |
| H | ? | pixi.lock | 66568 |
| H | ? | pixi.lock | 66569 |
| H | ? | pixi.lock | 66570 |
| H | ? | pixi.lock | 66580 |
| H | ? | pixi.lock | 66583 |
| H | ? | pixi.lock | 66821 |
| H | ? | pixi.lock | 66841 |
| H | ? | pixi.lock | 66861 |
| H | ? | pixi.lock | 66881 |
| H | ? | pixi.lock | 67155 |
| H | ? | pixi.lock | 67309 |
| H | ? | pixi.lock | 67331 |
| H | ? | pixi.lock | 67391 |
| H | ? | pixi.lock | 67415 |
| H | ? | pixi.lock | 67440 |
| H | ? | pixi.lock | 67472 |
| H | ? | pixi.lock | 67513 |
| H | ? | pixi.lock | 67526 |
| H | ? | pixi.lock | 67622 |
| H | ? | pixi.lock | 67651 |
| H | ? | pixi.lock | 67668 |
| H | ? | pixi.lock | 67685 |
| H | ? | pixi.lock | 67702 |
| H | ? | pixi.lock | 67776 |
| H | ? | pixi.lock | 67794 |
| H | ? | pixi.lock | 67864 |
| H | ? | pixi.lock | 67915 |
| H | ? | pixi.lock | 67925 |
| H | ? | pixi.lock | 67932 |
| H | ? | pixi.lock | 67943 |
| H | ? | pixi.lock | 68560 |
| H | ? | pixi.lock | 68574 |
| H | ? | pixi.lock | 68590 |
| H | ? | pixi.lock | 68604 |
| H | ? | pixi.lock | 68618 |
| H | ? | pixi.lock | 69473 |
| H | ? | pixi.lock | 69486 |
| H | ? | pixi.lock | 69501 |
| H | ? | pixi.lock | 69509 |
| H | ? | pixi.lock | 70065 |
| H | ? | pixi.lock | 71265 |
| H | ? | pixi.lock | 71696 |
| H | ? | pixi.lock | 71791 |
| H | ? | pixi.lock | 72327 |
| H | ? | pixi.lock | 72775 |
| H | ? | pixi.lock | 72782 |
| H | ? | pixi.lock | 72851 |
| H | ? | pixi.lock | 72871 |
| H | ? | pixi.lock | 72893 |
| H | ? | pixi.lock | 72913 |
| C | ? | hashing.py | 45 |
| M | ? | run_stubtest.py | 98 |
| M | ? | validate_min_versions_in_sync.py | 33 |
| M | ? | validate_min_versions_in_sync.py | 231 |
| H | ? | eval_performance.py | 20 |
| H | ? | eval_performance.py | 107 |
| H | ? | eval.py | 179 |
| H | ? | ops.py | 430 |
| H | ? | frame.py | 5232 |
| H | ? | frame.py | 5243 |
| H | ? | frame.py | 5260 |
| H | ? | frame.py | 5276 |
| H | ? | frame.py | 5288 |
| H | ? | eval.py | 25 |
| H | ? | eval.py | 28 |
| H | ? | eval.py | 34 |
| H | ? | eval.py | 37 |
| C | ? | pickle.py | 240 |
| H | ? | environment.yml | 0 |
| H | ? | pyright_reportGeneralTypeIssues.json | 0 |
| H | ? | codecov.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| C | GS005 | sql.py | 2460 |
| M | ? | package.py | 15 |

---
*Сгенерировано GSC v0.6 · 2026-06-28T04:01:29.505479*