---
title: "GSC Audit: /tmp/gsc-learn/django"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/django

**Дата:** 07.08.2026 04:05  
**Путь:** `/tmp/gsc-learn/django`  
**Всего находок:** 2763  
**CRITICAL:** 351 | **HIGH:** 187 | **MEDIUM:** 86 | **LOW:** 1416

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 1162 |
| GS022 | 336 |
| GS001 | 311 |
| GS025-debug_mode | 113 |
| GS025-eval_usage | 102 |
| GS021 | 91 |
| Python: File upload without content-type validation | 59 |
| GS003 | 50 |
| Rust: .clone() in hot path | 47 |
| Python: assert in production | 36 |
| GS020 | 30 |
| GS012 | 28 |
| GS007 | 27 |
| GS015 | 23 |
| eval() or exec() usage | 22 |
| CVE-2026-37270: Hardcoded credential | 21 |
| Хардкод IP адреса | 18 |
| GS025-hardcoded_secret | 11 |
| CVE-2026-55223: Insecure deserialization | 10 |
| Hardcoded encryption key | 9 |
| pickle.load() — unsafe deserialization | 9 |
| GS005 | 9 |
| SQL injection risk: f-string in query | 7 |
| Синхронный код в async | 7 |
| CVE-2026-54696: Buffer overflow | 6 |
| CVE-2026-56233: Path traversal | 6 |
| CVE-2026-56318: Information disclosure | 6 |
| GS019 | 5 |
| CVE-2026-55721: SQL injection | 4 |
| GS004 | 4 |
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
| GS018 | 3 |
| GS025-insecure_random | 3 |
| Python: raw string concatenation in SQL | 1 |
| Rails: params without permit | 1 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 1 |
| Debug mode enabled | 1 |
| World-readable file: package.json (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| World-readable file: biome.json (664) | 1 |
| World-readable file: zizmor.yml (664) | 1 |
| GS009 | 1 |
| GS017 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | text.py | 273 | OWASP A03: Injection |
| CRITICAL | ? | operations.py | 113 | OWASP A03: Injection |
| CRITICAL | ? | operations.py | 277 | OWASP A03: Injection |
| CRITICAL | ? | operations.py | 280 | OWASP A03: Injection |
| CRITICAL | ? | operations.py | 73 | OWASP A03: Injection |
| CRITICAL | ? | operations.py | 684 | OWASP A03: Injection |
| CRITICAL | ? | operations.py | 155 | OWASP A03: Injection |
| CRITICAL | ? | operations.py | 145 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | operations.py | 113 |  |
| CRITICAL | ? | operations.py | 73 |  |
| CRITICAL | ? | operations.py | 684 |  |
| CRITICAL | ? | operations.py | 155 |  |
| CRITICAL | GS001 | django.po | 696 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 699 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 731 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 556 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 559 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 586 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 708 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 711 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 744 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 649 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 652 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 684 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 561 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 564 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 588 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 711 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 714 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 747 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 729 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 732 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 765 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 710 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 713 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 745 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 623 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 626 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 659 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 592 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 595 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 619 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 580 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 583 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 609 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 718 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 721 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 753 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 729 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 732 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 765 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 733 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 736 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 769 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 592 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 595 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 625 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 724 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 727 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 760 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 710 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 713 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 746 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 702 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 705 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 738 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 645 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 648 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 682 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 918 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 922 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 951 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 635 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 636 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 638 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 639 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 670 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 671 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 610 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 611 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 613 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 614 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 639 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 640 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 639 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 642 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 674 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 753 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 756 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 790 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 718 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 721 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 755 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 610 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 613 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 647 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 634 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 637 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 666 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 610 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 613 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 648 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 711 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 714 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 746 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 643 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 646 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 678 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 708 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 711 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 743 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 696 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 699 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 731 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 743 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 746 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 781 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 531 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 534 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 558 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 715 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 718 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 751 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 660 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 663 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 698 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 714 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 717 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 749 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 708 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 711 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 743 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 623 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 626 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 654 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 717 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 720 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 752 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 703 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 706 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 738 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 706 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 709 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 742 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 679 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 682 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 710 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 586 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 589 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 616 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 706 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 709 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 743 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 585 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 588 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 618 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 629 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 632 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 666 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 705 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 706 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 708 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 709 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 740 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 741 | Found: password:"

msgid " |
| CRITICAL | GS001 | django.po | 719 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 722 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 754 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 678 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 681 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 709 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 556 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 559 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 583 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 614 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 617 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 643 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 561 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 564 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 588 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 564 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 567 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 591 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 748 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 751 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 783 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 626 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 629 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 659 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 557 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 560 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 584 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 736 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 739 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 772 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 712 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 715 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 747 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 641 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 644 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 672 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 617 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 620 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 648 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 695 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 698 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 730 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 676 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 679 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 711 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 631 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 634 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 667 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 554 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 557 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 581 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 630 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 633 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 666 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 606 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 609 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 634 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 727 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 730 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 763 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 646 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 649 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 682 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 582 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 585 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 615 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 625 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 628 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 654 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 732 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 735 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 768 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 723 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 726 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 759 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 741 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 744 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 776 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 669 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 672 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 704 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 727 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 730 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 764 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 714 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 717 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 749 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 682 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 685 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 717 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 710 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 713 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 746 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 729 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 732 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 764 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 729 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 732 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 764 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 723 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 726 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 759 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 687 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 690 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 722 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 568 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 571 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 595 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 565 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 568 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 592 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 615 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 618 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 647 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 590 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 593 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 619 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 656 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 659 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 683 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 731 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 734 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 766 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 578 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 581 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 607 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 528 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 531 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 555 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 708 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 711 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 746 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 718 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 721 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 753 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 702 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 705 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 737 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 642 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 645 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 669 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 637 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 640 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 672 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 706 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 709 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 737 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 685 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 688 | Found: password:"
msgstr " |
| CRITICAL | GS001 | django.po | 716 | Found: password:"
msgstr " |
| CRITICAL | GS001 | password_reset_confirm.html | 28 | Found: password:' %}</label>
        {{ form.new_password1.e |
| CRITICAL | GS001 | password_reset_confirm.html | 35 | Found: password:' %}</label>
        {{ form.new_password2.e |
| CRITICAL | GS001 | password_reset_email.html | 4 | Found: password:" %}
{% block reset_link %}
{{ protocol }}:/ |
| CRITICAL | GS001 | changepassword.py | 17 | Found: Password: "):
        p = getpass.getpass(prompt=prom |
| CRITICAL | GS001 | views.py | 246 | Found: TOKEN = "_password_reset_token" |
| CRITICAL | GS001 | creation.py | 292 | Found: password = 'ALTER USER %(user)s IDENTIFIED BY " |
| CRITICAL | GS001 | text.py | 25 | Found: 'AL32UTF8' |
| CRITICAL | GS001 | pyproject.toml | 57 | Found: "py312" |
| CRITICAL | ? | widgets.py | 673 | Match:     format_key = "DATE_INPUT_FORMATS" |
| CRITICAL | ? | widgets.py | 678 | Match:     format_key = "DATETIME_INPUT_FORMATS" |
| CRITICAL | ? | widgets.py | 683 | Match:     format_key = "TIME_INPUT_FORMATS" |
| CRITICAL | ? | creation.py | 292 | Match:             set_password = 'ALTER USER %(user)s IDENT |
| CRITICAL | ? | views.py | 262 | Match:     reset_url_token = "set-password" |
| CRITICAL | ? | session.py | 13 | Match:     session_key = "_messages" |
| CRITICAL | ? | cookie.py | 16 | Match:     message_key = "__json_message" |
| CRITICAL | ? | loader_tags.py | 88 | Match:     context_key = "extends_context" |
| CRITICAL | ? | loader_tags.py | 164 | Match:     context_key = "__include_context" |
| CRITICAL | ? | filebased.py | 38 | Match:                     return pickle.loads(zlib.decompre |
| CRITICAL | ? | filebased.py | 71 | Match:                         previous_value = pickle.loads |
| CRITICAL | ? | filebased.py | 154 | Match:             exp = pickle.load(f) |
| CRITICAL | ? | redis.py | 29 | Match:             return pickle.loads(data) |
| CRITICAL | ? | db.py | 102 | Match:                 value = pickle.loads(base64.b64decode |
| CRITICAL | ? | locmem.py | 43 | Match:         return pickle.loads(pickled) |
| CRITICAL | ? | locmem.py | 73 | Match:             value = pickle.loads(pickled) |
| CRITICAL | ? | runner.py | 208 | Match:         pickle.loads(pickle.dumps(obj)) |
| CRITICAL | ? | testcases.py | 88 | Match:         pickle.loads(pickle.dumps(obj)) |
| CRITICAL | GS005 | introspection.py | 17 | Line 17: cursor.execute("DESCRIBE %s" % self.connection.ops. |
| CRITICAL | GS005 | operations.py | 341 | Line 341: cursor.execute("SELECT %s()" % func) |
| CRITICAL | GS005 | operations.py | 161 | Line 161: cursor.execute("SELECT %s" % func) |
| CRITICAL | GS005 | db.py | 136 | Line 136: cursor.execute("SELECT COUNT(*) FROM %s" % table) |
| CRITICAL | GS005 | db.py | 302 | Line 302: cursor.execute("DELETE FROM %s" % table) |
| CRITICAL | GS005 | operations.py | 354 | Line 354: cursor.execute('"%s".currval' % sq_name) |
| CRITICAL | GS005 | base.py | 331 | Line 331: self.cursor().execute(f"BEGIN {self.transaction_mo |
| CRITICAL | GS005 | compiler.py | 445 | Line 445: RawSQL("%s.%s" % (self.quote_name(table), col), [] |
| CRITICAL | GS005 | compiler.py | 2028 | Line 2028: innerq = RawSQL("SELECT * FROM (%s) subquery" % s |
| CRITICAL | GS017 | registry.py | 11 | Hardcoded default credential pair detected. Common in pentes |
| HIGH | ? | widgets.py | 538 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | widgets.py | 625 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 574 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 791 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 795 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | query.py | 736 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | query.py | 1120 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | query.py | 1122 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | files.py | 101 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | files.py | 107 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | files.py | 127 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | files.py | 341 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | files.py | 356 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | related_descriptors.py | 880 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | related_descriptors.py | 986 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | creation.py | 188 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | edit.py | 133 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | loaddata.py | 210 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | base.py | 328 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | uploadhandler.py | 9 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | client.py | 818 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | client.py | 894 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | layermapping.py | 673 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | base_session.py | 21 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | middleware.py | 60 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | cache.py | 57 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | file.py | 114 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | file.py | 187 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | signed_cookies.py | 49 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | signed_cookies.py | 80 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | cached_db.py | 89 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | db.py | 74 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | db.py | 127 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | db.py | 153 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | management.py | 37 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | collectstatic.py | 402 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 242 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 322 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 369 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | changepassword.py | 80 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 134 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 209 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 247 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 24 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 168 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | admin.py | 179 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | base_user.py | 62 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | base_user.py | 107 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 49 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | options.py | 1449 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | options.py | 1455 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | options.py | 1471 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | fields.py | 756 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 74 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | multipartparser.py | 185 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | multipartparser.py | 195 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | multipartparser.py | 287 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | multipartparser.py | 361 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | multipartparser.py | 536 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | inspectdb.py | 151 | Hacking APIs Ch.11 |
| HIGH | ? | shortcuts.py | 196 |  |
| HIGH | ? | runserver.py | 131 |  |
| HIGH | ? | layermapping.py | 697 |  |
| HIGH | ? | loader_tags.py | 256 |  |
| HIGH | ? | loader_tags.py | 274 |  |
| HIGH | ? | request.py | 289 |  |
| HIGH | ? | manage_translations.py | 76 |  |
| HIGH | ? | runserver.py | 33 | Match:     default_addr = "127.0.0.1" |
| HIGH | ? | runserver.py | 178 | Match:             addr = "0.0.0.0" |
| HIGH | ? | client.py | 420 | Match:             "REMOTE_ADDR": "127.0.0.1", |
| HIGH | ? | client.py | 701 | Match:             "client": ["127.0.0.1", 0], |
| HIGH | ? | client.py | 754 | Match:             "server": ("127.0.0.1", "443" if secure e |
| HIGH | ? | selenium.py | 46 | Match:             host = test_class.host if not test_class. |
| HIGH | ? | request.py | 197 | Match:             allowed_hosts = [".localhost", "127.0.0.1 |
| HIGH | ? | formats.py | 34 | Match:     "%d-%m-%Y %H.%M.%S.%f",  # '25-10-2009 14.30.59.0 |
| HIGH | ? | formats.py | 37 | Match:     "%d-%m-%y %H.%M.%S.%f",  # '25-10-09' 14.30.59.00 |
| HIGH | ? | formats.py | 40 | Match:     "%m/%d/%y %H.%M.%S.%f",  # '10/25/06 14.30.59.000 |
| HIGH | ? | formats.py | 43 | Match:     "%m/%d/%Y %H.%M.%S.%f",  # '25/10/2009 14.30.59.0 |
| HIGH | ? | formats.py | 26 | Match:     "%H.%M.%S.%f",  # '14.30.59.000200' |
| HIGH | ? | formats.py | 40 | Match:     "%d.%m.%y %H.%M.%S.%f",  # '25.10.06 14.30.59.000 |
| HIGH | ? | formats.py | 27 | Match:     "%H.%M.%S.%f",  # '14.30.59.000200' |
| HIGH | ? | formats.py | 41 | Match:     "%d.%m.%y %H.%M.%S.%f",  # '25.10.06 14.30.59.000 |
| HIGH | ? | formats.py | 22 | Match:     "%d.%m.%Y %H.%M.%S.%f",  # '20.3.2014 14.30.59.00 |
| HIGH | ? | formats.py | 25 | Match:     "%d.%m.%y %H.%M.%S.%f",  # '20.3.14 14.30.59.0002 |
| HIGH | ? | formats.py | 30 | Match:     "%H.%M.%S.%f",  # '14.30.59.000200' |
| HIGH | ? | csrf.py | 67 | Match:         "more": _("More information is available with |
| HIGH | ? | manage_translations.py | 404 | Match:     eval(cmd)(**kwargs) |
| HIGH | ? | shell.py | 89 | Match:                     exec(compile(pythonrc_code, pytho |
| HIGH | ? | shell.py | 262 | Match:             exec(options["command"], {**globals(), ** |
| HIGH | ? | shell.py | 272 | Match:             exec(sys.stdin.read(), {**globals(), **se |
| HIGH | ? | defaulttags.py | 326 | Match:                     match = condition.eval(context) |
| HIGH | ? | defaulttags.py | 917 | Match:     def eval(self, context): |
| HIGH | ? | smartif.py | 59 | Match:         def eval(self, context): |
| HIGH | ? | smartif.py | 86 | Match:         def eval(self, context): |
| HIGH | ? | smartif.py | 99 | Match:     "or": infix(6, lambda context, x, y: x.eval(conte |
| HIGH | ? | smartif.py | 100 | Match:     "and": infix(7, lambda context, x, y: x.eval(cont |
| HIGH | ? | smartif.py | 101 | Match:     "not": prefix(8, lambda context, x: not x.eval(co |
| HIGH | ? | smartif.py | 102 | Match:     "in": infix(9, lambda context, x, y: x.eval(conte |
| HIGH | ? | smartif.py | 103 | Match:     "not in": infix(9, lambda context, x, y: x.eval(c |
| HIGH | ? | smartif.py | 104 | Match:     "is": infix(10, lambda context, x, y: x.eval(cont |
| HIGH | ? | smartif.py | 105 | Match:     "is not": infix(10, lambda context, x, y: x.eval( |
| HIGH | ? | smartif.py | 106 | Match:     "==": infix(10, lambda context, x, y: x.eval(cont |
| HIGH | ? | smartif.py | 107 | Match:     "!=": infix(10, lambda context, x, y: x.eval(cont |
| HIGH | ? | smartif.py | 108 | Match:     ">": infix(10, lambda context, x, y: x.eval(conte |
| HIGH | ? | smartif.py | 109 | Match:     ">=": infix(10, lambda context, x, y: x.eval(cont |
| HIGH | ? | smartif.py | 110 | Match:     "<": infix(10, lambda context, x, y: x.eval(conte |
| HIGH | ? | smartif.py | 111 | Match:     "<=": infix(10, lambda context, x, y: x.eval(cont |
| HIGH | ? | smartif.py | 144 | Match:     def eval(self, context): |
| HIGH | ? | package.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | biome.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | zizmor.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | shell.py | 89 | Line 89: exec(compile(pythonrc_code, pythonrc, "exec"), impo |
| HIGH | GS004 | shell.py | 262 | Line 262: exec(options["command"], {**globals(), **self.get_ |
| HIGH | GS004 | shell.py | 272 | Line 272: exec(sys.stdin.read(), {**globals(), **self.get_na |
| HIGH | GS004 | version.py | 90 | Line 90: git_log = subprocess.run( |
| HIGH | GS007 | models.py | 54 | Line 54: return self.model.objects.bulk_create(log_entry_lis |
| HIGH | GS007 | migrate.py | 370 | Line 370: with post_migrate_apps.bulk_update(): |
| HIGH | GS007 | base.py | 2544 | Line 2544: ordered_obj.objects.db_manager(using).filter(**fi |
| HIGH | GS007 | related_descriptors.py | 1603 | Line 1603: self.through._default_manager.using(db).bulk_crea |
| HIGH | GS007 | related_descriptors.py | 1633 | Line 1633: self.through._default_manager.using(db).bulk_crea |
| HIGH | GS007 | query.py | 800 | Line 800: "bulk_create() can only be used with concrete fiel |
| HIGH | GS007 | query.py | 805 | Line 805: "bulk_create() cannot be used with primary keys in |
| HIGH | GS007 | query.py | 811 | Line 811: "bulk_create() can only be used with concrete fiel |
| HIGH | GS007 | query.py | 817 | Line 817: def bulk_create( |
| HIGH | GS007 | query.py | 975 | Line 975: def bulk_update(self, objs, fields, batch_size=Non |
| HIGH | GS007 | query.py | 982 | Line 982: raise ValueError("Field names must be given to bul |
| HIGH | GS007 | query.py | 985 | Line 985: raise ValueError("All bulk_update() objects must h |
| HIGH | GS007 | query.py | 989 | Line 989: raise ValueError("bulk_update() can only be used w |
| HIGH | GS007 | query.py | 994 | Line 994: raise ValueError("bulk_update() cannot be used wit |
| HIGH | GS012 | inspectdb.py | 151 | Direct params in model create/update bypasses strong paramet |
| HIGH | GS018 | base.py | 333 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | query.py | 1948 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | transaction.py | 47 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS019 | sites.py | 412 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | backends.py | 16 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | backends.py | 65 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | backends.py | 270 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | context_processors.py | 49 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | ? | special.py | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | special.py | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | expressions.py | 1829 | Clone in performance-critical code — consider references |
| HIGH | ? | expressions.py | 1863 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 1377 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 2364 | Clone in performance-critical code — consider references |
| HIGH | ? | generated.py | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | tuple_lookups.py | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | query_utils.py | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | query_utils.py | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | query_utils.py | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 534 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 663 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 690 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 783 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 1261 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 1767 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 1982 | Clone in performance-critical code — consider references |
| HIGH | ? | query.py | 2379 | Clone in performance-critical code — consider references |
| HIGH | ? | where.py | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | where.py | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | where.py | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | subqueries.py | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | compiler.py | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | compiler.py | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | compiler.py | 2018 | Clone in performance-critical code — consider references |
| HIGH | ? | options.py | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.py | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | schema.py | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | migrate.py | 358 | Clone in performance-critical code — consider references |
| HIGH | ? | adapter.py | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | adapter.py | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | geometry.py | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | geometry.py | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | geometry.py | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | geometry.py | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | geometry.py | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | OLMapWidget.js | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | geometries.py | 470 | Clone in performance-critical code — consider references |
| HIGH | ? | array.py | 151 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | text.py | 273 |
| C | ? | operations.py | 113 |
| C | ? | operations.py | 277 |
| C | ? | operations.py | 280 |
| C | ? | operations.py | 73 |
| C | ? | operations.py | 684 |
| C | ? | operations.py | 155 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| L | ? | manage_translations.py | 132 |
| L | ? | utils.py | 132 |
| L | ? | operations.py | 109 |
| M | ? | manage_translations.py | 60 |
| M | ? | expressions.py | 213 |
| M | ? | expressions.py | 1419 |
| M | ? | query.py | 913 |
| M | ? | base.py | 975 |
| M | ? | base.py | 976 |
| M | ? | related.py | 1616 |
| M | ? | related.py | 1767 |
| M | ? | query.py | 956 |
| M | ? | query.py | 1012 |
| M | ? | where.py | 200 |
| M | ? | compiler.py | 262 |
| M | ? | compiler.py | 1926 |
| M | ? | datetime.py | 80 |
| M | ? | utils.py | 19 |
| M | ? | handler.py | 50 |
| M | ? | handler.py | 67 |
| M | ? | asgi.py | 226 |
| M | ? | regex_helper.py | 351 |
| M | ? | version.py | 63 |
| M | ? | version.py | 64 |
| M | ? | runner.py | 998 |
| M | ? | client.py | 92 |
| M | ? | client.py | 105 |
| M | ? | utils.py | 577 |
| M | ? | utils.py | 580 |
| M | ? | hashers.py | 339 |
| M | ? | hashers.py | 418 |
| M | ? | hashers.py | 439 |
| M | ? | hashers.py | 521 |
| M | ? | hashers.py | 532 |
| M | ? | hashers.py | 610 |
| M | ? | hashers.py | 670 |
| M | ? | base.py | 463 |
| M | ? | multipartparser.py | 461 |
| M | ? | csrf.py | 156 |
| C | ? | operations.py | 145 |
| H | ? | widgets.py | 538 |
| H | ? | widgets.py | 625 |
| H | ? | models.py | 574 |
| H | ? | models.py | 791 |
| H | ? | models.py | 795 |
| H | ? | query.py | 736 |
| H | ? | query.py | 1120 |
| H | ? | query.py | 1122 |
| H | ? | files.py | 101 |
| H | ? | files.py | 107 |
| H | ? | files.py | 127 |
| H | ? | files.py | 341 |
| H | ? | files.py | 356 |
| H | ? | related_descriptors.py | 880 |
| H | ? | related_descriptors.py | 986 |
| H | ? | creation.py | 188 |
| H | ? | edit.py | 133 |
| H | ? | loaddata.py | 210 |
| H | ? | base.py | 328 |
| H | ? | uploadhandler.py | 9 |
| H | ? | client.py | 818 |
| H | ? | client.py | 894 |
| H | ? | layermapping.py | 673 |
| H | ? | base_session.py | 21 |
| H | ? | middleware.py | 60 |
| H | ? | cache.py | 57 |
| H | ? | file.py | 114 |
| H | ? | file.py | 187 |
| H | ? | signed_cookies.py | 49 |
| H | ? | signed_cookies.py | 80 |
| H | ? | cached_db.py | 89 |
| H | ? | db.py | 74 |
| H | ? | db.py | 127 |
| H | ? | db.py | 153 |
| H | ? | management.py | 37 |
| H | ? | collectstatic.py | 402 |
| H | ? | views.py | 242 |
| H | ? | views.py | 322 |
| H | ? | views.py | 369 |
| H | ? | changepassword.py | 80 |
| H | ? | forms.py | 134 |
| H | ? | forms.py | 209 |
| H | ? | forms.py | 247 |
| H | ? | models.py | 24 |
| H | ? | models.py | 168 |
| H | ? | admin.py | 179 |
| H | ? | base_user.py | 62 |
| H | ? | base_user.py | 107 |
| H | ? | models.py | 49 |
| H | ? | options.py | 1449 |
| H | ? | options.py | 1455 |
| H | ? | options.py | 1471 |
| H | ? | fields.py | 756 |
| H | ? | forms.py | 74 |
| H | ? | multipartparser.py | 185 |
| H | ? | multipartparser.py | 195 |
| H | ? | multipartparser.py | 287 |
| H | ? | multipartparser.py | 361 |
| H | ? | multipartparser.py | 536 |
| H | ? | inspectdb.py | 151 |
| M | ? | widgets.py | 340 |
| M | ? | widgets.py | 751 |
| M | ? | boundfield.py | 31 |
| M | ? | boundfield.py | 44 |
| M | ? | loaddata.py | 292 |
| M | ? | loaddata.py | 326 |
| M | ? | filebased.py | 38 |
| M | ? | filebased.py | 71 |
| M | ? | filebased.py | 154 |
| M | ? | redis.py | 29 |
| M | ? | db.py | 102 |
| M | ? | locmem.py | 43 |
| M | ? | locmem.py | 73 |
| M | ? | pyyaml.py | 70 |
| M | ? | runner.py | 208 |
| M | ? | testcases.py | 88 |
| C | ? | operations.py | 113 |
| C | ? | operations.py | 73 |
| C | ? | operations.py | 684 |
| C | ? | operations.py | 155 |
| H | ? | shortcuts.py | 196 |
| H | ? | runserver.py | 131 |
| H | ? | layermapping.py | 697 |
| H | ? | loader_tags.py | 256 |
| H | ? | loader_tags.py | 274 |
| H | ? | request.py | 289 |
| H | ? | manage_translations.py | 76 |
| M | ? | creation.py | 292 |
| M | ? | views.py | 262 |
| M | ? | smartif.py | 172 |
| M | ? | smartif.py | 175 |
| M | ? | global_settings.py | 279 |
| M | ? | csrf.py | 365 |
| M | ? | widgets.py | 659 |
| M | ? | widgets.py | 673 |
| M | ? | widgets.py | 678 |
| M | ? | widgets.py | 683 |
| M | ? | models.py | 739 |
| M | ? | query.py | 1310 |
| M | ? | related_descriptors.py | 1111 |
| M | ? | deletion.py | 382 |
| M | ? | deletion.py | 419 |
| M | ? | creation.py | 292 |
| M | ? | cache.py | 365 |
| M | ? | cache.py | 377 |
| M | ? | signed_cookies.py | 68 |
| M | ? | views.py | 262 |
| M | ? | session.py | 13 |
| M | ? | cookie.py | 16 |
| M | ? | smartif.py | 172 |
| M | ? | smartif.py | 175 |
| M | ? | loader_tags.py | 88 |
| M | ? | loader_tags.py | 164 |
| M | ? | csrf.py | 365 |
| C | GS001 | django.po | 696 |
| C | GS001 | django.po | 699 |
| C | GS001 | django.po | 731 |
| C | GS001 | django.po | 556 |
| C | GS001 | django.po | 559 |
| C | GS001 | django.po | 586 |
| C | GS001 | django.po | 708 |
| C | GS001 | django.po | 711 |
| C | GS001 | django.po | 744 |
| C | GS001 | django.po | 649 |
| C | GS001 | django.po | 652 |
| C | GS001 | django.po | 684 |
| C | GS001 | django.po | 561 |
| C | GS001 | django.po | 564 |
| C | GS001 | django.po | 588 |
| C | GS001 | django.po | 711 |
| C | GS001 | django.po | 714 |
| C | GS001 | django.po | 747 |
| C | GS001 | django.po | 729 |
| C | GS001 | django.po | 732 |
| C | GS001 | django.po | 765 |
| C | GS001 | django.po | 710 |
| C | GS001 | django.po | 713 |
| C | GS001 | django.po | 745 |
| C | GS001 | django.po | 623 |
| C | GS001 | django.po | 626 |
| C | GS001 | django.po | 659 |
| C | GS001 | django.po | 592 |
| C | GS001 | django.po | 595 |
| C | GS001 | django.po | 619 |
| C | GS001 | django.po | 580 |
| C | GS001 | django.po | 583 |
| C | GS001 | django.po | 609 |
| C | GS001 | django.po | 718 |
| C | GS001 | django.po | 721 |
| C | GS001 | django.po | 753 |
| C | GS001 | django.po | 729 |
| C | GS001 | django.po | 732 |
| C | GS001 | django.po | 765 |
| C | GS001 | django.po | 733 |
| C | GS001 | django.po | 736 |
| C | GS001 | django.po | 769 |
| C | GS001 | django.po | 592 |
| C | GS001 | django.po | 595 |
| C | GS001 | django.po | 625 |
| C | GS001 | django.po | 724 |
| C | GS001 | django.po | 727 |
| C | GS001 | django.po | 760 |
| C | GS001 | django.po | 710 |
| C | GS001 | django.po | 713 |
| C | GS001 | django.po | 746 |
| C | GS001 | django.po | 702 |
| C | GS001 | django.po | 705 |
| C | GS001 | django.po | 738 |
| C | GS001 | django.po | 645 |
| C | GS001 | django.po | 648 |
| C | GS001 | django.po | 682 |
| C | GS001 | django.po | 918 |
| C | GS001 | django.po | 922 |
| C | GS001 | django.po | 951 |
| C | GS001 | django.po | 635 |
| C | GS001 | django.po | 636 |
| C | GS001 | django.po | 638 |
| C | GS001 | django.po | 639 |
| C | GS001 | django.po | 670 |
| C | GS001 | django.po | 671 |
| C | GS001 | django.po | 610 |
| C | GS001 | django.po | 611 |
| C | GS001 | django.po | 613 |
| C | GS001 | django.po | 614 |
| C | GS001 | django.po | 639 |
| C | GS001 | django.po | 640 |
| C | GS001 | django.po | 639 |
| C | GS001 | django.po | 642 |
| C | GS001 | django.po | 674 |
| C | GS001 | django.po | 753 |
| C | GS001 | django.po | 756 |
| C | GS001 | django.po | 790 |
| C | GS001 | django.po | 718 |
| C | GS001 | django.po | 721 |
| C | GS001 | django.po | 755 |
| C | GS001 | django.po | 610 |
| C | GS001 | django.po | 613 |
| C | GS001 | django.po | 647 |
| C | GS001 | django.po | 634 |
| C | GS001 | django.po | 637 |
| C | GS001 | django.po | 666 |
| C | GS001 | django.po | 610 |
| C | GS001 | django.po | 613 |
| C | GS001 | django.po | 648 |
| C | GS001 | django.po | 711 |
| C | GS001 | django.po | 714 |
| C | GS001 | django.po | 746 |
| C | GS001 | django.po | 643 |
| C | GS001 | django.po | 646 |
| C | GS001 | django.po | 678 |
| C | GS001 | django.po | 708 |
| C | GS001 | django.po | 711 |
| C | GS001 | django.po | 743 |
| C | GS001 | django.po | 696 |
| C | GS001 | django.po | 699 |
| C | GS001 | django.po | 731 |
| C | GS001 | django.po | 743 |
| C | GS001 | django.po | 746 |
| C | GS001 | django.po | 781 |
| C | GS001 | django.po | 531 |
| C | GS001 | django.po | 534 |
| C | GS001 | django.po | 558 |
| C | GS001 | django.po | 715 |
| C | GS001 | django.po | 718 |
| C | GS001 | django.po | 751 |
| C | GS001 | django.po | 660 |
| C | GS001 | django.po | 663 |
| C | GS001 | django.po | 698 |
| C | GS001 | django.po | 714 |
| C | GS001 | django.po | 717 |
| C | GS001 | django.po | 749 |
| C | GS001 | django.po | 708 |
| C | GS001 | django.po | 711 |
| C | GS001 | django.po | 743 |
| C | GS001 | django.po | 623 |
| C | GS001 | django.po | 626 |
| C | GS001 | django.po | 654 |
| C | GS001 | django.po | 717 |
| C | GS001 | django.po | 720 |
| C | GS001 | django.po | 752 |
| C | GS001 | django.po | 703 |
| C | GS001 | django.po | 706 |
| C | GS001 | django.po | 738 |
| C | GS001 | django.po | 706 |
| C | GS001 | django.po | 709 |
| C | GS001 | django.po | 742 |
| C | GS001 | django.po | 679 |
| C | GS001 | django.po | 682 |
| C | GS001 | django.po | 710 |
| C | GS001 | django.po | 586 |
| C | GS001 | django.po | 589 |
| C | GS001 | django.po | 616 |
| C | GS001 | django.po | 706 |
| C | GS001 | django.po | 709 |
| C | GS001 | django.po | 743 |
| C | GS001 | django.po | 585 |
| C | GS001 | django.po | 588 |
| C | GS001 | django.po | 618 |
| C | GS001 | django.po | 629 |
| C | GS001 | django.po | 632 |
| C | GS001 | django.po | 666 |
| C | GS001 | django.po | 705 |
| C | GS001 | django.po | 706 |
| C | GS001 | django.po | 708 |
| C | GS001 | django.po | 709 |
| C | GS001 | django.po | 740 |
| C | GS001 | django.po | 741 |
| C | GS001 | django.po | 719 |
| C | GS001 | django.po | 722 |
| C | GS001 | django.po | 754 |
| C | GS001 | django.po | 678 |
| C | GS001 | django.po | 681 |
| C | GS001 | django.po | 709 |
| C | GS001 | django.po | 556 |
| C | GS001 | django.po | 559 |
| C | GS001 | django.po | 583 |
| C | GS001 | django.po | 614 |
| C | GS001 | django.po | 617 |
| C | GS001 | django.po | 643 |
| C | GS001 | django.po | 561 |
| C | GS001 | django.po | 564 |
| C | GS001 | django.po | 588 |
| C | GS001 | django.po | 564 |
| C | GS001 | django.po | 567 |
| C | GS001 | django.po | 591 |
| C | GS001 | django.po | 748 |
| C | GS001 | django.po | 751 |
| C | GS001 | django.po | 783 |
| C | GS001 | django.po | 626 |
| C | GS001 | django.po | 629 |
| C | GS001 | django.po | 659 |
| C | GS001 | django.po | 557 |
| C | GS001 | django.po | 560 |
| C | GS001 | django.po | 584 |
| C | GS001 | django.po | 736 |
| C | GS001 | django.po | 739 |
| C | GS001 | django.po | 772 |
| C | GS001 | django.po | 712 |
| C | GS001 | django.po | 715 |
| C | GS001 | django.po | 747 |
| C | GS001 | django.po | 641 |
| C | GS001 | django.po | 644 |
| C | GS001 | django.po | 672 |
| C | GS001 | django.po | 617 |
| C | GS001 | django.po | 620 |
| C | GS001 | django.po | 648 |
| C | GS001 | django.po | 695 |
| C | GS001 | django.po | 698 |
| C | GS001 | django.po | 730 |
| C | GS001 | django.po | 676 |
| C | GS001 | django.po | 679 |
| C | GS001 | django.po | 711 |
| C | GS001 | django.po | 631 |
| C | GS001 | django.po | 634 |
| C | GS001 | django.po | 667 |
| C | GS001 | django.po | 554 |
| C | GS001 | django.po | 557 |
| C | GS001 | django.po | 581 |
| C | GS001 | django.po | 630 |
| C | GS001 | django.po | 633 |
| C | GS001 | django.po | 666 |
| C | GS001 | django.po | 606 |
| C | GS001 | django.po | 609 |
| C | GS001 | django.po | 634 |
| C | GS001 | django.po | 727 |
| C | GS001 | django.po | 730 |
| C | GS001 | django.po | 763 |
| C | GS001 | django.po | 646 |
| C | GS001 | django.po | 649 |
| C | GS001 | django.po | 682 |
| C | GS001 | django.po | 582 |
| C | GS001 | django.po | 585 |
| C | GS001 | django.po | 615 |
| C | GS001 | django.po | 625 |
| C | GS001 | django.po | 628 |
| C | GS001 | django.po | 654 |
| C | GS001 | django.po | 732 |
| C | GS001 | django.po | 735 |
| C | GS001 | django.po | 768 |
| C | GS001 | django.po | 723 |
| C | GS001 | django.po | 726 |
| C | GS001 | django.po | 759 |
| C | GS001 | django.po | 741 |
| C | GS001 | django.po | 744 |
| C | GS001 | django.po | 776 |
| C | GS001 | django.po | 669 |
| C | GS001 | django.po | 672 |
| C | GS001 | django.po | 704 |
| C | GS001 | django.po | 727 |
| C | GS001 | django.po | 730 |
| C | GS001 | django.po | 764 |
| C | GS001 | django.po | 714 |
| C | GS001 | django.po | 717 |
| C | GS001 | django.po | 749 |
| C | GS001 | django.po | 682 |
| C | GS001 | django.po | 685 |
| C | GS001 | django.po | 717 |
| C | GS001 | django.po | 710 |
| C | GS001 | django.po | 713 |
| C | GS001 | django.po | 746 |
| C | GS001 | django.po | 729 |
| C | GS001 | django.po | 732 |
| C | GS001 | django.po | 764 |
| C | GS001 | django.po | 729 |
| C | GS001 | django.po | 732 |
| C | GS001 | django.po | 764 |
| C | GS001 | django.po | 723 |
| C | GS001 | django.po | 726 |
| C | GS001 | django.po | 759 |
| C | GS001 | django.po | 687 |
| C | GS001 | django.po | 690 |
| C | GS001 | django.po | 722 |
| C | GS001 | django.po | 568 |
| C | GS001 | django.po | 571 |
| C | GS001 | django.po | 595 |
| C | GS001 | django.po | 565 |
| C | GS001 | django.po | 568 |
| C | GS001 | django.po | 592 |
| C | GS001 | django.po | 615 |
| C | GS001 | django.po | 618 |
| C | GS001 | django.po | 647 |
| C | GS001 | django.po | 590 |
| C | GS001 | django.po | 593 |
| C | GS001 | django.po | 619 |
| C | GS001 | django.po | 656 |
| C | GS001 | django.po | 659 |
| C | GS001 | django.po | 683 |
| C | GS001 | django.po | 731 |
| C | GS001 | django.po | 734 |
| C | GS001 | django.po | 766 |
| C | GS001 | django.po | 578 |
| C | GS001 | django.po | 581 |
| C | GS001 | django.po | 607 |
| C | GS001 | django.po | 528 |
| C | GS001 | django.po | 531 |
| C | GS001 | django.po | 555 |
| C | GS001 | django.po | 708 |
| C | GS001 | django.po | 711 |
| C | GS001 | django.po | 746 |
| C | GS001 | django.po | 718 |
| C | GS001 | django.po | 721 |
| C | GS001 | django.po | 753 |
| C | GS001 | django.po | 702 |
| C | GS001 | django.po | 705 |
| C | GS001 | django.po | 737 |
| C | GS001 | django.po | 642 |
| C | GS001 | django.po | 645 |
| C | GS001 | django.po | 669 |
| C | GS001 | django.po | 637 |
| C | GS001 | django.po | 640 |
| C | GS001 | django.po | 672 |
| C | GS001 | django.po | 706 |
| C | GS001 | django.po | 709 |
| C | GS001 | django.po | 737 |
| C | GS001 | django.po | 685 |
| C | GS001 | django.po | 688 |
| C | GS001 | django.po | 716 |
| C | GS001 | password_reset_confirm.html | 28 |
| C | GS001 | password_reset_confirm.html | 35 |
| C | GS001 | password_reset_email.html | 4 |
| C | GS001 | changepassword.py | 17 |
| C | GS001 | views.py | 246 |
| C | GS001 | creation.py | 292 |
| C | GS001 | text.py | 25 |
| C | GS001 | pyproject.toml | 57 |
| L | GS003 | ogrinfo.py | 28 |
| L | GS003 | ogrinfo.py | 29 |
| L | GS003 | ogrinfo.py | 30 |
| L | GS003 | ogrinfo.py | 31 |
| L | GS003 | ogrinfo.py | 32 |
| L | GS003 | ogrinfo.py | 34 |
| L | GS003 | ogrinfo.py | 35 |
| L | GS003 | ogrinfo.py | 40 |
| L | GS003 | ogrinfo.py | 53 |
| L | GS003 | management.py | 34 |
| L | GS003 | management.py | 44 |
| L | GS003 | runserver.py | 184 |
| L | GS003 | shell.py | 109 |
| L | GS003 | creation.py | 334 |
| L | GS003 | archive.py | 191 |
| L | GS003 | archive_eol_stable_branches.py | 14 |
| L | GS003 | archive_eol_stable_branches.py | 16 |
| L | GS003 | archive_eol_stable_branches.py | 23 |
| L | GS003 | archive_eol_stable_branches.py | 26 |
| L | GS003 | archive_eol_stable_branches.py | 83 |
| L | GS003 | archive_eol_stable_branches.py | 120 |
| L | GS003 | archive_eol_stable_branches.py | 122 |
| L | GS003 | archive_eol_stable_branches.py | 124 |
| L | GS003 | archive_eol_stable_branches.py | 125 |
| L | GS003 | archive_eol_stable_branches.py | 128 |
| L | GS003 | archive_eol_stable_branches.py | 130 |
| L | GS003 | archive_eol_stable_branches.py | 137 |
| L | GS003 | archive_eol_stable_branches.py | 139 |
| L | GS003 | archive_eol_stable_branches.py | 146 |
| L | GS003 | manage_translations.py | 48 |
| L | GS003 | manage_translations.py | 75 |
| L | GS003 | manage_translations.py | 78 |
| L | GS003 | manage_translations.py | 90 |
| L | GS003 | manage_translations.py | 100 |
| L | GS003 | manage_translations.py | 115 |
| L | GS003 | manage_translations.py | 120 |
| L | GS003 | manage_translations.py | 139 |
| L | GS003 | manage_translations.py | 141 |
| L | GS003 | manage_translations.py | 171 |
| L | GS003 | manage_translations.py | 205 |
| L | GS003 | manage_translations.py | 216 |
| L | GS003 | manage_translations.py | 220 |
| L | GS003 | manage_translations.py | 222 |
| L | GS003 | manage_translations.py | 241 |
| L | GS003 | manage_translations.py | 259 |
| L | GS003 | manage_translations.py | 261 |
| L | GS003 | manage_translations.py | 316 |
| L | GS003 | manage_translations.py | 331 |
| L | GS003 | manage_translations.py | 333 |
| L | GS003 | manage_translations.py | 337 |
| L | GS008 | global_settings.py | 22 |
| L | GS008 | global_settings.py | 31 |
| L | GS008 | global_settings.py | 35 |
| L | GS008 | global_settings.py | 41 |
| L | GS008 | global_settings.py | 157 |
| L | GS008 | global_settings.py | 161 |
| L | GS008 | global_settings.py | 165 |
| L | GS008 | global_settings.py | 166 |
| L | GS008 | global_settings.py | 167 |
| L | GS008 | global_settings.py | 169 |
| L | GS008 | global_settings.py | 170 |
| L | GS008 | global_settings.py | 171 |
| L | GS008 | global_settings.py | 175 |
| L | GS008 | global_settings.py | 179 |
| L | GS008 | global_settings.py | 182 |
| L | GS008 | global_settings.py | 185 |
| L | GS008 | global_settings.py | 188 |
| L | GS008 | global_settings.py | 199 |
| L | GS008 | global_settings.py | 207 |
| L | GS008 | global_settings.py | 210 |
| L | GS008 | global_settings.py | 214 |
| L | GS008 | global_settings.py | 216 |
| L | GS008 | global_settings.py | 217 |
| L | GS008 | global_settings.py | 220 |
| L | GS008 | global_settings.py | 223 |
| L | GS008 | global_settings.py | 225 |
| L | GS008 | global_settings.py | 228 |
| L | GS008 | global_settings.py | 231 |
| L | GS008 | global_settings.py | 235 |
| L | GS008 | global_settings.py | 239 |
| L | GS008 | global_settings.py | 242 |
| L | GS008 | global_settings.py | 245 |
| L | GS008 | global_settings.py | 248 |
| L | GS008 | global_settings.py | 285 |
| L | GS008 | global_settings.py | 322 |
| L | GS008 | global_settings.py | 326 |
| L | GS008 | global_settings.py | 355 |
| L | GS008 | global_settings.py | 359 |
| L | GS008 | global_settings.py | 363 |
| L | GS008 | global_settings.py | 368 |
| L | GS008 | global_settings.py | 373 |
| L | GS008 | global_settings.py | 377 |
| L | GS008 | global_settings.py | 382 |
| L | GS008 | global_settings.py | 388 |
| L | GS008 | global_settings.py | 406 |
| L | GS008 | global_settings.py | 417 |
| L | GS008 | global_settings.py | 431 |
| L | GS008 | global_settings.py | 434 |
| L | GS008 | global_settings.py | 437 |
| L | GS008 | global_settings.py | 441 |
| L | GS008 | global_settings.py | 447 |
| L | GS008 | global_settings.py | 448 |
| L | GS008 | global_settings.py | 451 |
| L | GS008 | global_settings.py | 454 |
| L | GS008 | global_settings.py | 456 |
| L | GS008 | global_settings.py | 457 |
| L | GS008 | global_settings.py | 464 |
| L | GS008 | global_settings.py | 473 |
| L | GS008 | global_settings.py | 489 |
| L | GS008 | global_settings.py | 491 |
| L | GS008 | global_settings.py | 493 |
| L | GS008 | global_settings.py | 495 |
| L | GS008 | global_settings.py | 497 |
| L | GS008 | global_settings.py | 501 |
| L | GS008 | global_settings.py | 504 |
| L | GS008 | global_settings.py | 506 |
| L | GS008 | global_settings.py | 508 |
| L | GS008 | global_settings.py | 510 |
| L | GS008 | global_settings.py | 515 |
| L | GS008 | global_settings.py | 522 |
| L | GS008 | global_settings.py | 528 |
| L | GS008 | global_settings.py | 529 |
| L | GS008 | global_settings.py | 535 |
| L | GS008 | global_settings.py | 537 |
| L | GS008 | global_settings.py | 546 |
| L | GS008 | global_settings.py | 550 |
| L | GS008 | global_settings.py | 564 |
| L | GS008 | global_settings.py | 565 |
| L | GS008 | global_settings.py | 573 |
| L | GS008 | global_settings.py | 576 |
| L | GS008 | global_settings.py | 577 |
| L | GS008 | global_settings.py | 578 |
| L | GS008 | global_settings.py | 580 |
| L | GS008 | global_settings.py | 581 |
| L | GS008 | global_settings.py | 582 |
| L | GS008 | global_settings.py | 583 |
| L | GS008 | global_settings.py | 584 |
| L | GS008 | global_settings.py | 585 |
| L | GS008 | global_settings.py | 592 |
| L | GS008 | global_settings.py | 602 |
| L | GS008 | global_settings.py | 609 |
| L | GS008 | global_settings.py | 613 |
| L | GS008 | global_settings.py | 620 |
| L | GS008 | global_settings.py | 624 |
| L | GS008 | global_settings.py | 653 |
| L | GS008 | global_settings.py | 663 |
| L | GS008 | global_settings.py | 668 |
| L | GS008 | global_settings.py | 669 |
| L | GS008 | global_settings.py | 670 |
| L | GS008 | global_settings.py | 671 |
| L | GS008 | global_settings.py | 672 |
| L | GS008 | global_settings.py | 674 |
| L | GS008 | global_settings.py | 675 |
| L | GS008 | global_settings.py | 681 |
| L | GS008 | global_settings.py | 682 |
| L | GS008 | global_settings.py | 687 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 23 |
| L | GS008 | formats.py | 27 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 27 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 21 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 34 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 13 |
| L | GS008 | formats.py | 15 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 53 |
| L | GS008 | formats.py | 60 |
| L | GS008 | formats.py | 65 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 39 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 13 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 21 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 39 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 35 |
| L | GS008 | formats.py | 36 |
| L | GS008 | formats.py | 37 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 44 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 3 |
| L | GS008 | formats.py | 4 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 3 |
| L | GS008 | formats.py | 4 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 3 |
| L | GS008 | formats.py | 4 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 3 |
| L | GS008 | formats.py | 4 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 27 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 21 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 34 |
| L | GS008 | formats.py | 35 |
| L | GS008 | formats.py | 36 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 27 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 34 |
| L | GS008 | formats.py | 35 |
| L | GS008 | formats.py | 36 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 44 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 46 |
| L | GS008 | formats.py | 47 |
| L | GS008 | formats.py | 48 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 23 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 27 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 47 |
| L | GS008 | formats.py | 48 |
| L | GS008 | formats.py | 49 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 21 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 21 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 46 |
| L | GS008 | formats.py | 47 |
| L | GS008 | formats.py | 48 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 38 |
| L | GS008 | formats.py | 52 |
| L | GS008 | formats.py | 53 |
| L | GS008 | formats.py | 54 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 21 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 44 |
| L | GS008 | formats.py | 45 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 44 |
| L | GS008 | formats.py | 45 |
| L | GS008 | formats.py | 46 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 23 |
| L | GS008 | formats.py | 38 |
| L | GS008 | formats.py | 39 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 36 |
| L | GS008 | formats.py | 37 |
| L | GS008 | formats.py | 38 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 39 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 36 |
| L | GS008 | formats.py | 90 |
| L | GS008 | formats.py | 91 |
| L | GS008 | formats.py | 92 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 39 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 23 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 37 |
| L | GS008 | formats.py | 38 |
| L | GS008 | formats.py | 39 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 34 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 27 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 34 |
| L | GS008 | formats.py | 35 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 23 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 24 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 44 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 44 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 43 |
| L | GS008 | formats.py | 44 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 17 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 34 |
| L | GS008 | formats.py | 35 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 21 |
| L | GS008 | formats.py | 26 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 31 |
| L | GS008 | formats.py | 32 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 23 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 13 |
| L | GS008 | formats.py | 14 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 25 |
| L | GS008 | formats.py | 33 |
| L | GS008 | formats.py | 34 |
| L | GS008 | formats.py | 35 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 29 |
| L | GS008 | formats.py | 30 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 19 |
| L | GS008 | formats.py | 20 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 42 |
| L | GS008 | formats.py | 5 |
| L | GS008 | formats.py | 6 |
| L | GS008 | formats.py | 7 |
| L | GS008 | formats.py | 8 |
| L | GS008 | formats.py | 9 |
| L | GS008 | formats.py | 10 |
| L | GS008 | formats.py | 11 |
| L | GS008 | formats.py | 12 |
| L | GS008 | formats.py | 16 |
| L | GS008 | formats.py | 22 |
| L | GS008 | formats.py | 28 |
| L | GS008 | formats.py | 40 |
| L | GS008 | formats.py | 41 |
| L | GS008 | formats.py | 42 |
| L | GS008 | helpers.py | 27 |
| L | GS008 | options.py | 87 |
| L | GS008 | const.py | 6 |
| L | GS008 | const.py | 9 |
| L | GS008 | const.py | 19 |
| L | GS008 | const.py | 23 |
| L | GS008 | const.py | 42 |
| L | GS008 | const.py | 62 |
| L | GS008 | const.py | 63 |
| L | GS008 | libgdal.py | 123 |
| L | GS008 | ds.py | 26 |
| L | GS008 | ds.py | 27 |
| L | GS008 | ds.py | 29 |
| L | GS008 | ds.py | 30 |
| L | GS008 | ds.py | 31 |
| L | GS008 | const.py | 19 |
| L | GS008 | const.py | 38 |
| L | GS008 | const.py | 44 |
| L | GS008 | const.py | 63 |
| L | GS008 | const.py | 74 |
| L | GS008 | const.py | 102 |
| L | GS008 | const.py | 105 |
| L | GS008 | libgeos.py | 130 |
| L | GS008 | constants.py | 7 |
| L | GS008 | constants.py | 15 |
| L | GS008 | deprecation.py | 10 |
| L | GS008 | deprecation.py | 14 |
| L | GS008 | deprecation.py | 18 |
| L | GS008 | utils.py | 22 |
| L | GS008 | validators.py | 16 |
| L | GS008 | constants.py | 8 |
| L | GS008 | query_utils.py | 24 |
| L | GS008 | constants.py | 7 |
| L | GS008 | constants.py | 12 |
| L | GS008 | constants.py | 13 |
| L | GS008 | constants.py | 14 |
| L | GS008 | constants.py | 16 |
| L | GS008 | constants.py | 17 |
| L | GS008 | constants.py | 26 |
| L | GS008 | base.py | 19 |
| L | GS008 | base.py | 20 |
| L | GS008 | base.py | 78 |
| L | GS008 | base.py | 80 |
| L | GS008 | base.py | 82 |
| L | GS008 | base.py | 83 |
| L | GS008 | base.py | 84 |
| L | GS008 | dates.py | 6 |
| L | GS008 | dates.py | 15 |
| L | GS008 | dates.py | 24 |
| L | GS008 | dates.py | 38 |
| L | GS008 | dates.py | 52 |
| L | GS008 | dates.py | 66 |
| L | GS008 | encoding.py | 262 |
| L | GS008 | html.py | 24 |
| L | GS008 | version.py | 10 |
| L | GS008 | version.py | 16 |
| L | GS008 | version.py | 17 |
| L | GS008 | version.py | 18 |
| L | GS008 | version.py | 19 |
| L | GS008 | version.py | 20 |
| L | GS008 | version.py | 21 |
| L | GS008 | errors.py | 9 |
| L | GS008 | errors.py | 36 |
| L | GS008 | errors.py | 41 |
| L | GS008 | errors.py | 47 |
| L | GS008 | errors.py | 56 |
| L | GS008 | errors.py | 73 |
| L | GS008 | errors.py | 96 |
| L | GS008 | errors.py | 113 |
| L | GS008 | errors.py | 125 |
| L | GS008 | errors.py | 137 |
| L | GS008 | errors.py | 146 |
| I | GS015 | main.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | asgi.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | asgi.py | 1 |
| I | GS015 | wsgi.py | 1 |
| I | GS015 | wsgi.py | 1 |
| I | GS015 | cache.py | 1 |
| I | GS015 | clickjacking.py | 1 |
| I | GS015 | common.py | 1 |
| I | GS015 | csp.py | 1 |
| I | GS015 | csrf.py | 1 |
| I | GS015 | debug.py | 1 |
| I | GS015 | gzip.py | 1 |
| I | GS015 | http.py | 1 |
| I | GS015 | vary.py | 1 |
| I | GS015 | base.py | 1 |
| I | GS015 | dates.py | 1 |
| I | GS015 | detail.py | 1 |
| I | GS015 | edit.py | 1 |
| I | GS015 | list.py | 1 |
| i | GS020 |  | 13 |
| i | GS020 |  | 1 |
| i | GS020 |  | 9 |
| i | GS020 |  | 14 |
| i | GS020 |  | 9 |
| i | GS020 |  | 10 |
| i | GS020 |  | 11 |
| i | GS020 |  | 17 |
| i | GS020 |  | 23 |
| i | GS020 |  | 29 |
| i | GS020 |  | 36 |
| i | GS020 |  | 42 |
| i | GS020 |  | 48 |
| i | GS020 |  | 54 |
| i | GS020 |  | 1 |
| i | GS020 |  | 8 |
| i | GS020 |  | 109 |
| i | GS020 |  | 115 |
| i | GS020 |  | 302 |
| i | GS020 |  | 309 |
| i | GS020 |  | 341 |
| i | GS020 |  | 5 |
| i | GS020 |  | 35 |
| i | GS020 |  | 39 |
| i | GS020 |  | 5 |
| i | GS020 |  | 19 |
| i | GS020 |  | 22 |
| i | GS020 |  | 28 |
| i | GS020 |  | 122 |
| i | GS020 |  | 38 |
| H | ? | runserver.py | 33 |
| H | ? | runserver.py | 178 |
| H | ? | client.py | 420 |
| H | ? | client.py | 701 |
| H | ? | client.py | 754 |
| H | ? | selenium.py | 46 |
| H | ? | request.py | 197 |
| H | ? | formats.py | 34 |
| H | ? | formats.py | 37 |
| H | ? | formats.py | 40 |
| H | ? | formats.py | 43 |
| H | ? | formats.py | 26 |
| H | ? | formats.py | 40 |
| H | ? | formats.py | 27 |
| H | ? | formats.py | 41 |
| H | ? | formats.py | 22 |
| H | ? | formats.py | 25 |
| H | ? | formats.py | 30 |
| C | ? | widgets.py | 673 |
| C | ? | widgets.py | 678 |
| C | ? | widgets.py | 683 |
| C | ? | creation.py | 292 |
| C | ? | views.py | 262 |
| C | ? | session.py | 13 |
| C | ? | cookie.py | 16 |
| C | ? | loader_tags.py | 88 |
| C | ? | loader_tags.py | 164 |
| H | ? | csrf.py | 67 |
| H | ? | manage_translations.py | 404 |
| H | ? | shell.py | 89 |
| H | ? | shell.py | 262 |
| H | ? | shell.py | 272 |
| H | ? | defaulttags.py | 326 |
| H | ? | defaulttags.py | 917 |
| H | ? | smartif.py | 59 |
| H | ? | smartif.py | 86 |
| H | ? | smartif.py | 99 |
| H | ? | smartif.py | 100 |
| H | ? | smartif.py | 101 |
| H | ? | smartif.py | 102 |
| H | ? | smartif.py | 103 |
| H | ? | smartif.py | 104 |
| H | ? | smartif.py | 105 |
| H | ? | smartif.py | 106 |
| H | ? | smartif.py | 107 |
| H | ? | smartif.py | 108 |
| H | ? | smartif.py | 109 |
| H | ? | smartif.py | 110 |
| H | ? | smartif.py | 111 |
| H | ? | smartif.py | 144 |
| C | ? | filebased.py | 38 |
| C | ? | filebased.py | 71 |
| C | ? | filebased.py | 154 |
| C | ? | redis.py | 29 |
| C | ? | db.py | 102 |
| C | ? | locmem.py | 43 |
| C | ? | locmem.py | 73 |
| C | ? | runner.py | 208 |
| C | ? | testcases.py | 88 |
| H | ? | package.json | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | ? | biome.json | 0 |
| H | ? | zizmor.yml | 0 |
| H | GS004 | shell.py | 89 |
| H | GS004 | shell.py | 262 |
| H | GS004 | shell.py | 272 |
| H | GS004 | version.py | 90 |
| C | GS005 | introspection.py | 17 |
| C | GS005 | operations.py | 341 |
| C | GS005 | operations.py | 161 |
| C | GS005 | db.py | 136 |
| C | GS005 | db.py | 302 |
| C | GS005 | operations.py | 354 |
| C | GS005 | base.py | 331 |
| C | GS005 | compiler.py | 445 |
| C | GS005 | compiler.py | 2028 |
| H | GS007 | models.py | 54 |
| I | GS007 | layer.py | 54 |
| H | GS007 | migrate.py | 370 |
| I | GS007 | base.py | 112 |
| I | GS007 | base.py | 113 |
| I | GS007 | base.py | 133 |
| I | GS007 | features.py | 132 |
| I | GS007 | features.py | 133 |
| I | GS007 | introspection.py | 58 |
| I | GS007 | operations.py | 215 |
| I | GS007 | base.py | 101 |
| I | GS007 | base.py | 102 |
| I | GS007 | base.py | 103 |
| H | GS007 | base.py | 2544 |
| H | GS007 | related_descriptors.py | 1603 |
| H | GS007 | related_descriptors.py | 1633 |
| I | GS007 | query.py | 1317 |
| H | GS007 | query.py | 800 |
| H | GS007 | query.py | 805 |
| H | GS007 | query.py | 811 |
| H | GS007 | query.py | 817 |
| H | GS007 | query.py | 975 |
| H | GS007 | query.py | 982 |
| H | GS007 | query.py | 985 |
| H | GS007 | query.py | 989 |
| H | GS007 | query.py | 994 |
| I | GS007 | widgets.py | 1018 |
| s | GS009 |  | 0 |
| L | GS012 | models.py | 49 |
| L | GS012 | options.py | 1455 |
| L | GS012 | options.py | 1471 |
| L | GS012 | admin.py | 179 |
| L | GS012 | forms.py | 134 |
| L | GS012 | forms.py | 209 |
| L | GS012 | changepassword.py | 80 |
| L | GS012 | views.py | 322 |
| L | GS012 | views.py | 369 |
| L | GS012 | fields.py | 756 |
| L | GS012 | base.py | 21 |
| L | GS012 | signed_cookies.py | 80 |
| L | GS012 | base_session.py | 21 |
| L | GS012 | middleware.py | 60 |
| H | GS012 | inspectdb.py | 151 |
| L | GS012 | base.py | 328 |
| L | GS012 | creation.py | 188 |
| L | GS012 | compiler.py | 67 |
| L | GS012 | files.py | 107 |
| L | GS012 | files.py | 127 |
| L | GS012 | files.py | 409 |
| L | GS012 | related.py | 1383 |
| L | GS012 | related_descriptors.py | 880 |
| L | GS012 | related_descriptors.py | 980 |
| L | GS012 | query.py | 2129 |
| L | GS012 | transaction.py | 118 |
| L | GS012 | models.py | 574 |
| L | GS012 | edit.py | 133 |
| C | GS017 | registry.py | 11 |
| H | GS018 | base.py | 333 |
| H | GS018 | query.py | 1948 |
| H | GS018 | transaction.py | 47 |
| H | GS019 | sites.py | 412 |
| H | GS019 | backends.py | 16 |
| H | GS019 | backends.py | 65 |
| H | GS019 | backends.py | 270 |
| H | GS019 | context_processors.py | 49 |
| s | GS021 |  | 66 |
| s | GS021 |  | 55 |
| s | GS021 |  | 1804 |
| s | GS021 |  | 1804 |
| s | GS021 |  | 1805 |
| s | GS021 |  | 1805 |
| s | GS021 |  | 1808 |
| s | GS021 |  | 1808 |
| s | GS021 |  | 1809 |
| s | GS021 |  | 1809 |
| s | GS021 |  | 2938 |
| c | GS021 |  | 54 |
| c | GS021 |  | 315 |
| c | GS021 |  | 42 |
| s | GS021 |  | 1639 |
| s | GS021 |  | 1645 |
| s | GS021 |  | 1653 |
| s | GS021 |  | 1668 |
| s | GS021 |  | 1672 |
| s | GS021 |  | 1691 |
| s | GS021 |  | 1718 |
| s | GS021 |  | 1719 |
| s | GS021 |  | 1730 |
| s | GS021 |  | 1733 |
| s | GS021 |  | 51 |
| s | GS021 |  | 142 |
| s | GS021 |  | 186 |
| s | GS021 |  | 285 |
| s | GS021 |  | 288 |
| s | GS021 |  | 292 |
| s | GS021 |  | 309 |
| s | GS021 |  | 316 |
| s | GS021 |  | 348 |
| s | GS021 |  | 381 |
| s | GS021 |  | 411 |
| s | GS021 |  | 518 |
| s | GS021 |  | 828 |
| s | GS021 |  | 828 |
| s | GS021 |  | 829 |
| s | GS021 |  | 829 |
| s | GS021 |  | 131 |
| s | GS021 |  | 1440 |
| c | GS021 |  | 50 |
| s | GS021 |  | 39 |
| s | GS021 |  | 44 |
| s | GS021 |  | 46 |
| c | GS021 |  | 1083 |
| c | GS021 |  | 1083 |
| s | GS021 |  | 356 |
| s | GS021 |  | 941 |
| s | GS021 |  | 942 |
| s | GS021 |  | 261 |
| s | GS021 |  | 261 |
| s | GS021 |  | 261 |
| s | GS021 |  | 267 |
| s | GS021 |  | 267 |
| s | GS021 |  | 274 |
| c | GS021 |  | 95 |
| s | GS021 |  | 1497 |
| s | GS021 |  | 1500 |
| s | GS021 |  | 1500 |
| s | GS021 |  | 1500 |
| s | GS021 |  | 1572 |
| s | GS021 |  | 1572 |
| s | GS021 |  | 1573 |
| s | GS021 |  | 1573 |
| s | GS021 |  | 1582 |
| s | GS021 |  | 1582 |
| s | GS021 |  | 1583 |
| s | GS021 |  | 1583 |
| s | GS021 |  | 1326 |
| s | GS021 |  | 1379 |
| s | GS021 |  | 1872 |
| s | GS021 |  | 142 |
| s | GS021 |  | 234 |
| s | GS021 |  | 420 |
| s | GS021 |  | 701 |
| s | GS021 |  | 754 |
| s | GS021 |  | 1806 |
| s | GS021 |  | 46 |
| c | GS021 |  | 232 |
| s | GS021 |  | 197 |
| s | GS021 |  | 197 |
| c | GS021 |  | 170 |
| c | GS021 |  | 581 |
| s | GS021 |  | 182 |
| s | GS021 |  | 203 |
| s | GS021 |  | 235 |
| s | GS021 |  | 97 |
| s | GS021 |  | 33 |
| s | GS021 |  | 178 |
| r | GS022 |  | 1 |
| r | GS022 |  | 38 |
| r | GS022 |  | 60 |
| r | GS022 |  | 173 |
| r | GS022 |  | 188 |
| r | GS022 |  | 168 |
| r | GS022 |  | 175 |
| r | GS022 |  | 179 |
| r | GS022 |  | 285 |
| r | GS022 |  | 400 |
| r | GS022 |  | 404 |
| r | GS022 |  | 170 |
| r | GS022 |  | 2376 |
| r | GS022 |  | 828 |
| r | GS022 |  | 849 |
| r | GS022 |  | 11 |
| r | GS022 |  | 12 |
| r | GS022 |  | 17 |
| r | GS022 |  | 19 |
| r | GS022 |  | 23 |
| r | GS022 |  | 25 |
| r | GS022 |  | 26 |
| r | GS022 |  | 27 |
| r | GS022 |  | 28 |
| r | GS022 |  | 30 |
| r | GS022 |  | 32 |
| r | GS022 |  | 35 |
| r | GS022 |  | 39 |
| r | GS022 |  | 39 |
| r | GS022 |  | 43 |
| r | GS022 |  | 43 |
| r | GS022 |  | 47 |
| r | GS022 |  | 50 |
| r | GS022 |  | 54 |
| r | GS022 |  | 57 |
| r | GS022 |  | 60 |
| r | GS022 |  | 63 |
| r | GS022 |  | 66 |
| r | GS022 |  | 70 |
| r | GS022 |  | 73 |
| r | GS022 |  | 80 |
| r | GS022 |  | 86 |
| r | GS022 |  | 89 |
| r | GS022 |  | 94 |
| r | GS022 |  | 96 |
| r | GS022 |  | 100 |
| r | GS022 |  | 104 |
| r | GS022 |  | 10 |
| r | GS022 |  | 29 |
| r | GS022 |  | 30 |
| r | GS022 |  | 40 |
| r | GS022 |  | 44 |
| r | GS022 |  | 77 |
| r | GS022 |  | 93 |
| r | GS022 |  | 9 |
| r | GS022 |  | 16 |
| r | GS022 |  | 2790 |
| r | GS022 |  | 2849 |
| r | GS022 |  | 26 |
| r | GS022 |  | 50 |
| r | GS022 |  | 474 |
| r | GS022 |  | 604 |
| r | GS022 |  | 613 |
| r | GS022 |  | 634 |
| r | GS022 |  | 649 |
| r | GS022 |  | 654 |
| r | GS022 |  | 679 |
| r | GS022 |  | 66 |
| r | GS022 |  | 342 |
| r | GS022 |  | 347 |
| r | GS022 |  | 353 |
| r | GS022 |  | 356 |
| r | GS022 |  | 360 |
| r | GS022 |  | 365 |
| r | GS022 |  | 366 |
| r | GS022 |  | 367 |
| r | GS022 |  | 368 |
| r | GS022 |  | 370 |
| r | GS022 |  | 372 |
| r | GS022 |  | 378 |
| r | GS022 |  | 385 |
| r | GS022 |  | 591 |
| r | GS022 |  | 138 |
| r | GS022 |  | 181 |
| r | GS022 |  | 198 |
| r | GS022 |  | 18 |
| r | GS022 |  | 243 |
| r | GS022 |  | 18 |
| r | GS022 |  | 29 |
| r | GS022 |  | 32 |
| r | GS022 |  | 45 |
| r | GS022 |  | 48 |
| r | GS022 |  | 54 |
| r | GS022 |  | 60 |
| r | GS022 |  | 64 |
| r | GS022 |  | 69 |
| r | GS022 |  | 106 |
| r | GS022 |  | 114 |
| r | GS022 |  | 121 |
| r | GS022 |  | 1195 |
| r | GS022 |  | 70 |
| r | GS022 |  | 82 |
| r | GS022 |  | 82 |
| r | GS022 |  | 91 |
| r | GS022 |  | 10 |
| r | GS022 |  | 29 |
| r | GS022 |  | 30 |
| r | GS022 |  | 37 |
| r | GS022 |  | 407 |
| r | GS022 |  | 87 |
| r | GS022 |  | 147 |
| r | GS022 |  | 997 |
| r | GS022 |  | 1011 |
| r | GS022 |  | 1517 |
| r | GS022 |  | 1532 |
| r | GS022 |  | 1555 |
| r | GS022 |  | 2643 |
| r | GS022 |  | 3422 |
| r | GS022 |  | 9087 |
| r | GS022 |  | 9093 |
| r | GS022 |  | 9099 |
| r | GS022 |  | 9109 |
| r | GS022 |  | 9121 |
| r | GS022 |  | 9134 |
| r | GS022 |  | 9142 |
| r | GS022 |  | 9146 |
| r | GS022 |  | 9163 |
| r | GS022 |  | 9169 |
| r | GS022 |  | 9181 |
| r | GS022 |  | 9182 |
| r | GS022 |  | 9187 |
| r | GS022 |  | 9188 |
| r | GS022 |  | 9193 |
| r | GS022 |  | 9194 |
| r | GS022 |  | 9205 |
| r | GS022 |  | 9210 |
| r | GS022 |  | 9213 |
| r | GS022 |  | 9219 |
| r | GS022 |  | 9239 |
| r | GS022 |  | 9241 |
| r | GS022 |  | 9248 |
| r | GS022 |  | 9250 |
| r | GS022 |  | 9257 |
| r | GS022 |  | 9258 |
| r | GS022 |  | 9262 |
| r | GS022 |  | 9268 |
| r | GS022 |  | 9269 |
| r | GS022 |  | 9283 |
| r | GS022 |  | 9469 |
| r | GS022 |  | 9516 |
| r | GS022 |  | 9519 |
| r | GS022 |  | 9524 |
| r | GS022 |  | 9729 |
| r | GS022 |  | 199 |
| r | GS022 |  | 85 |
| r | GS022 |  | 291 |
| r | GS022 |  | 300 |
| r | GS022 |  | 15 |
| r | GS022 |  | 717 |
| r | GS022 |  | 756 |
| r | GS022 |  | 52 |
| r | GS022 |  | 153 |
| r | GS022 |  | 166 |
| r | GS022 |  | 227 |
| r | GS022 |  | 304 |
| r | GS022 |  | 15 |
| r | GS022 |  | 146 |
| r | GS022 |  | 8 |
| r | GS022 |  | 10 |
| r | GS022 |  | 13 |
| r | GS022 |  | 20 |
| r | GS022 |  | 22 |
| r | GS022 |  | 24 |
| r | GS022 |  | 27 |
| r | GS022 |  | 38 |
| r | GS022 |  | 40 |
| r | GS022 |  | 43 |
| r | GS022 |  | 52 |
| r | GS022 |  | 11 |
| r | GS022 |  | 40 |
| r | GS022 |  | 431 |
| r | GS022 |  | 461 |
| r | GS022 |  | 1600 |
| r | GS022 |  | 1950 |
| r | GS022 |  | 1987 |
| r | GS022 |  | 163 |
| r | GS022 |  | 177 |
| r | GS022 |  | 179 |
| r | GS022 |  | 182 |
| r | GS022 |  | 186 |
| r | GS022 |  | 192 |
| r | GS022 |  | 196 |
| r | GS022 |  | 203 |
| r | GS022 |  | 208 |
| r | GS022 |  | 273 |
| r | GS022 |  | 288 |
| r | GS022 |  | 405 |
| r | GS022 |  | 411 |
| r | GS022 |  | 425 |
| r | GS022 |  | 61 |
| r | GS022 |  | 391 |
| r | GS022 |  | 412 |
| r | GS022 |  | 29 |
| r | GS022 |  | 55 |
| r | GS022 |  | 89 |
| r | GS022 |  | 307 |
| r | GS022 |  | 343 |
| r | GS022 |  | 181 |
| r | GS022 |  | 11 |
| r | GS022 |  | 21 |
| r | GS022 |  | 31 |
| r | GS022 |  | 789 |
| r | GS022 |  | 23 |
| r | GS022 |  | 1668 |
| r | GS022 |  | 1668 |
| r | GS022 |  | 1718 |
| r | GS022 |  | 1731 |
| r | GS022 |  | 1812 |
| r | GS022 |  | 160 |
| r | GS022 |  | 111 |
| r | GS022 |  | 116 |
| r | GS022 |  | 129 |
| r | GS022 |  | 1515 |
| r | GS022 |  | 333 |
| r | GS022 |  | 340 |
| r | GS022 |  | 70 |
| r | GS022 |  | 72 |
| r | GS022 |  | 55 |
| r | GS022 |  | 63 |
| r | GS022 |  | 117 |
| r | GS022 |  | 123 |
| r | GS022 |  | 226 |
| r | GS022 |  | 234 |
| r | GS022 |  | 263 |
| r | GS022 |  | 269 |
| r | GS022 |  | 3 |
| r | GS022 |  | 240 |
| r | GS022 |  | 255 |
| r | GS022 |  | 262 |
| r | GS022 |  | 251 |
| r | GS022 |  | 299 |
| r | GS022 |  | 311 |
| r | GS022 |  | 384 |
| r | GS022 |  | 87 |
| r | GS022 |  | 197 |
| r | GS022 |  | 275 |
| r | GS022 |  | 174 |
| r | GS022 |  | 179 |
| r | GS022 |  | 48 |
| r | GS022 |  | 201 |
| r | GS022 |  | 1 |
| r | GS022 |  | 29 |
| r | GS022 |  | 75 |
| r | GS022 |  | 75 |
| r | GS022 |  | 92 |
| r | GS022 |  | 92 |
| r | GS022 |  | 289 |
| r | GS022 |  | 294 |
| r | GS022 |  | 66 |
| r | GS022 |  | 109 |
| r | GS022 |  | 200 |
| r | GS022 |  | 216 |
| r | GS022 |  | 231 |
| r | GS022 |  | 235 |
| r | GS022 |  | 276 |
| r | GS022 |  | 318 |
| r | GS022 |  | 51 |
| r | GS022 |  | 91 |
| r | GS022 |  | 147 |
| r | GS022 |  | 40 |
| r | GS022 |  | 41 |
| r | GS022 |  | 41 |
| r | GS022 |  | 43 |
| r | GS022 |  | 66 |
| r | GS022 |  | 69 |
| r | GS022 |  | 90 |
| r | GS022 |  | 99 |
| r | GS022 |  | 102 |
| r | GS022 |  | 104 |
| r | GS022 |  | 117 |
| r | GS022 |  | 124 |
| r | GS022 |  | 146 |
| r | GS022 |  | 152 |
| r | GS022 |  | 155 |
| r | GS022 |  | 157 |
| r | GS022 |  | 180 |
| r | GS022 |  | 188 |
| r | GS022 |  | 350 |
| r | GS022 |  | 25 |
| r | GS022 |  | 177 |
| r | GS022 |  | 177 |
| r | GS022 |  | 61 |
| r | GS022 |  | 76 |
| r | GS022 |  | 76 |
| r | GS022 |  | 21 |
| r | GS022 |  | 30 |
| r | GS022 |  | 52 |
| r | GS022 |  | 52 |
| r | GS022 |  | 254 |
| r | GS022 |  | 297 |
| r | GS022 |  | 349 |
| r | GS022 |  | 636 |
| r | GS022 |  | 330 |
| r | GS022 |  | 372 |
| r | GS022 |  | 374 |
| r | GS022 |  | 379 |
| r | GS022 |  | 535 |
| r | GS022 |  | 553 |
| r | GS022 |  | 186 |
| r | GS022 |  | 478 |
| r | GS022 |  | 422 |
| r | GS022 |  | 1897 |
| r | GS022 |  | 2071 |
| r | GS022 |  | 2115 |
| r | GS022 |  | 2328 |
| r | GS022 |  | 2392 |
| r | GS022 |  | 2410 |
| r | GS022 |  | 2507 |
| r | GS022 |  | 2570 |
| r | GS022 |  | 1897 |
| r | GS022 |  | 2115 |
| r | GS022 |  | 2328 |
| r | GS022 |  | 2392 |
| r | GS022 |  | 2410 |
| r | GS022 |  | 408 |
| r | GS022 |  | 1493 |
| r | GS022 |  | 17 |
| r | GS022 |  | 60 |
| r | GS022 |  | 63 |
| r | GS022 |  | 32 |
| r | GS022 |  | 35 |
| r | GS022 |  | 81 |
| r | GS022 |  | 33 |
| r | GS022 |  | 45 |
| r | GS022 |  | 43 |
| r | GS022 |  | 40 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
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
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| M | ? | prepare_commit_msg.py | 28 |
| M | ? | manage_translations.py | 48 |
| M | ? | manage_translations.py | 49 |
| M | ? | client.py | 31 |
| M | ? | utils.py | 175 |
| M | ? | version.py | 90 |
| M | ? | autoreload.py | 290 |
| H | ? | special.py | 37 |
| H | ? | special.py | 50 |
| H | ? | expressions.py | 1829 |
| H | ? | expressions.py | 1863 |
| H | ? | query.py | 1377 |
| H | ? | query.py | 2364 |
| H | ? | generated.py | 88 |
| H | ? | tuple_lookups.py | 386 |
| H | ? | query_utils.py | 540 |
| H | ? | query_utils.py | 544 |
| H | ? | query_utils.py | 550 |
| H | ? | query.py | 366 |
| H | ? | query.py | 402 |
| H | ? | query.py | 408 |
| H | ? | query.py | 438 |
| H | ? | query.py | 449 |
| H | ? | query.py | 534 |
| H | ? | query.py | 656 |
| H | ? | query.py | 663 |
| H | ? | query.py | 690 |
| H | ? | query.py | 726 |
| H | ? | query.py | 783 |
| H | ? | query.py | 1261 |
| H | ? | query.py | 1767 |
| H | ? | query.py | 1982 |
| H | ? | query.py | 2379 |
| H | ? | where.py | 221 |
| H | ? | where.py | 226 |
| H | ? | where.py | 287 |
| H | ? | subqueries.py | 68 |
| H | ? | compiler.py | 642 |
| H | ? | compiler.py | 667 |
| H | ? | compiler.py | 2018 |
| H | ? | options.py | 256 |
| H | ? | schema.py | 107 |
| H | ? | schema.py | 115 |
| H | ? | migrate.py | 358 |
| H | ? | adapter.py | 41 |
| H | ? | adapter.py | 58 |
| H | ? | geometry.py | 82 |
| H | ? | geometry.py | 91 |
| H | ? | geometry.py | 200 |
| H | ? | geometry.py | 240 |
| H | ? | geometry.py | 509 |
| H | ? | OLMapWidget.js | 257 |
| H | ? | geometries.py | 470 |
| H | ? | array.py | 151 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T04:05:07.279638*