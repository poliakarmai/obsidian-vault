---
title: "GSC Audit: /tmp/gsc-learn/pytest"
date: 2026-07-31
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pytest

**Дата:** 31.07.2026 04:01  
**Путь:** `/tmp/gsc-learn/pytest`  
**Всего находок:** 1285  
**CRITICAL:** 3 | **HIGH:** 36 | **MEDIUM:** 876 | **LOW:** 366

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 867 |
| GS003 | 50 |
| GS008 | 21 |
| eval() or exec() usage | 14 |
| CVE-2026-56233: Path traversal | 6 |
| GS004 | 6 |
| GS007 | 6 |
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
| Outdated dependency pattern | 3 |
| CVE-2026-55223: Insecure deserialization | 2 |
| CVE-2026-56413: Command injection | 2 |
| Синхронный код в async | 2 |
| JWT: Hardcoded secret <32 chars | 1 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| GS015 | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS016 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | capture.py | 1112 |  |
| CRITICAL | ? | capture.py | 1140 |  |
| CRITICAL | ? | multipython.py | 55 | Match:                 obj = pickle.load(f) |
| HIGH | ? | django_settings.py | 4 | Hacking APIs (No Starch Press) |
| HIGH | ? | fixtures.py | 3819 |  |
| HIGH | ? | fixtures.py | 3821 |  |
| HIGH | ? | fixtures.py | 3830 |  |
| HIGH | ? | fixtures.py | 3832 |  |
| HIGH | ? | release.py | 53 |  |
| HIGH | ? | release.py | 58 |  |
| HIGH | ? | get_issues.py | 18 |  |
| HIGH | ? | xunit.py | 5 | Match:     exec( |
| HIGH | ? | empty.py | 5 | Match:     exec(f"def test_func_{i}(): pass") |
| HIGH | ? | collect.py | 1237 | Match:             exec("def foo(): raise ValueError", ns) |
| HIGH | ? | raises_group.py | 1210 | Match:         evaled = eval(s) |
| HIGH | ? | multipython.py | 57 | Match:                 res = eval({expression!r}) |
| HIGH | ? | failure_demo.py | 202 | Match:     exec(code, module.__dict__) |
| HIGH | ? | code.py | 164 | Match:     def eval(self, code, **vars): |
| HIGH | ? | code.py | 173 | Match:         return eval(code, self.f_globals, f_locals) |
| HIGH | ? | skipping.py | 119 | Match:             result = eval(condition_code, globals_) |
| HIGH | ? | path.py | 1153 | Match:                         exec(f.read(), mod.__dict__) |
| HIGH | ? | expression.py | 295 | Match:     """Adapts a matcher function to a locals mapping  |
| HIGH | ? | expression.py | 353 | Match:         return bool(eval(self._code, {"__builtins__": |
| HIGH | ? | pytester.py | 296 | Match:                     if eval(check, backlocals, call._ |
| HIGH | ? | rewrite.py | 188 | Match:         exec(co, module.__dict__) |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | empty.py | 5 | Line 5: exec(f"def test_func_{i}(): pass") |
| HIGH | GS004 | xunit.py | 5 | Line 5: exec( |
| HIGH | GS004 | failure_demo.py | 202 | Line 202: exec(code, module.__dict__) |
| HIGH | GS004 | path.py | 1153 | Line 1153: exec(f.read(), mod.__dict__) |
| HIGH | GS004 | path.py | 1159 | Line 1159: def sysexec(self, *argv: os.PathLike[str], **pope |
| HIGH | GS004 | rewrite.py | 188 | Line 188: exec(co, module.__dict__) |
| HIGH | GS007 | capture.py | 755 | Line 755: f"<CaptureManager _method={self._method!r} _global |
| HIGH | GS007 | pytester.py | 698 | Line 698: self._method = self._request.config.getoption("--r |
| HIGH | GS007 | pytester.py | 1215 | Line 1215: if self._method == "inprocess": |
| HIGH | GS007 | pytester.py | 1217 | Line 1217: elif self._method == "subprocess": |
| HIGH | GS011 | django_settings.py | 4 | Found JWT secret in code: 'mysecret...'. JWT secrets must be |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| L | ? | fixtures.py | 1101 |
| L | ? | path.py | 193 |
| L | ? | path.py | 222 |
| L | ? | path.py | 232 |
| L | ? | terminal.py | 1069 |
| M | ? | simple_integration.py | 8 |
| M | ? | simple_integration.py | 13 |
| M | ? | bdd_wallet.py | 42 |
| M | ? | typing_raises_group.py | 19 |
| M | ? | typing_raises_group.py | 29 |
| M | ? | typing_raises_group.py | 186 |
| M | ? | typing_raises_group.py | 199 |
| M | ? | raises.py | 26 |
| M | ? | raises.py | 31 |
| M | ? | raises.py | 195 |
| M | ? | raises.py | 228 |
| M | ? | raises.py | 230 |
| M | ? | raises.py | 236 |
| M | ? | raises.py | 238 |
| M | ? | raises.py | 271 |
| M | ? | raises.py | 273 |
| M | ? | raises.py | 298 |
| M | ? | raises.py | 323 |
| M | ? | raises.py | 334 |
| M | ? | raises.py | 379 |
| M | ? | raises.py | 384 |
| M | ? | raises.py | 471 |
| M | ? | raises.py | 472 |
| M | ? | raises.py | 473 |
| M | ? | raises.py | 480 |
| M | ? | raises.py | 482 |
| M | ? | raises.py | 484 |
| M | ? | raises.py | 487 |
| M | ? | raises.py | 489 |
| M | ? | raises.py | 515 |
| M | ? | fixtures.py | 28 |
| M | ? | fixtures.py | 33 |
| M | ? | fixtures.py | 38 |
| M | ? | fixtures.py | 43 |
| M | ? | fixtures.py | 65 |
| M | ? | fixtures.py | 66 |
| M | ? | fixtures.py | 67 |
| M | ? | fixtures.py | 68 |
| M | ? | fixtures.py | 69 |
| M | ? | fixtures.py | 80 |
| M | ? | fixtures.py | 94 |
| M | ? | fixtures.py | 118 |
| M | ? | fixtures.py | 132 |
| M | ? | fixtures.py | 140 |
| M | ? | fixtures.py | 159 |
| M | ? | fixtures.py | 163 |
| M | ? | fixtures.py | 164 |
| M | ? | fixtures.py | 165 |
| M | ? | fixtures.py | 230 |
| M | ? | fixtures.py | 262 |
| M | ? | fixtures.py | 625 |
| M | ? | fixtures.py | 646 |
| M | ? | fixtures.py | 703 |
| M | ? | fixtures.py | 708 |
| M | ? | fixtures.py | 802 |
| M | ? | fixtures.py | 831 |
| M | ? | fixtures.py | 861 |
| M | ? | fixtures.py | 863 |
| M | ? | fixtures.py | 891 |
| M | ? | fixtures.py | 924 |
| M | ? | fixtures.py | 1001 |
| M | ? | fixtures.py | 1010 |
| M | ? | fixtures.py | 1012 |
| M | ? | fixtures.py | 1014 |
| M | ? | fixtures.py | 1016 |
| M | ? | fixtures.py | 1017 |
| M | ? | fixtures.py | 1018 |
| M | ? | fixtures.py | 1019 |
| M | ? | fixtures.py | 1032 |
| M | ? | fixtures.py | 1037 |
| M | ? | fixtures.py | 1040 |
| M | ? | fixtures.py | 1043 |
| M | ? | fixtures.py | 1081 |
| M | ? | fixtures.py | 1152 |
| M | ? | fixtures.py | 1154 |
| M | ? | fixtures.py | 1248 |
| M | ? | fixtures.py | 1257 |
| M | ? | fixtures.py | 1259 |
| M | ? | fixtures.py | 1324 |
| M | ? | fixtures.py | 1326 |
| M | ? | fixtures.py | 1328 |
| M | ? | fixtures.py | 1329 |
| M | ? | fixtures.py | 1331 |
| M | ? | fixtures.py | 1535 |
| M | ? | fixtures.py | 1536 |
| M | ? | fixtures.py | 1601 |
| M | ? | fixtures.py | 1602 |
| M | ? | fixtures.py | 1604 |
| M | ? | fixtures.py | 1605 |
| M | ? | fixtures.py | 1710 |
| M | ? | fixtures.py | 2033 |
| M | ? | fixtures.py | 2056 |
| M | ? | fixtures.py | 2097 |
| M | ? | fixtures.py | 2099 |
| M | ? | fixtures.py | 2147 |
| M | ? | fixtures.py | 2148 |
| M | ? | fixtures.py | 2149 |
| M | ? | fixtures.py | 2165 |
| M | ? | fixtures.py | 2172 |
| M | ? | fixtures.py | 2187 |
| M | ? | fixtures.py | 2189 |
| M | ? | fixtures.py | 2213 |
| M | ? | fixtures.py | 2217 |
| M | ? | fixtures.py | 2444 |
| M | ? | fixtures.py | 2553 |
| M | ? | fixtures.py | 2591 |
| M | ? | fixtures.py | 2608 |
| M | ? | fixtures.py | 2609 |
| M | ? | fixtures.py | 2658 |
| M | ? | fixtures.py | 2662 |
| M | ? | fixtures.py | 2679 |
| M | ? | fixtures.py | 2681 |
| M | ? | fixtures.py | 2682 |
| M | ? | fixtures.py | 2685 |
| M | ? | fixtures.py | 2686 |
| M | ? | fixtures.py | 2707 |
| M | ? | fixtures.py | 2732 |
| M | ? | fixtures.py | 2733 |
| M | ? | fixtures.py | 2762 |
| M | ? | fixtures.py | 2779 |
| M | ? | fixtures.py | 2781 |
| M | ? | fixtures.py | 2782 |
| M | ? | fixtures.py | 2785 |
| M | ? | fixtures.py | 2786 |
| M | ? | fixtures.py | 2801 |
| M | ? | fixtures.py | 2814 |
| M | ? | fixtures.py | 2815 |
| M | ? | fixtures.py | 2817 |
| M | ? | fixtures.py | 2818 |
| M | ? | fixtures.py | 2821 |
| M | ? | fixtures.py | 2822 |
| M | ? | fixtures.py | 2825 |
| M | ? | fixtures.py | 2826 |
| M | ? | fixtures.py | 2913 |
| M | ? | fixtures.py | 2917 |
| M | ? | fixtures.py | 2964 |
| M | ? | fixtures.py | 3298 |
| M | ? | fixtures.py | 3308 |
| M | ? | fixtures.py | 3314 |
| M | ? | fixtures.py | 3351 |
| M | ? | fixtures.py | 3374 |
| M | ? | fixtures.py | 3378 |
| M | ? | fixtures.py | 3382 |
| M | ? | fixtures.py | 3386 |
| M | ? | fixtures.py | 3402 |
| M | ? | fixtures.py | 3428 |
| M | ? | fixtures.py | 3429 |
| M | ? | fixtures.py | 3430 |
| M | ? | fixtures.py | 3431 |
| M | ? | fixtures.py | 3476 |
| M | ? | fixtures.py | 3523 |
| M | ? | fixtures.py | 3661 |
| M | ? | fixtures.py | 3662 |
| M | ? | fixtures.py | 3683 |
| M | ? | fixtures.py | 3687 |
| M | ? | fixtures.py | 3688 |
| M | ? | fixtures.py | 3703 |
| M | ? | fixtures.py | 3707 |
| M | ? | fixtures.py | 3708 |
| M | ? | fixtures.py | 3752 |
| M | ? | fixtures.py | 3798 |
| M | ? | fixtures.py | 3800 |
| M | ? | fixtures.py | 3803 |
| M | ? | fixtures.py | 3809 |
| M | ? | fixtures.py | 3813 |
| M | ? | fixtures.py | 4072 |
| M | ? | collect.py | 62 |
| M | ? | collect.py | 281 |
| M | ? | collect.py | 305 |
| M | ? | collect.py | 355 |
| M | ? | collect.py | 363 |
| M | ? | collect.py | 364 |
| M | ? | collect.py | 404 |
| M | ? | collect.py | 408 |
| M | ? | collect.py | 414 |
| M | ? | collect.py | 589 |
| M | ? | collect.py | 639 |
| M | ? | collect.py | 644 |
| M | ? | collect.py | 657 |
| M | ? | collect.py | 668 |
| M | ? | collect.py | 669 |
| M | ? | collect.py | 699 |
| M | ? | collect.py | 700 |
| M | ? | collect.py | 701 |
| M | ? | collect.py | 702 |
| M | ? | collect.py | 718 |
| M | ? | collect.py | 719 |
| M | ? | collect.py | 720 |
| M | ? | collect.py | 721 |
| M | ? | collect.py | 828 |
| M | ? | collect.py | 830 |
| M | ? | collect.py | 861 |
| M | ? | collect.py | 863 |
| M | ? | collect.py | 865 |
| M | ? | collect.py | 866 |
| M | ? | collect.py | 867 |
| M | ? | collect.py | 870 |
| M | ? | collect.py | 871 |
| M | ? | collect.py | 872 |
| M | ? | collect.py | 875 |
| M | ? | collect.py | 876 |
| M | ? | collect.py | 877 |
| M | ? | collect.py | 878 |
| M | ? | collect.py | 879 |
| M | ? | collect.py | 900 |
| M | ? | collect.py | 901 |
| M | ? | collect.py | 1060 |
| M | ? | collect.py | 1091 |
| M | ? | collect.py | 1092 |
| M | ? | collect.py | 1136 |
| M | ? | collect.py | 1144 |
| M | ? | collect.py | 1145 |
| M | ? | collect.py | 1146 |
| M | ? | collect.py | 1147 |
| M | ? | collect.py | 1161 |
| M | ? | collect.py | 1163 |
| M | ? | collect.py | 1164 |
| M | ? | collect.py | 1166 |
| M | ? | collect.py | 1170 |
| M | ? | collect.py | 1172 |
| M | ? | collect.py | 1184 |
| M | ? | collect.py | 1186 |
| M | ? | collect.py | 1187 |
| M | ? | collect.py | 1191 |
| M | ? | collect.py | 1192 |
| M | ? | collect.py | 1218 |
| M | ? | collect.py | 1220 |
| M | ? | collect.py | 1242 |
| M | ? | collect.py | 1244 |
| M | ? | collect.py | 1245 |
| M | ? | approx.py | 68 |
| M | ? | approx.py | 72 |
| M | ? | approx.py | 84 |
| M | ? | approx.py | 264 |
| M | ? | approx.py | 268 |
| M | ? | approx.py | 277 |
| M | ? | approx.py | 279 |
| M | ? | approx.py | 340 |
| M | ? | approx.py | 341 |
| M | ? | approx.py | 342 |
| M | ? | approx.py | 343 |
| M | ? | approx.py | 344 |
| M | ? | approx.py | 345 |
| M | ? | approx.py | 348 |
| M | ? | approx.py | 353 |
| M | ? | approx.py | 354 |
| M | ? | approx.py | 355 |
| M | ? | approx.py | 356 |
| M | ? | approx.py | 359 |
| M | ? | approx.py | 360 |
| M | ? | approx.py | 363 |
| M | ? | approx.py | 365 |
| M | ? | approx.py | 368 |
| M | ? | approx.py | 371 |
| M | ? | approx.py | 387 |
| M | ? | approx.py | 391 |
| M | ? | approx.py | 393 |
| M | ? | approx.py | 424 |
| M | ? | approx.py | 427 |
| M | ? | approx.py | 428 |
| M | ? | approx.py | 429 |
| M | ? | approx.py | 430 |
| M | ? | approx.py | 444 |
| M | ? | approx.py | 449 |
| M | ? | approx.py | 454 |
| M | ? | approx.py | 455 |
| M | ? | approx.py | 456 |
| M | ? | approx.py | 457 |
| M | ? | approx.py | 458 |
| M | ? | approx.py | 459 |
| M | ? | approx.py | 487 |
| M | ? | approx.py | 488 |
| M | ? | approx.py | 489 |
| M | ? | approx.py | 490 |
| M | ? | approx.py | 511 |
| M | ? | approx.py | 530 |
| M | ? | approx.py | 533 |
| M | ? | approx.py | 534 |
| M | ? | approx.py | 535 |
| M | ? | approx.py | 536 |
| M | ? | approx.py | 538 |
| M | ? | approx.py | 539 |
| M | ? | approx.py | 540 |
| M | ? | approx.py | 541 |
| M | ? | approx.py | 543 |
| M | ? | approx.py | 544 |
| M | ? | approx.py | 545 |
| M | ? | approx.py | 546 |
| M | ? | approx.py | 551 |
| M | ? | approx.py | 552 |
| M | ? | approx.py | 557 |
| M | ? | approx.py | 558 |
| M | ? | approx.py | 572 |
| M | ? | approx.py | 573 |
| M | ? | approx.py | 584 |
| M | ? | approx.py | 596 |
| M | ? | approx.py | 599 |
| M | ? | approx.py | 604 |
| M | ? | approx.py | 605 |
| M | ? | approx.py | 606 |
| M | ? | approx.py | 607 |
| M | ? | approx.py | 615 |
| M | ? | approx.py | 616 |
| M | ? | approx.py | 617 |
| M | ? | approx.py | 618 |
| M | ? | approx.py | 619 |
| M | ? | approx.py | 620 |
| M | ? | approx.py | 621 |
| M | ? | approx.py | 629 |
| M | ? | approx.py | 630 |
| M | ? | approx.py | 631 |
| M | ? | approx.py | 632 |
| M | ? | approx.py | 642 |
| M | ? | approx.py | 643 |
| M | ? | approx.py | 644 |
| M | ? | approx.py | 645 |
| M | ? | approx.py | 648 |
| M | ? | approx.py | 649 |
| M | ? | approx.py | 650 |
| M | ? | approx.py | 651 |
| M | ? | approx.py | 652 |
| M | ? | approx.py | 657 |
| M | ? | approx.py | 658 |
| M | ? | approx.py | 659 |
| M | ? | approx.py | 660 |
| M | ? | approx.py | 661 |
| M | ? | approx.py | 668 |
| M | ? | approx.py | 669 |
| M | ? | approx.py | 670 |
| M | ? | approx.py | 671 |
| M | ? | approx.py | 677 |
| M | ? | approx.py | 680 |
| M | ? | approx.py | 681 |
| M | ? | approx.py | 688 |
| M | ? | approx.py | 689 |
| M | ? | approx.py | 690 |
| M | ? | approx.py | 691 |
| M | ? | approx.py | 694 |
| M | ? | approx.py | 695 |
| M | ? | approx.py | 698 |
| M | ? | approx.py | 707 |
| M | ? | approx.py | 708 |
| M | ? | approx.py | 709 |
| M | ? | approx.py | 710 |
| M | ? | approx.py | 718 |
| M | ? | approx.py | 721 |
| M | ? | approx.py | 722 |
| M | ? | approx.py | 723 |
| M | ? | approx.py | 726 |
| M | ? | approx.py | 727 |
| M | ? | approx.py | 728 |
| M | ? | approx.py | 731 |
| M | ? | approx.py | 765 |
| M | ? | approx.py | 766 |
| M | ? | approx.py | 767 |
| M | ? | approx.py | 768 |
| M | ? | approx.py | 771 |
| M | ? | approx.py | 772 |
| M | ? | approx.py | 773 |
| M | ? | approx.py | 774 |
| M | ? | approx.py | 797 |
| M | ? | approx.py | 798 |
| M | ? | approx.py | 800 |
| M | ? | approx.py | 801 |
| M | ? | approx.py | 803 |
| M | ? | approx.py | 804 |
| M | ? | approx.py | 817 |
| M | ? | approx.py | 818 |
| M | ? | approx.py | 821 |
| M | ? | approx.py | 822 |
| M | ? | approx.py | 834 |
| M | ? | approx.py | 835 |
| M | ? | approx.py | 836 |
| M | ? | approx.py | 844 |
| M | ? | approx.py | 845 |
| M | ? | approx.py | 862 |
| M | ? | approx.py | 888 |
| M | ? | approx.py | 889 |
| M | ? | approx.py | 890 |
| M | ? | approx.py | 891 |
| M | ? | approx.py | 892 |
| M | ? | approx.py | 898 |
| M | ? | approx.py | 946 |
| M | ? | approx.py | 958 |
| M | ? | approx.py | 959 |
| M | ? | approx.py | 961 |
| M | ? | approx.py | 962 |
| M | ? | approx.py | 964 |
| M | ? | approx.py | 965 |
| M | ? | approx.py | 967 |
| M | ? | approx.py | 968 |
| M | ? | approx.py | 973 |
| M | ? | approx.py | 981 |
| M | ? | approx.py | 1003 |
| M | ? | approx.py | 1004 |
| M | ? | approx.py | 1005 |
| M | ? | approx.py | 1006 |
| M | ? | approx.py | 1014 |
| M | ? | approx.py | 1015 |
| M | ? | approx.py | 1016 |
| M | ? | approx.py | 1017 |
| M | ? | approx.py | 1028 |
| M | ? | approx.py | 1031 |
| M | ? | approx.py | 1036 |
| M | ? | approx.py | 1040 |
| M | ? | approx.py | 1041 |
| M | ? | approx.py | 1045 |
| M | ? | approx.py | 1046 |
| M | ? | approx.py | 1051 |
| M | ? | approx.py | 1061 |
| M | ? | approx.py | 1062 |
| M | ? | approx.py | 1076 |
| M | ? | approx.py | 1124 |
| M | ? | approx.py | 1126 |
| M | ? | approx.py | 1159 |
| M | ? | approx.py | 1167 |
| M | ? | approx.py | 1175 |
| M | ? | approx.py | 1183 |
| M | ? | approx.py | 1184 |
| M | ? | approx.py | 1191 |
| M | ? | approx.py | 1198 |
| M | ? | approx.py | 1205 |
| M | ? | approx.py | 1212 |
| M | ? | approx.py | 1267 |
| M | ? | approx.py | 1274 |
| M | ? | approx.py | 1275 |
| M | ? | approx.py | 1282 |
| M | ? | approx.py | 1283 |
| M | ? | approx.py | 1285 |
| M | ? | approx.py | 1286 |
| M | ? | approx.py | 1301 |
| M | ? | approx.py | 1302 |
| M | ? | approx.py | 1309 |
| M | ? | approx.py | 1310 |
| M | ? | approx.py | 1320 |
| M | ? | approx.py | 1321 |
| M | ? | approx.py | 1330 |
| M | ? | approx.py | 1331 |
| M | ? | approx.py | 1341 |
| M | ? | approx.py | 1350 |
| M | ? | approx.py | 1357 |
| M | ? | approx.py | 1366 |
| M | ? | approx.py | 1374 |
| M | ? | approx.py | 1375 |
| M | ? | approx.py | 1389 |
| M | ? | approx.py | 1390 |
| M | ? | approx.py | 1401 |
| M | ? | approx.py | 1410 |
| M | ? | approx.py | 1411 |
| M | ? | approx.py | 1416 |
| M | ? | approx.py | 1417 |
| M | ? | approx.py | 1418 |
| M | ? | approx.py | 1425 |
| M | ? | approx.py | 1428 |
| M | ? | approx.py | 1431 |
| M | ? | approx.py | 1439 |
| M | ? | approx.py | 1442 |
| M | ? | approx.py | 1450 |
| M | ? | approx.py | 1453 |
| M | ? | approx.py | 1486 |
| M | ? | approx.py | 1489 |
| M | ? | approx.py | 1492 |
| M | ? | approx.py | 1495 |
| M | ? | approx.py | 1498 |
| M | ? | approx.py | 1505 |
| M | ? | approx.py | 1512 |
| M | ? | raises_group.py | 29 |
| M | ? | raises_group.py | 449 |
| M | ? | raises_group.py | 467 |
| M | ? | raises_group.py | 472 |
| M | ? | raises_group.py | 473 |
| M | ? | raises_group.py | 474 |
| M | ? | raises_group.py | 477 |
| M | ? | raises_group.py | 478 |
| M | ? | raises_group.py | 1196 |
| M | ? | raises_group.py | 1197 |
| M | ? | raises_group.py | 1199 |
| M | ? | raises_group.py | 1201 |
| M | ? | raises_group.py | 1202 |
| M | ? | raises_group.py | 1211 |
| M | ? | raises_group.py | 1219 |
| M | ? | raises_group.py | 1229 |
| M | ? | raises_group.py | 1232 |
| M | ? | raises_group.py | 1233 |
| M | ? | raises_group.py | 1239 |
| M | ? | raises_group.py | 1245 |
| M | ? | raises_group.py | 1323 |
| M | ? | raises_group.py | 1327 |
| M | ? | integration.py | 26 |
| M | ? | integration.py | 45 |
| M | ? | integration.py | 61 |
| M | ? | integration.py | 144 |
| M | ? | integration.py | 172 |
| M | ? | integration.py | 244 |
| M | ? | integration.py | 443 |
| M | ? | integration.py | 445 |
| M | ? | integration.py | 446 |
| M | ? | integration.py | 447 |
| M | ? | integration.py | 449 |
| M | ? | integration.py | 450 |
| M | ? | integration.py | 451 |
| M | ? | integration.py | 452 |
| M | ? | integration.py | 457 |
| M | ? | integration.py | 458 |
| M | ? | integration.py | 459 |
| M | ? | integration.py | 461 |
| M | ? | integration.py | 462 |
| M | ? | integration.py | 463 |
| M | ? | integration.py | 465 |
| M | ? | metafunc.py | 98 |
| M | ? | metafunc.py | 106 |
| M | ? | metafunc.py | 107 |
| M | ? | metafunc.py | 108 |
| M | ? | metafunc.py | 109 |
| M | ? | metafunc.py | 130 |
| M | ? | metafunc.py | 131 |
| M | ? | metafunc.py | 136 |
| M | ? | metafunc.py | 137 |
| M | ? | metafunc.py | 142 |
| M | ? | metafunc.py | 143 |
| M | ? | metafunc.py | 148 |
| M | ? | metafunc.py | 149 |
| M | ? | metafunc.py | 187 |
| M | ? | metafunc.py | 249 |
| M | ? | metafunc.py | 250 |
| M | ? | metafunc.py | 251 |
| M | ? | metafunc.py | 252 |
| M | ? | metafunc.py | 253 |
| M | ? | metafunc.py | 255 |
| M | ? | metafunc.py | 256 |
| M | ? | metafunc.py | 257 |
| M | ? | metafunc.py | 258 |
| M | ? | metafunc.py | 261 |
| M | ? | metafunc.py | 264 |
| M | ? | metafunc.py | 267 |
| M | ? | metafunc.py | 271 |
| M | ? | metafunc.py | 277 |
| M | ? | metafunc.py | 288 |
| M | ? | metafunc.py | 299 |
| M | ? | metafunc.py | 325 |
| M | ? | metafunc.py | 331 |
| M | ? | metafunc.py | 352 |
| M | ? | metafunc.py | 365 |
| M | ? | metafunc.py | 366 |
| M | ? | metafunc.py | 367 |
| M | ? | metafunc.py | 368 |
| M | ? | metafunc.py | 376 |
| M | ? | metafunc.py | 397 |
| M | ? | metafunc.py | 413 |
| M | ? | metafunc.py | 425 |
| M | ? | metafunc.py | 441 |
| M | ? | metafunc.py | 451 |
| M | ? | metafunc.py | 463 |
| M | ? | metafunc.py | 473 |
| M | ? | metafunc.py | 478 |
| M | ? | metafunc.py | 484 |
| M | ? | metafunc.py | 509 |
| M | ? | metafunc.py | 541 |
| M | ? | metafunc.py | 555 |
| M | ? | metafunc.py | 563 |
| M | ? | metafunc.py | 585 |
| M | ? | metafunc.py | 605 |
| M | ? | metafunc.py | 627 |
| M | ? | metafunc.py | 644 |
| M | ? | metafunc.py | 673 |
| M | ? | metafunc.py | 711 |
| M | ? | metafunc.py | 723 |
| M | ? | metafunc.py | 757 |
| M | ? | metafunc.py | 779 |
| M | ? | metafunc.py | 786 |
| M | ? | metafunc.py | 850 |
| M | ? | metafunc.py | 861 |
| M | ? | metafunc.py | 872 |
| M | ? | metafunc.py | 883 |
| M | ? | metafunc.py | 884 |
| M | ? | metafunc.py | 885 |
| M | ? | metafunc.py | 895 |
| M | ? | metafunc.py | 898 |
| M | ? | metafunc.py | 908 |
| M | ? | metafunc.py | 909 |
| M | ? | metafunc.py | 919 |
| M | ? | metafunc.py | 920 |
| M | ? | metafunc.py | 1125 |
| M | ? | metafunc.py | 1126 |
| M | ? | metafunc.py | 1127 |
| M | ? | metafunc.py | 1128 |
| M | ? | metafunc.py | 1129 |
| M | ? | metafunc.py | 1134 |
| M | ? | metafunc.py | 1135 |
| M | ? | metafunc.py | 1136 |
| M | ? | metafunc.py | 1137 |
| M | ? | metafunc.py | 1142 |
| M | ? | metafunc.py | 1143 |
| M | ? | metafunc.py | 1144 |
| M | ? | metafunc.py | 1145 |
| M | ? | metafunc.py | 1146 |
| M | ? | metafunc.py | 1198 |
| M | ? | metafunc.py | 1242 |
| M | ? | metafunc.py | 1506 |
| M | ? | metafunc.py | 1544 |
| M | ? | metafunc.py | 1619 |
| M | ? | metafunc.py | 1641 |
| M | ? | metafunc.py | 1643 |
| M | ? | metafunc.py | 1645 |
| M | ? | metafunc.py | 1674 |
| M | ? | metafunc.py | 1692 |
| M | ? | metafunc.py | 1701 |
| M | ? | metafunc.py | 2054 |
| M | ? | metafunc.py | 2055 |
| M | ? | metafunc.py | 2088 |
| M | ? | metafunc.py | 2089 |
| M | ? | metafunc.py | 2106 |
| M | ? | metafunc.py | 2126 |
| M | ? | metafunc.py | 2145 |
| M | ? | metafunc.py | 2162 |
| M | ? | metafunc.py | 2178 |
| M | ? | metafunc.py | 2194 |
| M | ? | metafunc.py | 2210 |
| M | ? | metafunc.py | 2229 |
| M | ? | metafunc.py | 2253 |
| M | ? | metafunc.py | 2295 |
| M | ? | metafunc.py | 2420 |
| M | ? | metafunc.py | 2444 |
| M | ? | metafunc.py | 2518 |
| M | ? | issue_519.py | 23 |
| M | ? | __main__.py | 6 |
| M | ? | tmp_path_fixture.py | 9 |
| M | ? | tmp_path_fixture.py | 10 |
| M | ? | fixture_mock_integration.py | 21 |
| M | ? | xfail_demo.py | 11 |
| M | ? | xfail_demo.py | 16 |
| M | ? | xfail_demo.py | 21 |
| M | ? | xfail_demo.py | 26 |
| M | ? | xfail_demo.py | 31 |
| M | ? | failure_demo.py | 8 |
| M | ? | failure_demo.py | 16 |
| M | ? | failure_demo.py | 21 |
| M | ? | failure_demo.py | 32 |
| M | ? | failure_demo.py | 41 |
| M | ? | failure_demo.py | 46 |
| M | ? | failure_demo.py | 49 |
| M | ? | failure_demo.py | 52 |
| M | ? | failure_demo.py | 57 |
| M | ? | failure_demo.py | 62 |
| M | ? | failure_demo.py | 65 |
| M | ? | failure_demo.py | 70 |
| M | ? | failure_demo.py | 73 |
| M | ? | failure_demo.py | 76 |
| M | ? | failure_demo.py | 79 |
| M | ? | failure_demo.py | 82 |
| M | ? | failure_demo.py | 86 |
| M | ? | failure_demo.py | 90 |
| M | ? | failure_demo.py | 94 |
| M | ? | failure_demo.py | 98 |
| M | ? | failure_demo.py | 110 |
| M | ? | failure_demo.py | 122 |
| M | ? | failure_demo.py | 130 |
| M | ? | failure_demo.py | 137 |
| M | ? | failure_demo.py | 148 |
| M | ? | failure_demo.py | 158 |
| M | ? | failure_demo.py | 189 |
| M | ? | failure_demo.py | 197 |
| M | ? | failure_demo.py | 228 |
| M | ? | failure_demo.py | 237 |
| M | ? | failure_demo.py | 240 |
| M | ? | failure_demo.py | 244 |
| M | ? | failure_demo.py | 247 |
| M | ? | failure_demo.py | 252 |
| M | ? | failure_demo.py | 263 |
| M | ? | failure_demo.py | 270 |
| M | ? | failure_demo.py | 283 |
| M | ? | generate-gh-release-notes.py | 48 |
| M | ? | code.py | 270 |
| M | ? | code.py | 502 |
| M | ? | code.py | 544 |
| M | ? | code.py | 582 |
| M | ? | code.py | 583 |
| M | ? | code.py | 584 |
| M | ? | code.py | 595 |
| M | ? | code.py | 601 |
| M | ? | code.py | 609 |
| M | ? | code.py | 617 |
| M | ? | code.py | 625 |
| M | ? | code.py | 791 |
| M | ? | code.py | 862 |
| M | ? | code.py | 864 |
| M | ? | legacypath.py | 390 |
| M | ? | cacheprovider.py | 320 |
| M | ? | cacheprovider.py | 420 |
| M | ? | cacheprovider.py | 432 |
| M | ? | cacheprovider.py | 468 |
| M | ? | cacheprovider.py | 571 |
| M | ? | cacheprovider.py | 578 |
| M | ? | cacheprovider.py | 604 |
| M | ? | raises.py | 154 |
| M | ? | raises.py | 183 |
| M | ? | raises.py | 184 |
| M | ? | raises.py | 213 |
| M | ? | raises.py | 222 |
| M | ? | raises.py | 704 |
| M | ? | raises.py | 990 |
| M | ? | raises.py | 1150 |
| M | ? | raises.py | 1151 |
| M | ? | raises.py | 1168 |
| M | ? | raises.py | 1229 |
| M | ? | raises.py | 1291 |
| M | ? | raises.py | 1375 |
| M | ? | raises.py | 1408 |
| M | ? | raises.py | 1473 |
| M | ? | raises.py | 1482 |
| M | ? | raises.py | 1490 |
| M | ? | warning_types.py | 21 |
| M | ? | terminalwriter.py | 85 |
| M | ? | pprint.py | 318 |
| M | ? | pprint.py | 319 |
| M | ? | compat.py | 287 |
| M | ? | junitxml.py | 196 |
| M | ? | junitxml.py | 209 |
| M | ? | junitxml.py | 216 |
| M | ? | junitxml.py | 238 |
| M | ? | skipping.py | 285 |
| M | ? | debugging.py | 167 |
| M | ? | debugging.py | 181 |
| M | ? | debugging.py | 185 |
| M | ? | debugging.py | 296 |
| M | ? | debugging.py | 389 |
| M | ? | debugging.py | 392 |
| M | ? | faulthandler.py | 74 |
| M | ? | faulthandler.py | 84 |
| M | ? | fixtures.py | 288 |
| M | ? | fixtures.py | 609 |
| M | ? | fixtures.py | 692 |
| M | ? | fixtures.py | 911 |
| M | ? | fixtures.py | 1001 |
| M | ? | fixtures.py | 1271 |
| M | ? | fixtures.py | 1282 |
| M | ? | fixtures.py | 2285 |
| M | ? | fixtures.py | 2494 |
| M | ? | runner.py | 191 |
| M | ? | runner.py | 247 |
| M | ? | runner.py | 422 |
| M | ? | runner.py | 424 |
| M | ? | runner.py | 430 |
| M | ? | runner.py | 527 |
| M | ? | runner.py | 532 |
| M | ? | runner.py | 546 |
| M | ? | runner.py | 547 |
| M | ? | runner.py | 548 |
| M | ? | runner.py | 583 |
| M | ? | path.py | 844 |
| M | ? | path.py | 1124 |
| M | ? | approx.py | 113 |
| M | ? | approx.py | 177 |
| M | ? | approx.py | 687 |
| M | ? | helpconfig.py | 187 |
| M | ? | findpaths.py | 349 |
| M | ? | argparsing.py | 258 |
| M | ? | argparsing.py | 552 |
| M | ? | capture.py | 199 |
| M | ? | capture.py | 208 |
| M | ? | capture.py | 225 |
| M | ? | capture.py | 396 |
| M | ? | capture.py | 452 |
| M | ? | capture.py | 513 |
| M | ? | capture.py | 661 |
| M | ? | capture.py | 664 |
| M | ? | capture.py | 685 |
| M | ? | capture.py | 772 |
| M | ? | capture.py | 802 |
| M | ? | capture.py | 1023 |
| M | ? | capture.py | 1056 |
| M | ? | capture.py | 1086 |
| M | ? | capture.py | 1114 |
| M | ? | capture.py | 1142 |
| M | ? | unittest.py | 236 |
| M | ? | unittest.py | 385 |
| M | ? | unittest.py | 400 |
| M | ? | unittest.py | 487 |
| M | ? | unittest.py | 653 |
| M | ? | structures.py | 122 |
| M | ? | structures.py | 296 |
| M | ? | structures.py | 486 |
| M | ? | pytester.py | 319 |
| M | ? | pytester.py | 432 |
| M | ? | pytester.py | 437 |
| M | ? | pytester.py | 793 |
| M | ? | pytester.py | 1204 |
| M | ? | pytester.py | 1288 |
| M | ? | pytester.py | 1324 |
| M | ? | pytester.py | 1379 |
| M | ? | pytester.py | 1382 |
| M | ? | stepwise.py | 63 |
| M | ? | stepwise.py | 104 |
| M | ? | stepwise.py | 186 |
| M | ? | tmpdir.py | 226 |
| M | ? | tmpdir.py | 348 |
| M | ? | pytester_assertions.py | 34 |
| M | ? | pytester_assertions.py | 74 |
| M | ? | terminal.py | 703 |
| M | ? | terminal.py | 721 |
| M | ? | terminal.py | 768 |
| M | ? | terminal.py | 1028 |
| M | ? | terminal.py | 1029 |
| M | ? | terminal.py | 1364 |
| M | ? | terminal.py | 1365 |
| M | ? | terminal.py | 1366 |
| M | ? | terminal.py | 1408 |
| M | ? | terminal.py | 1409 |
| M | ? | terminal.py | 1592 |
| M | ? | terminal.py | 1593 |
| M | ? | terminal.py | 1594 |
| M | ? | terminal.py | 1698 |
| M | ? | terminal.py | 1699 |
| M | ? | terminal.py | 1737 |
| M | ? | terminal.py | 1745 |
| M | ? | terminal.py | 1770 |
| M | ? | terminal.py | 1785 |
| M | ? | warnings.py | 46 |
| M | ? | nodes.py | 262 |
| M | ? | nodes.py | 568 |
| M | ? | nodes.py | 571 |
| M | ? | nodes.py | 573 |
| M | ? | nodes.py | 588 |
| M | ? | nodes.py | 763 |
| M | ? | python.py | 242 |
| M | ? | python.py | 326 |
| M | ? | python.py | 472 |
| M | ? | python.py | 780 |
| M | ? | python.py | 789 |
| M | ? | python.py | 1443 |
| M | ? | python.py | 1449 |
| M | ? | python.py | 1456 |
| M | ? | python.py | 1770 |
| M | ? | _compare_any.py | 105 |
| M | ? | rewrite.py | 149 |
| M | ? | rewrite.py | 150 |
| M | ? | rewrite.py | 409 |
| M | ? | rewrite.py | 563 |
| M | ? | rewrite.py | 684 |
| M | ? | rewrite.py | 741 |
| M | ? | rewrite.py | 841 |
| M | ? | rewrite.py | 859 |
| M | ? | rewrite.py | 890 |
| M | ? | rewrite.py | 893 |
| M | ? | rewrite.py | 939 |
| M | ? | rewrite.py | 942 |
| M | ? | main.py | 942 |
| M | ? | main.py | 987 |
| M | ? | main.py | 1053 |
| M | ? | logging.py | 117 |
| M | ? | logging.py | 710 |
| M | ? | recwarn.py | 242 |
| M | ? | recwarn.py | 293 |
| M | ? | doctest.py | 352 |
| M | ? | doctest.py | 355 |
| M | ? | pastebin.py | 119 |
| M | ? | pathlib.py | 463 |
| M | ? | pathlib.py | 756 |
| M | ? | pathlib.py | 1062 |
| M | ? | pathlib.py | 1063 |
| M | ? | reports.py | 277 |
| M | ? | reports.py | 284 |
| M | ? | reports.py | 392 |
| M | ? | reports.py | 415 |
| M | ? | reports.py | 420 |
| M | ? | reports.py | 535 |
| M | ? | reports.py | 574 |
| H | ? | django_settings.py | 4 |
| M | ? | multipython.py | 55 |
| M | ? | path.py | 398 |
| H | ? | fixtures.py | 3819 |
| H | ? | fixtures.py | 3821 |
| H | ? | fixtures.py | 3830 |
| H | ? | fixtures.py | 3832 |
| H | ? | release.py | 53 |
| H | ? | release.py | 58 |
| H | ? | get_issues.py | 18 |
| M | ? | django_settings.py | 4 |
| C | ? | capture.py | 1112 |
| C | ? | capture.py | 1140 |
| L | GS003 | bench.py | 17 |
| L | GS003 | bench_argcomplete.py | 21 |
| L | GS003 | bench_argcomplete.py | 22 |
| L | GS003 | failure_demo.py | 181 |
| L | GS003 | get_issues.py | 22 |
| L | GS003 | get_issues.py | 67 |
| L | GS003 | get_issues.py | 68 |
| L | GS003 | get_issues.py | 69 |
| L | GS003 | get_issues.py | 75 |
| L | GS003 | generate-gh-release-notes.py | 54 |
| L | GS003 | generate-gh-release-notes.py | 58 |
| L | GS003 | generate-gh-release-notes.py | 62 |
| L | GS003 | generate-gh-release-notes.py | 63 |
| L | GS003 | generate-gh-release-notes.py | 64 |
| L | GS003 | release.py | 55 |
| L | GS003 | release.py | 67 |
| L | GS003 | release.py | 71 |
| L | GS003 | release.py | 81 |
| L | GS003 | release.py | 90 |
| L | GS003 | release.py | 98 |
| L | GS003 | release.py | 115 |
| L | GS003 | release.py | 117 |
| L | GS003 | release.py | 118 |
| L | GS003 | release.py | 119 |
| L | GS003 | capture.py | 1021 |
| L | GS003 | capture.py | 1054 |
| L | GS003 | capture.py | 1084 |
| L | GS003 | debugging.py | 66 |
| L | GS003 | debugging.py | 112 |
| L | GS003 | debugging.py | 139 |
| L | GS003 | hookspec.py | 18 |
| L | GS003 | pytester.py | 295 |
| L | GS003 | pytester.py | 297 |
| L | GS003 | pytester.py | 299 |
| L | GS003 | pytester.py | 303 |
| L | GS003 | pytester.py | 1429 |
| L | GS003 | pytester.py | 1430 |
| L | GS003 | pytester.py | 1476 |
| L | GS003 | pytester.py | 1478 |
| L | GS003 | reports.py | 250 |
| L | GS003 | reports.py | 251 |
| L | GS003 | reports.py | 252 |
| L | GS003 | reports.py | 253 |
| L | GS003 | reports.py | 254 |
| L | GS003 | reports.py | 255 |
| L | GS003 | fixtures.py | 1042 |
| L | GS003 | fixtures.py | 3483 |
| L | GS003 | integration.py | 246 |
| L | GS003 | raises.py | 87 |
| L | GS003 | raises.py | 88 |
| L | GS008 | prepare-release-pr.py | 33 |
| L | GS008 | _typing.py | 25 |
| L | GS008 | deprecated.py | 23 |
| L | GS008 | deprecated.py | 32 |
| L | GS008 | deprecated.py | 37 |
| L | GS008 | deprecated.py | 50 |
| L | GS008 | deprecated.py | 59 |
| L | GS008 | deprecated.py | 66 |
| L | GS008 | deprecated.py | 74 |
| L | GS008 | deprecated.py | 80 |
| L | GS008 | deprecated.py | 85 |
| L | GS008 | deprecated.py | 93 |
| L | GS008 | deprecated.py | 118 |
| L | GS008 | deprecated.py | 122 |
| L | GS008 | deprecated.py | 127 |
| L | GS008 | deprecated.py | 132 |
| L | GS008 | deprecated.py | 137 |
| L | GS008 | monkeypatch.py | 28 |
| L | GS008 | outcomes.py | 36 |
| L | GS008 | pathlib.py | 46 |
| L | GS008 | scope.py | 91 |
| I | GS015 | main.py | 1 |
| M | ? | helpconfig.py | 193 |
| M | ? | findpaths.py | 179 |
| M | ? | findpaths.py | 195 |
| H | ? | xunit.py | 5 |
| H | ? | empty.py | 5 |
| H | ? | collect.py | 1237 |
| H | ? | raises_group.py | 1210 |
| H | ? | multipython.py | 57 |
| H | ? | failure_demo.py | 202 |
| H | ? | code.py | 164 |
| H | ? | code.py | 173 |
| H | ? | skipping.py | 119 |
| H | ? | path.py | 1153 |
| H | ? | expression.py | 295 |
| H | ? | expression.py | 353 |
| H | ? | pytester.py | 296 |
| H | ? | rewrite.py | 188 |
| C | ? | multipython.py | 55 |
| H | ? | codecov.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | empty.py | 5 |
| H | GS004 | xunit.py | 5 |
| H | GS004 | failure_demo.py | 202 |
| H | GS004 | path.py | 1153 |
| H | GS004 | path.py | 1159 |
| H | GS004 | rewrite.py | 188 |
| I | GS007 | update-plugin-list.py | 95 |
| I | GS007 | update-plugin-list.py | 115 |
| H | GS007 | capture.py | 755 |
| H | GS007 | pytester.py | 698 |
| H | GS007 | pytester.py | 1215 |
| H | GS007 | pytester.py | 1217 |
| s | GS009 |  | 0 |
| H | GS011 | django_settings.py | 4 |
| M | GS016 | tox.ini | 187 |
| M | ? | pytester.py | 129 |
| M | ? | pytester.py | 162 |

---
*Сгенерировано GSC v0.6 · 2026-07-31T04:01:01.289724*