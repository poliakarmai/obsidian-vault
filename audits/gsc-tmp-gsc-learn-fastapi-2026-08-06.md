---
title: "GSC Audit: /tmp/gsc-learn/fastapi"
date: 2026-08-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/fastapi

**Дата:** 06.08.2026 04:19  
**Путь:** `/tmp/gsc-learn/fastapi`  
**Всего находок:** 252  
**CRITICAL:** 6 | **HIGH:** 11 | **MEDIUM:** 95 | **LOW:** 70

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 80 |
| GS003 | 64 |
| GS021 | 34 |
| GS022 | 13 |
| Синхронный код в async | 13 |
| Python: File upload without content-type validation | 8 |
| GS020 | 8 |
| GS025-hardcoded_secret | 7 |
| GS008 | 6 |
| GS001 | 5 |
| GS025-eval_usage | 4 |
| GS019 | 2 |
| GS025-wildcard_bind | 2 |
| CVE-2026-37270: Hardcoded credential | 1 |
| GS015 | 1 |
| Weak password validation | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| GS009 | 1 |
| GS016 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | pyproject.toml | 299 | Found: "UP012" |
| CRITICAL | GS001 | pyproject.toml | 300 | Found: "UP028" |
| CRITICAL | GS001 | pyproject.toml | 301 | Found: "UP028" |
| CRITICAL | GS001 | pyproject.toml | 302 | Found: "UP028" |
| CRITICAL | GS001 | pyproject.toml | 303 | Found: "UP028" |
| CRITICAL | ? | models.py | 84 | Match:     enum: Annotated[list[str] | None, Field(min_lengt |
| HIGH | ? | shared.py | 145 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | shared.py | 171 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | shared.py | 176 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | shared.py | 181 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 45 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 46 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 498 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 500 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS019 | oauth2.py | 40 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | oauth2.py | 194 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | doc_parsing_utils.py | 374 |
| M | ? | doc_parsing_utils.py | 376 |
| M | ? | doc_parsing_utils.py | 379 |
| M | ? | doc_parsing_utils.py | 381 |
| M | ? | doc_parsing_utils.py | 387 |
| M | ? | doc_parsing_utils.py | 388 |
| M | ? | doc_parsing_utils.py | 389 |
| M | ? | translate.py | 43 |
| M | ? | translate.py | 53 |
| M | ? | translate.py | 112 |
| M | ? | translate.py | 120 |
| M | ? | translate.py | 124 |
| M | ? | deploy_docs_status.py | 59 |
| M | ? | deploy_docs_status.py | 69 |
| M | ? | routing.py | 349 |
| M | ? | routing.py | 393 |
| M | ? | routing.py | 409 |
| M | ? | routing.py | 478 |
| M | ? | routing.py | 490 |
| M | ? | routing.py | 758 |
| M | ? | routing.py | 780 |
| M | ? | routing.py | 795 |
| M | ? | routing.py | 878 |
| M | ? | routing.py | 1040 |
| M | ? | routing.py | 1043 |
| M | ? | routing.py | 1056 |
| M | ? | routing.py | 1104 |
| M | ? | routing.py | 1509 |
| M | ? | routing.py | 1530 |
| M | ? | routing.py | 1540 |
| M | ? | routing.py | 1932 |
| M | ? | routing.py | 1937 |
| M | ? | routing.py | 2539 |
| M | ? | routing.py | 2540 |
| M | ? | routing.py | 2720 |
| M | ? | routing.py | 3268 |
| M | ? | routing.py | 3272 |
| M | ? | routing.py | 3277 |
| M | ? | routing.py | 3278 |
| M | ? | routing.py | 6409 |
| M | ? | models.py | 19 |
| M | ? | utils.py | 242 |
| M | ? | utils.py | 324 |
| M | ? | utils.py | 329 |
| M | ? | utils.py | 487 |
| M | ? | utils.py | 564 |
| M | ? | encoders.py | 260 |
| M | ? | responses.py | 65 |
| M | ? | responses.py | 95 |
| M | ? | utils.py | 98 |
| M | ? | applications.py | 927 |
| M | ? | applications.py | 928 |
| M | ? | params.py | 185 |
| M | ? | v2.py | 375 |
| M | ? | models.py | 133 |
| M | ? | utils.py | 108 |
| M | ? | utils.py | 116 |
| M | ? | utils.py | 123 |
| M | ? | utils.py | 133 |
| M | ? | utils.py | 303 |
| M | ? | utils.py | 312 |
| M | ? | utils.py | 338 |
| M | ? | utils.py | 342 |
| M | ? | utils.py | 432 |
| M | ? | utils.py | 439 |
| M | ? | utils.py | 448 |
| M | ? | utils.py | 452 |
| M | ? | utils.py | 459 |
| M | ? | utils.py | 487 |
| M | ? | utils.py | 512 |
| M | ? | utils.py | 537 |
| M | ? | utils.py | 541 |
| M | ? | utils.py | 560 |
| M | ? | utils.py | 569 |
| M | ? | utils.py | 602 |
| M | ? | utils.py | 606 |
| M | ? | utils.py | 843 |
| M | ? | utils.py | 855 |
| M | ? | utils.py | 933 |
| M | ? | utils.py | 958 |
| H | ? | shared.py | 145 |
| H | ? | shared.py | 171 |
| H | ? | shared.py | 176 |
| H | ? | shared.py | 181 |
| H | ? | utils.py | 45 |
| H | ? | utils.py | 46 |
| H | ? | utils.py | 498 |
| H | ? | utils.py | 500 |
| M | ? | utils.py | 483 |
| C | GS001 | pyproject.toml | 299 |
| C | GS001 | pyproject.toml | 300 |
| C | GS001 | pyproject.toml | 301 |
| C | GS001 | pyproject.toml | 302 |
| C | GS001 | pyproject.toml | 303 |
| L | GS003 | cli.py | 11 |
| L | GS003 | add_latest_release_date.py | 24 |
| L | GS003 | add_latest_release_date.py | 29 |
| L | GS003 | add_latest_release_date.py | 34 |
| L | GS003 | deploy_docs_status.py | 131 |
| L | GS003 | doc_parsing_utils.py | 599 |
| L | GS003 | doc_parsing_utils.py | 690 |
| L | GS003 | doc_parsing_utils.py | 700 |
| L | GS003 | doc_parsing_utils.py | 710 |
| L | GS003 | doc_parsing_utils.py | 720 |
| L | GS003 | doc_parsing_utils.py | 730 |
| L | GS003 | docs.py | 144 |
| L | GS003 | translate.py | 132 |
| L | GS003 | translate.py | 134 |
| L | GS003 | translate.py | 140 |
| L | GS003 | translate.py | 165 |
| L | GS003 | translate.py | 175 |
| L | GS003 | translate.py | 176 |
| L | GS003 | translate.py | 216 |
| L | GS003 | translate.py | 218 |
| L | GS003 | translate.py | 219 |
| L | GS003 | translate.py | 228 |
| L | GS003 | translate.py | 230 |
| L | GS003 | translate.py | 231 |
| L | GS003 | translate.py | 232 |
| L | GS003 | translate.py | 234 |
| L | GS003 | translate.py | 235 |
| L | GS003 | translate.py | 237 |
| L | GS003 | translate.py | 239 |
| L | GS003 | translate.py | 257 |
| L | GS003 | translate.py | 268 |
| L | GS003 | translate.py | 272 |
| L | GS003 | translate.py | 294 |
| L | GS003 | translate.py | 298 |
| L | GS003 | translate.py | 309 |
| L | GS003 | translate.py | 322 |
| L | GS003 | translate.py | 331 |
| L | GS003 | translate.py | 332 |
| L | GS003 | translate.py | 340 |
| L | GS003 | translate.py | 341 |
| L | GS003 | translate.py | 352 |
| L | GS003 | translate.py | 375 |
| L | GS003 | translate.py | 386 |
| L | GS003 | translate.py | 388 |
| L | GS003 | translate.py | 389 |
| L | GS003 | translate.py | 399 |
| L | GS003 | translate.py | 401 |
| L | GS003 | translate.py | 402 |
| L | GS003 | translate.py | 410 |
| L | GS003 | translate.py | 412 |
| L | GS003 | translate.py | 414 |
| L | GS003 | translate.py | 428 |
| L | GS003 | translate.py | 431 |
| L | GS003 | translate.py | 440 |
| L | GS003 | translate.py | 450 |
| L | GS003 | translate.py | 454 |
| L | GS003 | translate.py | 455 |
| L | GS003 | translate.py | 458 |
| L | GS003 | translate.py | 465 |
| L | GS003 | translate.py | 468 |
| L | GS003 | translate.py | 480 |
| L | GS003 | translate.py | 481 |
| L | GS003 | translation_fixer.py | 76 |
| L | GS003 | translation_fixer.py | 97 |
| L | GS008 | shared.py | 31 |
| L | GS008 | constants.py | 1 |
| L | GS008 | constants.py | 2 |
| L | GS008 | constants.py | 3 |
| L | GS008 | sse.py | 237 |
| L | GS008 | doc_parsing_utils.py | 8 |
| I | GS015 | wsgi.py | 1 |
| i | GS020 |  | 86 |
| i | GS020 |  | 134 |
| i | GS020 |  | 139 |
| i | GS020 |  | 154 |
| i | GS020 |  | 228 |
| i | GS020 |  | 228 |
| i | GS020 |  | 250 |
| i | GS020 |  | 309 |
| C | ? | models.py | 84 |
| H | ? | .pre-commit-config.yaml | 0 |
| s | GS009 |  | 0 |
| M | GS016 | test.sh | 6 |
| H | GS019 | oauth2.py | 40 |
| H | GS019 | oauth2.py | 194 |
| s | GS021 |  | 456 |
| s | GS021 |  | 473 |
| s | GS021 |  | 2508 |
| s | GS021 |  | 852 |
| s | GS021 |  | 37 |
| s | GS021 |  | 39 |
| s | GS021 |  | 24 |
| s | GS021 |  | 21 |
| s | GS021 |  | 15 |
| s | GS021 |  | 7 |
| s | GS021 |  | 8 |
| s | GS021 |  | 9 |
| s | GS021 |  | 10 |
| s | GS021 |  | 8 |
| s | GS021 |  | 8 |
| s | GS021 |  | 14 |
| s | GS021 |  | 30 |
| s | GS021 |  | 14 |
| s | GS021 |  | 30 |
| s | GS021 |  | 14 |
| s | GS021 |  | 31 |
| s | GS021 |  | 14 |
| s | GS021 |  | 31 |
| s | GS021 |  | 14 |
| s | GS021 |  | 30 |
| s | GS021 |  | 16 |
| s | GS021 |  | 32 |
| s | GS021 |  | 12 |
| s | GS021 |  | 12 |
| s | GS021 |  | 12 |
| s | GS021 |  | 12 |
| s | GS021 |  | 12 |
| s | GS021 |  | 16 |
| s | GS021 |  | 34 |
| r | GS022 |  | 180 |
| r | GS022 |  | 186 |
| r | GS022 |  | 279 |
| r | GS022 |  | 297 |
| r | GS022 |  | 419 |
| r | GS022 |  | 191 |
| r | GS022 |  | 240 |
| r | GS022 |  | 316 |
| r | GS022 |  | 321 |
| r | GS022 |  | 326 |
| r | GS022 |  | 332 |
| r | GS022 |  | 1956 |
| r | GS022 |  | 2756 |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| M | ? | docs.py | 285 |
| M | ? | translate.py | 433 |
| M | ? | translate.py | 434 |
| M | ? | translate.py | 451 |
| M | ? | translate.py | 457 |
| M | ? | translate.py | 464 |
| M | ? | translate.py | 466 |
| M | ? | topic_repos.py | 59 |
| M | ? | topic_repos.py | 60 |
| M | ? | topic_repos.py | 66 |
| M | ? | topic_repos.py | 68 |
| M | ? | topic_repos.py | 71 |
| M | ? | topic_repos.py | 73 |

---
*Сгенерировано GSC v0.6 · 2026-08-06T04:19:24.416197*