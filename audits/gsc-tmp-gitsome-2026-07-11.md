---
title: "GSC Audit: /tmp/gitsome"
date: 2026-07-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gitsome

**Дата:** 11.07.2026 13:49  
**Путь:** `/tmp/gitsome`  
**Всего находок:** 436  
**CRITICAL:** 4 | **HIGH:** 102 | **MEDIUM:** 39 | **LOW:** 287

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 260 |
| eval() or exec() usage | 60 |
| GS008 | 27 |
| Bare except: | 18 |
| CVE-2026-56233: Path traversal | 17 |
| Python: assert in production | 15 |
| CVE-2026-56233: Privilege escalation | 11 |
| GS004 | 7 |
| CVE-2026-37270: Hardcoded credential | 5 |
| GS015 | 3 |
| Хардкод IP адреса | 2 |
| CVE-2026-55223: Insecure deserialization | 1 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 1 |
| CVE-2026-56413: Command injection | 1 |
| GS001 | 1 |
| Hardcoded encryption key | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: appveyor.yml (664) | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .travis.yml (664) | 1 |
| GS009 | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | readline_shell.py | 655 |  |
| CRITICAL | GS001 | config.py | 301 | Found: Password: ')
                login_kwargs.update({' |
| CRITICAL | ? | formatter.py | 259 | Match:         item += self._format_issue_comment(event, key |
| CRITICAL | ? | man.py | 36 | Match:                 OPTIONS = pickle.load(f) |
| HIGH | ? | calc.py | 9 |  |
| HIGH | ? | hedit.py | 18 |  |
| HIGH | ? | GardenSnake.py | 40 |  |
| HIGH | ? | calc.py | 9 |  |
| HIGH | ? | ylex.py | 7 |  |
| HIGH | ? | yply.py | 24 |  |
| HIGH | ? | calc.py | 9 |  |
| HIGH | ? | basiclog.py | 5 |  |
| HIGH | ? | basic.py | 5 |  |
| HIGH | ? | calc.py | 11 |  |
| HIGH | ? | calc.py | 9 |  |
| HIGH | ? | calc.py | 15 |  |
| HIGH | ? | clex.py | 8 |  |
| HIGH | ? | calc.py | 10 |  |
| HIGH | ? | calc.py | 13 |  |
| HIGH | ? | bash_completion.py | 295 |  |
| HIGH | ? | _which.py | 58 |  |
| HIGH | ? | winutils.py | 47 |  |
| HIGH | ? | winutils.py | 132 |  |
| HIGH | ? | commands.py | 9 |  |
| HIGH | ? | commands_cache.py | 426 |  |
| HIGH | ? | job.py | 13 |  |
| HIGH | ? | aliases.py | 719 |  |
| HIGH | ? | aliases.py | 791 |  |
| HIGH | ? | aliases.py | 794 |  |
| HIGH | ? | aliases.py | 802 |  |
| HIGH | ? | aliases.py | 805 |  |
| HIGH | ? | aliases.py | 810 |  |
| HIGH | ? | web_viewer.py | 114 |  |
| HIGH | ? | jupyter_kernel.py | 107 | Match:                 "ip": "127.0.0.1", |
| HIGH | ? | xontribs.json | 71 | Match:     "    with dsubmit('127.0.0.1:8786', rtn='x') as d |
| HIGH | ? | lex.py | 217 | Match:             exec('import %s' % tabfile) |
| HIGH | ? | lex.py | 1038 | Match:                     exec('import %s' % pkgname) |
| HIGH | ? | cpp.py | 656 | Match:             result = eval(expr) |
| HIGH | ? | hedit.py | 32 | Match:     n = eval(t.value[:i]) |
| HIGH | ? | basparse.py | 318 | Match:     p[0] = (p[1], eval(p[3]), 0) |
| HIGH | ? | basparse.py | 323 | Match:     p[0] = (p[1], eval(p[3]), eval(p[5])) |
| HIGH | ? | basparse.py | 341 | Match:     p[0] = ('NUM', eval(p[1])) |
| HIGH | ? | basparse.py | 415 | Match:     p[0] = eval(p[1]) |
| HIGH | ? | basparse.py | 423 | Match:     p[0] = eval("-" + p[2]) |
| HIGH | ? | basinterp.py | 17 | Match:             'SIN': lambda z: math.sin(self.eval(z)), |
| HIGH | ? | basinterp.py | 18 | Match:             'COS': lambda z: math.cos(self.eval(z)), |
| HIGH | ? | basinterp.py | 19 | Match:             'TAN': lambda z: math.tan(self.eval(z)), |
| HIGH | ? | basinterp.py | 20 | Match:             'ATN': lambda z: math.atan(self.eval(z)), |
| HIGH | ? | basinterp.py | 21 | Match:             'EXP': lambda z: math.exp(self.eval(z)), |
| HIGH | ? | basinterp.py | 22 | Match:             'ABS': lambda z: abs(self.eval(z)), |
| HIGH | ? | basinterp.py | 23 | Match:             'LOG': lambda z: math.log(self.eval(z)), |
| HIGH | ? | basinterp.py | 24 | Match:             'SQR': lambda z: math.sqrt(self.eval(z)), |
| HIGH | ? | basinterp.py | 25 | Match:             'INT': lambda z: int(self.eval(z)), |
| HIGH | ? | basinterp.py | 70 | Match:     def eval(self, expr): |
| HIGH | ? | basinterp.py | 75 | Match:             return self.eval(expr[1]) |
| HIGH | ? | basinterp.py | 78 | Match:                 return -self.eval(expr[2]) |
| HIGH | ? | basinterp.py | 81 | Match:                 return self.eval(expr[2]) + self.eval |
| HIGH | ? | basinterp.py | 83 | Match:                 return self.eval(expr[2]) - self.eval |
| HIGH | ? | basinterp.py | 85 | Match:                 return self.eval(expr[2]) * self.eval |
| HIGH | ? | basinterp.py | 87 | Match:                 return float(self.eval(expr[2])) / se |
| HIGH | ? | basinterp.py | 89 | Match:                 return abs(self.eval(expr[2]))**self. |
| HIGH | ? | basinterp.py | 107 | Match:                         dim1val = self.eval(dim1) |
| HIGH | ? | basinterp.py | 115 | Match:                     dim1val = self.eval(dim1) |
| HIGH | ? | basinterp.py | 116 | Match:                     dim2val = self.eval(dim2) |
| HIGH | ? | basinterp.py | 129 | Match:         lhs = self.eval(expr[2]) |
| HIGH | ? | basinterp.py | 130 | Match:         rhs = self.eval(expr[3]) |
| HIGH | ? | basinterp.py | 171 | Match:             self.vars[var] = self.eval(value) |
| HIGH | ? | basinterp.py | 174 | Match:             dim1val = self.eval(dim1) |
| HIGH | ? | basinterp.py | 181 | Match:             self.lists[var][dim1val - 1] = self.eval( |
| HIGH | ? | basinterp.py | 183 | Match:             dim1val = self.eval(dim1) |
| HIGH | ? | basinterp.py | 184 | Match:             dim2val = self.eval(dim2) |
| HIGH | ? | basinterp.py | 195 | Match:             self.tables[var][dim1val - 1][dim2val - 1 |
| HIGH | ? | basinterp.py | 255 | Match:                         eval = self.eval(val) |
| HIGH | ? | basinterp.py | 302 | Match:                     stepval = self.eval(stepval)    # |
| HIGH | ? | basinterp.py | 359 | Match:                     return self.eval(expr) |
| HIGH | ? | testyacc.py | 76 | Match:     exec(code) |
| HIGH | ? | lex_hedit.py | 31 | Match:     n = eval(t.value[:i]) |
| HIGH | ? | lex_many_tokens.py | 15 | Match:         exec("t_%s = '%s:'" % (tok,tok)) |
| HIGH | ? | lex_many_tokens.py | 17 | Match:         exec("t_%s = '%s:'" % (tok,tok), globals()) |
| HIGH | ? | testlex.py | 83 | Match:     exec(code) |
| HIGH | ? | pygments_cache.py | 275 | Match:     CACHE = eval(s, ctx, ctx) |
| HIGH | ? | base.py | 246 | Match:             eval_field = "__xonsh__.execer.eval(r" +  |
| HIGH | ? | execer.py | 141 | Match:     def eval( |
| HIGH | ? | execer.py | 161 | Match:         return eval(code, glbs, locs) |
| HIGH | ? | execer.py | 163 | Match:     def exec( |
| HIGH | ? | execer.py | 190 | Match:         return exec(code, glbs, locs) |
| HIGH | ? | shortcuts.py | 96 | Match:             exec( |
| HIGH | ? | contexts.py | 97 | Match:         execer.exec(fstr, glbs=glbs, locs=locs) |
| HIGH | ? | built_ins.py | 1109 | Match:         arg = execer.eval(raw_arg, glbs=glbs, locs=lo |
| HIGH | ? | built_ins.py | 1114 | Match:         arg = execer.exec(raw_arg, mode=mode, glbs=gl |
| HIGH | ? | built_ins.py | 1116 | Match:         arg = type(execer.eval(raw_arg, glbs=glbs, lo |
| HIGH | ? | built_ins.py | 1210 | Match:         kwargs = execer.eval(kwargstr, glbs=glbs, loc |
| HIGH | ? | built_ins.py | 1213 | Match:         args = execer.eval(argstr, glbs=glbs, locs=lo |
| HIGH | ? | built_ins.py | 1219 | Match:         args, kwargs = execer.eval(both, glbs=glbs, l |
| HIGH | ? | aliases.py | 188 | Match:         execer.exec( |
| HIGH | ? | appveyor.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .travis.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | aliases.py | 188 | Line 188: execer.exec( |
| HIGH | GS004 | aliases.py | 609 | Line 609: def xexec(args, stdin=None): |
| HIGH | GS004 | built_ins.py | 1114 | Line 1114: arg = execer.exec(raw_arg, mode=mode, glbs=glbs,  |
| HIGH | GS004 | contexts.py | 97 | Line 97: execer.exec(fstr, glbs=glbs, locs=locs) |
| HIGH | GS004 | execer.py | 163 | Line 163: def exec( |
| HIGH | GS004 | execer.py | 190 | Line 190: return exec(code, glbs, locs) |
| HIGH | GS004 | shortcuts.py | 96 | Line 96: exec( |
| HIGH | ? | cpp.py | 310 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | web_viewer.py | 45 |
| M | ? | utils.py | 185 |
| M | ? | inspectors.py | 289 |
| M | ? | inspectors.py | 323 |
| M | ? | inspectors.py | 359 |
| M | ? | inspectors.py | 429 |
| M | ? | inspectors.py | 652 |
| M | ? | inspectors.py | 666 |
| M | ? | inspectors.py | 675 |
| M | ? | inspectors.py | 756 |
| M | ? | calc.py | 38 |
| M | ? | calc.py | 36 |
| M | ? | CHANGES | 499 |
| M | ? | python.py | 196 |
| M | ? | python.py | 200 |
| M | ? | tty.py | 24 |
| M | ? | tty.py | 33 |
| M | ? | tee.py | 29 |
| M | ? | GardenSnake.py | 203 |
| M | ? | GardenSnake.py | 261 |
| M | ? | GardenSnake.py | 312 |
| M | ? | tokenize.py | 1002 |
| M | ? | base.py | 1028 |
| M | ? | base.py | 1197 |
| M | ? | base.py | 1527 |
| M | ? | base.py | 1872 |
| M | ? | base.py | 2237 |
| M | ? | base.py | 2918 |
| M | ? | v34.py | 66 |
| M | ? | v34.py | 122 |
| M | ? | v34.py | 156 |
| M | ? | python.py | 69 |
| M | ? | built_ins.py | 757 |
| M | ? | man.py | 36 |
| H | ? | calc.py | 9 |
| H | ? | hedit.py | 18 |
| H | ? | GardenSnake.py | 40 |
| H | ? | calc.py | 9 |
| H | ? | ylex.py | 7 |
| H | ? | yply.py | 24 |
| H | ? | calc.py | 9 |
| H | ? | basiclog.py | 5 |
| H | ? | basic.py | 5 |
| H | ? | calc.py | 11 |
| H | ? | calc.py | 9 |
| H | ? | calc.py | 15 |
| H | ? | clex.py | 8 |
| H | ? | calc.py | 10 |
| H | ? | calc.py | 13 |
| H | ? | bash_completion.py | 295 |
| H | ? | _which.py | 58 |
| H | ? | winutils.py | 47 |
| H | ? | winutils.py | 132 |
| H | ? | commands.py | 9 |
| H | ? | commands_cache.py | 426 |
| H | ? | job.py | 13 |
| H | ? | aliases.py | 719 |
| H | ? | aliases.py | 791 |
| H | ? | aliases.py | 794 |
| H | ? | aliases.py | 802 |
| H | ? | aliases.py | 805 |
| H | ? | aliases.py | 810 |
| H | ? | web_viewer.py | 114 |
| C | ? | readline_shell.py | 655 |
| M | ? | formatter.py | 229 |
| M | ? | formatter.py | 245 |
| M | ? | formatter.py | 259 |
| M | ? | readline_shell.py | 294 |
| M | ? | _which.py | 116 |
| C | GS001 | config.py | 301 |
| L | GS003 | aliases.py | 331 |
| L | GS003 | aliases.py | 536 |
| L | GS003 | aliases.py | 553 |
| L | GS003 | aliases.py | 697 |
| L | GS003 | aliases.py | 796 |
| L | GS003 | aliases.py | 808 |
| L | GS003 | ansi_colors.py | 61 |
| L | GS003 | ast.py | 449 |
| L | GS003 | ast.py | 653 |
| L | GS003 | base_shell.py | 365 |
| L | GS003 | base_shell.py | 382 |
| L | GS003 | base_shell.py | 570 |
| L | GS003 | bash_completion.py | 449 |
| L | GS003 | environ.py | 650 |
| L | GS003 | execer.py | 202 |
| L | GS003 | foreign_shells.py | 268 |
| L | GS003 | foreign_shells.py | 712 |
| L | GS003 | json.py | 411 |
| L | GS003 | main.py | 33 |
| L | GS003 | main.py | 89 |
| L | GS003 | main.py | 117 |
| L | GS003 | main.py | 188 |
| L | GS003 | main.py | 196 |
| L | GS003 | main.py | 203 |
| L | GS003 | main.py | 207 |
| L | GS003 | main.py | 212 |
| L | GS003 | main.py | 394 |
| L | GS003 | main.py | 397 |
| L | GS003 | main.py | 401 |
| L | GS003 | main.py | 405 |
| L | GS003 | main.py | 417 |
| L | GS003 | sqlite.py | 158 |
| L | GS003 | inspectors.py | 364 |
| L | GS003 | inspectors.py | 366 |
| L | GS003 | inspectors.py | 368 |
| L | GS003 | inspectors.py | 377 |
| L | GS003 | inspectors.py | 390 |
| L | GS003 | inspectors.py | 421 |
| L | GS003 | inspectors.py | 432 |
| L | GS003 | inspectors.py | 446 |
| L | GS003 | inspectors.py | 448 |
| L | GS003 | inspectors.py | 454 |
| L | GS003 | jobs.py | 209 |
| L | GS003 | jobs.py | 213 |
| L | GS003 | jobs.py | 264 |
| L | GS003 | jobs.py | 323 |
| L | GS003 | jobs.py | 324 |
| L | GS003 | jobs.py | 325 |
| L | GS003 | jobs.py | 327 |
| L | GS003 | jobs.py | 328 |
| L | GS003 | jupyter_kernel.py | 199 |
| L | GS003 | main.py | 265 |
| L | GS003 | main.py | 324 |
| L | GS003 | main.py | 341 |
| L | GS003 | main.py | 394 |
| L | GS003 | main.py | 395 |
| L | GS003 | main.py | 452 |
| L | GS003 | basiclex.py | 58 |
| L | GS003 | basinterp.py | 44 |
| L | GS003 | basinterp.py | 48 |
| L | GS003 | basinterp.py | 66 |
| L | GS003 | basinterp.py | 96 |
| L | GS003 | basinterp.py | 109 |
| L | GS003 | basinterp.py | 118 |
| L | GS003 | basinterp.py | 122 |
| L | GS003 | basinterp.py | 179 |
| L | GS003 | basinterp.py | 193 |
| L | GS003 | basinterp.py | 200 |
| L | GS003 | basinterp.py | 325 |
| L | GS003 | basinterp.py | 333 |
| L | GS003 | basinterp.py | 339 |
| L | GS003 | basinterp.py | 347 |
| L | GS003 | basinterp.py | 411 |
| L | GS003 | basinterp.py | 414 |
| L | GS003 | basinterp.py | 430 |
| L | GS003 | basinterp.py | 432 |
| L | GS003 | basinterp.py | 442 |
| L | GS003 | basinterp.py | 444 |
| L | GS003 | basinterp.py | 447 |
| L | GS003 | basinterp.py | 453 |
| L | GS003 | basinterp.py | 455 |
| L | GS003 | basinterp.py | 457 |
| L | GS003 | basinterp.py | 470 |
| L | GS003 | basinterp.py | 480 |
| L | GS003 | basparse.py | 51 |
| L | GS003 | basparse.py | 79 |
| L | GS003 | basparse.py | 464 |
| L | GS003 | GardenSnake.py | 731 |
| L | GS003 | GardenSnake.py | 736 |
| L | GS003 | GardenSnake.py | 747 |
| L | GS003 | GardenSnake.py | 750 |
| L | GS003 | GardenSnake.py | 751 |
| L | GS003 | GardenSnake.py | 756 |
| L | GS003 | GardenSnake.py | 757 |
| L | GS003 | GardenSnake.py | 759 |
| L | GS003 | GardenSnake.py | 760 |
| L | GS003 | GardenSnake.py | 761 |
| L | GS003 | GardenSnake.py | 762 |
| L | GS003 | clex.py | 163 |
| L | GS003 | cparse.py | 1040 |
| L | GS003 | calc.py | 39 |
| L | GS003 | calc.py | 65 |
| L | GS003 | calc.py | 103 |
| L | GS003 | calc.py | 109 |
| L | GS003 | calc.py | 111 |
| L | GS003 | calc.py | 39 |
| L | GS003 | calc.py | 65 |
| L | GS003 | calc.py | 103 |
| L | GS003 | calc.py | 109 |
| L | GS003 | calc.py | 111 |
| L | GS003 | calc.py | 48 |
| L | GS003 | calc.py | 74 |
| L | GS003 | calc.py | 112 |
| L | GS003 | calc.py | 118 |
| L | GS003 | calc.py | 120 |
| L | GS003 | calc.py | 85 |
| L | GS003 | calc.py | 97 |
| L | GS003 | calc.py | 115 |
| L | GS003 | calc.py | 154 |
| L | GS003 | calc.py | 159 |
| L | GS003 | calc.py | 161 |
| L | GS003 | calc.py | 48 |
| L | GS003 | calc.py | 102 |
| L | GS003 | calc.py | 107 |
| L | GS003 | calc.py | 109 |
| L | GS003 | calc.py | 132 |
| L | GS003 | hedit.py | 42 |
| L | GS003 | calc.py | 87 |
| L | GS003 | calc.py | 99 |
| L | GS003 | calc.py | 117 |
| L | GS003 | calc.py | 156 |
| L | GS003 | calc.py | 161 |
| L | GS003 | calc.py | 163 |
| L | GS003 | calc.py | 37 |
| L | GS003 | calc.py | 50 |
| L | GS003 | calc.py | 76 |
| L | GS003 | calc.py | 116 |
| L | GS003 | calc.py | 122 |
| L | GS003 | calc.py | 124 |
| L | GS003 | ylex.py | 112 |
| L | GS003 | ylex.py | 113 |
| L | GS003 | yparse.py | 25 |
| L | GS003 | yparse.py | 26 |
| L | GS003 | yparse.py | 27 |
| L | GS003 | yparse.py | 28 |
| L | GS003 | yparse.py | 29 |
| L | GS003 | yparse.py | 30 |
| L | GS003 | yparse.py | 35 |
| L | GS003 | yparse.py | 52 |
| L | GS003 | yparse.py | 141 |
| L | GS003 | yparse.py | 158 |
| L | GS003 | yparse.py | 161 |
| L | GS003 | yparse.py | 165 |
| L | GS003 | yparse.py | 166 |
| L | GS003 | yparse.py | 168 |
| L | GS003 | yparse.py | 244 |
| L | GS003 | yply.py | 32 |
| L | GS003 | yply.py | 39 |
| L | GS003 | yply.py | 46 |
| L | GS003 | cpp.py | 226 |
| L | GS003 | cpp.py | 243 |
| L | GS003 | cpp.py | 251 |
| L | GS003 | cpp.py | 260 |
| L | GS003 | cpp.py | 277 |
| L | GS003 | cpp.py | 289 |
| L | GS003 | cpp.py | 814 |
| L | GS003 | cpp.py | 822 |
| L | GS003 | cpp.py | 839 |
| L | GS003 | cpp.py | 884 |
| L | GS003 | cpp.py | 903 |
| L | GS003 | cpp.py | 920 |
| L | GS003 | cpp.py | 922 |
| L | GS003 | cpp.py | 974 |
| L | GS003 | ygen.py | 65 |
| L | GS003 | proc.py | 2242 |
| L | GS003 | base.py | 84 |
| L | GS003 | env.py | 53 |
| L | GS003 | vc.py | 122 |
| L | GS003 | shell.py | 171 |
| L | GS003 | shell.py | 186 |
| L | GS003 | shell.py | 281 |
| L | GS003 | shell.py | 180 |
| L | GS003 | shell.py | 195 |
| L | GS003 | shell.py | 289 |
| L | GS003 | pyghooks.py | 453 |
| L | GS003 | pygments_cache.py | 33 |
| L | GS003 | pygments_cache.py | 300 |
| L | GS003 | pygments_cache.py | 303 |
| L | GS003 | readline_shell.py | 77 |
| L | GS003 | readline_shell.py | 126 |
| L | GS003 | readline_shell.py | 268 |
| L | GS003 | readline_shell.py | 381 |
| L | GS003 | readline_shell.py | 393 |
| L | GS003 | readline_shell.py | 395 |
| L | GS003 | readline_shell.py | 397 |
| L | GS003 | readline_shell.py | 401 |
| L | GS003 | readline_shell.py | 575 |
| L | GS003 | readline_shell.py | 626 |
| L | GS003 | replay.py | 129 |
| L | GS003 | replay.py | 130 |
| L | GS003 | replay.py | 131 |
| L | GS003 | replay.py | 135 |
| L | GS003 | replay.py | 138 |
| L | GS003 | timings.py | 231 |
| L | GS003 | timings.py | 238 |
| L | GS003 | timings.py | 244 |
| L | GS003 | timings.py | 329 |
| L | GS003 | timings.py | 330 |
| L | GS003 | timings.py | 331 |
| L | GS003 | timings.py | 332 |
| L | GS003 | timings.py | 335 |
| L | GS003 | timings.py | 337 |
| L | GS003 | tokenize.py | 1150 |
| L | GS003 | tokenize.py | 1195 |
| L | GS003 | tokenize.py | 1207 |
| L | GS003 | tools.py | 2378 |
| L | GS003 | tracer.py | 156 |
| L | GS003 | wizard.py | 763 |
| L | GS003 | wizard.py | 796 |
| L | GS003 | wizard.py | 843 |
| L | GS003 | xonfig.py | 468 |
| L | GS003 | xonfig.py | 536 |
| L | GS003 | xonfig.py | 599 |
| L | GS003 | xontribs.py | 50 |
| L | GS003 | xontribs.py | 89 |
| L | GS003 | xontribs.py | 123 |
| L | GS003 | _which.py | 322 |
| L | GS003 | _which.py | 325 |
| L | GS003 | _which.py | 355 |
| L | GS003 | _which.py | 357 |
| L | GS003 | cat.py | 45 |
| L | GS003 | cat.py | 48 |
| L | GS003 | cat.py | 76 |
| L | GS003 | cat.py | 79 |
| L | GS003 | cat.py | 90 |
| L | GS003 | echo.py | 10 |
| L | GS003 | echo.py | 16 |
| L | GS003 | pwd.py | 9 |
| L | GS003 | pwd.py | 13 |
| L | GS003 | tee.py | 14 |
| L | GS003 | tee.py | 18 |
| L | GS003 | tee.py | 30 |
| L | GS003 | tty.py | 9 |
| L | GS003 | tty.py | 19 |
| L | GS003 | tty.py | 20 |
| L | GS003 | tty.py | 28 |
| L | GS003 | tty.py | 32 |
| L | GS003 | which.py | 79 |
| L | GS003 | which.py | 93 |
| L | GS003 | which.py | 96 |
| L | GS003 | which.py | 103 |
| L | GS003 | which.py | 105 |
| L | GS003 | which.py | 107 |
| L | GS003 | which.py | 167 |
| L | GS003 | which.py | 169 |
| L | GS003 | which.py | 170 |
| L | GS003 | which.py | 172 |
| L | GS003 | which.py | 173 |
| L | GS003 | yes.py | 7 |
| L | GS003 | yes.py | 13 |
| L | GS008 | completions_git.py | 16 |
| L | GS008 | completions_git.py | 200 |
| L | GS008 | jupyter_kernel.py | 26 |
| L | GS008 | platform.py | 22 |
| L | GS008 | platform.py | 23 |
| L | GS008 | platform.py | 24 |
| L | GS008 | platform.py | 271 |
| L | GS008 | platform.py | 272 |
| L | GS008 | platform.py | 273 |
| L | GS008 | platform.py | 274 |
| L | GS008 | platform.py | 275 |
| L | GS008 | platform.py | 276 |
| L | GS008 | platform.py | 306 |
| L | GS008 | readline_shell.py | 54 |
| L | GS008 | style_tools.py | 437 |
| L | GS008 | tools.py | 2355 |
| L | GS008 | winutils.py | 66 |
| L | GS008 | winutils.py | 168 |
| L | GS008 | winutils.py | 169 |
| L | GS008 | winutils.py | 170 |
| L | GS008 | winutils.py | 171 |
| L | GS008 | winutils.py | 172 |
| L | GS008 | winutils.py | 173 |
| L | GS008 | winutils.py | 174 |
| L | GS008 | winutils.py | 177 |
| L | GS008 | winutils.py | 178 |
| L | GS008 | winutils.py | 179 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| H | ? | jupyter_kernel.py | 107 |
| H | ? | xontribs.json | 71 |
| C | ? | formatter.py | 259 |
| H | ? | lex.py | 217 |
| H | ? | lex.py | 1038 |
| H | ? | cpp.py | 656 |
| H | ? | hedit.py | 32 |
| H | ? | basparse.py | 318 |
| H | ? | basparse.py | 323 |
| H | ? | basparse.py | 341 |
| H | ? | basparse.py | 415 |
| H | ? | basparse.py | 423 |
| H | ? | basinterp.py | 17 |
| H | ? | basinterp.py | 18 |
| H | ? | basinterp.py | 19 |
| H | ? | basinterp.py | 20 |
| H | ? | basinterp.py | 21 |
| H | ? | basinterp.py | 22 |
| H | ? | basinterp.py | 23 |
| H | ? | basinterp.py | 24 |
| H | ? | basinterp.py | 25 |
| H | ? | basinterp.py | 70 |
| H | ? | basinterp.py | 75 |
| H | ? | basinterp.py | 78 |
| H | ? | basinterp.py | 81 |
| H | ? | basinterp.py | 83 |
| H | ? | basinterp.py | 85 |
| H | ? | basinterp.py | 87 |
| H | ? | basinterp.py | 89 |
| H | ? | basinterp.py | 107 |
| H | ? | basinterp.py | 115 |
| H | ? | basinterp.py | 116 |
| H | ? | basinterp.py | 129 |
| H | ? | basinterp.py | 130 |
| H | ? | basinterp.py | 171 |
| H | ? | basinterp.py | 174 |
| H | ? | basinterp.py | 181 |
| H | ? | basinterp.py | 183 |
| H | ? | basinterp.py | 184 |
| H | ? | basinterp.py | 195 |
| H | ? | basinterp.py | 255 |
| H | ? | basinterp.py | 302 |
| H | ? | basinterp.py | 359 |
| H | ? | testyacc.py | 76 |
| H | ? | lex_hedit.py | 31 |
| H | ? | lex_many_tokens.py | 15 |
| H | ? | lex_many_tokens.py | 17 |
| H | ? | testlex.py | 83 |
| H | ? | pygments_cache.py | 275 |
| H | ? | base.py | 246 |
| H | ? | execer.py | 141 |
| H | ? | execer.py | 161 |
| H | ? | execer.py | 163 |
| H | ? | execer.py | 190 |
| H | ? | shortcuts.py | 96 |
| H | ? | contexts.py | 97 |
| H | ? | built_ins.py | 1109 |
| H | ? | built_ins.py | 1114 |
| H | ? | built_ins.py | 1116 |
| H | ? | built_ins.py | 1210 |
| H | ? | built_ins.py | 1213 |
| H | ? | built_ins.py | 1219 |
| H | ? | aliases.py | 188 |
| C | ? | man.py | 36 |
| H | ? | appveyor.yml | 0 |
| H | ? | codecov.yml | 0 |
| H | ? | .travis.yml | 0 |
| H | GS004 | aliases.py | 188 |
| H | GS004 | aliases.py | 609 |
| H | GS004 | built_ins.py | 1114 |
| H | GS004 | contexts.py | 97 |
| H | GS004 | execer.py | 163 |
| H | GS004 | execer.py | 190 |
| H | GS004 | shortcuts.py | 96 |
| s | GS009 |  | 0 |
| H | ? | cpp.py | 310 |

---
*Сгенерировано GSC v0.6 · 2026-07-11T13:49:55.663906*