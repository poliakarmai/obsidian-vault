---
title: "GSC Audit: /tmp/gsc-learn/uv"
date: 2026-07-15
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/uv

**Дата:** 15.07.2026 04:02  
**Путь:** `/tmp/gsc-learn/uv`  
**Всего находок:** 3491  
**CRITICAL:** 53 | **HIGH:** 3125 | **MEDIUM:** 102 | **LOW:** 210

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 3015 |
| GS003 | 208 |
| Хардкод IP адреса | 104 |
| Синхронный код в async | 49 |
| Python: assert in production | 29 |
| GS001 | 29 |
| Hardcoded encryption key | 24 |
| Outdated dependency pattern | 24 |
| GS002 | 2 |
| GS014 | 2 |
| CVE-2026-56233: Path traversal | 1 |
| World-readable file: uv.schema.json (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | login.rs | 142 | Found: password: ";
                uv_console::password(pro |
| CRITICAL | GS001 | publish.rs | 608 | Found: password: ";
    let username = uv_console::input(use |
| CRITICAL | GS001 | credentials.rs | 884 | Found: token = "super_secret_token" |
| CRITICAL | GS001 | middleware.rs | 1063 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1109 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1223 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1264 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1312 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1352 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1395 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1460 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1525 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 1556 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 2246 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 2341 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 2437 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 2551 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 2583 | Found: password = "password" |
| CRITICAL | GS001 | middleware.rs | 2606 | Found: password = "testpass" |
| CRITICAL | GS001 | middleware.rs | 2685 | Found: password = "token" |
| CRITICAL | GS001 | store.rs | 495 | Found: password = "testpass" |
| CRITICAL | GS001 | store.rs | 500 | Found: password = "pass2" |
| CRITICAL | GS001 | registry_client.rs | 1902 | Found: password = "password" |
| CRITICAL | GS001 | registry_client.rs | 1958 | Found: password = "password" |
| CRITICAL | GS001 | registry_client.rs | 2008 | Found: password = "password" |
| CRITICAL | GS001 | mock.rs | 246 | Found: password = "test ascii password" |
| CRITICAL | GS001 | secret_service.rs | 64 | Found: Password: " pass
    echo -n " |
| CRITICAL | GS001 | secret_service.rs | 771 | Found: password = "password in new collection" |
| CRITICAL | GS001 | windows.rs | 751 | Found: password = "test get password" |
| CRITICAL | ? | registry_client.rs | 1902 | Match:         let password = "password"; |
| CRITICAL | ? | registry_client.rs | 1958 | Match:         let password = "password"; |
| CRITICAL | ? | registry_client.rs | 2008 | Match:         let password = "password"; |
| CRITICAL | ? | store.rs | 495 | Match: password = "testpass" |
| CRITICAL | ? | credentials.rs | 884 | Match:         let token = "super_secret_token"; |
| CRITICAL | ? | middleware.rs | 1063 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1109 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1223 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1264 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1312 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1352 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1395 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1460 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1525 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 1556 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 2246 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 2341 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 2437 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 2551 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 2583 | Match:         let password = "password"; |
| CRITICAL | ? | middleware.rs | 2606 | Match:         let password = "testpass"; |
| CRITICAL | ? | mock.rs | 246 | Match:         let password = "test ascii password"; |
| CRITICAL | ? | secret_service.rs | 771 | Match:         let password = "password in new collection"; |
| CRITICAL | ? | windows.rs | 751 | Match:         let password = "test get password"; |
| HIGH | ? | update_schemastore.py | 61 |  |
| HIGH | ? | wheel.rs | 544 | Match:             "example-1.2.3.4.5.6.7.8.9.0.1.2.3.4.5.6. |
| HIGH | ? | wheel.rs | 546 | Match:         insta::assert_snapshot!(filename.cache_key(), |
| HIGH | ? | lib.rs | 1337 | Match:         let listener = std::net::TcpListener::bind("1 |
| HIGH | ? | pyproject_mut.rs | 1960 | Match:             ("0.0.0.1", "==0.0.0.1"), |
| HIGH | ? | pyproject_mut.rs | 1964 | Match:             ("1.2.3.4", "==1.2.3.4"), |
| HIGH | ? | pyproject_mut.rs | 1965 | Match:             ("1.2.3.4a1.post1", "==1.2.3.4a1.post1"), |
| HIGH | ? | pyproject_mut.rs | 1984 | Match:             ("0.0.0.1", ">=0.0.0.1"), |
| HIGH | ? | pyproject_mut.rs | 1989 | Match:             ("1.2.3.4", ">=1.2.3.4"), |
| HIGH | ? | pyproject_mut.rs | 1990 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1"), |
| HIGH | ? | pyproject_mut.rs | 2007 | Match:             ("0.0.0.0", ">=0.0.0.0, <0.1.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2010 | Match:             ("0.0.1.1", ">=0.0.1.1, <0.0.2.0"), |
| HIGH | ? | pyproject_mut.rs | 2011 | Match:             ("0.0.0.1", ">=0.0.0.1, <0.0.0.2"), |
| HIGH | ? | pyproject_mut.rs | 2016 | Match:             ("1.2.3.4", ">=1.2.3.4, <2.0.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2017 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1, < |
| HIGH | ? | pyproject_mut.rs | 2034 | Match:             ("0.0.0.0", ">=0.0.0.0, <0.0.1.0"), |
| HIGH | ? | pyproject_mut.rs | 2037 | Match:             ("0.0.1.1", ">=0.0.1.1, <0.0.2.0"), |
| HIGH | ? | pyproject_mut.rs | 2038 | Match:             ("0.0.0.1", ">=0.0.0.1, <0.0.0.2"), |
| HIGH | ? | pyproject_mut.rs | 2043 | Match:             ("1.2.3.4", ">=1.2.3.4, <1.3.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2044 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1, < |
| HIGH | ? | self_update.rs | 857 | Match:         let listener = TcpListener::bind("127.0.0.1:0 |
| HIGH | ? | keyring.rs | 610 | Match:         let url = Url::parse("http://127.0.0.1:8080/b |
| HIGH | ? | keyring.rs | 611 | Match:         let keyring = KeyringProvider::dummy([("http: |
| HIGH | ? | keyring.rs | 627 | Match:         let url = Url::parse("https://127.0.0.1:8080/ |
| HIGH | ? | keyring.rs | 628 | Match:         let keyring = KeyringProvider::dummy([("http: |
| HIGH | ? | service.rs | 35 | Match:             "http" if matches!(url.host_str(), Some(" |
| HIGH | ? | path.rs | 869 | Match:                 r"\\127.0.0.1\c$\path\to\logging.", |
| HIGH | ? | path.rs | 870 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 873 | Match:                 r"\\127.0.0.1\c$\path\to\.\logging.", |
| HIGH | ? | path.rs | 874 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 877 | Match:                 r"\\127.0.0.1\c$\path\to\..\to\loggin |
| HIGH | ? | path.rs | 878 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 881 | Match:                 r"//127.0.0.1/c$/path/to/../to/./logg |
| HIGH | ? | path.rs | 882 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 888 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 889 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | settings.rs | 417 | Match:             no-proxy = ["localhost", "127.0.0.1"] |
| HIGH | ? | tree.rs | 2784 | Match:             ("3.9.0.0.*", "3.9", "3.9.*"), |
| HIGH | ? | tree.rs | 2801 | Match:         let cases_false = ["3.9.1.*", "3.9.1.0.*", "3 |
| HIGH | ? | vendor.rs | 61 | Match:         url: "https://github.com/astral-sh/futzed-whe |
| HIGH | ? | vendor.rs | 67 | Match:         url: "https://github.com/astral-sh/futzed-whe |
| HIGH | ? | version.rs | 3609 | Match:         assert_eq!(p("1.2.3.4"), Version::new([1, 2,  |
| HIGH | ? | version.rs | 3610 | Match:         assert_eq!(p("1.2.3.4.5"), Version::new([1, 2 |
| HIGH | ? | version.rs | 4338 | Match:             "1!2.3.0.0" |
| HIGH | ? | version.rs | 4415 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4420 | Match:         assert_eq!(version.to_string().as_str(), "2.0 |
| HIGH | ? | version.rs | 4423 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4430 | Match:         assert_eq!(version.to_string().as_str(), "5!2 |
| HIGH | ? | version.rs | 4435 | Match:         assert_eq!(version.to_string().as_str(), "5!3 |
| HIGH | ? | version.rs | 4467 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4472 | Match:         assert_eq!(version.to_string().as_str(), "1.3 |
| HIGH | ? | version.rs | 4475 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4482 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4487 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4519 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4524 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4527 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4534 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4539 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4571 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4576 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4579 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4586 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4591 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4623 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4628 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4631 | Match:         let mut version = "5!1.7.3.5a2.post345.dev456 |
| HIGH | ? | version.rs | 4638 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4643 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4675 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4680 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4683 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4690 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4695 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4718 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4720 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4723 | Match:         let mut version = "5!1.7.3.5b2.dev123+local". |
| HIGH | ? | version.rs | 4725 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4727 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4750 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4752 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4755 | Match:         let mut version = "5!1.7.3.5b2.post345+local" |
| HIGH | ? | version.rs | 4759 | Match:             "5!1.7.3.5b2.post345.dev1+local" |
| HIGH | ? | version.rs | 4764 | Match:             "5!1.7.3.5b2.post345.dev2+local" |
| HIGH | ? | version.rs | 4788 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4790 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4793 | Match:         let mut version = "5!1.7.3.5b2.post345+local" |
| HIGH | ? | version.rs | 4795 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4797 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version_specifier.rs | 2182 | Match:             ("~=1.4.5", "~=1.4.5.0"), |
| HIGH | ? | Dockerfile | 13 | Match: ARG XWIN_CRT_VERSION=14.44.17.14 |
| HIGH | ? | home-assistant.in | 1323 | Match: knx-frontend==2023.6.23.191712 |
| HIGH | ? | home-assistant.in | 1362 | Match: lightify==1.0.7.3 |
| HIGH | ? | home-assistant.in | 1482 | Match: netmap==0.7.0.2 |
| HIGH | ? | home-assistant.in | 1801 | Match: pyatag==0.3.5.3 |
| HIGH | ? | home-assistant.in | 1915 | Match: pyezviz==0.2.1.2 |
| HIGH | ? | home-assistant.in | 2062 | Match: pymediaroom==0.6.5.4 |
| HIGH | ? | home-assistant.in | 2092 | Match: pynetio==0.1.9.1 |
| HIGH | ? | PKG-INFO | 1395 | Match: - Exclude typing-extensions version 3.10.0.1 due to i |
| HIGH | ? | pyproject.toml | 145 | Match:   "types-requests==2.31.0.6", # See https://github.co |
| HIGH | ? | pyproject.toml | 88 | Match:   "trove-classifiers==2026.1.14.14", |
| HIGH | ? | pyproject.toml | 91 | Match:   "types-aiofiles==25.1.0.20260409", |
| HIGH | ? | pyproject.toml | 26 | Match:     "types-requests >=2.31.0.20240406,<3", |
| HIGH | ? | pyproject.toml | 141 | Match:     "types-redis ~= 4.6.0.20240425", |
| HIGH | ? | pyproject.toml | 171 | Match:     "types-PyYAML ~= 6.0.12.20240311", |
| HIGH | ? | uv.schema.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | credentials.rs | 0 | File credentials.rs has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | credentials.rs | 0 | File credentials.rs has permissions -rw-rw-r-- — readable by |
| HIGH | ? | lib.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | candidate_selector.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | candidate_selector.rs | 797 | Clone in performance-critical code — consider references |
| HIGH | ? | candidate_selector.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | exclude_newer.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | graph_ops.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | graph_ops.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | graph_ops.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | graph_ops.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_urls.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_urls.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_urls.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_urls.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_urls.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | universal_marker.rs | 839 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | redirect.rs | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | redirect.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | redirect.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | redirect.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | redirect.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | redirect.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 359 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 415 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 471 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 495 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 753 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 802 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 889 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 890 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 914 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 916 | Clone in performance-critical code — consider references |
| HIGH | ? | output.rs | 947 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | display.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 506 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 626 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 668 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 670 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 697 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 698 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 722 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 736 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1730 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1838 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1892 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1967 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1982 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2101 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2119 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2188 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2345 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2399 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2406 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2410 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2431 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2432 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2530 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2537 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2541 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2661 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2666 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3053 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3191 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3346 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3367 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3379 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3382 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3387 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3396 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3411 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3418 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3419 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3424 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3429 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3437 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3444 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3451 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3471 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3482 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3486 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3490 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3494 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3499 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3505 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3545 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3555 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3556 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3567 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3579 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3591 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3608 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3617 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3626 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3627 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3632 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3635 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3642 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3643 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3647 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3650 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3660 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3669 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3670 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3674 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3676 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3695 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3696 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3701 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3705 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3713 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3718 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3728 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3729 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3751 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3767 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3768 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3776 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3780 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3788 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3804 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3805 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4057 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4061 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4063 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4075 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4126 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4184 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4188 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4189 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4271 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4324 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4328 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4334 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4342 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4468 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4546 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4571 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4590 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4594 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4800 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5208 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5226 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5244 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5351 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5546 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5577 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5585 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5590 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5598 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5603 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5613 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5619 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5632 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5642 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5659 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5682 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5692 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5828 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6152 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6171 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6172 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6196 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6207 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6215 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6216 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6322 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6323 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6456 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6480 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6496 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6500 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 818 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1027 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1094 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1101 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1117 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1119 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1120 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1121 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1123 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1129 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1130 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1135 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1141 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1142 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1144 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1186 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1220 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1222 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1236 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1297 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1310 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1364 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 471 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 637 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 753 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 754 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 980 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1078 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1094 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1205 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1210 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1227 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1228 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1235 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1236 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1296 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1312 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1324 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1336 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1348 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1371 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1375 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1383 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1384 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1388 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1390 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1395 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1397 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1398 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1412 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1424 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 506 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 526 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 532 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 545 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 578 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 764 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 847 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 869 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 934 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1066 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1068 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1076 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1077 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1078 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1093 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1097 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1100 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1105 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1109 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1112 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1116 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1120 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1125 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1128 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1146 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1166 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1215 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1229 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1232 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1235 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1237 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1240 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1246 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1393 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1398 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1414 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1421 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1426 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1447 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1451 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1460 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1468 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1501 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1517 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1522 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1529 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1536 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1547 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1548 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1552 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1554 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1568 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1574 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1578 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1608 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1612 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1621 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1629 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1639 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1662 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1683 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1694 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1702 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1703 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1708 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1709 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1710 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1712 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1717 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1729 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1737 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1742 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclonedx_json.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclonedx_json.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclonedx_json.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclonedx_json.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclonedx_json.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclonedx_json.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | cyclonedx_json.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | requirements_txt.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 407 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 472 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 646 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 647 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 648 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 769 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 833 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 890 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 897 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 1345 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 749 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 802 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 808 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 888 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 898 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 923 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 924 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 938 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 952 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 953 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 954 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 955 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 968 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 971 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 973 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 979 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 981 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1010 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1012 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1043 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1115 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1141 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1142 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1167 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1168 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1200 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1201 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1206 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1207 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1212 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1230 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1231 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1237 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1238 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1244 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1245 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1251 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1252 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1253 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1254 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1259 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1260 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1290 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1291 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1292 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1293 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1304 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1309 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1365 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1366 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1371 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1372 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1387 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1388 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1393 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1394 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1788 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1795 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1796 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1830 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1840 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1842 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1947 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1968 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1987 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2057 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2450 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2462 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2463 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2496 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2498 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2501 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2502 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2511 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2517 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2761 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2763 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2765 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2766 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2769 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2770 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2771 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2772 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2793 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2795 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 368 | Clone in performance-critical code — consider references |
| HIGH | ? | dependencies.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | range.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | package.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | package.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | marker.rs | 22 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 670 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 715 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 699 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1014 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1091 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1201 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1204 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1208 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1209 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1210 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1218 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1552 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1602 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1609 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 1680 | Clone in performance-critical code — consider references |
| HIGH | ? | yanks.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | yanks.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | yanks.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | yanks.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | provider.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 288 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 584 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 629 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 768 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 769 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 774 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 777 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 916 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 973 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1034 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1038 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1047 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1049 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1053 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1054 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1102 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1104 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1105 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1106 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1140 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1154 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1189 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1204 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1264 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1272 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1274 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1311 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1324 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1341 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1343 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1349 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1373 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1381 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1388 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1394 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1400 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1431 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1434 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1477 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1520 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1575 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1622 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1623 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1690 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1746 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1748 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1751 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1753 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1781 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1782 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1790 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1814 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1823 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1923 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1943 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1966 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1969 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1977 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1979 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1989 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2047 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2052 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2075 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2080 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2101 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2103 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2106 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2186 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2207 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2208 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2210 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2211 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2239 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2241 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2242 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2243 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2289 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2392 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2393 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2394 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2395 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2396 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2429 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2430 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2431 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2432 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2433 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2578 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2607 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2608 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2623 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2624 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2648 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2662 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2708 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2714 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2718 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2777 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2789 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2798 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2831 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2844 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2846 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2872 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2881 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2884 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2909 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2932 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2939 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2952 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2956 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2957 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2958 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2959 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2966 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2967 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2968 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3240 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3241 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3245 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3251 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3271 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3368 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3382 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3507 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3512 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3513 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3516 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3517 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3539 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3544 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3545 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3571 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3576 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3577 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3580 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3589 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3594 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3595 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3621 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3626 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3627 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3631 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3656 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3657 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3779 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3866 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3933 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3962 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3981 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4002 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4008 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4019 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4026 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4066 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4123 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4135 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4347 | Clone in performance-critical code — consider references |
| HIGH | ? | urls.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | urls.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | urls.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | urls.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | urls.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | urls.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | urls.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | indexes.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_map.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_map.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_map.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_map.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_map.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | batch_prefetch.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | derivation.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | derivation.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | derivation.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | availability.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 313 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 623 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 765 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | preferences.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | pins.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | pins.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | pins.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_indexes.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_indexes.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_indexes.rs | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | fork_indexes.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | control.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 985 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 987 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 584 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 601 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 702 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 485 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 616 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 622 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 629 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 634 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 668 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 688 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 734 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 740 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 760 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 819 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 824 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 826 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 831 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 840 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 846 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 852 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 858 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 864 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 870 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 876 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 891 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 896 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 919 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 964 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 983 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1017 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1062 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1073 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1095 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1127 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1134 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1142 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1145 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1206 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1213 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1219 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1238 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1240 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1241 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1244 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1249 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1264 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1280 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1292 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1302 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1374 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1457 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1521 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1589 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1609 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1610 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1638 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1937 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1987 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 2037 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 430 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 474 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 566 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 594 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 609 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 631 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 639 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 888 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1023 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1129 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1135 | Clone in performance-critical code — consider references |
| HIGH | ? | retry.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 351 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | html.rs | 25 | Clone in performance-critical code — consider references |
| HIGH | ? | html.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | html.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | remote_metadata.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | remote_metadata.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | remote_metadata.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | tags.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 309 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 361 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 407 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | site_packages.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | preparer.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | satisfies.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | satisfies.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 610 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 686 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 720 | Clone in performance-critical code — consider references |
| HIGH | ? | plan.rs | 746 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 10 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 11 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 417 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 474 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 576 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 600 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 662 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 712 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 737 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 816 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 841 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 924 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1184 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1226 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 359 | Clone in performance-critical code — consider references |
| HIGH | ? | overrides.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | package_options.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | package_options.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | package_options.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | package_options.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | constraints.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | constraints.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | extras.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | extras.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | proxy_url.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | proxy_url.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | libc.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | libc.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | libc.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 556 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 794 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 809 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 835 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1216 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1219 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1255 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1357 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 331 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 557 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 570 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 631 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 637 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 687 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 766 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 851 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 865 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 879 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1063 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1068 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1076 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1150 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1152 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1154 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1155 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1156 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1162 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1172 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1175 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1186 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1191 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1293 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1319 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1331 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1333 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1340 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1359 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1507 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1563 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1568 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1601 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1604 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1669 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1699 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1700 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1712 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1713 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1723 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1741 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1745 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1749 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1759 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1771 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1780 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1785 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1844 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1871 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2047 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2051 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2060 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2084 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2087 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2088 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2096 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2104 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2107 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2116 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2132 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2136 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2191 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2192 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2193 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2195 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2293 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 534 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1305 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1451 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1477 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1491 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1497 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1584 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1611 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1687 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1688 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1694 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1695 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1696 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1822 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1835 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1861 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1874 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 564 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 686 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | direct_url.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata_resolver.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | module_name.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | simple_json.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | simple_json.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 585 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 708 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 713 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 715 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 724 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 725 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1117 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1120 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1123 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1615 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6826 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6827 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6828 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6889 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6890 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6891 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | file.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | config_settings.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | config_settings.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | config_settings.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | traits.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | traits.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | traits.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | prioritized_distribution.rs | 533 | Clone in performance-critical code — consider references |
| HIGH | ? | prioritized_distribution.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | prioritized_distribution.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | prioritized_distribution.rs | 561 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 26 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 113 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 537 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_python.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | resolved.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | resolved.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | resolved.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | any.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | any.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 632 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 685 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 696 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 930 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 986 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 1135 | Clone in performance-critical code — consider references |
| HIGH | ? | requirement.rs | 1149 | Clone in performance-critical code — consider references |
| HIGH | ? | installed.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 187 | Clone in performance-critical code — consider references |
| HIGH | ? | specified_requirement.rs | 193 | Clone in performance-critical code — consider references |
| HIGH | ? | specified_requirement.rs | 194 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | resolution.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | id.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | id.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | id.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | id.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | id.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | id.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | id.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | dist_error.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | dist_error.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | dist_error.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | dist_error.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | dist_error.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | dist_error.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_metadata.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | status_code_strategy.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | status_code_strategy.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | cached.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | annotation.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 804 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 815 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 826 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 838 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 848 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 849 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 858 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 859 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 869 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 870 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 880 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1027 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1060 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1061 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1423 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1427 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1776 | Clone in performance-critical code — consider references |
| HIGH | ? | trusted_publishing.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | pypi.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | pypi.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | pypi.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | pypi.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | pypi.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | pypi.rs | 90 | Clone in performance-critical code — consider references |
| HIGH | ? | pypi.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 361 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 566 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 567 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 606 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 607 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 682 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 753 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 771 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 786 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 792 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 812 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 838 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 844 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 853 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 898 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 930 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 937 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 962 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 963 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 965 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1044 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1051 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1071 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1139 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1238 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1244 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1245 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1256 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1280 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1327 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1341 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1367 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1371 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1412 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1422 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1426 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1636 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1700 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1775 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 56 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 472 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 562 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 587 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 244 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 523 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 526 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 185 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 927 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 1053 | Clone in performance-critical code — consider references |
| HIGH | ? | operations.rs | 1061 | Clone in performance-critical code — consider references |
| HIGH | ? | freeze.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | venv.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | venv.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | venv.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | venv.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 417 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 611 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 628 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 646 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 766 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1161 | Clone in performance-critical code — consider references |
| HIGH | ? | logout.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | logout.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | logout.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | logout.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | login.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | login.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | login.rs | 69 | Clone in performance-critical code — consider references |
| HIGH | ? | login.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | login.rs | 189 | Clone in performance-critical code — consider references |
| HIGH | ? | login.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | login.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 91 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 356 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 654 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 661 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 690 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 715 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 438 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 461 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 477 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 502 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 790 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 805 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 814 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 818 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 824 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 911 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 938 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 670 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 759 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 789 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 791 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 797 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 804 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 910 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 965 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 605 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 711 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 833 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 839 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 855 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 856 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 887 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 889 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 891 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 899 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 917 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 922 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 957 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 961 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 981 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 988 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1038 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1053 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1104 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostics.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostics.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | diagnostics.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | self_update.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | self_update.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | self_update.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | self_update.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | self_update.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | self_update.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | list.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 645 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 648 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 661 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 666 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 724 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 835 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1022 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1037 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1040 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1042 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1089 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1162 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1176 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1184 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1198 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1201 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1203 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1208 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1219 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1227 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | help.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 258 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 631 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 639 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 647 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 648 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 668 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 682 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 969 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 982 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 989 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1167 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1503 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1556 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1599 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1605 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2190 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2199 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2200 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2213 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2217 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2231 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2243 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2253 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2254 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2256 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2257 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2380 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2425 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2432 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2433 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2435 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2445 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2449 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2458 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2460 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2479 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2511 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2523 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2533 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2534 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2536 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2537 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2611 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2620 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2621 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2653 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2665 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2675 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2679 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2783 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2868 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2875 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2876 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2878 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2896 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2898 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2930 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2940 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2941 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2943 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2944 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2961 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2966 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3087 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3091 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3093 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3126 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3131 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3133 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3308 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | ty.rs | 68 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 361 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 121 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 677 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 684 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 685 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 686 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 689 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 704 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 868 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 878 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 879 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 881 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 882 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 950 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 997 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1000 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1004 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1022 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1030 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1078 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1321 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1475 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 719 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 724 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 732 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 743 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 747 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 766 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 768 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 769 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 791 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 826 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 976 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 977 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 993 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1016 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1027 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1566 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 367 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 445 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 477 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | toolchain.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | toolchain.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1043 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1341 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1438 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1539 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1544 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1549 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1580 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1591 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1605 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1618 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1772 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1776 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1803 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1807 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 466 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 471 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 728 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 932 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 959 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 967 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 968 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 969 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 977 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 983 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 987 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 988 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 1157 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 1292 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 1440 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | remove.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 474 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 556 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | json.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | json.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | json.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 237 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 430 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 489 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 758 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 759 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 811 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 955 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 960 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 963 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1080 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1085 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1088 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1237 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1254 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1396 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1397 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1398 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1407 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1413 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1419 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1486 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1577 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1691 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1747 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1844 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1845 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1949 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2023 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2024 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2075 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2076 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2081 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2129 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2130 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2305 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2350 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2510 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2511 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2602 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2603 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2699 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2700 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2726 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2843 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2844 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2891 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3040 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3041 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3081 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3154 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3155 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3160 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3188 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3193 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3239 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3245 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3344 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3360 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3369 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3381 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3389 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3649 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3665 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3674 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4112 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4118 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4326 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4329 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4332 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4344 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4441 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4456 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4459 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4462 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4751 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4857 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4981 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 5170 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 120 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 472 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 637 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 735 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 736 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 812 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 854 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 855 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 900 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 998 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1011 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1025 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1026 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1061 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1297 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1365 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1366 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1500 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1534 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1535 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1625 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1626 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1627 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1655 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2049 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2050 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2162 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2292 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2293 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2363 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2364 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2420 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2421 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2468 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2539 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2552 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2566 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2567 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2635 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2636 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2690 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2691 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2861 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2862 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 622 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1077 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1084 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1090 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1110 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1116 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1134 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1329 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1343 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1369 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1414 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1455 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1461 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1510 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1515 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1571 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 1814 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 2273 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 2932 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 2971 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 3098 | Clone in performance-critical code — consider references |
| HIGH | ? | discovery.rs | 3333 | Clone in performance-critical code — consider references |
| HIGH | ? | replacements.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 24 | Clone in performance-critical code — consider references |
| HIGH | ? | target.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | target.rs | 15 | Clone in performance-critical code — consider references |
| HIGH | ? | target.rs | 17 | Clone in performance-critical code — consider references |
| HIGH | ? | windows_registry.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | interpreter.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | interpreter.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | interpreter.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | interpreter.rs | 1224 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1010 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1016 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1141 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1143 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1149 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1248 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1295 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1296 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1412 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1608 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1832 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1835 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 1845 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 2155 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 2187 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 2219 | Clone in performance-critical code — consider references |
| HIGH | ? | downloads.rs | 2251 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 288 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 321 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | managed.rs | 810 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 230 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 831 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | installation.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1039 | Clone in performance-critical code — consider references |
| HIGH | ? | build.rs | 14 | Clone in performance-critical code — consider references |
| HIGH | ? | source.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | source.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | source.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | resolver.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | resolver.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | resolver.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | resolver.rs | 213 | Clone in performance-critical code — consider references |
| HIGH | ? | resolver.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | resolver.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | git.rs | 242 | Clone in performance-critical code — consider references |
| HIGH | ? | git.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | git.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | git.rs | 881 | Clone in performance-critical code — consider references |
| HIGH | ? | git.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | git.rs | 898 | Clone in performance-critical code — consider references |
| HIGH | ? | git.rs | 935 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 779 | Clone in performance-critical code — consider references |
| HIGH | ? | tool.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 192 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | cache.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 404 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 576 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 623 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 711 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 712 | Clone in performance-critical code — consider references |
| HIGH | ? | store.rs | 719 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 600 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 607 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 682 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 734 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 744 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 756 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 766 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 788 | Clone in performance-critical code — consider references |
| HIGH | ? | credentials.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 719 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 742 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 755 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 758 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 777 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 780 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 785 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 802 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 840 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 967 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 974 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1072 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1094 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1126 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1148 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1180 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1202 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1291 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1373 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1381 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1421 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1429 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1438 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1441 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1446 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1488 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1496 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1505 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1542 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1591 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1720 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1723 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1733 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1736 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1832 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1837 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1870 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1960 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1965 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1970 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1973 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1978 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1983 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 1986 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2019 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2067 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2068 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2075 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2080 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2085 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2088 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2093 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2107 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2110 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2163 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2164 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2168 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2169 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2179 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2180 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2188 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2193 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2198 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2201 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2206 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2220 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2223 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2271 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2272 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2281 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2291 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2297 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2300 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2305 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2308 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2326 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2330 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2331 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2368 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2383 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2463 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2561 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2616 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 2707 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | pyx.rs | 511 | Clone in performance-critical code — consider references |
| HIGH | ? | providers.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 704 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 891 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 906 | Clone in performance-critical code — consider references |
| HIGH | ? | validate_zip.rs | 40 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_cli_reference.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 58 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 375 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 383 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 384 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 459 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | builds.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 298 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 310 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 617 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 794 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 970 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 976 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1004 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1076 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1083 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1093 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1099 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1104 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1111 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1161 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1166 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1171 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1178 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 243 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 632 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 722 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 760 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 775 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 776 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 806 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 901 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 914 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 927 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 934 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 936 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 937 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 274 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 430 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 431 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_wheel_index.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_wheel_index.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | built_wheel_index.rs | 349 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 284 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 597 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 711 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 844 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 977 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 997 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1003 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1022 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1311 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1432 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1492 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1548 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1571 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1600 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1636 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1667 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1686 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1737 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1745 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1845 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1955 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2122 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2181 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2314 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2350 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2388 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2416 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2445 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2483 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2514 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2571 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2752 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2774 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2784 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2786 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3001 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3049 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3140 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3161 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3162 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3490 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3491 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3497 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3499 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3500 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3512 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3513 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3519 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3520 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 341 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 420 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 437 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 521 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 536 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 545 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 677 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 532 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 539 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 60 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 79 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 117 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 171 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | macos.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | mock.rs | 111 | Clone in performance-critical code — consider references |
| HIGH | ? | mock.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | secret_service.rs | 702 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 610 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | windows.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | glob.rs | 122 | Clone in performance-critical code — consider references |
| HIGH | ? | git_info.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | git_info.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | git_info.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | locked_file.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 849 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 1535 | Clone in performance-critical code — consider references |
| HIGH | ? | link.rs | 1536 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 240 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 431 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 486 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 440 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 359 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 558 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 604 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 755 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 765 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 869 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2365 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2651 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2842 | Clone in performance-critical code — consider references |
| HIGH | ? | combine.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | combine.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 946 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | unnamed.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | unnamed.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 144 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 354 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 491 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 583 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 584 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 622 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 623 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 649 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 650 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | lookahead.rs | 215 | Clone in performance-critical code — consider references |
| HIGH | ? | source_tree.rs | 133 | Clone in performance-critical code — consider references |
| HIGH | ? | source_tree.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | source_tree.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | source_tree.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | extras.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | extras.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 82 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 102 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 299 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | project_status.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | project_status.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | project_status.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 191 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 1189 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 3670 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 3675 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 3682 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 697 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 728 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 762 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 776 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 797 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 844 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 911 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 980 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 987 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 994 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 1432 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 1575 | Clone in performance-critical code — consider references |
| HIGH | ? | algebra.rs | 1887 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 59 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | simplify.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | unnamed.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | unnamed.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 728 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 739 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 944 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 972 | Clone in performance-critical code — consider references |
| HIGH | ? | options_metadata.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | options_metadata.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | find_links.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 779 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 804 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | linker.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | linker.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | script.rs | 112 | Clone in performance-critical code — consider references |
| HIGH | ? | main.rs | 16 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 2464 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 606 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 609 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 622 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 641 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 736 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 862 | Clone in performance-critical code — consider references |
| HIGH | ? | version_specifier.rs | 1032 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 358 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 370 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 429 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 688 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 787 | Clone in performance-critical code — consider references |
| HIGH | ? | version_ranges.rs | 890 | Clone in performance-critical code — consider references |
| HIGH | ? | line_wrap.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | package_name.rs | 75 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | _musllinux.py | 77 |
| M | ? | _manylinux.py | 94 |
| M | ? | resolver.py | 222 |
| M | ? | resolver.py | 265 |
| M | ? | resolver.py | 446 |
| M | ? | resolver.py | 458 |
| M | ? | resolver.py | 502 |
| M | ? | resolver.py | 514 |
| M | ? | resolver.py | 539 |
| M | ? | resolver.py | 551 |
| M | ? | resolver.py | 584 |
| M | ? | resolver.py | 595 |
| M | ? | resolver.py | 703 |
| M | ? | resolver.py | 713 |
| M | ? | resolver.py | 748 |
| M | ? | resolver.py | 758 |
| M | ? | resolver.py | 778 |
| M | ? | resolver.py | 788 |
| M | ? | resolver.py | 813 |
| M | ? | resolver.py | 823 |
| M | ? | resolver.py | 923 |
| M | ? | resolver.py | 1108 |
| M | ? | resolver.py | 1118 |
| M | ? | resolver.py | 1156 |
| M | ? | resolver.py | 1166 |
| M | ? | resolver.py | 1189 |
| M | ? | resolver.py | 1199 |
| M | ? | resolver.py | 1227 |
| M | ? | resolver.py | 1237 |
| H | ? | update_schemastore.py | 61 |
| C | GS001 | login.rs | 142 |
| C | GS001 | publish.rs | 608 |
| C | GS001 | credentials.rs | 884 |
| C | GS001 | middleware.rs | 1063 |
| C | GS001 | middleware.rs | 1109 |
| C | GS001 | middleware.rs | 1223 |
| C | GS001 | middleware.rs | 1264 |
| C | GS001 | middleware.rs | 1312 |
| C | GS001 | middleware.rs | 1352 |
| C | GS001 | middleware.rs | 1395 |
| C | GS001 | middleware.rs | 1460 |
| C | GS001 | middleware.rs | 1525 |
| C | GS001 | middleware.rs | 1556 |
| C | GS001 | middleware.rs | 2246 |
| C | GS001 | middleware.rs | 2341 |
| C | GS001 | middleware.rs | 2437 |
| C | GS001 | middleware.rs | 2551 |
| C | GS001 | middleware.rs | 2583 |
| C | GS001 | middleware.rs | 2606 |
| C | GS001 | middleware.rs | 2685 |
| C | GS001 | store.rs | 495 |
| C | GS001 | store.rs | 500 |
| C | GS001 | registry_client.rs | 1902 |
| C | GS001 | registry_client.rs | 1958 |
| C | GS001 | registry_client.rs | 2008 |
| C | GS001 | mock.rs | 246 |
| C | GS001 | secret_service.rs | 64 |
| C | GS001 | secret_service.rs | 771 |
| C | GS001 | windows.rs | 751 |
| L | GS003 | __main__.py | 5 |
| L | GS003 | pip_compileall.py | 21 |
| L | GS003 | pip_compileall.py | 33 |
| L | GS003 | pip_compileall.py | 67 |
| L | GS003 | get_interpreter_info.py | 26 |
| L | GS003 | get_interpreter_info.py | 448 |
| L | GS003 | get_interpreter_info.py | 497 |
| L | GS003 | get_interpreter_info.py | 510 |
| L | GS003 | get_interpreter_info.py | 558 |
| L | GS003 | get_interpreter_info.py | 600 |
| L | GS003 | get_interpreter_info.py | 671 |
| L | GS003 | get_interpreter_info.py | 718 |
| L | GS003 | _musllinux.py | 78 |
| L | GS003 | _musllinux.py | 80 |
| L | GS003 | _musllinux.py | 81 |
| L | GS003 | _musllinux.py | 83 |
| L | GS003 | check-trampoline-version-consistency.py | 39 |
| L | GS003 | check-trampoline-version-consistency.py | 41 |
| L | GS003 | check-trampoline-version-consistency.py | 44 |
| L | GS003 | check-trampoline-version-consistency.py | 50 |
| L | GS003 | check_uv_wheel_contents.py | 60 |
| L | GS003 | check_uv_wheel_contents.py | 61 |
| L | GS003 | check_uv_wheel_contents.py | 62 |
| L | GS003 | check_uv_wheel_contents.py | 64 |
| L | GS003 | check_uv_wheel_contents.py | 66 |
| L | GS003 | check_uv_wheel_contents.py | 68 |
| L | GS003 | check_uv_wheel_contents.py | 80 |
| L | GS003 | create-python-mirror.py | 279 |
| L | GS003 | create-python-mirror.py | 281 |
| L | GS003 | create-python-mirror.py | 283 |
| L | GS003 | create-python-mirror.py | 284 |
| L | GS003 | patch-dist-manifest-checksums.py | 47 |
| L | GS003 | patch-dist-manifest-checksums.py | 59 |
| L | GS003 | patch-dist-manifest-checksums.py | 66 |
| L | GS003 | publish-crates.py | 105 |
| L | GS003 | publish-crates.py | 128 |
| L | GS003 | publish-crates.py | 130 |
| L | GS003 | publish-crates.py | 133 |
| L | GS003 | registries-test.py | 132 |
| L | GS003 | registries-test.py | 185 |
| L | GS003 | registries-test.py | 189 |
| L | GS003 | registries-test.py | 192 |
| L | GS003 | registries-test.py | 235 |
| L | GS003 | registries-test.py | 243 |
| L | GS003 | registries-test.py | 245 |
| L | GS003 | registries-test.py | 246 |
| L | GS003 | registries-test.py | 249 |
| L | GS003 | registries-test.py | 254 |
| L | GS003 | registries-test.py | 256 |
| L | GS003 | registries-test.py | 258 |
| L | GS003 | registries-test.py | 262 |
| L | GS003 | registries-test.py | 264 |
| L | GS003 | registries-test.py | 336 |
| L | GS003 | registries-test.py | 340 |
| L | GS003 | registries-test.py | 341 |
| L | GS003 | registries-test.py | 359 |
| L | GS003 | registries-test.py | 362 |
| L | GS003 | registries-test.py | 367 |
| L | GS003 | registries-test.py | 372 |
| L | GS003 | registries-test.py | 402 |
| L | GS003 | registries-test.py | 405 |
| L | GS003 | registries-test.py | 407 |
| L | GS003 | registries-test.py | 409 |
| L | GS003 | registries-test.py | 411 |
| L | GS003 | registries-test.py | 413 |
| L | GS003 | registries-test.py | 415 |
| L | GS003 | registries-test.py | 416 |
| L | GS003 | registries-test.py | 420 |
| L | GS003 | registries-test.py | 424 |
| L | GS003 | registries-test.py | 425 |
| L | GS003 | registries-test.py | 429 |
| L | GS003 | registries-test.py | 430 |
| L | GS003 | registries-test.py | 431 |
| L | GS003 | registries-test.py | 432 |
| L | GS003 | registries-test.py | 435 |
| L | GS003 | repair-sdist-cargo-lock.py | 26 |
| L | GS003 | repair-sdist-cargo-lock.py | 37 |
| L | GS003 | repair-sdist-cargo-lock.py | 48 |
| L | GS003 | repair-sdist-cargo-lock.py | 56 |
| L | GS003 | repair-sdist-cargo-lock.py | 64 |
| L | GS003 | repair-sdist-cargo-lock.py | 71 |
| L | GS003 | repair-sdist-cargo-lock.py | 76 |
| L | GS003 | repair-sdist-cargo-lock.py | 79 |
| L | GS003 | repair-sdist-cargo-lock.py | 82 |
| L | GS003 | reverse-changelog.py | 37 |
| L | GS003 | reverse-changelog.py | 51 |
| L | GS003 | setup-crates-io-publish.py | 186 |
| L | GS003 | setup-crates-io-publish.py | 250 |
| L | GS003 | setup-crates-io-publish.py | 256 |
| L | GS003 | setup-crates-io-publish.py | 263 |
| L | GS003 | setup-crates-io-publish.py | 268 |
| L | GS003 | setup-crates-io-publish.py | 305 |
| L | GS003 | setup-crates-io-publish.py | 313 |
| L | GS003 | setup-crates-io-publish.py | 317 |
| L | GS003 | setup-crates-io-publish.py | 322 |
| L | GS003 | setup-crates-io-publish.py | 336 |
| L | GS003 | setup-crates-io-publish.py | 356 |
| L | GS003 | setup-crates-io-publish.py | 384 |
| L | GS003 | setup-crates-io-publish.py | 386 |
| L | GS003 | setup-crates-io-publish.py | 391 |
| L | GS003 | setup-crates-io-publish.py | 399 |
| L | GS003 | setup-crates-io-publish.py | 401 |
| L | GS003 | setup-crates-io-publish.py | 404 |
| L | GS003 | setup-crates-io-publish.py | 413 |
| L | GS003 | setup-crates-io-publish.py | 421 |
| L | GS003 | setup-crates-io-publish.py | 428 |
| L | GS003 | setup-crates-io-publish.py | 431 |
| L | GS003 | setup-crates-io-publish.py | 438 |
| L | GS003 | setup-crates-io-publish.py | 450 |
| L | GS003 | __main__.py | 35 |
| L | GS003 | __main__.py | 36 |
| L | GS003 | __main__.py | 37 |
| L | GS003 | __main__.py | 38 |
| L | GS003 | __main__.py | 39 |
| L | GS003 | __main__.py | 40 |
| L | GS003 | __main__.py | 41 |
| L | GS003 | __main__.py | 42 |
| L | GS003 | __main__.py | 43 |
| L | GS003 | __main__.py | 51 |
| L | GS003 | __main__.py | 54 |
| L | GS003 | __main__.py | 57 |
| L | GS003 | sync-python-version-constants.py | 103 |
| L | GS003 | sync-python-version-constants.py | 105 |
| L | GS003 | sync-python-version-constants.py | 107 |
| L | GS003 | update_schemastore.py | 95 |
| L | GS003 | build.rs | 40 |
| L | GS003 | uvw.rs | 42 |
| L | GS003 | uvw.rs | 97 |
| L | GS003 | uvx.rs | 43 |
| L | GS003 | uvx.rs | 100 |
| L | GS003 | diagnostics.rs | 117 |
| L | GS003 | settings.rs | 5157 |
| L | GS003 | lib.rs | 1326 |
| L | GS003 | build.rs | 23 |
| L | GS003 | build.rs | 41 |
| L | GS003 | build.rs | 54 |
| L | GS003 | build.rs | 73 |
| L | GS003 | build.rs | 74 |
| L | GS003 | build.rs | 79 |
| L | GS003 | build.rs | 85 |
| L | GS003 | build.rs | 91 |
| L | GS003 | options.rs | 24 |
| L | GS003 | options.rs | 201 |
| L | GS003 | options.rs | 275 |
| L | GS003 | options.rs | 401 |
| L | GS003 | generate_cli_reference.rs | 48 |
| L | GS003 | generate_cli_reference.rs | 53 |
| L | GS003 | generate_cli_reference.rs | 71 |
| L | GS003 | generate_cli_reference.rs | 73 |
| L | GS003 | generate_cli_reference.rs | 78 |
| L | GS003 | generate_env_vars_reference.rs | 29 |
| L | GS003 | generate_env_vars_reference.rs | 34 |
| L | GS003 | generate_env_vars_reference.rs | 54 |
| L | GS003 | generate_env_vars_reference.rs | 56 |
| L | GS003 | generate_env_vars_reference.rs | 61 |
| L | GS003 | generate_json_schema.rs | 43 |
| L | GS003 | generate_json_schema.rs | 48 |
| L | GS003 | generate_json_schema.rs | 66 |
| L | GS003 | generate_json_schema.rs | 68 |
| L | GS003 | generate_json_schema.rs | 73 |
| L | GS003 | generate_options_reference.rs | 51 |
| L | GS003 | generate_options_reference.rs | 56 |
| L | GS003 | generate_options_reference.rs | 76 |
| L | GS003 | generate_options_reference.rs | 78 |
| L | GS003 | generate_options_reference.rs | 83 |
| L | GS003 | generate_scenarios.rs | 80 |
| L | GS003 | generate_scenarios.rs | 95 |
| L | GS003 | generate_scenarios.rs | 97 |
| L | GS003 | generate_scenarios.rs | 102 |
| L | GS003 | generate_scenarios.rs | 218 |
| L | GS003 | generate_scenarios.rs | 281 |
| L | GS003 | generate_sysconfig_mappings.rs | 54 |
| L | GS003 | generate_sysconfig_mappings.rs | 59 |
| L | GS003 | generate_sysconfig_mappings.rs | 79 |
| L | GS003 | generate_sysconfig_mappings.rs | 81 |
| L | GS003 | generate_sysconfig_mappings.rs | 86 |
| L | GS003 | generate_sysconfig_mappings.rs | 101 |
| L | GS003 | list_packages.rs | 35 |
| L | GS003 | wheel_metadata.rs | 56 |
| L | GS003 | lib.rs | 324 |
| L | GS003 | link.rs | 1063 |
| L | GS003 | link.rs | 1089 |
| L | GS003 | link.rs | 1120 |
| L | GS003 | link.rs | 1160 |
| L | GS003 | link.rs | 1188 |
| L | GS003 | link.rs | 1210 |
| L | GS003 | link.rs | 1232 |
| L | GS003 | link.rs | 1271 |
| L | GS003 | link.rs | 1290 |
| L | GS003 | link.rs | 1981 |
| L | GS003 | path.rs | 13 |
| L | GS003 | main.rs | 61 |
| L | GS003 | lib.rs | 20 |
| L | GS003 | trusted_publishing.rs | 157 |
| L | GS003 | build.rs | 32 |
| L | GS003 | build.rs | 37 |
| L | GS003 | error.rs | 851 |
| L | GS003 | lib.rs | 2197 |
| L | GS003 | lib.rs | 2198 |
| L | GS003 | lib.rs | 2203 |
| L | GS003 | build.rs | 14 |
| L | GS003 | build.rs | 15 |
| L | GS003 | lib.rs | 664 |
| L | GS003 | lib.rs | 687 |
| L | GS003 | lib.rs | 752 |
| L | GS003 | lib.rs | 807 |
| L | GS003 | lib.rs | 56 |
| L | GS003 | lib.rs | 75 |
| H | ? | wheel.rs | 544 |
| H | ? | wheel.rs | 546 |
| H | ? | lib.rs | 1337 |
| H | ? | pyproject_mut.rs | 1960 |
| H | ? | pyproject_mut.rs | 1964 |
| H | ? | pyproject_mut.rs | 1965 |
| H | ? | pyproject_mut.rs | 1984 |
| H | ? | pyproject_mut.rs | 1989 |
| H | ? | pyproject_mut.rs | 1990 |
| H | ? | pyproject_mut.rs | 2007 |
| H | ? | pyproject_mut.rs | 2010 |
| H | ? | pyproject_mut.rs | 2011 |
| H | ? | pyproject_mut.rs | 2016 |
| H | ? | pyproject_mut.rs | 2017 |
| H | ? | pyproject_mut.rs | 2034 |
| H | ? | pyproject_mut.rs | 2037 |
| H | ? | pyproject_mut.rs | 2038 |
| H | ? | pyproject_mut.rs | 2043 |
| H | ? | pyproject_mut.rs | 2044 |
| H | ? | self_update.rs | 857 |
| H | ? | keyring.rs | 610 |
| H | ? | keyring.rs | 611 |
| H | ? | keyring.rs | 627 |
| H | ? | keyring.rs | 628 |
| H | ? | service.rs | 35 |
| H | ? | path.rs | 869 |
| H | ? | path.rs | 870 |
| H | ? | path.rs | 873 |
| H | ? | path.rs | 874 |
| H | ? | path.rs | 877 |
| H | ? | path.rs | 878 |
| H | ? | path.rs | 881 |
| H | ? | path.rs | 882 |
| H | ? | path.rs | 888 |
| H | ? | path.rs | 889 |
| H | ? | settings.rs | 417 |
| H | ? | tree.rs | 2784 |
| H | ? | tree.rs | 2801 |
| H | ? | vendor.rs | 61 |
| H | ? | vendor.rs | 67 |
| H | ? | version.rs | 3609 |
| H | ? | version.rs | 3610 |
| H | ? | version.rs | 4338 |
| H | ? | version.rs | 4415 |
| H | ? | version.rs | 4420 |
| H | ? | version.rs | 4423 |
| H | ? | version.rs | 4430 |
| H | ? | version.rs | 4435 |
| H | ? | version.rs | 4467 |
| H | ? | version.rs | 4472 |
| H | ? | version.rs | 4475 |
| H | ? | version.rs | 4482 |
| H | ? | version.rs | 4487 |
| H | ? | version.rs | 4519 |
| H | ? | version.rs | 4524 |
| H | ? | version.rs | 4527 |
| H | ? | version.rs | 4534 |
| H | ? | version.rs | 4539 |
| H | ? | version.rs | 4571 |
| H | ? | version.rs | 4576 |
| H | ? | version.rs | 4579 |
| H | ? | version.rs | 4586 |
| H | ? | version.rs | 4591 |
| H | ? | version.rs | 4623 |
| H | ? | version.rs | 4628 |
| H | ? | version.rs | 4631 |
| H | ? | version.rs | 4638 |
| H | ? | version.rs | 4643 |
| H | ? | version.rs | 4675 |
| H | ? | version.rs | 4680 |
| H | ? | version.rs | 4683 |
| H | ? | version.rs | 4690 |
| H | ? | version.rs | 4695 |
| H | ? | version.rs | 4718 |
| H | ? | version.rs | 4720 |
| H | ? | version.rs | 4723 |
| H | ? | version.rs | 4725 |
| H | ? | version.rs | 4727 |
| H | ? | version.rs | 4750 |
| H | ? | version.rs | 4752 |
| H | ? | version.rs | 4755 |
| H | ? | version.rs | 4759 |
| H | ? | version.rs | 4764 |
| H | ? | version.rs | 4788 |
| H | ? | version.rs | 4790 |
| H | ? | version.rs | 4793 |
| H | ? | version.rs | 4795 |
| H | ? | version.rs | 4797 |
| H | ? | version_specifier.rs | 2182 |
| H | ? | Dockerfile | 13 |
| H | ? | home-assistant.in | 1323 |
| H | ? | home-assistant.in | 1362 |
| H | ? | home-assistant.in | 1482 |
| H | ? | home-assistant.in | 1801 |
| H | ? | home-assistant.in | 1915 |
| H | ? | home-assistant.in | 2062 |
| H | ? | home-assistant.in | 2092 |
| H | ? | PKG-INFO | 1395 |
| H | ? | pyproject.toml | 145 |
| H | ? | pyproject.toml | 88 |
| H | ? | pyproject.toml | 91 |
| H | ? | pyproject.toml | 26 |
| H | ? | pyproject.toml | 141 |
| H | ? | pyproject.toml | 171 |
| C | ? | registry_client.rs | 1902 |
| C | ? | registry_client.rs | 1958 |
| C | ? | registry_client.rs | 2008 |
| C | ? | store.rs | 495 |
| C | ? | credentials.rs | 884 |
| C | ? | middleware.rs | 1063 |
| C | ? | middleware.rs | 1109 |
| C | ? | middleware.rs | 1223 |
| C | ? | middleware.rs | 1264 |
| C | ? | middleware.rs | 1312 |
| C | ? | middleware.rs | 1352 |
| C | ? | middleware.rs | 1395 |
| C | ? | middleware.rs | 1460 |
| C | ? | middleware.rs | 1525 |
| C | ? | middleware.rs | 1556 |
| C | ? | middleware.rs | 2246 |
| C | ? | middleware.rs | 2341 |
| C | ? | middleware.rs | 2437 |
| C | ? | middleware.rs | 2551 |
| C | ? | middleware.rs | 2583 |
| C | ? | middleware.rs | 2606 |
| C | ? | mock.rs | 246 |
| C | ? | secret_service.rs | 771 |
| C | ? | windows.rs | 751 |
| M | ? | registries-test.py | 154 |
| M | ? | transform_readme.py | 73 |
| M | ? | transform_readme.py | 79 |
| M | ? | resolver.py | 168 |
| M | ? | resolver.py | 186 |
| M | ? | resolver.py | 225 |
| M | ? | resolver.py | 248 |
| M | ? | resolver.py | 373 |
| M | ? | resolver.py | 385 |
| M | ? | resolver.py | 461 |
| M | ? | resolver.py | 471 |
| M | ? | resolver.py | 649 |
| M | ? | resolver.py | 657 |
| M | ? | resolver.py | 716 |
| M | ? | resolver.py | 722 |
| M | ? | resolver.py | 864 |
| M | ? | resolver.py | 883 |
| M | ? | resolver.py | 926 |
| M | ? | resolver.py | 951 |
| M | ? | resolver.py | 1046 |
| M | ? | resolver.py | 1054 |
| M | ? | resolver.py | 1121 |
| M | ? | resolver.py | 1127 |
| M | ? | resolver.py | 1269 |
| H | ? | uv.schema.json | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | mkdocs.yml | 0 |
| H | GS002 | credentials.rs | 0 |
| H | GS002 | credentials.rs | 0 |
| s | GS009 |  | 0 |
| L | GS014 | credentials.rs | 1 |
| L | GS014 | credentials.rs | 1 |
| M | ? | _musllinux.py | 50 |
| M | ? | check_embedded_python.py | 27 |
| M | ? | check_embedded_python.py | 39 |
| M | ? | check_embedded_python.py | 60 |
| M | ? | check_embedded_python.py | 69 |
| M | ? | check_embedded_python.py | 80 |
| M | ? | check_embedded_python.py | 89 |
| M | ? | registries-test.py | 80 |
| M | ? | registries-test.py | 100 |
| M | ? | registries-test.py | 224 |
| M | ? | registries-test.py | 351 |
| M | ? | setup-crates-io-publish.py | 60 |
| M | ? | setup-crates-io-publish.py | 174 |
| M | ? | __main__.py | 31 |
| M | ? | bump-workspace-crate-versions.py | 54 |
| M | ? | vendor-packaging.py | 44 |
| M | ? | vendor-packaging.py | 48 |
| M | ? | check_system_python.py | 23 |
| M | ? | check_system_python.py | 30 |
| M | ? | check_system_python.py | 37 |
| M | ? | check_system_python.py | 104 |
| M | ? | check_system_python.py | 129 |
| M | ? | check_system_python.py | 138 |
| M | ? | check_system_python.py | 147 |
| M | ? | check_system_python.py | 159 |
| M | ? | check_system_python.py | 172 |
| M | ? | check_system_python.py | 182 |
| M | ? | check_system_python.py | 191 |
| M | ? | check_system_python.py | 203 |
| M | ? | check_system_python.py | 217 |
| M | ? | check_system_python.py | 226 |
| M | ? | check_system_python.py | 237 |
| M | ? | check_system_python.py | 248 |
| M | ? | check_system_python.py | 257 |
| M | ? | check_system_python.py | 292 |
| M | ? | check_system_python.py | 300 |
| M | ? | check_system_python.py | 309 |
| M | ? | publish-crates.py | 45 |
| M | ? | publish-crates.py | 136 |
| M | ? | repair-sdist-cargo-lock.py | 57 |
| M | ? | repair-sdist-cargo-lock.py | 65 |
| M | ? | check_cache_compat.py | 35 |
| M | ? | check_cache_compat.py | 43 |
| M | ? | check_cache_compat.py | 49 |
| M | ? | check_cache_compat.py | 125 |
| M | ? | __main__.py | 42 |
| M | ? | post-edit-format.py | 18 |
| M | ? | post-edit-format.py | 30 |
| M | ? | post-edit-format.py | 42 |
| H | ? | lib.rs | 220 |
| H | ? | candidate_selector.rs | 336 |
| H | ? | candidate_selector.rs | 797 |
| H | ? | candidate_selector.rs | 799 |
| H | ? | exclude_newer.rs | 357 |
| H | ? | exclude_newer.rs | 367 |
| H | ? | exclude_newer.rs | 369 |
| H | ? | exclude_newer.rs | 378 |
| H | ? | exclude_newer.rs | 380 |
| H | ? | exclude_newer.rs | 386 |
| H | ? | exclude_newer.rs | 394 |
| H | ? | exclude_newer.rs | 395 |
| H | ? | exclude_newer.rs | 512 |
| H | ? | graph_ops.rs | 136 |
| H | ? | graph_ops.rs | 144 |
| H | ? | graph_ops.rs | 153 |
| H | ? | graph_ops.rs | 196 |
| H | ? | fork_urls.rs | 33 |
| H | ? | fork_urls.rs | 37 |
| H | ? | fork_urls.rs | 40 |
| H | ? | fork_urls.rs | 42 |
| H | ? | fork_urls.rs | 47 |
| H | ? | universal_marker.rs | 839 |
| H | ? | flat_index.rs | 46 |
| H | ? | flat_index.rs | 106 |
| H | ? | flat_index.rs | 137 |
| H | ? | flat_index.rs | 138 |
| H | ? | redirect.rs | 13 |
| H | ? | redirect.rs | 23 |
| H | ? | redirect.rs | 25 |
| H | ? | redirect.rs | 37 |
| H | ? | redirect.rs | 47 |
| H | ? | redirect.rs | 50 |
| H | ? | output.rs | 359 |
| H | ? | output.rs | 360 |
| H | ? | output.rs | 369 |
| H | ? | output.rs | 370 |
| H | ? | output.rs | 379 |
| H | ? | output.rs | 380 |
| H | ? | output.rs | 381 |
| H | ? | output.rs | 382 |
| H | ? | output.rs | 415 |
| H | ? | output.rs | 416 |
| H | ? | output.rs | 442 |
| H | ? | output.rs | 448 |
| H | ? | output.rs | 457 |
| H | ? | output.rs | 465 |
| H | ? | output.rs | 471 |
| H | ? | output.rs | 495 |
| H | ? | output.rs | 527 |
| H | ? | output.rs | 558 |
| H | ? | output.rs | 753 |
| H | ? | output.rs | 800 |
| H | ? | output.rs | 801 |
| H | ? | output.rs | 802 |
| H | ? | output.rs | 889 |
| H | ? | output.rs | 890 |
| H | ? | output.rs | 914 |
| H | ? | output.rs | 916 |
| H | ? | output.rs | 947 |
| H | ? | display.rs | 99 |
| H | ? | display.rs | 115 |
| H | ? | display.rs | 131 |
| H | ? | display.rs | 155 |
| H | ? | display.rs | 383 |
| H | ? | display.rs | 440 |
| H | ? | requirements_txt.rs | 119 |
| H | ? | requirements_txt.rs | 185 |
| H | ? | mod.rs | 410 |
| H | ? | mod.rs | 487 |
| H | ? | mod.rs | 490 |
| H | ? | mod.rs | 506 |
| H | ? | mod.rs | 524 |
| H | ? | mod.rs | 536 |
| H | ? | mod.rs | 554 |
| H | ? | mod.rs | 569 |
| H | ? | mod.rs | 612 |
| H | ? | mod.rs | 613 |
| H | ? | mod.rs | 625 |
| H | ? | mod.rs | 626 |
| H | ? | mod.rs | 627 |
| H | ? | mod.rs | 640 |
| H | ? | mod.rs | 641 |
| H | ? | mod.rs | 642 |
| H | ? | mod.rs | 655 |
| H | ? | mod.rs | 657 |
| H | ? | mod.rs | 668 |
| H | ? | mod.rs | 670 |
| H | ? | mod.rs | 697 |
| H | ? | mod.rs | 698 |
| H | ? | mod.rs | 709 |
| H | ? | mod.rs | 710 |
| H | ? | mod.rs | 722 |
| H | ? | mod.rs | 723 |
| H | ? | mod.rs | 736 |
| H | ? | mod.rs | 1730 |
| H | ? | mod.rs | 1838 |
| H | ? | mod.rs | 1892 |
| H | ? | mod.rs | 1967 |
| H | ? | mod.rs | 1982 |
| H | ? | mod.rs | 2101 |
| H | ? | mod.rs | 2119 |
| H | ? | mod.rs | 2188 |
| H | ? | mod.rs | 2345 |
| H | ? | mod.rs | 2399 |
| H | ? | mod.rs | 2406 |
| H | ? | mod.rs | 2410 |
| H | ? | mod.rs | 2431 |
| H | ? | mod.rs | 2432 |
| H | ? | mod.rs | 2530 |
| H | ? | mod.rs | 2537 |
| H | ? | mod.rs | 2541 |
| H | ? | mod.rs | 2655 |
| H | ? | mod.rs | 2661 |
| H | ? | mod.rs | 2666 |
| H | ? | mod.rs | 3053 |
| H | ? | mod.rs | 3191 |
| H | ? | mod.rs | 3209 |
| H | ? | mod.rs | 3346 |
| H | ? | mod.rs | 3367 |
| H | ? | mod.rs | 3379 |
| H | ? | mod.rs | 3382 |
| H | ? | mod.rs | 3387 |
| H | ? | mod.rs | 3396 |
| H | ? | mod.rs | 3411 |
| H | ? | mod.rs | 3418 |
| H | ? | mod.rs | 3419 |
| H | ? | mod.rs | 3424 |
| H | ? | mod.rs | 3429 |
| H | ? | mod.rs | 3437 |
| H | ? | mod.rs | 3444 |
| H | ? | mod.rs | 3451 |
| H | ? | mod.rs | 3471 |
| H | ? | mod.rs | 3482 |
| H | ? | mod.rs | 3486 |
| H | ? | mod.rs | 3490 |
| H | ? | mod.rs | 3494 |
| H | ? | mod.rs | 3499 |
| H | ? | mod.rs | 3505 |
| H | ? | mod.rs | 3545 |
| H | ? | mod.rs | 3555 |
| H | ? | mod.rs | 3556 |
| H | ? | mod.rs | 3567 |
| H | ? | mod.rs | 3579 |
| H | ? | mod.rs | 3591 |
| H | ? | mod.rs | 3608 |
| H | ? | mod.rs | 3617 |
| H | ? | mod.rs | 3626 |
| H | ? | mod.rs | 3627 |
| H | ? | mod.rs | 3632 |
| H | ? | mod.rs | 3635 |
| H | ? | mod.rs | 3642 |
| H | ? | mod.rs | 3643 |
| H | ? | mod.rs | 3647 |
| H | ? | mod.rs | 3650 |
| H | ? | mod.rs | 3660 |
| H | ? | mod.rs | 3669 |
| H | ? | mod.rs | 3670 |
| H | ? | mod.rs | 3674 |
| H | ? | mod.rs | 3676 |
| H | ? | mod.rs | 3695 |
| H | ? | mod.rs | 3696 |
| H | ? | mod.rs | 3701 |
| H | ? | mod.rs | 3705 |
| H | ? | mod.rs | 3713 |
| H | ? | mod.rs | 3718 |
| H | ? | mod.rs | 3728 |
| H | ? | mod.rs | 3729 |
| H | ? | mod.rs | 3751 |
| H | ? | mod.rs | 3767 |
| H | ? | mod.rs | 3768 |
| H | ? | mod.rs | 3776 |
| H | ? | mod.rs | 3780 |
| H | ? | mod.rs | 3788 |
| H | ? | mod.rs | 3804 |
| H | ? | mod.rs | 3805 |
| H | ? | mod.rs | 4057 |
| H | ? | mod.rs | 4061 |
| H | ? | mod.rs | 4063 |
| H | ? | mod.rs | 4075 |
| H | ? | mod.rs | 4126 |
| H | ? | mod.rs | 4184 |
| H | ? | mod.rs | 4188 |
| H | ? | mod.rs | 4189 |
| H | ? | mod.rs | 4202 |
| H | ? | mod.rs | 4269 |
| H | ? | mod.rs | 4271 |
| H | ? | mod.rs | 4324 |
| H | ? | mod.rs | 4328 |
| H | ? | mod.rs | 4334 |
| H | ? | mod.rs | 4342 |
| H | ? | mod.rs | 4468 |
| H | ? | mod.rs | 4546 |
| H | ? | mod.rs | 4571 |
| H | ? | mod.rs | 4590 |
| H | ? | mod.rs | 4594 |
| H | ? | mod.rs | 4800 |
| H | ? | mod.rs | 5208 |
| H | ? | mod.rs | 5226 |
| H | ? | mod.rs | 5244 |
| H | ? | mod.rs | 5351 |
| H | ? | mod.rs | 5546 |
| H | ? | mod.rs | 5577 |
| H | ? | mod.rs | 5585 |
| H | ? | mod.rs | 5590 |
| H | ? | mod.rs | 5598 |
| H | ? | mod.rs | 5603 |
| H | ? | mod.rs | 5613 |
| H | ? | mod.rs | 5619 |
| H | ? | mod.rs | 5632 |
| H | ? | mod.rs | 5642 |
| H | ? | mod.rs | 5659 |
| H | ? | mod.rs | 5682 |
| H | ? | mod.rs | 5692 |
| H | ? | mod.rs | 5828 |
| H | ? | mod.rs | 6152 |
| H | ? | mod.rs | 6163 |
| H | ? | mod.rs | 6171 |
| H | ? | mod.rs | 6172 |
| H | ? | mod.rs | 6196 |
| H | ? | mod.rs | 6207 |
| H | ? | mod.rs | 6215 |
| H | ? | mod.rs | 6216 |
| H | ? | mod.rs | 6322 |
| H | ? | mod.rs | 6323 |
| H | ? | mod.rs | 6456 |
| H | ? | mod.rs | 6480 |
| H | ? | mod.rs | 6496 |
| H | ? | mod.rs | 6500 |
| H | ? | tree.rs | 496 |
| H | ? | tree.rs | 524 |
| H | ? | tree.rs | 653 |
| H | ? | tree.rs | 800 |
| H | ? | tree.rs | 818 |
| H | ? | tree.rs | 884 |
| H | ? | tree.rs | 1027 |
| H | ? | tree.rs | 1094 |
| H | ? | tree.rs | 1101 |
| H | ? | tree.rs | 1103 |
| H | ? | tree.rs | 1117 |
| H | ? | tree.rs | 1119 |
| H | ? | tree.rs | 1120 |
| H | ? | tree.rs | 1121 |
| H | ? | tree.rs | 1123 |
| H | ? | tree.rs | 1129 |
| H | ? | tree.rs | 1130 |
| H | ? | tree.rs | 1135 |
| H | ? | tree.rs | 1141 |
| H | ? | tree.rs | 1142 |
| H | ? | tree.rs | 1144 |
| H | ? | tree.rs | 1186 |
| H | ? | tree.rs | 1220 |
| H | ? | tree.rs | 1222 |
| H | ? | tree.rs | 1236 |
| H | ? | tree.rs | 1297 |
| H | ? | tree.rs | 1310 |
| H | ? | tree.rs | 1364 |
| H | ? | mod.rs | 81 |
| H | ? | mod.rs | 84 |
| H | ? | mod.rs | 88 |
| H | ? | mod.rs | 105 |
| H | ? | mod.rs | 112 |
| H | ? | mod.rs | 133 |
| H | ? | mod.rs | 490 |
| H | ? | mod.rs | 494 |
| H | ? | mod.rs | 522 |
| H | ? | mod.rs | 544 |
| H | ? | metadata.rs | 172 |
| H | ? | metadata.rs | 370 |
| H | ? | metadata.rs | 374 |
| H | ? | metadata.rs | 467 |
| H | ? | metadata.rs | 471 |
| H | ? | metadata.rs | 527 |
| H | ? | metadata.rs | 537 |
| H | ? | metadata.rs | 568 |
| H | ? | metadata.rs | 588 |
| H | ? | metadata.rs | 637 |
| H | ? | metadata.rs | 656 |
| H | ? | metadata.rs | 752 |
| H | ? | metadata.rs | 753 |
| H | ? | metadata.rs | 754 |
| H | ? | metadata.rs | 980 |
| H | ? | metadata.rs | 1078 |
| H | ? | metadata.rs | 1094 |
| H | ? | metadata.rs | 1205 |
| H | ? | metadata.rs | 1210 |
| H | ? | metadata.rs | 1227 |
| H | ? | metadata.rs | 1228 |
| H | ? | metadata.rs | 1235 |
| H | ? | metadata.rs | 1236 |
| H | ? | metadata.rs | 1296 |
| H | ? | metadata.rs | 1312 |
| H | ? | metadata.rs | 1324 |
| H | ? | metadata.rs | 1336 |
| H | ? | metadata.rs | 1348 |
| H | ? | metadata.rs | 1371 |
| H | ? | metadata.rs | 1375 |
| H | ? | metadata.rs | 1383 |
| H | ? | metadata.rs | 1384 |
| H | ? | metadata.rs | 1388 |
| H | ? | metadata.rs | 1390 |
| H | ? | metadata.rs | 1395 |
| H | ? | metadata.rs | 1397 |
| H | ? | metadata.rs | 1398 |
| H | ? | metadata.rs | 1412 |
| H | ? | metadata.rs | 1424 |
| H | ? | pylock_toml.rs | 381 |
| H | ? | pylock_toml.rs | 412 |
| H | ? | pylock_toml.rs | 428 |
| H | ? | pylock_toml.rs | 433 |
| H | ? | pylock_toml.rs | 443 |
| H | ? | pylock_toml.rs | 450 |
| H | ? | pylock_toml.rs | 484 |
| H | ? | pylock_toml.rs | 494 |
| H | ? | pylock_toml.rs | 501 |
| H | ? | pylock_toml.rs | 505 |
| H | ? | pylock_toml.rs | 506 |
| H | ? | pylock_toml.rs | 516 |
| H | ? | pylock_toml.rs | 526 |
| H | ? | pylock_toml.rs | 532 |
| H | ? | pylock_toml.rs | 545 |
| H | ? | pylock_toml.rs | 552 |
| H | ? | pylock_toml.rs | 578 |
| H | ? | pylock_toml.rs | 588 |
| H | ? | pylock_toml.rs | 664 |
| H | ? | pylock_toml.rs | 680 |
| H | ? | pylock_toml.rs | 717 |
| H | ? | pylock_toml.rs | 764 |
| H | ? | pylock_toml.rs | 828 |
| H | ? | pylock_toml.rs | 834 |
| H | ? | pylock_toml.rs | 847 |
| H | ? | pylock_toml.rs | 869 |
| H | ? | pylock_toml.rs | 873 |
| H | ? | pylock_toml.rs | 884 |
| H | ? | pylock_toml.rs | 912 |
| H | ? | pylock_toml.rs | 934 |
| H | ? | pylock_toml.rs | 1066 |
| H | ? | pylock_toml.rs | 1068 |
| H | ? | pylock_toml.rs | 1076 |
| H | ? | pylock_toml.rs | 1077 |
| H | ? | pylock_toml.rs | 1078 |
| H | ? | pylock_toml.rs | 1093 |
| H | ? | pylock_toml.rs | 1097 |
| H | ? | pylock_toml.rs | 1100 |
| H | ? | pylock_toml.rs | 1105 |
| H | ? | pylock_toml.rs | 1109 |
| H | ? | pylock_toml.rs | 1112 |
| H | ? | pylock_toml.rs | 1116 |
| H | ? | pylock_toml.rs | 1120 |
| H | ? | pylock_toml.rs | 1125 |
| H | ? | pylock_toml.rs | 1128 |
| H | ? | pylock_toml.rs | 1146 |
| H | ? | pylock_toml.rs | 1166 |
| H | ? | pylock_toml.rs | 1215 |
| H | ? | pylock_toml.rs | 1229 |
| H | ? | pylock_toml.rs | 1232 |
| H | ? | pylock_toml.rs | 1235 |
| H | ? | pylock_toml.rs | 1237 |
| H | ? | pylock_toml.rs | 1240 |
| H | ? | pylock_toml.rs | 1246 |
| H | ? | pylock_toml.rs | 1393 |
| H | ? | pylock_toml.rs | 1398 |
| H | ? | pylock_toml.rs | 1414 |
| H | ? | pylock_toml.rs | 1421 |
| H | ? | pylock_toml.rs | 1426 |
| H | ? | pylock_toml.rs | 1447 |
| H | ? | pylock_toml.rs | 1451 |
| H | ? | pylock_toml.rs | 1460 |
| H | ? | pylock_toml.rs | 1468 |
| H | ? | pylock_toml.rs | 1501 |
| H | ? | pylock_toml.rs | 1517 |
| H | ? | pylock_toml.rs | 1522 |
| H | ? | pylock_toml.rs | 1529 |
| H | ? | pylock_toml.rs | 1536 |
| H | ? | pylock_toml.rs | 1547 |
| H | ? | pylock_toml.rs | 1548 |
| H | ? | pylock_toml.rs | 1552 |
| H | ? | pylock_toml.rs | 1554 |
| H | ? | pylock_toml.rs | 1568 |
| H | ? | pylock_toml.rs | 1574 |
| H | ? | pylock_toml.rs | 1578 |
| H | ? | pylock_toml.rs | 1608 |
| H | ? | pylock_toml.rs | 1612 |
| H | ? | pylock_toml.rs | 1621 |
| H | ? | pylock_toml.rs | 1629 |
| H | ? | pylock_toml.rs | 1639 |
| H | ? | pylock_toml.rs | 1662 |
| H | ? | pylock_toml.rs | 1683 |
| H | ? | pylock_toml.rs | 1694 |
| H | ? | pylock_toml.rs | 1702 |
| H | ? | pylock_toml.rs | 1703 |
| H | ? | pylock_toml.rs | 1708 |
| H | ? | pylock_toml.rs | 1709 |
| H | ? | pylock_toml.rs | 1710 |
| H | ? | pylock_toml.rs | 1712 |
| H | ? | pylock_toml.rs | 1717 |
| H | ? | pylock_toml.rs | 1729 |
| H | ? | pylock_toml.rs | 1737 |
| H | ? | pylock_toml.rs | 1742 |
| H | ? | cyclonedx_json.rs | 149 |
| H | ? | cyclonedx_json.rs | 341 |
| H | ? | cyclonedx_json.rs | 363 |
| H | ? | cyclonedx_json.rs | 370 |
| H | ? | cyclonedx_json.rs | 375 |
| H | ? | cyclonedx_json.rs | 424 |
| H | ? | cyclonedx_json.rs | 432 |
| H | ? | requirements_txt.rs | 92 |
| H | ? | requirements_txt.rs | 103 |
| H | ? | requirements_txt.rs | 104 |
| H | ? | requirements_txt.rs | 109 |
| H | ? | requirements_txt.rs | 110 |
| H | ? | requirements_txt.rs | 119 |
| H | ? | installable.rs | 95 |
| H | ? | installable.rs | 99 |
| H | ? | installable.rs | 369 |
| H | ? | installable.rs | 407 |
| H | ? | installable.rs | 410 |
| H | ? | installable.rs | 469 |
| H | ? | installable.rs | 472 |
| H | ? | installable.rs | 508 |
| H | ? | installable.rs | 563 |
| H | ? | installable.rs | 646 |
| H | ? | installable.rs | 647 |
| H | ? | installable.rs | 648 |
| H | ? | installable.rs | 649 |
| H | ? | installable.rs | 706 |
| H | ? | installable.rs | 769 |
| H | ? | installable.rs | 770 |
| H | ? | installable.rs | 827 |
| H | ? | installable.rs | 833 |
| H | ? | installable.rs | 890 |
| H | ? | installable.rs | 897 |
| H | ? | installable.rs | 1345 |
| H | ? | report.rs | 401 |
| H | ? | report.rs | 404 |
| H | ? | report.rs | 749 |
| H | ? | report.rs | 752 |
| H | ? | report.rs | 763 |
| H | ? | report.rs | 801 |
| H | ? | report.rs | 802 |
| H | ? | report.rs | 807 |
| H | ? | report.rs | 808 |
| H | ? | report.rs | 888 |
| H | ? | report.rs | 898 |
| H | ? | report.rs | 923 |
| H | ? | report.rs | 924 |
| H | ? | report.rs | 938 |
| H | ? | report.rs | 952 |
| H | ? | report.rs | 953 |
| H | ? | report.rs | 954 |
| H | ? | report.rs | 955 |
| H | ? | report.rs | 968 |
| H | ? | report.rs | 971 |
| H | ? | report.rs | 973 |
| H | ? | report.rs | 979 |
| H | ? | report.rs | 981 |
| H | ? | report.rs | 1010 |
| H | ? | report.rs | 1012 |
| H | ? | report.rs | 1043 |
| H | ? | report.rs | 1092 |
| H | ? | report.rs | 1114 |
| H | ? | report.rs | 1115 |
| H | ? | report.rs | 1141 |
| H | ? | report.rs | 1142 |
| H | ? | report.rs | 1167 |
| H | ? | report.rs | 1168 |
| H | ? | report.rs | 1200 |
| H | ? | report.rs | 1201 |
| H | ? | report.rs | 1206 |
| H | ? | report.rs | 1207 |
| H | ? | report.rs | 1212 |
| H | ? | report.rs | 1230 |
| H | ? | report.rs | 1231 |
| H | ? | report.rs | 1237 |
| H | ? | report.rs | 1238 |
| H | ? | report.rs | 1244 |
| H | ? | report.rs | 1245 |
| H | ? | report.rs | 1251 |
| H | ? | report.rs | 1252 |
| H | ? | report.rs | 1253 |
| H | ? | report.rs | 1254 |
| H | ? | report.rs | 1259 |
| H | ? | report.rs | 1260 |
| H | ? | report.rs | 1290 |
| H | ? | report.rs | 1291 |
| H | ? | report.rs | 1292 |
| H | ? | report.rs | 1293 |
| H | ? | report.rs | 1304 |
| H | ? | report.rs | 1309 |
| H | ? | report.rs | 1365 |
| H | ? | report.rs | 1366 |
| H | ? | report.rs | 1371 |
| H | ? | report.rs | 1372 |
| H | ? | report.rs | 1387 |
| H | ? | report.rs | 1388 |
| H | ? | report.rs | 1393 |
| H | ? | report.rs | 1394 |
| H | ? | report.rs | 1788 |
| H | ? | report.rs | 1795 |
| H | ? | report.rs | 1796 |
| H | ? | report.rs | 1830 |
| H | ? | report.rs | 1840 |
| H | ? | report.rs | 1842 |
| H | ? | report.rs | 1947 |
| H | ? | report.rs | 1968 |
| H | ? | report.rs | 1987 |
| H | ? | report.rs | 2057 |
| H | ? | report.rs | 2450 |
| H | ? | report.rs | 2462 |
| H | ? | report.rs | 2463 |
| H | ? | report.rs | 2496 |
| H | ? | report.rs | 2498 |
| H | ? | report.rs | 2501 |
| H | ? | report.rs | 2502 |
| H | ? | report.rs | 2511 |
| H | ? | report.rs | 2517 |
| H | ? | report.rs | 2761 |
| H | ? | report.rs | 2763 |
| H | ? | report.rs | 2765 |
| H | ? | report.rs | 2766 |
| H | ? | report.rs | 2769 |
| H | ? | report.rs | 2770 |
| H | ? | report.rs | 2771 |
| H | ? | report.rs | 2772 |
| H | ? | report.rs | 2793 |
| H | ? | report.rs | 2795 |
| H | ? | dependencies.rs | 48 |
| H | ? | dependencies.rs | 175 |
| H | ? | dependencies.rs | 188 |
| H | ? | dependencies.rs | 284 |
| H | ? | dependencies.rs | 305 |
| H | ? | dependencies.rs | 306 |
| H | ? | dependencies.rs | 317 |
| H | ? | dependencies.rs | 318 |
| H | ? | dependencies.rs | 329 |
| H | ? | dependencies.rs | 330 |
| H | ? | dependencies.rs | 341 |
| H | ? | dependencies.rs | 354 |
| H | ? | dependencies.rs | 368 |
| H | ? | dependencies.rs | 382 |
| H | ? | range.rs | 147 |
| H | ? | range.rs | 159 |
| H | ? | range.rs | 319 |
| H | ? | range.rs | 398 |
| H | ? | package.rs | 153 |
| H | ? | package.rs | 409 |
| H | ? | marker.rs | 22 |
| H | ? | upgrade.rs | 32 |
| H | ? | upgrade.rs | 47 |
| H | ? | upgrade.rs | 56 |
| H | ? | upgrade.rs | 67 |
| H | ? | version_map.rs | 641 |
| H | ? | version_map.rs | 656 |
| H | ? | version_map.rs | 670 |
| H | ? | version_map.rs | 671 |
| H | ? | version_map.rs | 674 |
| H | ? | version_map.rs | 715 |
| H | ? | version_map.rs | 761 |
| H | ? | python_requirement.rs | 25 |
| H | ? | python_requirement.rs | 57 |
| H | ? | python_requirement.rs | 85 |
| H | ? | python_requirement.rs | 106 |
| H | ? | python_requirement.rs | 107 |
| H | ? | python_requirement.rs | 121 |
| H | ? | python_requirement.rs | 122 |
| H | ? | python_requirement.rs | 127 |
| H | ? | python_requirement.rs | 128 |
| H | ? | error.rs | 65 |
| H | ? | error.rs | 699 |
| H | ? | error.rs | 1014 |
| H | ? | error.rs | 1091 |
| H | ? | error.rs | 1201 |
| H | ? | error.rs | 1204 |
| H | ? | error.rs | 1208 |
| H | ? | error.rs | 1209 |
| H | ? | error.rs | 1210 |
| H | ? | error.rs | 1218 |
| H | ? | error.rs | 1552 |
| H | ? | error.rs | 1602 |
| H | ? | error.rs | 1609 |
| H | ? | error.rs | 1680 |
| H | ? | yanks.rs | 37 |
| H | ? | yanks.rs | 39 |
| H | ? | yanks.rs | 46 |
| H | ? | yanks.rs | 48 |
| H | ? | provider.rs | 148 |
| H | ? | provider.rs | 150 |
| H | ? | provider.rs | 152 |
| H | ? | provider.rs | 214 |
| H | ? | provider.rs | 215 |
| H | ? | provider.rs | 216 |
| H | ? | provider.rs | 217 |
| H | ? | provider.rs | 218 |
| H | ? | provider.rs | 342 |
| H | ? | provider.rs | 357 |
| H | ? | mod.rs | 186 |
| H | ? | mod.rs | 232 |
| H | ? | mod.rs | 233 |
| H | ? | mod.rs | 234 |
| H | ? | mod.rs | 247 |
| H | ? | mod.rs | 248 |
| H | ? | mod.rs | 250 |
| H | ? | mod.rs | 252 |
| H | ? | mod.rs | 268 |
| H | ? | mod.rs | 288 |
| H | ? | mod.rs | 291 |
| H | ? | mod.rs | 333 |
| H | ? | mod.rs | 334 |
| H | ? | mod.rs | 336 |
| H | ? | mod.rs | 337 |
| H | ? | mod.rs | 338 |
| H | ? | mod.rs | 342 |
| H | ? | mod.rs | 343 |
| H | ? | mod.rs | 346 |
| H | ? | mod.rs | 375 |
| H | ? | mod.rs | 448 |
| H | ? | mod.rs | 449 |
| H | ? | mod.rs | 454 |
| H | ? | mod.rs | 528 |
| H | ? | mod.rs | 550 |
| H | ? | mod.rs | 573 |
| H | ? | mod.rs | 574 |
| H | ? | mod.rs | 584 |
| H | ? | mod.rs | 629 |
| H | ? | mod.rs | 660 |
| H | ? | mod.rs | 768 |
| H | ? | mod.rs | 769 |
| H | ? | mod.rs | 770 |
| H | ? | mod.rs | 774 |
| H | ? | mod.rs | 777 |
| H | ? | mod.rs | 913 |
| H | ? | mod.rs | 916 |
| H | ? | mod.rs | 973 |
| H | ? | mod.rs | 1034 |
| H | ? | mod.rs | 1038 |
| H | ? | mod.rs | 1047 |
| H | ? | mod.rs | 1049 |
| H | ? | mod.rs | 1053 |
| H | ? | mod.rs | 1054 |
| H | ? | mod.rs | 1102 |
| H | ? | mod.rs | 1104 |
| H | ? | mod.rs | 1105 |
| H | ? | mod.rs | 1106 |
| H | ? | mod.rs | 1140 |
| H | ? | mod.rs | 1154 |
| H | ? | mod.rs | 1159 |
| H | ? | mod.rs | 1189 |
| H | ? | mod.rs | 1204 |
| H | ? | mod.rs | 1250 |
| H | ? | mod.rs | 1264 |
| H | ? | mod.rs | 1272 |
| H | ? | mod.rs | 1274 |
| H | ? | mod.rs | 1311 |
| H | ? | mod.rs | 1324 |
| H | ? | mod.rs | 1341 |
| H | ? | mod.rs | 1343 |
| H | ? | mod.rs | 1349 |
| H | ? | mod.rs | 1373 |
| H | ? | mod.rs | 1381 |
| H | ? | mod.rs | 1388 |
| H | ? | mod.rs | 1394 |
| H | ? | mod.rs | 1400 |
| H | ? | mod.rs | 1431 |
| H | ? | mod.rs | 1434 |
| H | ? | mod.rs | 1477 |
| H | ? | mod.rs | 1520 |
| H | ? | mod.rs | 1575 |
| H | ? | mod.rs | 1622 |
| H | ? | mod.rs | 1623 |
| H | ? | mod.rs | 1690 |
| H | ? | mod.rs | 1746 |
| H | ? | mod.rs | 1748 |
| H | ? | mod.rs | 1751 |
| H | ? | mod.rs | 1753 |
| H | ? | mod.rs | 1781 |
| H | ? | mod.rs | 1782 |
| H | ? | mod.rs | 1790 |
| H | ? | mod.rs | 1814 |
| H | ? | mod.rs | 1823 |
| H | ? | mod.rs | 1923 |
| H | ? | mod.rs | 1943 |
| H | ? | mod.rs | 1966 |
| H | ? | mod.rs | 1969 |
| H | ? | mod.rs | 1977 |
| H | ? | mod.rs | 1979 |
| H | ? | mod.rs | 1989 |
| H | ? | mod.rs | 2047 |
| H | ? | mod.rs | 2052 |
| H | ? | mod.rs | 2075 |
| H | ? | mod.rs | 2080 |
| H | ? | mod.rs | 2101 |
| H | ? | mod.rs | 2103 |
| H | ? | mod.rs | 2106 |
| H | ? | mod.rs | 2186 |
| H | ? | mod.rs | 2207 |
| H | ? | mod.rs | 2208 |
| H | ? | mod.rs | 2209 |
| H | ? | mod.rs | 2210 |
| H | ? | mod.rs | 2211 |
| H | ? | mod.rs | 2239 |
| H | ? | mod.rs | 2241 |
| H | ? | mod.rs | 2242 |
| H | ? | mod.rs | 2243 |
| H | ? | mod.rs | 2289 |
| H | ? | mod.rs | 2392 |
| H | ? | mod.rs | 2393 |
| H | ? | mod.rs | 2394 |
| H | ? | mod.rs | 2395 |
| H | ? | mod.rs | 2396 |
| H | ? | mod.rs | 2429 |
| H | ? | mod.rs | 2430 |
| H | ? | mod.rs | 2431 |
| H | ? | mod.rs | 2432 |
| H | ? | mod.rs | 2433 |
| H | ? | mod.rs | 2578 |
| H | ? | mod.rs | 2607 |
| H | ? | mod.rs | 2608 |
| H | ? | mod.rs | 2623 |
| H | ? | mod.rs | 2624 |
| H | ? | mod.rs | 2648 |
| H | ? | mod.rs | 2655 |
| H | ? | mod.rs | 2662 |
| H | ? | mod.rs | 2708 |
| H | ? | mod.rs | 2714 |
| H | ? | mod.rs | 2718 |
| H | ? | mod.rs | 2777 |
| H | ? | mod.rs | 2789 |
| H | ? | mod.rs | 2798 |
| H | ? | mod.rs | 2831 |
| H | ? | mod.rs | 2844 |
| H | ? | mod.rs | 2846 |
| H | ? | mod.rs | 2872 |
| H | ? | mod.rs | 2881 |
| H | ? | mod.rs | 2884 |
| H | ? | mod.rs | 2909 |
| H | ? | mod.rs | 2932 |
| H | ? | mod.rs | 2939 |
| H | ? | mod.rs | 2952 |
| H | ? | mod.rs | 2956 |
| H | ? | mod.rs | 2957 |
| H | ? | mod.rs | 2958 |
| H | ? | mod.rs | 2959 |
| H | ? | mod.rs | 2966 |
| H | ? | mod.rs | 2967 |
| H | ? | mod.rs | 2968 |
| H | ? | mod.rs | 3240 |
| H | ? | mod.rs | 3241 |
| H | ? | mod.rs | 3245 |
| H | ? | mod.rs | 3251 |
| H | ? | mod.rs | 3271 |
| H | ? | mod.rs | 3368 |
| H | ? | mod.rs | 3382 |
| H | ? | mod.rs | 3507 |
| H | ? | mod.rs | 3512 |
| H | ? | mod.rs | 3513 |
| H | ? | mod.rs | 3516 |
| H | ? | mod.rs | 3517 |
| H | ? | mod.rs | 3539 |
| H | ? | mod.rs | 3544 |
| H | ? | mod.rs | 3545 |
| H | ? | mod.rs | 3571 |
| H | ? | mod.rs | 3576 |
| H | ? | mod.rs | 3577 |
| H | ? | mod.rs | 3580 |
| H | ? | mod.rs | 3589 |
| H | ? | mod.rs | 3594 |
| H | ? | mod.rs | 3595 |
| H | ? | mod.rs | 3621 |
| H | ? | mod.rs | 3626 |
| H | ? | mod.rs | 3627 |
| H | ? | mod.rs | 3631 |
| H | ? | mod.rs | 3655 |
| H | ? | mod.rs | 3656 |
| H | ? | mod.rs | 3657 |
| H | ? | mod.rs | 3779 |
| H | ? | mod.rs | 3866 |
| H | ? | mod.rs | 3933 |
| H | ? | mod.rs | 3962 |
| H | ? | mod.rs | 3981 |
| H | ? | mod.rs | 4002 |
| H | ? | mod.rs | 4008 |
| H | ? | mod.rs | 4019 |
| H | ? | mod.rs | 4026 |
| H | ? | mod.rs | 4066 |
| H | ? | mod.rs | 4123 |
| H | ? | mod.rs | 4135 |
| H | ? | mod.rs | 4347 |
| H | ? | urls.rs | 52 |
| H | ? | urls.rs | 145 |
| H | ? | urls.rs | 158 |
| H | ? | urls.rs | 159 |
| H | ? | urls.rs | 163 |
| H | ? | urls.rs | 165 |
| H | ? | urls.rs | 178 |
| H | ? | indexes.rs | 38 |
| H | ? | fork_map.rs | 54 |
| H | ? | fork_map.rs | 63 |
| H | ? | fork_map.rs | 92 |
| H | ? | fork_map.rs | 146 |
| H | ? | fork_map.rs | 148 |
| H | ? | batch_prefetch.rs | 113 |
| H | ? | batch_prefetch.rs | 124 |
| H | ? | batch_prefetch.rs | 125 |
| H | ? | batch_prefetch.rs | 128 |
| H | ? | batch_prefetch.rs | 157 |
| H | ? | batch_prefetch.rs | 159 |
| H | ? | batch_prefetch.rs | 235 |
| H | ? | batch_prefetch.rs | 239 |
| H | ? | batch_prefetch.rs | 270 |
| H | ? | derivation.rs | 59 |
| H | ? | derivation.rs | 62 |
| H | ? | derivation.rs | 63 |
| H | ? | availability.rs | 51 |
| H | ? | availability.rs | 52 |
| H | ? | availability.rs | 53 |
| H | ? | availability.rs | 54 |
| H | ? | availability.rs | 195 |
| H | ? | availability.rs | 277 |
| H | ? | availability.rs | 280 |
| H | ? | availability.rs | 283 |
| H | ? | environment.rs | 313 |
| H | ? | environment.rs | 314 |
| H | ? | environment.rs | 382 |
| H | ? | environment.rs | 623 |
| H | ? | environment.rs | 624 |
| H | ? | environment.rs | 765 |
| H | ? | preferences.rs | 66 |
| H | ? | preferences.rs | 91 |
| H | ? | preferences.rs | 92 |
| H | ? | preferences.rs | 107 |
| H | ? | preferences.rs | 108 |
| H | ? | preferences.rs | 114 |
| H | ? | preferences.rs | 129 |
| H | ? | preferences.rs | 130 |
| H | ? | preferences.rs | 275 |
| H | ? | preferences.rs | 277 |
| H | ? | preferences.rs | 279 |
| H | ? | preferences.rs | 280 |
| H | ? | preferences.rs | 402 |
| H | ? | pins.rs | 33 |
| H | ? | pins.rs | 47 |
| H | ? | pins.rs | 58 |
| H | ? | fork_indexes.rs | 25 |
| H | ? | fork_indexes.rs | 27 |
| H | ? | fork_indexes.rs | 30 |
| H | ? | fork_indexes.rs | 32 |
| H | ? | control.rs | 333 |
| H | ? | mod.rs | 208 |
| H | ? | mod.rs | 985 |
| H | ? | mod.rs | 987 |
| H | ? | flat_index.rs | 170 |
| H | ? | flat_index.rs | 203 |
| H | ? | flat_index.rs | 208 |
| H | ? | flat_index.rs | 214 |
| H | ? | flat_index.rs | 217 |
| H | ? | flat_index.rs | 224 |
| H | ? | flat_index.rs | 268 |
| H | ? | flat_index.rs | 346 |
| H | ? | cached_client.rs | 252 |
| H | ? | cached_client.rs | 258 |
| H | ? | cached_client.rs | 260 |
| H | ? | cached_client.rs | 277 |
| H | ? | cached_client.rs | 303 |
| H | ? | cached_client.rs | 322 |
| H | ? | cached_client.rs | 478 |
| H | ? | cached_client.rs | 519 |
| H | ? | cached_client.rs | 528 |
| H | ? | cached_client.rs | 540 |
| H | ? | cached_client.rs | 551 |
| H | ? | cached_client.rs | 584 |
| H | ? | cached_client.rs | 589 |
| H | ? | cached_client.rs | 601 |
| H | ? | cached_client.rs | 664 |
| H | ? | cached_client.rs | 671 |
| H | ? | cached_client.rs | 702 |
| H | ? | cached_client.rs | 709 |
| H | ? | registry_client.rs | 157 |
| H | ? | registry_client.rs | 424 |
| H | ? | registry_client.rs | 463 |
| H | ? | registry_client.rs | 485 |
| H | ? | registry_client.rs | 512 |
| H | ? | registry_client.rs | 514 |
| H | ? | registry_client.rs | 611 |
| H | ? | registry_client.rs | 616 |
| H | ? | registry_client.rs | 622 |
| H | ? | registry_client.rs | 627 |
| H | ? | registry_client.rs | 629 |
| H | ? | registry_client.rs | 634 |
| H | ? | registry_client.rs | 643 |
| H | ? | registry_client.rs | 649 |
| H | ? | registry_client.rs | 662 |
| H | ? | registry_client.rs | 668 |
| H | ? | registry_client.rs | 681 |
| H | ? | registry_client.rs | 688 |
| H | ? | registry_client.rs | 700 |
| H | ? | registry_client.rs | 734 |
| H | ? | registry_client.rs | 740 |
| H | ? | registry_client.rs | 760 |
| H | ? | registry_client.rs | 762 |
| H | ? | registry_client.rs | 819 |
| H | ? | registry_client.rs | 824 |
| H | ? | registry_client.rs | 826 |
| H | ? | registry_client.rs | 831 |
| H | ? | registry_client.rs | 840 |
| H | ? | registry_client.rs | 846 |
| H | ? | registry_client.rs | 852 |
| H | ? | registry_client.rs | 858 |
| H | ? | registry_client.rs | 864 |
| H | ? | registry_client.rs | 870 |
| H | ? | registry_client.rs | 876 |
| H | ? | registry_client.rs | 891 |
| H | ? | registry_client.rs | 896 |
| H | ? | registry_client.rs | 919 |
| H | ? | registry_client.rs | 964 |
| H | ? | registry_client.rs | 983 |
| H | ? | registry_client.rs | 1017 |
| H | ? | registry_client.rs | 1062 |
| H | ? | registry_client.rs | 1073 |
| H | ? | registry_client.rs | 1095 |
| H | ? | registry_client.rs | 1127 |
| H | ? | registry_client.rs | 1134 |
| H | ? | registry_client.rs | 1142 |
| H | ? | registry_client.rs | 1145 |
| H | ? | registry_client.rs | 1206 |
| H | ? | registry_client.rs | 1213 |
| H | ? | registry_client.rs | 1219 |
| H | ? | registry_client.rs | 1238 |
| H | ? | registry_client.rs | 1240 |
| H | ? | registry_client.rs | 1241 |
| H | ? | registry_client.rs | 1244 |
| H | ? | registry_client.rs | 1249 |
| H | ? | registry_client.rs | 1264 |
| H | ? | registry_client.rs | 1280 |
| H | ? | registry_client.rs | 1292 |
| H | ? | registry_client.rs | 1302 |
| H | ? | registry_client.rs | 1374 |
| H | ? | registry_client.rs | 1457 |
| H | ? | registry_client.rs | 1521 |
| H | ? | registry_client.rs | 1589 |
| H | ? | registry_client.rs | 1609 |
| H | ? | registry_client.rs | 1610 |
| H | ? | registry_client.rs | 1638 |
| H | ? | registry_client.rs | 1937 |
| H | ? | registry_client.rs | 1987 |
| H | ? | registry_client.rs | 2037 |
| H | ? | base_client.rs | 401 |
| H | ? | base_client.rs | 409 |
| H | ? | base_client.rs | 414 |
| H | ? | base_client.rs | 421 |
| H | ? | base_client.rs | 430 |
| H | ? | base_client.rs | 439 |
| H | ? | base_client.rs | 444 |
| H | ? | base_client.rs | 451 |
| H | ? | base_client.rs | 456 |
| H | ? | base_client.rs | 457 |
| H | ? | base_client.rs | 460 |
| H | ? | base_client.rs | 474 |
| H | ? | base_client.rs | 494 |
| H | ? | base_client.rs | 566 |
| H | ? | base_client.rs | 577 |
| H | ? | base_client.rs | 594 |
| H | ? | base_client.rs | 609 |
| H | ? | base_client.rs | 631 |
| H | ? | base_client.rs | 639 |
| H | ? | base_client.rs | 641 |
| H | ? | base_client.rs | 651 |
| H | ? | base_client.rs | 653 |
| H | ? | base_client.rs | 738 |
| H | ? | base_client.rs | 888 |
| H | ? | base_client.rs | 1023 |
| H | ? | base_client.rs | 1129 |
| H | ? | base_client.rs | 1135 |
| H | ? | retry.rs | 148 |
| H | ? | middleware.rs | 46 |
| H | ? | tls.rs | 108 |
| H | ? | tls.rs | 259 |
| H | ? | tls.rs | 351 |
| H | ? | tls.rs | 381 |
| H | ? | html.rs | 25 |
| H | ? | html.rs | 32 |
| H | ? | html.rs | 108 |
| H | ? | remote_metadata.rs | 67 |
| H | ? | remote_metadata.rs | 103 |
| H | ? | remote_metadata.rs | 106 |
| H | ? | source_dist.rs | 59 |
| H | ? | source_dist.rs | 69 |
| H | ? | source_dist.rs | 79 |
| H | ? | source_dist.rs | 89 |
| H | ? | wheel.rs | 258 |
| H | ? | tags.rs | 205 |
| H | ? | tags.rs | 224 |
| H | ? | tags.rs | 237 |
| H | ? | tags.rs | 245 |
| H | ? | tags.rs | 255 |
| H | ? | tags.rs | 270 |
| H | ? | tags.rs | 282 |
| H | ? | tags.rs | 373 |
| H | ? | tags.rs | 374 |
| H | ? | site_packages.rs | 133 |
| H | ? | site_packages.rs | 139 |
| H | ? | site_packages.rs | 148 |
| H | ? | site_packages.rs | 223 |
| H | ? | site_packages.rs | 245 |
| H | ? | site_packages.rs | 257 |
| H | ? | site_packages.rs | 258 |
| H | ? | site_packages.rs | 259 |
| H | ? | site_packages.rs | 270 |
| H | ? | site_packages.rs | 277 |
| H | ? | site_packages.rs | 294 |
| H | ? | site_packages.rs | 295 |
| H | ? | site_packages.rs | 308 |
| H | ? | site_packages.rs | 309 |
| H | ? | site_packages.rs | 310 |
| H | ? | site_packages.rs | 361 |
| H | ? | site_packages.rs | 363 |
| H | ? | site_packages.rs | 366 |
| H | ? | site_packages.rs | 367 |
| H | ? | site_packages.rs | 401 |
| H | ? | site_packages.rs | 403 |
| H | ? | site_packages.rs | 406 |
| H | ? | site_packages.rs | 407 |
| H | ? | site_packages.rs | 487 |
| H | ? | site_packages.rs | 573 |
| H | ? | site_packages.rs | 761 |
| H | ? | preparer.rs | 59 |
| H | ? | preparer.rs | 75 |
| H | ? | preparer.rs | 121 |
| H | ? | preparer.rs | 129 |
| H | ? | preparer.rs | 151 |
| H | ? | preparer.rs | 152 |
| H | ? | preparer.rs | 158 |
| H | ? | preparer.rs | 161 |
| H | ? | preparer.rs | 162 |
| H | ? | preparer.rs | 167 |
| H | ? | preparer.rs | 178 |
| H | ? | preparer.rs | 195 |
| H | ? | preparer.rs | 275 |
| H | ? | satisfies.rs | 134 |
| H | ? | satisfies.rs | 458 |
| H | ? | compile.rs | 111 |
| H | ? | compile.rs | 519 |
| H | ? | plan.rs | 376 |
| H | ? | plan.rs | 395 |
| H | ? | plan.rs | 404 |
| H | ? | plan.rs | 444 |
| H | ? | plan.rs | 447 |
| H | ? | plan.rs | 513 |
| H | ? | plan.rs | 516 |
| H | ? | plan.rs | 577 |
| H | ? | plan.rs | 580 |
| H | ? | plan.rs | 598 |
| H | ? | plan.rs | 610 |
| H | ? | plan.rs | 638 |
| H | ? | plan.rs | 659 |
| H | ? | plan.rs | 686 |
| H | ? | plan.rs | 720 |
| H | ? | plan.rs | 746 |
| H | ? | uninstall.rs | 10 |
| H | ? | uninstall.rs | 11 |
| H | ? | source_dist.rs | 38 |
| H | ? | source_dist.rs | 39 |
| H | ? | source_dist.rs | 53 |
| H | ? | source_dist.rs | 66 |
| H | ? | source_dist.rs | 67 |
| H | ? | source_dist.rs | 213 |
| H | ? | source_dist.rs | 214 |
| H | ? | source_dist.rs | 266 |
| H | ? | source_dist.rs | 481 |
| H | ? | source_dist.rs | 516 |
| H | ? | source_dist.rs | 530 |
| H | ? | source_dist.rs | 537 |
| H | ? | wheel.rs | 57 |
| H | ? | wheel.rs | 58 |
| H | ? | wheel.rs | 88 |
| H | ? | wheel.rs | 105 |
| H | ? | wheel.rs | 106 |
| H | ? | wheel.rs | 268 |
| H | ? | wheel.rs | 269 |
| H | ? | wheel.rs | 324 |
| H | ? | wheel.rs | 397 |
| H | ? | wheel.rs | 416 |
| H | ? | wheel.rs | 417 |
| H | ? | metadata.rs | 279 |
| H | ? | metadata.rs | 304 |
| H | ? | metadata.rs | 323 |
| H | ? | metadata.rs | 439 |
| H | ? | metadata.rs | 455 |
| H | ? | metadata.rs | 468 |
| H | ? | metadata.rs | 474 |
| H | ? | metadata.rs | 483 |
| H | ? | metadata.rs | 489 |
| H | ? | metadata.rs | 516 |
| H | ? | metadata.rs | 546 |
| H | ? | metadata.rs | 576 |
| H | ? | metadata.rs | 600 |
| H | ? | metadata.rs | 624 |
| H | ? | metadata.rs | 653 |
| H | ? | metadata.rs | 662 |
| H | ? | metadata.rs | 712 |
| H | ? | metadata.rs | 737 |
| H | ? | metadata.rs | 816 |
| H | ? | metadata.rs | 828 |
| H | ? | metadata.rs | 830 |
| H | ? | metadata.rs | 841 |
| H | ? | metadata.rs | 924 |
| H | ? | metadata.rs | 1184 |
| H | ? | metadata.rs | 1226 |
| H | ? | overrides.rs | 122 |
| H | ? | overrides.rs | 144 |
| H | ? | overrides.rs | 153 |
| H | ? | overrides.rs | 154 |
| H | ? | overrides.rs | 164 |
| H | ? | overrides.rs | 165 |
| H | ? | overrides.rs | 170 |
| H | ? | overrides.rs | 185 |
| H | ? | overrides.rs | 304 |
| H | ? | overrides.rs | 359 |
| H | ? | overrides.rs | 363 |
| H | ? | package_options.rs | 178 |
| H | ? | package_options.rs | 185 |
| H | ? | package_options.rs | 199 |
| H | ? | package_options.rs | 278 |
| H | ? | constraints.rs | 27 |
| H | ? | constraints.rs | 77 |
| H | ? | dependency_groups.rs | 42 |
| H | ? | dependency_groups.rs | 46 |
| H | ? | dependency_groups.rs | 47 |
| H | ? | dependency_groups.rs | 48 |
| H | ? | dependency_groups.rs | 156 |
| H | ? | dependency_groups.rs | 161 |
| H | ? | extras.rs | 41 |
| H | ? | extras.rs | 116 |
| H | ? | proxy_url.rs | 173 |
| H | ? | proxy_url.rs | 190 |
| H | ? | libc.rs | 232 |
| H | ? | libc.rs | 237 |
| H | ? | libc.rs | 363 |
| H | ? | lib.rs | 556 |
| H | ? | lib.rs | 619 |
| H | ? | lib.rs | 672 |
| H | ? | lib.rs | 794 |
| H | ? | lib.rs | 798 |
| H | ? | lib.rs | 809 |
| H | ? | lib.rs | 835 |
| H | ? | lib.rs | 1216 |
| H | ? | lib.rs | 1219 |
| H | ? | lib.rs | 1255 |
| H | ? | lib.rs | 1357 |
| H | ? | workspace.rs | 99 |
| H | ? | workspace.rs | 102 |
| H | ? | workspace.rs | 331 |
| H | ? | workspace.rs | 352 |
| H | ? | workspace.rs | 379 |
| H | ? | workspace.rs | 380 |
| H | ? | workspace.rs | 381 |
| H | ? | workspace.rs | 400 |
| H | ? | workspace.rs | 402 |
| H | ? | workspace.rs | 426 |
| H | ? | workspace.rs | 434 |
| H | ? | workspace.rs | 443 |
| H | ? | workspace.rs | 457 |
| H | ? | workspace.rs | 489 |
| H | ? | workspace.rs | 494 |
| H | ? | workspace.rs | 548 |
| H | ? | workspace.rs | 557 |
| H | ? | workspace.rs | 570 |
| H | ? | workspace.rs | 631 |
| H | ? | workspace.rs | 637 |
| H | ? | workspace.rs | 673 |
| H | ? | workspace.rs | 687 |
| H | ? | workspace.rs | 693 |
| H | ? | workspace.rs | 700 |
| H | ? | workspace.rs | 766 |
| H | ? | workspace.rs | 837 |
| H | ? | workspace.rs | 851 |
| H | ? | workspace.rs | 865 |
| H | ? | workspace.rs | 879 |
| H | ? | workspace.rs | 1063 |
| H | ? | workspace.rs | 1068 |
| H | ? | workspace.rs | 1076 |
| H | ? | workspace.rs | 1150 |
| H | ? | workspace.rs | 1152 |
| H | ? | workspace.rs | 1154 |
| H | ? | workspace.rs | 1155 |
| H | ? | workspace.rs | 1156 |
| H | ? | workspace.rs | 1162 |
| H | ? | workspace.rs | 1172 |
| H | ? | workspace.rs | 1175 |
| H | ? | workspace.rs | 1186 |
| H | ? | workspace.rs | 1191 |
| H | ? | workspace.rs | 1293 |
| H | ? | workspace.rs | 1319 |
| H | ? | workspace.rs | 1331 |
| H | ? | workspace.rs | 1333 |
| H | ? | workspace.rs | 1340 |
| H | ? | workspace.rs | 1359 |
| H | ? | workspace.rs | 1507 |
| H | ? | workspace.rs | 1563 |
| H | ? | workspace.rs | 1568 |
| H | ? | workspace.rs | 1601 |
| H | ? | workspace.rs | 1604 |
| H | ? | workspace.rs | 1669 |
| H | ? | workspace.rs | 1699 |
| H | ? | workspace.rs | 1700 |
| H | ? | workspace.rs | 1712 |
| H | ? | workspace.rs | 1713 |
| H | ? | workspace.rs | 1723 |
| H | ? | workspace.rs | 1741 |
| H | ? | workspace.rs | 1745 |
| H | ? | workspace.rs | 1749 |
| H | ? | workspace.rs | 1759 |
| H | ? | workspace.rs | 1771 |
| H | ? | workspace.rs | 1780 |
| H | ? | workspace.rs | 1785 |
| H | ? | workspace.rs | 1844 |
| H | ? | workspace.rs | 1871 |
| H | ? | workspace.rs | 2047 |
| H | ? | workspace.rs | 2051 |
| H | ? | workspace.rs | 2060 |
| H | ? | workspace.rs | 2084 |
| H | ? | workspace.rs | 2087 |
| H | ? | workspace.rs | 2088 |
| H | ? | workspace.rs | 2096 |
| H | ? | workspace.rs | 2104 |
| H | ? | workspace.rs | 2107 |
| H | ? | workspace.rs | 2116 |
| H | ? | workspace.rs | 2132 |
| H | ? | workspace.rs | 2136 |
| H | ? | workspace.rs | 2191 |
| H | ? | workspace.rs | 2192 |
| H | ? | workspace.rs | 2193 |
| H | ? | workspace.rs | 2195 |
| H | ? | workspace.rs | 2293 |
| H | ? | dependency_groups.rs | 80 |
| H | ? | dependency_groups.rs | 83 |
| H | ? | dependency_groups.rs | 110 |
| H | ? | dependency_groups.rs | 111 |
| H | ? | dependency_groups.rs | 137 |
| H | ? | dependency_groups.rs | 138 |
| H | ? | dependency_groups.rs | 152 |
| H | ? | dependency_groups.rs | 159 |
| H | ? | dependency_groups.rs | 160 |
| H | ? | dependency_groups.rs | 175 |
| H | ? | dependency_groups.rs | 183 |
| H | ? | dependency_groups.rs | 191 |
| H | ? | dependency_groups.rs | 208 |
| H | ? | pyproject_mut.rs | 43 |
| H | ? | pyproject_mut.rs | 401 |
| H | ? | pyproject_mut.rs | 509 |
| H | ? | pyproject_mut.rs | 512 |
| H | ? | pyproject_mut.rs | 531 |
| H | ? | pyproject_mut.rs | 534 |
| H | ? | pyproject_mut.rs | 550 |
| H | ? | pyproject_mut.rs | 553 |
| H | ? | pyproject_mut.rs | 572 |
| H | ? | pyproject_mut.rs | 575 |
| H | ? | pyproject_mut.rs | 1305 |
| H | ? | pyproject_mut.rs | 1451 |
| H | ? | pyproject_mut.rs | 1477 |
| H | ? | pyproject_mut.rs | 1491 |
| H | ? | pyproject_mut.rs | 1497 |
| H | ? | pyproject_mut.rs | 1584 |
| H | ? | pyproject_mut.rs | 1611 |
| H | ? | pyproject.rs | 1687 |
| H | ? | pyproject.rs | 1688 |
| H | ? | pyproject.rs | 1694 |
| H | ? | pyproject.rs | 1695 |
| H | ? | pyproject.rs | 1696 |
| H | ? | pyproject.rs | 1822 |
| H | ? | pyproject.rs | 1835 |
| H | ? | pyproject.rs | 1861 |
| H | ? | pyproject.rs | 1874 |
| H | ? | parsed_url.rs | 340 |
| H | ? | parsed_url.rs | 494 |
| H | ? | parsed_url.rs | 549 |
| H | ? | parsed_url.rs | 564 |
| H | ? | parsed_url.rs | 581 |
| H | ? | parsed_url.rs | 664 |
| H | ? | parsed_url.rs | 669 |
| H | ? | parsed_url.rs | 673 |
| H | ? | parsed_url.rs | 679 |
| H | ? | parsed_url.rs | 686 |
| H | ? | parsed_url.rs | 693 |
| H | ? | parsed_url.rs | 706 |
| H | ? | parsed_url.rs | 718 |
| H | ? | direct_url.rs | 139 |
| H | ? | requires_dist.rs | 78 |
| H | ? | metadata_resolver.rs | 248 |
| H | ? | module_name.rs | 66 |
| H | ? | simple_json.rs | 73 |
| H | ? | simple_json.rs | 80 |
| H | ? | conflicts.rs | 106 |
| H | ? | conflicts.rs | 115 |
| H | ? | conflicts.rs | 117 |
| H | ? | conflicts.rs | 120 |
| H | ? | conflicts.rs | 130 |
| H | ? | conflicts.rs | 131 |
| H | ? | conflicts.rs | 164 |
| H | ? | conflicts.rs | 166 |
| H | ? | conflicts.rs | 168 |
| H | ? | conflicts.rs | 170 |
| H | ? | conflicts.rs | 192 |
| H | ? | conflicts.rs | 251 |
| H | ? | conflicts.rs | 381 |
| H | ? | conflicts.rs | 468 |
| H | ? | conflicts.rs | 469 |
| H | ? | conflicts.rs | 585 |
| H | ? | conflicts.rs | 588 |
| H | ? | conflicts.rs | 703 |
| H | ? | conflicts.rs | 708 |
| H | ? | conflicts.rs | 709 |
| H | ? | conflicts.rs | 713 |
| H | ? | conflicts.rs | 715 |
| H | ? | conflicts.rs | 724 |
| H | ? | conflicts.rs | 725 |
| H | ? | conflicts.rs | 726 |
| H | ? | lib.rs | 262 |
| H | ? | lib.rs | 303 |
| H | ? | lib.rs | 311 |
| H | ? | lib.rs | 322 |
| H | ? | lib.rs | 1114 |
| H | ? | lib.rs | 1117 |
| H | ? | lib.rs | 1120 |
| H | ? | lib.rs | 1123 |
| H | ? | lib.rs | 1615 |
| H | ? | lib.rs | 6826 |
| H | ? | lib.rs | 6827 |
| H | ? | lib.rs | 6828 |
| H | ? | lib.rs | 6889 |
| H | ? | lib.rs | 6890 |
| H | ? | lib.rs | 6891 |
| H | ? | file.rs | 63 |
| H | ? | file.rs | 109 |
| H | ? | file.rs | 143 |
| H | ? | config_settings.rs | 125 |
| H | ? | config_settings.rs | 160 |
| H | ? | config_settings.rs | 277 |
| H | ? | build_requires.rs | 104 |
| H | ? | build_requires.rs | 105 |
| H | ? | build_requires.rs | 111 |
| H | ? | build_requires.rs | 112 |
| H | ? | build_requires.rs | 120 |
| H | ? | traits.rs | 36 |
| H | ? | traits.rs | 50 |
| H | ? | traits.rs | 51 |
| H | ? | prioritized_distribution.rs | 533 |
| H | ? | prioritized_distribution.rs | 536 |
| H | ? | prioritized_distribution.rs | 552 |
| H | ? | prioritized_distribution.rs | 561 |
| H | ? | index_url.rs | 26 |
| H | ? | index_url.rs | 65 |
| H | ? | index_url.rs | 113 |
| H | ? | index_url.rs | 303 |
| H | ? | index_url.rs | 537 |
| H | ? | index_url.rs | 540 |
| H | ? | index_url.rs | 674 |
| H | ? | requires_python.rs | 40 |
| H | ? | requires_python.rs | 43 |
| H | ? | requires_python.rs | 51 |
| H | ? | requires_python.rs | 69 |
| H | ? | requires_python.rs | 93 |
| H | ? | requires_python.rs | 97 |
| H | ? | requires_python.rs | 98 |
| H | ? | requires_python.rs | 134 |
| H | ? | requires_python.rs | 135 |
| H | ? | requires_python.rs | 136 |
| H | ? | requires_python.rs | 162 |
| H | ? | requires_python.rs | 166 |
| H | ? | requires_python.rs | 174 |
| H | ? | requires_python.rs | 178 |
| H | ? | requires_python.rs | 186 |
| H | ? | requires_python.rs | 190 |
| H | ? | requires_python.rs | 198 |
| H | ? | requires_python.rs | 202 |
| H | ? | requires_python.rs | 211 |
| H | ? | requires_python.rs | 217 |
| H | ? | requires_python.rs | 223 |
| H | ? | requires_python.rs | 229 |
| H | ? | requires_python.rs | 266 |
| H | ? | requires_python.rs | 274 |
| H | ? | requires_python.rs | 522 |
| H | ? | index.rs | 499 |
| H | ? | index.rs | 536 |
| H | ? | index.rs | 544 |
| H | ? | resolved.rs | 119 |
| H | ? | resolved.rs | 135 |
| H | ? | resolved.rs | 139 |
| H | ? | any.rs | 85 |
| H | ? | any.rs | 87 |
| H | ? | requirement.rs | 614 |
| H | ? | requirement.rs | 619 |
| H | ? | requirement.rs | 632 |
| H | ? | requirement.rs | 655 |
| H | ? | requirement.rs | 656 |
| H | ? | requirement.rs | 659 |
| H | ? | requirement.rs | 667 |
| H | ? | requirement.rs | 671 |
| H | ? | requirement.rs | 680 |
| H | ? | requirement.rs | 685 |
| H | ? | requirement.rs | 693 |
| H | ? | requirement.rs | 694 |
| H | ? | requirement.rs | 696 |
| H | ? | requirement.rs | 705 |
| H | ? | requirement.rs | 706 |
| H | ? | requirement.rs | 709 |
| H | ? | requirement.rs | 930 |
| H | ? | requirement.rs | 986 |
| H | ? | requirement.rs | 1135 |
| H | ? | requirement.rs | 1149 |
| H | ? | installed.rs | 434 |
| H | ? | hash.rs | 166 |
| H | ? | hash.rs | 167 |
| H | ? | hash.rs | 187 |
| H | ? | specified_requirement.rs | 193 |
| H | ? | specified_requirement.rs | 194 |
| H | ? | resolution.rs | 211 |
| H | ? | resolution.rs | 214 |
| H | ? | resolution.rs | 222 |
| H | ? | resolution.rs | 229 |
| H | ? | resolution.rs | 230 |
| H | ? | resolution.rs | 234 |
| H | ? | resolution.rs | 235 |
| H | ? | resolution.rs | 236 |
| H | ? | resolution.rs | 241 |
| H | ? | resolution.rs | 243 |
| H | ? | resolution.rs | 250 |
| H | ? | resolution.rs | 252 |
| H | ? | resolution.rs | 257 |
| H | ? | resolution.rs | 258 |
| H | ? | resolution.rs | 259 |
| H | ? | resolution.rs | 263 |
| H | ? | resolution.rs | 264 |
| H | ? | resolution.rs | 265 |
| H | ? | resolution.rs | 268 |
| H | ? | resolution.rs | 269 |
| H | ? | resolution.rs | 273 |
| H | ? | resolution.rs | 274 |
| H | ? | resolution.rs | 281 |
| H | ? | id.rs | 102 |
| H | ? | id.rs | 104 |
| H | ? | id.rs | 119 |
| H | ? | id.rs | 143 |
| H | ? | id.rs | 221 |
| H | ? | id.rs | 228 |
| H | ? | id.rs | 235 |
| H | ? | dist_error.rs | 119 |
| H | ? | dist_error.rs | 121 |
| H | ? | dist_error.rs | 122 |
| H | ? | dist_error.rs | 123 |
| H | ? | dist_error.rs | 129 |
| H | ? | dist_error.rs | 133 |
| H | ? | dependency_metadata.rs | 18 |
| H | ? | dependency_metadata.rs | 48 |
| H | ? | dependency_metadata.rs | 49 |
| H | ? | dependency_metadata.rs | 50 |
| H | ? | dependency_metadata.rs | 51 |
| H | ? | dependency_metadata.rs | 52 |
| H | ? | dependency_metadata.rs | 62 |
| H | ? | dependency_metadata.rs | 69 |
| H | ? | dependency_metadata.rs | 71 |
| H | ? | dependency_metadata.rs | 72 |
| H | ? | dependency_metadata.rs | 73 |
| H | ? | status_code_strategy.rs | 74 |
| H | ? | status_code_strategy.rs | 78 |
| H | ? | cached.rs | 238 |
| H | ? | annotation.rs | 78 |
| H | ? | lib.rs | 448 |
| H | ? | lib.rs | 544 |
| H | ? | lib.rs | 804 |
| H | ? | lib.rs | 815 |
| H | ? | lib.rs | 826 |
| H | ? | lib.rs | 837 |
| H | ? | lib.rs | 838 |
| H | ? | lib.rs | 848 |
| H | ? | lib.rs | 849 |
| H | ? | lib.rs | 858 |
| H | ? | lib.rs | 859 |
| H | ? | lib.rs | 869 |
| H | ? | lib.rs | 870 |
| H | ? | lib.rs | 880 |
| H | ? | lib.rs | 1027 |
| H | ? | lib.rs | 1060 |
| H | ? | lib.rs | 1061 |
| H | ? | lib.rs | 1423 |
| H | ? | lib.rs | 1427 |
| H | ? | lib.rs | 1776 |
| H | ? | trusted_publishing.rs | 173 |
| H | ? | pypi.rs | 50 |
| H | ? | pypi.rs | 53 |
| H | ? | pypi.rs | 56 |
| H | ? | pypi.rs | 59 |
| H | ? | pypi.rs | 85 |
| H | ? | pypi.rs | 90 |
| H | ? | pypi.rs | 98 |
| H | ? | pyx.rs | 54 |
| H | ? | pyx.rs | 57 |
| H | ? | pyx.rs | 60 |
| H | ? | pyx.rs | 63 |
| H | ? | pyx.rs | 93 |
| H | ? | pyx.rs | 111 |
| H | ? | pyx.rs | 116 |
| H | ? | pyx.rs | 124 |
| H | ? | lib.rs | 294 |
| H | ? | lib.rs | 361 |
| H | ? | lib.rs | 518 |
| H | ? | lib.rs | 519 |
| H | ? | lib.rs | 528 |
| H | ? | lib.rs | 531 |
| H | ? | lib.rs | 548 |
| H | ? | lib.rs | 549 |
| H | ? | lib.rs | 558 |
| H | ? | lib.rs | 559 |
| H | ? | lib.rs | 566 |
| H | ? | lib.rs | 567 |
| H | ? | lib.rs | 573 |
| H | ? | lib.rs | 574 |
| H | ? | lib.rs | 580 |
| H | ? | lib.rs | 581 |
| H | ? | lib.rs | 606 |
| H | ? | lib.rs | 607 |
| H | ? | lib.rs | 630 |
| H | ? | lib.rs | 641 |
| H | ? | lib.rs | 642 |
| H | ? | lib.rs | 665 |
| H | ? | lib.rs | 682 |
| H | ? | lib.rs | 718 |
| H | ? | lib.rs | 753 |
| H | ? | lib.rs | 771 |
| H | ? | lib.rs | 786 |
| H | ? | lib.rs | 792 |
| H | ? | lib.rs | 801 |
| H | ? | lib.rs | 812 |
| H | ? | lib.rs | 828 |
| H | ? | lib.rs | 834 |
| H | ? | lib.rs | 838 |
| H | ? | lib.rs | 844 |
| H | ? | lib.rs | 853 |
| H | ? | lib.rs | 885 |
| H | ? | lib.rs | 898 |
| H | ? | lib.rs | 912 |
| H | ? | lib.rs | 930 |
| H | ? | lib.rs | 937 |
| H | ? | lib.rs | 962 |
| H | ? | lib.rs | 963 |
| H | ? | lib.rs | 965 |
| H | ? | lib.rs | 1044 |
| H | ? | lib.rs | 1051 |
| H | ? | lib.rs | 1071 |
| H | ? | lib.rs | 1139 |
| H | ? | lib.rs | 1238 |
| H | ? | lib.rs | 1244 |
| H | ? | lib.rs | 1245 |
| H | ? | lib.rs | 1256 |
| H | ? | lib.rs | 1280 |
| H | ? | lib.rs | 1327 |
| H | ? | lib.rs | 1341 |
| H | ? | lib.rs | 1367 |
| H | ? | lib.rs | 1371 |
| H | ? | lib.rs | 1412 |
| H | ? | lib.rs | 1422 |
| H | ? | lib.rs | 1426 |
| H | ? | lib.rs | 1636 |
| H | ? | lib.rs | 1700 |
| H | ? | lib.rs | 1775 |
| H | ? | lib.rs | 74 |
| H | ? | mod.rs | 28 |
| H | ? | mod.rs | 31 |
| H | ? | mod.rs | 34 |
| H | ? | mod.rs | 56 |
| H | ? | sync.rs | 101 |
| H | ? | sync.rs | 323 |
| H | ? | sync.rs | 324 |
| H | ? | sync.rs | 326 |
| H | ? | sync.rs | 369 |
| H | ? | sync.rs | 377 |
| H | ? | sync.rs | 389 |
| H | ? | sync.rs | 399 |
| H | ? | sync.rs | 400 |
| H | ? | sync.rs | 402 |
| H | ? | sync.rs | 403 |
| H | ? | sync.rs | 424 |
| H | ? | sync.rs | 449 |
| H | ? | sync.rs | 452 |
| H | ? | sync.rs | 467 |
| H | ? | sync.rs | 472 |
| H | ? | sync.rs | 510 |
| H | ? | sync.rs | 520 |
| H | ? | sync.rs | 524 |
| H | ? | compile.rs | 199 |
| H | ? | compile.rs | 363 |
| H | ? | compile.rs | 462 |
| H | ? | compile.rs | 463 |
| H | ? | compile.rs | 465 |
| H | ? | compile.rs | 508 |
| H | ? | compile.rs | 512 |
| H | ? | compile.rs | 522 |
| H | ? | compile.rs | 527 |
| H | ? | compile.rs | 549 |
| H | ? | compile.rs | 553 |
| H | ? | compile.rs | 562 |
| H | ? | compile.rs | 565 |
| H | ? | compile.rs | 587 |
| H | ? | list.rs | 105 |
| H | ? | list.rs | 106 |
| H | ? | list.rs | 111 |
| H | ? | list.rs | 118 |
| H | ? | list.rs | 184 |
| H | ? | list.rs | 185 |
| H | ? | tree.rs | 91 |
| H | ? | tree.rs | 96 |
| H | ? | tree.rs | 103 |
| H | ? | tree.rs | 247 |
| H | ? | tree.rs | 460 |
| H | ? | install.rs | 138 |
| H | ? | install.rs | 244 |
| H | ? | install.rs | 451 |
| H | ? | install.rs | 452 |
| H | ? | install.rs | 454 |
| H | ? | install.rs | 497 |
| H | ? | install.rs | 512 |
| H | ? | install.rs | 522 |
| H | ? | install.rs | 523 |
| H | ? | install.rs | 525 |
| H | ? | install.rs | 526 |
| H | ? | install.rs | 544 |
| H | ? | install.rs | 569 |
| H | ? | install.rs | 572 |
| H | ? | install.rs | 588 |
| H | ? | install.rs | 593 |
| H | ? | install.rs | 643 |
| H | ? | install.rs | 653 |
| H | ? | install.rs | 657 |
| H | ? | uninstall.rs | 41 |
| H | ? | operations.rs | 157 |
| H | ? | operations.rs | 175 |
| H | ? | operations.rs | 185 |
| H | ? | operations.rs | 224 |
| H | ? | operations.rs | 251 |
| H | ? | operations.rs | 252 |
| H | ? | operations.rs | 253 |
| H | ? | operations.rs | 266 |
| H | ? | operations.rs | 293 |
| H | ? | operations.rs | 335 |
| H | ? | operations.rs | 348 |
| H | ? | operations.rs | 389 |
| H | ? | operations.rs | 927 |
| H | ? | operations.rs | 1053 |
| H | ? | operations.rs | 1061 |
| H | ? | freeze.rs | 70 |
| H | ? | venv.rs | 280 |
| H | ? | venv.rs | 281 |
| H | ? | venv.rs | 327 |
| H | ? | venv.rs | 340 |
| H | ? | build_frontend.rs | 375 |
| H | ? | build_frontend.rs | 414 |
| H | ? | build_frontend.rs | 417 |
| H | ? | build_frontend.rs | 426 |
| H | ? | build_frontend.rs | 439 |
| H | ? | build_frontend.rs | 440 |
| H | ? | build_frontend.rs | 611 |
| H | ? | build_frontend.rs | 612 |
| H | ? | build_frontend.rs | 624 |
| H | ? | build_frontend.rs | 628 |
| H | ? | build_frontend.rs | 646 |
| H | ? | build_frontend.rs | 658 |
| H | ? | build_frontend.rs | 669 |
| H | ? | build_frontend.rs | 671 |
| H | ? | build_frontend.rs | 672 |
| H | ? | build_frontend.rs | 766 |
| H | ? | build_frontend.rs | 1161 |
| H | ? | logout.rs | 35 |
| H | ? | logout.rs | 36 |
| H | ? | logout.rs | 37 |
| H | ? | logout.rs | 116 |
| H | ? | login.rs | 67 |
| H | ? | login.rs | 68 |
| H | ? | login.rs | 69 |
| H | ? | login.rs | 167 |
| H | ? | login.rs | 189 |
| H | ? | login.rs | 208 |
| H | ? | login.rs | 217 |
| H | ? | publish.rs | 91 |
| H | ? | publish.rs | 99 |
| H | ? | publish.rs | 140 |
| H | ? | publish.rs | 155 |
| H | ? | publish.rs | 161 |
| H | ? | publish.rs | 191 |
| H | ? | publish.rs | 195 |
| H | ? | publish.rs | 234 |
| H | ? | publish.rs | 284 |
| H | ? | publish.rs | 286 |
| H | ? | publish.rs | 356 |
| H | ? | publish.rs | 390 |
| H | ? | publish.rs | 654 |
| H | ? | publish.rs | 661 |
| H | ? | publish.rs | 669 |
| H | ? | publish.rs | 678 |
| H | ? | publish.rs | 690 |
| H | ? | publish.rs | 703 |
| H | ? | publish.rs | 715 |
| H | ? | common.rs | 138 |
| H | ? | common.rs | 221 |
| H | ? | common.rs | 264 |
| H | ? | common.rs | 341 |
| H | ? | common.rs | 435 |
| H | ? | common.rs | 436 |
| H | ? | common.rs | 438 |
| H | ? | common.rs | 448 |
| H | ? | common.rs | 452 |
| H | ? | common.rs | 461 |
| H | ? | common.rs | 463 |
| H | ? | common.rs | 477 |
| H | ? | common.rs | 489 |
| H | ? | common.rs | 499 |
| H | ? | common.rs | 500 |
| H | ? | common.rs | 502 |
| H | ? | common.rs | 503 |
| H | ? | common.rs | 509 |
| H | ? | common.rs | 672 |
| H | ? | common.rs | 673 |
| H | ? | common.rs | 790 |
| H | ? | common.rs | 805 |
| H | ? | common.rs | 814 |
| H | ? | common.rs | 818 |
| H | ? | common.rs | 824 |
| H | ? | common.rs | 911 |
| H | ? | common.rs | 938 |
| H | ? | list.rs | 59 |
| H | ? | list.rs | 120 |
| H | ? | list.rs | 127 |
| H | ? | list.rs | 128 |
| H | ? | list.rs | 129 |
| H | ? | list.rs | 130 |
| H | ? | list.rs | 134 |
| H | ? | list.rs | 140 |
| H | ? | list.rs | 142 |
| H | ? | list.rs | 144 |
| H | ? | list.rs | 178 |
| H | ? | install.rs | 160 |
| H | ? | install.rs | 169 |
| H | ? | install.rs | 227 |
| H | ? | install.rs | 228 |
| H | ? | install.rs | 233 |
| H | ? | install.rs | 251 |
| H | ? | install.rs | 252 |
| H | ? | install.rs | 282 |
| H | ? | install.rs | 284 |
| H | ? | install.rs | 286 |
| H | ? | install.rs | 294 |
| H | ? | install.rs | 312 |
| H | ? | install.rs | 317 |
| H | ? | install.rs | 341 |
| H | ? | install.rs | 353 |
| H | ? | install.rs | 374 |
| H | ? | install.rs | 377 |
| H | ? | install.rs | 403 |
| H | ? | install.rs | 414 |
| H | ? | install.rs | 448 |
| H | ? | install.rs | 593 |
| H | ? | install.rs | 619 |
| H | ? | install.rs | 636 |
| H | ? | install.rs | 670 |
| H | ? | install.rs | 706 |
| H | ? | install.rs | 759 |
| H | ? | install.rs | 789 |
| H | ? | install.rs | 791 |
| H | ? | install.rs | 797 |
| H | ? | install.rs | 798 |
| H | ? | install.rs | 799 |
| H | ? | install.rs | 800 |
| H | ? | install.rs | 801 |
| H | ? | install.rs | 804 |
| H | ? | install.rs | 910 |
| H | ? | install.rs | 965 |
| H | ? | upgrade.rs | 78 |
| H | ? | upgrade.rs | 160 |
| H | ? | upgrade.rs | 161 |
| H | ? | upgrade.rs | 322 |
| H | ? | upgrade.rs | 323 |
| H | ? | upgrade.rs | 324 |
| H | ? | upgrade.rs | 326 |
| H | ? | upgrade.rs | 374 |
| H | ? | upgrade.rs | 398 |
| H | ? | upgrade.rs | 435 |
| H | ? | upgrade.rs | 481 |
| H | ? | upgrade.rs | 499 |
| H | ? | upgrade.rs | 511 |
| H | ? | upgrade.rs | 547 |
| H | ? | upgrade.rs | 605 |
| H | ? | upgrade.rs | 638 |
| H | ? | run.rs | 711 |
| H | ? | run.rs | 778 |
| H | ? | run.rs | 833 |
| H | ? | run.rs | 834 |
| H | ? | run.rs | 839 |
| H | ? | run.rs | 855 |
| H | ? | run.rs | 856 |
| H | ? | run.rs | 887 |
| H | ? | run.rs | 889 |
| H | ? | run.rs | 891 |
| H | ? | run.rs | 899 |
| H | ? | run.rs | 917 |
| H | ? | run.rs | 922 |
| H | ? | run.rs | 957 |
| H | ? | run.rs | 961 |
| H | ? | run.rs | 981 |
| H | ? | run.rs | 988 |
| H | ? | run.rs | 1038 |
| H | ? | run.rs | 1053 |
| H | ? | run.rs | 1103 |
| H | ? | run.rs | 1104 |
| H | ? | diagnostics.rs | 204 |
| H | ? | diagnostics.rs | 205 |
| H | ? | diagnostics.rs | 214 |
| H | ? | self_update.rs | 86 |
| H | ? | self_update.rs | 162 |
| H | ? | self_update.rs | 230 |
| H | ? | self_update.rs | 447 |
| H | ? | self_update.rs | 456 |
| H | ? | self_update.rs | 464 |
| H | ? | list.rs | 124 |
| H | ? | list.rs | 261 |
| H | ? | install.rs | 132 |
| H | ? | install.rs | 136 |
| H | ? | install.rs | 140 |
| H | ? | install.rs | 329 |
| H | ? | install.rs | 489 |
| H | ? | install.rs | 548 |
| H | ? | install.rs | 645 |
| H | ? | install.rs | 648 |
| H | ? | install.rs | 653 |
| H | ? | install.rs | 659 |
| H | ? | install.rs | 661 |
| H | ? | install.rs | 666 |
| H | ? | install.rs | 724 |
| H | ? | install.rs | 835 |
| H | ? | install.rs | 1022 |
| H | ? | install.rs | 1037 |
| H | ? | install.rs | 1040 |
| H | ? | install.rs | 1042 |
| H | ? | install.rs | 1089 |
| H | ? | install.rs | 1162 |
| H | ? | install.rs | 1176 |
| H | ? | install.rs | 1184 |
| H | ? | install.rs | 1198 |
| H | ? | install.rs | 1201 |
| H | ? | install.rs | 1203 |
| H | ? | install.rs | 1208 |
| H | ? | install.rs | 1219 |
| H | ? | install.rs | 1227 |
| H | ? | uninstall.rs | 108 |
| H | ? | uninstall.rs | 196 |
| H | ? | uninstall.rs | 214 |
| H | ? | uninstall.rs | 216 |
| H | ? | module_owners.rs | 68 |
| H | ? | module_owners.rs | 140 |
| H | ? | module_owners.rs | 160 |
| H | ? | help.rs | 52 |
| H | ? | pylock.rs | 35 |
| H | ? | lock_target.rs | 46 |
| H | ? | lock_target.rs | 258 |
| H | ? | lock_target.rs | 363 |
| H | ? | lock_target.rs | 412 |
| H | ? | lock_target.rs | 424 |
| H | ? | mod.rs | 630 |
| H | ? | mod.rs | 631 |
| H | ? | mod.rs | 639 |
| H | ? | mod.rs | 640 |
| H | ? | mod.rs | 647 |
| H | ? | mod.rs | 648 |
| H | ? | mod.rs | 668 |
| H | ? | mod.rs | 669 |
| H | ? | mod.rs | 675 |
| H | ? | mod.rs | 676 |
| H | ? | mod.rs | 681 |
| H | ? | mod.rs | 682 |
| H | ? | mod.rs | 969 |
| H | ? | mod.rs | 982 |
| H | ? | mod.rs | 989 |
| H | ? | mod.rs | 1167 |
| H | ? | mod.rs | 1503 |
| H | ? | mod.rs | 1556 |
| H | ? | mod.rs | 1599 |
| H | ? | mod.rs | 1605 |
| H | ? | mod.rs | 2174 |
| H | ? | mod.rs | 2190 |
| H | ? | mod.rs | 2199 |
| H | ? | mod.rs | 2200 |
| H | ? | mod.rs | 2202 |
| H | ? | mod.rs | 2213 |
| H | ? | mod.rs | 2217 |
| H | ? | mod.rs | 2231 |
| H | ? | mod.rs | 2243 |
| H | ? | mod.rs | 2253 |
| H | ? | mod.rs | 2254 |
| H | ? | mod.rs | 2256 |
| H | ? | mod.rs | 2257 |
| H | ? | mod.rs | 2269 |
| H | ? | mod.rs | 2380 |
| H | ? | mod.rs | 2425 |
| H | ? | mod.rs | 2432 |
| H | ? | mod.rs | 2433 |
| H | ? | mod.rs | 2435 |
| H | ? | mod.rs | 2445 |
| H | ? | mod.rs | 2449 |
| H | ? | mod.rs | 2458 |
| H | ? | mod.rs | 2460 |
| H | ? | mod.rs | 2479 |
| H | ? | mod.rs | 2511 |
| H | ? | mod.rs | 2523 |
| H | ? | mod.rs | 2533 |
| H | ? | mod.rs | 2534 |
| H | ? | mod.rs | 2536 |
| H | ? | mod.rs | 2537 |
| H | ? | mod.rs | 2611 |
| H | ? | mod.rs | 2620 |
| H | ? | mod.rs | 2621 |
| H | ? | mod.rs | 2653 |
| H | ? | mod.rs | 2665 |
| H | ? | mod.rs | 2675 |
| H | ? | mod.rs | 2679 |
| H | ? | mod.rs | 2783 |
| H | ? | mod.rs | 2868 |
| H | ? | mod.rs | 2875 |
| H | ? | mod.rs | 2876 |
| H | ? | mod.rs | 2878 |
| H | ? | mod.rs | 2896 |
| H | ? | mod.rs | 2898 |
| H | ? | mod.rs | 2930 |
| H | ? | mod.rs | 2940 |
| H | ? | mod.rs | 2941 |
| H | ? | mod.rs | 2943 |
| H | ? | mod.rs | 2944 |
| H | ? | mod.rs | 2961 |
| H | ? | mod.rs | 2966 |
| H | ? | mod.rs | 3087 |
| H | ? | mod.rs | 3091 |
| H | ? | mod.rs | 3093 |
| H | ? | mod.rs | 3126 |
| H | ? | mod.rs | 3131 |
| H | ? | mod.rs | 3133 |
| H | ? | mod.rs | 3308 |
| H | ? | version.rs | 275 |
| H | ? | version.rs | 419 |
| H | ? | ty.rs | 68 |
| H | ? | install_target.rs | 360 |
| H | ? | install_target.rs | 361 |
| H | ? | install_target.rs | 364 |
| H | ? | install_target.rs | 366 |
| H | ? | install_target.rs | 377 |
| H | ? | install_target.rs | 421 |
| H | ? | install_target.rs | 443 |
| H | ? | install_target.rs | 446 |
| H | ? | install_target.rs | 455 |
| H | ? | sync.rs | 121 |
| H | ? | sync.rs | 265 |
| H | ? | sync.rs | 270 |
| H | ? | sync.rs | 664 |
| H | ? | sync.rs | 674 |
| H | ? | sync.rs | 675 |
| H | ? | sync.rs | 676 |
| H | ? | sync.rs | 677 |
| H | ? | sync.rs | 678 |
| H | ? | sync.rs | 680 |
| H | ? | sync.rs | 684 |
| H | ? | sync.rs | 685 |
| H | ? | sync.rs | 686 |
| H | ? | sync.rs | 689 |
| H | ? | sync.rs | 704 |
| H | ? | sync.rs | 707 |
| H | ? | sync.rs | 716 |
| H | ? | sync.rs | 717 |
| H | ? | sync.rs | 827 |
| H | ? | sync.rs | 828 |
| H | ? | sync.rs | 868 |
| H | ? | sync.rs | 878 |
| H | ? | sync.rs | 879 |
| H | ? | sync.rs | 881 |
| H | ? | sync.rs | 882 |
| H | ? | sync.rs | 950 |
| H | ? | sync.rs | 997 |
| H | ? | sync.rs | 1000 |
| H | ? | sync.rs | 1004 |
| H | ? | sync.rs | 1022 |
| H | ? | sync.rs | 1030 |
| H | ? | sync.rs | 1078 |
| H | ? | sync.rs | 1321 |
| H | ? | sync.rs | 1475 |
| H | ? | tree.rs | 246 |
| H | ? | tree.rs | 247 |
| H | ? | tree.rs | 249 |
| H | ? | tree.rs | 252 |
| H | ? | tree.rs | 292 |
| H | ? | lock.rs | 370 |
| H | ? | lock.rs | 372 |
| H | ? | lock.rs | 706 |
| H | ? | lock.rs | 716 |
| H | ? | lock.rs | 719 |
| H | ? | lock.rs | 724 |
| H | ? | lock.rs | 731 |
| H | ? | lock.rs | 732 |
| H | ? | lock.rs | 743 |
| H | ? | lock.rs | 747 |
| H | ? | lock.rs | 766 |
| H | ? | lock.rs | 768 |
| H | ? | lock.rs | 769 |
| H | ? | lock.rs | 791 |
| H | ? | lock.rs | 826 |
| H | ? | lock.rs | 827 |
| H | ? | lock.rs | 829 |
| H | ? | lock.rs | 830 |
| H | ? | lock.rs | 837 |
| H | ? | lock.rs | 976 |
| H | ? | lock.rs | 977 |
| H | ? | lock.rs | 993 |
| H | ? | lock.rs | 1016 |
| H | ? | lock.rs | 1027 |
| H | ? | lock.rs | 1566 |
| H | ? | upgrade.rs | 76 |
| H | ? | upgrade.rs | 107 |
| H | ? | upgrade.rs | 149 |
| H | ? | upgrade.rs | 188 |
| H | ? | upgrade.rs | 260 |
| H | ? | upgrade.rs | 266 |
| H | ? | upgrade.rs | 363 |
| H | ? | upgrade.rs | 367 |
| H | ? | upgrade.rs | 373 |
| H | ? | upgrade.rs | 376 |
| H | ? | upgrade.rs | 410 |
| H | ? | upgrade.rs | 445 |
| H | ? | upgrade.rs | 452 |
| H | ? | upgrade.rs | 460 |
| H | ? | upgrade.rs | 477 |
| H | ? | upgrade.rs | 513 |
| H | ? | upgrade.rs | 515 |
| H | ? | toolchain.rs | 48 |
| H | ? | toolchain.rs | 50 |
| H | ? | run.rs | 287 |
| H | ? | run.rs | 404 |
| H | ? | run.rs | 541 |
| H | ? | run.rs | 1043 |
| H | ? | run.rs | 1341 |
| H | ? | run.rs | 1438 |
| H | ? | run.rs | 1539 |
| H | ? | run.rs | 1544 |
| H | ? | run.rs | 1549 |
| H | ? | run.rs | 1580 |
| H | ? | run.rs | 1591 |
| H | ? | run.rs | 1605 |
| H | ? | run.rs | 1618 |
| H | ? | run.rs | 1772 |
| H | ? | run.rs | 1776 |
| H | ? | run.rs | 1803 |
| H | ? | run.rs | 1807 |
| H | ? | add.rs | 152 |
| H | ? | add.rs | 158 |
| H | ? | add.rs | 341 |
| H | ? | add.rs | 393 |
| H | ? | add.rs | 394 |
| H | ? | add.rs | 405 |
| H | ? | add.rs | 409 |
| H | ? | add.rs | 433 |
| H | ? | add.rs | 441 |
| H | ? | add.rs | 447 |
| H | ? | add.rs | 456 |
| H | ? | add.rs | 466 |
| H | ? | add.rs | 471 |
| H | ? | add.rs | 482 |
| H | ? | add.rs | 728 |
| H | ? | add.rs | 761 |
| H | ? | add.rs | 762 |
| H | ? | add.rs | 932 |
| H | ? | add.rs | 959 |
| H | ? | add.rs | 967 |
| H | ? | add.rs | 968 |
| H | ? | add.rs | 969 |
| H | ? | add.rs | 977 |
| H | ? | add.rs | 983 |
| H | ? | add.rs | 987 |
| H | ? | add.rs | 988 |
| H | ? | add.rs | 1157 |
| H | ? | add.rs | 1292 |
| H | ? | add.rs | 1440 |
| H | ? | remove.rs | 98 |
| H | ? | remove.rs | 130 |
| H | ? | remove.rs | 131 |
| H | ? | remove.rs | 143 |
| H | ? | remove.rs | 144 |
| H | ? | remove.rs | 154 |
| H | ? | remove.rs | 155 |
| H | ? | remove.rs | 168 |
| H | ? | remove.rs | 169 |
| H | ? | remove.rs | 178 |
| H | ? | remove.rs | 179 |
| H | ? | export.rs | 115 |
| H | ? | init.rs | 474 |
| H | ? | init.rs | 489 |
| H | ? | init.rs | 556 |
| H | ? | sarif.rs | 51 |
| H | ? | sarif.rs | 52 |
| H | ? | sarif.rs | 62 |
| H | ? | sarif.rs | 63 |
| H | ? | sarif.rs | 156 |
| H | ? | sarif.rs | 295 |
| H | ? | sarif.rs | 308 |
| H | ? | sarif.rs | 340 |
| H | ? | sarif.rs | 343 |
| H | ? | json.rs | 117 |
| H | ? | json.rs | 118 |
| H | ? | json.rs | 152 |
| H | ? | audit.rs | 237 |
| H | ? | audit.rs | 239 |
| H | ? | audit.rs | 241 |
| H | ? | audit.rs | 242 |
| H | ? | audit.rs | 247 |
| H | ? | audit.rs | 253 |
| H | ? | environment.rs | 163 |
| H | ? | environment.rs | 266 |
| H | ? | environment.rs | 267 |
| H | ? | environment.rs | 310 |
| H | ? | environment.rs | 379 |
| H | ? | environment.rs | 403 |
| H | ? | environment.rs | 405 |
| H | ? | editable.rs | 37 |
| H | ? | editable.rs | 38 |
| H | ? | editable.rs | 41 |
| H | ? | editable.rs | 43 |
| H | ? | settings.rs | 106 |
| H | ? | settings.rs | 370 |
| H | ? | settings.rs | 376 |
| H | ? | settings.rs | 381 |
| H | ? | settings.rs | 382 |
| H | ? | settings.rs | 383 |
| H | ? | settings.rs | 430 |
| H | ? | settings.rs | 489 |
| H | ? | settings.rs | 758 |
| H | ? | settings.rs | 759 |
| H | ? | settings.rs | 811 |
| H | ? | settings.rs | 955 |
| H | ? | settings.rs | 960 |
| H | ? | settings.rs | 963 |
| H | ? | settings.rs | 1080 |
| H | ? | settings.rs | 1085 |
| H | ? | settings.rs | 1088 |
| H | ? | settings.rs | 1237 |
| H | ? | settings.rs | 1254 |
| H | ? | settings.rs | 1396 |
| H | ? | settings.rs | 1397 |
| H | ? | settings.rs | 1398 |
| H | ? | settings.rs | 1407 |
| H | ? | settings.rs | 1413 |
| H | ? | settings.rs | 1419 |
| H | ? | settings.rs | 1486 |
| H | ? | settings.rs | 1577 |
| H | ? | settings.rs | 1691 |
| H | ? | settings.rs | 1747 |
| H | ? | settings.rs | 1844 |
| H | ? | settings.rs | 1845 |
| H | ? | settings.rs | 1949 |
| H | ? | settings.rs | 2023 |
| H | ? | settings.rs | 2024 |
| H | ? | settings.rs | 2075 |
| H | ? | settings.rs | 2076 |
| H | ? | settings.rs | 2081 |
| H | ? | settings.rs | 2129 |
| H | ? | settings.rs | 2130 |
| H | ? | settings.rs | 2305 |
| H | ? | settings.rs | 2350 |
| H | ? | settings.rs | 2510 |
| H | ? | settings.rs | 2511 |
| H | ? | settings.rs | 2602 |
| H | ? | settings.rs | 2603 |
| H | ? | settings.rs | 2699 |
| H | ? | settings.rs | 2700 |
| H | ? | settings.rs | 2726 |
| H | ? | settings.rs | 2843 |
| H | ? | settings.rs | 2844 |
| H | ? | settings.rs | 2891 |
| H | ? | settings.rs | 3040 |
| H | ? | settings.rs | 3041 |
| H | ? | settings.rs | 3081 |
| H | ? | settings.rs | 3154 |
| H | ? | settings.rs | 3155 |
| H | ? | settings.rs | 3160 |
| H | ? | settings.rs | 3188 |
| H | ? | settings.rs | 3193 |
| H | ? | settings.rs | 3239 |
| H | ? | settings.rs | 3245 |
| H | ? | settings.rs | 3344 |
| H | ? | settings.rs | 3360 |
| H | ? | settings.rs | 3369 |
| H | ? | settings.rs | 3381 |
| H | ? | settings.rs | 3389 |
| H | ? | settings.rs | 3649 |
| H | ? | settings.rs | 3665 |
| H | ? | settings.rs | 3674 |
| H | ? | settings.rs | 4112 |
| H | ? | settings.rs | 4118 |
| H | ? | settings.rs | 4326 |
| H | ? | settings.rs | 4329 |
| H | ? | settings.rs | 4332 |
| H | ? | settings.rs | 4344 |
| H | ? | settings.rs | 4441 |
| H | ? | settings.rs | 4456 |
| H | ? | settings.rs | 4459 |
| H | ? | settings.rs | 4462 |
| H | ? | settings.rs | 4751 |
| H | ? | settings.rs | 4857 |
| H | ? | settings.rs | 4981 |
| H | ? | settings.rs | 5170 |
| H | ? | lib.rs | 120 |
| H | ? | lib.rs | 297 |
| H | ? | lib.rs | 472 |
| H | ? | lib.rs | 630 |
| H | ? | lib.rs | 636 |
| H | ? | lib.rs | 637 |
| H | ? | lib.rs | 638 |
| H | ? | lib.rs | 735 |
| H | ? | lib.rs | 736 |
| H | ? | lib.rs | 812 |
| H | ? | lib.rs | 854 |
| H | ? | lib.rs | 855 |
| H | ? | lib.rs | 900 |
| H | ? | lib.rs | 998 |
| H | ? | lib.rs | 1011 |
| H | ? | lib.rs | 1025 |
| H | ? | lib.rs | 1026 |
| H | ? | lib.rs | 1061 |
| H | ? | lib.rs | 1297 |
| H | ? | lib.rs | 1365 |
| H | ? | lib.rs | 1366 |
| H | ? | lib.rs | 1500 |
| H | ? | lib.rs | 1534 |
| H | ? | lib.rs | 1535 |
| H | ? | lib.rs | 1625 |
| H | ? | lib.rs | 1626 |
| H | ? | lib.rs | 1627 |
| H | ? | lib.rs | 1655 |
| H | ? | lib.rs | 2049 |
| H | ? | lib.rs | 2050 |
| H | ? | lib.rs | 2162 |
| H | ? | lib.rs | 2292 |
| H | ? | lib.rs | 2293 |
| H | ? | lib.rs | 2363 |
| H | ? | lib.rs | 2364 |
| H | ? | lib.rs | 2420 |
| H | ? | lib.rs | 2421 |
| H | ? | lib.rs | 2468 |
| H | ? | lib.rs | 2539 |
| H | ? | lib.rs | 2552 |
| H | ? | lib.rs | 2566 |
| H | ? | lib.rs | 2567 |
| H | ? | lib.rs | 2635 |
| H | ? | lib.rs | 2636 |
| H | ? | lib.rs | 2690 |
| H | ? | lib.rs | 2691 |
| H | ? | lib.rs | 2861 |
| H | ? | lib.rs | 2862 |
| H | ? | discovery.rs | 428 |
| H | ? | discovery.rs | 622 |
| H | ? | discovery.rs | 640 |
| H | ? | discovery.rs | 1077 |
| H | ? | discovery.rs | 1084 |
| H | ? | discovery.rs | 1090 |
| H | ? | discovery.rs | 1103 |
| H | ? | discovery.rs | 1110 |
| H | ? | discovery.rs | 1116 |
| H | ? | discovery.rs | 1134 |
| H | ? | discovery.rs | 1329 |
| H | ? | discovery.rs | 1343 |
| H | ? | discovery.rs | 1369 |
| H | ? | discovery.rs | 1414 |
| H | ? | discovery.rs | 1455 |
| H | ? | discovery.rs | 1461 |
| H | ? | discovery.rs | 1510 |
| H | ? | discovery.rs | 1515 |
| H | ? | discovery.rs | 1571 |
| H | ? | discovery.rs | 1814 |
| H | ? | discovery.rs | 2273 |
| H | ? | discovery.rs | 2932 |
| H | ? | discovery.rs | 2971 |
| H | ? | discovery.rs | 3098 |
| H | ? | discovery.rs | 3333 |
| H | ? | replacements.rs | 24 |
| H | ? | cursor.rs | 24 |
| H | ? | target.rs | 14 |
| H | ? | target.rs | 15 |
| H | ? | target.rs | 17 |
| H | ? | windows_registry.rs | 253 |
| H | ? | interpreter.rs | 201 |
| H | ? | interpreter.rs | 250 |
| H | ? | interpreter.rs | 312 |
| H | ? | interpreter.rs | 1224 |
| H | ? | downloads.rs | 390 |
| H | ? | downloads.rs | 397 |
| H | ? | downloads.rs | 399 |
| H | ? | downloads.rs | 1010 |
| H | ? | downloads.rs | 1016 |
| H | ? | downloads.rs | 1141 |
| H | ? | downloads.rs | 1143 |
| H | ? | downloads.rs | 1149 |
| H | ? | downloads.rs | 1248 |
| H | ? | downloads.rs | 1250 |
| H | ? | downloads.rs | 1295 |
| H | ? | downloads.rs | 1296 |
| H | ? | downloads.rs | 1412 |
| H | ? | downloads.rs | 1608 |
| H | ? | downloads.rs | 1832 |
| H | ? | downloads.rs | 1835 |
| H | ? | downloads.rs | 1845 |
| H | ? | downloads.rs | 2155 |
| H | ? | downloads.rs | 2187 |
| H | ? | downloads.rs | 2219 |
| H | ? | downloads.rs | 2251 |
| H | ? | managed.rs | 241 |
| H | ? | managed.rs | 283 |
| H | ? | managed.rs | 288 |
| H | ? | managed.rs | 321 |
| H | ? | managed.rs | 322 |
| H | ? | managed.rs | 460 |
| H | ? | managed.rs | 524 |
| H | ? | managed.rs | 810 |
| H | ? | installation.rs | 230 |
| H | ? | installation.rs | 271 |
| H | ? | installation.rs | 274 |
| H | ? | installation.rs | 281 |
| H | ? | installation.rs | 290 |
| H | ? | installation.rs | 299 |
| H | ? | installation.rs | 831 |
| H | ? | installation.rs | 834 |
| H | ? | installation.rs | 837 |
| H | ? | environment.rs | 213 |
| H | ? | environment.rs | 360 |
| H | ? | lib.rs | 1039 |
| H | ? | build.rs | 14 |
| H | ? | source.rs | 74 |
| H | ? | source.rs | 82 |
| H | ? | source.rs | 151 |
| H | ? | resolver.rs | 191 |
| H | ? | resolver.rs | 200 |
| H | ? | resolver.rs | 210 |
| H | ? | resolver.rs | 213 |
| H | ? | resolver.rs | 305 |
| H | ? | resolver.rs | 306 |
| H | ? | credentials.rs | 40 |
| H | ? | git.rs | 242 |
| H | ? | git.rs | 369 |
| H | ? | git.rs | 640 |
| H | ? | git.rs | 881 |
| H | ? | git.rs | 885 |
| H | ? | git.rs | 898 |
| H | ? | git.rs | 935 |
| H | ? | wheel.rs | 32 |
| H | ? | wheel.rs | 35 |
| H | ? | wheel.rs | 38 |
| H | ? | wheel.rs | 41 |
| H | ? | wheel.rs | 44 |
| H | ? | lib.rs | 468 |
| H | ? | lib.rs | 504 |
| H | ? | lib.rs | 779 |
| H | ? | tool.rs | 340 |
| H | ? | lib.rs | 48 |
| H | ? | lib.rs | 49 |
| H | ? | lib.rs | 228 |
| H | ? | lib.rs | 277 |
| H | ? | lib.rs | 402 |
| H | ? | cache.rs | 140 |
| H | ? | cache.rs | 186 |
| H | ? | cache.rs | 192 |
| H | ? | cache.rs | 322 |
| H | ? | cache.rs | 326 |
| H | ? | cache.rs | 330 |
| H | ? | cache.rs | 334 |
| H | ? | cache.rs | 376 |
| H | ? | cache.rs | 382 |
| H | ? | cache.rs | 383 |
| H | ? | cache.rs | 387 |
| H | ? | cache.rs | 388 |
| H | ? | store.rs | 282 |
| H | ? | store.rs | 286 |
| H | ? | store.rs | 352 |
| H | ? | store.rs | 389 |
| H | ? | store.rs | 404 |
| H | ? | store.rs | 467 |
| H | ? | store.rs | 538 |
| H | ? | store.rs | 576 |
| H | ? | store.rs | 623 |
| H | ? | store.rs | 624 |
| H | ? | store.rs | 643 |
| H | ? | store.rs | 711 |
| H | ? | store.rs | 712 |
| H | ? | store.rs | 719 |
| H | ? | index.rs | 138 |
| H | ? | credentials.rs | 170 |
| H | ? | credentials.rs | 226 |
| H | ? | credentials.rs | 227 |
| H | ? | credentials.rs | 536 |
| H | ? | credentials.rs | 543 |
| H | ? | credentials.rs | 568 |
| H | ? | credentials.rs | 575 |
| H | ? | credentials.rs | 600 |
| H | ? | credentials.rs | 607 |
| H | ? | credentials.rs | 682 |
| H | ? | credentials.rs | 707 |
| H | ? | credentials.rs | 734 |
| H | ? | credentials.rs | 744 |
| H | ? | credentials.rs | 756 |
| H | ? | credentials.rs | 766 |
| H | ? | credentials.rs | 778 |
| H | ? | credentials.rs | 788 |
| H | ? | credentials.rs | 800 |
| H | ? | middleware.rs | 464 |
| H | ? | middleware.rs | 591 |
| H | ? | middleware.rs | 719 |
| H | ? | middleware.rs | 742 |
| H | ? | middleware.rs | 755 |
| H | ? | middleware.rs | 758 |
| H | ? | middleware.rs | 763 |
| H | ? | middleware.rs | 777 |
| H | ? | middleware.rs | 780 |
| H | ? | middleware.rs | 785 |
| H | ? | middleware.rs | 799 |
| H | ? | middleware.rs | 802 |
| H | ? | middleware.rs | 807 |
| H | ? | middleware.rs | 837 |
| H | ? | middleware.rs | 840 |
| H | ? | middleware.rs | 967 |
| H | ? | middleware.rs | 974 |
| H | ? | middleware.rs | 1072 |
| H | ? | middleware.rs | 1094 |
| H | ? | middleware.rs | 1126 |
| H | ? | middleware.rs | 1148 |
| H | ? | middleware.rs | 1180 |
| H | ? | middleware.rs | 1202 |
| H | ? | middleware.rs | 1291 |
| H | ? | middleware.rs | 1373 |
| H | ? | middleware.rs | 1381 |
| H | ? | middleware.rs | 1421 |
| H | ? | middleware.rs | 1429 |
| H | ? | middleware.rs | 1438 |
| H | ? | middleware.rs | 1441 |
| H | ? | middleware.rs | 1446 |
| H | ? | middleware.rs | 1488 |
| H | ? | middleware.rs | 1496 |
| H | ? | middleware.rs | 1505 |
| H | ? | middleware.rs | 1542 |
| H | ? | middleware.rs | 1591 |
| H | ? | middleware.rs | 1720 |
| H | ? | middleware.rs | 1723 |
| H | ? | middleware.rs | 1733 |
| H | ? | middleware.rs | 1736 |
| H | ? | middleware.rs | 1832 |
| H | ? | middleware.rs | 1837 |
| H | ? | middleware.rs | 1870 |
| H | ? | middleware.rs | 1960 |
| H | ? | middleware.rs | 1965 |
| H | ? | middleware.rs | 1970 |
| H | ? | middleware.rs | 1973 |
| H | ? | middleware.rs | 1978 |
| H | ? | middleware.rs | 1983 |
| H | ? | middleware.rs | 1986 |
| H | ? | middleware.rs | 2019 |
| H | ? | middleware.rs | 2067 |
| H | ? | middleware.rs | 2068 |
| H | ? | middleware.rs | 2075 |
| H | ? | middleware.rs | 2080 |
| H | ? | middleware.rs | 2085 |
| H | ? | middleware.rs | 2088 |
| H | ? | middleware.rs | 2093 |
| H | ? | middleware.rs | 2107 |
| H | ? | middleware.rs | 2110 |
| H | ? | middleware.rs | 2163 |
| H | ? | middleware.rs | 2164 |
| H | ? | middleware.rs | 2168 |
| H | ? | middleware.rs | 2169 |
| H | ? | middleware.rs | 2179 |
| H | ? | middleware.rs | 2180 |
| H | ? | middleware.rs | 2188 |
| H | ? | middleware.rs | 2193 |
| H | ? | middleware.rs | 2198 |
| H | ? | middleware.rs | 2201 |
| H | ? | middleware.rs | 2206 |
| H | ? | middleware.rs | 2220 |
| H | ? | middleware.rs | 2223 |
| H | ? | middleware.rs | 2271 |
| H | ? | middleware.rs | 2272 |
| H | ? | middleware.rs | 2281 |
| H | ? | middleware.rs | 2291 |
| H | ? | middleware.rs | 2297 |
| H | ? | middleware.rs | 2300 |
| H | ? | middleware.rs | 2305 |
| H | ? | middleware.rs | 2308 |
| H | ? | middleware.rs | 2326 |
| H | ? | middleware.rs | 2330 |
| H | ? | middleware.rs | 2331 |
| H | ? | middleware.rs | 2368 |
| H | ? | middleware.rs | 2383 |
| H | ? | middleware.rs | 2463 |
| H | ? | middleware.rs | 2561 |
| H | ? | middleware.rs | 2616 |
| H | ? | middleware.rs | 2707 |
| H | ? | pyx.rs | 238 |
| H | ? | pyx.rs | 419 |
| H | ? | pyx.rs | 488 |
| H | ? | pyx.rs | 511 |
| H | ? | providers.rs | 53 |
| H | ? | virtualenv.rs | 226 |
| H | ? | virtualenv.rs | 240 |
| H | ? | virtualenv.rs | 243 |
| H | ? | virtualenv.rs | 246 |
| H | ? | virtualenv.rs | 487 |
| H | ? | virtualenv.rs | 536 |
| H | ? | lib.rs | 131 |
| H | ? | generate_scenarios.rs | 85 |
| H | ? | generate_scenarios.rs | 704 |
| H | ? | generate_scenarios.rs | 705 |
| H | ? | generate_scenarios.rs | 891 |
| H | ? | generate_scenarios.rs | 906 |
| H | ? | validate_zip.rs | 40 |
| H | ? | generate_cli_reference.rs | 150 |
| H | ? | hash.rs | 58 |
| H | ? | hash.rs | 103 |
| H | ? | hash.rs | 220 |
| H | ? | hash.rs | 341 |
| H | ? | hash.rs | 374 |
| H | ? | hash.rs | 375 |
| H | ? | hash.rs | 383 |
| H | ? | hash.rs | 384 |
| H | ? | hash.rs | 458 |
| H | ? | hash.rs | 459 |
| H | ? | hash.rs | 462 |
| H | ? | builds.rs | 72 |
| H | ? | distribution_database.rs | 89 |
| H | ? | distribution_database.rs | 151 |
| H | ? | distribution_database.rs | 153 |
| H | ? | distribution_database.rs | 205 |
| H | ? | distribution_database.rs | 221 |
| H | ? | distribution_database.rs | 233 |
| H | ? | distribution_database.rs | 240 |
| H | ? | distribution_database.rs | 271 |
| H | ? | distribution_database.rs | 278 |
| H | ? | distribution_database.rs | 298 |
| H | ? | distribution_database.rs | 310 |
| H | ? | distribution_database.rs | 317 |
| H | ? | distribution_database.rs | 336 |
| H | ? | distribution_database.rs | 347 |
| H | ? | distribution_database.rs | 354 |
| H | ? | distribution_database.rs | 372 |
| H | ? | distribution_database.rs | 483 |
| H | ? | distribution_database.rs | 496 |
| H | ? | distribution_database.rs | 527 |
| H | ? | distribution_database.rs | 549 |
| H | ? | distribution_database.rs | 617 |
| H | ? | distribution_database.rs | 667 |
| H | ? | distribution_database.rs | 717 |
| H | ? | distribution_database.rs | 794 |
| H | ? | distribution_database.rs | 801 |
| H | ? | distribution_database.rs | 829 |
| H | ? | distribution_database.rs | 970 |
| H | ? | distribution_database.rs | 976 |
| H | ? | distribution_database.rs | 1004 |
| H | ? | distribution_database.rs | 1076 |
| H | ? | distribution_database.rs | 1083 |
| H | ? | distribution_database.rs | 1093 |
| H | ? | distribution_database.rs | 1099 |
| H | ? | distribution_database.rs | 1104 |
| H | ? | distribution_database.rs | 1111 |
| H | ? | distribution_database.rs | 1161 |
| H | ? | distribution_database.rs | 1166 |
| H | ? | distribution_database.rs | 1171 |
| H | ? | distribution_database.rs | 1178 |
| H | ? | build_requires.rs | 132 |
| H | ? | build_requires.rs | 152 |
| H | ? | build_requires.rs | 206 |
| H | ? | build_requires.rs | 227 |
| H | ? | build_requires.rs | 296 |
| H | ? | build_requires.rs | 320 |
| H | ? | lowering.rs | 97 |
| H | ? | lowering.rs | 106 |
| H | ? | lowering.rs | 114 |
| H | ? | lowering.rs | 122 |
| H | ? | lowering.rs | 130 |
| H | ? | lowering.rs | 165 |
| H | ? | lowering.rs | 243 |
| H | ? | lowering.rs | 252 |
| H | ? | lowering.rs | 257 |
| H | ? | lowering.rs | 260 |
| H | ? | lowering.rs | 280 |
| H | ? | lowering.rs | 283 |
| H | ? | lowering.rs | 317 |
| H | ? | lowering.rs | 352 |
| H | ? | lowering.rs | 353 |
| H | ? | lowering.rs | 357 |
| H | ? | lowering.rs | 413 |
| H | ? | lowering.rs | 483 |
| H | ? | lowering.rs | 492 |
| H | ? | lowering.rs | 507 |
| H | ? | lowering.rs | 508 |
| H | ? | lowering.rs | 512 |
| H | ? | lowering.rs | 632 |
| H | ? | lowering.rs | 722 |
| H | ? | lowering.rs | 760 |
| H | ? | lowering.rs | 775 |
| H | ? | lowering.rs | 776 |
| H | ? | lowering.rs | 806 |
| H | ? | lowering.rs | 901 |
| H | ? | lowering.rs | 913 |
| H | ? | lowering.rs | 914 |
| H | ? | lowering.rs | 927 |
| H | ? | lowering.rs | 934 |
| H | ? | lowering.rs | 936 |
| H | ? | lowering.rs | 937 |
| H | ? | requires_dist.rs | 85 |
| H | ? | requires_dist.rs | 154 |
| H | ? | requires_dist.rs | 155 |
| H | ? | requires_dist.rs | 175 |
| H | ? | requires_dist.rs | 176 |
| H | ? | requires_dist.rs | 197 |
| H | ? | requires_dist.rs | 218 |
| H | ? | requires_dist.rs | 252 |
| H | ? | requires_dist.rs | 253 |
| H | ? | requires_dist.rs | 263 |
| H | ? | requires_dist.rs | 264 |
| H | ? | requires_dist.rs | 273 |
| H | ? | requires_dist.rs | 274 |
| H | ? | requires_dist.rs | 285 |
| H | ? | requires_dist.rs | 286 |
| H | ? | requires_dist.rs | 381 |
| H | ? | requires_dist.rs | 394 |
| H | ? | requires_dist.rs | 395 |
| H | ? | requires_dist.rs | 396 |
| H | ? | requires_dist.rs | 397 |
| H | ? | requires_dist.rs | 398 |
| H | ? | requires_dist.rs | 428 |
| H | ? | requires_dist.rs | 430 |
| H | ? | requires_dist.rs | 431 |
| H | ? | requires_dist.rs | 432 |
| H | ? | dependency_groups.rs | 155 |
| H | ? | dependency_groups.rs | 156 |
| H | ? | dependency_groups.rs | 176 |
| H | ? | dependency_groups.rs | 177 |
| H | ? | dependency_groups.rs | 210 |
| H | ? | dependency_groups.rs | 211 |
| H | ? | dependency_groups.rs | 222 |
| H | ? | dependency_groups.rs | 223 |
| H | ? | registry_wheel_index.rs | 349 |
| H | ? | registry_wheel_index.rs | 391 |
| H | ? | built_wheel_index.rs | 349 |
| H | ? | mod.rs | 284 |
| H | ? | mod.rs | 447 |
| H | ? | mod.rs | 597 |
| H | ? | mod.rs | 598 |
| H | ? | mod.rs | 711 |
| H | ? | mod.rs | 844 |
| H | ? | mod.rs | 977 |
| H | ? | mod.rs | 997 |
| H | ? | mod.rs | 1003 |
| H | ? | mod.rs | 1022 |
| H | ? | mod.rs | 1311 |
| H | ? | mod.rs | 1432 |
| H | ? | mod.rs | 1492 |
| H | ? | mod.rs | 1548 |
| H | ? | mod.rs | 1571 |
| H | ? | mod.rs | 1600 |
| H | ? | mod.rs | 1636 |
| H | ? | mod.rs | 1667 |
| H | ? | mod.rs | 1686 |
| H | ? | mod.rs | 1737 |
| H | ? | mod.rs | 1745 |
| H | ? | mod.rs | 1845 |
| H | ? | mod.rs | 1955 |
| H | ? | mod.rs | 2122 |
| H | ? | mod.rs | 2181 |
| H | ? | mod.rs | 2314 |
| H | ? | mod.rs | 2350 |
| H | ? | mod.rs | 2388 |
| H | ? | mod.rs | 2416 |
| H | ? | mod.rs | 2445 |
| H | ? | mod.rs | 2483 |
| H | ? | mod.rs | 2514 |
| H | ? | mod.rs | 2571 |
| H | ? | mod.rs | 2752 |
| H | ? | mod.rs | 2774 |
| H | ? | mod.rs | 2784 |
| H | ? | mod.rs | 2786 |
| H | ? | mod.rs | 3001 |
| H | ? | mod.rs | 3049 |
| H | ? | mod.rs | 3140 |
| H | ? | mod.rs | 3150 |
| H | ? | mod.rs | 3161 |
| H | ? | mod.rs | 3162 |
| H | ? | mod.rs | 3490 |
| H | ? | mod.rs | 3491 |
| H | ? | mod.rs | 3497 |
| H | ? | mod.rs | 3499 |
| H | ? | mod.rs | 3500 |
| H | ? | mod.rs | 3512 |
| H | ? | mod.rs | 3513 |
| H | ? | mod.rs | 3519 |
| H | ? | mod.rs | 3520 |
| H | ? | lib.rs | 182 |
| H | ? | lib.rs | 293 |
| H | ? | lib.rs | 308 |
| H | ? | lib.rs | 316 |
| H | ? | lib.rs | 322 |
| H | ? | lib.rs | 324 |
| H | ? | lib.rs | 341 |
| H | ? | lib.rs | 420 |
| H | ? | lib.rs | 437 |
| H | ? | lib.rs | 521 |
| H | ? | lib.rs | 536 |
| H | ? | lib.rs | 538 |
| H | ? | lib.rs | 541 |
| H | ? | lib.rs | 545 |
| H | ? | lib.rs | 565 |
| H | ? | lib.rs | 568 |
| H | ? | lib.rs | 675 |
| H | ? | lib.rs | 676 |
| H | ? | lib.rs | 677 |
| H | ? | lib.rs | 142 |
| H | ? | lib.rs | 74 |
| H | ? | lib.rs | 78 |
| H | ? | lib.rs | 116 |
| H | ? | lib.rs | 125 |
| H | ? | lib.rs | 200 |
| H | ? | uv.rs | 275 |
| H | ? | uv.rs | 360 |
| H | ? | uv.rs | 370 |
| H | ? | uv.rs | 371 |
| H | ? | uv.rs | 382 |
| H | ? | uv.rs | 390 |
| H | ? | uv.rs | 391 |
| H | ? | uv.rs | 456 |
| H | ? | uv.rs | 494 |
| H | ? | uv.rs | 532 |
| H | ? | uv.rs | 539 |
| H | ? | uv.rs | 558 |
| H | ? | macos.rs | 59 |
| H | ? | macos.rs | 60 |
| H | ? | macos.rs | 78 |
| H | ? | macos.rs | 79 |
| H | ? | macos.rs | 96 |
| H | ? | macos.rs | 97 |
| H | ? | macos.rs | 116 |
| H | ? | macos.rs | 117 |
| H | ? | macos.rs | 136 |
| H | ? | macos.rs | 137 |
| H | ? | macos.rs | 171 |
| H | ? | macos.rs | 172 |
| H | ? | macos.rs | 181 |
| H | ? | error.rs | 86 |
| H | ? | mock.rs | 111 |
| H | ? | mock.rs | 128 |
| H | ? | secret_service.rs | 702 |
| H | ? | windows.rs | 132 |
| H | ? | windows.rs | 133 |
| H | ? | windows.rs | 134 |
| H | ? | windows.rs | 610 |
| H | ? | windows.rs | 612 |
| H | ? | windows.rs | 613 |
| H | ? | windows.rs | 614 |
| H | ? | windows.rs | 615 |
| H | ? | windows.rs | 694 |
| H | ? | glob.rs | 122 |
| H | ? | git_info.rs | 49 |
| H | ? | git_info.rs | 140 |
| H | ? | git_info.rs | 276 |
| H | ? | locked_file.rs | 232 |
| H | ? | link.rs | 118 |
| H | ? | link.rs | 377 |
| H | ? | link.rs | 516 |
| H | ? | link.rs | 613 |
| H | ? | link.rs | 614 |
| H | ? | link.rs | 849 |
| H | ? | link.rs | 1535 |
| H | ? | link.rs | 1536 |
| H | ? | lib.rs | 565 |
| H | ? | stream.rs | 142 |
| H | ? | stream.rs | 152 |
| H | ? | stream.rs | 163 |
| H | ? | stream.rs | 225 |
| H | ? | stream.rs | 240 |
| H | ? | stream.rs | 254 |
| H | ? | stream.rs | 270 |
| H | ? | stream.rs | 279 |
| H | ? | stream.rs | 297 |
| H | ? | stream.rs | 304 |
| H | ? | stream.rs | 314 |
| H | ? | stream.rs | 323 |
| H | ? | stream.rs | 332 |
| H | ? | stream.rs | 354 |
| H | ? | stream.rs | 413 |
| H | ? | stream.rs | 414 |
| H | ? | stream.rs | 421 |
| H | ? | stream.rs | 431 |
| H | ? | stream.rs | 442 |
| H | ? | stream.rs | 454 |
| H | ? | stream.rs | 478 |
| H | ? | stream.rs | 486 |
| H | ? | stream.rs | 558 |
| H | ? | sync.rs | 34 |
| H | ? | sync.rs | 35 |
| H | ? | sync.rs | 73 |
| H | ? | sync.rs | 116 |
| H | ? | sync.rs | 124 |
| H | ? | error.rs | 440 |
| H | ? | error.rs | 441 |
| H | ? | error.rs | 462 |
| H | ? | error.rs | 463 |
| H | ? | lib.rs | 357 |
| H | ? | lib.rs | 359 |
| H | ? | lib.rs | 370 |
| H | ? | lib.rs | 374 |
| H | ? | lib.rs | 399 |
| H | ? | lib.rs | 447 |
| H | ? | lib.rs | 538 |
| H | ? | lib.rs | 546 |
| H | ? | lib.rs | 558 |
| H | ? | lib.rs | 604 |
| H | ? | lib.rs | 680 |
| H | ? | lib.rs | 755 |
| H | ? | lib.rs | 765 |
| H | ? | lib.rs | 869 |
| H | ? | settings.rs | 2365 |
| H | ? | settings.rs | 2651 |
| H | ? | settings.rs | 2842 |
| H | ? | combine.rs | 256 |
| H | ? | combine.rs | 257 |
| H | ? | lib.rs | 134 |
| H | ? | lib.rs | 286 |
| H | ? | lib.rs | 946 |
| H | ? | backend.rs | 253 |
| H | ? | backend.rs | 254 |
| H | ? | backend.rs | 260 |
| H | ? | backend.rs | 267 |
| H | ? | unnamed.rs | 306 |
| H | ? | unnamed.rs | 316 |
| H | ? | specification.rs | 144 |
| H | ? | specification.rs | 147 |
| H | ? | specification.rs | 162 |
| H | ? | specification.rs | 167 |
| H | ? | specification.rs | 173 |
| H | ? | specification.rs | 181 |
| H | ? | specification.rs | 188 |
| H | ? | specification.rs | 196 |
| H | ? | specification.rs | 257 |
| H | ? | specification.rs | 263 |
| H | ? | specification.rs | 302 |
| H | ? | specification.rs | 308 |
| H | ? | specification.rs | 311 |
| H | ? | specification.rs | 334 |
| H | ? | specification.rs | 344 |
| H | ? | specification.rs | 354 |
| H | ? | specification.rs | 366 |
| H | ? | specification.rs | 369 |
| H | ? | specification.rs | 491 |
| H | ? | specification.rs | 496 |
| H | ? | specification.rs | 519 |
| H | ? | specification.rs | 524 |
| H | ? | specification.rs | 583 |
| H | ? | specification.rs | 584 |
| H | ? | specification.rs | 622 |
| H | ? | specification.rs | 623 |
| H | ? | specification.rs | 649 |
| H | ? | specification.rs | 650 |
| H | ? | specification.rs | 752 |
| H | ? | lookahead.rs | 93 |
| H | ? | lookahead.rs | 101 |
| H | ? | lookahead.rs | 107 |
| H | ? | lookahead.rs | 108 |
| H | ? | lookahead.rs | 136 |
| H | ? | lookahead.rs | 175 |
| H | ? | lookahead.rs | 184 |
| H | ? | lookahead.rs | 196 |
| H | ? | lookahead.rs | 197 |
| H | ? | lookahead.rs | 215 |
| H | ? | source_tree.rs | 133 |
| H | ? | source_tree.rs | 150 |
| H | ? | source_tree.rs | 227 |
| H | ? | source_tree.rs | 233 |
| H | ? | extras.rs | 94 |
| H | ? | extras.rs | 102 |
| H | ? | lib.rs | 70 |
| H | ? | lib.rs | 71 |
| H | ? | lib.rs | 72 |
| H | ? | lib.rs | 73 |
| H | ? | lib.rs | 81 |
| H | ? | lib.rs | 82 |
| H | ? | lib.rs | 83 |
| H | ? | lib.rs | 84 |
| H | ? | lib.rs | 92 |
| H | ? | lib.rs | 93 |
| H | ? | lib.rs | 94 |
| H | ? | lib.rs | 95 |
| H | ? | lib.rs | 102 |
| H | ? | lib.rs | 109 |
| H | ? | lib.rs | 110 |
| H | ? | osv.rs | 250 |
| H | ? | osv.rs | 285 |
| H | ? | osv.rs | 299 |
| H | ? | osv.rs | 330 |
| H | ? | osv.rs | 333 |
| H | ? | osv.rs | 379 |
| H | ? | osv.rs | 396 |
| H | ? | osv.rs | 413 |
| H | ? | osv.rs | 449 |
| H | ? | osv.rs | 490 |
| H | ? | project_status.rs | 48 |
| H | ? | project_status.rs | 52 |
| H | ? | project_status.rs | 108 |
| H | ? | lowering.rs | 191 |
| H | ? | tree.rs | 312 |
| H | ? | tree.rs | 315 |
| H | ? | tree.rs | 326 |
| H | ? | tree.rs | 327 |
| H | ? | tree.rs | 335 |
| H | ? | tree.rs | 336 |
| H | ? | tree.rs | 1189 |
| H | ? | tree.rs | 3670 |
| H | ? | tree.rs | 3675 |
| H | ? | tree.rs | 3682 |
| H | ? | algebra.rs | 155 |
| H | ? | algebra.rs | 396 |
| H | ? | algebra.rs | 401 |
| H | ? | algebra.rs | 406 |
| H | ? | algebra.rs | 553 |
| H | ? | algebra.rs | 595 |
| H | ? | algebra.rs | 641 |
| H | ? | algebra.rs | 697 |
| H | ? | algebra.rs | 728 |
| H | ? | algebra.rs | 762 |
| H | ? | algebra.rs | 776 |
| H | ? | algebra.rs | 797 |
| H | ? | algebra.rs | 844 |
| H | ? | algebra.rs | 911 |
| H | ? | algebra.rs | 980 |
| H | ? | algebra.rs | 987 |
| H | ? | algebra.rs | 994 |
| H | ? | algebra.rs | 1432 |
| H | ? | algebra.rs | 1575 |
| H | ? | algebra.rs | 1887 |
| H | ? | simplify.rs | 48 |
| H | ? | simplify.rs | 59 |
| H | ? | simplify.rs | 103 |
| H | ? | simplify.rs | 118 |
| H | ? | simplify.rs | 168 |
| H | ? | simplify.rs | 190 |
| H | ? | simplify.rs | 333 |
| H | ? | simplify.rs | 385 |
| H | ? | unnamed.rs | 381 |
| H | ? | unnamed.rs | 392 |
| H | ? | verbatim_url.rs | 141 |
| H | ? | verbatim_url.rs | 142 |
| H | ? | verbatim_url.rs | 182 |
| H | ? | verbatim_url.rs | 277 |
| H | ? | cursor.rs | 45 |
| H | ? | cursor.rs | 50 |
| H | ? | cursor.rs | 85 |
| H | ? | lib.rs | 452 |
| H | ? | lib.rs | 728 |
| H | ? | lib.rs | 739 |
| H | ? | lib.rs | 944 |
| H | ? | lib.rs | 972 |
| H | ? | options_metadata.rs | 51 |
| H | ? | options_metadata.rs | 401 |
| H | ? | server.rs | 139 |
| H | ? | server.rs | 143 |
| H | ? | server.rs | 159 |
| H | ? | server.rs | 163 |
| H | ? | server.rs | 170 |
| H | ? | wheel.rs | 61 |
| H | ? | wheel.rs | 167 |
| H | ? | find_links.rs | 49 |
| H | ? | lib.rs | 779 |
| H | ? | lib.rs | 798 |
| H | ? | lib.rs | 804 |
| H | ? | wheel.rs | 219 |
| H | ? | wheel.rs | 624 |
| H | ? | linker.rs | 70 |
| H | ? | linker.rs | 184 |
| H | ? | install.rs | 77 |
| H | ? | install.rs | 80 |
| H | ? | install.rs | 81 |
| H | ? | script.rs | 112 |
| H | ? | main.rs | 16 |
| H | ? | version.rs | 658 |
| H | ? | version.rs | 2464 |
| H | ? | version_specifier.rs | 99 |
| H | ? | version_specifier.rs | 575 |
| H | ? | version_specifier.rs | 606 |
| H | ? | version_specifier.rs | 609 |
| H | ? | version_specifier.rs | 619 |
| H | ? | version_specifier.rs | 622 |
| H | ? | version_specifier.rs | 641 |
| H | ? | version_specifier.rs | 736 |
| H | ? | version_specifier.rs | 862 |
| H | ? | version_specifier.rs | 1032 |
| H | ? | version_ranges.rs | 67 |
| H | ? | version_ranges.rs | 145 |
| H | ? | version_ranges.rs | 160 |
| H | ? | version_ranges.rs | 168 |
| H | ? | version_ranges.rs | 202 |
| H | ? | version_ranges.rs | 260 |
| H | ? | version_ranges.rs | 277 |
| H | ? | version_ranges.rs | 358 |
| H | ? | version_ranges.rs | 370 |
| H | ? | version_ranges.rs | 426 |
| H | ? | version_ranges.rs | 429 |
| H | ? | version_ranges.rs | 569 |
| H | ? | version_ranges.rs | 571 |
| H | ? | version_ranges.rs | 688 |
| H | ? | version_ranges.rs | 787 |
| H | ? | version_ranges.rs | 890 |
| H | ? | line_wrap.rs | 77 |
| H | ? | package_name.rs | 75 |

---
*Сгенерировано GSC v0.6 · 2026-07-15T04:02:32.624985*