---
title: "GSC Audit: /tmp/gsc-learn/pandas"
date: 2026-07-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pandas

**Дата:** 29.07.2026 04:03  
**Путь:** `/tmp/gsc-learn/pandas`  
**Всего находок:** 2256  
**CRITICAL:** 16 | **HIGH:** 1280 | **MEDIUM:** 452 | **LOW:** 503

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Хардкод IP адреса | 1199 |
| Python: assert in production | 418 |
| CVE-2026-56233: Path traversal | 56 |
| Bare except: | 21 |
| GS003 | 18 |
| eval() or exec() usage | 13 |
| GS008 | 12 |
| Generic code smell #24 | 8 |
| Generic code smell #27 | 8 |
| Generic code smell #30 | 8 |
| Generic code smell #33 | 8 |
| Generic code smell #36 | 8 |
| Generic code smell #39 | 8 |
| Generic code smell #42 | 8 |
| Generic code smell #45 | 8 |
| Generic code smell #48 | 8 |
| Generic code smell #51 | 8 |
| Generic code smell #54 | 8 |
| Generic code smell #57 | 8 |
| Generic code smell #60 | 8 |
| Generic code smell #63 | 8 |
| Generic code smell #66 | 8 |
| Generic code smell #69 | 8 |
| Generic code smell #72 | 8 |
| Generic code smell #75 | 8 |
| Generic code smell #78 | 8 |
| Generic code smell #81 | 8 |
| Generic code smell #84 | 8 |
| Generic code smell #87 | 8 |
| Generic code smell #90 | 8 |
| Generic code smell #93 | 8 |
| Generic code smell #96 | 8 |
| Generic code smell #99 | 8 |
| Generic code smell #102 | 8 |
| Generic code smell #105 | 8 |
| Generic code smell #108 | 8 |
| Generic code smell #111 | 8 |
| Generic code smell #114 | 8 |
| Generic code smell #117 | 8 |
| Generic code smell #120 | 8 |
| Generic code smell #123 | 8 |
| Generic code smell #126 | 8 |
| Generic code smell #129 | 8 |
| Generic code smell #132 | 8 |
| Generic code smell #135 | 8 |
| Generic code smell #138 | 8 |
| Generic code smell #141 | 8 |
| Generic code smell #144 | 8 |
| Generic code smell #147 | 8 |
| Generic code smell #150 | 8 |
| Generic code smell #153 | 8 |
| Generic code smell #156 | 8 |
| Generic code smell #159 | 8 |
| Generic code smell #162 | 8 |
| Generic code smell #165 | 8 |
| Generic code smell #168 | 8 |
| Generic code smell #171 | 8 |
| Generic code smell #174 | 8 |
| Generic code smell #177 | 8 |
| Generic code smell #180 | 8 |
| Generic code smell #183 | 8 |
| Generic code smell #186 | 8 |
| Generic code smell #189 | 8 |
| Generic code smell #192 | 8 |
| Generic code smell #195 | 8 |
| Generic code smell #198 | 8 |
| SQL injection risk: f-string in query | 7 |
| CVE-2026-55721: SQL injection | 6 |
| CVE-2026-37270: Hardcoded credential | 6 |
| Python: File upload without content-type validation | 4 |
| Outdated dependency pattern | 3 |
| GS007 | 3 |
| CVE-2026-55223: Insecure deserialization | 2 |
| CVE-2026-56219: Authentication bypass | 2 |
| GS014 | 2 |
| CVE-2026-54696: Buffer overflow | 1 |
| GS015 | 1 |
| Hardcoded encryption key | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: environment.yml (664) | 1 |
| World-readable file: pyright_reportGeneralTypeIssues.json (664) | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| GS005 | 1 |
| GS009 | 1 |
| GS012 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | sql.py | 26 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 75 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2269 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2271 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2483 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2633 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 2791 | OWASP A03: Injection |
| CRITICAL | ? | sql.py | 26 |  |
| CRITICAL | ? | sql.py | 75 |  |
| CRITICAL | ? | sql.py | 2269 |  |
| CRITICAL | ? | sql.py | 2271 |  |
| CRITICAL | ? | sql.py | 2483 |  |
| CRITICAL | ? | sql.py | 2633 |  |
| CRITICAL | ? | hashing.py | 45 | Match: _default_hash_key = "0123456789123456" |
| CRITICAL | ? | pickle.py | 240 | Match:                 return pickle.load(handles.handle) |
| CRITICAL | GS005 | sql.py | 2483 | Line 2483: self.execute(f"DELETE FROM {quoted_table_name}"). |
| HIGH | ? | excel.py | 83 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _odswriter.py | 91 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _openpyxl.py | 109 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | format.py | 1028 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | algorithms.py | 986 |  |
| HIGH | ? | merge.py | 3110 |  |
| HIGH | ? | style_render.py | 1202 |  |
| HIGH | ? | style.py | 211 |  |
| HIGH | ? | style.py | 331 |  |
| HIGH | ? | style.py | 350 |  |
| HIGH | ? | style.py | 885 |  |
| HIGH | ? | style.py | 942 |  |
| HIGH | ? | style.py | 1003 |  |
| HIGH | ? | style.py | 1132 |  |
| HIGH | ? | style.py | 1192 |  |
| HIGH | ? | style.py | 1939 |  |
| HIGH | ? | style.py | 2092 |  |
| HIGH | ? | style.py | 2176 |  |
| HIGH | ? | style.py | 2188 |  |
| HIGH | ? | style.py | 2252 |  |
| HIGH | ? | style.py | 2264 |  |
| HIGH | ? | style.py | 2340 |  |
| HIGH | ? | style.py | 2550 |  |
| HIGH | ? | style.py | 2589 |  |
| HIGH | ? | style.py | 2657 |  |
| HIGH | ? | style.py | 2863 |  |
| HIGH | ? | style.py | 3218 |  |
| HIGH | ? | style.py | 3224 |  |
| HIGH | ? | style.py | 3232 |  |
| HIGH | ? | style.py | 3240 |  |
| HIGH | ? | style.py | 3247 |  |
| HIGH | ? | style.py | 3260 |  |
| HIGH | ? | style.py | 3371 |  |
| HIGH | ? | style.py | 3377 |  |
| HIGH | ? | style.py | 3383 |  |
| HIGH | ? | style.py | 3389 |  |
| HIGH | ? | style.py | 3396 |  |
| HIGH | ? | style.py | 3409 |  |
| HIGH | ? | style.py | 3467 |  |
| HIGH | ? | style.py | 3559 |  |
| HIGH | ? | style.py | 3646 |  |
| HIGH | ? | style.py | 3703 |  |
| HIGH | ? | style.py | 3762 |  |
| HIGH | ? | style.py | 3850 |  |
| HIGH | ? | style.py | 3859 |  |
| HIGH | ? | style.py | 3871 |  |
| HIGH | ? | style.py | 3879 |  |
| HIGH | ? | style.py | 3959 |  |
| HIGH | ? | style.py | 3966 |  |
| HIGH | ? | style.py | 3977 |  |
| HIGH | ? | style.py | 4053 |  |
| HIGH | ? | style.py | 4156 |  |
| HIGH | ? | style.py | 4167 |  |
| HIGH | ? | style.py | 4191 |  |
| HIGH | ? | style.py | 4207 |  |
| HIGH | ? | pandas_web.py | 457 |  |
| HIGH | ? | pandas_web.py | 488 |  |
| HIGH | ? | conf.py | 117 |  |
| HIGH | ? | conf.py | 121 |  |
| HIGH | ? | conf.py | 449 |  |
| HIGH | ? | conf.py | 584 |  |
| HIGH | ? | conf.py | 599 |  |
| HIGH | ? | pixi.toml | 199 | Match: scipy-stubs = ">=1.17.1.5" |
| HIGH | ? | pixi.lock | 17 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 371 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1020 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1332 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1816 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2165 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2245 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2593 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2774 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3040 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3161 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3427 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3545 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3818 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4170 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4815 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 5125 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6129 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6364 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6920 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 7282 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8555 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8910 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9561 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9873 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10374 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10447 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10506 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10891 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11601 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11943 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12274 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12659 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13369 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13711 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14042 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14425 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15133 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15474 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16036 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16122 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16196 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16578 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17285 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17625 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18175 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18257 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18329 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18655 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19017 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19029 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19030 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19031 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19032 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19050 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19411 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19423 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19424 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19425 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19426 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19559 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19571 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19572 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19573 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19574 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19780 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19912 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19924 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19925 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19926 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19927 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20133 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20263 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20274 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20275 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20276 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20277 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20628 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 20639 | Match:     - alsa-lib >=1.2.16.1,<1.3.0a0 |
| HIGH | ? | pixi.lock | 20686 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20687 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20688 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20689 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 20690 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20696 | Match:     - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 20704 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20705 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20706 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20707 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20708 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 20714 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 20722 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20729 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20737 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20745 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20759 | Match:     - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20771 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20778 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20784 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 20793 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20799 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 20807 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20808 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20809 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 20816 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 20826 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 20827 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20828 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20834 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20843 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 20844 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20845 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20846 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20852 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20860 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20861 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20862 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 20863 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20869 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20877 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20878 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20880 | Match:   - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 20885 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20894 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20895 | Match:   - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 20896 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20902 | Match:     - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20910 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20911 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20912 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20918 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 20927 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20928 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20929 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20935 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 20944 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 20945 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20947 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20948 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 20949 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 20950 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 20956 | Match:     - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 20964 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 20965 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20966 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20967 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20968 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20969 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 20976 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 20983 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20989 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 20998 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 21004 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 21011 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21017 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 21026 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 21032 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 21040 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 21041 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 21042 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21043 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 21044 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 21045 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 21046 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 21047 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 21048 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 21055 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 21065 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 21066 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 21067 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 21068 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 21069 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 21070 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 21071 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 21072 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 21073 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 21079 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 21087 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21088 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 21089 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 21090 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 21111 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 21112 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 21114 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 21137 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21145 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21154 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 21162 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21163 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 21171 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 21179 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21190 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 21198 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21199 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 21200 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 21208 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 21267 | Match:   - binutils_impl_linux-64 >=2.46.1,<2.46.2.0a0 |
| HIGH | ? | pixi.lock | 21913 | Match:   - gcc_impl_linux-64 >=14.3.0,<14.3.1.0a0 |
| HIGH | ? | pixi.lock | 23144 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 23321 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 23329 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 23330 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 23331 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 23332 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 23333 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 23334 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 23574 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 23751 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 23764 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 23767 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 23772 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 23795 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23797 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23798 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23799 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23800 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23811 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23815 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23835 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23837 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23838 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23839 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23840 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23851 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23855 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23875 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23877 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23878 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23879 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23880 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23891 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23895 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23915 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23917 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23918 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23919 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23920 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23931 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 23935 | Match:   - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 24185 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24206 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24227 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24248 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 24263 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 24671 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 24921 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 24944 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24967 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25049 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 25073 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25097 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25121 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25418 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 25447 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25470 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25522 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25540 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25558 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25576 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25661 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 25678 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25696 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25846 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 25921 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 25930 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 25938 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 25948 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25959 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 26532 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 26546 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 26562 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 26576 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 26590 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 27509 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 27520 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 27535 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 27542 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 27557 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 27565 | Match:     - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 27943 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 27965 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 27991 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 28013 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 28102 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 29419 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 29886 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 29900 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 29962 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 30047 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 30297 | Match:     - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 30312 | Match:     - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 31388 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 31460 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31476 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31494 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31510 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31681 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 31691 | Match:     - alsa-lib >=1.2.16.1,<1.3.0a0 |
| HIGH | ? | pixi.lock | 31736 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31737 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 31738 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31739 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31740 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31746 | Match:     - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 31753 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31754 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31755 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31756 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31757 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 31763 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 31770 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31777 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31784 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31792 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31805 | Match:     - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31817 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31824 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31830 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 31838 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31844 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 31851 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31852 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31853 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 31860 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 31869 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31870 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31871 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 31877 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31885 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31886 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31887 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31888 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 31894 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31901 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31902 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31903 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 31904 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31910 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31917 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31918 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31920 | Match:   - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 31925 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31933 | Match:   - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 31934 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31935 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31941 | Match:     - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31948 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31949 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31950 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31956 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 31964 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31965 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31966 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31972 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 31980 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31981 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 31983 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 31984 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 31985 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 31986 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31992 | Match:     - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 31999 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 32000 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32001 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32002 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 32003 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 32004 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 32011 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 32018 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32024 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 32032 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 32038 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 32045 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32051 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 32059 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 32065 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 32072 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 32073 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32074 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32075 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 32076 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 32077 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 32078 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 32079 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 32080 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 32087 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 32096 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 32097 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 32098 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 32099 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 32100 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32101 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 32102 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 32103 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 32104 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 32110 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 32117 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32118 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 32119 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 32120 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 32139 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 32140 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32142 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 32165 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32172 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32181 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 32188 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32189 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 32197 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 32204 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32215 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 32222 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32223 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 32224 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 32232 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 32288 | Match:   - binutils_impl_linux-aarch64 >=2.46.1,<2.46.2.0a0 |
| HIGH | ? | pixi.lock | 32819 | Match:   - gcc_impl_linux-aarch64 >=14.3.0,<14.3.1.0a0 |
| HIGH | ? | pixi.lock | 34020 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 34194 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 34201 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 34202 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 34203 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 34204 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 34205 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 34206 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 34437 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 34613 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 34626 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 34629 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 34634 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 34656 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34658 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34659 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34660 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34661 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34672 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34676 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34695 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34697 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34698 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34699 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34700 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34711 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34715 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34734 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34736 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34737 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34738 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34739 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34750 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34754 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34773 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34775 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34776 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34777 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34778 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34789 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 34793 | Match:   - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 35030 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35050 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35070 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35090 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 35105 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 35476 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 35717 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 35739 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35761 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 35840 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 35863 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35886 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35909 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 36188 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 36216 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 36239 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 36289 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36306 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36323 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36340 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36420 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 36436 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 36453 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 36583 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 36675 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 36684 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 36691 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 36701 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36711 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 37240 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 37254 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 37269 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 37283 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 37297 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 38190 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 38201 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 38212 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 38222 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 38232 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 38244 | Match:     - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 38616 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38642 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38666 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38685 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38775 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 40027 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 40487 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 40501 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 40562 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 40636 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 40892 | Match:     - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 40906 | Match:     - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 41918 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 41987 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42003 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42021 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42037 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42078 | Match:   - libadbc-driver-postgresql >=1.11.0,<1.11.1.0a0 |
| HIGH | ? | pixi.lock | 42095 | Match:   - libadbc-driver-postgresql >=1.2.0,<1.2.1.0a0 |
| HIGH | ? | pixi.lock | 42110 | Match:   - libadbc-driver-postgresql >=1.8.0,<1.8.1.0a0 |
| HIGH | ? | pixi.lock | 42125 | Match:   - libadbc-driver-sqlite >=1.11.0,<1.11.1.0a0 |
| HIGH | ? | pixi.lock | 42142 | Match:   - libadbc-driver-sqlite >=1.2.0,<1.2.1.0a0 |
| HIGH | ? | pixi.lock | 42157 | Match:   - libadbc-driver-sqlite >=1.3.0,<1.3.1.0a0 |
| HIGH | ? | pixi.lock | 42815 | Match:   - dask-core >=2026.7.1,<2026.7.2.0a0 |
| HIGH | ? | pixi.lock | 42816 | Match:   - distributed >=2026.7.1,<2026.7.2.0a0 |
| HIGH | ? | pixi.lock | 42894 | Match:   - dask-core >=2026.7.1,<2026.7.2.0a0 |
| HIGH | ? | pixi.lock | 43201 | Match:   - typing_extensions >=3.10.0.2 |
| HIGH | ? | pixi.lock | 43658 | Match:   - importlib-resources >=7.1.0,<7.1.1.0a0 |
| HIGH | ? | pixi.lock | 44818 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 45750 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46217 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46227 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46237 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46247 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46796 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 46797 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 46798 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 46799 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 46800 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 46806 | Match:     - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 46814 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46815 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46816 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 46817 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 46818 | Match:   - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 46823 | Match:     - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46831 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46837 | Match:     - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46845 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 46851 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 46863 | Match:     - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46876 | Match:     - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 46884 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46889 | Match:     - aws-c-compression >=0.3.0,<0.3.1.0a0 |
| HIGH | ? | pixi.lock | 46897 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 46903 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 46911 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46912 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 46913 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 46919 | Match:     - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 46928 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 46929 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 46930 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 46936 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 46944 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 46945 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 46946 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 46947 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 46953 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 46961 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46962 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46963 | Match:   - aws-c-compression >=0.3.0,<0.3.1.0a0 |
| HIGH | ? | pixi.lock | 46964 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 46969 | Match:     - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 46977 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46978 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46983 | Match:     - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 46991 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 46992 | Match:   - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 46993 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 46999 | Match:     - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 47007 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47008 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 47009 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47014 | Match:     - aws-c-mqtt >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47022 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47023 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 47024 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 47030 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 47038 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47039 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 47040 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 47041 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 47042 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 47043 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 47049 | Match:     - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 47057 | Match:   - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47058 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47059 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47060 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 47061 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47062 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47067 | Match:     - aws-c-s3 >=0.7.9,<0.7.10.0a0 |
| HIGH | ? | pixi.lock | 47075 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47080 | Match:     - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47088 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 47094 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 47102 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 47108 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 47116 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47121 | Match:     - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47129 | Match:   - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47130 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47131 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47132 | Match:   - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 47133 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 47134 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47135 | Match:   - aws-c-mqtt >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47136 | Match:   - aws-c-s3 >=0.7.9,<0.7.10.0a0 |
| HIGH | ? | pixi.lock | 47137 | Match:   - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47143 | Match:     - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 47152 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 47153 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 47154 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 47155 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 47156 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47157 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 47158 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 47159 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 47160 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 47166 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 47174 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47175 | Match:   - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 47176 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47177 | Match:   - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 47195 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 47196 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 47197 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 47221 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47229 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47237 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 47245 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47246 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 47253 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 47261 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47271 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 47279 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47280 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 47281 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 47288 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 49065 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 49073 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 49074 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 49075 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 49076 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 49077 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 49078 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 49276 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 49328 | Match:   - tapi >=1600.0.11.8,<1601.0a0 |
| HIGH | ? | pixi.lock | 49484 | Match:   - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 49499 | Match:   - orc >=2.0.3,<2.0.4.0a0 |
| HIGH | ? | pixi.lock | 49520 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49522 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49523 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49524 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49525 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49536 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49539 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49559 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49561 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49562 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49563 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49564 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49575 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49578 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49598 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49600 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49601 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49602 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49603 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49614 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49617 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49637 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49639 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49640 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49641 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49642 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49653 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 49656 | Match:   - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 49698 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49718 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49738 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49758 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 49778 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49800 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49822 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49844 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 49887 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49909 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49931 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49953 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 49973 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 49990 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50028 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50048 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50068 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50088 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50108 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 50122 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 50388 | Match:   - libcxx-headers >=19.1.7,<19.1.8.0a0 |
| HIGH | ? | pixi.lock | 50400 | Match:   - libcxx-headers >=21.1.8,<21.1.9.0a0 |
| HIGH | ? | pixi.lock | 50455 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 50577 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50599 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50621 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 50700 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50723 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50746 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50769 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51098 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 51116 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51139 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51189 | Match:   - libthrift >=0.21.0,<0.21.1.0a0 |
| HIGH | ? | pixi.lock | 51209 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51210 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51230 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51231 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51251 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51252 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51272 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51273 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51340 | Match:     - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 51356 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51373 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51481 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 51531 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 51538 | Match:     - libthrift >=0.21.0,<0.21.1.0a0 |
| HIGH | ? | pixi.lock | 51547 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 51555 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51566 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 52071 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 52084 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 52098 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 52111 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 52124 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 52979 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 52989 | Match:     - orc >=2.0.3,<2.0.4.0a0 |
| HIGH | ? | pixi.lock | 52999 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 53010 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 53025 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 53032 | Match:     - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 53388 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 53409 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 53434 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 53451 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 54613 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 55230 | Match:     - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 55616 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-6 |
| HIGH | ? | pixi.lock | 55939 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 56008 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56023 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56040 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56055 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56265 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56266 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56267 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56268 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56269 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 56275 | Match:     - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 56283 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56284 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56285 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56286 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56287 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 56292 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 56300 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56306 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56314 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56320 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56333 | Match:     - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56345 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56353 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56358 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 56366 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56372 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 56380 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56381 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56382 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56388 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 56397 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 56398 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56399 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56405 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56413 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56414 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56415 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 56416 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56422 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56430 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56431 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56432 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 56433 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56438 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56446 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56447 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56452 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56460 | Match:   - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 56461 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56462 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56468 | Match:     - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56476 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56477 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56478 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56483 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 56491 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56492 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56493 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56499 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 56507 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56508 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56509 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56510 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 56511 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56512 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 56518 | Match:     - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 56526 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 56527 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56528 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56529 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56530 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56531 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56536 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 56544 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56549 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 56557 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56563 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 56571 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56576 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56584 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56590 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 56598 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 56599 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56600 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56601 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 56602 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56603 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56604 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 56605 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 56606 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 56612 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56621 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 56622 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 56623 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56624 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56625 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56626 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 56627 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56628 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 56629 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56635 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 56643 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56644 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 56645 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56646 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56665 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 56667 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56668 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 56690 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56698 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56706 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 56714 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56715 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 56722 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 56730 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56740 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 56748 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56749 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 56750 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 56757 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 58603 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 58611 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 58612 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 58613 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 58614 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 58615 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 58616 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 58822 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 58887 | Match:   - tapi >=1600.0.11.8,<1601.0a0 |
| HIGH | ? | pixi.lock | 59043 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 59055 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 59057 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 59062 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 59084 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59086 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59087 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59088 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59089 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59100 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59103 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59123 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59125 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59126 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59127 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59128 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59139 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59142 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59162 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59164 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59165 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59166 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59167 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59178 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59181 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59201 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59203 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59204 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59205 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59206 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59217 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59220 | Match:   - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 59247 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59267 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59287 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59307 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59327 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59349 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59371 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59393 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59419 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59441 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59463 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59485 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59506 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59526 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59546 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59566 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59580 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 59845 | Match:   - libcxx-headers >=19.1.7,<19.1.8.0a0 |
| HIGH | ? | pixi.lock | 59901 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 60023 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 60045 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60067 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60145 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 60168 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60191 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60214 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60541 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 60559 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60581 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60635 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60636 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60656 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60657 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60677 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60678 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60698 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60699 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60766 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 60782 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60799 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60906 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 60941 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 60948 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 60957 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 60965 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60976 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 61522 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 61535 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 61550 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 61563 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 61576 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 62452 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 62462 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 62475 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 62483 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 62493 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 62505 | Match:     - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 62863 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 62885 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 62916 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 62934 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 63023 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 64084 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 64718 | Match:     - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 65097 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-a |
| HIGH | ? | pixi.lock | 65436 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 65506 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 65522 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 65540 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 65556 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 65777 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 65778 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 65779 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 65780 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 65781 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 65787 | Match:     - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 65794 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 65795 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 65796 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 65797 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 65798 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 65806 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 65813 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 65822 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 65829 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 65838 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 65853 | Match:     - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 65867 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 65874 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 65882 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 65892 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 65898 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 65905 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 65906 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 65907 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 65915 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 65925 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 65926 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 65927 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 65933 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 65943 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 65944 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 65945 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 65946 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 65952 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 65959 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 65960 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 65961 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 65962 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 65970 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 65977 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 65978 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 65986 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 65996 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 65997 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 66003 | Match:     - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66010 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66011 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66012 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66020 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 66030 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 66031 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66032 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66038 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 66048 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66049 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 66050 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 66051 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66052 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 66053 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66059 | Match:     - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 66066 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 66067 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66068 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66069 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66070 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66071 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 66079 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 66086 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66094 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 66104 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 66110 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 66117 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66125 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 66135 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 66141 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 66148 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 66149 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66150 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66151 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 66152 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66153 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66154 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 66155 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 66156 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 66164 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66174 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 66175 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66176 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66177 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66178 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 66179 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66180 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 66181 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 66182 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 66188 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66195 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66196 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 66197 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 66198 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66217 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 66219 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66220 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66241 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66248 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66257 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 66264 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66265 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 66274 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66281 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66290 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 66297 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66298 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66299 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 66308 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 66851 | Match:   - gcc_impl_win-64 >=15.2.0,<15.2.1.0a0 |
| HIGH | ? | pixi.lock | 67945 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 67952 | Match:   - aws-c-auth >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 67953 | Match:   - aws-c-common >=0.14.2,<0.14.3.0a0 |
| HIGH | ? | pixi.lock | 67954 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 67955 | Match:   - aws-c-io >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 67956 | Match:   - aws-c-s3 >=0.12.8,<0.12.9.0a0 |
| HIGH | ? | pixi.lock | 67957 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 68146 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 68323 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 68335 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 68337 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 68342 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 68366 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68368 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68369 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68370 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68371 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68381 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68384 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 68406 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68408 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68409 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68410 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68411 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68421 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68424 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 68446 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68448 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68449 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68450 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68451 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68461 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68464 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 68486 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68488 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68489 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68490 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68491 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68501 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 68504 | Match:   - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 68755 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68776 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68797 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68818 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 69112 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 69232 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 69254 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69276 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 69355 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 69379 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69403 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69427 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 69509 | Match:     - libhwloc >=2.13.0,<2.13.1.0a0 |
| HIGH | ? | pixi.lock | 69674 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 69697 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69733 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 69751 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 69769 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 69787 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 69862 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 69879 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69897 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 70001 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 70052 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 70062 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 70069 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 70080 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 70089 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 70678 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 70692 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 70708 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 70722 | Match:   - matplotlib-base >=3.11.1,<3.11.2.0a0 |
| HIGH | ? | pixi.lock | 70736 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 71595 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 71608 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 71623 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 71630 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 71645 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 71653 | Match:     - orc >=2.3.1,<2.3.2.0a0 |
| HIGH | ? | pixi.lock | 72024 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72049 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72078 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72100 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72190 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 73424 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 73869 | Match:   - zeromq >=4.3.5,<4.3.6.0a0 |
| HIGH | ? | pixi.lock | 73964 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 74497 | Match:   - libhwloc >=2.13.0,<2.13.1.0a0 |
| HIGH | ? | pixi.lock | 74948 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 74955 | Match:     - zeromq >=4.3.5,<4.3.6.0a0 |
| HIGH | ? | pixi.lock | 75024 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 75044 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 75066 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 75086 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | eval.py | 25 | Match:         pd.eval("self.df + self.df2 + self.df3 + self |
| HIGH | ? | eval.py | 28 | Match:         pd.eval( |
| HIGH | ? | eval.py | 34 | Match:         pd.eval("self.df < self.df2 < self.df3 < self |
| HIGH | ? | eval.py | 37 | Match:         pd.eval("self.df * self.df2 * self.df3 * self |
| HIGH | ? | frame.py | 5280 | Match:         >>> df.eval("A + B") |
| HIGH | ? | frame.py | 5291 | Match:         >>> df.eval("D = A + B") |
| HIGH | ? | frame.py | 5308 | Match:         >>> df.eval( |
| HIGH | ? | frame.py | 5324 | Match:         >>> df.eval("B * `C&C`") |
| HIGH | ? | frame.py | 5336 | Match:         >>> df.eval("@local_var * A") |
| HIGH | ? | ops.py | 430 | Match:                 res = eval(self, local_dict=env, engi |
| HIGH | ? | eval.py | 179 | Match: def eval( |
| HIGH | ? | eval_performance.py | 20 | Match:                 f"df.eval(s, engine={engine!r})", |
| HIGH | ? | eval_performance.py | 107 | Match:     plot_perf(ev, engines, "DataFrame.eval()", filena |
| HIGH | ? | environment.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | pyright_reportGeneralTypeIssues.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS014 | sql.py | 369 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | sql.py | 683 | Database URL contains password in plaintext. Use environment |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | sql.py | 26 |
| C | ? | sql.py | 75 |
| C | ? | sql.py | 2269 |
| C | ? | sql.py | 2271 |
| C | ? | sql.py | 2483 |
| C | ? | sql.py | 2633 |
| C | ? | sql.py | 2791 |
| M | ? | np_datetime.pyx | 282 |
| M | ? | np_datetime.pyx | 318 |
| M | ? | parsing.pyx | 1097 |
| M | ? | timedeltas.pyx | 330 |
| M | ? | strptime.pyx | 274 |
| M | ? | np_datetime.pxd | 68 |
| M | ? | util.pxd | 41 |
| M | ? | util.pxd | 48 |
| M | ? | util.pxd | 118 |
| M | ? | util.pxd | 122 |
| M | ? | period.pyx | 1107 |
| M | ? | tzconversion.pyx | 476 |
| M | ? | parsers.pyx | 376 |
| M | ? | parsers.pyx | 2773 |
| M | ? | groupby.pyx | 1621 |
| M | ? | sas.pyx | 357 |
| M | ? | sas.pyx | 366 |
| M | ? | sas.pyx | 375 |
| M | ? | sas.pyx | 384 |
| M | ? | hashtable_class_helper.pxi.in | 235 |
| M | ? | hashtable_class_helper.pxi.in | 309 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 940 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1613 |
| L | ? | datetimes.py | 1249 |
| L | ? | groupby.py | 1592 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| M | ? | indexing.py | 162 |
| M | ? | indexing.py | 167 |
| M | ? | indexing_engines.py | 89 |
| M | ? | indexing_engines.py | 147 |
| M | ? | gil.py | 60 |
| M | ? | gil.py | 63 |
| M | ? | index_cached_properties.py | 50 |
| M | ? | orc.py | 242 |
| M | ? | orc.py | 256 |
| M | ? | common.py | 135 |
| M | ? | common.py | 421 |
| M | ? | common.py | 881 |
| M | ? | common.py | 887 |
| M | ? | common.py | 928 |
| M | ? | common.py | 987 |
| M | ? | common.py | 1171 |
| M | ? | common.py | 1337 |
| M | ? | pytables.py | 673 |
| M | ? | pytables.py | 773 |
| M | ? | pytables.py | 1935 |
| M | ? | pytables.py | 1936 |
| M | ? | pytables.py | 1995 |
| M | ? | pytables.py | 1996 |
| M | ? | pytables.py | 2020 |
| M | ? | pytables.py | 2021 |
| M | ? | pytables.py | 2027 |
| M | ? | pytables.py | 2265 |
| M | ? | pytables.py | 2419 |
| M | ? | pytables.py | 2423 |
| M | ? | pytables.py | 2456 |
| M | ? | pytables.py | 2668 |
| M | ? | pytables.py | 2669 |
| M | ? | pytables.py | 2731 |
| M | ? | pytables.py | 3008 |
| M | ? | pytables.py | 3093 |
| M | ? | pytables.py | 3094 |
| M | ? | pytables.py | 3215 |
| M | ? | pytables.py | 3225 |
| M | ? | pytables.py | 3236 |
| M | ? | pytables.py | 3244 |
| M | ? | pytables.py | 3338 |
| M | ? | pytables.py | 3403 |
| M | ? | pytables.py | 3404 |
| M | ? | pytables.py | 3405 |
| M | ? | pytables.py | 3601 |
| M | ? | pytables.py | 4320 |
| M | ? | pytables.py | 4531 |
| M | ? | pytables.py | 4819 |
| M | ? | pytables.py | 4903 |
| M | ? | pytables.py | 4906 |
| M | ? | pytables.py | 4973 |
| M | ? | pytables.py | 5126 |
| M | ? | pytables.py | 5139 |
| M | ? | pytables.py | 5428 |
| M | ? | pytables.py | 5602 |
| M | ? | pytables.py | 5662 |
| M | ? | pytables.py | 5715 |
| M | ? | pytables.py | 5742 |
| M | ? | pytables.py | 5793 |
| M | ? | pytables.py | 5835 |
| M | ? | pytables.py | 5903 |
| M | ? | pytables.py | 5996 |
| M | ? | pytables.py | 6118 |
| M | ? | pytables.py | 6119 |
| M | ? | pytables.py | 6314 |
| M | ? | python_parser.py | 140 |
| M | ? | python_parser.py | 962 |
| M | ? | python_parser.py | 1222 |
| M | ? | python_parser.py | 1327 |
| M | ? | python_parser.py | 1332 |
| M | ? | base_parser.py | 314 |
| M | ? | base_parser.py | 355 |
| M | ? | readers.py | 365 |
| M | ? | readers.py | 747 |
| M | ? | readers.py | 818 |
| M | ? | c_parser_wrapper.py | 133 |
| M | ? | c_parser_wrapper.py | 171 |
| M | ? | c_parser_wrapper.py | 190 |
| M | ? | c_parser_wrapper.py | 265 |
| M | ? | c_parser_wrapper.py | 349 |
| M | ? | html.py | 998 |
| M | ? | sql.py | 375 |
| M | ? | sql.py | 517 |
| M | ? | sql.py | 722 |
| M | ? | sql.py | 1096 |
| M | ? | sql.py | 1332 |
| M | ? | parquet.py | 537 |
| M | ? | _util.py | 81 |
| M | ? | _util.py | 293 |
| M | ? | _util.py | 296 |
| M | ? | _odswriter.py | 117 |
| M | ? | _base.py | 849 |
| M | ? | _base.py | 860 |
| M | ? | _base.py | 867 |
| M | ? | _base.py | 890 |
| M | ? | _base.py | 895 |
| M | ? | _base.py | 922 |
| M | ? | _base.py | 1226 |
| M | ? | _base.py | 1508 |
| M | ? | _base.py | 1695 |
| M | ? | excel.py | 361 |
| M | ? | css.py | 349 |
| M | ? | string.py | 133 |
| M | ? | xml.py | 550 |
| M | ? | html.py | 491 |
| M | ? | format.py | 672 |
| M | ? | format.py | 697 |
| M | ? | format.py | 1031 |
| M | ? | format.py | 1316 |
| M | ? | csvs.py | 222 |
| M | ? | csvs.py | 238 |
| M | ? | stata.py | 1483 |
| M | ? | stata.py | 1527 |
| M | ? | stata.py | 1695 |
| M | ? | stata.py | 2540 |
| M | ? | stata.py | 2955 |
| M | ? | stata.py | 3519 |
| M | ? | sas7bdat.py | 490 |
| M | ? | sas7bdat.py | 505 |
| M | ? | sas7bdat.py | 525 |
| M | ? | _exceptions.py | 55 |
| M | ? | _exceptions.py | 56 |
| M | ? | _print_versions.py | 141 |
| M | ? | _print_versions.py | 146 |
| M | ? | config.py | 405 |
| M | ? | config.py | 762 |
| M | ? | _optional.py | 148 |
| M | ? | asserters.py | 899 |
| M | ? | asserters.py | 900 |
| M | ? | asserters.py | 948 |
| M | ? | asserters.py | 956 |
| M | ? | asserters.py | 1131 |
| M | ? | asserters.py | 1438 |
| M | ? | asserters.py | 1448 |
| M | ? | asserters.py | 1488 |
| M | ? | asserters.py | 1489 |
| M | ? | asserters.py | 1566 |
| M | ? | asserters.py | 1567 |
| M | ? | asserters.py | 1569 |
| M | ? | asserters.py | 1587 |
| M | ? | asserters.py | 1588 |
| M | ? | asserters.py | 1608 |
| M | ? | asserters.py | 1626 |
| M | ? | asserters.py | 1668 |
| M | ? | asserters.py | 1670 |
| M | ? | _warnings.py | 266 |
| M | ? | construction.py | 395 |
| M | ? | indexing.py | 1018 |
| M | ? | indexing.py | 1027 |
| M | ? | indexing.py | 1028 |
| M | ? | indexing.py | 1174 |
| M | ? | indexing.py | 2650 |
| M | ? | indexing.py | 3398 |
| M | ? | rolling.py | 3561 |
| M | ? | objects.py | 190 |
| M | ? | objects.py | 615 |
| M | ? | sample.py | 109 |
| M | ? | sample.py | 158 |
| M | ? | hashing.py | 79 |
| M | ? | missing.py | 261 |
| M | ? | extension.py | 174 |
| M | ? | base.py | 667 |
| M | ? | base.py | 745 |
| M | ? | base.py | 3888 |
| M | ? | base.py | 4703 |
| M | ? | base.py | 4875 |
| M | ? | base.py | 4953 |
| M | ? | base.py | 5052 |
| M | ? | base.py | 5053 |
| M | ? | base.py | 5119 |
| M | ? | base.py | 7252 |
| M | ? | period.py | 553 |
| M | ? | datetimes.py | 99 |
| M | ? | timedeltas.py | 306 |
| M | ? | timedeltas.py | 349 |
| M | ? | range.py | 254 |
| M | ? | range.py | 1108 |
| M | ? | multi.py | 1613 |
| M | ? | multi.py | 1688 |
| M | ? | datetimelike.py | 1360 |
| M | ? | datetimelike.py | 1369 |
| M | ? | datetimelike.py | 1370 |
| M | ? | datetimelike.py | 1406 |
| M | ? | from_dataframe.py | 331 |
| M | ? | from_dataframe.py | 335 |
| M | ? | from_dataframe.py | 513 |
| M | ? | sorting.py | 505 |
| M | ? | nanops.py | 369 |
| M | ? | nanops.py | 436 |
| M | ? | nanops.py | 447 |
| M | ? | nanops.py | 1799 |
| M | ? | accessor.py | 278 |
| M | ? | apply.py | 283 |
| M | ? | apply.py | 365 |
| M | ? | apply.py | 420 |
| M | ? | apply.py | 785 |
| M | ? | apply.py | 828 |
| M | ? | apply.py | 837 |
| M | ? | apply.py | 838 |
| M | ? | apply.py | 896 |
| M | ? | apply.py | 1161 |
| M | ? | apply.py | 1252 |
| M | ? | apply.py | 1289 |
| M | ? | apply.py | 1464 |
| M | ? | apply.py | 1704 |
| M | ? | apply.py | 1828 |
| M | ? | apply.py | 1985 |
| M | ? | apply.py | 2191 |
| M | ? | apply.py | 2192 |
| M | ? | algorithms.py | 496 |
| M | ? | algorithms.py | 1243 |
| M | ? | quantile.py | 85 |
| M | ? | quantile.py | 93 |
| M | ? | quantile.py | 203 |
| M | ? | take.py | 193 |
| M | ? | take.py | 194 |
| M | ? | take.py | 195 |
| M | ? | series.py | 1251 |
| M | ? | series.py | 4695 |
| M | ? | series.py | 4749 |
| M | ? | series.py | 7326 |
| M | ? | series.py | 7327 |
| M | ? | generic.py | 533 |
| M | ? | generic.py | 5775 |
| M | ? | generic.py | 6111 |
| M | ? | generic.py | 10863 |
| M | ? | generic.py | 10894 |
| M | ? | generic.py | 11774 |
| M | ? | generic.py | 11885 |
| M | ? | arraylike.py | 521 |
| M | ? | resample.py | 243 |
| M | ? | resample.py | 526 |
| M | ? | resample.py | 528 |
| M | ? | resample.py | 2019 |
| M | ? | resample.py | 2022 |
| M | ? | resample.py | 2092 |
| M | ? | resample.py | 2141 |
| M | ? | resample.py | 3075 |
| M | ? | managers.py | 259 |
| M | ? | managers.py | 425 |
| M | ? | managers.py | 511 |
| M | ? | managers.py | 512 |
| M | ? | managers.py | 854 |
| M | ? | managers.py | 1050 |
| M | ? | managers.py | 1719 |
| M | ? | managers.py | 1762 |
| M | ? | managers.py | 1763 |
| M | ? | managers.py | 1807 |
| M | ? | managers.py | 2079 |
| M | ? | managers.py | 2080 |
| M | ? | managers.py | 2586 |
| M | ? | ops.py | 124 |
| M | ? | ops.py | 131 |
| M | ? | ops.py | 133 |
| M | ? | ops.py | 140 |
| M | ? | ops.py | 144 |
| M | ? | blocks.py | 362 |
| M | ? | blocks.py | 400 |
| M | ? | blocks.py | 424 |
| M | ? | blocks.py | 872 |
| M | ? | blocks.py | 1050 |
| M | ? | blocks.py | 1051 |
| M | ? | blocks.py | 1207 |
| M | ? | blocks.py | 1268 |
| M | ? | blocks.py | 1269 |
| M | ? | blocks.py | 1583 |
| M | ? | blocks.py | 1584 |
| M | ? | blocks.py | 2090 |
| M | ? | blocks.py | 2097 |
| M | ? | blocks.py | 2449 |
| M | ? | expressions.py | 268 |
| M | ? | pytables.py | 108 |
| M | ? | pytables.py | 665 |
| M | ? | expr.py | 136 |
| M | ? | expr.py | 170 |
| M | ? | expr.py | 258 |
| M | ? | scope.py | 236 |
| M | ? | scope.py | 326 |
| M | ? | scope.py | 328 |
| M | ? | base.py | 3088 |
| M | ? | masked.py | 1504 |
| M | ? | period.py | 262 |
| M | ? | period.py | 1204 |
| M | ? | period.py | 1211 |
| M | ? | period.py | 1301 |
| M | ? | datetimes.py | 307 |
| M | ? | datetimes.py | 308 |
| M | ? | datetimes.py | 310 |
| M | ? | datetimes.py | 311 |
| M | ? | datetimes.py | 315 |
| M | ? | datetimes.py | 794 |
| M | ? | _ranges.py | 151 |
| M | ? | _ranges.py | 216 |
| M | ? | _ranges.py | 249 |
| M | ? | _ranges.py | 262 |
| M | ? | _ranges.py | 283 |
| M | ? | _ranges.py | 292 |
| M | ? | timedeltas.py | 241 |
| M | ? | timedeltas.py | 242 |
| M | ? | timedeltas.py | 243 |
| M | ? | timedeltas.py | 244 |
| M | ? | timedeltas.py | 455 |
| M | ? | timedeltas.py | 767 |
| M | ? | timedeltas.py | 1234 |
| M | ? | timedeltas.py | 1315 |
| M | ? | timedeltas.py | 1316 |
| M | ? | string_.py | 767 |
| M | ? | string_arrow.py | 172 |
| M | ? | string_arrow.py | 237 |
| M | ? | array.py | 2109 |
| M | ? | interval.py | 1697 |
| M | ? | interval.py | 1701 |
| M | ? | interval.py | 1731 |
| M | ? | interval.py | 1735 |
| M | ? | interval.py | 1878 |
| M | ? | interval.py | 1882 |
| M | ? | interval.py | 1887 |
| M | ? | boolean.py | 390 |
| M | ? | boolean.py | 394 |
| M | ? | datetimelike.py | 1075 |
| M | ? | datetimelike.py | 1296 |
| M | ? | datetimelike.py | 1312 |
| M | ? | datetimelike.py | 1689 |
| M | ? | _mixins.py | 191 |
| M | ? | numeric.py | 212 |
| M | ? | categorical.py | 1643 |
| M | ? | categorical.py | 2009 |
| M | ? | categorical.py | 2386 |
| M | ? | categorical.py | 2612 |
| M | ? | categorical.py | 2895 |
| M | ? | array.py | 508 |
| M | ? | array.py | 2113 |
| M | ? | array.py | 2125 |
| M | ? | extension_types.py | 66 |
| M | ? | reshape.py | 433 |
| M | ? | reshape.py | 547 |
| M | ? | reshape.py | 615 |
| M | ? | reshape.py | 831 |
| M | ? | reshape.py | 1023 |
| M | ? | reshape.py | 1088 |
| M | ? | pivot.py | 490 |
| M | ? | pivot.py | 563 |
| M | ? | pivot.py | 700 |
| M | ? | merge.py | 1281 |
| M | ? | merge.py | 1396 |
| M | ? | merge.py | 1531 |
| M | ? | merge.py | 2060 |
| M | ? | merge.py | 2644 |
| M | ? | merge.py | 2906 |
| M | ? | merge.py | 2907 |
| M | ? | merge.py | 2985 |
| M | ? | merge.py | 2989 |
| M | ? | merge.py | 3026 |
| M | ? | merge.py | 3027 |
| M | ? | describe.py | 379 |
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
| M | ? | common.py | 161 |
| M | ? | common.py | 325 |
| M | ? | dtypes.py | 2447 |
| M | ? | cast.py | 1030 |
| M | ? | cast.py | 1069 |
| M | ? | cast.py | 1086 |
| M | ? | cast.py | 1556 |
| M | ? | datetimes.py | 230 |
| M | ? | datetimes.py | 236 |
| M | ? | numeric.py | 312 |
| M | ? | array_ops.py | 378 |
| M | ? | array_ops.py | 384 |
| M | ? | grouper.py | 347 |
| M | ? | grouper.py | 367 |
| M | ? | grouper.py | 508 |
| M | ? | grouper.py | 861 |
| M | ? | numba_.py | 109 |
| M | ? | numba_.py | 166 |
| M | ? | ops.py | 527 |
| M | ? | ops.py | 552 |
| M | ? | ops.py | 556 |
| M | ? | ops.py | 620 |
| M | ? | ops.py | 1014 |
| M | ? | ops.py | 1287 |
| M | ? | generic.py | 482 |
| M | ? | generic.py | 592 |
| M | ? | generic.py | 792 |
| M | ? | generic.py | 2804 |
| M | ? | generic.py | 4256 |
| M | ? | groupby.py | 839 |
| M | ? | groupby.py | 1510 |
| M | ? | groupby.py | 1520 |
| M | ? | groupby.py | 1601 |
| M | ? | groupby.py | 1763 |
| M | ? | groupby.py | 1988 |
| M | ? | groupby.py | 1989 |
| M | ? | groupby.py | 5715 |
| M | ? | groupby.py | 5763 |
| M | ? | groupby.py | 5806 |
| M | ? | frequencies.py | 470 |
| M | ? | frequencies.py | 617 |
| M | ? | boxplot.py | 60 |
| M | ? | hist.py | 281 |
| M | ? | hist.py | 378 |
| M | ? | timeseries.py | 312 |
| M | ? | core.py | 291 |
| M | ? | converter.py | 1139 |
| M | ? | groupby.py | 80 |
| M | ? | pandas_web.py | 405 |
| M | ? | check_test_naming.py | 122 |
| M | ? | validate_min_versions_in_sync.py | 115 |
| M | ? | validate_min_versions_in_sync.py | 135 |
| H | ? | excel.py | 83 |
| H | ? | _odswriter.py | 91 |
| H | ? | _openpyxl.py | 109 |
| H | ? | format.py | 1028 |
| M | ? | indexing.py | 142 |
| M | ? | pickle.py | 240 |
| M | ? | pickle_compat.py | 139 |
| C | ? | sql.py | 26 |
| C | ? | sql.py | 75 |
| C | ? | sql.py | 2269 |
| C | ? | sql.py | 2271 |
| C | ? | sql.py | 2483 |
| C | ? | sql.py | 2633 |
| H | ? | algorithms.py | 986 |
| H | ? | merge.py | 3110 |
| H | ? | style_render.py | 1202 |
| H | ? | style.py | 211 |
| H | ? | style.py | 331 |
| H | ? | style.py | 350 |
| H | ? | style.py | 885 |
| H | ? | style.py | 942 |
| H | ? | style.py | 1003 |
| H | ? | style.py | 1132 |
| H | ? | style.py | 1192 |
| H | ? | style.py | 1939 |
| H | ? | style.py | 2092 |
| H | ? | style.py | 2176 |
| H | ? | style.py | 2188 |
| H | ? | style.py | 2252 |
| H | ? | style.py | 2264 |
| H | ? | style.py | 2340 |
| H | ? | style.py | 2550 |
| H | ? | style.py | 2589 |
| H | ? | style.py | 2657 |
| H | ? | style.py | 2863 |
| H | ? | style.py | 3218 |
| H | ? | style.py | 3224 |
| H | ? | style.py | 3232 |
| H | ? | style.py | 3240 |
| H | ? | style.py | 3247 |
| H | ? | style.py | 3260 |
| H | ? | style.py | 3371 |
| H | ? | style.py | 3377 |
| H | ? | style.py | 3383 |
| H | ? | style.py | 3389 |
| H | ? | style.py | 3396 |
| H | ? | style.py | 3409 |
| H | ? | style.py | 3467 |
| H | ? | style.py | 3559 |
| H | ? | style.py | 3646 |
| H | ? | style.py | 3703 |
| H | ? | style.py | 3762 |
| H | ? | style.py | 3850 |
| H | ? | style.py | 3859 |
| H | ? | style.py | 3871 |
| H | ? | style.py | 3879 |
| H | ? | style.py | 3959 |
| H | ? | style.py | 3966 |
| H | ? | style.py | 3977 |
| H | ? | style.py | 4053 |
| H | ? | style.py | 4156 |
| H | ? | style.py | 4167 |
| H | ? | style.py | 4191 |
| H | ? | style.py | 4207 |
| H | ? | pandas_web.py | 457 |
| H | ? | pandas_web.py | 488 |
| H | ? | conf.py | 117 |
| H | ? | conf.py | 121 |
| H | ? | conf.py | 449 |
| H | ? | conf.py | 584 |
| H | ? | conf.py | 599 |
| M | ? | hdf.py | 126 |
| M | ? | hdf.py | 131 |
| M | ? | hdf.py | 140 |
| M | ? | series_methods.py | 146 |
| M | ? | pytables.py | 2018 |
| M | ? | hashing.py | 45 |
| L | GS003 | eval_performance.py | 58 |
| L | GS003 | announce.py | 167 |
| L | GS003 | generate_version.py | 66 |
| L | GS003 | config.py | 340 |
| L | GS003 | _base.py | 772 |
| L | GS003 | sas7bdat.py | 637 |
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
| L | GS003 | validate_unwanted_patterns.py | 538 |
| L | GS008 | _hypothesis.py | 47 |
| L | GS008 | _hypothesis.py | 56 |
| L | GS008 | _hypothesis.py | 62 |
| L | GS008 | _hypothesis.py | 67 |
| L | GS008 | _hypothesis.py | 71 |
| L | GS008 | _constants.py | 23 |
| L | GS008 | _constants.py | 24 |
| L | GS008 | _constants.py | 25 |
| L | GS008 | _constants.py | 26 |
| L | GS008 | col.py | 24 |
| L | GS008 | ops.py | 47 |
| L | GS008 | format.py | 117 |
| I | GS015 | aliases.py | 1 |
| H | ? | pixi.toml | 199 |
| H | ? | pixi.lock | 17 |
| H | ? | pixi.lock | 371 |
| H | ? | pixi.lock | 1020 |
| H | ? | pixi.lock | 1332 |
| H | ? | pixi.lock | 1816 |
| H | ? | pixi.lock | 2165 |
| H | ? | pixi.lock | 2245 |
| H | ? | pixi.lock | 2593 |
| H | ? | pixi.lock | 2774 |
| H | ? | pixi.lock | 3040 |
| H | ? | pixi.lock | 3161 |
| H | ? | pixi.lock | 3427 |
| H | ? | pixi.lock | 3545 |
| H | ? | pixi.lock | 3818 |
| H | ? | pixi.lock | 4170 |
| H | ? | pixi.lock | 4815 |
| H | ? | pixi.lock | 5125 |
| H | ? | pixi.lock | 6129 |
| H | ? | pixi.lock | 6364 |
| H | ? | pixi.lock | 6920 |
| H | ? | pixi.lock | 7282 |
| H | ? | pixi.lock | 8555 |
| H | ? | pixi.lock | 8910 |
| H | ? | pixi.lock | 9561 |
| H | ? | pixi.lock | 9873 |
| H | ? | pixi.lock | 10374 |
| H | ? | pixi.lock | 10447 |
| H | ? | pixi.lock | 10506 |
| H | ? | pixi.lock | 10891 |
| H | ? | pixi.lock | 11601 |
| H | ? | pixi.lock | 11943 |
| H | ? | pixi.lock | 12274 |
| H | ? | pixi.lock | 12659 |
| H | ? | pixi.lock | 13369 |
| H | ? | pixi.lock | 13711 |
| H | ? | pixi.lock | 14042 |
| H | ? | pixi.lock | 14425 |
| H | ? | pixi.lock | 15133 |
| H | ? | pixi.lock | 15474 |
| H | ? | pixi.lock | 16036 |
| H | ? | pixi.lock | 16122 |
| H | ? | pixi.lock | 16196 |
| H | ? | pixi.lock | 16578 |
| H | ? | pixi.lock | 17285 |
| H | ? | pixi.lock | 17625 |
| H | ? | pixi.lock | 18175 |
| H | ? | pixi.lock | 18257 |
| H | ? | pixi.lock | 18329 |
| H | ? | pixi.lock | 18655 |
| H | ? | pixi.lock | 19017 |
| H | ? | pixi.lock | 19029 |
| H | ? | pixi.lock | 19030 |
| H | ? | pixi.lock | 19031 |
| H | ? | pixi.lock | 19032 |
| H | ? | pixi.lock | 19050 |
| H | ? | pixi.lock | 19411 |
| H | ? | pixi.lock | 19423 |
| H | ? | pixi.lock | 19424 |
| H | ? | pixi.lock | 19425 |
| H | ? | pixi.lock | 19426 |
| H | ? | pixi.lock | 19559 |
| H | ? | pixi.lock | 19571 |
| H | ? | pixi.lock | 19572 |
| H | ? | pixi.lock | 19573 |
| H | ? | pixi.lock | 19574 |
| H | ? | pixi.lock | 19780 |
| H | ? | pixi.lock | 19912 |
| H | ? | pixi.lock | 19924 |
| H | ? | pixi.lock | 19925 |
| H | ? | pixi.lock | 19926 |
| H | ? | pixi.lock | 19927 |
| H | ? | pixi.lock | 20133 |
| H | ? | pixi.lock | 20263 |
| H | ? | pixi.lock | 20274 |
| H | ? | pixi.lock | 20275 |
| H | ? | pixi.lock | 20276 |
| H | ? | pixi.lock | 20277 |
| H | ? | pixi.lock | 20628 |
| H | ? | pixi.lock | 20639 |
| H | ? | pixi.lock | 20686 |
| H | ? | pixi.lock | 20687 |
| H | ? | pixi.lock | 20688 |
| H | ? | pixi.lock | 20689 |
| H | ? | pixi.lock | 20690 |
| H | ? | pixi.lock | 20696 |
| H | ? | pixi.lock | 20704 |
| H | ? | pixi.lock | 20705 |
| H | ? | pixi.lock | 20706 |
| H | ? | pixi.lock | 20707 |
| H | ? | pixi.lock | 20708 |
| H | ? | pixi.lock | 20714 |
| H | ? | pixi.lock | 20722 |
| H | ? | pixi.lock | 20729 |
| H | ? | pixi.lock | 20737 |
| H | ? | pixi.lock | 20745 |
| H | ? | pixi.lock | 20759 |
| H | ? | pixi.lock | 20771 |
| H | ? | pixi.lock | 20778 |
| H | ? | pixi.lock | 20784 |
| H | ? | pixi.lock | 20793 |
| H | ? | pixi.lock | 20799 |
| H | ? | pixi.lock | 20807 |
| H | ? | pixi.lock | 20808 |
| H | ? | pixi.lock | 20809 |
| H | ? | pixi.lock | 20816 |
| H | ? | pixi.lock | 20826 |
| H | ? | pixi.lock | 20827 |
| H | ? | pixi.lock | 20828 |
| H | ? | pixi.lock | 20834 |
| H | ? | pixi.lock | 20843 |
| H | ? | pixi.lock | 20844 |
| H | ? | pixi.lock | 20845 |
| H | ? | pixi.lock | 20846 |
| H | ? | pixi.lock | 20852 |
| H | ? | pixi.lock | 20860 |
| H | ? | pixi.lock | 20861 |
| H | ? | pixi.lock | 20862 |
| H | ? | pixi.lock | 20863 |
| H | ? | pixi.lock | 20869 |
| H | ? | pixi.lock | 20877 |
| H | ? | pixi.lock | 20878 |
| H | ? | pixi.lock | 20880 |
| H | ? | pixi.lock | 20885 |
| H | ? | pixi.lock | 20894 |
| H | ? | pixi.lock | 20895 |
| H | ? | pixi.lock | 20896 |
| H | ? | pixi.lock | 20902 |
| H | ? | pixi.lock | 20910 |
| H | ? | pixi.lock | 20911 |
| H | ? | pixi.lock | 20912 |
| H | ? | pixi.lock | 20918 |
| H | ? | pixi.lock | 20927 |
| H | ? | pixi.lock | 20928 |
| H | ? | pixi.lock | 20929 |
| H | ? | pixi.lock | 20935 |
| H | ? | pixi.lock | 20944 |
| H | ? | pixi.lock | 20945 |
| H | ? | pixi.lock | 20947 |
| H | ? | pixi.lock | 20948 |
| H | ? | pixi.lock | 20949 |
| H | ? | pixi.lock | 20950 |
| H | ? | pixi.lock | 20956 |
| H | ? | pixi.lock | 20964 |
| H | ? | pixi.lock | 20965 |
| H | ? | pixi.lock | 20966 |
| H | ? | pixi.lock | 20967 |
| H | ? | pixi.lock | 20968 |
| H | ? | pixi.lock | 20969 |
| H | ? | pixi.lock | 20976 |
| H | ? | pixi.lock | 20983 |
| H | ? | pixi.lock | 20989 |
| H | ? | pixi.lock | 20998 |
| H | ? | pixi.lock | 21004 |
| H | ? | pixi.lock | 21011 |
| H | ? | pixi.lock | 21017 |
| H | ? | pixi.lock | 21026 |
| H | ? | pixi.lock | 21032 |
| H | ? | pixi.lock | 21040 |
| H | ? | pixi.lock | 21041 |
| H | ? | pixi.lock | 21042 |
| H | ? | pixi.lock | 21043 |
| H | ? | pixi.lock | 21044 |
| H | ? | pixi.lock | 21045 |
| H | ? | pixi.lock | 21046 |
| H | ? | pixi.lock | 21047 |
| H | ? | pixi.lock | 21048 |
| H | ? | pixi.lock | 21055 |
| H | ? | pixi.lock | 21065 |
| H | ? | pixi.lock | 21066 |
| H | ? | pixi.lock | 21067 |
| H | ? | pixi.lock | 21068 |
| H | ? | pixi.lock | 21069 |
| H | ? | pixi.lock | 21070 |
| H | ? | pixi.lock | 21071 |
| H | ? | pixi.lock | 21072 |
| H | ? | pixi.lock | 21073 |
| H | ? | pixi.lock | 21079 |
| H | ? | pixi.lock | 21087 |
| H | ? | pixi.lock | 21088 |
| H | ? | pixi.lock | 21089 |
| H | ? | pixi.lock | 21090 |
| H | ? | pixi.lock | 21111 |
| H | ? | pixi.lock | 21112 |
| H | ? | pixi.lock | 21114 |
| H | ? | pixi.lock | 21137 |
| H | ? | pixi.lock | 21145 |
| H | ? | pixi.lock | 21154 |
| H | ? | pixi.lock | 21162 |
| H | ? | pixi.lock | 21163 |
| H | ? | pixi.lock | 21171 |
| H | ? | pixi.lock | 21179 |
| H | ? | pixi.lock | 21190 |
| H | ? | pixi.lock | 21198 |
| H | ? | pixi.lock | 21199 |
| H | ? | pixi.lock | 21200 |
| H | ? | pixi.lock | 21208 |
| H | ? | pixi.lock | 21267 |
| H | ? | pixi.lock | 21913 |
| H | ? | pixi.lock | 23144 |
| H | ? | pixi.lock | 23321 |
| H | ? | pixi.lock | 23329 |
| H | ? | pixi.lock | 23330 |
| H | ? | pixi.lock | 23331 |
| H | ? | pixi.lock | 23332 |
| H | ? | pixi.lock | 23333 |
| H | ? | pixi.lock | 23334 |
| H | ? | pixi.lock | 23574 |
| H | ? | pixi.lock | 23751 |
| H | ? | pixi.lock | 23764 |
| H | ? | pixi.lock | 23767 |
| H | ? | pixi.lock | 23772 |
| H | ? | pixi.lock | 23795 |
| H | ? | pixi.lock | 23797 |
| H | ? | pixi.lock | 23798 |
| H | ? | pixi.lock | 23799 |
| H | ? | pixi.lock | 23800 |
| H | ? | pixi.lock | 23811 |
| H | ? | pixi.lock | 23815 |
| H | ? | pixi.lock | 23835 |
| H | ? | pixi.lock | 23837 |
| H | ? | pixi.lock | 23838 |
| H | ? | pixi.lock | 23839 |
| H | ? | pixi.lock | 23840 |
| H | ? | pixi.lock | 23851 |
| H | ? | pixi.lock | 23855 |
| H | ? | pixi.lock | 23875 |
| H | ? | pixi.lock | 23877 |
| H | ? | pixi.lock | 23878 |
| H | ? | pixi.lock | 23879 |
| H | ? | pixi.lock | 23880 |
| H | ? | pixi.lock | 23891 |
| H | ? | pixi.lock | 23895 |
| H | ? | pixi.lock | 23915 |
| H | ? | pixi.lock | 23917 |
| H | ? | pixi.lock | 23918 |
| H | ? | pixi.lock | 23919 |
| H | ? | pixi.lock | 23920 |
| H | ? | pixi.lock | 23931 |
| H | ? | pixi.lock | 23935 |
| H | ? | pixi.lock | 24185 |
| H | ? | pixi.lock | 24206 |
| H | ? | pixi.lock | 24227 |
| H | ? | pixi.lock | 24248 |
| H | ? | pixi.lock | 24263 |
| H | ? | pixi.lock | 24671 |
| H | ? | pixi.lock | 24921 |
| H | ? | pixi.lock | 24944 |
| H | ? | pixi.lock | 24967 |
| H | ? | pixi.lock | 25049 |
| H | ? | pixi.lock | 25073 |
| H | ? | pixi.lock | 25097 |
| H | ? | pixi.lock | 25121 |
| H | ? | pixi.lock | 25418 |
| H | ? | pixi.lock | 25447 |
| H | ? | pixi.lock | 25470 |
| H | ? | pixi.lock | 25522 |
| H | ? | pixi.lock | 25540 |
| H | ? | pixi.lock | 25558 |
| H | ? | pixi.lock | 25576 |
| H | ? | pixi.lock | 25661 |
| H | ? | pixi.lock | 25678 |
| H | ? | pixi.lock | 25696 |
| H | ? | pixi.lock | 25846 |
| H | ? | pixi.lock | 25921 |
| H | ? | pixi.lock | 25930 |
| H | ? | pixi.lock | 25938 |
| H | ? | pixi.lock | 25948 |
| H | ? | pixi.lock | 25959 |
| H | ? | pixi.lock | 26532 |
| H | ? | pixi.lock | 26546 |
| H | ? | pixi.lock | 26562 |
| H | ? | pixi.lock | 26576 |
| H | ? | pixi.lock | 26590 |
| H | ? | pixi.lock | 27509 |
| H | ? | pixi.lock | 27520 |
| H | ? | pixi.lock | 27535 |
| H | ? | pixi.lock | 27542 |
| H | ? | pixi.lock | 27557 |
| H | ? | pixi.lock | 27565 |
| H | ? | pixi.lock | 27943 |
| H | ? | pixi.lock | 27965 |
| H | ? | pixi.lock | 27991 |
| H | ? | pixi.lock | 28013 |
| H | ? | pixi.lock | 28102 |
| H | ? | pixi.lock | 29419 |
| H | ? | pixi.lock | 29886 |
| H | ? | pixi.lock | 29900 |
| H | ? | pixi.lock | 29962 |
| H | ? | pixi.lock | 30047 |
| H | ? | pixi.lock | 30297 |
| H | ? | pixi.lock | 30312 |
| H | ? | pixi.lock | 31388 |
| H | ? | pixi.lock | 31460 |
| H | ? | pixi.lock | 31476 |
| H | ? | pixi.lock | 31494 |
| H | ? | pixi.lock | 31510 |
| H | ? | pixi.lock | 31681 |
| H | ? | pixi.lock | 31691 |
| H | ? | pixi.lock | 31736 |
| H | ? | pixi.lock | 31737 |
| H | ? | pixi.lock | 31738 |
| H | ? | pixi.lock | 31739 |
| H | ? | pixi.lock | 31740 |
| H | ? | pixi.lock | 31746 |
| H | ? | pixi.lock | 31753 |
| H | ? | pixi.lock | 31754 |
| H | ? | pixi.lock | 31755 |
| H | ? | pixi.lock | 31756 |
| H | ? | pixi.lock | 31757 |
| H | ? | pixi.lock | 31763 |
| H | ? | pixi.lock | 31770 |
| H | ? | pixi.lock | 31777 |
| H | ? | pixi.lock | 31784 |
| H | ? | pixi.lock | 31792 |
| H | ? | pixi.lock | 31805 |
| H | ? | pixi.lock | 31817 |
| H | ? | pixi.lock | 31824 |
| H | ? | pixi.lock | 31830 |
| H | ? | pixi.lock | 31838 |
| H | ? | pixi.lock | 31844 |
| H | ? | pixi.lock | 31851 |
| H | ? | pixi.lock | 31852 |
| H | ? | pixi.lock | 31853 |
| H | ? | pixi.lock | 31860 |
| H | ? | pixi.lock | 31869 |
| H | ? | pixi.lock | 31870 |
| H | ? | pixi.lock | 31871 |
| H | ? | pixi.lock | 31877 |
| H | ? | pixi.lock | 31885 |
| H | ? | pixi.lock | 31886 |
| H | ? | pixi.lock | 31887 |
| H | ? | pixi.lock | 31888 |
| H | ? | pixi.lock | 31894 |
| H | ? | pixi.lock | 31901 |
| H | ? | pixi.lock | 31902 |
| H | ? | pixi.lock | 31903 |
| H | ? | pixi.lock | 31904 |
| H | ? | pixi.lock | 31910 |
| H | ? | pixi.lock | 31917 |
| H | ? | pixi.lock | 31918 |
| H | ? | pixi.lock | 31920 |
| H | ? | pixi.lock | 31925 |
| H | ? | pixi.lock | 31933 |
| H | ? | pixi.lock | 31934 |
| H | ? | pixi.lock | 31935 |
| H | ? | pixi.lock | 31941 |
| H | ? | pixi.lock | 31948 |
| H | ? | pixi.lock | 31949 |
| H | ? | pixi.lock | 31950 |
| H | ? | pixi.lock | 31956 |
| H | ? | pixi.lock | 31964 |
| H | ? | pixi.lock | 31965 |
| H | ? | pixi.lock | 31966 |
| H | ? | pixi.lock | 31972 |
| H | ? | pixi.lock | 31980 |
| H | ? | pixi.lock | 31981 |
| H | ? | pixi.lock | 31983 |
| H | ? | pixi.lock | 31984 |
| H | ? | pixi.lock | 31985 |
| H | ? | pixi.lock | 31986 |
| H | ? | pixi.lock | 31992 |
| H | ? | pixi.lock | 31999 |
| H | ? | pixi.lock | 32000 |
| H | ? | pixi.lock | 32001 |
| H | ? | pixi.lock | 32002 |
| H | ? | pixi.lock | 32003 |
| H | ? | pixi.lock | 32004 |
| H | ? | pixi.lock | 32011 |
| H | ? | pixi.lock | 32018 |
| H | ? | pixi.lock | 32024 |
| H | ? | pixi.lock | 32032 |
| H | ? | pixi.lock | 32038 |
| H | ? | pixi.lock | 32045 |
| H | ? | pixi.lock | 32051 |
| H | ? | pixi.lock | 32059 |
| H | ? | pixi.lock | 32065 |
| H | ? | pixi.lock | 32072 |
| H | ? | pixi.lock | 32073 |
| H | ? | pixi.lock | 32074 |
| H | ? | pixi.lock | 32075 |
| H | ? | pixi.lock | 32076 |
| H | ? | pixi.lock | 32077 |
| H | ? | pixi.lock | 32078 |
| H | ? | pixi.lock | 32079 |
| H | ? | pixi.lock | 32080 |
| H | ? | pixi.lock | 32087 |
| H | ? | pixi.lock | 32096 |
| H | ? | pixi.lock | 32097 |
| H | ? | pixi.lock | 32098 |
| H | ? | pixi.lock | 32099 |
| H | ? | pixi.lock | 32100 |
| H | ? | pixi.lock | 32101 |
| H | ? | pixi.lock | 32102 |
| H | ? | pixi.lock | 32103 |
| H | ? | pixi.lock | 32104 |
| H | ? | pixi.lock | 32110 |
| H | ? | pixi.lock | 32117 |
| H | ? | pixi.lock | 32118 |
| H | ? | pixi.lock | 32119 |
| H | ? | pixi.lock | 32120 |
| H | ? | pixi.lock | 32139 |
| H | ? | pixi.lock | 32140 |
| H | ? | pixi.lock | 32142 |
| H | ? | pixi.lock | 32165 |
| H | ? | pixi.lock | 32172 |
| H | ? | pixi.lock | 32181 |
| H | ? | pixi.lock | 32188 |
| H | ? | pixi.lock | 32189 |
| H | ? | pixi.lock | 32197 |
| H | ? | pixi.lock | 32204 |
| H | ? | pixi.lock | 32215 |
| H | ? | pixi.lock | 32222 |
| H | ? | pixi.lock | 32223 |
| H | ? | pixi.lock | 32224 |
| H | ? | pixi.lock | 32232 |
| H | ? | pixi.lock | 32288 |
| H | ? | pixi.lock | 32819 |
| H | ? | pixi.lock | 34020 |
| H | ? | pixi.lock | 34194 |
| H | ? | pixi.lock | 34201 |
| H | ? | pixi.lock | 34202 |
| H | ? | pixi.lock | 34203 |
| H | ? | pixi.lock | 34204 |
| H | ? | pixi.lock | 34205 |
| H | ? | pixi.lock | 34206 |
| H | ? | pixi.lock | 34437 |
| H | ? | pixi.lock | 34613 |
| H | ? | pixi.lock | 34626 |
| H | ? | pixi.lock | 34629 |
| H | ? | pixi.lock | 34634 |
| H | ? | pixi.lock | 34656 |
| H | ? | pixi.lock | 34658 |
| H | ? | pixi.lock | 34659 |
| H | ? | pixi.lock | 34660 |
| H | ? | pixi.lock | 34661 |
| H | ? | pixi.lock | 34672 |
| H | ? | pixi.lock | 34676 |
| H | ? | pixi.lock | 34695 |
| H | ? | pixi.lock | 34697 |
| H | ? | pixi.lock | 34698 |
| H | ? | pixi.lock | 34699 |
| H | ? | pixi.lock | 34700 |
| H | ? | pixi.lock | 34711 |
| H | ? | pixi.lock | 34715 |
| H | ? | pixi.lock | 34734 |
| H | ? | pixi.lock | 34736 |
| H | ? | pixi.lock | 34737 |
| H | ? | pixi.lock | 34738 |
| H | ? | pixi.lock | 34739 |
| H | ? | pixi.lock | 34750 |
| H | ? | pixi.lock | 34754 |
| H | ? | pixi.lock | 34773 |
| H | ? | pixi.lock | 34775 |
| H | ? | pixi.lock | 34776 |
| H | ? | pixi.lock | 34777 |
| H | ? | pixi.lock | 34778 |
| H | ? | pixi.lock | 34789 |
| H | ? | pixi.lock | 34793 |
| H | ? | pixi.lock | 35030 |
| H | ? | pixi.lock | 35050 |
| H | ? | pixi.lock | 35070 |
| H | ? | pixi.lock | 35090 |
| H | ? | pixi.lock | 35105 |
| H | ? | pixi.lock | 35476 |
| H | ? | pixi.lock | 35717 |
| H | ? | pixi.lock | 35739 |
| H | ? | pixi.lock | 35761 |
| H | ? | pixi.lock | 35840 |
| H | ? | pixi.lock | 35863 |
| H | ? | pixi.lock | 35886 |
| H | ? | pixi.lock | 35909 |
| H | ? | pixi.lock | 36188 |
| H | ? | pixi.lock | 36216 |
| H | ? | pixi.lock | 36239 |
| H | ? | pixi.lock | 36289 |
| H | ? | pixi.lock | 36306 |
| H | ? | pixi.lock | 36323 |
| H | ? | pixi.lock | 36340 |
| H | ? | pixi.lock | 36420 |
| H | ? | pixi.lock | 36436 |
| H | ? | pixi.lock | 36453 |
| H | ? | pixi.lock | 36583 |
| H | ? | pixi.lock | 36675 |
| H | ? | pixi.lock | 36684 |
| H | ? | pixi.lock | 36691 |
| H | ? | pixi.lock | 36701 |
| H | ? | pixi.lock | 36711 |
| H | ? | pixi.lock | 37240 |
| H | ? | pixi.lock | 37254 |
| H | ? | pixi.lock | 37269 |
| H | ? | pixi.lock | 37283 |
| H | ? | pixi.lock | 37297 |
| H | ? | pixi.lock | 38190 |
| H | ? | pixi.lock | 38201 |
| H | ? | pixi.lock | 38212 |
| H | ? | pixi.lock | 38222 |
| H | ? | pixi.lock | 38232 |
| H | ? | pixi.lock | 38244 |
| H | ? | pixi.lock | 38616 |
| H | ? | pixi.lock | 38642 |
| H | ? | pixi.lock | 38666 |
| H | ? | pixi.lock | 38685 |
| H | ? | pixi.lock | 38775 |
| H | ? | pixi.lock | 40027 |
| H | ? | pixi.lock | 40487 |
| H | ? | pixi.lock | 40501 |
| H | ? | pixi.lock | 40562 |
| H | ? | pixi.lock | 40636 |
| H | ? | pixi.lock | 40892 |
| H | ? | pixi.lock | 40906 |
| H | ? | pixi.lock | 41918 |
| H | ? | pixi.lock | 41987 |
| H | ? | pixi.lock | 42003 |
| H | ? | pixi.lock | 42021 |
| H | ? | pixi.lock | 42037 |
| H | ? | pixi.lock | 42078 |
| H | ? | pixi.lock | 42095 |
| H | ? | pixi.lock | 42110 |
| H | ? | pixi.lock | 42125 |
| H | ? | pixi.lock | 42142 |
| H | ? | pixi.lock | 42157 |
| H | ? | pixi.lock | 42815 |
| H | ? | pixi.lock | 42816 |
| H | ? | pixi.lock | 42894 |
| H | ? | pixi.lock | 43201 |
| H | ? | pixi.lock | 43658 |
| H | ? | pixi.lock | 44818 |
| H | ? | pixi.lock | 45750 |
| H | ? | pixi.lock | 46217 |
| H | ? | pixi.lock | 46227 |
| H | ? | pixi.lock | 46237 |
| H | ? | pixi.lock | 46247 |
| H | ? | pixi.lock | 46796 |
| H | ? | pixi.lock | 46797 |
| H | ? | pixi.lock | 46798 |
| H | ? | pixi.lock | 46799 |
| H | ? | pixi.lock | 46800 |
| H | ? | pixi.lock | 46806 |
| H | ? | pixi.lock | 46814 |
| H | ? | pixi.lock | 46815 |
| H | ? | pixi.lock | 46816 |
| H | ? | pixi.lock | 46817 |
| H | ? | pixi.lock | 46818 |
| H | ? | pixi.lock | 46823 |
| H | ? | pixi.lock | 46831 |
| H | ? | pixi.lock | 46837 |
| H | ? | pixi.lock | 46845 |
| H | ? | pixi.lock | 46851 |
| H | ? | pixi.lock | 46863 |
| H | ? | pixi.lock | 46876 |
| H | ? | pixi.lock | 46884 |
| H | ? | pixi.lock | 46889 |
| H | ? | pixi.lock | 46897 |
| H | ? | pixi.lock | 46903 |
| H | ? | pixi.lock | 46911 |
| H | ? | pixi.lock | 46912 |
| H | ? | pixi.lock | 46913 |
| H | ? | pixi.lock | 46919 |
| H | ? | pixi.lock | 46928 |
| H | ? | pixi.lock | 46929 |
| H | ? | pixi.lock | 46930 |
| H | ? | pixi.lock | 46936 |
| H | ? | pixi.lock | 46944 |
| H | ? | pixi.lock | 46945 |
| H | ? | pixi.lock | 46946 |
| H | ? | pixi.lock | 46947 |
| H | ? | pixi.lock | 46953 |
| H | ? | pixi.lock | 46961 |
| H | ? | pixi.lock | 46962 |
| H | ? | pixi.lock | 46963 |
| H | ? | pixi.lock | 46964 |
| H | ? | pixi.lock | 46969 |
| H | ? | pixi.lock | 46977 |
| H | ? | pixi.lock | 46978 |
| H | ? | pixi.lock | 46983 |
| H | ? | pixi.lock | 46991 |
| H | ? | pixi.lock | 46992 |
| H | ? | pixi.lock | 46993 |
| H | ? | pixi.lock | 46999 |
| H | ? | pixi.lock | 47007 |
| H | ? | pixi.lock | 47008 |
| H | ? | pixi.lock | 47009 |
| H | ? | pixi.lock | 47014 |
| H | ? | pixi.lock | 47022 |
| H | ? | pixi.lock | 47023 |
| H | ? | pixi.lock | 47024 |
| H | ? | pixi.lock | 47030 |
| H | ? | pixi.lock | 47038 |
| H | ? | pixi.lock | 47039 |
| H | ? | pixi.lock | 47040 |
| H | ? | pixi.lock | 47041 |
| H | ? | pixi.lock | 47042 |
| H | ? | pixi.lock | 47043 |
| H | ? | pixi.lock | 47049 |
| H | ? | pixi.lock | 47057 |
| H | ? | pixi.lock | 47058 |
| H | ? | pixi.lock | 47059 |
| H | ? | pixi.lock | 47060 |
| H | ? | pixi.lock | 47061 |
| H | ? | pixi.lock | 47062 |
| H | ? | pixi.lock | 47067 |
| H | ? | pixi.lock | 47075 |
| H | ? | pixi.lock | 47080 |
| H | ? | pixi.lock | 47088 |
| H | ? | pixi.lock | 47094 |
| H | ? | pixi.lock | 47102 |
| H | ? | pixi.lock | 47108 |
| H | ? | pixi.lock | 47116 |
| H | ? | pixi.lock | 47121 |
| H | ? | pixi.lock | 47129 |
| H | ? | pixi.lock | 47130 |
| H | ? | pixi.lock | 47131 |
| H | ? | pixi.lock | 47132 |
| H | ? | pixi.lock | 47133 |
| H | ? | pixi.lock | 47134 |
| H | ? | pixi.lock | 47135 |
| H | ? | pixi.lock | 47136 |
| H | ? | pixi.lock | 47137 |
| H | ? | pixi.lock | 47143 |
| H | ? | pixi.lock | 47152 |
| H | ? | pixi.lock | 47153 |
| H | ? | pixi.lock | 47154 |
| H | ? | pixi.lock | 47155 |
| H | ? | pixi.lock | 47156 |
| H | ? | pixi.lock | 47157 |
| H | ? | pixi.lock | 47158 |
| H | ? | pixi.lock | 47159 |
| H | ? | pixi.lock | 47160 |
| H | ? | pixi.lock | 47166 |
| H | ? | pixi.lock | 47174 |
| H | ? | pixi.lock | 47175 |
| H | ? | pixi.lock | 47176 |
| H | ? | pixi.lock | 47177 |
| H | ? | pixi.lock | 47195 |
| H | ? | pixi.lock | 47196 |
| H | ? | pixi.lock | 47197 |
| H | ? | pixi.lock | 47221 |
| H | ? | pixi.lock | 47229 |
| H | ? | pixi.lock | 47237 |
| H | ? | pixi.lock | 47245 |
| H | ? | pixi.lock | 47246 |
| H | ? | pixi.lock | 47253 |
| H | ? | pixi.lock | 47261 |
| H | ? | pixi.lock | 47271 |
| H | ? | pixi.lock | 47279 |
| H | ? | pixi.lock | 47280 |
| H | ? | pixi.lock | 47281 |
| H | ? | pixi.lock | 47288 |
| H | ? | pixi.lock | 49065 |
| H | ? | pixi.lock | 49073 |
| H | ? | pixi.lock | 49074 |
| H | ? | pixi.lock | 49075 |
| H | ? | pixi.lock | 49076 |
| H | ? | pixi.lock | 49077 |
| H | ? | pixi.lock | 49078 |
| H | ? | pixi.lock | 49276 |
| H | ? | pixi.lock | 49328 |
| H | ? | pixi.lock | 49484 |
| H | ? | pixi.lock | 49499 |
| H | ? | pixi.lock | 49520 |
| H | ? | pixi.lock | 49522 |
| H | ? | pixi.lock | 49523 |
| H | ? | pixi.lock | 49524 |
| H | ? | pixi.lock | 49525 |
| H | ? | pixi.lock | 49536 |
| H | ? | pixi.lock | 49539 |
| H | ? | pixi.lock | 49559 |
| H | ? | pixi.lock | 49561 |
| H | ? | pixi.lock | 49562 |
| H | ? | pixi.lock | 49563 |
| H | ? | pixi.lock | 49564 |
| H | ? | pixi.lock | 49575 |
| H | ? | pixi.lock | 49578 |
| H | ? | pixi.lock | 49598 |
| H | ? | pixi.lock | 49600 |
| H | ? | pixi.lock | 49601 |
| H | ? | pixi.lock | 49602 |
| H | ? | pixi.lock | 49603 |
| H | ? | pixi.lock | 49614 |
| H | ? | pixi.lock | 49617 |
| H | ? | pixi.lock | 49637 |
| H | ? | pixi.lock | 49639 |
| H | ? | pixi.lock | 49640 |
| H | ? | pixi.lock | 49641 |
| H | ? | pixi.lock | 49642 |
| H | ? | pixi.lock | 49653 |
| H | ? | pixi.lock | 49656 |
| H | ? | pixi.lock | 49698 |
| H | ? | pixi.lock | 49718 |
| H | ? | pixi.lock | 49738 |
| H | ? | pixi.lock | 49758 |
| H | ? | pixi.lock | 49778 |
| H | ? | pixi.lock | 49800 |
| H | ? | pixi.lock | 49822 |
| H | ? | pixi.lock | 49844 |
| H | ? | pixi.lock | 49887 |
| H | ? | pixi.lock | 49909 |
| H | ? | pixi.lock | 49931 |
| H | ? | pixi.lock | 49953 |
| H | ? | pixi.lock | 49973 |
| H | ? | pixi.lock | 49990 |
| H | ? | pixi.lock | 50028 |
| H | ? | pixi.lock | 50048 |
| H | ? | pixi.lock | 50068 |
| H | ? | pixi.lock | 50088 |
| H | ? | pixi.lock | 50108 |
| H | ? | pixi.lock | 50122 |
| H | ? | pixi.lock | 50388 |
| H | ? | pixi.lock | 50400 |
| H | ? | pixi.lock | 50455 |
| H | ? | pixi.lock | 50577 |
| H | ? | pixi.lock | 50599 |
| H | ? | pixi.lock | 50621 |
| H | ? | pixi.lock | 50700 |
| H | ? | pixi.lock | 50723 |
| H | ? | pixi.lock | 50746 |
| H | ? | pixi.lock | 50769 |
| H | ? | pixi.lock | 51098 |
| H | ? | pixi.lock | 51116 |
| H | ? | pixi.lock | 51139 |
| H | ? | pixi.lock | 51189 |
| H | ? | pixi.lock | 51209 |
| H | ? | pixi.lock | 51210 |
| H | ? | pixi.lock | 51230 |
| H | ? | pixi.lock | 51231 |
| H | ? | pixi.lock | 51251 |
| H | ? | pixi.lock | 51252 |
| H | ? | pixi.lock | 51272 |
| H | ? | pixi.lock | 51273 |
| H | ? | pixi.lock | 51340 |
| H | ? | pixi.lock | 51356 |
| H | ? | pixi.lock | 51373 |
| H | ? | pixi.lock | 51481 |
| H | ? | pixi.lock | 51531 |
| H | ? | pixi.lock | 51538 |
| H | ? | pixi.lock | 51547 |
| H | ? | pixi.lock | 51555 |
| H | ? | pixi.lock | 51566 |
| H | ? | pixi.lock | 52071 |
| H | ? | pixi.lock | 52084 |
| H | ? | pixi.lock | 52098 |
| H | ? | pixi.lock | 52111 |
| H | ? | pixi.lock | 52124 |
| H | ? | pixi.lock | 52979 |
| H | ? | pixi.lock | 52989 |
| H | ? | pixi.lock | 52999 |
| H | ? | pixi.lock | 53010 |
| H | ? | pixi.lock | 53025 |
| H | ? | pixi.lock | 53032 |
| H | ? | pixi.lock | 53388 |
| H | ? | pixi.lock | 53409 |
| H | ? | pixi.lock | 53434 |
| H | ? | pixi.lock | 53451 |
| H | ? | pixi.lock | 54613 |
| H | ? | pixi.lock | 55230 |
| H | ? | pixi.lock | 55616 |
| H | ? | pixi.lock | 55939 |
| H | ? | pixi.lock | 56008 |
| H | ? | pixi.lock | 56023 |
| H | ? | pixi.lock | 56040 |
| H | ? | pixi.lock | 56055 |
| H | ? | pixi.lock | 56265 |
| H | ? | pixi.lock | 56266 |
| H | ? | pixi.lock | 56267 |
| H | ? | pixi.lock | 56268 |
| H | ? | pixi.lock | 56269 |
| H | ? | pixi.lock | 56275 |
| H | ? | pixi.lock | 56283 |
| H | ? | pixi.lock | 56284 |
| H | ? | pixi.lock | 56285 |
| H | ? | pixi.lock | 56286 |
| H | ? | pixi.lock | 56287 |
| H | ? | pixi.lock | 56292 |
| H | ? | pixi.lock | 56300 |
| H | ? | pixi.lock | 56306 |
| H | ? | pixi.lock | 56314 |
| H | ? | pixi.lock | 56320 |
| H | ? | pixi.lock | 56333 |
| H | ? | pixi.lock | 56345 |
| H | ? | pixi.lock | 56353 |
| H | ? | pixi.lock | 56358 |
| H | ? | pixi.lock | 56366 |
| H | ? | pixi.lock | 56372 |
| H | ? | pixi.lock | 56380 |
| H | ? | pixi.lock | 56381 |
| H | ? | pixi.lock | 56382 |
| H | ? | pixi.lock | 56388 |
| H | ? | pixi.lock | 56397 |
| H | ? | pixi.lock | 56398 |
| H | ? | pixi.lock | 56399 |
| H | ? | pixi.lock | 56405 |
| H | ? | pixi.lock | 56413 |
| H | ? | pixi.lock | 56414 |
| H | ? | pixi.lock | 56415 |
| H | ? | pixi.lock | 56416 |
| H | ? | pixi.lock | 56422 |
| H | ? | pixi.lock | 56430 |
| H | ? | pixi.lock | 56431 |
| H | ? | pixi.lock | 56432 |
| H | ? | pixi.lock | 56433 |
| H | ? | pixi.lock | 56438 |
| H | ? | pixi.lock | 56446 |
| H | ? | pixi.lock | 56447 |
| H | ? | pixi.lock | 56452 |
| H | ? | pixi.lock | 56460 |
| H | ? | pixi.lock | 56461 |
| H | ? | pixi.lock | 56462 |
| H | ? | pixi.lock | 56468 |
| H | ? | pixi.lock | 56476 |
| H | ? | pixi.lock | 56477 |
| H | ? | pixi.lock | 56478 |
| H | ? | pixi.lock | 56483 |
| H | ? | pixi.lock | 56491 |
| H | ? | pixi.lock | 56492 |
| H | ? | pixi.lock | 56493 |
| H | ? | pixi.lock | 56499 |
| H | ? | pixi.lock | 56507 |
| H | ? | pixi.lock | 56508 |
| H | ? | pixi.lock | 56509 |
| H | ? | pixi.lock | 56510 |
| H | ? | pixi.lock | 56511 |
| H | ? | pixi.lock | 56512 |
| H | ? | pixi.lock | 56518 |
| H | ? | pixi.lock | 56526 |
| H | ? | pixi.lock | 56527 |
| H | ? | pixi.lock | 56528 |
| H | ? | pixi.lock | 56529 |
| H | ? | pixi.lock | 56530 |
| H | ? | pixi.lock | 56531 |
| H | ? | pixi.lock | 56536 |
| H | ? | pixi.lock | 56544 |
| H | ? | pixi.lock | 56549 |
| H | ? | pixi.lock | 56557 |
| H | ? | pixi.lock | 56563 |
| H | ? | pixi.lock | 56571 |
| H | ? | pixi.lock | 56576 |
| H | ? | pixi.lock | 56584 |
| H | ? | pixi.lock | 56590 |
| H | ? | pixi.lock | 56598 |
| H | ? | pixi.lock | 56599 |
| H | ? | pixi.lock | 56600 |
| H | ? | pixi.lock | 56601 |
| H | ? | pixi.lock | 56602 |
| H | ? | pixi.lock | 56603 |
| H | ? | pixi.lock | 56604 |
| H | ? | pixi.lock | 56605 |
| H | ? | pixi.lock | 56606 |
| H | ? | pixi.lock | 56612 |
| H | ? | pixi.lock | 56621 |
| H | ? | pixi.lock | 56622 |
| H | ? | pixi.lock | 56623 |
| H | ? | pixi.lock | 56624 |
| H | ? | pixi.lock | 56625 |
| H | ? | pixi.lock | 56626 |
| H | ? | pixi.lock | 56627 |
| H | ? | pixi.lock | 56628 |
| H | ? | pixi.lock | 56629 |
| H | ? | pixi.lock | 56635 |
| H | ? | pixi.lock | 56643 |
| H | ? | pixi.lock | 56644 |
| H | ? | pixi.lock | 56645 |
| H | ? | pixi.lock | 56646 |
| H | ? | pixi.lock | 56665 |
| H | ? | pixi.lock | 56667 |
| H | ? | pixi.lock | 56668 |
| H | ? | pixi.lock | 56690 |
| H | ? | pixi.lock | 56698 |
| H | ? | pixi.lock | 56706 |
| H | ? | pixi.lock | 56714 |
| H | ? | pixi.lock | 56715 |
| H | ? | pixi.lock | 56722 |
| H | ? | pixi.lock | 56730 |
| H | ? | pixi.lock | 56740 |
| H | ? | pixi.lock | 56748 |
| H | ? | pixi.lock | 56749 |
| H | ? | pixi.lock | 56750 |
| H | ? | pixi.lock | 56757 |
| H | ? | pixi.lock | 58603 |
| H | ? | pixi.lock | 58611 |
| H | ? | pixi.lock | 58612 |
| H | ? | pixi.lock | 58613 |
| H | ? | pixi.lock | 58614 |
| H | ? | pixi.lock | 58615 |
| H | ? | pixi.lock | 58616 |
| H | ? | pixi.lock | 58822 |
| H | ? | pixi.lock | 58887 |
| H | ? | pixi.lock | 59043 |
| H | ? | pixi.lock | 59055 |
| H | ? | pixi.lock | 59057 |
| H | ? | pixi.lock | 59062 |
| H | ? | pixi.lock | 59084 |
| H | ? | pixi.lock | 59086 |
| H | ? | pixi.lock | 59087 |
| H | ? | pixi.lock | 59088 |
| H | ? | pixi.lock | 59089 |
| H | ? | pixi.lock | 59100 |
| H | ? | pixi.lock | 59103 |
| H | ? | pixi.lock | 59123 |
| H | ? | pixi.lock | 59125 |
| H | ? | pixi.lock | 59126 |
| H | ? | pixi.lock | 59127 |
| H | ? | pixi.lock | 59128 |
| H | ? | pixi.lock | 59139 |
| H | ? | pixi.lock | 59142 |
| H | ? | pixi.lock | 59162 |
| H | ? | pixi.lock | 59164 |
| H | ? | pixi.lock | 59165 |
| H | ? | pixi.lock | 59166 |
| H | ? | pixi.lock | 59167 |
| H | ? | pixi.lock | 59178 |
| H | ? | pixi.lock | 59181 |
| H | ? | pixi.lock | 59201 |
| H | ? | pixi.lock | 59203 |
| H | ? | pixi.lock | 59204 |
| H | ? | pixi.lock | 59205 |
| H | ? | pixi.lock | 59206 |
| H | ? | pixi.lock | 59217 |
| H | ? | pixi.lock | 59220 |
| H | ? | pixi.lock | 59247 |
| H | ? | pixi.lock | 59267 |
| H | ? | pixi.lock | 59287 |
| H | ? | pixi.lock | 59307 |
| H | ? | pixi.lock | 59327 |
| H | ? | pixi.lock | 59349 |
| H | ? | pixi.lock | 59371 |
| H | ? | pixi.lock | 59393 |
| H | ? | pixi.lock | 59419 |
| H | ? | pixi.lock | 59441 |
| H | ? | pixi.lock | 59463 |
| H | ? | pixi.lock | 59485 |
| H | ? | pixi.lock | 59506 |
| H | ? | pixi.lock | 59526 |
| H | ? | pixi.lock | 59546 |
| H | ? | pixi.lock | 59566 |
| H | ? | pixi.lock | 59580 |
| H | ? | pixi.lock | 59845 |
| H | ? | pixi.lock | 59901 |
| H | ? | pixi.lock | 60023 |
| H | ? | pixi.lock | 60045 |
| H | ? | pixi.lock | 60067 |
| H | ? | pixi.lock | 60145 |
| H | ? | pixi.lock | 60168 |
| H | ? | pixi.lock | 60191 |
| H | ? | pixi.lock | 60214 |
| H | ? | pixi.lock | 60541 |
| H | ? | pixi.lock | 60559 |
| H | ? | pixi.lock | 60581 |
| H | ? | pixi.lock | 60635 |
| H | ? | pixi.lock | 60636 |
| H | ? | pixi.lock | 60656 |
| H | ? | pixi.lock | 60657 |
| H | ? | pixi.lock | 60677 |
| H | ? | pixi.lock | 60678 |
| H | ? | pixi.lock | 60698 |
| H | ? | pixi.lock | 60699 |
| H | ? | pixi.lock | 60766 |
| H | ? | pixi.lock | 60782 |
| H | ? | pixi.lock | 60799 |
| H | ? | pixi.lock | 60906 |
| H | ? | pixi.lock | 60941 |
| H | ? | pixi.lock | 60948 |
| H | ? | pixi.lock | 60957 |
| H | ? | pixi.lock | 60965 |
| H | ? | pixi.lock | 60976 |
| H | ? | pixi.lock | 61522 |
| H | ? | pixi.lock | 61535 |
| H | ? | pixi.lock | 61550 |
| H | ? | pixi.lock | 61563 |
| H | ? | pixi.lock | 61576 |
| H | ? | pixi.lock | 62452 |
| H | ? | pixi.lock | 62462 |
| H | ? | pixi.lock | 62475 |
| H | ? | pixi.lock | 62483 |
| H | ? | pixi.lock | 62493 |
| H | ? | pixi.lock | 62505 |
| H | ? | pixi.lock | 62863 |
| H | ? | pixi.lock | 62885 |
| H | ? | pixi.lock | 62916 |
| H | ? | pixi.lock | 62934 |
| H | ? | pixi.lock | 63023 |
| H | ? | pixi.lock | 64084 |
| H | ? | pixi.lock | 64718 |
| H | ? | pixi.lock | 65097 |
| H | ? | pixi.lock | 65436 |
| H | ? | pixi.lock | 65506 |
| H | ? | pixi.lock | 65522 |
| H | ? | pixi.lock | 65540 |
| H | ? | pixi.lock | 65556 |
| H | ? | pixi.lock | 65777 |
| H | ? | pixi.lock | 65778 |
| H | ? | pixi.lock | 65779 |
| H | ? | pixi.lock | 65780 |
| H | ? | pixi.lock | 65781 |
| H | ? | pixi.lock | 65787 |
| H | ? | pixi.lock | 65794 |
| H | ? | pixi.lock | 65795 |
| H | ? | pixi.lock | 65796 |
| H | ? | pixi.lock | 65797 |
| H | ? | pixi.lock | 65798 |
| H | ? | pixi.lock | 65806 |
| H | ? | pixi.lock | 65813 |
| H | ? | pixi.lock | 65822 |
| H | ? | pixi.lock | 65829 |
| H | ? | pixi.lock | 65838 |
| H | ? | pixi.lock | 65853 |
| H | ? | pixi.lock | 65867 |
| H | ? | pixi.lock | 65874 |
| H | ? | pixi.lock | 65882 |
| H | ? | pixi.lock | 65892 |
| H | ? | pixi.lock | 65898 |
| H | ? | pixi.lock | 65905 |
| H | ? | pixi.lock | 65906 |
| H | ? | pixi.lock | 65907 |
| H | ? | pixi.lock | 65915 |
| H | ? | pixi.lock | 65925 |
| H | ? | pixi.lock | 65926 |
| H | ? | pixi.lock | 65927 |
| H | ? | pixi.lock | 65933 |
| H | ? | pixi.lock | 65943 |
| H | ? | pixi.lock | 65944 |
| H | ? | pixi.lock | 65945 |
| H | ? | pixi.lock | 65946 |
| H | ? | pixi.lock | 65952 |
| H | ? | pixi.lock | 65959 |
| H | ? | pixi.lock | 65960 |
| H | ? | pixi.lock | 65961 |
| H | ? | pixi.lock | 65962 |
| H | ? | pixi.lock | 65970 |
| H | ? | pixi.lock | 65977 |
| H | ? | pixi.lock | 65978 |
| H | ? | pixi.lock | 65986 |
| H | ? | pixi.lock | 65996 |
| H | ? | pixi.lock | 65997 |
| H | ? | pixi.lock | 66003 |
| H | ? | pixi.lock | 66010 |
| H | ? | pixi.lock | 66011 |
| H | ? | pixi.lock | 66012 |
| H | ? | pixi.lock | 66020 |
| H | ? | pixi.lock | 66030 |
| H | ? | pixi.lock | 66031 |
| H | ? | pixi.lock | 66032 |
| H | ? | pixi.lock | 66038 |
| H | ? | pixi.lock | 66048 |
| H | ? | pixi.lock | 66049 |
| H | ? | pixi.lock | 66050 |
| H | ? | pixi.lock | 66051 |
| H | ? | pixi.lock | 66052 |
| H | ? | pixi.lock | 66053 |
| H | ? | pixi.lock | 66059 |
| H | ? | pixi.lock | 66066 |
| H | ? | pixi.lock | 66067 |
| H | ? | pixi.lock | 66068 |
| H | ? | pixi.lock | 66069 |
| H | ? | pixi.lock | 66070 |
| H | ? | pixi.lock | 66071 |
| H | ? | pixi.lock | 66079 |
| H | ? | pixi.lock | 66086 |
| H | ? | pixi.lock | 66094 |
| H | ? | pixi.lock | 66104 |
| H | ? | pixi.lock | 66110 |
| H | ? | pixi.lock | 66117 |
| H | ? | pixi.lock | 66125 |
| H | ? | pixi.lock | 66135 |
| H | ? | pixi.lock | 66141 |
| H | ? | pixi.lock | 66148 |
| H | ? | pixi.lock | 66149 |
| H | ? | pixi.lock | 66150 |
| H | ? | pixi.lock | 66151 |
| H | ? | pixi.lock | 66152 |
| H | ? | pixi.lock | 66153 |
| H | ? | pixi.lock | 66154 |
| H | ? | pixi.lock | 66155 |
| H | ? | pixi.lock | 66156 |
| H | ? | pixi.lock | 66164 |
| H | ? | pixi.lock | 66174 |
| H | ? | pixi.lock | 66175 |
| H | ? | pixi.lock | 66176 |
| H | ? | pixi.lock | 66177 |
| H | ? | pixi.lock | 66178 |
| H | ? | pixi.lock | 66179 |
| H | ? | pixi.lock | 66180 |
| H | ? | pixi.lock | 66181 |
| H | ? | pixi.lock | 66182 |
| H | ? | pixi.lock | 66188 |
| H | ? | pixi.lock | 66195 |
| H | ? | pixi.lock | 66196 |
| H | ? | pixi.lock | 66197 |
| H | ? | pixi.lock | 66198 |
| H | ? | pixi.lock | 66217 |
| H | ? | pixi.lock | 66219 |
| H | ? | pixi.lock | 66220 |
| H | ? | pixi.lock | 66241 |
| H | ? | pixi.lock | 66248 |
| H | ? | pixi.lock | 66257 |
| H | ? | pixi.lock | 66264 |
| H | ? | pixi.lock | 66265 |
| H | ? | pixi.lock | 66274 |
| H | ? | pixi.lock | 66281 |
| H | ? | pixi.lock | 66290 |
| H | ? | pixi.lock | 66297 |
| H | ? | pixi.lock | 66298 |
| H | ? | pixi.lock | 66299 |
| H | ? | pixi.lock | 66308 |
| H | ? | pixi.lock | 66851 |
| H | ? | pixi.lock | 67945 |
| H | ? | pixi.lock | 67952 |
| H | ? | pixi.lock | 67953 |
| H | ? | pixi.lock | 67954 |
| H | ? | pixi.lock | 67955 |
| H | ? | pixi.lock | 67956 |
| H | ? | pixi.lock | 67957 |
| H | ? | pixi.lock | 68146 |
| H | ? | pixi.lock | 68323 |
| H | ? | pixi.lock | 68335 |
| H | ? | pixi.lock | 68337 |
| H | ? | pixi.lock | 68342 |
| H | ? | pixi.lock | 68366 |
| H | ? | pixi.lock | 68368 |
| H | ? | pixi.lock | 68369 |
| H | ? | pixi.lock | 68370 |
| H | ? | pixi.lock | 68371 |
| H | ? | pixi.lock | 68381 |
| H | ? | pixi.lock | 68384 |
| H | ? | pixi.lock | 68406 |
| H | ? | pixi.lock | 68408 |
| H | ? | pixi.lock | 68409 |
| H | ? | pixi.lock | 68410 |
| H | ? | pixi.lock | 68411 |
| H | ? | pixi.lock | 68421 |
| H | ? | pixi.lock | 68424 |
| H | ? | pixi.lock | 68446 |
| H | ? | pixi.lock | 68448 |
| H | ? | pixi.lock | 68449 |
| H | ? | pixi.lock | 68450 |
| H | ? | pixi.lock | 68451 |
| H | ? | pixi.lock | 68461 |
| H | ? | pixi.lock | 68464 |
| H | ? | pixi.lock | 68486 |
| H | ? | pixi.lock | 68488 |
| H | ? | pixi.lock | 68489 |
| H | ? | pixi.lock | 68490 |
| H | ? | pixi.lock | 68491 |
| H | ? | pixi.lock | 68501 |
| H | ? | pixi.lock | 68504 |
| H | ? | pixi.lock | 68755 |
| H | ? | pixi.lock | 68776 |
| H | ? | pixi.lock | 68797 |
| H | ? | pixi.lock | 68818 |
| H | ? | pixi.lock | 69112 |
| H | ? | pixi.lock | 69232 |
| H | ? | pixi.lock | 69254 |
| H | ? | pixi.lock | 69276 |
| H | ? | pixi.lock | 69355 |
| H | ? | pixi.lock | 69379 |
| H | ? | pixi.lock | 69403 |
| H | ? | pixi.lock | 69427 |
| H | ? | pixi.lock | 69509 |
| H | ? | pixi.lock | 69674 |
| H | ? | pixi.lock | 69697 |
| H | ? | pixi.lock | 69733 |
| H | ? | pixi.lock | 69751 |
| H | ? | pixi.lock | 69769 |
| H | ? | pixi.lock | 69787 |
| H | ? | pixi.lock | 69862 |
| H | ? | pixi.lock | 69879 |
| H | ? | pixi.lock | 69897 |
| H | ? | pixi.lock | 70001 |
| H | ? | pixi.lock | 70052 |
| H | ? | pixi.lock | 70062 |
| H | ? | pixi.lock | 70069 |
| H | ? | pixi.lock | 70080 |
| H | ? | pixi.lock | 70089 |
| H | ? | pixi.lock | 70678 |
| H | ? | pixi.lock | 70692 |
| H | ? | pixi.lock | 70708 |
| H | ? | pixi.lock | 70722 |
| H | ? | pixi.lock | 70736 |
| H | ? | pixi.lock | 71595 |
| H | ? | pixi.lock | 71608 |
| H | ? | pixi.lock | 71623 |
| H | ? | pixi.lock | 71630 |
| H | ? | pixi.lock | 71645 |
| H | ? | pixi.lock | 71653 |
| H | ? | pixi.lock | 72024 |
| H | ? | pixi.lock | 72049 |
| H | ? | pixi.lock | 72078 |
| H | ? | pixi.lock | 72100 |
| H | ? | pixi.lock | 72190 |
| H | ? | pixi.lock | 73424 |
| H | ? | pixi.lock | 73869 |
| H | ? | pixi.lock | 73964 |
| H | ? | pixi.lock | 74497 |
| H | ? | pixi.lock | 74948 |
| H | ? | pixi.lock | 74955 |
| H | ? | pixi.lock | 75024 |
| H | ? | pixi.lock | 75044 |
| H | ? | pixi.lock | 75066 |
| H | ? | pixi.lock | 75086 |
| C | ? | hashing.py | 45 |
| M | ? | validate_min_versions_in_sync.py | 32 |
| M | ? | validate_min_versions_in_sync.py | 283 |
| M | ? | run_stubtest.py | 98 |
| H | ? | eval.py | 25 |
| H | ? | eval.py | 28 |
| H | ? | eval.py | 34 |
| H | ? | eval.py | 37 |
| H | ? | frame.py | 5280 |
| H | ? | frame.py | 5291 |
| H | ? | frame.py | 5308 |
| H | ? | frame.py | 5324 |
| H | ? | frame.py | 5336 |
| H | ? | ops.py | 430 |
| H | ? | eval.py | 179 |
| H | ? | eval_performance.py | 20 |
| H | ? | eval_performance.py | 107 |
| C | ? | pickle.py | 240 |
| H | ? | environment.yml | 0 |
| H | ? | pyright_reportGeneralTypeIssues.json | 0 |
| H | ? | codecov.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| C | GS005 | sql.py | 2483 |
| I | GS007 | csv.py | 735 |
| I | GS007 | reshape.py | 177 |
| I | GS007 | _doctools.py | 140 |
| s | GS009 |  | 0 |
| L | GS012 | format.py | 1028 |
| H | GS014 | sql.py | 369 |
| H | GS014 | sql.py | 683 |
| M | ? | package.py | 15 |

---
*Сгенерировано GSC v0.6 · 2026-07-29T04:03:56.625004*