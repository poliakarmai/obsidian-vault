---
title: "GSC Audit: /tmp/gsc-learn/pandas"
date: 2026-07-18
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pandas

**Дата:** 18.07.2026 04:03  
**Путь:** `/tmp/gsc-learn/pandas`  
**Всего находок:** 2355  
**CRITICAL:** 15 | **HIGH:** 1328 | **MEDIUM:** 448 | **LOW:** 562

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Хардкод IP адреса | 1248 |
| Python: assert in production | 420 |
| CVE-2026-56233: Path traversal | 56 |
| GS003 | 18 |
| Bare except: | 16 |
| eval() or exec() usage | 13 |
| GS008 | 12 |
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
| CVE-2026-55721: SQL injection | 6 |
| CVE-2026-37270: Hardcoded credential | 6 |
| Python: File upload without content-type validation | 4 |
| Outdated dependency pattern | 3 |
| CVE-2026-55223: Insecure deserialization | 2 |
| GS014 | 2 |
| CVE-2026-56219: Authentication bypass | 1 |
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
| HIGH | ? | _odswriter.py | 92 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _openpyxl.py | 109 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | format.py | 1028 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | algorithms.py | 896 |  |
| HIGH | ? | style_render.py | 1203 |  |
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
| HIGH | ? | pixi.lock | 373 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1025 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1338 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 1823 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2175 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2255 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2606 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 2790 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3055 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3179 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3444 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3565 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 3838 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4193 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 4843 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 5155 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6161 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6395 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 6954 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 7316 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8589 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 8944 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9594 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 9905 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10409 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10483 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10543 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 10928 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11637 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 11978 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12309 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 12694 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13403 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 13744 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14075 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 14458 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15165 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 15505 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16067 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16153 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16227 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 16612 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17324 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 17666 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18222 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18305 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18378 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 18704 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19066 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19078 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19079 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19080 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19081 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19099 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19460 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19472 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19473 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19474 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19475 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19608 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19620 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19621 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19622 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19623 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19828 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19960 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19972 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19973 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19974 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 19975 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20180 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20310 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20321 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20322 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20323 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20324 | Match:       - conda: https://conda.anaconda.org/conda-forge |
| HIGH | ? | pixi.lock | 20675 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 20686 | Match:     - alsa-lib >=1.2.16.1,<1.3.0a0 |
| HIGH | ? | pixi.lock | 20733 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 20734 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20735 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20736 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20737 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20743 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 20751 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20752 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20753 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20754 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20755 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 20761 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 20769 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20776 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20784 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20792 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20806 | Match:     - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20818 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20825 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20831 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 20840 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20846 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 20854 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20855 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20856 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 20863 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 20873 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20874 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20875 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 20881 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20890 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20891 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20892 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20893 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 20899 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20907 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20908 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20909 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 20910 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20916 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20924 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 20925 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20927 | Match:   - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 20932 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20941 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 20942 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20943 | Match:   - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 20949 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20957 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 20958 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 20959 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 20965 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 20974 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20975 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20976 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20982 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 20992 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 20993 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 20994 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 20995 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 20996 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 20997 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 21003 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 21011 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 21012 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 21013 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21014 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 21015 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 21016 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 21023 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 21030 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21036 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 21045 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 21051 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 21058 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21064 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 21073 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 21079 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 21087 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 21088 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 21089 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21090 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 21091 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 21092 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 21093 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 21094 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 21095 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 21102 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 21112 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 21113 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 21114 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 21115 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 21116 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 21117 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 21118 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 21119 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 21120 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 21126 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 21134 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 21135 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 21136 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 21137 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 21157 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 21160 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 21161 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 21184 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21192 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21201 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 21209 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21210 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 21218 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 21226 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21237 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 21245 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 21246 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 21247 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 21255 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 21314 | Match:   - binutils_impl_linux-64 >=2.45.1,<2.45.2.0a0 |
| HIGH | ? | pixi.lock | 21960 | Match:   - gcc_impl_linux-64 >=14.3.0,<14.3.1.0a0 |
| HIGH | ? | pixi.lock | 23124 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 23301 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 23309 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 23310 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 23311 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 23312 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 23313 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 23314 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 23555 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 23732 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 23745 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 23748 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 23753 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 23776 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23778 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23779 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23780 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23781 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23792 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23796 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23816 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23818 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23819 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23820 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23821 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23832 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23836 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23856 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23858 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23859 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23860 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23861 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23872 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23876 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23896 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23898 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23899 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23900 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23901 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23912 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 23916 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 23937 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 23939 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 23940 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 23941 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 23942 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 23953 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 23957 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 24261 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24282 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24303 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24324 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 24345 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 24360 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 24768 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 25018 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 25041 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25065 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25146 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 25170 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25195 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25219 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25515 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 25544 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25566 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25619 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25637 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25655 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25673 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25691 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 25776 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 25794 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 25811 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 25961 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 26036 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 26045 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 26053 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 26063 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 26074 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 26647 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 26661 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 26677 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 26691 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 26705 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 27624 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 27635 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 27650 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 27658 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 27672 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 27680 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 28058 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 28080 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 28106 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 28128 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 28218 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 29497 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 29964 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 29978 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 30040 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 30125 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 30375 | Match:     - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 30390 | Match:     - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 31501 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 31573 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31589 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31607 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31623 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 31794 | Match: - conda: https://conda.anaconda.org/conda-forge/linux |
| HIGH | ? | pixi.lock | 31804 | Match:     - alsa-lib >=1.2.16.1,<1.3.0a0 |
| HIGH | ? | pixi.lock | 31849 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 31850 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 31851 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31852 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 31853 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31859 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 31866 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31867 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31868 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 31869 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31870 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 31876 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 31883 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31890 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31897 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 31905 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 31918 | Match:     - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 31930 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31937 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31943 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 31951 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 31957 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 31964 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 31965 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 31966 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 31973 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 31982 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 31983 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 31984 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 31990 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 31998 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 31999 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32000 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 32001 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 32007 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 32014 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32015 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32016 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 32017 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 32023 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 32030 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32031 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32033 | Match:   - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 32038 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 32046 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 32047 | Match:   - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 32048 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32054 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 32061 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32062 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 32063 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 32069 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 32077 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 32078 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32079 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 32085 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 32093 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 32095 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 32096 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 32097 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 32098 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32099 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 32105 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 32112 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 32113 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32114 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32115 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 32116 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 32117 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 32124 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 32131 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32137 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 32145 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32151 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 32158 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32164 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 32172 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32178 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 32185 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 32186 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32187 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32188 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 32189 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 32190 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 32191 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 32192 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 32193 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 32200 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 32209 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32210 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 32211 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 32212 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 32213 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32214 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 32215 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 32216 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 32217 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 32223 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 32230 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 32231 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 32232 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 32233 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 32252 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 32254 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 32255 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 32278 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32285 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32294 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 32301 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32302 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 32310 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 32317 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32328 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 32335 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 32336 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 32337 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 32345 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 32401 | Match:   - binutils_impl_linux-aarch64 >=2.45.1,<2.45.2.0a0 |
| HIGH | ? | pixi.lock | 32932 | Match:   - gcc_impl_linux-aarch64 >=14.3.0,<14.3.1.0a0 |
| HIGH | ? | pixi.lock | 34071 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 34245 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 34252 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 34253 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 34254 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 34255 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 34256 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 34257 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 34489 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 34665 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 34678 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 34681 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 34686 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 34708 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34710 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34711 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34712 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34713 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34724 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34728 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34747 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34749 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34750 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34751 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34752 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34763 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34767 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34786 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34788 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34789 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34790 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34791 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34802 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34806 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34825 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34827 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34828 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34829 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34830 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34841 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 34845 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 34864 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 34866 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 34867 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 34868 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 34869 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 34880 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 34884 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 35173 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35193 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35213 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35233 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 35253 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35268 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 35639 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 35880 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 35902 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 35925 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 36003 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 36026 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 36050 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 36073 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 36351 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 36379 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 36401 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 36452 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36469 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36486 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36503 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36520 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36600 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 36617 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 36633 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 36763 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 36855 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 36864 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 36871 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 36881 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 36891 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 37424 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 37438 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 37453 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 37467 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 37481 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 38378 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 38389 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 38401 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 38410 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 38421 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 38432 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 38804 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38830 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38854 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38873 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 38964 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 40184 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 40644 | Match:   - alsa-lib >=1.2.15.3,<1.3.0a0 |
| HIGH | ? | pixi.lock | 40658 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 40719 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 40793 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 41049 | Match:     - s2n >=1.4.17,<1.4.18.0a0 |
| HIGH | ? | pixi.lock | 41063 | Match:     - s2n >=1.7.5,<1.7.6.0a0 |
| HIGH | ? | pixi.lock | 42109 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 42178 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42194 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42212 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42228 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 42269 | Match:   - libadbc-driver-postgresql >=1.11.0,<1.11.1.0a0 |
| HIGH | ? | pixi.lock | 42286 | Match:   - libadbc-driver-postgresql >=1.2.0,<1.2.1.0a0 |
| HIGH | ? | pixi.lock | 42301 | Match:   - libadbc-driver-postgresql >=1.8.0,<1.8.1.0a0 |
| HIGH | ? | pixi.lock | 42316 | Match:   - libadbc-driver-sqlite >=1.11.0,<1.11.1.0a0 |
| HIGH | ? | pixi.lock | 42333 | Match:   - libadbc-driver-sqlite >=1.2.0,<1.2.1.0a0 |
| HIGH | ? | pixi.lock | 42348 | Match:   - libadbc-driver-sqlite >=1.3.0,<1.3.1.0a0 |
| HIGH | ? | pixi.lock | 43006 | Match:   - dask-core >=2026.7.0,<2026.7.1.0a0 |
| HIGH | ? | pixi.lock | 43007 | Match:   - distributed >=2026.7.0,<2026.7.1.0a0 |
| HIGH | ? | pixi.lock | 43085 | Match:   - dask-core >=2026.7.0,<2026.7.1.0a0 |
| HIGH | ? | pixi.lock | 43365 | Match:   - typing_extensions >=3.10.0.2 |
| HIGH | ? | pixi.lock | 43795 | Match:   - importlib-resources >=7.1.0,<7.1.1.0a0 |
| HIGH | ? | pixi.lock | 44956 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 45851 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46318 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46328 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46338 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46348 | Match: - conda: https://conda.anaconda.org/conda-forge/noarc |
| HIGH | ? | pixi.lock | 46897 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 46898 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 46899 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 46900 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 46901 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 46907 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 46915 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46916 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46917 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 46918 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 46919 | Match:   - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 46924 | Match:     - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46932 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46938 | Match:     - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 46946 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 46952 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 46964 | Match:     - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46977 | Match:     - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 46985 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 46990 | Match:     - aws-c-compression >=0.3.0,<0.3.1.0a0 |
| HIGH | ? | pixi.lock | 46998 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47004 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 47012 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47013 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47014 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47020 | Match:     - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 47029 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47030 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 47031 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47037 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 47045 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 47046 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 47047 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47048 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47054 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47062 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47063 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47064 | Match:   - aws-c-compression >=0.3.0,<0.3.1.0a0 |
| HIGH | ? | pixi.lock | 47065 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47070 | Match:     - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 47078 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47079 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47084 | Match:     - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47092 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 47093 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47099 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47107 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47108 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 47109 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47114 | Match:     - aws-c-mqtt >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47122 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47123 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47124 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47130 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 47138 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47139 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 47140 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47141 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 47142 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47143 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 47149 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 47157 | Match:   - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47158 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47159 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47160 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 47161 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47162 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47167 | Match:     - aws-c-s3 >=0.7.9,<0.7.10.0a0 |
| HIGH | ? | pixi.lock | 47175 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47180 | Match:     - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47188 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47194 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 47202 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47208 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 47216 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47221 | Match:     - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47229 | Match:   - aws-c-auth >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47230 | Match:   - aws-c-cal >=0.8.1,<0.8.2.0a0 |
| HIGH | ? | pixi.lock | 47231 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47232 | Match:   - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 47233 | Match:   - aws-c-http >=0.9.2,<0.9.3.0a0 |
| HIGH | ? | pixi.lock | 47234 | Match:   - aws-c-io >=0.15.3,<0.15.4.0a0 |
| HIGH | ? | pixi.lock | 47235 | Match:   - aws-c-mqtt >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47236 | Match:   - aws-c-s3 >=0.7.9,<0.7.10.0a0 |
| HIGH | ? | pixi.lock | 47237 | Match:   - aws-c-sdkutils >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47243 | Match:     - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 47252 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 47253 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 47254 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 47255 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47256 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 47257 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 47258 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 47259 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 47260 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 47266 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 47274 | Match:   - aws-c-common >=0.10.6,<0.10.7.0a0 |
| HIGH | ? | pixi.lock | 47275 | Match:   - aws-c-event-stream >=0.5.0,<0.5.1.0a0 |
| HIGH | ? | pixi.lock | 47276 | Match:   - aws-checksums >=0.2.2,<0.2.3.0a0 |
| HIGH | ? | pixi.lock | 47277 | Match:   - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 47296 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 47298 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 47299 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 47321 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47329 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47337 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 47345 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47346 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 47353 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 47361 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47371 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 47379 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 47380 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 47381 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 47388 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 49129 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 49137 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 49138 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 49139 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 49140 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 49141 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 49142 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 49341 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 49393 | Match:   - tapi >=1600.0.11.8,<1601.0a0 |
| HIGH | ? | pixi.lock | 49549 | Match:   - aws-crt-cpp >=0.29.9,<0.29.10.0a0 |
| HIGH | ? | pixi.lock | 49564 | Match:   - orc >=2.0.3,<2.0.4.0a0 |
| HIGH | ? | pixi.lock | 49585 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49587 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49588 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49589 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49590 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49601 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49604 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49624 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49626 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49627 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49628 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49629 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49640 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49643 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49663 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49665 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49666 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49667 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49668 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49679 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49682 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49702 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49704 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49705 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49706 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49707 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49718 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49721 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49742 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 49744 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 49745 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 49746 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 49747 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 49758 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 49761 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 49802 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49822 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49842 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49862 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 49882 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49902 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49924 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49946 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 49968 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 49990 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50033 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50055 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50077 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50099 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 50121 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50141 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50158 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50196 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50216 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50236 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50256 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50276 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 50296 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50310 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 50576 | Match:   - libcxx-headers >=19.1.7,<19.1.8.0a0 |
| HIGH | ? | pixi.lock | 50588 | Match:   - libcxx-headers >=21.1.8,<21.1.9.0a0 |
| HIGH | ? | pixi.lock | 50643 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 50765 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50787 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50810 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 50888 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 50911 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50935 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 50958 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51286 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 51304 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51326 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51377 | Match:   - libthrift >=0.21.0,<0.21.1.0a0 |
| HIGH | ? | pixi.lock | 51397 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51398 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51418 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51419 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51439 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51440 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51460 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51461 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51482 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51483 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51549 | Match:     - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 51566 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 51582 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 51690 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 51740 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 51747 | Match:     - libthrift >=0.21.0,<0.21.1.0a0 |
| HIGH | ? | pixi.lock | 51756 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 51764 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 51775 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 52276 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 52289 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 52303 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 52316 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 52329 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 53180 | Match:   - libprotobuf >=5.28.3,<5.28.4.0a0 |
| HIGH | ? | pixi.lock | 53190 | Match:     - orc >=2.0.3,<2.0.4.0a0 |
| HIGH | ? | pixi.lock | 53201 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 53211 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 53221 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 53233 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 53589 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 53610 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 53635 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 53652 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 54778 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 55788 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-6 |
| HIGH | ? | pixi.lock | 56124 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 56193 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56208 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56225 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56240 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 56450 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56451 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 56452 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56453 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56454 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 56460 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 56468 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56469 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56470 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56471 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56472 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 56477 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 56485 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56491 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56499 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56505 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56518 | Match:     - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56530 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56538 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56543 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 56551 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56557 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 56565 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56566 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56567 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56573 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 56582 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56583 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 56584 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 56590 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56598 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56599 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 56600 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56601 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 56607 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56615 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56616 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56617 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 56618 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56623 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56631 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56632 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56637 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56645 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56646 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56652 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 56660 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56661 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56662 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56667 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 56675 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 56676 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56677 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56683 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 56691 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 56692 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56693 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 56694 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 56695 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56696 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56702 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 56710 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 56711 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56712 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56713 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56714 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56715 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56720 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 56728 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56733 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 56741 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56747 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 56755 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56760 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56768 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56774 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 56782 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 56783 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56784 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56785 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 56786 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 56787 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 56788 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 56789 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 56790 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 56796 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56805 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 56806 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56807 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 56808 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 56809 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56810 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 56811 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 56812 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 56813 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 56819 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 56827 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 56828 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 56829 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 56830 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 56848 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 56849 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 56851 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 56874 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56882 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56890 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 56898 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56899 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 56906 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 56914 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56924 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 56932 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 56933 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 56934 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 56941 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 58752 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 58760 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 58761 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 58762 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 58763 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 58764 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 58765 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 58972 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 59037 | Match:   - tapi >=1600.0.11.8,<1601.0a0 |
| HIGH | ? | pixi.lock | 59193 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 59205 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 59207 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 59212 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 59234 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59236 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59237 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59238 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59239 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59250 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59253 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59273 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59275 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59276 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59277 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59278 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59289 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59292 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59312 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59314 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59315 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59316 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59317 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59328 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59331 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59351 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59353 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59354 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59355 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59356 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59367 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59370 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59391 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 59393 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 59394 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 59395 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 59396 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 59407 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59410 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 59436 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59456 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59476 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59496 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59517 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59536 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59558 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59580 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59602 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59625 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59650 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59672 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59694 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59716 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59739 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59759 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59779 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59799 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59819 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 59840 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 59853 | Match:   - libopenblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 60118 | Match:   - libcxx-headers >=19.1.7,<19.1.8.0a0 |
| HIGH | ? | pixi.lock | 60174 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 60296 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 60318 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60341 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60418 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 60441 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60465 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60488 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60814 | Match:   - openblas >=0.3.33,<0.3.34.0a0 |
| HIGH | ? | pixi.lock | 60832 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60855 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60908 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60909 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60929 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60930 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60950 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60951 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60971 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 60972 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 60992 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 60993 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 61060 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 61077 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 61093 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 61200 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 61235 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 61242 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 61251 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 61259 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 61270 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 61820 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 61833 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 61848 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 61861 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 61874 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 62754 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 62764 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 62777 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 62786 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 62797 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 62807 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 63165 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 63187 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 63218 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 63236 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 63325 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 64353 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 65373 | Match: - conda: https://conda.anaconda.org/conda-forge/osx-a |
| HIGH | ? | pixi.lock | 65726 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 65796 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 65812 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 65830 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 65846 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 66067 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66068 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66069 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66070 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 66071 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66077 | Match:     - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 66084 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66085 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66086 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66087 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66088 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 66096 | Match:     - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 66103 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66112 | Match:     - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66119 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66128 | Match:     - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66143 | Match:     - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66157 | Match:     - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66164 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66172 | Match:     - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 66182 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66188 | Match:     - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 66195 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66196 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66197 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 66205 | Match:     - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 66215 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66216 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66217 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 66223 | Match:     - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66233 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66234 | Match:   - aws-c-compression >=0.3.2,<0.3.3.0a0 |
| HIGH | ? | pixi.lock | 66235 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66236 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66242 | Match:     - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66249 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66250 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66251 | Match:   - aws-c-compression >=0.2.18,<0.2.19.0a0 |
| HIGH | ? | pixi.lock | 66252 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66260 | Match:     - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66267 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66268 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66276 | Match:     - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66286 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66287 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66293 | Match:     - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66300 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66301 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66302 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66310 | Match:     - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 66320 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66321 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66322 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66328 | Match:     - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 66338 | Match:   - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 66339 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66340 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 66341 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66342 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66343 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66349 | Match:     - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 66356 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 66357 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66358 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66359 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66360 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66361 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 66369 | Match:     - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 66376 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66384 | Match:     - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 66394 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66400 | Match:     - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 66407 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66415 | Match:     - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 66425 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66431 | Match:     - aws-checksums >=0.2.10,<0.2.11.0a0 |
| HIGH | ? | pixi.lock | 66438 | Match:   - aws-c-auth >=0.7.22,<0.7.23.0a0 |
| HIGH | ? | pixi.lock | 66439 | Match:   - aws-c-cal >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66440 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66441 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 66442 | Match:   - aws-c-http >=0.8.2,<0.8.3.0a0 |
| HIGH | ? | pixi.lock | 66443 | Match:   - aws-c-io >=0.14.10,<0.14.11.0a0 |
| HIGH | ? | pixi.lock | 66444 | Match:   - aws-c-mqtt >=0.10.4,<0.10.5.0a0 |
| HIGH | ? | pixi.lock | 66445 | Match:   - aws-c-s3 >=0.6.0,<0.6.1.0a0 |
| HIGH | ? | pixi.lock | 66446 | Match:   - aws-c-sdkutils >=0.1.16,<0.1.17.0a0 |
| HIGH | ? | pixi.lock | 66454 | Match:     - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66464 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 66465 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66466 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 66467 | Match:   - aws-c-cal >=0.9.14,<0.9.15.0a0 |
| HIGH | ? | pixi.lock | 66468 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 66469 | Match:   - aws-c-mqtt >=0.16.0,<0.16.1.0a0 |
| HIGH | ? | pixi.lock | 66470 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66471 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 66472 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 66478 | Match:     - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66485 | Match:   - aws-c-common >=0.9.23,<0.9.24.0a0 |
| HIGH | ? | pixi.lock | 66486 | Match:   - aws-c-event-stream >=0.4.2,<0.4.3.0a0 |
| HIGH | ? | pixi.lock | 66487 | Match:   - aws-checksums >=0.1.18,<0.1.19.0a0 |
| HIGH | ? | pixi.lock | 66488 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 66508 | Match:   - aws-c-event-stream >=0.7.1,<0.7.2.0a0 |
| HIGH | ? | pixi.lock | 66509 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 66510 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 66531 | Match:     - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66538 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66547 | Match:     - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 66554 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66555 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 66564 | Match:     - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66571 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66580 | Match:     - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 66587 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 66588 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 66589 | Match:   - azure-storage-common-cpp >=12.14.0,<12.14.1.0a0 |
| HIGH | ? | pixi.lock | 66598 | Match:     - azure-storage-files-datalake-cpp >=12.16.0,<12. |
| HIGH | ? | pixi.lock | 67141 | Match:   - gcc_impl_win-64 >=15.2.0,<15.2.1.0a0 |
| HIGH | ? | pixi.lock | 68197 | Match:     - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 68204 | Match:   - aws-c-auth >=0.10.3,<0.10.4.0a0 |
| HIGH | ? | pixi.lock | 68205 | Match:   - aws-c-common >=0.14.1,<0.14.2.0a0 |
| HIGH | ? | pixi.lock | 68206 | Match:   - aws-c-http >=0.11.0,<0.11.1.0a0 |
| HIGH | ? | pixi.lock | 68207 | Match:   - aws-c-io >=0.26.3,<0.26.4.0a0 |
| HIGH | ? | pixi.lock | 68208 | Match:   - aws-c-s3 >=0.12.6,<0.12.7.0a0 |
| HIGH | ? | pixi.lock | 68209 | Match:   - aws-c-sdkutils >=0.2.7,<0.2.8.0a0 |
| HIGH | ? | pixi.lock | 68399 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 68576 | Match:   - aws-crt-cpp >=0.27.3,<0.27.4.0a0 |
| HIGH | ? | pixi.lock | 68588 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 68590 | Match:   - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 68595 | Match:   - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 68619 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68621 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68622 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68623 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68624 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68634 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68637 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 68659 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68661 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68662 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68663 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68664 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68674 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68677 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 68699 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68701 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68702 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68703 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68704 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68714 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68717 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 68739 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68741 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68742 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68743 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68744 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68754 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 68757 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 68779 | Match:   - aws-crt-cpp >=0.40.1,<0.40.2.0a0 |
| HIGH | ? | pixi.lock | 68781 | Match:   - azure-core-cpp >=1.16.3,<1.16.4.0a0 |
| HIGH | ? | pixi.lock | 68782 | Match:   - azure-identity-cpp >=1.13.3,<1.13.4.0a0 |
| HIGH | ? | pixi.lock | 68783 | Match:   - azure-storage-blobs-cpp >=12.18.0,<12.18.1.0a0 |
| HIGH | ? | pixi.lock | 68784 | Match:   - azure-storage-files-datalake-cpp >=12.16.0,<12.16 |
| HIGH | ? | pixi.lock | 68794 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 68797 | Match:   - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 69103 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69124 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69145 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69166 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69188 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 69481 | Match:     - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 69601 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 69623 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69646 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 69724 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 69748 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69773 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 69797 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 69878 | Match:     - libhwloc >=2.13.0,<2.13.1.0a0 |
| HIGH | ? | pixi.lock | 70043 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 70065 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 70102 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 70120 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 70138 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 70156 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 70174 | Match:   - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 70249 | Match:     - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 70267 | Match:     - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 70284 | Match:     - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 70388 | Match:     - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 70439 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 70449 | Match:     - libthrift >=0.19.0,<0.19.1.0a0 |
| HIGH | ? | pixi.lock | 70456 | Match:   - libevent >=2.1.12,<2.1.13.0a0 |
| HIGH | ? | pixi.lock | 70467 | Match:     - libthrift >=0.22.0,<0.22.1.0a0 |
| HIGH | ? | pixi.lock | 70476 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 71065 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 71079 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 71095 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 71109 | Match:   - matplotlib-base >=3.11.0,<3.11.1.0a0 |
| HIGH | ? | pixi.lock | 71123 | Match:   - matplotlib-base >=3.9.3,<3.9.4.0a0 |
| HIGH | ? | pixi.lock | 71982 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 71995 | Match:     - orc >=2.0.1,<2.0.2.0a0 |
| HIGH | ? | pixi.lock | 72010 | Match:   - libprotobuf >=6.33.5,<6.33.6.0a0 |
| HIGH | ? | pixi.lock | 72018 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 72031 | Match:   - libprotobuf >=7.35.1,<7.35.2.0a0 |
| HIGH | ? | pixi.lock | 72040 | Match:     - orc >=2.3.0,<2.3.1.0a0 |
| HIGH | ? | pixi.lock | 72411 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72436 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72465 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72487 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 72580 | Match:   - libprotobuf >=4.25.3,<4.25.4.0a0 |
| HIGH | ? | pixi.lock | 73780 | Match:   - hdf5 >=1.14.4,<1.14.5.0a0 |
| HIGH | ? | pixi.lock | 74211 | Match:   - zeromq >=4.3.5,<4.3.6.0a0 |
| HIGH | ? | pixi.lock | 74306 | Match:   - libjpeg-turbo >=3.1.4.1,<4.0a0 |
| HIGH | ? | pixi.lock | 74859 | Match:   - libhwloc >=2.13.0,<2.13.1.0a0 |
| HIGH | ? | pixi.lock | 75325 | Match:   - libsodium >=1.0.22,<1.0.23.0a0 |
| HIGH | ? | pixi.lock | 75332 | Match:     - zeromq >=4.3.5,<4.3.6.0a0 |
| HIGH | ? | pixi.lock | 75401 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 75421 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 75443 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | pixi.lock | 75463 | Match:   - zstd >=1.5.7,<1.5.8.0a0 |
| HIGH | ? | eval.py | 25 | Match:         pd.eval("self.df + self.df2 + self.df3 + self |
| HIGH | ? | eval.py | 28 | Match:         pd.eval( |
| HIGH | ? | eval.py | 34 | Match:         pd.eval("self.df < self.df2 < self.df3 < self |
| HIGH | ? | eval.py | 37 | Match:         pd.eval("self.df * self.df2 * self.df3 * self |
| HIGH | ? | frame.py | 5249 | Match:         >>> df.eval("A + B") |
| HIGH | ? | frame.py | 5260 | Match:         >>> df.eval("D = A + B") |
| HIGH | ? | frame.py | 5277 | Match:         >>> df.eval( |
| HIGH | ? | frame.py | 5293 | Match:         >>> df.eval("B * `C&C`") |
| HIGH | ? | frame.py | 5305 | Match:         >>> df.eval("@local_var * A") |
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
| M | ? | np_datetime.pyx | 282 |
| M | ? | np_datetime.pyx | 318 |
| M | ? | parsing.pyx | 1097 |
| M | ? | timedeltas.pyx | 328 |
| M | ? | strptime.pyx | 269 |
| M | ? | np_datetime.pxd | 68 |
| M | ? | util.pxd | 41 |
| M | ? | util.pxd | 48 |
| M | ? | util.pxd | 118 |
| M | ? | util.pxd | 122 |
| M | ? | period.pyx | 1107 |
| M | ? | tzconversion.pyx | 475 |
| M | ? | parsers.pyx | 325 |
| M | ? | groupby.pyx | 1621 |
| M | ? | hashtable_class_helper.pxi.in | 235 |
| M | ? | hashtable_class_helper.pxi.in | 309 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| L | ? | managers.py | 1332 |
| L | ? | masked.py | 937 |
| L | ? | array.py | 1296 |
| L | ? | merge.py | 1610 |
| L | ? | datetimes.py | 1221 |
| L | ? | groupby.py | 1579 |
| L | ? | hashtable.pyi | 165 |
| L | ? | hashtable.pyi | 167 |
| L | ? | numba.pyi | 22 |
| M | ? | indexing.py | 130 |
| M | ? | indexing.py | 135 |
| M | ? | indexing_engines.py | 89 |
| M | ? | indexing_engines.py | 147 |
| M | ? | gil.py | 60 |
| M | ? | gil.py | 63 |
| M | ? | index_cached_properties.py | 50 |
| M | ? | orc.py | 242 |
| M | ? | orc.py | 256 |
| M | ? | common.py | 136 |
| M | ? | common.py | 422 |
| M | ? | common.py | 882 |
| M | ? | common.py | 888 |
| M | ? | common.py | 929 |
| M | ? | common.py | 988 |
| M | ? | common.py | 1172 |
| M | ? | common.py | 1338 |
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
| M | ? | readers.py | 349 |
| M | ? | readers.py | 701 |
| M | ? | readers.py | 762 |
| M | ? | c_parser_wrapper.py | 133 |
| M | ? | c_parser_wrapper.py | 171 |
| M | ? | c_parser_wrapper.py | 190 |
| M | ? | c_parser_wrapper.py | 225 |
| M | ? | c_parser_wrapper.py | 309 |
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
| M | ? | _odswriter.py | 118 |
| M | ? | _base.py | 840 |
| M | ? | _base.py | 851 |
| M | ? | _base.py | 858 |
| M | ? | _base.py | 881 |
| M | ? | _base.py | 886 |
| M | ? | _base.py | 913 |
| M | ? | _base.py | 1209 |
| M | ? | _base.py | 1491 |
| M | ? | _base.py | 1650 |
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
| M | ? | sas7bdat.py | 340 |
| M | ? | sas7bdat.py | 355 |
| M | ? | sas7bdat.py | 375 |
| M | ? | _exceptions.py | 55 |
| M | ? | _exceptions.py | 56 |
| M | ? | _print_versions.py | 141 |
| M | ? | _print_versions.py | 146 |
| M | ? | config.py | 405 |
| M | ? | config.py | 756 |
| M | ? | _optional.py | 148 |
| M | ? | asserters.py | 839 |
| M | ? | asserters.py | 840 |
| M | ? | asserters.py | 888 |
| M | ? | asserters.py | 896 |
| M | ? | asserters.py | 1070 |
| M | ? | asserters.py | 1093 |
| M | ? | asserters.py | 1370 |
| M | ? | asserters.py | 1380 |
| M | ? | asserters.py | 1418 |
| M | ? | asserters.py | 1419 |
| M | ? | asserters.py | 1476 |
| M | ? | asserters.py | 1494 |
| M | ? | asserters.py | 1495 |
| M | ? | asserters.py | 1497 |
| M | ? | asserters.py | 1515 |
| M | ? | asserters.py | 1516 |
| M | ? | asserters.py | 1536 |
| M | ? | asserters.py | 1554 |
| M | ? | asserters.py | 1596 |
| M | ? | asserters.py | 1598 |
| M | ? | _warnings.py | 267 |
| M | ? | construction.py | 395 |
| M | ? | indexing.py | 977 |
| M | ? | indexing.py | 986 |
| M | ? | indexing.py | 987 |
| M | ? | indexing.py | 1126 |
| M | ? | indexing.py | 2596 |
| M | ? | indexing.py | 3324 |
| M | ? | rolling.py | 3561 |
| M | ? | objects.py | 190 |
| M | ? | objects.py | 615 |
| M | ? | sample.py | 109 |
| M | ? | sample.py | 158 |
| M | ? | hashing.py | 79 |
| M | ? | missing.py | 260 |
| M | ? | extension.py | 175 |
| M | ? | base.py | 667 |
| M | ? | base.py | 745 |
| M | ? | base.py | 3888 |
| M | ? | base.py | 4703 |
| M | ? | base.py | 4875 |
| M | ? | base.py | 4953 |
| M | ? | base.py | 5052 |
| M | ? | base.py | 5053 |
| M | ? | base.py | 5119 |
| M | ? | base.py | 7240 |
| M | ? | period.py | 553 |
| M | ? | datetimes.py | 99 |
| M | ? | timedeltas.py | 306 |
| M | ? | timedeltas.py | 349 |
| M | ? | range.py | 251 |
| M | ? | range.py | 1089 |
| M | ? | multi.py | 1606 |
| M | ? | multi.py | 1681 |
| M | ? | datetimelike.py | 1360 |
| M | ? | datetimelike.py | 1369 |
| M | ? | datetimelike.py | 1370 |
| M | ? | datetimelike.py | 1406 |
| M | ? | from_dataframe.py | 331 |
| M | ? | from_dataframe.py | 335 |
| M | ? | from_dataframe.py | 513 |
| M | ? | sorting.py | 505 |
| M | ? | nanops.py | 368 |
| M | ? | nanops.py | 435 |
| M | ? | nanops.py | 446 |
| M | ? | nanops.py | 1796 |
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
| M | ? | algorithms.py | 1153 |
| M | ? | quantile.py | 85 |
| M | ? | quantile.py | 93 |
| M | ? | quantile.py | 203 |
| M | ? | take.py | 193 |
| M | ? | take.py | 194 |
| M | ? | take.py | 195 |
| M | ? | series.py | 1251 |
| M | ? | series.py | 4681 |
| M | ? | series.py | 4735 |
| M | ? | series.py | 7295 |
| M | ? | series.py | 7296 |
| M | ? | generic.py | 533 |
| M | ? | generic.py | 5761 |
| M | ? | generic.py | 6097 |
| M | ? | generic.py | 10822 |
| M | ? | generic.py | 10853 |
| M | ? | generic.py | 11733 |
| M | ? | generic.py | 11844 |
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
| M | ? | blocks.py | 2079 |
| M | ? | blocks.py | 2086 |
| M | ? | blocks.py | 2438 |
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
| M | ? | masked.py | 1501 |
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
| M | ? | timedeltas.py | 1205 |
| M | ? | timedeltas.py | 1286 |
| M | ? | timedeltas.py | 1287 |
| M | ? | string_.py | 767 |
| M | ? | string_arrow.py | 172 |
| M | ? | string_arrow.py | 237 |
| M | ? | array.py | 2109 |
| M | ? | interval.py | 1695 |
| M | ? | interval.py | 1699 |
| M | ? | interval.py | 1729 |
| M | ? | interval.py | 1733 |
| M | ? | interval.py | 1876 |
| M | ? | interval.py | 1880 |
| M | ? | interval.py | 1885 |
| M | ? | boolean.py | 390 |
| M | ? | boolean.py | 394 |
| M | ? | datetimelike.py | 1076 |
| M | ? | datetimelike.py | 1297 |
| M | ? | datetimelike.py | 1313 |
| M | ? | datetimelike.py | 1690 |
| M | ? | _mixins.py | 191 |
| M | ? | numeric.py | 212 |
| M | ? | categorical.py | 1642 |
| M | ? | categorical.py | 1994 |
| M | ? | categorical.py | 2371 |
| M | ? | categorical.py | 2597 |
| M | ? | categorical.py | 2880 |
| M | ? | array.py | 507 |
| M | ? | array.py | 2112 |
| M | ? | array.py | 2124 |
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
| M | ? | common.py | 120 |
| M | ? | common.py | 284 |
| M | ? | dtypes.py | 2447 |
| M | ? | cast.py | 999 |
| M | ? | cast.py | 1038 |
| M | ? | cast.py | 1055 |
| M | ? | cast.py | 1525 |
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
| M | ? | generic.py | 478 |
| M | ? | generic.py | 588 |
| M | ? | generic.py | 788 |
| M | ? | generic.py | 2800 |
| M | ? | generic.py | 4252 |
| M | ? | groupby.py | 840 |
| M | ? | groupby.py | 1497 |
| M | ? | groupby.py | 1507 |
| M | ? | groupby.py | 1588 |
| M | ? | groupby.py | 1750 |
| M | ? | groupby.py | 1975 |
| M | ? | groupby.py | 1976 |
| M | ? | groupby.py | 5699 |
| M | ? | groupby.py | 5747 |
| M | ? | groupby.py | 5790 |
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
| H | ? | _odswriter.py | 92 |
| H | ? | _openpyxl.py | 109 |
| H | ? | format.py | 1028 |
| M | ? | pickle.py | 240 |
| M | ? | pickle_compat.py | 139 |
| C | ? | sql.py | 26 |
| C | ? | sql.py | 75 |
| C | ? | sql.py | 2269 |
| C | ? | sql.py | 2271 |
| C | ? | sql.py | 2483 |
| C | ? | sql.py | 2633 |
| H | ? | algorithms.py | 896 |
| H | ? | style_render.py | 1203 |
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
| H | ? | pixi.lock | 373 |
| H | ? | pixi.lock | 1025 |
| H | ? | pixi.lock | 1338 |
| H | ? | pixi.lock | 1823 |
| H | ? | pixi.lock | 2175 |
| H | ? | pixi.lock | 2255 |
| H | ? | pixi.lock | 2606 |
| H | ? | pixi.lock | 2790 |
| H | ? | pixi.lock | 3055 |
| H | ? | pixi.lock | 3179 |
| H | ? | pixi.lock | 3444 |
| H | ? | pixi.lock | 3565 |
| H | ? | pixi.lock | 3838 |
| H | ? | pixi.lock | 4193 |
| H | ? | pixi.lock | 4843 |
| H | ? | pixi.lock | 5155 |
| H | ? | pixi.lock | 6161 |
| H | ? | pixi.lock | 6395 |
| H | ? | pixi.lock | 6954 |
| H | ? | pixi.lock | 7316 |
| H | ? | pixi.lock | 8589 |
| H | ? | pixi.lock | 8944 |
| H | ? | pixi.lock | 9594 |
| H | ? | pixi.lock | 9905 |
| H | ? | pixi.lock | 10409 |
| H | ? | pixi.lock | 10483 |
| H | ? | pixi.lock | 10543 |
| H | ? | pixi.lock | 10928 |
| H | ? | pixi.lock | 11637 |
| H | ? | pixi.lock | 11978 |
| H | ? | pixi.lock | 12309 |
| H | ? | pixi.lock | 12694 |
| H | ? | pixi.lock | 13403 |
| H | ? | pixi.lock | 13744 |
| H | ? | pixi.lock | 14075 |
| H | ? | pixi.lock | 14458 |
| H | ? | pixi.lock | 15165 |
| H | ? | pixi.lock | 15505 |
| H | ? | pixi.lock | 16067 |
| H | ? | pixi.lock | 16153 |
| H | ? | pixi.lock | 16227 |
| H | ? | pixi.lock | 16612 |
| H | ? | pixi.lock | 17324 |
| H | ? | pixi.lock | 17666 |
| H | ? | pixi.lock | 18222 |
| H | ? | pixi.lock | 18305 |
| H | ? | pixi.lock | 18378 |
| H | ? | pixi.lock | 18704 |
| H | ? | pixi.lock | 19066 |
| H | ? | pixi.lock | 19078 |
| H | ? | pixi.lock | 19079 |
| H | ? | pixi.lock | 19080 |
| H | ? | pixi.lock | 19081 |
| H | ? | pixi.lock | 19099 |
| H | ? | pixi.lock | 19460 |
| H | ? | pixi.lock | 19472 |
| H | ? | pixi.lock | 19473 |
| H | ? | pixi.lock | 19474 |
| H | ? | pixi.lock | 19475 |
| H | ? | pixi.lock | 19608 |
| H | ? | pixi.lock | 19620 |
| H | ? | pixi.lock | 19621 |
| H | ? | pixi.lock | 19622 |
| H | ? | pixi.lock | 19623 |
| H | ? | pixi.lock | 19828 |
| H | ? | pixi.lock | 19960 |
| H | ? | pixi.lock | 19972 |
| H | ? | pixi.lock | 19973 |
| H | ? | pixi.lock | 19974 |
| H | ? | pixi.lock | 19975 |
| H | ? | pixi.lock | 20180 |
| H | ? | pixi.lock | 20310 |
| H | ? | pixi.lock | 20321 |
| H | ? | pixi.lock | 20322 |
| H | ? | pixi.lock | 20323 |
| H | ? | pixi.lock | 20324 |
| H | ? | pixi.lock | 20675 |
| H | ? | pixi.lock | 20686 |
| H | ? | pixi.lock | 20733 |
| H | ? | pixi.lock | 20734 |
| H | ? | pixi.lock | 20735 |
| H | ? | pixi.lock | 20736 |
| H | ? | pixi.lock | 20737 |
| H | ? | pixi.lock | 20743 |
| H | ? | pixi.lock | 20751 |
| H | ? | pixi.lock | 20752 |
| H | ? | pixi.lock | 20753 |
| H | ? | pixi.lock | 20754 |
| H | ? | pixi.lock | 20755 |
| H | ? | pixi.lock | 20761 |
| H | ? | pixi.lock | 20769 |
| H | ? | pixi.lock | 20776 |
| H | ? | pixi.lock | 20784 |
| H | ? | pixi.lock | 20792 |
| H | ? | pixi.lock | 20806 |
| H | ? | pixi.lock | 20818 |
| H | ? | pixi.lock | 20825 |
| H | ? | pixi.lock | 20831 |
| H | ? | pixi.lock | 20840 |
| H | ? | pixi.lock | 20846 |
| H | ? | pixi.lock | 20854 |
| H | ? | pixi.lock | 20855 |
| H | ? | pixi.lock | 20856 |
| H | ? | pixi.lock | 20863 |
| H | ? | pixi.lock | 20873 |
| H | ? | pixi.lock | 20874 |
| H | ? | pixi.lock | 20875 |
| H | ? | pixi.lock | 20881 |
| H | ? | pixi.lock | 20890 |
| H | ? | pixi.lock | 20891 |
| H | ? | pixi.lock | 20892 |
| H | ? | pixi.lock | 20893 |
| H | ? | pixi.lock | 20899 |
| H | ? | pixi.lock | 20907 |
| H | ? | pixi.lock | 20908 |
| H | ? | pixi.lock | 20909 |
| H | ? | pixi.lock | 20910 |
| H | ? | pixi.lock | 20916 |
| H | ? | pixi.lock | 20924 |
| H | ? | pixi.lock | 20925 |
| H | ? | pixi.lock | 20927 |
| H | ? | pixi.lock | 20932 |
| H | ? | pixi.lock | 20941 |
| H | ? | pixi.lock | 20942 |
| H | ? | pixi.lock | 20943 |
| H | ? | pixi.lock | 20949 |
| H | ? | pixi.lock | 20957 |
| H | ? | pixi.lock | 20958 |
| H | ? | pixi.lock | 20959 |
| H | ? | pixi.lock | 20965 |
| H | ? | pixi.lock | 20974 |
| H | ? | pixi.lock | 20975 |
| H | ? | pixi.lock | 20976 |
| H | ? | pixi.lock | 20982 |
| H | ? | pixi.lock | 20992 |
| H | ? | pixi.lock | 20993 |
| H | ? | pixi.lock | 20994 |
| H | ? | pixi.lock | 20995 |
| H | ? | pixi.lock | 20996 |
| H | ? | pixi.lock | 20997 |
| H | ? | pixi.lock | 21003 |
| H | ? | pixi.lock | 21011 |
| H | ? | pixi.lock | 21012 |
| H | ? | pixi.lock | 21013 |
| H | ? | pixi.lock | 21014 |
| H | ? | pixi.lock | 21015 |
| H | ? | pixi.lock | 21016 |
| H | ? | pixi.lock | 21023 |
| H | ? | pixi.lock | 21030 |
| H | ? | pixi.lock | 21036 |
| H | ? | pixi.lock | 21045 |
| H | ? | pixi.lock | 21051 |
| H | ? | pixi.lock | 21058 |
| H | ? | pixi.lock | 21064 |
| H | ? | pixi.lock | 21073 |
| H | ? | pixi.lock | 21079 |
| H | ? | pixi.lock | 21087 |
| H | ? | pixi.lock | 21088 |
| H | ? | pixi.lock | 21089 |
| H | ? | pixi.lock | 21090 |
| H | ? | pixi.lock | 21091 |
| H | ? | pixi.lock | 21092 |
| H | ? | pixi.lock | 21093 |
| H | ? | pixi.lock | 21094 |
| H | ? | pixi.lock | 21095 |
| H | ? | pixi.lock | 21102 |
| H | ? | pixi.lock | 21112 |
| H | ? | pixi.lock | 21113 |
| H | ? | pixi.lock | 21114 |
| H | ? | pixi.lock | 21115 |
| H | ? | pixi.lock | 21116 |
| H | ? | pixi.lock | 21117 |
| H | ? | pixi.lock | 21118 |
| H | ? | pixi.lock | 21119 |
| H | ? | pixi.lock | 21120 |
| H | ? | pixi.lock | 21126 |
| H | ? | pixi.lock | 21134 |
| H | ? | pixi.lock | 21135 |
| H | ? | pixi.lock | 21136 |
| H | ? | pixi.lock | 21137 |
| H | ? | pixi.lock | 21157 |
| H | ? | pixi.lock | 21160 |
| H | ? | pixi.lock | 21161 |
| H | ? | pixi.lock | 21184 |
| H | ? | pixi.lock | 21192 |
| H | ? | pixi.lock | 21201 |
| H | ? | pixi.lock | 21209 |
| H | ? | pixi.lock | 21210 |
| H | ? | pixi.lock | 21218 |
| H | ? | pixi.lock | 21226 |
| H | ? | pixi.lock | 21237 |
| H | ? | pixi.lock | 21245 |
| H | ? | pixi.lock | 21246 |
| H | ? | pixi.lock | 21247 |
| H | ? | pixi.lock | 21255 |
| H | ? | pixi.lock | 21314 |
| H | ? | pixi.lock | 21960 |
| H | ? | pixi.lock | 23124 |
| H | ? | pixi.lock | 23301 |
| H | ? | pixi.lock | 23309 |
| H | ? | pixi.lock | 23310 |
| H | ? | pixi.lock | 23311 |
| H | ? | pixi.lock | 23312 |
| H | ? | pixi.lock | 23313 |
| H | ? | pixi.lock | 23314 |
| H | ? | pixi.lock | 23555 |
| H | ? | pixi.lock | 23732 |
| H | ? | pixi.lock | 23745 |
| H | ? | pixi.lock | 23748 |
| H | ? | pixi.lock | 23753 |
| H | ? | pixi.lock | 23776 |
| H | ? | pixi.lock | 23778 |
| H | ? | pixi.lock | 23779 |
| H | ? | pixi.lock | 23780 |
| H | ? | pixi.lock | 23781 |
| H | ? | pixi.lock | 23792 |
| H | ? | pixi.lock | 23796 |
| H | ? | pixi.lock | 23816 |
| H | ? | pixi.lock | 23818 |
| H | ? | pixi.lock | 23819 |
| H | ? | pixi.lock | 23820 |
| H | ? | pixi.lock | 23821 |
| H | ? | pixi.lock | 23832 |
| H | ? | pixi.lock | 23836 |
| H | ? | pixi.lock | 23856 |
| H | ? | pixi.lock | 23858 |
| H | ? | pixi.lock | 23859 |
| H | ? | pixi.lock | 23860 |
| H | ? | pixi.lock | 23861 |
| H | ? | pixi.lock | 23872 |
| H | ? | pixi.lock | 23876 |
| H | ? | pixi.lock | 23896 |
| H | ? | pixi.lock | 23898 |
| H | ? | pixi.lock | 23899 |
| H | ? | pixi.lock | 23900 |
| H | ? | pixi.lock | 23901 |
| H | ? | pixi.lock | 23912 |
| H | ? | pixi.lock | 23916 |
| H | ? | pixi.lock | 23937 |
| H | ? | pixi.lock | 23939 |
| H | ? | pixi.lock | 23940 |
| H | ? | pixi.lock | 23941 |
| H | ? | pixi.lock | 23942 |
| H | ? | pixi.lock | 23953 |
| H | ? | pixi.lock | 23957 |
| H | ? | pixi.lock | 24261 |
| H | ? | pixi.lock | 24282 |
| H | ? | pixi.lock | 24303 |
| H | ? | pixi.lock | 24324 |
| H | ? | pixi.lock | 24345 |
| H | ? | pixi.lock | 24360 |
| H | ? | pixi.lock | 24768 |
| H | ? | pixi.lock | 25018 |
| H | ? | pixi.lock | 25041 |
| H | ? | pixi.lock | 25065 |
| H | ? | pixi.lock | 25146 |
| H | ? | pixi.lock | 25170 |
| H | ? | pixi.lock | 25195 |
| H | ? | pixi.lock | 25219 |
| H | ? | pixi.lock | 25515 |
| H | ? | pixi.lock | 25544 |
| H | ? | pixi.lock | 25566 |
| H | ? | pixi.lock | 25619 |
| H | ? | pixi.lock | 25637 |
| H | ? | pixi.lock | 25655 |
| H | ? | pixi.lock | 25673 |
| H | ? | pixi.lock | 25691 |
| H | ? | pixi.lock | 25776 |
| H | ? | pixi.lock | 25794 |
| H | ? | pixi.lock | 25811 |
| H | ? | pixi.lock | 25961 |
| H | ? | pixi.lock | 26036 |
| H | ? | pixi.lock | 26045 |
| H | ? | pixi.lock | 26053 |
| H | ? | pixi.lock | 26063 |
| H | ? | pixi.lock | 26074 |
| H | ? | pixi.lock | 26647 |
| H | ? | pixi.lock | 26661 |
| H | ? | pixi.lock | 26677 |
| H | ? | pixi.lock | 26691 |
| H | ? | pixi.lock | 26705 |
| H | ? | pixi.lock | 27624 |
| H | ? | pixi.lock | 27635 |
| H | ? | pixi.lock | 27650 |
| H | ? | pixi.lock | 27658 |
| H | ? | pixi.lock | 27672 |
| H | ? | pixi.lock | 27680 |
| H | ? | pixi.lock | 28058 |
| H | ? | pixi.lock | 28080 |
| H | ? | pixi.lock | 28106 |
| H | ? | pixi.lock | 28128 |
| H | ? | pixi.lock | 28218 |
| H | ? | pixi.lock | 29497 |
| H | ? | pixi.lock | 29964 |
| H | ? | pixi.lock | 29978 |
| H | ? | pixi.lock | 30040 |
| H | ? | pixi.lock | 30125 |
| H | ? | pixi.lock | 30375 |
| H | ? | pixi.lock | 30390 |
| H | ? | pixi.lock | 31501 |
| H | ? | pixi.lock | 31573 |
| H | ? | pixi.lock | 31589 |
| H | ? | pixi.lock | 31607 |
| H | ? | pixi.lock | 31623 |
| H | ? | pixi.lock | 31794 |
| H | ? | pixi.lock | 31804 |
| H | ? | pixi.lock | 31849 |
| H | ? | pixi.lock | 31850 |
| H | ? | pixi.lock | 31851 |
| H | ? | pixi.lock | 31852 |
| H | ? | pixi.lock | 31853 |
| H | ? | pixi.lock | 31859 |
| H | ? | pixi.lock | 31866 |
| H | ? | pixi.lock | 31867 |
| H | ? | pixi.lock | 31868 |
| H | ? | pixi.lock | 31869 |
| H | ? | pixi.lock | 31870 |
| H | ? | pixi.lock | 31876 |
| H | ? | pixi.lock | 31883 |
| H | ? | pixi.lock | 31890 |
| H | ? | pixi.lock | 31897 |
| H | ? | pixi.lock | 31905 |
| H | ? | pixi.lock | 31918 |
| H | ? | pixi.lock | 31930 |
| H | ? | pixi.lock | 31937 |
| H | ? | pixi.lock | 31943 |
| H | ? | pixi.lock | 31951 |
| H | ? | pixi.lock | 31957 |
| H | ? | pixi.lock | 31964 |
| H | ? | pixi.lock | 31965 |
| H | ? | pixi.lock | 31966 |
| H | ? | pixi.lock | 31973 |
| H | ? | pixi.lock | 31982 |
| H | ? | pixi.lock | 31983 |
| H | ? | pixi.lock | 31984 |
| H | ? | pixi.lock | 31990 |
| H | ? | pixi.lock | 31998 |
| H | ? | pixi.lock | 31999 |
| H | ? | pixi.lock | 32000 |
| H | ? | pixi.lock | 32001 |
| H | ? | pixi.lock | 32007 |
| H | ? | pixi.lock | 32014 |
| H | ? | pixi.lock | 32015 |
| H | ? | pixi.lock | 32016 |
| H | ? | pixi.lock | 32017 |
| H | ? | pixi.lock | 32023 |
| H | ? | pixi.lock | 32030 |
| H | ? | pixi.lock | 32031 |
| H | ? | pixi.lock | 32033 |
| H | ? | pixi.lock | 32038 |
| H | ? | pixi.lock | 32046 |
| H | ? | pixi.lock | 32047 |
| H | ? | pixi.lock | 32048 |
| H | ? | pixi.lock | 32054 |
| H | ? | pixi.lock | 32061 |
| H | ? | pixi.lock | 32062 |
| H | ? | pixi.lock | 32063 |
| H | ? | pixi.lock | 32069 |
| H | ? | pixi.lock | 32077 |
| H | ? | pixi.lock | 32078 |
| H | ? | pixi.lock | 32079 |
| H | ? | pixi.lock | 32085 |
| H | ? | pixi.lock | 32093 |
| H | ? | pixi.lock | 32095 |
| H | ? | pixi.lock | 32096 |
| H | ? | pixi.lock | 32097 |
| H | ? | pixi.lock | 32098 |
| H | ? | pixi.lock | 32099 |
| H | ? | pixi.lock | 32105 |
| H | ? | pixi.lock | 32112 |
| H | ? | pixi.lock | 32113 |
| H | ? | pixi.lock | 32114 |
| H | ? | pixi.lock | 32115 |
| H | ? | pixi.lock | 32116 |
| H | ? | pixi.lock | 32117 |
| H | ? | pixi.lock | 32124 |
| H | ? | pixi.lock | 32131 |
| H | ? | pixi.lock | 32137 |
| H | ? | pixi.lock | 32145 |
| H | ? | pixi.lock | 32151 |
| H | ? | pixi.lock | 32158 |
| H | ? | pixi.lock | 32164 |
| H | ? | pixi.lock | 32172 |
| H | ? | pixi.lock | 32178 |
| H | ? | pixi.lock | 32185 |
| H | ? | pixi.lock | 32186 |
| H | ? | pixi.lock | 32187 |
| H | ? | pixi.lock | 32188 |
| H | ? | pixi.lock | 32189 |
| H | ? | pixi.lock | 32190 |
| H | ? | pixi.lock | 32191 |
| H | ? | pixi.lock | 32192 |
| H | ? | pixi.lock | 32193 |
| H | ? | pixi.lock | 32200 |
| H | ? | pixi.lock | 32209 |
| H | ? | pixi.lock | 32210 |
| H | ? | pixi.lock | 32211 |
| H | ? | pixi.lock | 32212 |
| H | ? | pixi.lock | 32213 |
| H | ? | pixi.lock | 32214 |
| H | ? | pixi.lock | 32215 |
| H | ? | pixi.lock | 32216 |
| H | ? | pixi.lock | 32217 |
| H | ? | pixi.lock | 32223 |
| H | ? | pixi.lock | 32230 |
| H | ? | pixi.lock | 32231 |
| H | ? | pixi.lock | 32232 |
| H | ? | pixi.lock | 32233 |
| H | ? | pixi.lock | 32252 |
| H | ? | pixi.lock | 32254 |
| H | ? | pixi.lock | 32255 |
| H | ? | pixi.lock | 32278 |
| H | ? | pixi.lock | 32285 |
| H | ? | pixi.lock | 32294 |
| H | ? | pixi.lock | 32301 |
| H | ? | pixi.lock | 32302 |
| H | ? | pixi.lock | 32310 |
| H | ? | pixi.lock | 32317 |
| H | ? | pixi.lock | 32328 |
| H | ? | pixi.lock | 32335 |
| H | ? | pixi.lock | 32336 |
| H | ? | pixi.lock | 32337 |
| H | ? | pixi.lock | 32345 |
| H | ? | pixi.lock | 32401 |
| H | ? | pixi.lock | 32932 |
| H | ? | pixi.lock | 34071 |
| H | ? | pixi.lock | 34245 |
| H | ? | pixi.lock | 34252 |
| H | ? | pixi.lock | 34253 |
| H | ? | pixi.lock | 34254 |
| H | ? | pixi.lock | 34255 |
| H | ? | pixi.lock | 34256 |
| H | ? | pixi.lock | 34257 |
| H | ? | pixi.lock | 34489 |
| H | ? | pixi.lock | 34665 |
| H | ? | pixi.lock | 34678 |
| H | ? | pixi.lock | 34681 |
| H | ? | pixi.lock | 34686 |
| H | ? | pixi.lock | 34708 |
| H | ? | pixi.lock | 34710 |
| H | ? | pixi.lock | 34711 |
| H | ? | pixi.lock | 34712 |
| H | ? | pixi.lock | 34713 |
| H | ? | pixi.lock | 34724 |
| H | ? | pixi.lock | 34728 |
| H | ? | pixi.lock | 34747 |
| H | ? | pixi.lock | 34749 |
| H | ? | pixi.lock | 34750 |
| H | ? | pixi.lock | 34751 |
| H | ? | pixi.lock | 34752 |
| H | ? | pixi.lock | 34763 |
| H | ? | pixi.lock | 34767 |
| H | ? | pixi.lock | 34786 |
| H | ? | pixi.lock | 34788 |
| H | ? | pixi.lock | 34789 |
| H | ? | pixi.lock | 34790 |
| H | ? | pixi.lock | 34791 |
| H | ? | pixi.lock | 34802 |
| H | ? | pixi.lock | 34806 |
| H | ? | pixi.lock | 34825 |
| H | ? | pixi.lock | 34827 |
| H | ? | pixi.lock | 34828 |
| H | ? | pixi.lock | 34829 |
| H | ? | pixi.lock | 34830 |
| H | ? | pixi.lock | 34841 |
| H | ? | pixi.lock | 34845 |
| H | ? | pixi.lock | 34864 |
| H | ? | pixi.lock | 34866 |
| H | ? | pixi.lock | 34867 |
| H | ? | pixi.lock | 34868 |
| H | ? | pixi.lock | 34869 |
| H | ? | pixi.lock | 34880 |
| H | ? | pixi.lock | 34884 |
| H | ? | pixi.lock | 35173 |
| H | ? | pixi.lock | 35193 |
| H | ? | pixi.lock | 35213 |
| H | ? | pixi.lock | 35233 |
| H | ? | pixi.lock | 35253 |
| H | ? | pixi.lock | 35268 |
| H | ? | pixi.lock | 35639 |
| H | ? | pixi.lock | 35880 |
| H | ? | pixi.lock | 35902 |
| H | ? | pixi.lock | 35925 |
| H | ? | pixi.lock | 36003 |
| H | ? | pixi.lock | 36026 |
| H | ? | pixi.lock | 36050 |
| H | ? | pixi.lock | 36073 |
| H | ? | pixi.lock | 36351 |
| H | ? | pixi.lock | 36379 |
| H | ? | pixi.lock | 36401 |
| H | ? | pixi.lock | 36452 |
| H | ? | pixi.lock | 36469 |
| H | ? | pixi.lock | 36486 |
| H | ? | pixi.lock | 36503 |
| H | ? | pixi.lock | 36520 |
| H | ? | pixi.lock | 36600 |
| H | ? | pixi.lock | 36617 |
| H | ? | pixi.lock | 36633 |
| H | ? | pixi.lock | 36763 |
| H | ? | pixi.lock | 36855 |
| H | ? | pixi.lock | 36864 |
| H | ? | pixi.lock | 36871 |
| H | ? | pixi.lock | 36881 |
| H | ? | pixi.lock | 36891 |
| H | ? | pixi.lock | 37424 |
| H | ? | pixi.lock | 37438 |
| H | ? | pixi.lock | 37453 |
| H | ? | pixi.lock | 37467 |
| H | ? | pixi.lock | 37481 |
| H | ? | pixi.lock | 38378 |
| H | ? | pixi.lock | 38389 |
| H | ? | pixi.lock | 38401 |
| H | ? | pixi.lock | 38410 |
| H | ? | pixi.lock | 38421 |
| H | ? | pixi.lock | 38432 |
| H | ? | pixi.lock | 38804 |
| H | ? | pixi.lock | 38830 |
| H | ? | pixi.lock | 38854 |
| H | ? | pixi.lock | 38873 |
| H | ? | pixi.lock | 38964 |
| H | ? | pixi.lock | 40184 |
| H | ? | pixi.lock | 40644 |
| H | ? | pixi.lock | 40658 |
| H | ? | pixi.lock | 40719 |
| H | ? | pixi.lock | 40793 |
| H | ? | pixi.lock | 41049 |
| H | ? | pixi.lock | 41063 |
| H | ? | pixi.lock | 42109 |
| H | ? | pixi.lock | 42178 |
| H | ? | pixi.lock | 42194 |
| H | ? | pixi.lock | 42212 |
| H | ? | pixi.lock | 42228 |
| H | ? | pixi.lock | 42269 |
| H | ? | pixi.lock | 42286 |
| H | ? | pixi.lock | 42301 |
| H | ? | pixi.lock | 42316 |
| H | ? | pixi.lock | 42333 |
| H | ? | pixi.lock | 42348 |
| H | ? | pixi.lock | 43006 |
| H | ? | pixi.lock | 43007 |
| H | ? | pixi.lock | 43085 |
| H | ? | pixi.lock | 43365 |
| H | ? | pixi.lock | 43795 |
| H | ? | pixi.lock | 44956 |
| H | ? | pixi.lock | 45851 |
| H | ? | pixi.lock | 46318 |
| H | ? | pixi.lock | 46328 |
| H | ? | pixi.lock | 46338 |
| H | ? | pixi.lock | 46348 |
| H | ? | pixi.lock | 46897 |
| H | ? | pixi.lock | 46898 |
| H | ? | pixi.lock | 46899 |
| H | ? | pixi.lock | 46900 |
| H | ? | pixi.lock | 46901 |
| H | ? | pixi.lock | 46907 |
| H | ? | pixi.lock | 46915 |
| H | ? | pixi.lock | 46916 |
| H | ? | pixi.lock | 46917 |
| H | ? | pixi.lock | 46918 |
| H | ? | pixi.lock | 46919 |
| H | ? | pixi.lock | 46924 |
| H | ? | pixi.lock | 46932 |
| H | ? | pixi.lock | 46938 |
| H | ? | pixi.lock | 46946 |
| H | ? | pixi.lock | 46952 |
| H | ? | pixi.lock | 46964 |
| H | ? | pixi.lock | 46977 |
| H | ? | pixi.lock | 46985 |
| H | ? | pixi.lock | 46990 |
| H | ? | pixi.lock | 46998 |
| H | ? | pixi.lock | 47004 |
| H | ? | pixi.lock | 47012 |
| H | ? | pixi.lock | 47013 |
| H | ? | pixi.lock | 47014 |
| H | ? | pixi.lock | 47020 |
| H | ? | pixi.lock | 47029 |
| H | ? | pixi.lock | 47030 |
| H | ? | pixi.lock | 47031 |
| H | ? | pixi.lock | 47037 |
| H | ? | pixi.lock | 47045 |
| H | ? | pixi.lock | 47046 |
| H | ? | pixi.lock | 47047 |
| H | ? | pixi.lock | 47048 |
| H | ? | pixi.lock | 47054 |
| H | ? | pixi.lock | 47062 |
| H | ? | pixi.lock | 47063 |
| H | ? | pixi.lock | 47064 |
| H | ? | pixi.lock | 47065 |
| H | ? | pixi.lock | 47070 |
| H | ? | pixi.lock | 47078 |
| H | ? | pixi.lock | 47079 |
| H | ? | pixi.lock | 47084 |
| H | ? | pixi.lock | 47092 |
| H | ? | pixi.lock | 47093 |
| H | ? | pixi.lock | 47099 |
| H | ? | pixi.lock | 47107 |
| H | ? | pixi.lock | 47108 |
| H | ? | pixi.lock | 47109 |
| H | ? | pixi.lock | 47114 |
| H | ? | pixi.lock | 47122 |
| H | ? | pixi.lock | 47123 |
| H | ? | pixi.lock | 47124 |
| H | ? | pixi.lock | 47130 |
| H | ? | pixi.lock | 47138 |
| H | ? | pixi.lock | 47139 |
| H | ? | pixi.lock | 47140 |
| H | ? | pixi.lock | 47141 |
| H | ? | pixi.lock | 47142 |
| H | ? | pixi.lock | 47143 |
| H | ? | pixi.lock | 47149 |
| H | ? | pixi.lock | 47157 |
| H | ? | pixi.lock | 47158 |
| H | ? | pixi.lock | 47159 |
| H | ? | pixi.lock | 47160 |
| H | ? | pixi.lock | 47161 |
| H | ? | pixi.lock | 47162 |
| H | ? | pixi.lock | 47167 |
| H | ? | pixi.lock | 47175 |
| H | ? | pixi.lock | 47180 |
| H | ? | pixi.lock | 47188 |
| H | ? | pixi.lock | 47194 |
| H | ? | pixi.lock | 47202 |
| H | ? | pixi.lock | 47208 |
| H | ? | pixi.lock | 47216 |
| H | ? | pixi.lock | 47221 |
| H | ? | pixi.lock | 47229 |
| H | ? | pixi.lock | 47230 |
| H | ? | pixi.lock | 47231 |
| H | ? | pixi.lock | 47232 |
| H | ? | pixi.lock | 47233 |
| H | ? | pixi.lock | 47234 |
| H | ? | pixi.lock | 47235 |
| H | ? | pixi.lock | 47236 |
| H | ? | pixi.lock | 47237 |
| H | ? | pixi.lock | 47243 |
| H | ? | pixi.lock | 47252 |
| H | ? | pixi.lock | 47253 |
| H | ? | pixi.lock | 47254 |
| H | ? | pixi.lock | 47255 |
| H | ? | pixi.lock | 47256 |
| H | ? | pixi.lock | 47257 |
| H | ? | pixi.lock | 47258 |
| H | ? | pixi.lock | 47259 |
| H | ? | pixi.lock | 47260 |
| H | ? | pixi.lock | 47266 |
| H | ? | pixi.lock | 47274 |
| H | ? | pixi.lock | 47275 |
| H | ? | pixi.lock | 47276 |
| H | ? | pixi.lock | 47277 |
| H | ? | pixi.lock | 47296 |
| H | ? | pixi.lock | 47298 |
| H | ? | pixi.lock | 47299 |
| H | ? | pixi.lock | 47321 |
| H | ? | pixi.lock | 47329 |
| H | ? | pixi.lock | 47337 |
| H | ? | pixi.lock | 47345 |
| H | ? | pixi.lock | 47346 |
| H | ? | pixi.lock | 47353 |
| H | ? | pixi.lock | 47361 |
| H | ? | pixi.lock | 47371 |
| H | ? | pixi.lock | 47379 |
| H | ? | pixi.lock | 47380 |
| H | ? | pixi.lock | 47381 |
| H | ? | pixi.lock | 47388 |
| H | ? | pixi.lock | 49129 |
| H | ? | pixi.lock | 49137 |
| H | ? | pixi.lock | 49138 |
| H | ? | pixi.lock | 49139 |
| H | ? | pixi.lock | 49140 |
| H | ? | pixi.lock | 49141 |
| H | ? | pixi.lock | 49142 |
| H | ? | pixi.lock | 49341 |
| H | ? | pixi.lock | 49393 |
| H | ? | pixi.lock | 49549 |
| H | ? | pixi.lock | 49564 |
| H | ? | pixi.lock | 49585 |
| H | ? | pixi.lock | 49587 |
| H | ? | pixi.lock | 49588 |
| H | ? | pixi.lock | 49589 |
| H | ? | pixi.lock | 49590 |
| H | ? | pixi.lock | 49601 |
| H | ? | pixi.lock | 49604 |
| H | ? | pixi.lock | 49624 |
| H | ? | pixi.lock | 49626 |
| H | ? | pixi.lock | 49627 |
| H | ? | pixi.lock | 49628 |
| H | ? | pixi.lock | 49629 |
| H | ? | pixi.lock | 49640 |
| H | ? | pixi.lock | 49643 |
| H | ? | pixi.lock | 49663 |
| H | ? | pixi.lock | 49665 |
| H | ? | pixi.lock | 49666 |
| H | ? | pixi.lock | 49667 |
| H | ? | pixi.lock | 49668 |
| H | ? | pixi.lock | 49679 |
| H | ? | pixi.lock | 49682 |
| H | ? | pixi.lock | 49702 |
| H | ? | pixi.lock | 49704 |
| H | ? | pixi.lock | 49705 |
| H | ? | pixi.lock | 49706 |
| H | ? | pixi.lock | 49707 |
| H | ? | pixi.lock | 49718 |
| H | ? | pixi.lock | 49721 |
| H | ? | pixi.lock | 49742 |
| H | ? | pixi.lock | 49744 |
| H | ? | pixi.lock | 49745 |
| H | ? | pixi.lock | 49746 |
| H | ? | pixi.lock | 49747 |
| H | ? | pixi.lock | 49758 |
| H | ? | pixi.lock | 49761 |
| H | ? | pixi.lock | 49802 |
| H | ? | pixi.lock | 49822 |
| H | ? | pixi.lock | 49842 |
| H | ? | pixi.lock | 49862 |
| H | ? | pixi.lock | 49882 |
| H | ? | pixi.lock | 49902 |
| H | ? | pixi.lock | 49924 |
| H | ? | pixi.lock | 49946 |
| H | ? | pixi.lock | 49968 |
| H | ? | pixi.lock | 49990 |
| H | ? | pixi.lock | 50033 |
| H | ? | pixi.lock | 50055 |
| H | ? | pixi.lock | 50077 |
| H | ? | pixi.lock | 50099 |
| H | ? | pixi.lock | 50121 |
| H | ? | pixi.lock | 50141 |
| H | ? | pixi.lock | 50158 |
| H | ? | pixi.lock | 50196 |
| H | ? | pixi.lock | 50216 |
| H | ? | pixi.lock | 50236 |
| H | ? | pixi.lock | 50256 |
| H | ? | pixi.lock | 50276 |
| H | ? | pixi.lock | 50296 |
| H | ? | pixi.lock | 50310 |
| H | ? | pixi.lock | 50576 |
| H | ? | pixi.lock | 50588 |
| H | ? | pixi.lock | 50643 |
| H | ? | pixi.lock | 50765 |
| H | ? | pixi.lock | 50787 |
| H | ? | pixi.lock | 50810 |
| H | ? | pixi.lock | 50888 |
| H | ? | pixi.lock | 50911 |
| H | ? | pixi.lock | 50935 |
| H | ? | pixi.lock | 50958 |
| H | ? | pixi.lock | 51286 |
| H | ? | pixi.lock | 51304 |
| H | ? | pixi.lock | 51326 |
| H | ? | pixi.lock | 51377 |
| H | ? | pixi.lock | 51397 |
| H | ? | pixi.lock | 51398 |
| H | ? | pixi.lock | 51418 |
| H | ? | pixi.lock | 51419 |
| H | ? | pixi.lock | 51439 |
| H | ? | pixi.lock | 51440 |
| H | ? | pixi.lock | 51460 |
| H | ? | pixi.lock | 51461 |
| H | ? | pixi.lock | 51482 |
| H | ? | pixi.lock | 51483 |
| H | ? | pixi.lock | 51549 |
| H | ? | pixi.lock | 51566 |
| H | ? | pixi.lock | 51582 |
| H | ? | pixi.lock | 51690 |
| H | ? | pixi.lock | 51740 |
| H | ? | pixi.lock | 51747 |
| H | ? | pixi.lock | 51756 |
| H | ? | pixi.lock | 51764 |
| H | ? | pixi.lock | 51775 |
| H | ? | pixi.lock | 52276 |
| H | ? | pixi.lock | 52289 |
| H | ? | pixi.lock | 52303 |
| H | ? | pixi.lock | 52316 |
| H | ? | pixi.lock | 52329 |
| H | ? | pixi.lock | 53180 |
| H | ? | pixi.lock | 53190 |
| H | ? | pixi.lock | 53201 |
| H | ? | pixi.lock | 53211 |
| H | ? | pixi.lock | 53221 |
| H | ? | pixi.lock | 53233 |
| H | ? | pixi.lock | 53589 |
| H | ? | pixi.lock | 53610 |
| H | ? | pixi.lock | 53635 |
| H | ? | pixi.lock | 53652 |
| H | ? | pixi.lock | 54778 |
| H | ? | pixi.lock | 55788 |
| H | ? | pixi.lock | 56124 |
| H | ? | pixi.lock | 56193 |
| H | ? | pixi.lock | 56208 |
| H | ? | pixi.lock | 56225 |
| H | ? | pixi.lock | 56240 |
| H | ? | pixi.lock | 56450 |
| H | ? | pixi.lock | 56451 |
| H | ? | pixi.lock | 56452 |
| H | ? | pixi.lock | 56453 |
| H | ? | pixi.lock | 56454 |
| H | ? | pixi.lock | 56460 |
| H | ? | pixi.lock | 56468 |
| H | ? | pixi.lock | 56469 |
| H | ? | pixi.lock | 56470 |
| H | ? | pixi.lock | 56471 |
| H | ? | pixi.lock | 56472 |
| H | ? | pixi.lock | 56477 |
| H | ? | pixi.lock | 56485 |
| H | ? | pixi.lock | 56491 |
| H | ? | pixi.lock | 56499 |
| H | ? | pixi.lock | 56505 |
| H | ? | pixi.lock | 56518 |
| H | ? | pixi.lock | 56530 |
| H | ? | pixi.lock | 56538 |
| H | ? | pixi.lock | 56543 |
| H | ? | pixi.lock | 56551 |
| H | ? | pixi.lock | 56557 |
| H | ? | pixi.lock | 56565 |
| H | ? | pixi.lock | 56566 |
| H | ? | pixi.lock | 56567 |
| H | ? | pixi.lock | 56573 |
| H | ? | pixi.lock | 56582 |
| H | ? | pixi.lock | 56583 |
| H | ? | pixi.lock | 56584 |
| H | ? | pixi.lock | 56590 |
| H | ? | pixi.lock | 56598 |
| H | ? | pixi.lock | 56599 |
| H | ? | pixi.lock | 56600 |
| H | ? | pixi.lock | 56601 |
| H | ? | pixi.lock | 56607 |
| H | ? | pixi.lock | 56615 |
| H | ? | pixi.lock | 56616 |
| H | ? | pixi.lock | 56617 |
| H | ? | pixi.lock | 56618 |
| H | ? | pixi.lock | 56623 |
| H | ? | pixi.lock | 56631 |
| H | ? | pixi.lock | 56632 |
| H | ? | pixi.lock | 56637 |
| H | ? | pixi.lock | 56645 |
| H | ? | pixi.lock | 56646 |
| H | ? | pixi.lock | 56652 |
| H | ? | pixi.lock | 56660 |
| H | ? | pixi.lock | 56661 |
| H | ? | pixi.lock | 56662 |
| H | ? | pixi.lock | 56667 |
| H | ? | pixi.lock | 56675 |
| H | ? | pixi.lock | 56676 |
| H | ? | pixi.lock | 56677 |
| H | ? | pixi.lock | 56683 |
| H | ? | pixi.lock | 56691 |
| H | ? | pixi.lock | 56692 |
| H | ? | pixi.lock | 56693 |
| H | ? | pixi.lock | 56694 |
| H | ? | pixi.lock | 56695 |
| H | ? | pixi.lock | 56696 |
| H | ? | pixi.lock | 56702 |
| H | ? | pixi.lock | 56710 |
| H | ? | pixi.lock | 56711 |
| H | ? | pixi.lock | 56712 |
| H | ? | pixi.lock | 56713 |
| H | ? | pixi.lock | 56714 |
| H | ? | pixi.lock | 56715 |
| H | ? | pixi.lock | 56720 |
| H | ? | pixi.lock | 56728 |
| H | ? | pixi.lock | 56733 |
| H | ? | pixi.lock | 56741 |
| H | ? | pixi.lock | 56747 |
| H | ? | pixi.lock | 56755 |
| H | ? | pixi.lock | 56760 |
| H | ? | pixi.lock | 56768 |
| H | ? | pixi.lock | 56774 |
| H | ? | pixi.lock | 56782 |
| H | ? | pixi.lock | 56783 |
| H | ? | pixi.lock | 56784 |
| H | ? | pixi.lock | 56785 |
| H | ? | pixi.lock | 56786 |
| H | ? | pixi.lock | 56787 |
| H | ? | pixi.lock | 56788 |
| H | ? | pixi.lock | 56789 |
| H | ? | pixi.lock | 56790 |
| H | ? | pixi.lock | 56796 |
| H | ? | pixi.lock | 56805 |
| H | ? | pixi.lock | 56806 |
| H | ? | pixi.lock | 56807 |
| H | ? | pixi.lock | 56808 |
| H | ? | pixi.lock | 56809 |
| H | ? | pixi.lock | 56810 |
| H | ? | pixi.lock | 56811 |
| H | ? | pixi.lock | 56812 |
| H | ? | pixi.lock | 56813 |
| H | ? | pixi.lock | 56819 |
| H | ? | pixi.lock | 56827 |
| H | ? | pixi.lock | 56828 |
| H | ? | pixi.lock | 56829 |
| H | ? | pixi.lock | 56830 |
| H | ? | pixi.lock | 56848 |
| H | ? | pixi.lock | 56849 |
| H | ? | pixi.lock | 56851 |
| H | ? | pixi.lock | 56874 |
| H | ? | pixi.lock | 56882 |
| H | ? | pixi.lock | 56890 |
| H | ? | pixi.lock | 56898 |
| H | ? | pixi.lock | 56899 |
| H | ? | pixi.lock | 56906 |
| H | ? | pixi.lock | 56914 |
| H | ? | pixi.lock | 56924 |
| H | ? | pixi.lock | 56932 |
| H | ? | pixi.lock | 56933 |
| H | ? | pixi.lock | 56934 |
| H | ? | pixi.lock | 56941 |
| H | ? | pixi.lock | 58752 |
| H | ? | pixi.lock | 58760 |
| H | ? | pixi.lock | 58761 |
| H | ? | pixi.lock | 58762 |
| H | ? | pixi.lock | 58763 |
| H | ? | pixi.lock | 58764 |
| H | ? | pixi.lock | 58765 |
| H | ? | pixi.lock | 58972 |
| H | ? | pixi.lock | 59037 |
| H | ? | pixi.lock | 59193 |
| H | ? | pixi.lock | 59205 |
| H | ? | pixi.lock | 59207 |
| H | ? | pixi.lock | 59212 |
| H | ? | pixi.lock | 59234 |
| H | ? | pixi.lock | 59236 |
| H | ? | pixi.lock | 59237 |
| H | ? | pixi.lock | 59238 |
| H | ? | pixi.lock | 59239 |
| H | ? | pixi.lock | 59250 |
| H | ? | pixi.lock | 59253 |
| H | ? | pixi.lock | 59273 |
| H | ? | pixi.lock | 59275 |
| H | ? | pixi.lock | 59276 |
| H | ? | pixi.lock | 59277 |
| H | ? | pixi.lock | 59278 |
| H | ? | pixi.lock | 59289 |
| H | ? | pixi.lock | 59292 |
| H | ? | pixi.lock | 59312 |
| H | ? | pixi.lock | 59314 |
| H | ? | pixi.lock | 59315 |
| H | ? | pixi.lock | 59316 |
| H | ? | pixi.lock | 59317 |
| H | ? | pixi.lock | 59328 |
| H | ? | pixi.lock | 59331 |
| H | ? | pixi.lock | 59351 |
| H | ? | pixi.lock | 59353 |
| H | ? | pixi.lock | 59354 |
| H | ? | pixi.lock | 59355 |
| H | ? | pixi.lock | 59356 |
| H | ? | pixi.lock | 59367 |
| H | ? | pixi.lock | 59370 |
| H | ? | pixi.lock | 59391 |
| H | ? | pixi.lock | 59393 |
| H | ? | pixi.lock | 59394 |
| H | ? | pixi.lock | 59395 |
| H | ? | pixi.lock | 59396 |
| H | ? | pixi.lock | 59407 |
| H | ? | pixi.lock | 59410 |
| H | ? | pixi.lock | 59436 |
| H | ? | pixi.lock | 59456 |
| H | ? | pixi.lock | 59476 |
| H | ? | pixi.lock | 59496 |
| H | ? | pixi.lock | 59517 |
| H | ? | pixi.lock | 59536 |
| H | ? | pixi.lock | 59558 |
| H | ? | pixi.lock | 59580 |
| H | ? | pixi.lock | 59602 |
| H | ? | pixi.lock | 59625 |
| H | ? | pixi.lock | 59650 |
| H | ? | pixi.lock | 59672 |
| H | ? | pixi.lock | 59694 |
| H | ? | pixi.lock | 59716 |
| H | ? | pixi.lock | 59739 |
| H | ? | pixi.lock | 59759 |
| H | ? | pixi.lock | 59779 |
| H | ? | pixi.lock | 59799 |
| H | ? | pixi.lock | 59819 |
| H | ? | pixi.lock | 59840 |
| H | ? | pixi.lock | 59853 |
| H | ? | pixi.lock | 60118 |
| H | ? | pixi.lock | 60174 |
| H | ? | pixi.lock | 60296 |
| H | ? | pixi.lock | 60318 |
| H | ? | pixi.lock | 60341 |
| H | ? | pixi.lock | 60418 |
| H | ? | pixi.lock | 60441 |
| H | ? | pixi.lock | 60465 |
| H | ? | pixi.lock | 60488 |
| H | ? | pixi.lock | 60814 |
| H | ? | pixi.lock | 60832 |
| H | ? | pixi.lock | 60855 |
| H | ? | pixi.lock | 60908 |
| H | ? | pixi.lock | 60909 |
| H | ? | pixi.lock | 60929 |
| H | ? | pixi.lock | 60930 |
| H | ? | pixi.lock | 60950 |
| H | ? | pixi.lock | 60951 |
| H | ? | pixi.lock | 60971 |
| H | ? | pixi.lock | 60972 |
| H | ? | pixi.lock | 60992 |
| H | ? | pixi.lock | 60993 |
| H | ? | pixi.lock | 61060 |
| H | ? | pixi.lock | 61077 |
| H | ? | pixi.lock | 61093 |
| H | ? | pixi.lock | 61200 |
| H | ? | pixi.lock | 61235 |
| H | ? | pixi.lock | 61242 |
| H | ? | pixi.lock | 61251 |
| H | ? | pixi.lock | 61259 |
| H | ? | pixi.lock | 61270 |
| H | ? | pixi.lock | 61820 |
| H | ? | pixi.lock | 61833 |
| H | ? | pixi.lock | 61848 |
| H | ? | pixi.lock | 61861 |
| H | ? | pixi.lock | 61874 |
| H | ? | pixi.lock | 62754 |
| H | ? | pixi.lock | 62764 |
| H | ? | pixi.lock | 62777 |
| H | ? | pixi.lock | 62786 |
| H | ? | pixi.lock | 62797 |
| H | ? | pixi.lock | 62807 |
| H | ? | pixi.lock | 63165 |
| H | ? | pixi.lock | 63187 |
| H | ? | pixi.lock | 63218 |
| H | ? | pixi.lock | 63236 |
| H | ? | pixi.lock | 63325 |
| H | ? | pixi.lock | 64353 |
| H | ? | pixi.lock | 65373 |
| H | ? | pixi.lock | 65726 |
| H | ? | pixi.lock | 65796 |
| H | ? | pixi.lock | 65812 |
| H | ? | pixi.lock | 65830 |
| H | ? | pixi.lock | 65846 |
| H | ? | pixi.lock | 66067 |
| H | ? | pixi.lock | 66068 |
| H | ? | pixi.lock | 66069 |
| H | ? | pixi.lock | 66070 |
| H | ? | pixi.lock | 66071 |
| H | ? | pixi.lock | 66077 |
| H | ? | pixi.lock | 66084 |
| H | ? | pixi.lock | 66085 |
| H | ? | pixi.lock | 66086 |
| H | ? | pixi.lock | 66087 |
| H | ? | pixi.lock | 66088 |
| H | ? | pixi.lock | 66096 |
| H | ? | pixi.lock | 66103 |
| H | ? | pixi.lock | 66112 |
| H | ? | pixi.lock | 66119 |
| H | ? | pixi.lock | 66128 |
| H | ? | pixi.lock | 66143 |
| H | ? | pixi.lock | 66157 |
| H | ? | pixi.lock | 66164 |
| H | ? | pixi.lock | 66172 |
| H | ? | pixi.lock | 66182 |
| H | ? | pixi.lock | 66188 |
| H | ? | pixi.lock | 66195 |
| H | ? | pixi.lock | 66196 |
| H | ? | pixi.lock | 66197 |
| H | ? | pixi.lock | 66205 |
| H | ? | pixi.lock | 66215 |
| H | ? | pixi.lock | 66216 |
| H | ? | pixi.lock | 66217 |
| H | ? | pixi.lock | 66223 |
| H | ? | pixi.lock | 66233 |
| H | ? | pixi.lock | 66234 |
| H | ? | pixi.lock | 66235 |
| H | ? | pixi.lock | 66236 |
| H | ? | pixi.lock | 66242 |
| H | ? | pixi.lock | 66249 |
| H | ? | pixi.lock | 66250 |
| H | ? | pixi.lock | 66251 |
| H | ? | pixi.lock | 66252 |
| H | ? | pixi.lock | 66260 |
| H | ? | pixi.lock | 66267 |
| H | ? | pixi.lock | 66268 |
| H | ? | pixi.lock | 66276 |
| H | ? | pixi.lock | 66286 |
| H | ? | pixi.lock | 66287 |
| H | ? | pixi.lock | 66293 |
| H | ? | pixi.lock | 66300 |
| H | ? | pixi.lock | 66301 |
| H | ? | pixi.lock | 66302 |
| H | ? | pixi.lock | 66310 |
| H | ? | pixi.lock | 66320 |
| H | ? | pixi.lock | 66321 |
| H | ? | pixi.lock | 66322 |
| H | ? | pixi.lock | 66328 |
| H | ? | pixi.lock | 66338 |
| H | ? | pixi.lock | 66339 |
| H | ? | pixi.lock | 66340 |
| H | ? | pixi.lock | 66341 |
| H | ? | pixi.lock | 66342 |
| H | ? | pixi.lock | 66343 |
| H | ? | pixi.lock | 66349 |
| H | ? | pixi.lock | 66356 |
| H | ? | pixi.lock | 66357 |
| H | ? | pixi.lock | 66358 |
| H | ? | pixi.lock | 66359 |
| H | ? | pixi.lock | 66360 |
| H | ? | pixi.lock | 66361 |
| H | ? | pixi.lock | 66369 |
| H | ? | pixi.lock | 66376 |
| H | ? | pixi.lock | 66384 |
| H | ? | pixi.lock | 66394 |
| H | ? | pixi.lock | 66400 |
| H | ? | pixi.lock | 66407 |
| H | ? | pixi.lock | 66415 |
| H | ? | pixi.lock | 66425 |
| H | ? | pixi.lock | 66431 |
| H | ? | pixi.lock | 66438 |
| H | ? | pixi.lock | 66439 |
| H | ? | pixi.lock | 66440 |
| H | ? | pixi.lock | 66441 |
| H | ? | pixi.lock | 66442 |
| H | ? | pixi.lock | 66443 |
| H | ? | pixi.lock | 66444 |
| H | ? | pixi.lock | 66445 |
| H | ? | pixi.lock | 66446 |
| H | ? | pixi.lock | 66454 |
| H | ? | pixi.lock | 66464 |
| H | ? | pixi.lock | 66465 |
| H | ? | pixi.lock | 66466 |
| H | ? | pixi.lock | 66467 |
| H | ? | pixi.lock | 66468 |
| H | ? | pixi.lock | 66469 |
| H | ? | pixi.lock | 66470 |
| H | ? | pixi.lock | 66471 |
| H | ? | pixi.lock | 66472 |
| H | ? | pixi.lock | 66478 |
| H | ? | pixi.lock | 66485 |
| H | ? | pixi.lock | 66486 |
| H | ? | pixi.lock | 66487 |
| H | ? | pixi.lock | 66488 |
| H | ? | pixi.lock | 66508 |
| H | ? | pixi.lock | 66509 |
| H | ? | pixi.lock | 66510 |
| H | ? | pixi.lock | 66531 |
| H | ? | pixi.lock | 66538 |
| H | ? | pixi.lock | 66547 |
| H | ? | pixi.lock | 66554 |
| H | ? | pixi.lock | 66555 |
| H | ? | pixi.lock | 66564 |
| H | ? | pixi.lock | 66571 |
| H | ? | pixi.lock | 66580 |
| H | ? | pixi.lock | 66587 |
| H | ? | pixi.lock | 66588 |
| H | ? | pixi.lock | 66589 |
| H | ? | pixi.lock | 66598 |
| H | ? | pixi.lock | 67141 |
| H | ? | pixi.lock | 68197 |
| H | ? | pixi.lock | 68204 |
| H | ? | pixi.lock | 68205 |
| H | ? | pixi.lock | 68206 |
| H | ? | pixi.lock | 68207 |
| H | ? | pixi.lock | 68208 |
| H | ? | pixi.lock | 68209 |
| H | ? | pixi.lock | 68399 |
| H | ? | pixi.lock | 68576 |
| H | ? | pixi.lock | 68588 |
| H | ? | pixi.lock | 68590 |
| H | ? | pixi.lock | 68595 |
| H | ? | pixi.lock | 68619 |
| H | ? | pixi.lock | 68621 |
| H | ? | pixi.lock | 68622 |
| H | ? | pixi.lock | 68623 |
| H | ? | pixi.lock | 68624 |
| H | ? | pixi.lock | 68634 |
| H | ? | pixi.lock | 68637 |
| H | ? | pixi.lock | 68659 |
| H | ? | pixi.lock | 68661 |
| H | ? | pixi.lock | 68662 |
| H | ? | pixi.lock | 68663 |
| H | ? | pixi.lock | 68664 |
| H | ? | pixi.lock | 68674 |
| H | ? | pixi.lock | 68677 |
| H | ? | pixi.lock | 68699 |
| H | ? | pixi.lock | 68701 |
| H | ? | pixi.lock | 68702 |
| H | ? | pixi.lock | 68703 |
| H | ? | pixi.lock | 68704 |
| H | ? | pixi.lock | 68714 |
| H | ? | pixi.lock | 68717 |
| H | ? | pixi.lock | 68739 |
| H | ? | pixi.lock | 68741 |
| H | ? | pixi.lock | 68742 |
| H | ? | pixi.lock | 68743 |
| H | ? | pixi.lock | 68744 |
| H | ? | pixi.lock | 68754 |
| H | ? | pixi.lock | 68757 |
| H | ? | pixi.lock | 68779 |
| H | ? | pixi.lock | 68781 |
| H | ? | pixi.lock | 68782 |
| H | ? | pixi.lock | 68783 |
| H | ? | pixi.lock | 68784 |
| H | ? | pixi.lock | 68794 |
| H | ? | pixi.lock | 68797 |
| H | ? | pixi.lock | 69103 |
| H | ? | pixi.lock | 69124 |
| H | ? | pixi.lock | 69145 |
| H | ? | pixi.lock | 69166 |
| H | ? | pixi.lock | 69188 |
| H | ? | pixi.lock | 69481 |
| H | ? | pixi.lock | 69601 |
| H | ? | pixi.lock | 69623 |
| H | ? | pixi.lock | 69646 |
| H | ? | pixi.lock | 69724 |
| H | ? | pixi.lock | 69748 |
| H | ? | pixi.lock | 69773 |
| H | ? | pixi.lock | 69797 |
| H | ? | pixi.lock | 69878 |
| H | ? | pixi.lock | 70043 |
| H | ? | pixi.lock | 70065 |
| H | ? | pixi.lock | 70102 |
| H | ? | pixi.lock | 70120 |
| H | ? | pixi.lock | 70138 |
| H | ? | pixi.lock | 70156 |
| H | ? | pixi.lock | 70174 |
| H | ? | pixi.lock | 70249 |
| H | ? | pixi.lock | 70267 |
| H | ? | pixi.lock | 70284 |
| H | ? | pixi.lock | 70388 |
| H | ? | pixi.lock | 70439 |
| H | ? | pixi.lock | 70449 |
| H | ? | pixi.lock | 70456 |
| H | ? | pixi.lock | 70467 |
| H | ? | pixi.lock | 70476 |
| H | ? | pixi.lock | 71065 |
| H | ? | pixi.lock | 71079 |
| H | ? | pixi.lock | 71095 |
| H | ? | pixi.lock | 71109 |
| H | ? | pixi.lock | 71123 |
| H | ? | pixi.lock | 71982 |
| H | ? | pixi.lock | 71995 |
| H | ? | pixi.lock | 72010 |
| H | ? | pixi.lock | 72018 |
| H | ? | pixi.lock | 72031 |
| H | ? | pixi.lock | 72040 |
| H | ? | pixi.lock | 72411 |
| H | ? | pixi.lock | 72436 |
| H | ? | pixi.lock | 72465 |
| H | ? | pixi.lock | 72487 |
| H | ? | pixi.lock | 72580 |
| H | ? | pixi.lock | 73780 |
| H | ? | pixi.lock | 74211 |
| H | ? | pixi.lock | 74306 |
| H | ? | pixi.lock | 74859 |
| H | ? | pixi.lock | 75325 |
| H | ? | pixi.lock | 75332 |
| H | ? | pixi.lock | 75401 |
| H | ? | pixi.lock | 75421 |
| H | ? | pixi.lock | 75443 |
| H | ? | pixi.lock | 75463 |
| C | ? | hashing.py | 45 |
| M | ? | validate_min_versions_in_sync.py | 32 |
| M | ? | validate_min_versions_in_sync.py | 283 |
| M | ? | run_stubtest.py | 98 |
| H | ? | eval.py | 25 |
| H | ? | eval.py | 28 |
| H | ? | eval.py | 34 |
| H | ? | eval.py | 37 |
| H | ? | frame.py | 5249 |
| H | ? | frame.py | 5260 |
| H | ? | frame.py | 5277 |
| H | ? | frame.py | 5293 |
| H | ? | frame.py | 5305 |
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
| s | GS009 |  | 0 |
| L | GS012 | format.py | 1028 |
| H | GS014 | sql.py | 369 |
| H | GS014 | sql.py | 683 |
| M | ? | package.py | 15 |

---
*Сгенерировано GSC v0.6 · 2026-07-18T04:03:54.061156*