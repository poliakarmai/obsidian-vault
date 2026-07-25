---
title: "GSC Audit: /tmp/gsc-learn/numpy"
date: 2026-07-18
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/numpy

**Дата:** 18.07.2026 04:02  
**Путь:** `/tmp/gsc-learn/numpy`  
**Всего находок:** 888  
**CRITICAL:** 6 | **HIGH:** 75 | **MEDIUM:** 93 | **LOW:** 713

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 180 |
| Python: assert in production | 61 |
| CVE-2026-56233: Path traversal | 24 |
| eval() or exec() usage | 23 |
| GS004 | 13 |
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
| Синхронный код в async | 9 |
| Bare except: | 8 |
| Хардкод IP адреса | 7 |
| CVE-2026-37270: Hardcoded credential | 6 |
| CVE-2026-56219: Authentication bypass | 4 |
| CVE-2026-55223: Insecure deserialization | 3 |
| Outdated dependency pattern | 3 |
| pickle.load() — unsafe deserialization | 3 |
| CVE-2026-54696: Buffer overflow | 2 |
| GS008 | 2 |
| Hardcoded encryption key | 2 |
| Python: File upload without content-type validation | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| CVE-2026-56413: Command injection | 1 |
| os.system() without sanitization | 1 |
| World-readable file: environment.yml (664) | 1 |
| World-readable file: .codecov.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | write_release.py | 54 |  |
| CRITICAL | ? | cb_rules.py | 78 | Match:     char *key = "__f2py_cb_#name#"; |
| CRITICAL | ? | cb_rules.py | 83 | Match:     char *key = "__f2py_cb_#name#"; |
| CRITICAL | ? | _format_impl.py | 844 | Match:             array = pickle.load(fp, **pickle_kwargs) |
| CRITICAL | ? | _npyio_impl.py | 492 | Match:                     "`allow_pickle=` keyword argument |
| CRITICAL | ? | _npyio_impl.py | 494 | Match:                 return pickle.load(fid, **pickle_kwar |
| HIGH | ? | bench_io.py | 100 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _ufunclike_impl.py | 18 |  |
| HIGH | ? | _ufunclike_impl.py | 75 |  |
| HIGH | ? | _ufunclike_impl.py | 145 |  |
| HIGH | ? | multiarray.py | 112 |  |
| HIGH | ? | gitversion.py | 7 |  |
| HIGH | ? | f90mod_rules.py | 114 |  |
| HIGH | ? | f90mod_rules.py | 116 |  |
| HIGH | ? | f90mod_rules.py | 121 |  |
| HIGH | ? | f90mod_rules.py | 125 |  |
| HIGH | ? | crackfortran.py | 3490 |  |
| HIGH | ? | crackfortran.py | 3492 |  |
| HIGH | ? | crackfortran.py | 3495 |  |
| HIGH | ? | crackfortran.py | 3499 |  |
| HIGH | ? | common_rules.py | 70 |  |
| HIGH | ? | common_rules.py | 73 |  |
| HIGH | ? | rules.py | 1356 |  |
| HIGH | ? | rules.py | 1570 |  |
| HIGH | ? | rules.py | 1572 |  |
| HIGH | ? | capi_maps.py | 159 |  |
| HIGH | ? | f2py2e.py | 383 |  |
| HIGH | ? | func2subr.py | 320 |  |
| HIGH | ? | func2subr.py | 345 |  |
| HIGH | ? | conf.py | 39 |  |
| HIGH | ? | conf.py | 90 |  |
| HIGH | ? | conf.py | 102 |  |
| HIGH | ? | conf.py | 95 |  |
| HIGH | ? | check_c_api_usage.py | 195 |  |
| HIGH | ? | check_c_api_usage.py | 237 |  |
| HIGH | ? | dragon4.c | 1072 | Match:  *    https://citeseerx.ist.psu.edu/viewdoc/download? |
| HIGH | ? | dragon4.c | 1247 | Match:      * https://citeseerx.ist.psu.edu/viewdoc/download |
| HIGH | ? | intdiv.h | 21 | Match:  * https://citeseerx.ist.psu.edu/viewdoc/summary?doi= |
| HIGH | ? | loops_arithmetic.dispatch.c.src | 20 | Match:  * https://citeseerx.ist.psu.edu/viewdoc/summary?doi= |
| HIGH | ? | numpylogo_dark.svg | 3 | Match: <!--Generator: Xara Designer (www.xara.com), SVG filt |
| HIGH | ? | numpylogo.svg | 3 | Match: <!--Generator: Xara Designer (www.xara.com), SVG filt |
| HIGH | ? | getting_started.svg | 1 | Match: <svg xmlns="http://www.w3.org/2000/svg" xml:space="pr |
| HIGH | ? | bench_indexing.py | 29 | Match:         exec(code, ns) |
| HIGH | ? | bench_ma.py | 141 | Match:         fun = eval(f"{mtype}.{func}") |
| HIGH | ? | bench_ma.py | 192 | Match:         fun = eval(f"{mtype}.{func}") |
| HIGH | ? | bench_ma.py | 264 | Match:         fun = eval(f"{mtype}.where") |
| HIGH | ? | _tempita.py | 320 | Match:                 value = eval(code, self.default_names |
| HIGH | ? | _tempita.py | 335 | Match:             exec(code, self.default_namespace, ns) |
| HIGH | ? | auxfuncs.py | 632 | Match:     return eval(f"{l1}:{' and '.join(l2)}") |
| HIGH | ? | auxfuncs.py | 640 | Match:     return eval(f"{l1}:{' or '.join(l2)}") |
| HIGH | ? | auxfuncs.py | 644 | Match:     return eval('lambda v,f=f:not f(v)') |
| HIGH | ? | crackfortran.py | 1325 | Match:                 v = eval(initexpr, {}, params) |
| HIGH | ? | crackfortran.py | 2274 | Match:     r = eval(e, g, l) |
| HIGH | ? | crackfortran.py | 2562 | Match:         value = eval(value, {}, params) |
| HIGH | ? | crackfortran.py | 2639 | Match:                     l = str(eval(l, {}, params)) |
| HIGH | ? | crackfortran.py | 2648 | Match:                     l = str(eval(l, {}, params)) |
| HIGH | ? | crackfortran.py | 2916 | Match:                                     kindselect['kind' |
| HIGH | ? | crackfortran.py | 2987 | Match:             p = eval(v, g_params, params) |
| HIGH | ? | crackfortran.py | 3018 | Match:             item = eval(item, g_params, params) |
| HIGH | ? | crackfortran.py | 3470 | Match:                     v = eval(v) |
| HIGH | ? | capi_maps.py | 161 | Match:             d = eval(f.read().lower(), {}, {}) |
| HIGH | ? | capi_maps.py | 301 | Match:             ret['size'] = repr(eval(ret['size'])) |
| HIGH | ? | capi_maps.py | 449 | Match:                     v = eval(v, {}, {}) |
| HIGH | ? | utils.py | 1373 | Match:     exec(astr, dict) |
| HIGH | ? | utils.py | 1661 | Match:         exec(code, globs, locs) |
| HIGH | ? | write_release.py | 54 | Match:     os.system(f"cp {notes} {target_rst}") |
| HIGH | ? | environment.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | bench_indexing.py | 29 | Line 29: exec(code, ns) |
| HIGH | GS004 | bench_ma.py | 141 | Line 141: fun = eval(f"{mtype}.{func}") |
| HIGH | GS004 | bench_ma.py | 192 | Line 192: fun = eval(f"{mtype}.{func}") |
| HIGH | GS004 | bench_ma.py | 264 | Line 264: fun = eval(f"{mtype}.where") |
| HIGH | GS004 | _tempita.py | 243 | Line 243: self._exec(code[2], ns, pos) |
| HIGH | GS004 | _tempita.py | 332 | Line 332: def _exec(self, code, ns, pos): |
| HIGH | GS004 | _tempita.py | 335 | Line 335: exec(code, self.default_namespace, ns) |
| HIGH | GS004 | auxfuncs.py | 632 | Line 632: return eval(f"{l1}:{' and '.join(l2)}") |
| HIGH | GS004 | auxfuncs.py | 640 | Line 640: return eval(f"{l1}:{' or '.join(l2)}") |
| HIGH | GS004 | rules.py | 248 | Line 248: static int f2py_module_exec(PyObject *m) { |
| HIGH | GS004 | utils.py | 1373 | Line 1373: exec(astr, dict) |
| HIGH | GS004 | utils.py | 1661 | Line 1661: exec(code, globs, locs) |
| HIGH | GS004 | write_release.py | 54 | Line 54: os.system(f"cp {notes} {target_rst}") |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | _generator.pyx | 4157 |
| M | ? | _generator.pyx | 4186 |
| M | ? | _generator.pyx | 4538 |
| M | ? | mtrand.pyx | 4402 |
| M | ? | mtrand.pyx | 4545 |
| M | ? | _common.pyx | 179 |
| M | ? | __init__.cython-30.pxd | 1096 |
| M | ? | __init__.cython-30.pxd | 1111 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| L | ? | _twodim_base_impl.pyi | 66 |
| L | ? | _dtype_like.py | 21 |
| L | ? | _add_newdocs.py | 2426 |
| L | ? | umath.pyi | 3121 |
| L | ? | crackfortran.py | 2142 |
| L | ? | crackfortran.py | 2518 |
| L | ? | cfuncs.py | 754 |
| L | ? | polynomial.py | 405 |
| L | ? | chebyshev.py | 797 |
| M | ? | _format_impl.py | 402 |
| M | ? | _function_base_impl.py | 3991 |
| M | ? | _function_base_impl.py | 3995 |
| M | ? | _function_base_impl.py | 4193 |
| M | ? | _function_base_impl.py | 4473 |
| M | ? | _tempita.py | 281 |
| M | ? | _tempita.py | 306 |
| M | ? | _linalg.py | 3024 |
| M | ? | generate_umath.py | 88 |
| M | ? | generate_umath.py | 91 |
| M | ? | _exceptions.py | 26 |
| M | ? | _exceptions.py | 57 |
| M | ? | crackfortran.py | 670 |
| M | ? | crackfortran.py | 713 |
| M | ? | crackfortran.py | 886 |
| M | ? | crackfortran.py | 1201 |
| M | ? | symbolic.py | 170 |
| M | ? | symbolic.py | 176 |
| M | ? | symbolic.py | 177 |
| M | ? | symbolic.py | 178 |
| M | ? | symbolic.py | 182 |
| M | ? | symbolic.py | 183 |
| M | ? | symbolic.py | 184 |
| M | ? | symbolic.py | 187 |
| M | ? | symbolic.py | 191 |
| M | ? | symbolic.py | 192 |
| M | ? | symbolic.py | 194 |
| M | ? | symbolic.py | 197 |
| M | ? | symbolic.py | 200 |
| M | ? | symbolic.py | 201 |
| M | ? | symbolic.py | 205 |
| M | ? | symbolic.py | 209 |
| M | ? | symbolic.py | 211 |
| M | ? | symbolic.py | 212 |
| M | ? | symbolic.py | 213 |
| M | ? | symbolic.py | 216 |
| M | ? | symbolic.py | 218 |
| M | ? | symbolic.py | 221 |
| M | ? | symbolic.py | 224 |
| M | ? | symbolic.py | 227 |
| M | ? | symbolic.py | 599 |
| M | ? | symbolic.py | 846 |
| M | ? | symbolic.py | 1194 |
| M | ? | symbolic.py | 1195 |
| M | ? | symbolic.py | 1257 |
| M | ? | symbolic.py | 1331 |
| M | ? | symbolic.py | 1358 |
| M | ? | symbolic.py | 1397 |
| M | ? | symbolic.py | 1424 |
| M | ? | symbolic.py | 1506 |
| M | ? | f2py2e.py | 668 |
| M | ? | func2subr.py | 96 |
| M | ? | func2subr.py | 224 |
| M | ? | utils.py | 841 |
| M | ? | core.py | 7087 |
| M | ? | core.py | 7094 |
| M | ? | core.py | 8898 |
| M | ? | refguide_check.py | 628 |
| M | ? | check_openblas_version.py | 32 |
| M | ? | check_openblas_version.py | 35 |
| M | ? | check_openblas_version.py | 36 |
| H | ? | bench_io.py | 100 |
| M | ? | _simd.pyi | 21 |
| M | ? | cfuncs.py | 520 |
| M | ? | _format_impl.py | 844 |
| M | ? | _npyio_impl.py | 492 |
| M | ? | _npyio_impl.py | 494 |
| H | ? | _ufunclike_impl.py | 18 |
| H | ? | _ufunclike_impl.py | 75 |
| H | ? | _ufunclike_impl.py | 145 |
| H | ? | multiarray.py | 112 |
| H | ? | gitversion.py | 7 |
| H | ? | f90mod_rules.py | 114 |
| H | ? | f90mod_rules.py | 116 |
| H | ? | f90mod_rules.py | 121 |
| H | ? | f90mod_rules.py | 125 |
| H | ? | crackfortran.py | 3490 |
| H | ? | crackfortran.py | 3492 |
| H | ? | crackfortran.py | 3495 |
| H | ? | crackfortran.py | 3499 |
| H | ? | common_rules.py | 70 |
| H | ? | common_rules.py | 73 |
| H | ? | rules.py | 1356 |
| H | ? | rules.py | 1570 |
| H | ? | rules.py | 1572 |
| H | ? | capi_maps.py | 159 |
| H | ? | f2py2e.py | 383 |
| H | ? | func2subr.py | 320 |
| H | ? | func2subr.py | 345 |
| H | ? | conf.py | 39 |
| H | ? | conf.py | 90 |
| H | ? | conf.py | 102 |
| H | ? | conf.py | 95 |
| H | ? | check_c_api_usage.py | 195 |
| H | ? | check_c_api_usage.py | 237 |
| M | ? | refguide_check.py | 438 |
| C | ? | write_release.py | 54 |
| M | ? | conv_template.py | 305 |
| M | ? | cb_rules.py | 78 |
| M | ? | cb_rules.py | 83 |
| M | ? | f2py2e.py | 584 |
| M | ? | core.py | 4125 |
| M | ? | refguide_check.py | 438 |
| L | GS003 | asv_pip_nopep517.py | 14 |
| L | GS003 | build_index.py | 29 |
| L | GS003 | build_index.py | 31 |
| L | GS003 | build_index.py | 122 |
| L | GS003 | conf.py | 124 |
| L | GS003 | conf.py | 147 |
| L | GS003 | gcc_build_bitness.py | 13 |
| L | GS003 | gcc_build_bitness.py | 15 |
| L | GS003 | _configtool.py | 32 |
| L | GS003 | _configtool.py | 35 |
| L | GS003 | genapi.py | 551 |
| L | GS003 | genapi.py | 554 |
| L | GS003 | genapi.py | 555 |
| L | GS003 | cversions.py | 13 |
| L | GS003 | _pytesttester.py | 39 |
| L | GS003 | _pytesttester.py | 42 |
| L | GS003 | _src_pyf.py | 173 |
| L | GS003 | crackfortran.py | 956 |
| L | GS003 | crackfortran.py | 1241 |
| L | GS003 | crackfortran.py | 1530 |
| L | GS003 | crackfortran.py | 1552 |
| L | GS003 | crackfortran.py | 2543 |
| L | GS003 | diagnose.py | 10 |
| L | GS003 | diagnose.py | 11 |
| L | GS003 | diagnose.py | 12 |
| L | GS003 | diagnose.py | 13 |
| L | GS003 | diagnose.py | 14 |
| L | GS003 | diagnose.py | 15 |
| L | GS003 | diagnose.py | 16 |
| L | GS003 | diagnose.py | 17 |
| L | GS003 | diagnose.py | 18 |
| L | GS003 | diagnose.py | 19 |
| L | GS003 | diagnose.py | 20 |
| L | GS003 | diagnose.py | 21 |
| L | GS003 | diagnose.py | 22 |
| L | GS003 | diagnose.py | 28 |
| L | GS003 | diagnose.py | 35 |
| L | GS003 | diagnose.py | 40 |
| L | GS003 | diagnose.py | 42 |
| L | GS003 | diagnose.py | 43 |
| L | GS003 | diagnose.py | 47 |
| L | GS003 | diagnose.py | 50 |
| L | GS003 | diagnose.py | 51 |
| L | GS003 | f2py2e.py | 258 |
| L | GS003 | f2py2e.py | 300 |
| L | GS003 | f2py2e.py | 701 |
| L | GS003 | rules.py | 1375 |
| L | GS003 | _user_array_impl.py | 298 |
| L | GS003 | _user_array_impl.py | 299 |
| L | GS003 | _user_array_impl.py | 302 |
| L | GS003 | _user_array_impl.py | 305 |
| L | GS003 | _user_array_impl.py | 306 |
| L | GS003 | _user_array_impl.py | 307 |
| L | GS003 | _user_array_impl.py | 308 |
| L | GS003 | _user_array_impl.py | 309 |
| L | GS003 | _user_array_impl.py | 310 |
| L | GS003 | _utils_impl.py | 70 |
| L | GS003 | _utils_impl.py | 219 |
| L | GS003 | _utils_impl.py | 221 |
| L | GS003 | _utils_impl.py | 222 |
| L | GS003 | _utils_impl.py | 223 |
| L | GS003 | _utils_impl.py | 224 |
| L | GS003 | _utils_impl.py | 225 |
| L | GS003 | _utils_impl.py | 226 |
| L | GS003 | _utils_impl.py | 227 |
| L | GS003 | _utils_impl.py | 231 |
| L | GS003 | _utils_impl.py | 233 |
| L | GS003 | _utils_impl.py | 236 |
| L | GS003 | _utils_impl.py | 239 |
| L | GS003 | _utils_impl.py | 241 |
| L | GS003 | _utils_impl.py | 242 |
| L | GS003 | _utils_impl.py | 336 |
| L | GS003 | _utils_impl.py | 341 |
| L | GS003 | _utils_impl.py | 343 |
| L | GS003 | _utils_impl.py | 348 |
| L | GS003 | _utils_impl.py | 350 |
| L | GS003 | _utils_impl.py | 366 |
| L | GS003 | _utils_impl.py | 368 |
| L | GS003 | _utils_impl.py | 381 |
| L | GS003 | _utils_impl.py | 386 |
| L | GS003 | _utils_impl.py | 388 |
| L | GS003 | _utils_impl.py | 394 |
| L | GS003 | _utils_impl.py | 401 |
| L | GS003 | _utils_impl.py | 404 |
| L | GS003 | _utils_impl.py | 74 |
| L | GS003 | clapack_scrub.py | 299 |
| L | GS003 | print_coercion_tables.py | 25 |
| L | GS003 | print_coercion_tables.py | 27 |
| L | GS003 | print_coercion_tables.py | 28 |
| L | GS003 | print_coercion_tables.py | 30 |
| L | GS003 | print_coercion_tables.py | 42 |
| L | GS003 | print_coercion_tables.py | 43 |
| L | GS003 | print_coercion_tables.py | 47 |
| L | GS003 | print_coercion_tables.py | 49 |
| L | GS003 | print_coercion_tables.py | 50 |
| L | GS003 | print_coercion_tables.py | 56 |
| L | GS003 | print_coercion_tables.py | 83 |
| L | GS003 | print_coercion_tables.py | 84 |
| L | GS003 | print_coercion_tables.py | 152 |
| L | GS003 | print_coercion_tables.py | 154 |
| L | GS003 | print_coercion_tables.py | 155 |
| L | GS003 | print_coercion_tables.py | 157 |
| L | GS003 | print_coercion_tables.py | 160 |
| L | GS003 | print_coercion_tables.py | 161 |
| L | GS003 | print_coercion_tables.py | 165 |
| L | GS003 | print_coercion_tables.py | 166 |
| L | GS003 | print_coercion_tables.py | 167 |
| L | GS003 | print_coercion_tables.py | 171 |
| L | GS003 | print_coercion_tables.py | 172 |
| L | GS003 | print_coercion_tables.py | 173 |
| L | GS003 | print_coercion_tables.py | 177 |
| L | GS003 | print_coercion_tables.py | 178 |
| L | GS003 | print_coercion_tables.py | 182 |
| L | GS003 | print_coercion_tables.py | 187 |
| L | GS003 | print_coercion_tables.py | 189 |
| L | GS003 | print_coercion_tables.py | 190 |
| L | GS003 | print_coercion_tables.py | 191 |
| L | GS003 | print_coercion_tables.py | 192 |
| L | GS003 | print_coercion_tables.py | 194 |
| L | GS003 | print_coercion_tables.py | 195 |
| L | GS003 | print_coercion_tables.py | 197 |
| L | GS003 | print_coercion_tables.py | 198 |
| L | GS003 | print_coercion_tables.py | 200 |
| L | GS003 | print_coercion_tables.py | 201 |
| L | GS003 | print_coercion_tables.py | 203 |
| L | GS003 | print_coercion_tables.py | 204 |
| L | GS003 | print_coercion_tables.py | 206 |
| L | GS003 | c_coverage_report.py | 21 |
| L | GS003 | c_coverage_report.py | 179 |
| L | GS003 | changelog.py | 118 |
| L | GS003 | changelog.py | 119 |
| L | GS003 | changelog.py | 120 |
| L | GS003 | changelog.py | 121 |
| L | GS003 | changelog.py | 124 |
| L | GS003 | changelog.py | 130 |
| L | GS003 | changelog.py | 132 |
| L | GS003 | changelog.py | 133 |
| L | GS003 | changelog.py | 134 |
| L | GS003 | changelog.py | 176 |
| L | GS003 | check_installed_files.py | 51 |
| L | GS003 | check_installed_files.py | 59 |
| L | GS003 | check_installed_files.py | 72 |
| L | GS003 | check_openblas_version.py | 33 |
| L | GS003 | check_openblas_version.py | 41 |
| L | GS003 | check_python_h_first.py | 98 |
| L | GS003 | check_python_h_first.py | 120 |
| L | GS003 | check_python_h_first.py | 135 |
| L | GS003 | check_python_h_first.py | 185 |
| L | GS003 | check_c_api_usage.py | 185 |
| L | GS003 | check_c_api_usage.py | 195 |
| L | GS003 | check_c_api_usage.py | 216 |
| L | GS003 | check_c_api_usage.py | 224 |
| L | GS003 | check_c_api_usage.py | 257 |
| L | GS003 | push_docs_to_repo.py | 32 |
| L | GS003 | push_docs_to_repo.py | 39 |
| L | GS003 | push_docs_to_repo.py | 47 |
| L | GS003 | push_docs_to_repo.py | 61 |
| L | GS003 | push_docs_to_repo.py | 66 |
| L | GS003 | push_docs_to_repo.py | 71 |
| L | GS003 | push_docs_to_repo.py | 72 |
| L | GS003 | functions_missing_types.py | 113 |
| L | GS003 | get_submodule_paths.py | 31 |
| L | GS003 | linter.py | 21 |
| L | GS003 | linter.py | 35 |
| L | GS003 | linter.py | 70 |
| L | GS003 | refguide_check.py | 612 |
| L | GS003 | refguide_check.py | 644 |
| L | GS003 | refguide_check.py | 646 |
| L | GS003 | refguide_check.py | 647 |
| L | GS003 | refguide_check.py | 648 |
| L | GS003 | refguide_check.py | 649 |
| L | GS003 | refguide_check.py | 654 |
| L | GS003 | refguide_check.py | 655 |
| L | GS003 | refguide_check.py | 657 |
| L | GS003 | refguide_check.py | 658 |
| L | GS003 | refguide_check.py | 659 |
| L | GS003 | refguide_check.py | 660 |
| L | GS003 | refguide_check.py | 661 |
| L | GS003 | refguide_check.py | 664 |
| L | GS003 | refguide_check.py | 667 |
| L | GS008 | common.py | 28 |
| L | GS008 | utils.py | 131 |
| H | ? | dragon4.c | 1072 |
| H | ? | dragon4.c | 1247 |
| H | ? | intdiv.h | 21 |
| H | ? | loops_arithmetic.dispatch.c.src | 20 |
| H | ? | numpylogo_dark.svg | 3 |
| H | ? | numpylogo.svg | 3 |
| H | ? | getting_started.svg | 1 |
| C | ? | cb_rules.py | 78 |
| C | ? | cb_rules.py | 83 |
| M | ? | gitversion.py | 7 |
| M | ? | check_openblas_version.py | 60 |
| M | ? | check_openblas_version.py | 66 |
| H | ? | bench_indexing.py | 29 |
| H | ? | bench_ma.py | 141 |
| H | ? | bench_ma.py | 192 |
| H | ? | bench_ma.py | 264 |
| H | ? | _tempita.py | 320 |
| H | ? | _tempita.py | 335 |
| H | ? | auxfuncs.py | 632 |
| H | ? | auxfuncs.py | 640 |
| H | ? | auxfuncs.py | 644 |
| H | ? | crackfortran.py | 1325 |
| H | ? | crackfortran.py | 2274 |
| H | ? | crackfortran.py | 2562 |
| H | ? | crackfortran.py | 2639 |
| H | ? | crackfortran.py | 2648 |
| H | ? | crackfortran.py | 2916 |
| H | ? | crackfortran.py | 2987 |
| H | ? | crackfortran.py | 3018 |
| H | ? | crackfortran.py | 3470 |
| H | ? | capi_maps.py | 161 |
| H | ? | capi_maps.py | 301 |
| H | ? | capi_maps.py | 449 |
| H | ? | utils.py | 1373 |
| H | ? | utils.py | 1661 |
| C | ? | _format_impl.py | 844 |
| C | ? | _npyio_impl.py | 492 |
| C | ? | _npyio_impl.py | 494 |
| H | ? | write_release.py | 54 |
| H | ? | environment.yml | 0 |
| H | ? | .codecov.yml | 0 |
| H | GS004 | bench_indexing.py | 29 |
| H | GS004 | bench_ma.py | 141 |
| H | GS004 | bench_ma.py | 192 |
| H | GS004 | bench_ma.py | 264 |
| H | GS004 | _tempita.py | 243 |
| H | GS004 | _tempita.py | 332 |
| H | GS004 | _tempita.py | 335 |
| H | GS004 | auxfuncs.py | 632 |
| H | GS004 | auxfuncs.py | 640 |
| H | GS004 | rules.py | 248 |
| H | GS004 | utils.py | 1373 |
| H | GS004 | utils.py | 1661 |
| H | GS004 | write_release.py | 54 |
| s | GS009 |  | 0 |
| M | ? | asv_pip_nopep517.py | 17 |
| M | ? | _meson.py | 197 |
| M | ? | utils.py | 1507 |
| M | ? | utils.py | 2910 |
| M | ? | write_release.py | 55 |
| M | ? | linter.py | 26 |
| M | ? | linter.py | 38 |
| M | ? | linter.py | 74 |
| M | ? | check_python_h_first.py | 219 |

---
*Сгенерировано GSC v0.6 · 2026-07-18T04:02:00.134085*