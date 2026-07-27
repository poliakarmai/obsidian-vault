---
title: "GSC Audit: /tmp/gsc-learn/fastapi"
date: 2026-07-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/fastapi

**Дата:** 27.07.2026 04:01  
**Путь:** `/tmp/gsc-learn/fastapi`  
**Всего находок:** 177  
**CRITICAL:** 1 | **HIGH:** 9 | **MEDIUM:** 95 | **LOW:** 70

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 80 |
| GS003 | 64 |
| Синхронный код в async | 13 |
| Python: File upload without content-type validation | 8 |
| GS008 | 6 |
| CVE-2026-37270: Hardcoded credential | 1 |
| GS015 | 1 |
| Weak password validation | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| GS009 | 1 |
| GS016 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | models.py | 84 | Match:     enum: Annotated[list[str] | None, Field(min_lengt |
| HIGH | ? | shared.py | 137 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | shared.py | 163 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | shared.py | 168 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | shared.py | 173 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 45 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 46 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 538 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | utils.py | 540 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |

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
| M | ? | routing.py | 347 |
| M | ? | routing.py | 391 |
| M | ? | routing.py | 407 |
| M | ? | routing.py | 476 |
| M | ? | routing.py | 488 |
| M | ? | routing.py | 750 |
| M | ? | routing.py | 772 |
| M | ? | routing.py | 787 |
| M | ? | routing.py | 870 |
| M | ? | routing.py | 1048 |
| M | ? | routing.py | 1075 |
| M | ? | routing.py | 1078 |
| M | ? | routing.py | 1091 |
| M | ? | routing.py | 1502 |
| M | ? | routing.py | 1523 |
| M | ? | routing.py | 1533 |
| M | ? | routing.py | 1907 |
| M | ? | routing.py | 1912 |
| M | ? | routing.py | 2503 |
| M | ? | routing.py | 2504 |
| M | ? | routing.py | 2678 |
| M | ? | routing.py | 3226 |
| M | ? | routing.py | 3230 |
| M | ? | routing.py | 3235 |
| M | ? | routing.py | 3236 |
| M | ? | routing.py | 6367 |
| M | ? | models.py | 19 |
| M | ? | utils.py | 197 |
| M | ? | utils.py | 279 |
| M | ? | utils.py | 284 |
| M | ? | utils.py | 430 |
| M | ? | utils.py | 508 |
| M | ? | encoders.py | 260 |
| M | ? | responses.py | 65 |
| M | ? | responses.py | 95 |
| M | ? | utils.py | 98 |
| M | ? | applications.py | 927 |
| M | ? | applications.py | 928 |
| M | ? | params.py | 185 |
| M | ? | v2.py | 375 |
| M | ? | models.py | 132 |
| M | ? | utils.py | 108 |
| M | ? | utils.py | 116 |
| M | ? | utils.py | 123 |
| M | ? | utils.py | 133 |
| M | ? | utils.py | 343 |
| M | ? | utils.py | 352 |
| M | ? | utils.py | 378 |
| M | ? | utils.py | 382 |
| M | ? | utils.py | 472 |
| M | ? | utils.py | 479 |
| M | ? | utils.py | 488 |
| M | ? | utils.py | 492 |
| M | ? | utils.py | 499 |
| M | ? | utils.py | 527 |
| M | ? | utils.py | 552 |
| M | ? | utils.py | 577 |
| M | ? | utils.py | 581 |
| M | ? | utils.py | 600 |
| M | ? | utils.py | 609 |
| M | ? | utils.py | 642 |
| M | ? | utils.py | 646 |
| M | ? | utils.py | 883 |
| M | ? | utils.py | 895 |
| M | ? | utils.py | 973 |
| M | ? | utils.py | 998 |
| H | ? | shared.py | 137 |
| H | ? | shared.py | 163 |
| H | ? | shared.py | 168 |
| H | ? | shared.py | 173 |
| H | ? | utils.py | 45 |
| H | ? | utils.py | 46 |
| H | ? | utils.py | 538 |
| H | ? | utils.py | 540 |
| M | ? | utils.py | 426 |
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
| L | GS008 | sse.py | 231 |
| L | GS008 | doc_parsing_utils.py | 8 |
| I | GS015 | wsgi.py | 1 |
| C | ? | models.py | 84 |
| H | ? | .pre-commit-config.yaml | 0 |
| s | GS009 |  | 0 |
| M | GS016 | test.sh | 6 |
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
*Сгенерировано GSC v0.6 · 2026-07-27T04:01:46.198107*