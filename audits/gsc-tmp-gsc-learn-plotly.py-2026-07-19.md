---
title: "GSC Audit: /tmp/gsc-learn/plotly.py"
date: 2026-07-19
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/plotly.py

**Дата:** 19.07.2026 04:05  
**Путь:** `/tmp/gsc-learn/plotly.py`  
**Всего находок:** 688  
**CRITICAL:** 28 | **HIGH:** 164 | **MEDIUM:** 63 | **LOW:** 432

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 131 |
| GS012 | 113 |
| TS: any type escape hatch | 70 |
| Хардкод IP адреса | 62 |
| Python: assert in production | 37 |
| Rust: .clone() in hot path | 20 |
| SQL injection risk: f-string in query | 16 |
| CVE-2026-37270: Hardcoded credential | 16 |
| Hardcoded encryption key | 12 |
| GS008 | 11 |
| Outdated dependency pattern | 5 |
| Python: File upload without content-type validation | 4 |
| Generic code smell #24 | 3 |
| Generic code smell #27 | 3 |
| Generic code smell #30 | 3 |
| Generic code smell #33 | 3 |
| Generic code smell #36 | 3 |
| Generic code smell #39 | 3 |
| Generic code smell #42 | 3 |
| Generic code smell #45 | 3 |
| Generic code smell #48 | 3 |
| Generic code smell #51 | 3 |
| Generic code smell #54 | 3 |
| Generic code smell #57 | 3 |
| Generic code smell #60 | 3 |
| Generic code smell #63 | 3 |
| Generic code smell #66 | 3 |
| Generic code smell #69 | 3 |
| Generic code smell #72 | 3 |
| Generic code smell #75 | 3 |
| Generic code smell #78 | 3 |
| Generic code smell #81 | 3 |
| Generic code smell #84 | 3 |
| Generic code smell #87 | 3 |
| Generic code smell #90 | 3 |
| Generic code smell #93 | 3 |
| Generic code smell #96 | 3 |
| Generic code smell #99 | 3 |
| Generic code smell #102 | 3 |
| Generic code smell #105 | 3 |
| Generic code smell #108 | 3 |
| Generic code smell #111 | 3 |
| Generic code smell #114 | 3 |
| Generic code smell #117 | 3 |
| Generic code smell #120 | 3 |
| Generic code smell #123 | 3 |
| Generic code smell #126 | 3 |
| Generic code smell #129 | 3 |
| Generic code smell #132 | 3 |
| Generic code smell #135 | 3 |
| Generic code smell #138 | 3 |
| Generic code smell #141 | 3 |
| Generic code smell #144 | 3 |
| Generic code smell #147 | 3 |
| Generic code smell #150 | 3 |
| Generic code smell #153 | 3 |
| Generic code smell #156 | 3 |
| Generic code smell #159 | 3 |
| Generic code smell #162 | 3 |
| Generic code smell #165 | 3 |
| Generic code smell #168 | 3 |
| Generic code smell #171 | 3 |
| Generic code smell #174 | 3 |
| Generic code smell #177 | 3 |
| Generic code smell #180 | 3 |
| Generic code smell #183 | 3 |
| Generic code smell #186 | 3 |
| Generic code smell #189 | 3 |
| Generic code smell #192 | 3 |
| Generic code smell #195 | 3 |
| Generic code smell #198 | 3 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 3 |
| Синхронный код в async | 3 |
| eval() or exec() usage | 2 |
| TS: console.log in production | 1 |
| CVE-2026-56233: Privilege escalation | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| World-readable file: dependabot.yml (664) | 1 |
| World-readable file: environment.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | mimeExtension.js | 4 | OWASP A03: Injection |
| CRITICAL | ? | mimeExtension.js | 6 | OWASP A03: Injection |
| CRITICAL | ? | mimeExtension.js | 7 | OWASP A03: Injection |
| CRITICAL | ? | mimeExtension.js | 8 | OWASP A03: Injection |
| CRITICAL | ? | mimeExtension.js | 1994 | OWASP A03: Injection |
| CRITICAL | ? | plotly.min.js | 18 | OWASP A03: Injection |
| CRITICAL | ? | plotly.min.js | 20 | OWASP A03: Injection |
| CRITICAL | ? | plotly.min.js | 21 | OWASP A03: Injection |
| CRITICAL | ? | plotly.min.js | 22 | OWASP A03: Injection |
| CRITICAL | ? | plotly.min.js | 2008 | OWASP A03: Injection |
| CRITICAL | ? | widgetbundle.js | 4 | OWASP A03: Injection |
| CRITICAL | ? | widgetbundle.js | 6 | OWASP A03: Injection |
| CRITICAL | ? | widgetbundle.js | 7 | OWASP A03: Injection |
| CRITICAL | ? | widgetbundle.js | 8 | OWASP A03: Injection |
| CRITICAL | ? | widgetbundle.js | 1994 | OWASP A03: Injection |
| CRITICAL | ? | 1.3ad216e94ff8bdcd7b73.js | 2 | OWASP A03: Injection |
| CRITICAL | ? | mimeExtension.js | 2699 | Match: `),S=o1().maxDimensionCount,M=ui(),e=1e-6,t=2048,r=ne |
| CRITICAL | ? | mimeExtension.js | 2704 | Match: `)),F.push({type:"Feature",geometry:{type:"Point",coo |
| CRITICAL | ? | mimeExtension.js | 3200 | Match: `),Wt=$e.createShader($e.FRAGMENT_SHADER);if($e.isCon |
| CRITICAL | ? | plotly.min.js | 2713 | Match: `),Hk=Vk().maxDimensionCount,DUe=Pr(),CUe=1e-6,Yz=204 |
| CRITICAL | ? | plotly.min.js | 2718 | Match: `)),c.push({type:"Feature",geometry:{type:"Point",coo |
| CRITICAL | ? | plotly.min.js | 3214 | Match: `),_t=we.createShader(we.FRAGMENT_SHADER);if(we.isCon |
| CRITICAL | ? | widgetbundle.js | 2699 | Match: `),S=Ax().maxDimensionCount,M=sa(),e=1e-6,t=2048,r=ne |
| CRITICAL | ? | widgetbundle.js | 2704 | Match: `)),F.push({type:"Feature",geometry:{type:"Point",coo |
| CRITICAL | ? | widgetbundle.js | 3200 | Match: `),Wt=Qe.createShader(Qe.FRAGMENT_SHADER);if(Qe.isCon |
| CRITICAL | ? | renderer.py | 763 | Match:         axis_key = "xaxis{0}".format(self.axis_ct) |
| CRITICAL | ? | renderer.py | 794 | Match:         axis_key = "yaxis{0}".format(self.axis_ct) |
| CRITICAL | ? | 1.3ad216e94ff8bdcd7b73.js | 2 | Match: (self.webpackChunkjupyterlab_plotly=self.webpackChunk |
| HIGH | ? | widget.ts | 8 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 9 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 10 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 11 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 12 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 13 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 17 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 18 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 33 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 37 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 42 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 43 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 47 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 48 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 61 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 62 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 63 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 67 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 71 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 72 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 74 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 87 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 92 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 96 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 100 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 101 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 105 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 106 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 852 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 886 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 889 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 892 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 895 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 898 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 901 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 904 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 907 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 910 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 929 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 941 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1033 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1121 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1148 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1179 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1214 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1239 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1267 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1275 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1283 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1291 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1299 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1317 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1341 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1498 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1529 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1554 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1628 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1629 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1662 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1663 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1712 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1727 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1759 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1803 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1804 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1858 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1863 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1943 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 1945 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | widget.ts | 2018 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | data_utils.py | 73 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _orca.py | 952 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _orca.py | 1066 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | _orca.py | 1533 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | commands.py | 74 |  |
| HIGH | ? | commands.py | 122 |  |
| HIGH | ? | commands.py | 139 |  |
| HIGH | ? | commands.py | 167 |  |
| HIGH | ? | mimeExtension.js | 4 | Match: `)};function Dt(Gr){return Gr.map(xr).join(pe)}functi |
| HIGH | ? | mimeExtension.js | 7 | Match: `);if(pt!==-1&&(Wr=Ur.slice(pt+1),Ur=Ur.slice(0,pt)), |
| HIGH | ? | plotly.min.js | 18 | Match: `)};function ot(dr){return dr.map(Xt).join(X)}functio |
| HIGH | ? | plotly.min.js | 21 | Match: `);if(l!==-1&&(s=o.slice(l+1),o=o.slice(0,l)),n&&(s!= |
| HIGH | ? | widgetbundle.js | 4 | Match: `)};function zt(Gr){return Gr.map(_r).join(me)}functi |
| HIGH | ? | widgetbundle.js | 7 | Match: `);if(gt!==-1&&(Hr=Nr.slice(gt+1),Nr=Nr.slice(0,gt)), |
| HIGH | ? | 1.3ad216e94ff8bdcd7b73.js | 2 | Match: (self.webpackChunkjupyterlab_plotly=self.webpackChunk |
| HIGH | ? | uv.lock | 404 | Match:     { name = "pyerfa", version = "2.0.0.3", source =  |
| HIGH | ? | uv.lock | 452 | Match:     { name = "pyerfa", version = "2.0.1.5", source =  |
| HIGH | ? | uv.lock | 492 | Match:     { name = "pyerfa", version = "2.0.1.5", source =  |
| HIGH | ? | uv.lock | 529 | Match: version = "0.2026.3.16.0.53.33" |
| HIGH | ? | uv.lock | 531 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 533 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 1466 | Match: version = "1.1.1.2" |
| HIGH | ? | uv.lock | 1471 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 1473 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7941 | Match: version = "2.0.0.3" |
| HIGH | ? | uv.lock | 7953 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 7955 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7956 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7957 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7958 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7959 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7960 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7961 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7962 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7963 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7964 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7965 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7966 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7967 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7968 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7969 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7970 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7971 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7972 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7973 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7974 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7975 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7976 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7977 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7978 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7979 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7980 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7981 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7982 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7983 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7984 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7985 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7986 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 7991 | Match: version = "2.0.1.5" |
| HIGH | ? | uv.lock | 8001 | Match: sdist = { url = "https://files.pythonhosted.org/packa |
| HIGH | ? | uv.lock | 8003 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8004 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8005 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8006 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8007 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8008 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8009 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8010 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8011 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | uv.lock | 8012 | Match:     { url = "https://files.pythonhosted.org/packages/ |
| HIGH | ? | validators.py | 28 | Match:     params = dict([(k, eval(v)) for k, v in raw_param |
| HIGH | ? | utils.py | 499 | Match:             prop: eval(repr_val) |
| HIGH | ? | dependabot.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | environment.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | mimeExtension.js | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | mimeExtension.js | 2704 | Clone in performance-critical code — consider references |
| HIGH | ? | mimeExtension.js | 3200 | Clone in performance-critical code — consider references |
| HIGH | ? | mimeExtension.js | 3213 | Clone in performance-critical code — consider references |
| HIGH | ? | mimeExtension.js | 3214 | Clone in performance-critical code — consider references |
| HIGH | ? | mimeExtension.js | 3789 | Clone in performance-critical code — consider references |
| HIGH | ? | plotly.min.js | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | plotly.min.js | 2718 | Clone in performance-critical code — consider references |
| HIGH | ? | plotly.min.js | 3214 | Clone in performance-critical code — consider references |
| HIGH | ? | plotly.min.js | 3227 | Clone in performance-critical code — consider references |
| HIGH | ? | plotly.min.js | 3228 | Clone in performance-critical code — consider references |
| HIGH | ? | plotly.min.js | 3803 | Clone in performance-critical code — consider references |
| HIGH | ? | widgetbundle.js | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | widgetbundle.js | 2704 | Clone in performance-critical code — consider references |
| HIGH | ? | widgetbundle.js | 3200 | Clone in performance-critical code — consider references |
| HIGH | ? | widgetbundle.js | 3213 | Clone in performance-critical code — consider references |
| HIGH | ? | widgetbundle.js | 3214 | Clone in performance-critical code — consider references |
| HIGH | ? | widgetbundle.js | 3789 | Clone in performance-critical code — consider references |
| HIGH | ? | widgetbundle.js | 3808 | Clone in performance-critical code — consider references |
| HIGH | ? | 1.3ad216e94ff8bdcd7b73.js | 2 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | mimeExtension.js | 4 |
| C | ? | mimeExtension.js | 6 |
| C | ? | mimeExtension.js | 7 |
| C | ? | mimeExtension.js | 8 |
| C | ? | mimeExtension.js | 1994 |
| C | ? | plotly.min.js | 18 |
| C | ? | plotly.min.js | 20 |
| C | ? | plotly.min.js | 21 |
| C | ? | plotly.min.js | 22 |
| C | ? | plotly.min.js | 2008 |
| C | ? | widgetbundle.js | 4 |
| C | ? | widgetbundle.js | 6 |
| C | ? | widgetbundle.js | 7 |
| C | ? | widgetbundle.js | 8 |
| C | ? | widgetbundle.js | 1994 |
| C | ? | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| L | ? | renderer.py | 318 |
| L | ? | renderer.py | 320 |
| L | ? | renderer.py | 323 |
| H | ? | widget.ts | 8 |
| H | ? | widget.ts | 9 |
| H | ? | widget.ts | 10 |
| H | ? | widget.ts | 11 |
| H | ? | widget.ts | 12 |
| H | ? | widget.ts | 13 |
| H | ? | widget.ts | 17 |
| H | ? | widget.ts | 18 |
| H | ? | widget.ts | 33 |
| H | ? | widget.ts | 37 |
| H | ? | widget.ts | 42 |
| H | ? | widget.ts | 43 |
| H | ? | widget.ts | 47 |
| H | ? | widget.ts | 48 |
| H | ? | widget.ts | 61 |
| H | ? | widget.ts | 62 |
| H | ? | widget.ts | 63 |
| H | ? | widget.ts | 67 |
| H | ? | widget.ts | 71 |
| H | ? | widget.ts | 72 |
| H | ? | widget.ts | 74 |
| H | ? | widget.ts | 87 |
| H | ? | widget.ts | 92 |
| H | ? | widget.ts | 96 |
| H | ? | widget.ts | 100 |
| H | ? | widget.ts | 101 |
| H | ? | widget.ts | 105 |
| H | ? | widget.ts | 106 |
| H | ? | widget.ts | 852 |
| H | ? | widget.ts | 886 |
| H | ? | widget.ts | 889 |
| H | ? | widget.ts | 892 |
| H | ? | widget.ts | 895 |
| H | ? | widget.ts | 898 |
| H | ? | widget.ts | 901 |
| H | ? | widget.ts | 904 |
| H | ? | widget.ts | 907 |
| H | ? | widget.ts | 910 |
| H | ? | widget.ts | 929 |
| H | ? | widget.ts | 941 |
| H | ? | widget.ts | 1033 |
| H | ? | widget.ts | 1121 |
| H | ? | widget.ts | 1148 |
| H | ? | widget.ts | 1179 |
| H | ? | widget.ts | 1214 |
| H | ? | widget.ts | 1239 |
| H | ? | widget.ts | 1267 |
| H | ? | widget.ts | 1275 |
| H | ? | widget.ts | 1283 |
| H | ? | widget.ts | 1291 |
| H | ? | widget.ts | 1299 |
| H | ? | widget.ts | 1317 |
| H | ? | widget.ts | 1341 |
| H | ? | widget.ts | 1498 |
| H | ? | widget.ts | 1529 |
| H | ? | widget.ts | 1554 |
| H | ? | widget.ts | 1628 |
| H | ? | widget.ts | 1629 |
| H | ? | widget.ts | 1662 |
| H | ? | widget.ts | 1663 |
| H | ? | widget.ts | 1712 |
| H | ? | widget.ts | 1727 |
| H | ? | widget.ts | 1759 |
| H | ? | widget.ts | 1803 |
| H | ? | widget.ts | 1804 |
| H | ? | widget.ts | 1858 |
| H | ? | widget.ts | 1863 |
| H | ? | widget.ts | 1943 |
| H | ? | widget.ts | 1945 |
| H | ? | widget.ts | 2018 |
| M | ? | widget.ts | 2054 |
| M | ? | png.py | 590 |
| M | ? | png.py | 591 |
| M | ? | png.py | 593 |
| M | ? | png.py | 619 |
| M | ? | png.py | 948 |
| M | ? | png.py | 968 |
| M | ? | png.py | 969 |
| M | ? | png.py | 1057 |
| M | ? | png.py | 1061 |
| M | ? | png.py | 1247 |
| M | ? | png.py | 1511 |
| M | ? | png.py | 1545 |
| M | ? | png.py | 1584 |
| M | ? | png.py | 2156 |
| M | ? | basevalidators.py | 89 |
| M | ? | basevalidators.py | 2044 |
| M | ? | basevalidators.py | 2065 |
| M | ? | commands.py | 123 |
| M | ? | commands.py | 141 |
| M | ? | commands.py | 168 |
| M | ? | basewidget.py | 834 |
| M | ? | basewidget.py | 861 |
| M | ? | basedatatypes.py | 1894 |
| M | ? | basedatatypes.py | 4537 |
| M | ? | basedatatypes.py | 4594 |
| M | ? | basedatatypes.py | 4636 |
| M | ? | _core.py | 439 |
| M | ? | _core.py | 1423 |
| M | ? | _core.py | 1824 |
| M | ? | validators.py | 24 |
| M | ? | validators.py | 25 |
| M | ? | validators.py | 48 |
| M | ? | datatypes.py | 76 |
| M | ? | datatypes.py | 534 |
| M | ? | utils.py | 454 |
| M | ? | utils.py | 895 |
| M | ? | utils.py | 1204 |
| H | ? | data_utils.py | 73 |
| H | ? | _orca.py | 952 |
| H | ? | _orca.py | 1066 |
| H | ? | _orca.py | 1533 |
| H | ? | commands.py | 74 |
| H | ? | commands.py | 122 |
| H | ? | commands.py | 139 |
| H | ? | commands.py | 167 |
| M | ? | _orca.py | 1528 |
| M | ? | _scatterplot.py | 189 |
| M | ? | _scatterplot.py | 192 |
| M | ? | _scatterplot.py | 337 |
| M | ? | _scatterplot.py | 341 |
| M | ? | _scatterplot.py | 511 |
| M | ? | _scatterplot.py | 515 |
| M | ? | _scatterplot.py | 670 |
| M | ? | _scatterplot.py | 673 |
| M | ? | _scatterplot.py | 805 |
| M | ? | _scatterplot.py | 808 |
| M | ? | _orca.py | 1528 |
| M | ? | _core.py | 637 |
| M | ? | _core.py | 638 |
| M | ? | renderer.py | 763 |
| M | ? | renderer.py | 794 |
| M | ? | validators.py | 31 |
| L | GS003 | commands.py | 140 |
| L | GS003 | commands.py | 300 |
| L | GS003 | commands.py | 311 |
| L | GS003 | commands.py | 330 |
| L | GS003 | commands.py | 335 |
| L | GS003 | commands.py | 343 |
| L | GS003 | commands.py | 367 |
| L | GS003 | commands.py | 380 |
| L | GS003 | commands.py | 388 |
| L | GS003 | commands.py | 410 |
| L | GS003 | commands.py | 424 |
| L | GS003 | commands.py | 432 |
| L | GS003 | commands.py | 454 |
| L | GS003 | commands.py | 459 |
| L | GS003 | commands.py | 527 |
| L | GS003 | commands.py | 538 |
| L | GS003 | helper_go_names.py | 9 |
| L | GS003 | helper_go_names.py | 36 |
| L | GS003 | _subplots.py | 883 |
| L | GS003 | basedatatypes.py | 852 |
| L | GS003 | _kaleido.py | 861 |
| L | GS003 | _kaleido.py | 863 |
| L | GS003 | _kaleido.py | 865 |
| L | GS003 | _kaleido.py | 866 |
| L | GS003 | _orca.py | 132 |
| L | GS003 | tools.py | 15 |
| L | GS003 | tools.py | 102 |
| L | GS003 | tools.py | 208 |
| L | GS003 | tools.py | 217 |
| L | GS003 | mimeExtension.js | 8 |
| L | GS003 | mimeExtension.js | 17 |
| L | GS003 | mimeExtension.js | 17 |
| L | GS003 | mimeExtension.js | 17 |
| L | GS003 | mimeExtension.js | 26 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 2704 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3214 |
| L | GS003 | mimeExtension.js | 3789 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS003 | plotly.min.js | 22 |
| L | GS003 | plotly.min.js | 31 |
| L | GS003 | plotly.min.js | 31 |
| L | GS003 | plotly.min.js | 31 |
| L | GS003 | plotly.min.js | 40 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 2718 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | plotly.min.js | 3228 |
| L | GS003 | widgetbundle.js | 8 |
| L | GS003 | widgetbundle.js | 17 |
| L | GS003 | widgetbundle.js | 17 |
| L | GS003 | widgetbundle.js | 17 |
| L | GS003 | widgetbundle.js | 26 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 2704 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS003 | widgetbundle.js | 3214 |
| L | GS008 | utils.py | 10 |
| L | GS008 | _facet_grid.py | 20 |
| L | GS008 | tools.py | 17 |
| L | GS008 | tools.py | 32 |
| L | GS008 | tools.py | 53 |
| L | GS008 | tools.py | 54 |
| L | GS008 | tools.py | 55 |
| L | GS008 | tools.py | 560 |
| L | GS008 | tools.py | 561 |
| L | GS008 | tools.py | 563 |
| L | GS008 | tools.py | 564 |
| H | ? | mimeExtension.js | 4 |
| H | ? | mimeExtension.js | 7 |
| H | ? | plotly.min.js | 18 |
| H | ? | plotly.min.js | 21 |
| H | ? | widgetbundle.js | 4 |
| H | ? | widgetbundle.js | 7 |
| H | ? | 1.3ad216e94ff8bdcd7b73.js | 2 |
| H | ? | uv.lock | 404 |
| H | ? | uv.lock | 452 |
| H | ? | uv.lock | 492 |
| H | ? | uv.lock | 529 |
| H | ? | uv.lock | 531 |
| H | ? | uv.lock | 533 |
| H | ? | uv.lock | 1466 |
| H | ? | uv.lock | 1471 |
| H | ? | uv.lock | 1473 |
| H | ? | uv.lock | 7941 |
| H | ? | uv.lock | 7953 |
| H | ? | uv.lock | 7955 |
| H | ? | uv.lock | 7956 |
| H | ? | uv.lock | 7957 |
| H | ? | uv.lock | 7958 |
| H | ? | uv.lock | 7959 |
| H | ? | uv.lock | 7960 |
| H | ? | uv.lock | 7961 |
| H | ? | uv.lock | 7962 |
| H | ? | uv.lock | 7963 |
| H | ? | uv.lock | 7964 |
| H | ? | uv.lock | 7965 |
| H | ? | uv.lock | 7966 |
| H | ? | uv.lock | 7967 |
| H | ? | uv.lock | 7968 |
| H | ? | uv.lock | 7969 |
| H | ? | uv.lock | 7970 |
| H | ? | uv.lock | 7971 |
| H | ? | uv.lock | 7972 |
| H | ? | uv.lock | 7973 |
| H | ? | uv.lock | 7974 |
| H | ? | uv.lock | 7975 |
| H | ? | uv.lock | 7976 |
| H | ? | uv.lock | 7977 |
| H | ? | uv.lock | 7978 |
| H | ? | uv.lock | 7979 |
| H | ? | uv.lock | 7980 |
| H | ? | uv.lock | 7981 |
| H | ? | uv.lock | 7982 |
| H | ? | uv.lock | 7983 |
| H | ? | uv.lock | 7984 |
| H | ? | uv.lock | 7985 |
| H | ? | uv.lock | 7986 |
| H | ? | uv.lock | 7991 |
| H | ? | uv.lock | 8001 |
| H | ? | uv.lock | 8003 |
| H | ? | uv.lock | 8004 |
| H | ? | uv.lock | 8005 |
| H | ? | uv.lock | 8006 |
| H | ? | uv.lock | 8007 |
| H | ? | uv.lock | 8008 |
| H | ? | uv.lock | 8009 |
| H | ? | uv.lock | 8010 |
| H | ? | uv.lock | 8011 |
| H | ? | uv.lock | 8012 |
| C | ? | mimeExtension.js | 2699 |
| C | ? | mimeExtension.js | 2704 |
| C | ? | mimeExtension.js | 3200 |
| C | ? | plotly.min.js | 2713 |
| C | ? | plotly.min.js | 2718 |
| C | ? | plotly.min.js | 3214 |
| C | ? | widgetbundle.js | 2699 |
| C | ? | widgetbundle.js | 2704 |
| C | ? | widgetbundle.js | 3200 |
| C | ? | renderer.py | 763 |
| C | ? | renderer.py | 794 |
| C | ? | 1.3ad216e94ff8bdcd7b73.js | 2 |
| M | ? | commands.py | 36 |
| M | ? | commands.py | 38 |
| M | ? | commands.py | 257 |
| M | ? | commands.py | 288 |
| M | ? | commands.py | 331 |
| H | ? | validators.py | 28 |
| H | ? | utils.py | 499 |
| H | ? | dependabot.yml | 0 |
| H | ? | environment.yml | 0 |
| s | GS009 |  | 0 |
| L | GS012 | png.py | 1291 |
| L | GS012 | mimeExtension.js | 2620 |
| L | GS012 | mimeExtension.js | 2620 |
| L | GS012 | mimeExtension.js | 2620 |
| L | GS012 | mimeExtension.js | 2620 |
| L | GS012 | mimeExtension.js | 2697 |
| L | GS012 | mimeExtension.js | 2697 |
| L | GS012 | mimeExtension.js | 2697 |
| L | GS012 | mimeExtension.js | 2697 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.js | 3789 |
| L | GS012 | mimeExtension.ts | 143 |
| L | GS012 | mimeExtension.ts | 184 |
| L | GS012 | mimeExtension.ts | 191 |
| L | GS012 | _orca.py | 695 |
| L | GS012 | _orca.py | 952 |
| L | GS012 | _orca.py | 1066 |
| L | GS012 | _orca.py | 1533 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | 1.3ad216e94ff8bdcd7b73.js | 2 |
| L | GS012 | vega_renderer.py | 150 |
| L | GS012 | widgetbundle.js | 2620 |
| L | GS012 | widgetbundle.js | 2620 |
| L | GS012 | widgetbundle.js | 2620 |
| L | GS012 | widgetbundle.js | 2620 |
| L | GS012 | widgetbundle.js | 2697 |
| L | GS012 | widgetbundle.js | 2697 |
| L | GS012 | widgetbundle.js | 2697 |
| L | GS012 | widgetbundle.js | 2697 |
| M | ? | commands.py | 310 |
| M | ? | commands.py | 325 |
| M | ? | commands.py | 336 |
| H | ? | mimeExtension.js | 87 |
| H | ? | mimeExtension.js | 2704 |
| H | ? | mimeExtension.js | 3200 |
| H | ? | mimeExtension.js | 3213 |
| H | ? | mimeExtension.js | 3214 |
| H | ? | mimeExtension.js | 3789 |
| H | ? | plotly.min.js | 101 |
| H | ? | plotly.min.js | 2718 |
| H | ? | plotly.min.js | 3214 |
| H | ? | plotly.min.js | 3227 |
| H | ? | plotly.min.js | 3228 |
| H | ? | plotly.min.js | 3803 |
| H | ? | widgetbundle.js | 87 |
| H | ? | widgetbundle.js | 2704 |
| H | ? | widgetbundle.js | 3200 |
| H | ? | widgetbundle.js | 3213 |
| H | ? | widgetbundle.js | 3214 |
| H | ? | widgetbundle.js | 3789 |
| H | ? | widgetbundle.js | 3808 |
| H | ? | 1.3ad216e94ff8bdcd7b73.js | 2 |

---
*Сгенерировано GSC v0.6 · 2026-07-19T04:05:52.140144*