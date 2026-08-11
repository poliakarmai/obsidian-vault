---
title: "GSC Audit: /tmp/gsc-learn/tornado"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/tornado

**Дата:** 07.08.2026 04:06  
**Путь:** `/tmp/gsc-learn/tornado`  
**Всего находок:** 1016  
**CRITICAL:** 2 | **HIGH:** 24 | **MEDIUM:** 144 | **LOW:** 394

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 227 |
| GS021 | 190 |
| Python: assert in production | 128 |
| GS003 | 36 |
| Хардкод IP адреса | 12 |
| GS025-eval_usage | 11 |
| Bare except: | 8 |
| GS020 | 7 |
| GS025-debug_mode | 7 |
| Generic code smell #24 | 6 |
| Generic code smell #27 | 6 |
| Generic code smell #30 | 6 |
| Generic code smell #33 | 6 |
| Generic code smell #36 | 6 |
| Generic code smell #39 | 6 |
| Generic code smell #42 | 6 |
| Generic code smell #45 | 6 |
| Generic code smell #48 | 6 |
| Generic code smell #51 | 6 |
| Generic code smell #54 | 6 |
| Generic code smell #57 | 6 |
| Generic code smell #60 | 6 |
| Generic code smell #63 | 6 |
| Generic code smell #66 | 6 |
| Generic code smell #69 | 6 |
| Generic code smell #72 | 6 |
| Generic code smell #75 | 6 |
| Generic code smell #78 | 6 |
| Generic code smell #81 | 6 |
| Generic code smell #84 | 6 |
| Generic code smell #87 | 6 |
| Generic code smell #90 | 6 |
| Generic code smell #93 | 6 |
| Generic code smell #96 | 6 |
| Generic code smell #99 | 6 |
| Generic code smell #102 | 6 |
| Generic code smell #105 | 6 |
| Generic code smell #108 | 6 |
| Generic code smell #111 | 6 |
| Generic code smell #114 | 6 |
| Generic code smell #117 | 6 |
| Generic code smell #120 | 6 |
| Generic code smell #123 | 6 |
| Generic code smell #126 | 6 |
| Generic code smell #129 | 6 |
| Generic code smell #132 | 6 |
| Generic code smell #135 | 6 |
| Generic code smell #138 | 6 |
| Generic code smell #141 | 6 |
| Generic code smell #144 | 6 |
| Generic code smell #147 | 6 |
| Generic code smell #150 | 6 |
| Generic code smell #153 | 6 |
| Generic code smell #156 | 6 |
| Generic code smell #159 | 6 |
| Generic code smell #162 | 6 |
| Generic code smell #165 | 6 |
| Generic code smell #168 | 6 |
| Generic code smell #171 | 6 |
| Generic code smell #174 | 6 |
| Generic code smell #177 | 6 |
| Generic code smell #180 | 6 |
| Generic code smell #183 | 6 |
| Generic code smell #186 | 6 |
| Generic code smell #189 | 6 |
| Generic code smell #192 | 6 |
| Generic code smell #195 | 6 |
| Generic code smell #198 | 6 |
| CVE-2026-37270: Hardcoded credential | 6 |
| GS018 | 5 |
| GS008 | 4 |
| GS025-hardcoded_secret | 4 |
| GS015 | 3 |
| Python: File upload without content-type validation | 2 |
| eval() or exec() usage | 2 |
| GS007 | 2 |
| CVE-2026-56318: Information disclosure | 1 |
| GS001 | 1 |
| Hardcoded encryption key | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS004 | 1 |
| GS009 | 1 |
| GS014 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | pyproject.toml | 9 | Found: 'py310' |
| CRITICAL | ? | main.py | 105 | Match:         cookie_secret="__TODO:_GENERATE_YOUR_OWN_RAND |
| HIGH | ? | file_uploader.py | 106 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | httputil.py | 454 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | blog.py | 30 | Match: define("db_host", default="127.0.0.1", help="blog dat |
| HIGH | ? | chunk_benchmark.py | 33 | Match:     app.listen(options.port, address='127.0.0.1') |
| HIGH | ? | benchmark.py | 58 | Match:     app.listen(port, address="127.0.0.1") |
| HIGH | ? | benchmark.py | 67 | Match:     args.append("http://127.0.0.1:%d/" % port) |
| HIGH | ? | Vagrantfile | 4 | Match:     config.vm.network :hostonly, "172.19.1.8" |
| HIGH | ? | Vagrantfile | 5 | Match:     config.vm.network :hostonly, "172.19.1.5" |
| HIGH | ? | server.py | 22 | Match:     app.listen(options.port, address='127.0.0.1') |
| HIGH | ? | testing.py | 47 | Match:     reuse_port: bool = False, address: str = "127.0.0 |
| HIGH | ? | testing.py | 466 | Match:         return f"{self.get_protocol()}://127.0.0.1:{s |
| HIGH | ? | util.py | 72 | Match:     client_socket.connect(("127.0.0.1", port)) |
| HIGH | ? | tcpclient.py | 303 | Match:             source_ip_bind = "::1" if af == socket.AF |
| HIGH | ? | web.py | 2174 | Match:        relevant to applications that only listen on ` |
| HIGH | ? | util.py | 137 | Match:     exec(code, glob, loc) |
| HIGH | ? | util.py | 90 | Match:     exec(textwrap.dedent(s), global_namespace, local_ |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | util.py | 137 | Line 137: exec(code, glob, loc) |
| HIGH | GS018 | routing.py | 223 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | routing.py | 433 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | routing.py | 482 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | routing.py | 510 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | routing.py | 598 | Cancel/refund function lacks state check. Risk: refund after |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | chatdemo.py | 76 |
| M | ? | process.py | 232 |
| M | ? | twisted.py | 59 |
| M | ? | iostream.py | 349 |
| M | ? | iostream.py | 386 |
| M | ? | iostream.py | 414 |
| M | ? | iostream.py | 459 |
| M | ? | iostream.py | 489 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| L | ? | chatdemo.py | 119 |
| L | ? | chatdemo.py | 36 |
| L | ? | main.py | 105 |
| L | ? | blog.py | 72 |
| L | ? | facebook.py | 36 |
| L | ? | simple_httpclient.py | 702 |
| M | ? | webspider.py | 87 |
| M | ? | chunk_benchmark.py | 37 |
| M | ? | client.py | 19 |
| M | ? | client.py | 34 |
| M | ? | routing.py | 248 |
| M | ? | routing.py | 268 |
| M | ? | routing.py | 272 |
| M | ? | routing.py | 347 |
| M | ? | routing.py | 397 |
| M | ? | routing.py | 401 |
| M | ? | routing.py | 568 |
| M | ? | routing.py | 601 |
| M | ? | process.py | 113 |
| M | ? | process.py | 342 |
| M | ? | process.py | 353 |
| M | ? | template.py | 303 |
| M | ? | template.py | 580 |
| M | ? | template.py | 585 |
| M | ? | template.py | 746 |
| M | ? | template.py | 787 |
| M | ? | template.py | 794 |
| M | ? | template.py | 922 |
| M | ? | wsgi.py | 53 |
| M | ? | tcpserver.py | 293 |
| M | ? | tcpserver.py | 311 |
| M | ? | tcpserver.py | 335 |
| M | ? | netutil.py | 610 |
| M | ? | netutil.py | 611 |
| M | ? | netutil.py | 664 |
| M | ? | testing.py | 181 |
| M | ? | testing.py | 285 |
| M | ? | testing.py | 340 |
| M | ? | ioloop.py | 512 |
| M | ? | ioloop.py | 525 |
| M | ? | ioloop.py | 533 |
| M | ? | ioloop.py | 704 |
| M | ? | gen.py | 517 |
| M | ? | locale.py | 259 |
| M | ? | locale.py | 500 |
| M | ? | locale.py | 539 |
| M | ? | locale.py | 571 |
| M | ? | auth.py | 136 |
| M | ? | auth.py | 352 |
| M | ? | auth.py | 399 |
| M | ? | auth.py | 1071 |
| M | ? | queues.py | 218 |
| M | ? | queues.py | 267 |
| M | ? | asyncio.py | 566 |
| M | ? | asyncio.py | 577 |
| M | ? | httpclient.py | 106 |
| M | ? | options.py | 279 |
| M | ? | options.py | 511 |
| M | ? | simple_httpclient.py | 162 |
| M | ? | simple_httpclient.py | 163 |
| M | ? | simple_httpclient.py | 386 |
| M | ? | simple_httpclient.py | 586 |
| M | ? | simple_httpclient.py | 606 |
| M | ? | simple_httpclient.py | 616 |
| M | ? | simple_httpclient.py | 621 |
| M | ? | simple_httpclient.py | 622 |
| M | ? | simple_httpclient.py | 654 |
| M | ? | simple_httpclient.py | 663 |
| M | ? | simple_httpclient.py | 694 |
| M | ? | iostream.py | 157 |
| M | ? | iostream.py | 173 |
| M | ? | iostream.py | 194 |
| M | ? | iostream.py | 409 |
| M | ? | iostream.py | 708 |
| M | ? | iostream.py | 795 |
| M | ? | iostream.py | 943 |
| M | ? | iostream.py | 980 |
| M | ? | http1connection.py | 65 |
| M | ? | http1connection.py | 233 |
| M | ? | http1connection.py | 392 |
| M | ? | http1connection.py | 403 |
| M | ? | http1connection.py | 404 |
| M | ? | http1connection.py | 405 |
| M | ? | http1connection.py | 691 |
| M | ? | http1connection.py | 806 |
| M | ? | http1connection.py | 817 |
| M | ? | websocket.py | 392 |
| M | ? | websocket.py | 580 |
| M | ? | websocket.py | 665 |
| M | ? | websocket.py | 774 |
| M | ? | websocket.py | 928 |
| M | ? | websocket.py | 986 |
| M | ? | websocket.py | 987 |
| M | ? | websocket.py | 989 |
| M | ? | websocket.py | 1091 |
| M | ? | websocket.py | 1117 |
| M | ? | websocket.py | 1180 |
| M | ? | websocket.py | 1222 |
| M | ? | websocket.py | 1508 |
| M | ? | websocket.py | 1613 |
| M | ? | websocket.py | 1622 |
| M | ? | websocket.py | 1623 |
| M | ? | websocket.py | 1691 |
| M | ? | autoreload.py | 215 |
| M | ? | web.py | 221 |
| M | ? | web.py | 471 |
| M | ? | web.py | 954 |
| M | ? | web.py | 1144 |
| M | ? | web.py | 1211 |
| M | ? | web.py | 1217 |
| M | ? | web.py | 1285 |
| M | ? | web.py | 1293 |
| M | ? | web.py | 1410 |
| M | ? | web.py | 1597 |
| M | ? | web.py | 1598 |
| M | ? | web.py | 2085 |
| M | ? | web.py | 2850 |
| M | ? | web.py | 2861 |
| M | ? | web.py | 2912 |
| M | ? | web.py | 3030 |
| M | ? | web.py | 3052 |
| M | ? | web.py | 3102 |
| M | ? | web.py | 3382 |
| M | ? | web.py | 3576 |
| M | ? | web.py | 3610 |
| M | ? | web.py | 3613 |
| M | ? | web.py | 3673 |
| M | ? | curl_httpclient.py | 245 |
| M | ? | curl_httpclient.py | 247 |
| M | ? | curl_httpclient.py | 354 |
| M | ? | curl_httpclient.py | 363 |
| M | ? | curl_httpclient.py | 365 |
| M | ? | curl_httpclient.py | 381 |
| M | ? | curl_httpclient.py | 482 |
| H | ? | file_uploader.py | 106 |
| H | ? | httputil.py | 454 |
| M | ? | httpclient.py | 353 |
| M | ? | chatdemo.py | 119 |
| M | ? | chatdemo.py | 36 |
| M | ? | main.py | 105 |
| M | ? | blog.py | 72 |
| M | ? | facebook.py | 36 |
| M | ? | httpclient.py | 353 |
| C | GS001 | pyproject.toml | 9 |
| L | GS003 | facebook.py | 105 |
| L | GS003 | file_uploader.py | 68 |
| L | GS003 | file_uploader.py | 97 |
| L | GS003 | file_uploader.py | 106 |
| L | GS003 | main.py | 53 |
| L | GS003 | client.py | 15 |
| L | GS003 | client.py | 17 |
| L | GS003 | server.py | 28 |
| L | GS003 | webspider.py | 24 |
| L | GS003 | webspider.py | 59 |
| L | GS003 | webspider.py | 77 |
| L | GS003 | webspider.py | 88 |
| L | GS003 | webspider.py | 89 |
| L | GS003 | gen_benchmark.py | 46 |
| L | GS003 | gen_benchmark.py | 49 |
| L | GS003 | parsing_benchmark.py | 61 |
| L | GS003 | parsing_benchmark.py | 66 |
| L | GS003 | parsing_benchmark.py | 67 |
| L | GS003 | parsing_benchmark.py | 73 |
| L | GS003 | parsing_benchmark.py | 78 |
| L | GS003 | parsing_benchmark.py | 79 |
| L | GS003 | parsing_benchmark.py | 101 |
| L | GS003 | httpclient.py | 781 |
| L | GS003 | httpclient.py | 783 |
| L | GS003 | iostream.py | 1078 |
| L | GS003 | options.py | 436 |
| L | GS003 | options.py | 437 |
| L | GS003 | options.py | 444 |
| L | GS003 | options.py | 457 |
| L | GS003 | options.py | 459 |
| L | GS003 | options.py | 460 |
| L | GS003 | template.py | 775 |
| L | GS003 | testing.py | 848 |
| L | GS003 | chat.js | 60 |
| L | GS003 | chat.js | 113 |
| L | GS003 | chat.js | 121 |
| L | GS008 | _locale_data.py | 17 |
| L | GS008 | concurrent.py | 138 |
| L | GS008 | web.py | 123 |
| L | GS008 | web.py | 131 |
| I | GS015 | main.py | 32 |
| I | GS015 | server.py | 1 |
| I | GS015 | wsgi.py | 1 |
| i | GS020 |  | 22 |
| i | GS020 |  | 22 |
| i | GS020 |  | 4 |
| i | GS020 |  | 18 |
| i | GS020 |  | 58 |
| i | GS020 |  | 102 |
| i | GS020 |  | 20 |
| H | ? | blog.py | 30 |
| H | ? | chunk_benchmark.py | 33 |
| H | ? | benchmark.py | 58 |
| H | ? | benchmark.py | 67 |
| H | ? | Vagrantfile | 4 |
| H | ? | Vagrantfile | 5 |
| H | ? | server.py | 22 |
| H | ? | testing.py | 47 |
| H | ? | testing.py | 466 |
| H | ? | util.py | 72 |
| H | ? | tcpclient.py | 303 |
| H | ? | web.py | 2174 |
| C | ? | main.py | 105 |
| H | ? | util.py | 137 |
| H | ? | util.py | 90 |
| H | ? | codecov.yml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | GS004 | util.py | 137 |
| I | GS007 | schema.sql | 25 |
| I | GS007 | schema.sql | 33 |
| s | GS009 |  | 0 |
| M | GS014 | test.key | 1 |
| H | GS018 | routing.py | 223 |
| H | GS018 | routing.py | 433 |
| H | GS018 | routing.py | 482 |
| H | GS018 | routing.py | 510 |
| H | GS018 | routing.py | 598 |
| s | GS021 |  | 116 |
| s | GS021 |  | 166 |
| s | GS021 |  | 553 |
| s | GS021 |  | 47 |
| s | GS021 |  | 49 |
| s | GS021 |  | 54 |
| s | GS021 |  | 55 |
| s | GS021 |  | 59 |
| s | GS021 |  | 466 |
| s | GS021 |  | 317 |
| s | GS021 |  | 33 |
| s | GS021 |  | 34 |
| s | GS021 |  | 539 |
| s | GS021 |  | 175 |
| s | GS021 |  | 303 |
| c | GS021 |  | 758 |
| s | GS021 |  | 2174 |
| s | GS021 |  | 7 |
| s | GS021 |  | 6 |
| s | GS021 |  | 11 |
| s | GS021 |  | 100 |
| s | GS021 |  | 63 |
| s | GS021 |  | 92 |
| s | GS021 |  | 30 |
| s | GS021 |  | 33 |
| s | GS021 |  | 43 |
| s | GS021 |  | 49 |
| s | GS021 |  | 58 |
| s | GS021 |  | 67 |
| s | GS021 |  | 22 |
| s | GS021 |  | 8 |
| s | GS021 |  | 33 |
| s | GS021 |  | 34 |
| s | GS021 |  | 39 |
| s | GS021 |  | 167 |
| s | GS021 |  | 176 |
| s | GS021 |  | 181 |
| s | GS021 |  | 183 |
| s | GS021 |  | 193 |
| s | GS021 |  | 208 |
| s | GS021 |  | 178 |
| s | GS021 |  | 186 |
| s | GS021 |  | 41 |
| s | GS021 |  | 75 |
| s | GS021 |  | 78 |
| s | GS021 |  | 81 |
| s | GS021 |  | 101 |
| s | GS021 |  | 104 |
| s | GS021 |  | 108 |
| s | GS021 |  | 113 |
| s | GS021 |  | 114 |
| s | GS021 |  | 117 |
| s | GS021 |  | 121 |
| s | GS021 |  | 125 |
| s | GS021 |  | 132 |
| s | GS021 |  | 140 |
| s | GS021 |  | 145 |
| s | GS021 |  | 146 |
| s | GS021 |  | 146 |
| s | GS021 |  | 159 |
| s | GS021 |  | 111 |
| s | GS021 |  | 57 |
| c | GS021 |  | 379 |
| s | GS021 |  | 531 |
| s | GS021 |  | 558 |
| s | GS021 |  | 1757 |
| s | GS021 |  | 2464 |
| s | GS021 |  | 2466 |
| s | GS021 |  | 3341 |
| s | GS021 |  | 202 |
| s | GS021 |  | 271 |
| s | GS021 |  | 564 |
| s | GS021 |  | 626 |
| s | GS021 |  | 922 |
| s | GS021 |  | 72 |
| s | GS021 |  | 156 |
| s | GS021 |  | 34 |
| s | GS021 |  | 57 |
| s | GS021 |  | 85 |
| s | GS021 |  | 148 |
| s | GS021 |  | 168 |
| s | GS021 |  | 185 |
| s | GS021 |  | 206 |
| s | GS021 |  | 214 |
| s | GS021 |  | 39 |
| s | GS021 |  | 40 |
| s | GS021 |  | 43 |
| s | GS021 |  | 44 |
| s | GS021 |  | 47 |
| s | GS021 |  | 48 |
| s | GS021 |  | 51 |
| s | GS021 |  | 52 |
| s | GS021 |  | 55 |
| s | GS021 |  | 56 |
| s | GS021 |  | 59 |
| s | GS021 |  | 60 |
| s | GS021 |  | 63 |
| s | GS021 |  | 64 |
| s | GS021 |  | 67 |
| s | GS021 |  | 68 |
| s | GS021 |  | 71 |
| s | GS021 |  | 72 |
| s | GS021 |  | 75 |
| s | GS021 |  | 76 |
| s | GS021 |  | 79 |
| s | GS021 |  | 80 |
| s | GS021 |  | 83 |
| s | GS021 |  | 84 |
| s | GS021 |  | 31 |
| s | GS021 |  | 117 |
| s | GS021 |  | 207 |
| s | GS021 |  | 261 |
| s | GS021 |  | 266 |
| s | GS021 |  | 421 |
| s | GS021 |  | 478 |
| s | GS021 |  | 499 |
| s | GS021 |  | 520 |
| s | GS021 |  | 539 |
| s | GS021 |  | 562 |
| s | GS021 |  | 582 |
| s | GS021 |  | 618 |
| s | GS021 |  | 621 |
| s | GS021 |  | 653 |
| s | GS021 |  | 654 |
| s | GS021 |  | 677 |
| s | GS021 |  | 684 |
| s | GS021 |  | 703 |
| s | GS021 |  | 708 |
| s | GS021 |  | 713 |
| s | GS021 |  | 717 |
| s | GS021 |  | 940 |
| s | GS021 |  | 963 |
| s | GS021 |  | 965 |
| s | GS021 |  | 973 |
| s | GS021 |  | 1021 |
| s | GS021 |  | 1021 |
| s | GS021 |  | 1031 |
| s | GS021 |  | 1031 |
| s | GS021 |  | 1040 |
| s | GS021 |  | 1048 |
| s | GS021 |  | 1076 |
| s | GS021 |  | 1079 |
| s | GS021 |  | 1323 |
| s | GS021 |  | 1342 |
| s | GS021 |  | 1442 |
| s | GS021 |  | 1460 |
| s | GS021 |  | 1464 |
| s | GS021 |  | 1473 |
| s | GS021 |  | 299 |
| s | GS021 |  | 378 |
| s | GS021 |  | 391 |
| s | GS021 |  | 736 |
| s | GS021 |  | 737 |
| s | GS021 |  | 766 |
| s | GS021 |  | 296 |
| s | GS021 |  | 301 |
| s | GS021 |  | 108 |
| s | GS021 |  | 118 |
| s | GS021 |  | 138 |
| s | GS021 |  | 161 |
| s | GS021 |  | 177 |
| s | GS021 |  | 187 |
| s | GS021 |  | 775 |
| s | GS021 |  | 794 |
| s | GS021 |  | 812 |
| s | GS021 |  | 992 |
| s | GS021 |  | 1070 |
| s | GS021 |  | 1082 |
| s | GS021 |  | 1125 |
| s | GS021 |  | 1223 |
| s | GS021 |  | 1244 |
| s | GS021 |  | 1260 |
| s | GS021 |  | 86 |
| s | GS021 |  | 231 |
| s | GS021 |  | 339 |
| s | GS021 |  | 409 |
| s | GS021 |  | 415 |
| s | GS021 |  | 429 |
| s | GS021 |  | 447 |
| s | GS021 |  | 519 |
| s | GS021 |  | 520 |
| s | GS021 |  | 533 |
| s | GS021 |  | 534 |
| s | GS021 |  | 547 |
| s | GS021 |  | 548 |
| s | GS021 |  | 558 |
| s | GS021 |  | 575 |
| s | GS021 |  | 578 |
| s | GS021 |  | 581 |
| s | GS021 |  | 584 |
| r | GS022 |  | 223 |
| r | GS022 |  | 433 |
| r | GS022 |  | 439 |
| r | GS022 |  | 372 |
| r | GS022 |  | 442 |
| r | GS022 |  | 464 |
| r | GS022 |  | 545 |
| r | GS022 |  | 554 |
| r | GS022 |  | 558 |
| r | GS022 |  | 174 |
| r | GS022 |  | 49 |
| r | GS022 |  | 180 |
| r | GS022 |  | 355 |
| r | GS022 |  | 360 |
| r | GS022 |  | 400 |
| r | GS022 |  | 408 |
| r | GS022 |  | 428 |
| r | GS022 |  | 459 |
| r | GS022 |  | 463 |
| r | GS022 |  | 617 |
| r | GS022 |  | 764 |
| r | GS022 |  | 938 |
| r | GS022 |  | 1017 |
| r | GS022 |  | 1064 |
| r | GS022 |  | 1174 |
| r | GS022 |  | 1205 |
| r | GS022 |  | 37 |
| r | GS022 |  | 596 |
| r | GS022 |  | 813 |
| r | GS022 |  | 35 |
| r | GS022 |  | 551 |
| r | GS022 |  | 557 |
| r | GS022 |  | 1077 |
| r | GS022 |  | 1112 |
| r | GS022 |  | 1501 |
| r | GS022 |  | 1695 |
| r | GS022 |  | 1731 |
| r | GS022 |  | 1741 |
| r | GS022 |  | 1743 |
| r | GS022 |  | 2385 |
| r | GS022 |  | 2394 |
| r | GS022 |  | 3138 |
| r | GS022 |  | 3146 |
| r | GS022 |  | 3376 |
| r | GS022 |  | 3380 |
| r | GS022 |  | 3480 |
| r | GS022 |  | 68 |
| r | GS022 |  | 293 |
| r | GS022 |  | 16 |
| r | GS022 |  | 56 |
| r | GS022 |  | 62 |
| r | GS022 |  | 75 |
| r | GS022 |  | 62 |
| r | GS022 |  | 96 |
| r | GS022 |  | 97 |
| r | GS022 |  | 98 |
| r | GS022 |  | 76 |
| r | GS022 |  | 79 |
| r | GS022 |  | 131 |
| r | GS022 |  | 138 |
| r | GS022 |  | 141 |
| r | GS022 |  | 142 |
| r | GS022 |  | 146 |
| r | GS022 |  | 149 |
| r | GS022 |  | 152 |
| r | GS022 |  | 158 |
| r | GS022 |  | 165 |
| r | GS022 |  | 170 |
| r | GS022 |  | 178 |
| r | GS022 |  | 186 |
| r | GS022 |  | 194 |
| r | GS022 |  | 202 |
| r | GS022 |  | 211 |
| r | GS022 |  | 219 |
| r | GS022 |  | 227 |
| r | GS022 |  | 235 |
| r | GS022 |  | 231 |
| r | GS022 |  | 238 |
| r | GS022 |  | 106 |
| r | GS022 |  | 108 |
| r | GS022 |  | 56 |
| r | GS022 |  | 93 |
| r | GS022 |  | 258 |
| r | GS022 |  | 263 |
| r | GS022 |  | 269 |
| r | GS022 |  | 501 |
| r | GS022 |  | 522 |
| r | GS022 |  | 527 |
| r | GS022 |  | 674 |
| r | GS022 |  | 852 |
| r | GS022 |  | 853 |
| r | GS022 |  | 854 |
| r | GS022 |  | 855 |
| r | GS022 |  | 856 |
| r | GS022 |  | 857 |
| r | GS022 |  | 858 |
| r | GS022 |  | 859 |
| r | GS022 |  | 860 |
| r | GS022 |  | 865 |
| r | GS022 |  | 870 |
| r | GS022 |  | 875 |
| r | GS022 |  | 876 |
| r | GS022 |  | 877 |
| r | GS022 |  | 878 |
| r | GS022 |  | 948 |
| r | GS022 |  | 949 |
| r | GS022 |  | 950 |
| r | GS022 |  | 951 |
| r | GS022 |  | 953 |
| r | GS022 |  | 956 |
| r | GS022 |  | 1130 |
| r | GS022 |  | 1131 |
| r | GS022 |  | 1132 |
| r | GS022 |  | 1179 |
| r | GS022 |  | 1189 |
| r | GS022 |  | 1190 |
| r | GS022 |  | 1268 |
| r | GS022 |  | 1272 |
| r | GS022 |  | 1276 |
| r | GS022 |  | 1285 |
| r | GS022 |  | 1627 |
| r | GS022 |  | 1671 |
| r | GS022 |  | 1684 |
| r | GS022 |  | 2410 |
| r | GS022 |  | 3347 |
| r | GS022 |  | 3348 |
| r | GS022 |  | 3358 |
| r | GS022 |  | 3370 |
| r | GS022 |  | 3374 |
| r | GS022 |  | 89 |
| r | GS022 |  | 171 |
| r | GS022 |  | 172 |
| r | GS022 |  | 173 |
| r | GS022 |  | 174 |
| r | GS022 |  | 175 |
| r | GS022 |  | 176 |
| r | GS022 |  | 177 |
| r | GS022 |  | 178 |
| r | GS022 |  | 179 |
| r | GS022 |  | 180 |
| r | GS022 |  | 181 |
| r | GS022 |  | 182 |
| r | GS022 |  | 183 |
| r | GS022 |  | 184 |
| r | GS022 |  | 185 |
| r | GS022 |  | 186 |
| r | GS022 |  | 187 |
| r | GS022 |  | 388 |
| r | GS022 |  | 389 |
| r | GS022 |  | 520 |
| r | GS022 |  | 573 |
| r | GS022 |  | 591 |
| r | GS022 |  | 597 |
| r | GS022 |  | 606 |
| r | GS022 |  | 616 |
| r | GS022 |  | 625 |
| r | GS022 |  | 745 |
| r | GS022 |  | 784 |
| r | GS022 |  | 803 |
| r | GS022 |  | 804 |
| r | GS022 |  | 921 |
| r | GS022 |  | 925 |
| r | GS022 |  | 932 |
| r | GS022 |  | 389 |
| r | GS022 |  | 793 |
| r | GS022 |  | 807 |
| r | GS022 |  | 107 |
| r | GS022 |  | 129 |
| r | GS022 |  | 139 |
| r | GS022 |  | 140 |
| r | GS022 |  | 251 |
| r | GS022 |  | 124 |
| r | GS022 |  | 135 |
| r | GS022 |  | 74 |
| r | GS022 |  | 75 |
| r | GS022 |  | 84 |
| r | GS022 |  | 85 |
| r | GS022 |  | 103 |
| r | GS022 |  | 104 |
| r | GS022 |  | 112 |
| r | GS022 |  | 113 |
| r | GS022 |  | 28 |
| r | GS022 |  | 64 |
| r | GS022 |  | 65 |
| r | GS022 |  | 66 |
| r | GS022 |  | 136 |
| r | GS022 |  | 145 |
| r | GS022 |  | 146 |
| r | GS022 |  | 147 |
| r | GS022 |  | 153 |
| r | GS022 |  | 161 |
| r | GS022 |  | 179 |
| r | GS022 |  | 180 |
| r | GS022 |  | 181 |
| r | GS022 |  | 182 |
| r | GS022 |  | 183 |
| r | GS022 |  | 553 |
| r | GS022 |  | 554 |
| r | GS022 |  | 555 |
| r | GS022 |  | 564 |
| r | GS022 |  | 162 |
| r | GS022 |  | 179 |
| r | GS022 |  | 184 |
| r | GS022 |  | 185 |
| r | GS022 |  | 186 |
| r | GS022 |  | 187 |
| r | GS022 |  | 188 |
| r | GS022 |  | 189 |
| r | GS022 |  | 190 |
| r | GS022 |  | 191 |
| r | GS022 |  | 192 |
| r | GS022 |  | 193 |
| r | GS022 |  | 194 |
| r | GS022 |  | 195 |
| r | GS022 |  | 196 |
| r | GS022 |  | 197 |
| r | GS022 |  | 198 |
| r | GS022 |  | 233 |
| r | GS022 |  | 255 |
| r | GS022 |  | 304 |
| r | GS022 |  | 382 |
| r | GS022 |  | 409 |
| r | GS022 |  | 414 |
| r | GS022 |  | 742 |
| r | GS022 |  | 772 |
| r | GS022 |  | 382 |
| r | GS022 |  | 544 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-07T04:06:46.284733*