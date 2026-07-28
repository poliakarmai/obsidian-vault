---
title: "GSC Audit: /tmp/gsc-learn/tornado"
date: 2026-07-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/tornado

**Дата:** 28.07.2026 04:01  
**Путь:** `/tmp/gsc-learn/tornado`  
**Всего находок:** 562  
**CRITICAL:** 1 | **HIGH:** 19 | **MEDIUM:** 144 | **LOW:** 394

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 128 |
| GS003 | 36 |
| Хардкод IP адреса | 12 |
| Bare except: | 8 |
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
| GS008 | 4 |
| GS015 | 3 |
| Python: File upload without content-type validation | 2 |
| eval() or exec() usage | 2 |
| CVE-2026-56318: Information disclosure | 1 |
| Hardcoded encryption key | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS004 | 1 |
| GS009 | 1 |
| GS014 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
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
| s | GS009 |  | 0 |
| M | GS014 | test.key | 1 |

---
*Сгенерировано GSC v0.6 · 2026-07-28T04:01:18.721225*