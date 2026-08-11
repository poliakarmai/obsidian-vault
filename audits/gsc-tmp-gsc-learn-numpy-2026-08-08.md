---
title: "GSC Audit: /tmp/gsc-learn/numpy"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/numpy

**Дата:** 08.08.2026 04:04  
**Путь:** `/tmp/gsc-learn/numpy`  
**Всего находок:** 209  
**CRITICAL:** 0 | **HIGH:** 0 | **MEDIUM:** 8 | **LOW:** 200

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 200 |
| GS010 | 8 |
| GS009 | 1 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS010 | _generator.pyx | 4157 |
| M | GS010 | _generator.pyx | 4186 |
| M | GS010 | _generator.pyx | 4538 |
| M | GS010 | mtrand.pyx | 4402 |
| M | GS010 | mtrand.pyx | 4545 |
| M | GS010 | _common.pyx | 179 |
| M | GS010 | __init__.cython-30.pxd | 1096 |
| M | GS010 | __init__.cython-30.pxd | 1111 |
| L | GS000-LEGACY | _format_impl.py | 284 |
| L | GS000-LEGACY | _twodim_base_impl.pyi | 66 |
| L | GS000-LEGACY | _nanfunctions_impl.py | 1667 |
| L | GS000-LEGACY | _arraypad_impl.pyi | 42 |
| L | GS000-LEGACY | _datasource.py | 71 |
| L | GS000-LEGACY | _datasource.py | 332 |
| L | GS000-LEGACY | _datasource.py | 400 |
| L | GS000-LEGACY | _datasource.py | 516 |
| L | GS000-LEGACY | _datasource.py | 519 |
| L | GS000-LEGACY | recfunctions.pyi | 218 |
| L | GS000-LEGACY | recfunctions.pyi | 228 |
| L | GS000-LEGACY | recfunctions.pyi | 289 |
| L | GS000-LEGACY | recfunctions.py | 249 |
| L | GS000-LEGACY | recfunctions.py | 410 |
| L | GS000-LEGACY | _npyio_impl.py | 249 |
| L | GS000-LEGACY | _index_tricks_impl.pyi | 162 |
| L | GS000-LEGACY | _function_base_impl.py | 886 |
| L | GS000-LEGACY | mixins.py | 166 |
| L | GS000-LEGACY | _user_array_impl.pyi | 133 |
| L | GS000-LEGACY | _dtype_like.py | 21 |
| L | GS000-LEGACY | _char_codes.py | 154 |
| L | GS000-LEGACY | _methods.py | 86 |
| L | GS000-LEGACY | numeric.pyi | 942 |
| L | GS000-LEGACY | _add_newdocs.py | 2426 |
| L | GS000-LEGACY | numpy_api.py | 487 |
| L | GS000-LEGACY | generate_umath.py | 129 |
| L | GS000-LEGACY | generate_umath.py | 657 |
| L | GS000-LEGACY | umath.pyi | 229 |
| L | GS000-LEGACY | umath.pyi | 3201 |
| L | GS000-LEGACY | umath.pyi | 4020 |
| L | GS000-LEGACY | umath.pyi | 4081 |
| L | GS000-LEGACY | umath.pyi | 4425 |
| L | GS000-LEGACY | arrayprint.py | 1580 |
| L | GS000-LEGACY | fromnumeric.pyi | 153 |
| L | GS000-LEGACY | fromnumeric.pyi | 638 |
| L | GS000-LEGACY | fromnumeric.pyi | 671 |
| L | GS000-LEGACY | fromnumeric.pyi | 2112 |
| L | GS000-LEGACY | fromnumeric.py | 43 |
| L | GS000-LEGACY | _internal.pyi | 21 |
| L | GS000-LEGACY | _add_newdocs_scalars.py | 131 |
| L | GS000-LEGACY | _add_newdocs_scalars.py | 319 |
| L | GS000-LEGACY | _dtype.py | 179 |
| L | GS000-LEGACY | numeric.py | 540 |
| L | GS000-LEGACY | einsumfunc.pyi | 29 |
| L | GS000-LEGACY | _isocbind.py | 55 |
| L | GS000-LEGACY | crackfortran.py | 136 |
| L | GS000-LEGACY | crackfortran.py | 712 |
| L | GS000-LEGACY | crackfortran.py | 1434 |
| L | GS000-LEGACY | crackfortran.py | 1440 |
| L | GS000-LEGACY | crackfortran.py | 1993 |
| L | GS000-LEGACY | crackfortran.py | 2039 |
| L | GS000-LEGACY | crackfortran.py | 2142 |
| L | GS000-LEGACY | crackfortran.py | 2403 |
| L | GS000-LEGACY | crackfortran.py | 2414 |
| L | GS000-LEGACY | crackfortran.py | 2430 |
| L | GS000-LEGACY | crackfortran.py | 2472 |
| L | GS000-LEGACY | crackfortran.py | 2518 |
| L | GS000-LEGACY | crackfortran.py | 2561 |
| L | GS000-LEGACY | cfuncs.py | 413 |
| L | GS000-LEGACY | cfuncs.py | 754 |
| L | GS000-LEGACY | cfuncs.py | 814 |
| L | GS000-LEGACY | cfuncs.py | 860 |
| L | GS000-LEGACY | capi_maps.py | 254 |
| L | GS000-LEGACY | capi_maps.py | 502 |
| L | GS000-LEGACY | symbolic.py | 23 |
| L | GS000-LEGACY | symbolic.py | 24 |
| L | GS000-LEGACY | symbolic.py | 25 |
| L | GS000-LEGACY | symbolic.py | 519 |
| L | GS000-LEGACY | symbolic.py | 569 |
| L | GS000-LEGACY | symbolic.py | 810 |
| L | GS000-LEGACY | symbolic.py | 845 |
| L | GS000-LEGACY | symbolic.py | 895 |
| L | GS000-LEGACY | symbolic.py | 1107 |
| L | GS000-LEGACY | f2py2e.py | 458 |
| L | GS000-LEGACY | f2py2e.py | 650 |
| L | GS000-LEGACY | utils.py | 407 |
| L | GS000-LEGACY | utils.py | 610 |
| L | GS000-LEGACY | _ctypeslib.pyi | 50 |
| L | GS000-LEGACY | polyutils.py | 536 |
| L | GS000-LEGACY | _polybase.py | 432 |
| L | GS000-LEGACY | polynomial.py | 405 |
| L | GS000-LEGACY | chebyshev.py | 797 |
| L | GS000-LEGACY | core.py | 481 |
| L | GS000-LEGACY | core.py | 2914 |
| L | GS000-LEGACY | core.py | 4762 |
| L | GS000-LEGACY | core.py | 7110 |
| L | GS000-LEGACY | core.pyi | 978 |
| L | GS000-LEGACY | core.pyi | 1044 |
| L | GS000-LEGACY | core.pyi | 1263 |
| L | GS000-LEGACY | __init__.pyi | 1773 |
| L | GS000-LEGACY | __init__.pyi | 1868 |
| L | GS000-LEGACY | __init__.pyi | 4151 |
| L | GS000-LEGACY | __init__.pyi | 4173 |
| L | GS000-LEGACY | __init__.pyi | 7667 |
| L | GS000-LEGACY | dtypes.pyi | 495 |
| L | GS000-LEGACY | dtypes.pyi | 540 |
| L | GS000-LEGACY | dtypes.pyi | 582 |
| L | GS000-LEGACY | conf.py | 142 |
| L | GS000-LEGACY | c_coverage_report.py | 117 |
| L | GS000-LEGACY | _dtype.py | 179 |
| L | GS000-LEGACY | numeric.py | 540 |
| L | GS000-LEGACY | einsumfunc.pyi | 29 |
| L | GS000-LEGACY | _isocbind.py | 55 |
| L | GS000-LEGACY | crackfortran.py | 136 |
| L | GS000-LEGACY | crackfortran.py | 712 |
| L | GS000-LEGACY | crackfortran.py | 1434 |
| L | GS000-LEGACY | crackfortran.py | 1440 |
| L | GS000-LEGACY | crackfortran.py | 1993 |
| L | GS000-LEGACY | crackfortran.py | 2039 |
| L | GS000-LEGACY | crackfortran.py | 2142 |
| L | GS000-LEGACY | crackfortran.py | 2403 |
| L | GS000-LEGACY | crackfortran.py | 2414 |
| L | GS000-LEGACY | crackfortran.py | 2430 |
| L | GS000-LEGACY | crackfortran.py | 2472 |
| L | GS000-LEGACY | crackfortran.py | 2518 |
| L | GS000-LEGACY | crackfortran.py | 2561 |
| L | GS000-LEGACY | cfuncs.py | 413 |
| L | GS000-LEGACY | cfuncs.py | 754 |
| L | GS000-LEGACY | cfuncs.py | 814 |
| L | GS000-LEGACY | cfuncs.py | 860 |
| L | GS000-LEGACY | capi_maps.py | 254 |
| L | GS000-LEGACY | capi_maps.py | 502 |
| L | GS000-LEGACY | symbolic.py | 23 |
| L | GS000-LEGACY | symbolic.py | 24 |
| L | GS000-LEGACY | symbolic.py | 25 |
| L | GS000-LEGACY | symbolic.py | 519 |
| L | GS000-LEGACY | symbolic.py | 569 |
| L | GS000-LEGACY | symbolic.py | 810 |
| L | GS000-LEGACY | symbolic.py | 845 |
| L | GS000-LEGACY | symbolic.py | 895 |
| L | GS000-LEGACY | symbolic.py | 1107 |
| L | GS000-LEGACY | f2py2e.py | 458 |
| L | GS000-LEGACY | f2py2e.py | 650 |
| L | GS000-LEGACY | utils.py | 407 |
| L | GS000-LEGACY | utils.py | 610 |
| L | GS000-LEGACY | _ctypeslib.pyi | 50 |
| L | GS000-LEGACY | polyutils.py | 536 |
| L | GS000-LEGACY | _polybase.py | 432 |
| L | GS000-LEGACY | polynomial.py | 405 |
| L | GS000-LEGACY | chebyshev.py | 797 |
| L | GS000-LEGACY | core.py | 481 |
| L | GS000-LEGACY | core.py | 2914 |
| L | GS000-LEGACY | core.py | 4762 |
| L | GS000-LEGACY | core.py | 7110 |
| L | GS000-LEGACY | core.pyi | 978 |
| L | GS000-LEGACY | core.pyi | 1044 |
| L | GS000-LEGACY | core.pyi | 1263 |
| L | GS000-LEGACY | __init__.pyi | 1773 |
| L | GS000-LEGACY | __init__.pyi | 1868 |
| L | GS000-LEGACY | __init__.pyi | 4151 |
| L | GS000-LEGACY | __init__.pyi | 4173 |
| L | GS000-LEGACY | __init__.pyi | 7667 |
| L | GS000-LEGACY | dtypes.pyi | 495 |
| L | GS000-LEGACY | dtypes.pyi | 540 |
| L | GS000-LEGACY | dtypes.pyi | 582 |
| L | GS000-LEGACY | conf.py | 142 |
| L | GS000-LEGACY | c_coverage_report.py | 117 |
| L | GS000-LEGACY | crackfortran.py | 136 |
| L | GS000-LEGACY | crackfortran.py | 712 |
| L | GS000-LEGACY | crackfortran.py | 1434 |
| L | GS000-LEGACY | crackfortran.py | 1440 |
| L | GS000-LEGACY | crackfortran.py | 1993 |
| L | GS000-LEGACY | crackfortran.py | 2039 |
| L | GS000-LEGACY | crackfortran.py | 2142 |
| L | GS000-LEGACY | crackfortran.py | 2403 |
| L | GS000-LEGACY | crackfortran.py | 2414 |
| L | GS000-LEGACY | crackfortran.py | 2430 |
| L | GS000-LEGACY | crackfortran.py | 2472 |
| L | GS000-LEGACY | crackfortran.py | 2518 |
| L | GS000-LEGACY | crackfortran.py | 2561 |
| L | GS000-LEGACY | utils.py | 407 |
| L | GS000-LEGACY | utils.py | 610 |
| L | GS000-LEGACY | _ctypeslib.pyi | 50 |
| L | GS000-LEGACY | polyutils.py | 536 |
| L | GS000-LEGACY | _polybase.py | 432 |
| L | GS000-LEGACY | polynomial.py | 405 |
| L | GS000-LEGACY | chebyshev.py | 797 |
| L | GS000-LEGACY | core.py | 481 |
| L | GS000-LEGACY | core.py | 2914 |
| L | GS000-LEGACY | core.py | 4762 |
| L | GS000-LEGACY | core.py | 7110 |
| L | GS000-LEGACY | core.pyi | 978 |
| L | GS000-LEGACY | core.pyi | 1044 |
| L | GS000-LEGACY | core.pyi | 1263 |
| L | GS000-LEGACY | __init__.pyi | 1773 |
| L | GS000-LEGACY | __init__.pyi | 1868 |
| L | GS000-LEGACY | __init__.pyi | 4151 |
| L | GS000-LEGACY | __init__.pyi | 4173 |
| L | GS000-LEGACY | __init__.pyi | 7667 |
| L | GS000-LEGACY | dtypes.pyi | 495 |
| L | GS000-LEGACY | dtypes.pyi | 540 |
| L | GS000-LEGACY | dtypes.pyi | 582 |
| L | GS000-LEGACY | conf.py | 142 |
| L | GS000-LEGACY | c_coverage_report.py | 117 |
| L | GS000-LEGACY | conf.py | 142 |
| L | GS000-LEGACY | c_coverage_report.py | 117 |
| L | GS000-LEGACY | conf.py | 142 |
| L | GS000-LEGACY | c_coverage_report.py | 117 |
| L | GS000-LEGACY | c_coverage_report.py | 117 |
| L | GS000-LEGACY | c_coverage_report.py | 117 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:04:06.703700*