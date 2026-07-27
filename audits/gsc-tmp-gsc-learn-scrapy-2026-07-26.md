---
title: "GSC Audit: /tmp/gsc-learn/scrapy"
date: 2026-07-26
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/scrapy

**Дата:** 26.07.2026 04:01  
**Путь:** `/tmp/gsc-learn/scrapy`  
**Всего находок:** 261  
**CRITICAL:** 4 | **HIGH:** 18 | **MEDIUM:** 186 | **LOW:** 52

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 179 |
| GS003 | 45 |
| Хардкод IP адреса | 7 |
| GS008 | 6 |
| CVE-2026-55223: Insecure deserialization | 5 |
| Python: File upload without content-type validation | 4 |
| pickle.load() — unsafe deserialization | 3 |
| CVE-2026-56233: Path traversal | 2 |
| eval() or exec() usage | 2 |
| Bare except: | 1 |
| CVE-2026-37270: Hardcoded credential | 1 |
| GS001 | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| GS009 | 1 |
| GS012 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | default_settings.py | 398 | Found: PASSWORD = "guest" |
| CRITICAL | ? | httpcache.py | 307 | Match:         return cast("dict[str, Any]", pickle.loads(db |
| CRITICAL | ? | httpcache.py | 391 | Match:             return cast("dict[str, Any]", pickle.load |
| CRITICAL | ? | spiderstate.py | 44 | Match:                 spider.state = pickle.load(f)  # type |
| HIGH | ? | feedexport.py | 272 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | feedexport.py | 279 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | feedexport.py | 334 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | images.py | 241 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | lxmlhtml.py | 272 |  |
| HIGH | ? | form.py | 236 |  |
| HIGH | ? | pyproject.toml | 67 | Match:     "brotlicffi>=1.2.0.0; implementation_name == 'pyp |
| HIGH | ? | default_settings.py | 569 | Match: TELNETCONSOLE_HOST = "127.0.0.1" |
| HIGH | ? | tox.ini | 86 | Match:     types-Pygments==2.20.0.20260518 |
| HIGH | ? | tox.ini | 87 | Match:     types-defusedxml==0.7.0.20260504 |
| HIGH | ? | tox.ini | 89 | Match:     types-pexpect==4.9.0.20260518 |
| HIGH | ? | tox.ini | 172 | Match:     brotlicffi >= 1.2.0.0; implementation_name == "py |
| HIGH | ? | tox.ini | 190 | Match:     brotlicffi==1.2.0.0; implementation_name == "pypy |
| HIGH | ? | shell.py | 163 | Match:             print(eval(self.code, globals(), self.var |
| HIGH | ? | engine.py | 35 | Match:             checks += [(test, eval(test))]  # noqa: S |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | defer.py | 440 |
| M | ? | depth.py | 51 |
| M | ? | referer.py | 327 |
| M | ? | urllength.py | 51 |
| M | ? | httperror.py | 81 |
| M | ? | edit.py | 53 |
| M | ? | edit.py | 63 |
| M | ? | runspider.py | 61 |
| M | ? | parse.py | 246 |
| M | ? | parse.py | 267 |
| M | ? | parse.py | 268 |
| M | ? | parse.py | 284 |
| M | ? | parse.py | 329 |
| M | ? | parse.py | 337 |
| M | ? | shell.py | 73 |
| M | ? | shell.py | 121 |
| M | ? | shell.py | 122 |
| M | ? | shell.py | 124 |
| M | ? | shell.py | 129 |
| M | ? | settings.py | 50 |
| M | ? | check.py | 75 |
| M | ? | check.py | 86 |
| M | ? | crawl.py | 30 |
| M | ? | genspider.py | 97 |
| M | ? | genspider.py | 135 |
| M | ? | genspider.py | 156 |
| M | ? | genspider.py | 160 |
| M | ? | genspider.py | 197 |
| M | ? | genspider.py | 232 |
| M | ? | fetch.py | 59 |
| M | ? | fetch.py | 86 |
| M | ? | bench.py | 32 |
| M | ? | bench.py | 43 |
| M | ? | bench.py | 67 |
| M | ? | startproject.py | 135 |
| M | ? | list.py | 21 |
| M | ? | shell.py | 196 |
| M | ? | shell.py | 207 |
| M | ? | shell.py | 241 |
| M | ? | feedexport.py | 222 |
| M | ? | feedexport.py | 300 |
| M | ? | feedexport.py | 445 |
| M | ? | feedexport.py | 458 |
| M | ? | feedexport.py | 561 |
| M | ? | feedexport.py | 582 |
| M | ? | feedexport.py | 644 |
| M | ? | statsmailer.py | 45 |
| M | ? | logstats.py | 40 |
| M | ? | closespider.py | 105 |
| M | ? | closespider.py | 149 |
| M | ? | memdebug.py | 32 |
| M | ? | memusage.py | 80 |
| M | ? | memusage.py | 101 |
| M | ? | memusage.py | 105 |
| M | ? | memusage.py | 106 |
| M | ? | memusage.py | 139 |
| M | ? | memusage.py | 160 |
| M | ? | memusage.py | 161 |
| M | ? | httpcache.py | 76 |
| M | ? | httpcache.py | 264 |
| M | ? | httpcache.py | 329 |
| M | ? | periodic_log.py | 91 |
| M | ? | periodic_log.py | 92 |
| M | ? | periodic_log.py | 93 |
| M | ? | spiderstate.py | 38 |
| M | ? | spiderstate.py | 50 |
| M | ? | debug.py | 48 |
| M | ? | debug.py | 78 |
| M | ? | throttle.py | 101 |
| M | ? | telnet.py | 107 |
| M | ? | corestats.py | 29 |
| M | ? | corestats.py | 44 |
| M | ? | corestats.py | 45 |
| M | ? | protocol.py | 161 |
| M | ? | protocol.py | 225 |
| M | ? | protocol.py | 256 |
| M | ? | protocol.py | 268 |
| M | ? | protocol.py | 275 |
| M | ? | protocol.py | 313 |
| M | ? | protocol.py | 431 |
| M | ? | stream.py | 484 |
| M | ? | agent.py | 119 |
| M | ? | scraper.py | 123 |
| M | ? | scraper.py | 201 |
| M | ? | scraper.py | 211 |
| M | ? | scraper.py | 213 |
| M | ? | scraper.py | 239 |
| M | ? | scraper.py | 269 |
| M | ? | scraper.py | 313 |
| M | ? | scraper.py | 317 |
| M | ? | scraper.py | 355 |
| M | ? | scraper.py | 358 |
| M | ? | scraper.py | 377 |
| M | ? | scraper.py | 459 |
| M | ? | scraper.py | 490 |
| M | ? | scraper.py | 491 |
| M | ? | scheduler.py | 448 |
| M | ? | scheduler.py | 449 |
| M | ? | scheduler.py | 460 |
| M | ? | scheduler.py | 461 |
| M | ? | scheduler.py | 462 |
| M | ? | ftp.py | 124 |
| M | ? | http2.py | 58 |
| M | ? | s3.py | 77 |
| M | ? | http11.py | 199 |
| M | ? | http11.py | 214 |
| M | ? | middleware.py | 102 |
| M | ? | middleware.py | 125 |
| M | ? | middleware.py | 144 |
| M | ? | spidermw.py | 82 |
| M | ? | engine.py | 115 |
| M | ? | engine.py | 275 |
| M | ? | engine.py | 293 |
| M | ? | engine.py | 306 |
| M | ? | engine.py | 347 |
| M | ? | engine.py | 357 |
| M | ? | engine.py | 361 |
| M | ? | engine.py | 362 |
| M | ? | engine.py | 415 |
| M | ? | engine.py | 478 |
| M | ? | engine.py | 488 |
| M | ? | engine.py | 489 |
| M | ? | engine.py | 531 |
| M | ? | engine.py | 545 |
| M | ? | engine.py | 567 |
| M | ? | engine.py | 582 |
| M | ? | engine.py | 657 |
| M | ? | asyncio.py | 183 |
| M | ? | asyncio.py | 184 |
| M | ? | conf.py | 40 |
| M | ? | defer.py | 338 |
| M | ? | iterators.py | 42 |
| M | ? | iterators.py | 52 |
| M | ? | log.py | 33 |
| M | ? | log.py | 34 |
| M | ? | log.py | 242 |
| M | ? | benchserver.py | 20 |
| M | ? | request.py | 216 |
| M | ? | crawler.py | 257 |
| M | ? | crawler.py | 955 |
| M | ? | crawler.py | 974 |
| M | ? | crawler.py | 975 |
| M | ? | crawler.py | 981 |
| M | ? | crawler.py | 1029 |
| M | ? | pqueues.py | 164 |
| M | ? | pqueues.py | 266 |
| M | ? | pqueues.py | 384 |
| M | ? | exporters.py | 322 |
| M | ? | files.py | 370 |
| M | ? | files.py | 371 |
| M | ? | files.py | 375 |
| M | ? | files.py | 376 |
| M | ? | files.py | 685 |
| M | ? | images.py | 173 |
| M | ? | media.py | 84 |
| M | ? | media.py | 125 |
| M | ? | media.py | 211 |
| M | ? | media.py | 256 |
| M | ? | media.py | 306 |
| M | ? | responsetypes.py | 43 |
| M | ? | offsite.py | 32 |
| M | ? | offsite.py | 47 |
| M | ? | retry.py | 97 |
| M | ? | retry.py | 198 |
| M | ? | robotstxt.py | 73 |
| M | ? | robotstxt.py | 80 |
| M | ? | robotstxt.py | 97 |
| M | ? | robotstxt.py | 98 |
| M | ? | robotstxt.py | 119 |
| M | ? | robotstxt.py | 126 |
| M | ? | robotstxt.py | 133 |
| M | ? | robotstxt.py | 136 |
| M | ? | redirect.py | 223 |
| M | ? | httpcache.py | 54 |
| M | ? | cookies.py | 66 |
| M | ? | stats.py | 46 |
| M | ? | form.py | 155 |
| M | ? | form.py | 306 |
| M | ? | dupefilters.py | 98 |
| M | ? | dupefilters.py | 137 |
| H | ? | feedexport.py | 272 |
| H | ? | feedexport.py | 279 |
| H | ? | feedexport.py | 334 |
| H | ? | images.py | 241 |
| M | ? | httpcache.py | 307 |
| M | ? | httpcache.py | 391 |
| M | ? | spiderstate.py | 44 |
| M | ? | squeues.py | 152 |
| M | ? | squeues.py | 157 |
| H | ? | lxmlhtml.py | 272 |
| H | ? | form.py | 236 |
| M | ? | scheduler.py | 454 |
| C | GS001 | default_settings.py | 398 |
| L | GS003 | qps-bench-server.py | 40 |
| L | GS003 | cmdline.py | 103 |
| L | GS003 | cmdline.py | 106 |
| L | GS003 | cmdline.py | 111 |
| L | GS003 | cmdline.py | 117 |
| L | GS003 | cmdline.py | 124 |
| L | GS003 | cmdline.py | 128 |
| L | GS003 | cmdline.py | 137 |
| L | GS003 | cmdline.py | 142 |
| L | GS003 | cmdline.py | 150 |
| L | GS003 | check.py | 107 |
| L | GS003 | fetch.py | 61 |
| L | GS003 | genspider.py | 104 |
| L | GS003 | genspider.py | 114 |
| L | GS003 | genspider.py | 168 |
| L | GS003 | genspider.py | 173 |
| L | GS003 | genspider.py | 180 |
| L | GS003 | genspider.py | 187 |
| L | GS003 | genspider.py | 202 |
| L | GS003 | genspider.py | 213 |
| L | GS003 | genspider.py | 225 |
| L | GS003 | list.py | 23 |
| L | GS003 | parse.py | 171 |
| L | GS003 | parse.py | 182 |
| L | GS003 | parse.py | 191 |
| L | GS003 | parse.py | 197 |
| L | GS003 | settings.py | 55 |
| L | GS003 | settings.py | 57 |
| L | GS003 | settings.py | 59 |
| L | GS003 | settings.py | 61 |
| L | GS003 | settings.py | 63 |
| L | GS003 | settings.py | 65 |
| L | GS003 | startproject.py | 51 |
| L | GS003 | startproject.py | 56 |
| L | GS003 | startproject.py | 102 |
| L | GS003 | startproject.py | 124 |
| L | GS003 | version.py | 34 |
| L | GS003 | version.py | 36 |
| L | GS003 | shell.py | 163 |
| L | GS003 | shell.py | 271 |
| L | GS003 | benchserver.py | 45 |
| L | GS003 | console.py | 67 |
| L | GS003 | display.py | 51 |
| L | GS003 | engine.py | 53 |
| L | GS003 | trackref.py | 70 |
| L | GS008 | default_settings.py | 275 |
| L | GS008 | _deps_compat.py | 14 |
| L | GS008 | _deps_compat.py | 16 |
| L | GS008 | _deps_compat.py | 18 |
| L | GS008 | _deps_compat.py | 22 |
| L | GS008 | _deps_compat.py | 24 |
| H | ? | pyproject.toml | 67 |
| H | ? | default_settings.py | 569 |
| H | ? | tox.ini | 86 |
| H | ? | tox.ini | 87 |
| H | ? | tox.ini | 89 |
| H | ? | tox.ini | 172 |
| H | ? | tox.ini | 190 |
| H | ? | shell.py | 163 |
| H | ? | engine.py | 35 |
| C | ? | httpcache.py | 307 |
| C | ? | httpcache.py | 391 |
| C | ? | spiderstate.py | 44 |
| H | ? | codecov.yml | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| s | GS009 |  | 0 |
| L | GS012 | datatypes.py | 86 |

---
*Сгенерировано GSC v0.6 · 2026-07-26T04:01:09.018749*