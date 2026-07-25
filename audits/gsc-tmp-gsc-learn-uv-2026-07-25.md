---
title: "GSC Audit: /tmp/gsc-learn/uv"
date: 2026-07-25
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/uv

**Дата:** 25.07.2026 04:03  
**Путь:** `/tmp/gsc-learn/uv`  
**Всего находок:** 3496  
**CRITICAL:** 53 | **HIGH:** 3156 | **MEDIUM:** 100 | **LOW:** 186

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 3046 |
| GS003 | 184 |
| Хардкод IP адреса | 104 |
| Синхронный код в async | 47 |
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
| CRITICAL | GS001 | registry_client.rs | 2090 | Found: password = "password" |
| CRITICAL | GS001 | registry_client.rs | 2146 | Found: password = "password" |
| CRITICAL | GS001 | registry_client.rs | 2196 | Found: password = "password" |
| CRITICAL | GS001 | mock.rs | 246 | Found: password = "test ascii password" |
| CRITICAL | GS001 | secret_service.rs | 64 | Found: Password: " pass
    echo -n " |
| CRITICAL | GS001 | secret_service.rs | 771 | Found: password = "password in new collection" |
| CRITICAL | GS001 | windows.rs | 751 | Found: password = "test get password" |
| CRITICAL | ? | registry_client.rs | 2090 | Match:         let password = "password"; |
| CRITICAL | ? | registry_client.rs | 2146 | Match:         let password = "password"; |
| CRITICAL | ? | registry_client.rs | 2196 | Match:         let password = "password"; |
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
| HIGH | ? | pyproject_mut.rs | 2069 | Match:             ("0.0.0.1", "==0.0.0.1"), |
| HIGH | ? | pyproject_mut.rs | 2073 | Match:             ("1.2.3.4", "==1.2.3.4"), |
| HIGH | ? | pyproject_mut.rs | 2074 | Match:             ("1.2.3.4a1.post1", "==1.2.3.4a1.post1"), |
| HIGH | ? | pyproject_mut.rs | 2093 | Match:             ("0.0.0.1", ">=0.0.0.1"), |
| HIGH | ? | pyproject_mut.rs | 2098 | Match:             ("1.2.3.4", ">=1.2.3.4"), |
| HIGH | ? | pyproject_mut.rs | 2099 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1"), |
| HIGH | ? | pyproject_mut.rs | 2116 | Match:             ("0.0.0.0", ">=0.0.0.0, <0.1.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2119 | Match:             ("0.0.1.1", ">=0.0.1.1, <0.0.2.0"), |
| HIGH | ? | pyproject_mut.rs | 2120 | Match:             ("0.0.0.1", ">=0.0.0.1, <0.0.0.2"), |
| HIGH | ? | pyproject_mut.rs | 2125 | Match:             ("1.2.3.4", ">=1.2.3.4, <2.0.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2126 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1, < |
| HIGH | ? | pyproject_mut.rs | 2143 | Match:             ("0.0.0.0", ">=0.0.0.0, <0.0.1.0"), |
| HIGH | ? | pyproject_mut.rs | 2146 | Match:             ("0.0.1.1", ">=0.0.1.1, <0.0.2.0"), |
| HIGH | ? | pyproject_mut.rs | 2147 | Match:             ("0.0.0.1", ">=0.0.0.1, <0.0.0.2"), |
| HIGH | ? | pyproject_mut.rs | 2152 | Match:             ("1.2.3.4", ">=1.2.3.4, <1.3.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2153 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1, < |
| HIGH | ? | self_update.rs | 857 | Match:         let listener = TcpListener::bind("127.0.0.1:0 |
| HIGH | ? | keyring.rs | 618 | Match:         let url = Url::parse("http://127.0.0.1:8080/b |
| HIGH | ? | keyring.rs | 619 | Match:         let keyring = KeyringProvider::dummy([("http: |
| HIGH | ? | keyring.rs | 635 | Match:         let url = Url::parse("https://127.0.0.1:8080/ |
| HIGH | ? | keyring.rs | 636 | Match:         let keyring = KeyringProvider::dummy([("http: |
| HIGH | ? | service.rs | 35 | Match:             "http" if matches!(url.host_str(), Some(" |
| HIGH | ? | path.rs | 911 | Match:                 r"\\127.0.0.1\c$\path\to\logging.", |
| HIGH | ? | path.rs | 912 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 915 | Match:                 r"\\127.0.0.1\c$\path\to\.\logging.", |
| HIGH | ? | path.rs | 916 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 919 | Match:                 r"\\127.0.0.1\c$\path\to\..\to\loggin |
| HIGH | ? | path.rs | 920 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 923 | Match:                 r"//127.0.0.1/c$/path/to/../to/./logg |
| HIGH | ? | path.rs | 924 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 930 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | path.rs | 931 | Match:                 r"\\?\UNC\127.0.0.1\c$\path\to\loggin |
| HIGH | ? | settings.rs | 419 | Match:             no-proxy = ["localhost", "127.0.0.1"] |
| HIGH | ? | tree.rs | 2784 | Match:             ("3.9.0.0.*", "3.9", "3.9.*"), |
| HIGH | ? | tree.rs | 2801 | Match:         let cases_false = ["3.9.1.*", "3.9.1.0.*", "3 |
| HIGH | ? | vendor.rs | 61 | Match:         url: "https://github.com/astral-sh/futzed-whe |
| HIGH | ? | vendor.rs | 67 | Match:         url: "https://github.com/astral-sh/futzed-whe |
| HIGH | ? | version.rs | 3609 | Match:         assert_eq!(p("1.2.3.4"), Version::new([1, 2,  |
| HIGH | ? | version.rs | 3610 | Match:         assert_eq!(p("1.2.3.4.5"), Version::new([1, 2 |
| HIGH | ? | version.rs | 4338 | Match:             "1!2.3.0.0" |
| HIGH | ? | version.rs | 4420 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4425 | Match:         assert_eq!(version.to_string().as_str(), "2.0 |
| HIGH | ? | version.rs | 4428 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4435 | Match:         assert_eq!(version.to_string().as_str(), "5!2 |
| HIGH | ? | version.rs | 4440 | Match:         assert_eq!(version.to_string().as_str(), "5!3 |
| HIGH | ? | version.rs | 4472 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4477 | Match:         assert_eq!(version.to_string().as_str(), "1.3 |
| HIGH | ? | version.rs | 4480 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4487 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4492 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4524 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4529 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4532 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4539 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4544 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4576 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4581 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4584 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4591 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4596 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4628 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4633 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4636 | Match:         let mut version = "5!1.7.3.5a2.post345.dev456 |
| HIGH | ? | version.rs | 4643 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4648 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4680 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4685 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4688 | Match:         let mut version = "5!1.7.3.5b2.post345.dev456 |
| HIGH | ? | version.rs | 4695 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4700 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4723 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4725 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4728 | Match:         let mut version = "5!1.7.3.5b2.dev123+local". |
| HIGH | ? | version.rs | 4730 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4732 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4755 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4757 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4760 | Match:         let mut version = "5!1.7.3.5b2.post345+local" |
| HIGH | ? | version.rs | 4764 | Match:             "5!1.7.3.5b2.post345.dev1+local" |
| HIGH | ? | version.rs | 4769 | Match:             "5!1.7.3.5b2.post345.dev2+local" |
| HIGH | ? | version.rs | 4793 | Match:         let mut version = "1.2.3.4".parse::<Version>( |
| HIGH | ? | version.rs | 4795 | Match:         assert_eq!(version.to_string().as_str(), "1.2 |
| HIGH | ? | version.rs | 4798 | Match:         let mut version = "5!1.7.3.5b2.post345+local" |
| HIGH | ? | version.rs | 4800 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
| HIGH | ? | version.rs | 4802 | Match:         assert_eq!(version.to_string().as_str(), "5!1 |
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
| HIGH | ? | candidate_selector.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | candidate_selector.rs | 801 | Clone in performance-critical code — consider references |
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
| HIGH | ? | universal_marker.rs | 840 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 532 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 628 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 629 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 670 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 672 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 699 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 712 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1493 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1547 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1653 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1668 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1787 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1805 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1874 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2009 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2063 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2070 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2074 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2095 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2096 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2194 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2205 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2279 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2285 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2290 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2677 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2816 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2834 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2895 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2898 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2956 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2977 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2989 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2992 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2997 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3006 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3021 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3028 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3029 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3034 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3039 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3047 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3054 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3061 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3081 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3092 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3096 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3100 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3104 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3109 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3115 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3155 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3165 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3166 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3177 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3189 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3218 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3227 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3236 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3237 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3242 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3245 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3252 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3253 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3257 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3260 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3270 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3279 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3280 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3284 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3286 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3305 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3306 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3311 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3315 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3323 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3328 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3338 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3339 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3361 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3377 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3378 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3386 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3390 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3398 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3414 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3415 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3523 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3527 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3529 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3541 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3600 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3658 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3662 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3663 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3676 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3743 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3745 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3781 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3785 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3791 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3799 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3925 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4003 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4028 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4047 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4051 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4209 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4628 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4646 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4664 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4742 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4951 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4996 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5004 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5009 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5017 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5022 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5032 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5038 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5051 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5061 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5078 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5101 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5111 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5203 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5391 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5538 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5549 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5557 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5558 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5582 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5593 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5601 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5602 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5708 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5709 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5842 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5866 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5882 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5886 | Clone in performance-critical code — consider references |
| HIGH | ? | serialize.rs | 120 | Clone in performance-critical code — consider references |
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
| HIGH | ? | metadata.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 606 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 626 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 790 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 791 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 792 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1018 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1116 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1132 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1243 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1248 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1265 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1266 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1273 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1274 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1334 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1350 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1362 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1374 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1386 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1409 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1413 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1421 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1422 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1426 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1428 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1433 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1435 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1436 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1450 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 1462 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 508 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 566 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 592 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 602 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 731 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 842 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 848 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 861 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 883 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 887 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 898 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 926 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 948 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1080 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1082 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1090 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1091 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1107 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1111 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1119 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1123 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1126 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1130 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1134 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1139 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1142 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1160 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1180 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1229 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1243 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1246 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1249 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1251 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1254 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1260 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1407 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1412 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1428 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1435 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1440 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1461 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1465 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1474 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1482 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1515 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1531 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1536 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1543 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1550 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1561 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1562 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1566 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1568 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1582 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1588 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1592 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1622 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1626 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1635 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1643 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1653 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1676 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1697 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1708 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1716 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1717 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1722 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1723 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1724 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1726 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1731 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1743 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1751 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1756 | Clone in performance-critical code — consider references |
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
| HIGH | ? | version_map.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 708 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 722 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 767 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 813 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 141 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | python_requirement.rs | 147 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 585 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 794 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 831 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 835 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 838 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 974 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 977 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1034 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1095 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1099 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1108 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1110 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1115 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1165 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1166 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1167 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1215 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1220 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1265 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1311 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1325 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1333 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1335 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1372 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1385 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1402 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1404 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1410 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1434 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1442 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1449 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1455 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1461 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1492 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1495 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1538 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1581 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1636 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1683 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1684 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1751 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1807 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1809 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1812 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1814 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1842 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1843 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1851 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1875 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1884 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1987 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2007 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2030 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2033 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2041 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2043 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2052 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2109 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2114 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2137 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2142 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2165 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2168 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2248 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2269 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2270 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2271 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2272 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2273 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2301 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2303 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2304 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2305 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2351 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2454 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2455 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2456 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2457 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2458 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2491 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2492 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2493 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2494 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2495 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2640 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2669 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2670 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2685 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2686 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2710 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2717 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2724 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2770 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2776 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2780 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2839 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2851 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2860 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2893 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2906 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2908 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2934 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2943 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2946 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2971 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2994 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3001 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3014 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3018 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3019 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3020 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3021 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3028 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3029 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3030 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3302 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3303 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3307 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3313 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3333 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3430 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3444 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3569 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3575 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3578 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3579 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3601 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3606 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3607 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3633 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3638 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3639 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3642 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3651 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3656 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3657 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3683 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3688 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3689 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3693 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3717 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3718 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3719 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3841 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3933 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4002 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4031 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4050 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4071 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4077 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4088 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4095 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4135 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4192 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4204 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4416 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 996 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 998 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 170 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 208 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 604 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 616 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 677 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 740 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 747 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | cached_client.rs | 785 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 486 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 617 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 623 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 628 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 635 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 650 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 663 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 682 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 689 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 701 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 735 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 761 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 820 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 825 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 832 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 841 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 847 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 853 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 859 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 865 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 871 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 877 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 892 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 897 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 920 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 965 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 984 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1018 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1063 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1074 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1096 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1128 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1135 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1143 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1146 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1207 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1214 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1220 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1239 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1241 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1242 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1245 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1265 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1281 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1293 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1303 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1375 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1574 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1645 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1710 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1778 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1796 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1797 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1826 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 2125 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 2175 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 2225 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 476 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 486 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 491 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 542 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 687 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 689 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 699 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 701 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 792 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 942 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1077 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1183 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1189 | Clone in performance-critical code — consider references |
| HIGH | ? | retry.rs | 149 | Clone in performance-critical code — consider references |
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
| HIGH | ? | dependency_groups.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | extras.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | extras.rs | 116 | Clone in performance-critical code — consider references |
| HIGH | ? | proxy_url.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | proxy_url.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | libc.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | libc.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | libc.rs | 357 | Clone in performance-critical code — consider references |
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
| HIGH | ? | workspace.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 678 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 692 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 698 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 771 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 842 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 856 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 870 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1068 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1073 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1081 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1155 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1157 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1159 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1160 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1161 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1167 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1177 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1180 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1191 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1196 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1298 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1324 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1336 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1338 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1345 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1364 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1512 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1568 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1573 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1606 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1609 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1674 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1704 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1705 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1717 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1718 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1728 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1746 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1750 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1754 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1764 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1776 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1785 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1790 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1849 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 1876 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2052 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2056 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2065 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2089 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2092 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2093 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2101 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2109 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2112 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2121 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2137 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2141 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2196 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2197 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2198 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2200 | Clone in performance-critical code — consider references |
| HIGH | ? | workspace.rs | 2298 | Clone in performance-critical code — consider references |
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
| HIGH | ? | pyproject_mut.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 524 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 546 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 565 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 587 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 590 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1403 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1549 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1575 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1589 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1595 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1682 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1709 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1699 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1700 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1706 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1707 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1708 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1834 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1847 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1873 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1886 | Clone in performance-critical code — consider references |
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
| HIGH | ? | conflicts.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 602 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 722 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 727 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 729 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 739 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 740 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 867 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 868 | Clone in performance-critical code — consider references |
| HIGH | ? | conflicts.rs | 885 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1117 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1120 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1123 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1615 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6758 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6759 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6760 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6821 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6822 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6823 | Clone in performance-critical code — consider references |
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
| HIGH | ? | index_url.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 544 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 681 | Clone in performance-critical code — consider references |
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
| HIGH | ? | index.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 587 | Clone in performance-critical code — consider references |
| HIGH | ? | index.rs | 595 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 812 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 823 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 845 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 846 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 856 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 857 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 866 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 867 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 877 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 878 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 888 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1035 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1068 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1069 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1431 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1435 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1784 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 1038 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1045 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1065 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1133 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1232 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1238 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1239 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1274 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1321 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1335 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1361 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1365 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1406 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1416 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1420 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1630 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1694 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1769 | Clone in performance-critical code — consider references |
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
| HIGH | ? | venv.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | venv.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | venv.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | venv.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 428 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 614 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 626 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 630 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 648 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 671 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 768 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1164 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1165 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1170 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1171 | Clone in performance-critical code — consider references |
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
| HIGH | ? | common.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 437 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 791 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 806 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 815 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 819 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 825 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 939 | Clone in performance-critical code — consider references |
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
| HIGH | ? | install.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 168 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 227 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 285 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 592 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 618 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 635 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 763 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 793 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 795 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 802 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 803 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 804 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 805 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 808 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 914 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 969 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 322 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 324 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 374 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 485 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 609 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 642 | Clone in performance-critical code — consider references |
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
| HIGH | ? | install.rs | 328 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 647 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 652 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 723 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1021 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1036 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1039 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1041 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1088 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1161 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1175 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1183 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1197 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1200 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1202 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1207 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1218 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1226 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | help.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 378 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 430 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 448 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 652 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 680 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 687 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 688 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 693 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 694 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 993 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1006 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1013 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1217 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1234 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1629 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1682 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1725 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1731 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2299 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2315 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2324 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2325 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2327 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2338 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2342 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2356 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2368 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2378 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2379 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2381 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2382 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2394 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2505 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2550 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2557 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2558 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2560 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2570 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2583 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2585 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2604 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2636 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2648 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2658 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2659 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2661 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2662 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2736 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2745 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2746 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2778 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2790 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2800 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2804 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2908 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2993 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3000 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3001 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3003 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3021 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3023 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3055 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3065 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3066 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3068 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3069 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3086 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3091 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3212 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3216 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3218 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3251 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3256 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3258 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3453 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | ty.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 361 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 366 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 446 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 127 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 689 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 702 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 704 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 705 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 706 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 708 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 712 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 713 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 714 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 735 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 747 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 748 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 858 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 859 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 899 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 909 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 910 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 912 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1005 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1017 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1052 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1076 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1102 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1125 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1129 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1147 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1155 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1203 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 1573 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 228 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 390 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 780 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 783 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 788 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 795 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 796 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 811 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 832 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 833 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 856 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 902 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 903 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 905 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 906 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1052 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1053 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1069 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1654 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 129 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 130 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 132 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 136 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 318 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 414 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 416 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 426 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 732 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 739 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 747 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 764 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 802 | Clone in performance-critical code — consider references |
| HIGH | ? | toolchain.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | toolchain.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1051 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1349 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1446 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1547 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1552 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1557 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1588 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1599 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1613 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1626 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1780 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1784 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1811 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1815 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 408 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 472 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 477 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 734 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 767 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 768 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 938 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 965 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 973 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 974 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 975 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 983 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 989 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 993 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 994 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 1163 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 1298 | Clone in performance-critical code — consider references |
| HIGH | ? | add.rs | 1446 | Clone in performance-critical code — consider references |
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
| HIGH | ? | environment.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 282 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | environment.rs | 421 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 41 | Clone in performance-critical code — consider references |
| HIGH | ? | editable.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 107 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 376 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 437 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 496 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 765 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 766 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 816 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 960 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 965 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 968 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1085 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1090 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1093 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1234 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1251 | Clone in performance-critical code — consider references |
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
| HIGH | ? | settings.rs | 1946 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2020 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2021 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2072 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2073 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2078 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2128 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2129 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2305 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2350 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2510 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2511 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2602 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2603 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2699 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2700 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2724 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2841 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2842 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2887 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3040 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3041 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3080 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3153 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3154 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3159 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3185 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3190 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3236 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3242 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3341 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3357 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3366 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3378 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3386 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3646 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3662 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3671 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4109 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4115 | Clone in performance-critical code — consider references |
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
| HIGH | ? | settings.rs | 5189 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 125 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 302 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 477 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 635 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 643 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 742 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 818 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 860 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 861 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 906 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1004 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1017 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1031 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1032 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1067 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1303 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1371 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1372 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1506 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1540 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1541 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1631 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1632 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1633 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1661 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2056 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2057 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2170 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2299 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2300 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2370 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2371 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2427 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2428 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2475 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2546 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2559 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2573 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2574 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2642 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2643 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2697 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2698 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2868 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2869 | Clone in performance-critical code — consider references |
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
| HIGH | ? | interpreter.rs | 1228 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 1040 | Clone in performance-critical code — consider references |
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
| HIGH | ? | virtualenv.rs | 231 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 245 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 248 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 251 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 131 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 896 | Clone in performance-critical code — consider references |
| HIGH | ? | generate_scenarios.rs | 911 | Clone in performance-critical code — consider references |
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
| HIGH | ? | build_requires.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | build_requires.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 118 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 147 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 273 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 312 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 373 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 488 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 492 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 627 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 755 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 770 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 771 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 836 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 875 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 883 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 998 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 1010 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 1011 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 1024 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 1031 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 1033 | Clone in performance-critical code — consider references |
| HIGH | ? | lowering.rs | 1034 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 201 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 225 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 268 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 385 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 401 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 435 | Clone in performance-critical code — consider references |
| HIGH | ? | requires_dist.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 177 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 209 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 210 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | dependency_groups.rs | 222 | Clone in performance-critical code — consider references |
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
| HIGH | ? | error.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 423 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 445 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 683 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 758 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 768 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 872 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2367 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2653 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2875 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2876 | Clone in performance-critical code — consider references |
| HIGH | ? | combine.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | combine.rs | 257 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 951 | Clone in performance-critical code — consider references |
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
| HIGH | ? | specification.rs | 517 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 522 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 573 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 612 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 639 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 742 | Clone in performance-critical code — consider references |
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
| HIGH | ? | osv.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 287 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 332 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 381 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 415 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 451 | Clone in performance-critical code — consider references |
| HIGH | ? | osv.rs | 499 | Clone in performance-critical code — consider references |
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
| HIGH | ? | verbatim_url.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 301 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 774 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 793 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | linker.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | linker.rs | 184 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 77 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 81 | Clone in performance-critical code — consider references |
| HIGH | ? | script.rs | 131 | Clone in performance-critical code — consider references |
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
| M | ? | resolver.py | 224 |
| M | ? | resolver.py | 267 |
| M | ? | resolver.py | 448 |
| M | ? | resolver.py | 460 |
| M | ? | resolver.py | 504 |
| M | ? | resolver.py | 516 |
| M | ? | resolver.py | 541 |
| M | ? | resolver.py | 553 |
| M | ? | resolver.py | 586 |
| M | ? | resolver.py | 597 |
| M | ? | resolver.py | 705 |
| M | ? | resolver.py | 715 |
| M | ? | resolver.py | 750 |
| M | ? | resolver.py | 760 |
| M | ? | resolver.py | 780 |
| M | ? | resolver.py | 790 |
| M | ? | resolver.py | 815 |
| M | ? | resolver.py | 825 |
| M | ? | resolver.py | 925 |
| M | ? | resolver.py | 1110 |
| M | ? | resolver.py | 1120 |
| M | ? | resolver.py | 1158 |
| M | ? | resolver.py | 1168 |
| M | ? | resolver.py | 1191 |
| M | ? | resolver.py | 1201 |
| M | ? | resolver.py | 1229 |
| M | ? | resolver.py | 1239 |
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
| C | GS001 | registry_client.rs | 2090 |
| C | GS001 | registry_client.rs | 2146 |
| C | GS001 | registry_client.rs | 2196 |
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
| L | GS003 | create-python-mirror.py | 281 |
| L | GS003 | create-python-mirror.py | 283 |
| L | GS003 | create-python-mirror.py | 285 |
| L | GS003 | create-python-mirror.py | 286 |
| L | GS003 | patch-dist-manifest-checksums.py | 47 |
| L | GS003 | patch-dist-manifest-checksums.py | 59 |
| L | GS003 | patch-dist-manifest-checksums.py | 66 |
| L | GS003 | publish-crates.py | 105 |
| L | GS003 | publish-crates.py | 128 |
| L | GS003 | publish-crates.py | 130 |
| L | GS003 | publish-crates.py | 133 |
| L | GS003 | registries-test.py | 131 |
| L | GS003 | registries-test.py | 184 |
| L | GS003 | registries-test.py | 188 |
| L | GS003 | registries-test.py | 191 |
| L | GS003 | registries-test.py | 234 |
| L | GS003 | registries-test.py | 242 |
| L | GS003 | registries-test.py | 244 |
| L | GS003 | registries-test.py | 245 |
| L | GS003 | registries-test.py | 248 |
| L | GS003 | registries-test.py | 253 |
| L | GS003 | registries-test.py | 255 |
| L | GS003 | registries-test.py | 257 |
| L | GS003 | registries-test.py | 261 |
| L | GS003 | registries-test.py | 263 |
| L | GS003 | registries-test.py | 335 |
| L | GS003 | registries-test.py | 339 |
| L | GS003 | registries-test.py | 340 |
| L | GS003 | registries-test.py | 358 |
| L | GS003 | registries-test.py | 361 |
| L | GS003 | registries-test.py | 366 |
| L | GS003 | registries-test.py | 371 |
| L | GS003 | registries-test.py | 401 |
| L | GS003 | registries-test.py | 404 |
| L | GS003 | registries-test.py | 406 |
| L | GS003 | registries-test.py | 408 |
| L | GS003 | registries-test.py | 410 |
| L | GS003 | registries-test.py | 412 |
| L | GS003 | registries-test.py | 414 |
| L | GS003 | registries-test.py | 415 |
| L | GS003 | registries-test.py | 419 |
| L | GS003 | registries-test.py | 423 |
| L | GS003 | registries-test.py | 424 |
| L | GS003 | registries-test.py | 428 |
| L | GS003 | registries-test.py | 429 |
| L | GS003 | registries-test.py | 430 |
| L | GS003 | registries-test.py | 431 |
| L | GS003 | registries-test.py | 434 |
| L | GS003 | repair-sdist-cargo-lock.py | 26 |
| L | GS003 | repair-sdist-cargo-lock.py | 37 |
| L | GS003 | repair-sdist-cargo-lock.py | 48 |
| L | GS003 | repair-sdist-cargo-lock.py | 56 |
| L | GS003 | repair-sdist-cargo-lock.py | 64 |
| L | GS003 | repair-sdist-cargo-lock.py | 72 |
| L | GS003 | repair-sdist-cargo-lock.py | 77 |
| L | GS003 | repair-sdist-cargo-lock.py | 80 |
| L | GS003 | repair-sdist-cargo-lock.py | 83 |
| L | GS003 | reverse-changelog.py | 37 |
| L | GS003 | reverse-changelog.py | 51 |
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
| L | GS003 | settings.rs | 5176 |
| L | GS003 | lib.rs | 1321 |
| L | GS003 | build.rs | 23 |
| L | GS003 | build.rs | 41 |
| L | GS003 | build.rs | 54 |
| L | GS003 | build.rs | 73 |
| L | GS003 | build.rs | 74 |
| L | GS003 | build.rs | 79 |
| L | GS003 | build.rs | 85 |
| L | GS003 | build.rs | 91 |
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
| L | GS003 | generate_preview_features_reference.rs | 28 |
| L | GS003 | generate_preview_features_reference.rs | 38 |
| L | GS003 | generate_preview_features_reference.rs | 43 |
| L | GS003 | generate_scenarios.rs | 80 |
| L | GS003 | generate_scenarios.rs | 95 |
| L | GS003 | generate_scenarios.rs | 97 |
| L | GS003 | generate_scenarios.rs | 102 |
| L | GS003 | generate_scenarios.rs | 223 |
| L | GS003 | generate_scenarios.rs | 286 |
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
| L | GS003 | lib.rs | 2187 |
| L | GS003 | lib.rs | 2188 |
| L | GS003 | lib.rs | 2193 |
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
| H | ? | pyproject_mut.rs | 2069 |
| H | ? | pyproject_mut.rs | 2073 |
| H | ? | pyproject_mut.rs | 2074 |
| H | ? | pyproject_mut.rs | 2093 |
| H | ? | pyproject_mut.rs | 2098 |
| H | ? | pyproject_mut.rs | 2099 |
| H | ? | pyproject_mut.rs | 2116 |
| H | ? | pyproject_mut.rs | 2119 |
| H | ? | pyproject_mut.rs | 2120 |
| H | ? | pyproject_mut.rs | 2125 |
| H | ? | pyproject_mut.rs | 2126 |
| H | ? | pyproject_mut.rs | 2143 |
| H | ? | pyproject_mut.rs | 2146 |
| H | ? | pyproject_mut.rs | 2147 |
| H | ? | pyproject_mut.rs | 2152 |
| H | ? | pyproject_mut.rs | 2153 |
| H | ? | self_update.rs | 857 |
| H | ? | keyring.rs | 618 |
| H | ? | keyring.rs | 619 |
| H | ? | keyring.rs | 635 |
| H | ? | keyring.rs | 636 |
| H | ? | service.rs | 35 |
| H | ? | path.rs | 911 |
| H | ? | path.rs | 912 |
| H | ? | path.rs | 915 |
| H | ? | path.rs | 916 |
| H | ? | path.rs | 919 |
| H | ? | path.rs | 920 |
| H | ? | path.rs | 923 |
| H | ? | path.rs | 924 |
| H | ? | path.rs | 930 |
| H | ? | path.rs | 931 |
| H | ? | settings.rs | 419 |
| H | ? | tree.rs | 2784 |
| H | ? | tree.rs | 2801 |
| H | ? | vendor.rs | 61 |
| H | ? | vendor.rs | 67 |
| H | ? | version.rs | 3609 |
| H | ? | version.rs | 3610 |
| H | ? | version.rs | 4338 |
| H | ? | version.rs | 4420 |
| H | ? | version.rs | 4425 |
| H | ? | version.rs | 4428 |
| H | ? | version.rs | 4435 |
| H | ? | version.rs | 4440 |
| H | ? | version.rs | 4472 |
| H | ? | version.rs | 4477 |
| H | ? | version.rs | 4480 |
| H | ? | version.rs | 4487 |
| H | ? | version.rs | 4492 |
| H | ? | version.rs | 4524 |
| H | ? | version.rs | 4529 |
| H | ? | version.rs | 4532 |
| H | ? | version.rs | 4539 |
| H | ? | version.rs | 4544 |
| H | ? | version.rs | 4576 |
| H | ? | version.rs | 4581 |
| H | ? | version.rs | 4584 |
| H | ? | version.rs | 4591 |
| H | ? | version.rs | 4596 |
| H | ? | version.rs | 4628 |
| H | ? | version.rs | 4633 |
| H | ? | version.rs | 4636 |
| H | ? | version.rs | 4643 |
| H | ? | version.rs | 4648 |
| H | ? | version.rs | 4680 |
| H | ? | version.rs | 4685 |
| H | ? | version.rs | 4688 |
| H | ? | version.rs | 4695 |
| H | ? | version.rs | 4700 |
| H | ? | version.rs | 4723 |
| H | ? | version.rs | 4725 |
| H | ? | version.rs | 4728 |
| H | ? | version.rs | 4730 |
| H | ? | version.rs | 4732 |
| H | ? | version.rs | 4755 |
| H | ? | version.rs | 4757 |
| H | ? | version.rs | 4760 |
| H | ? | version.rs | 4764 |
| H | ? | version.rs | 4769 |
| H | ? | version.rs | 4793 |
| H | ? | version.rs | 4795 |
| H | ? | version.rs | 4798 |
| H | ? | version.rs | 4800 |
| H | ? | version.rs | 4802 |
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
| C | ? | registry_client.rs | 2090 |
| C | ? | registry_client.rs | 2146 |
| C | ? | registry_client.rs | 2196 |
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
| M | ? | registries-test.py | 153 |
| M | ? | transform_readme.py | 73 |
| M | ? | transform_readme.py | 79 |
| M | ? | resolver.py | 170 |
| M | ? | resolver.py | 188 |
| M | ? | resolver.py | 227 |
| M | ? | resolver.py | 250 |
| M | ? | resolver.py | 375 |
| M | ? | resolver.py | 387 |
| M | ? | resolver.py | 463 |
| M | ? | resolver.py | 473 |
| M | ? | resolver.py | 651 |
| M | ? | resolver.py | 659 |
| M | ? | resolver.py | 718 |
| M | ? | resolver.py | 724 |
| M | ? | resolver.py | 866 |
| M | ? | resolver.py | 885 |
| M | ? | resolver.py | 928 |
| M | ? | resolver.py | 953 |
| M | ? | resolver.py | 1048 |
| M | ? | resolver.py | 1056 |
| M | ? | resolver.py | 1123 |
| M | ? | resolver.py | 1129 |
| M | ? | resolver.py | 1271 |
| H | ? | uv.schema.json | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | mkdocs.yml | 0 |
| H | GS002 | credentials.rs | 0 |
| H | GS002 | credentials.rs | 0 |
| s | GS009 |  | 0 |
| L | GS014 | credentials.rs | 1 |
| L | GS014 | credentials.rs | 1 |
| M | ? | _musllinux.py | 50 |
| M | ? | check_embedded_python.py | 29 |
| M | ? | check_embedded_python.py | 41 |
| M | ? | check_embedded_python.py | 62 |
| M | ? | check_embedded_python.py | 71 |
| M | ? | check_embedded_python.py | 83 |
| M | ? | check_embedded_python.py | 92 |
| M | ? | registries-test.py | 79 |
| M | ? | registries-test.py | 99 |
| M | ? | registries-test.py | 223 |
| M | ? | registries-test.py | 350 |
| M | ? | __main__.py | 31 |
| M | ? | bump-workspace-crate-versions.py | 54 |
| M | ? | vendor-packaging.py | 44 |
| M | ? | vendor-packaging.py | 48 |
| M | ? | check_system_python.py | 26 |
| M | ? | check_system_python.py | 33 |
| M | ? | check_system_python.py | 41 |
| M | ? | check_system_python.py | 108 |
| M | ? | check_system_python.py | 133 |
| M | ? | check_system_python.py | 142 |
| M | ? | check_system_python.py | 152 |
| M | ? | check_system_python.py | 164 |
| M | ? | check_system_python.py | 178 |
| M | ? | check_system_python.py | 188 |
| M | ? | check_system_python.py | 198 |
| M | ? | check_system_python.py | 210 |
| M | ? | check_system_python.py | 224 |
| M | ? | check_system_python.py | 233 |
| M | ? | check_system_python.py | 245 |
| M | ? | check_system_python.py | 257 |
| M | ? | check_system_python.py | 266 |
| M | ? | check_system_python.py | 302 |
| M | ? | check_system_python.py | 310 |
| M | ? | check_system_python.py | 319 |
| M | ? | publish-crates.py | 45 |
| M | ? | publish-crates.py | 136 |
| M | ? | repair-sdist-cargo-lock.py | 57 |
| M | ? | repair-sdist-cargo-lock.py | 65 |
| M | ? | check_cache_compat.py | 37 |
| M | ? | check_cache_compat.py | 45 |
| M | ? | check_cache_compat.py | 51 |
| M | ? | check_cache_compat.py | 127 |
| M | ? | __main__.py | 42 |
| M | ? | post-edit-format.py | 18 |
| M | ? | post-edit-format.py | 31 |
| M | ? | post-edit-format.py | 44 |
| H | ? | lib.rs | 220 |
| H | ? | candidate_selector.rs | 336 |
| H | ? | candidate_selector.rs | 799 |
| H | ? | candidate_selector.rs | 801 |
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
| H | ? | universal_marker.rs | 840 |
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
| H | ? | mod.rs | 441 |
| H | ? | mod.rs | 513 |
| H | ? | mod.rs | 516 |
| H | ? | mod.rs | 532 |
| H | ? | mod.rs | 550 |
| H | ? | mod.rs | 571 |
| H | ? | mod.rs | 614 |
| H | ? | mod.rs | 615 |
| H | ? | mod.rs | 627 |
| H | ? | mod.rs | 628 |
| H | ? | mod.rs | 629 |
| H | ? | mod.rs | 642 |
| H | ? | mod.rs | 643 |
| H | ? | mod.rs | 644 |
| H | ? | mod.rs | 657 |
| H | ? | mod.rs | 659 |
| H | ? | mod.rs | 670 |
| H | ? | mod.rs | 672 |
| H | ? | mod.rs | 699 |
| H | ? | mod.rs | 700 |
| H | ? | mod.rs | 712 |
| H | ? | mod.rs | 1493 |
| H | ? | mod.rs | 1547 |
| H | ? | mod.rs | 1653 |
| H | ? | mod.rs | 1668 |
| H | ? | mod.rs | 1787 |
| H | ? | mod.rs | 1805 |
| H | ? | mod.rs | 1874 |
| H | ? | mod.rs | 2009 |
| H | ? | mod.rs | 2063 |
| H | ? | mod.rs | 2070 |
| H | ? | mod.rs | 2074 |
| H | ? | mod.rs | 2095 |
| H | ? | mod.rs | 2096 |
| H | ? | mod.rs | 2194 |
| H | ? | mod.rs | 2201 |
| H | ? | mod.rs | 2205 |
| H | ? | mod.rs | 2279 |
| H | ? | mod.rs | 2285 |
| H | ? | mod.rs | 2290 |
| H | ? | mod.rs | 2677 |
| H | ? | mod.rs | 2816 |
| H | ? | mod.rs | 2834 |
| H | ? | mod.rs | 2895 |
| H | ? | mod.rs | 2898 |
| H | ? | mod.rs | 2956 |
| H | ? | mod.rs | 2977 |
| H | ? | mod.rs | 2989 |
| H | ? | mod.rs | 2992 |
| H | ? | mod.rs | 2997 |
| H | ? | mod.rs | 3006 |
| H | ? | mod.rs | 3021 |
| H | ? | mod.rs | 3028 |
| H | ? | mod.rs | 3029 |
| H | ? | mod.rs | 3034 |
| H | ? | mod.rs | 3039 |
| H | ? | mod.rs | 3047 |
| H | ? | mod.rs | 3054 |
| H | ? | mod.rs | 3061 |
| H | ? | mod.rs | 3081 |
| H | ? | mod.rs | 3092 |
| H | ? | mod.rs | 3096 |
| H | ? | mod.rs | 3100 |
| H | ? | mod.rs | 3104 |
| H | ? | mod.rs | 3109 |
| H | ? | mod.rs | 3115 |
| H | ? | mod.rs | 3155 |
| H | ? | mod.rs | 3165 |
| H | ? | mod.rs | 3166 |
| H | ? | mod.rs | 3177 |
| H | ? | mod.rs | 3189 |
| H | ? | mod.rs | 3201 |
| H | ? | mod.rs | 3218 |
| H | ? | mod.rs | 3227 |
| H | ? | mod.rs | 3236 |
| H | ? | mod.rs | 3237 |
| H | ? | mod.rs | 3242 |
| H | ? | mod.rs | 3245 |
| H | ? | mod.rs | 3252 |
| H | ? | mod.rs | 3253 |
| H | ? | mod.rs | 3257 |
| H | ? | mod.rs | 3260 |
| H | ? | mod.rs | 3270 |
| H | ? | mod.rs | 3279 |
| H | ? | mod.rs | 3280 |
| H | ? | mod.rs | 3284 |
| H | ? | mod.rs | 3286 |
| H | ? | mod.rs | 3305 |
| H | ? | mod.rs | 3306 |
| H | ? | mod.rs | 3311 |
| H | ? | mod.rs | 3315 |
| H | ? | mod.rs | 3323 |
| H | ? | mod.rs | 3328 |
| H | ? | mod.rs | 3338 |
| H | ? | mod.rs | 3339 |
| H | ? | mod.rs | 3361 |
| H | ? | mod.rs | 3377 |
| H | ? | mod.rs | 3378 |
| H | ? | mod.rs | 3386 |
| H | ? | mod.rs | 3390 |
| H | ? | mod.rs | 3398 |
| H | ? | mod.rs | 3414 |
| H | ? | mod.rs | 3415 |
| H | ? | mod.rs | 3523 |
| H | ? | mod.rs | 3527 |
| H | ? | mod.rs | 3529 |
| H | ? | mod.rs | 3541 |
| H | ? | mod.rs | 3600 |
| H | ? | mod.rs | 3658 |
| H | ? | mod.rs | 3662 |
| H | ? | mod.rs | 3663 |
| H | ? | mod.rs | 3676 |
| H | ? | mod.rs | 3743 |
| H | ? | mod.rs | 3745 |
| H | ? | mod.rs | 3781 |
| H | ? | mod.rs | 3785 |
| H | ? | mod.rs | 3791 |
| H | ? | mod.rs | 3799 |
| H | ? | mod.rs | 3925 |
| H | ? | mod.rs | 4003 |
| H | ? | mod.rs | 4028 |
| H | ? | mod.rs | 4047 |
| H | ? | mod.rs | 4051 |
| H | ? | mod.rs | 4209 |
| H | ? | mod.rs | 4628 |
| H | ? | mod.rs | 4646 |
| H | ? | mod.rs | 4664 |
| H | ? | mod.rs | 4742 |
| H | ? | mod.rs | 4951 |
| H | ? | mod.rs | 4996 |
| H | ? | mod.rs | 5004 |
| H | ? | mod.rs | 5009 |
| H | ? | mod.rs | 5017 |
| H | ? | mod.rs | 5022 |
| H | ? | mod.rs | 5032 |
| H | ? | mod.rs | 5038 |
| H | ? | mod.rs | 5051 |
| H | ? | mod.rs | 5061 |
| H | ? | mod.rs | 5078 |
| H | ? | mod.rs | 5101 |
| H | ? | mod.rs | 5111 |
| H | ? | mod.rs | 5203 |
| H | ? | mod.rs | 5391 |
| H | ? | mod.rs | 5538 |
| H | ? | mod.rs | 5549 |
| H | ? | mod.rs | 5557 |
| H | ? | mod.rs | 5558 |
| H | ? | mod.rs | 5582 |
| H | ? | mod.rs | 5593 |
| H | ? | mod.rs | 5601 |
| H | ? | mod.rs | 5602 |
| H | ? | mod.rs | 5708 |
| H | ? | mod.rs | 5709 |
| H | ? | mod.rs | 5842 |
| H | ? | mod.rs | 5866 |
| H | ? | mod.rs | 5882 |
| H | ? | mod.rs | 5886 |
| H | ? | serialize.rs | 120 |
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
| H | ? | metadata.rs | 136 |
| H | ? | metadata.rs | 210 |
| H | ? | metadata.rs | 408 |
| H | ? | metadata.rs | 412 |
| H | ? | metadata.rs | 505 |
| H | ? | metadata.rs | 509 |
| H | ? | metadata.rs | 565 |
| H | ? | metadata.rs | 575 |
| H | ? | metadata.rs | 606 |
| H | ? | metadata.rs | 626 |
| H | ? | metadata.rs | 675 |
| H | ? | metadata.rs | 694 |
| H | ? | metadata.rs | 790 |
| H | ? | metadata.rs | 791 |
| H | ? | metadata.rs | 792 |
| H | ? | metadata.rs | 1018 |
| H | ? | metadata.rs | 1116 |
| H | ? | metadata.rs | 1132 |
| H | ? | metadata.rs | 1243 |
| H | ? | metadata.rs | 1248 |
| H | ? | metadata.rs | 1265 |
| H | ? | metadata.rs | 1266 |
| H | ? | metadata.rs | 1273 |
| H | ? | metadata.rs | 1274 |
| H | ? | metadata.rs | 1334 |
| H | ? | metadata.rs | 1350 |
| H | ? | metadata.rs | 1362 |
| H | ? | metadata.rs | 1374 |
| H | ? | metadata.rs | 1386 |
| H | ? | metadata.rs | 1409 |
| H | ? | metadata.rs | 1413 |
| H | ? | metadata.rs | 1421 |
| H | ? | metadata.rs | 1422 |
| H | ? | metadata.rs | 1426 |
| H | ? | metadata.rs | 1428 |
| H | ? | metadata.rs | 1433 |
| H | ? | metadata.rs | 1435 |
| H | ? | metadata.rs | 1436 |
| H | ? | metadata.rs | 1450 |
| H | ? | metadata.rs | 1462 |
| H | ? | pylock_toml.rs | 395 |
| H | ? | pylock_toml.rs | 426 |
| H | ? | pylock_toml.rs | 442 |
| H | ? | pylock_toml.rs | 447 |
| H | ? | pylock_toml.rs | 457 |
| H | ? | pylock_toml.rs | 464 |
| H | ? | pylock_toml.rs | 498 |
| H | ? | pylock_toml.rs | 508 |
| H | ? | pylock_toml.rs | 515 |
| H | ? | pylock_toml.rs | 519 |
| H | ? | pylock_toml.rs | 520 |
| H | ? | pylock_toml.rs | 530 |
| H | ? | pylock_toml.rs | 540 |
| H | ? | pylock_toml.rs | 546 |
| H | ? | pylock_toml.rs | 559 |
| H | ? | pylock_toml.rs | 566 |
| H | ? | pylock_toml.rs | 592 |
| H | ? | pylock_toml.rs | 602 |
| H | ? | pylock_toml.rs | 678 |
| H | ? | pylock_toml.rs | 694 |
| H | ? | pylock_toml.rs | 731 |
| H | ? | pylock_toml.rs | 778 |
| H | ? | pylock_toml.rs | 842 |
| H | ? | pylock_toml.rs | 848 |
| H | ? | pylock_toml.rs | 861 |
| H | ? | pylock_toml.rs | 883 |
| H | ? | pylock_toml.rs | 887 |
| H | ? | pylock_toml.rs | 898 |
| H | ? | pylock_toml.rs | 926 |
| H | ? | pylock_toml.rs | 948 |
| H | ? | pylock_toml.rs | 1080 |
| H | ? | pylock_toml.rs | 1082 |
| H | ? | pylock_toml.rs | 1090 |
| H | ? | pylock_toml.rs | 1091 |
| H | ? | pylock_toml.rs | 1092 |
| H | ? | pylock_toml.rs | 1107 |
| H | ? | pylock_toml.rs | 1111 |
| H | ? | pylock_toml.rs | 1114 |
| H | ? | pylock_toml.rs | 1119 |
| H | ? | pylock_toml.rs | 1123 |
| H | ? | pylock_toml.rs | 1126 |
| H | ? | pylock_toml.rs | 1130 |
| H | ? | pylock_toml.rs | 1134 |
| H | ? | pylock_toml.rs | 1139 |
| H | ? | pylock_toml.rs | 1142 |
| H | ? | pylock_toml.rs | 1160 |
| H | ? | pylock_toml.rs | 1180 |
| H | ? | pylock_toml.rs | 1229 |
| H | ? | pylock_toml.rs | 1243 |
| H | ? | pylock_toml.rs | 1246 |
| H | ? | pylock_toml.rs | 1249 |
| H | ? | pylock_toml.rs | 1251 |
| H | ? | pylock_toml.rs | 1254 |
| H | ? | pylock_toml.rs | 1260 |
| H | ? | pylock_toml.rs | 1407 |
| H | ? | pylock_toml.rs | 1412 |
| H | ? | pylock_toml.rs | 1428 |
| H | ? | pylock_toml.rs | 1435 |
| H | ? | pylock_toml.rs | 1440 |
| H | ? | pylock_toml.rs | 1461 |
| H | ? | pylock_toml.rs | 1465 |
| H | ? | pylock_toml.rs | 1474 |
| H | ? | pylock_toml.rs | 1482 |
| H | ? | pylock_toml.rs | 1515 |
| H | ? | pylock_toml.rs | 1531 |
| H | ? | pylock_toml.rs | 1536 |
| H | ? | pylock_toml.rs | 1543 |
| H | ? | pylock_toml.rs | 1550 |
| H | ? | pylock_toml.rs | 1561 |
| H | ? | pylock_toml.rs | 1562 |
| H | ? | pylock_toml.rs | 1566 |
| H | ? | pylock_toml.rs | 1568 |
| H | ? | pylock_toml.rs | 1582 |
| H | ? | pylock_toml.rs | 1588 |
| H | ? | pylock_toml.rs | 1592 |
| H | ? | pylock_toml.rs | 1622 |
| H | ? | pylock_toml.rs | 1626 |
| H | ? | pylock_toml.rs | 1635 |
| H | ? | pylock_toml.rs | 1643 |
| H | ? | pylock_toml.rs | 1653 |
| H | ? | pylock_toml.rs | 1676 |
| H | ? | pylock_toml.rs | 1697 |
| H | ? | pylock_toml.rs | 1708 |
| H | ? | pylock_toml.rs | 1716 |
| H | ? | pylock_toml.rs | 1717 |
| H | ? | pylock_toml.rs | 1722 |
| H | ? | pylock_toml.rs | 1723 |
| H | ? | pylock_toml.rs | 1724 |
| H | ? | pylock_toml.rs | 1726 |
| H | ? | pylock_toml.rs | 1731 |
| H | ? | pylock_toml.rs | 1743 |
| H | ? | pylock_toml.rs | 1751 |
| H | ? | pylock_toml.rs | 1756 |
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
| H | ? | version_map.rs | 97 |
| H | ? | version_map.rs | 693 |
| H | ? | version_map.rs | 708 |
| H | ? | version_map.rs | 722 |
| H | ? | version_map.rs | 723 |
| H | ? | version_map.rs | 726 |
| H | ? | version_map.rs | 767 |
| H | ? | version_map.rs | 813 |
| H | ? | python_requirement.rs | 43 |
| H | ? | python_requirement.rs | 75 |
| H | ? | python_requirement.rs | 103 |
| H | ? | python_requirement.rs | 125 |
| H | ? | python_requirement.rs | 126 |
| H | ? | python_requirement.rs | 140 |
| H | ? | python_requirement.rs | 141 |
| H | ? | python_requirement.rs | 146 |
| H | ? | python_requirement.rs | 147 |
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
| H | ? | mod.rs | 452 |
| H | ? | mod.rs | 453 |
| H | ? | mod.rs | 455 |
| H | ? | mod.rs | 529 |
| H | ? | mod.rs | 551 |
| H | ? | mod.rs | 574 |
| H | ? | mod.rs | 575 |
| H | ? | mod.rs | 585 |
| H | ? | mod.rs | 660 |
| H | ? | mod.rs | 669 |
| H | ? | mod.rs | 710 |
| H | ? | mod.rs | 794 |
| H | ? | mod.rs | 829 |
| H | ? | mod.rs | 830 |
| H | ? | mod.rs | 831 |
| H | ? | mod.rs | 835 |
| H | ? | mod.rs | 838 |
| H | ? | mod.rs | 974 |
| H | ? | mod.rs | 977 |
| H | ? | mod.rs | 1034 |
| H | ? | mod.rs | 1095 |
| H | ? | mod.rs | 1099 |
| H | ? | mod.rs | 1108 |
| H | ? | mod.rs | 1110 |
| H | ? | mod.rs | 1114 |
| H | ? | mod.rs | 1115 |
| H | ? | mod.rs | 1163 |
| H | ? | mod.rs | 1165 |
| H | ? | mod.rs | 1166 |
| H | ? | mod.rs | 1167 |
| H | ? | mod.rs | 1201 |
| H | ? | mod.rs | 1215 |
| H | ? | mod.rs | 1220 |
| H | ? | mod.rs | 1250 |
| H | ? | mod.rs | 1265 |
| H | ? | mod.rs | 1311 |
| H | ? | mod.rs | 1325 |
| H | ? | mod.rs | 1333 |
| H | ? | mod.rs | 1335 |
| H | ? | mod.rs | 1372 |
| H | ? | mod.rs | 1385 |
| H | ? | mod.rs | 1402 |
| H | ? | mod.rs | 1404 |
| H | ? | mod.rs | 1410 |
| H | ? | mod.rs | 1434 |
| H | ? | mod.rs | 1442 |
| H | ? | mod.rs | 1449 |
| H | ? | mod.rs | 1455 |
| H | ? | mod.rs | 1461 |
| H | ? | mod.rs | 1492 |
| H | ? | mod.rs | 1495 |
| H | ? | mod.rs | 1538 |
| H | ? | mod.rs | 1581 |
| H | ? | mod.rs | 1636 |
| H | ? | mod.rs | 1683 |
| H | ? | mod.rs | 1684 |
| H | ? | mod.rs | 1751 |
| H | ? | mod.rs | 1807 |
| H | ? | mod.rs | 1809 |
| H | ? | mod.rs | 1812 |
| H | ? | mod.rs | 1814 |
| H | ? | mod.rs | 1842 |
| H | ? | mod.rs | 1843 |
| H | ? | mod.rs | 1851 |
| H | ? | mod.rs | 1875 |
| H | ? | mod.rs | 1884 |
| H | ? | mod.rs | 1987 |
| H | ? | mod.rs | 2007 |
| H | ? | mod.rs | 2030 |
| H | ? | mod.rs | 2033 |
| H | ? | mod.rs | 2041 |
| H | ? | mod.rs | 2043 |
| H | ? | mod.rs | 2052 |
| H | ? | mod.rs | 2109 |
| H | ? | mod.rs | 2114 |
| H | ? | mod.rs | 2137 |
| H | ? | mod.rs | 2142 |
| H | ? | mod.rs | 2163 |
| H | ? | mod.rs | 2165 |
| H | ? | mod.rs | 2168 |
| H | ? | mod.rs | 2248 |
| H | ? | mod.rs | 2269 |
| H | ? | mod.rs | 2270 |
| H | ? | mod.rs | 2271 |
| H | ? | mod.rs | 2272 |
| H | ? | mod.rs | 2273 |
| H | ? | mod.rs | 2301 |
| H | ? | mod.rs | 2303 |
| H | ? | mod.rs | 2304 |
| H | ? | mod.rs | 2305 |
| H | ? | mod.rs | 2351 |
| H | ? | mod.rs | 2454 |
| H | ? | mod.rs | 2455 |
| H | ? | mod.rs | 2456 |
| H | ? | mod.rs | 2457 |
| H | ? | mod.rs | 2458 |
| H | ? | mod.rs | 2491 |
| H | ? | mod.rs | 2492 |
| H | ? | mod.rs | 2493 |
| H | ? | mod.rs | 2494 |
| H | ? | mod.rs | 2495 |
| H | ? | mod.rs | 2640 |
| H | ? | mod.rs | 2669 |
| H | ? | mod.rs | 2670 |
| H | ? | mod.rs | 2685 |
| H | ? | mod.rs | 2686 |
| H | ? | mod.rs | 2710 |
| H | ? | mod.rs | 2717 |
| H | ? | mod.rs | 2724 |
| H | ? | mod.rs | 2770 |
| H | ? | mod.rs | 2776 |
| H | ? | mod.rs | 2780 |
| H | ? | mod.rs | 2839 |
| H | ? | mod.rs | 2851 |
| H | ? | mod.rs | 2860 |
| H | ? | mod.rs | 2893 |
| H | ? | mod.rs | 2906 |
| H | ? | mod.rs | 2908 |
| H | ? | mod.rs | 2934 |
| H | ? | mod.rs | 2943 |
| H | ? | mod.rs | 2946 |
| H | ? | mod.rs | 2971 |
| H | ? | mod.rs | 2994 |
| H | ? | mod.rs | 3001 |
| H | ? | mod.rs | 3014 |
| H | ? | mod.rs | 3018 |
| H | ? | mod.rs | 3019 |
| H | ? | mod.rs | 3020 |
| H | ? | mod.rs | 3021 |
| H | ? | mod.rs | 3028 |
| H | ? | mod.rs | 3029 |
| H | ? | mod.rs | 3030 |
| H | ? | mod.rs | 3302 |
| H | ? | mod.rs | 3303 |
| H | ? | mod.rs | 3307 |
| H | ? | mod.rs | 3313 |
| H | ? | mod.rs | 3333 |
| H | ? | mod.rs | 3430 |
| H | ? | mod.rs | 3444 |
| H | ? | mod.rs | 3569 |
| H | ? | mod.rs | 3574 |
| H | ? | mod.rs | 3575 |
| H | ? | mod.rs | 3578 |
| H | ? | mod.rs | 3579 |
| H | ? | mod.rs | 3601 |
| H | ? | mod.rs | 3606 |
| H | ? | mod.rs | 3607 |
| H | ? | mod.rs | 3633 |
| H | ? | mod.rs | 3638 |
| H | ? | mod.rs | 3639 |
| H | ? | mod.rs | 3642 |
| H | ? | mod.rs | 3651 |
| H | ? | mod.rs | 3656 |
| H | ? | mod.rs | 3657 |
| H | ? | mod.rs | 3683 |
| H | ? | mod.rs | 3688 |
| H | ? | mod.rs | 3689 |
| H | ? | mod.rs | 3693 |
| H | ? | mod.rs | 3717 |
| H | ? | mod.rs | 3718 |
| H | ? | mod.rs | 3719 |
| H | ? | mod.rs | 3841 |
| H | ? | mod.rs | 3933 |
| H | ? | mod.rs | 4002 |
| H | ? | mod.rs | 4031 |
| H | ? | mod.rs | 4050 |
| H | ? | mod.rs | 4071 |
| H | ? | mod.rs | 4077 |
| H | ? | mod.rs | 4088 |
| H | ? | mod.rs | 4095 |
| H | ? | mod.rs | 4135 |
| H | ? | mod.rs | 4192 |
| H | ? | mod.rs | 4204 |
| H | ? | mod.rs | 4416 |
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
| H | ? | mod.rs | 996 |
| H | ? | mod.rs | 998 |
| H | ? | flat_index.rs | 170 |
| H | ? | flat_index.rs | 203 |
| H | ? | flat_index.rs | 208 |
| H | ? | flat_index.rs | 214 |
| H | ? | flat_index.rs | 217 |
| H | ? | flat_index.rs | 224 |
| H | ? | flat_index.rs | 268 |
| H | ? | flat_index.rs | 346 |
| H | ? | cached_client.rs | 259 |
| H | ? | cached_client.rs | 287 |
| H | ? | cached_client.rs | 293 |
| H | ? | cached_client.rs | 295 |
| H | ? | cached_client.rs | 318 |
| H | ? | cached_client.rs | 350 |
| H | ? | cached_client.rs | 369 |
| H | ? | cached_client.rs | 554 |
| H | ? | cached_client.rs | 595 |
| H | ? | cached_client.rs | 604 |
| H | ? | cached_client.rs | 616 |
| H | ? | cached_client.rs | 627 |
| H | ? | cached_client.rs | 660 |
| H | ? | cached_client.rs | 665 |
| H | ? | cached_client.rs | 677 |
| H | ? | cached_client.rs | 740 |
| H | ? | cached_client.rs | 747 |
| H | ? | cached_client.rs | 778 |
| H | ? | cached_client.rs | 785 |
| H | ? | registry_client.rs | 158 |
| H | ? | registry_client.rs | 425 |
| H | ? | registry_client.rs | 464 |
| H | ? | registry_client.rs | 486 |
| H | ? | registry_client.rs | 513 |
| H | ? | registry_client.rs | 515 |
| H | ? | registry_client.rs | 612 |
| H | ? | registry_client.rs | 617 |
| H | ? | registry_client.rs | 623 |
| H | ? | registry_client.rs | 628 |
| H | ? | registry_client.rs | 630 |
| H | ? | registry_client.rs | 635 |
| H | ? | registry_client.rs | 644 |
| H | ? | registry_client.rs | 650 |
| H | ? | registry_client.rs | 663 |
| H | ? | registry_client.rs | 669 |
| H | ? | registry_client.rs | 682 |
| H | ? | registry_client.rs | 689 |
| H | ? | registry_client.rs | 701 |
| H | ? | registry_client.rs | 735 |
| H | ? | registry_client.rs | 741 |
| H | ? | registry_client.rs | 761 |
| H | ? | registry_client.rs | 763 |
| H | ? | registry_client.rs | 820 |
| H | ? | registry_client.rs | 825 |
| H | ? | registry_client.rs | 827 |
| H | ? | registry_client.rs | 832 |
| H | ? | registry_client.rs | 841 |
| H | ? | registry_client.rs | 847 |
| H | ? | registry_client.rs | 853 |
| H | ? | registry_client.rs | 859 |
| H | ? | registry_client.rs | 865 |
| H | ? | registry_client.rs | 871 |
| H | ? | registry_client.rs | 877 |
| H | ? | registry_client.rs | 892 |
| H | ? | registry_client.rs | 897 |
| H | ? | registry_client.rs | 920 |
| H | ? | registry_client.rs | 965 |
| H | ? | registry_client.rs | 984 |
| H | ? | registry_client.rs | 1018 |
| H | ? | registry_client.rs | 1063 |
| H | ? | registry_client.rs | 1074 |
| H | ? | registry_client.rs | 1096 |
| H | ? | registry_client.rs | 1128 |
| H | ? | registry_client.rs | 1135 |
| H | ? | registry_client.rs | 1143 |
| H | ? | registry_client.rs | 1146 |
| H | ? | registry_client.rs | 1207 |
| H | ? | registry_client.rs | 1214 |
| H | ? | registry_client.rs | 1220 |
| H | ? | registry_client.rs | 1239 |
| H | ? | registry_client.rs | 1241 |
| H | ? | registry_client.rs | 1242 |
| H | ? | registry_client.rs | 1245 |
| H | ? | registry_client.rs | 1250 |
| H | ? | registry_client.rs | 1265 |
| H | ? | registry_client.rs | 1281 |
| H | ? | registry_client.rs | 1293 |
| H | ? | registry_client.rs | 1303 |
| H | ? | registry_client.rs | 1375 |
| H | ? | registry_client.rs | 1574 |
| H | ? | registry_client.rs | 1645 |
| H | ? | registry_client.rs | 1710 |
| H | ? | registry_client.rs | 1778 |
| H | ? | registry_client.rs | 1796 |
| H | ? | registry_client.rs | 1797 |
| H | ? | registry_client.rs | 1826 |
| H | ? | registry_client.rs | 2125 |
| H | ? | registry_client.rs | 2175 |
| H | ? | registry_client.rs | 2225 |
| H | ? | base_client.rs | 447 |
| H | ? | base_client.rs | 455 |
| H | ? | base_client.rs | 460 |
| H | ? | base_client.rs | 467 |
| H | ? | base_client.rs | 476 |
| H | ? | base_client.rs | 478 |
| H | ? | base_client.rs | 486 |
| H | ? | base_client.rs | 491 |
| H | ? | base_client.rs | 498 |
| H | ? | base_client.rs | 503 |
| H | ? | base_client.rs | 504 |
| H | ? | base_client.rs | 507 |
| H | ? | base_client.rs | 509 |
| H | ? | base_client.rs | 522 |
| H | ? | base_client.rs | 542 |
| H | ? | base_client.rs | 614 |
| H | ? | base_client.rs | 625 |
| H | ? | base_client.rs | 642 |
| H | ? | base_client.rs | 657 |
| H | ? | base_client.rs | 679 |
| H | ? | base_client.rs | 687 |
| H | ? | base_client.rs | 689 |
| H | ? | base_client.rs | 699 |
| H | ? | base_client.rs | 701 |
| H | ? | base_client.rs | 792 |
| H | ? | base_client.rs | 942 |
| H | ? | base_client.rs | 1077 |
| H | ? | base_client.rs | 1183 |
| H | ? | base_client.rs | 1189 |
| H | ? | retry.rs | 149 |
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
| H | ? | dependency_groups.rs | 138 |
| H | ? | dependency_groups.rs | 143 |
| H | ? | extras.rs | 41 |
| H | ? | extras.rs | 116 |
| H | ? | proxy_url.rs | 173 |
| H | ? | proxy_url.rs | 190 |
| H | ? | libc.rs | 227 |
| H | ? | libc.rs | 232 |
| H | ? | libc.rs | 357 |
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
| H | ? | workspace.rs | 636 |
| H | ? | workspace.rs | 642 |
| H | ? | workspace.rs | 678 |
| H | ? | workspace.rs | 692 |
| H | ? | workspace.rs | 698 |
| H | ? | workspace.rs | 705 |
| H | ? | workspace.rs | 771 |
| H | ? | workspace.rs | 842 |
| H | ? | workspace.rs | 856 |
| H | ? | workspace.rs | 870 |
| H | ? | workspace.rs | 884 |
| H | ? | workspace.rs | 1068 |
| H | ? | workspace.rs | 1073 |
| H | ? | workspace.rs | 1081 |
| H | ? | workspace.rs | 1155 |
| H | ? | workspace.rs | 1157 |
| H | ? | workspace.rs | 1159 |
| H | ? | workspace.rs | 1160 |
| H | ? | workspace.rs | 1161 |
| H | ? | workspace.rs | 1167 |
| H | ? | workspace.rs | 1177 |
| H | ? | workspace.rs | 1180 |
| H | ? | workspace.rs | 1191 |
| H | ? | workspace.rs | 1196 |
| H | ? | workspace.rs | 1298 |
| H | ? | workspace.rs | 1324 |
| H | ? | workspace.rs | 1336 |
| H | ? | workspace.rs | 1338 |
| H | ? | workspace.rs | 1345 |
| H | ? | workspace.rs | 1364 |
| H | ? | workspace.rs | 1512 |
| H | ? | workspace.rs | 1568 |
| H | ? | workspace.rs | 1573 |
| H | ? | workspace.rs | 1606 |
| H | ? | workspace.rs | 1609 |
| H | ? | workspace.rs | 1674 |
| H | ? | workspace.rs | 1704 |
| H | ? | workspace.rs | 1705 |
| H | ? | workspace.rs | 1717 |
| H | ? | workspace.rs | 1718 |
| H | ? | workspace.rs | 1728 |
| H | ? | workspace.rs | 1746 |
| H | ? | workspace.rs | 1750 |
| H | ? | workspace.rs | 1754 |
| H | ? | workspace.rs | 1764 |
| H | ? | workspace.rs | 1776 |
| H | ? | workspace.rs | 1785 |
| H | ? | workspace.rs | 1790 |
| H | ? | workspace.rs | 1849 |
| H | ? | workspace.rs | 1876 |
| H | ? | workspace.rs | 2052 |
| H | ? | workspace.rs | 2056 |
| H | ? | workspace.rs | 2065 |
| H | ? | workspace.rs | 2089 |
| H | ? | workspace.rs | 2092 |
| H | ? | workspace.rs | 2093 |
| H | ? | workspace.rs | 2101 |
| H | ? | workspace.rs | 2109 |
| H | ? | workspace.rs | 2112 |
| H | ? | workspace.rs | 2121 |
| H | ? | workspace.rs | 2137 |
| H | ? | workspace.rs | 2141 |
| H | ? | workspace.rs | 2196 |
| H | ? | workspace.rs | 2197 |
| H | ? | workspace.rs | 2198 |
| H | ? | workspace.rs | 2200 |
| H | ? | workspace.rs | 2298 |
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
| H | ? | pyproject_mut.rs | 385 |
| H | ? | pyproject_mut.rs | 524 |
| H | ? | pyproject_mut.rs | 527 |
| H | ? | pyproject_mut.rs | 546 |
| H | ? | pyproject_mut.rs | 549 |
| H | ? | pyproject_mut.rs | 565 |
| H | ? | pyproject_mut.rs | 568 |
| H | ? | pyproject_mut.rs | 587 |
| H | ? | pyproject_mut.rs | 590 |
| H | ? | pyproject_mut.rs | 1403 |
| H | ? | pyproject_mut.rs | 1549 |
| H | ? | pyproject_mut.rs | 1575 |
| H | ? | pyproject_mut.rs | 1589 |
| H | ? | pyproject_mut.rs | 1595 |
| H | ? | pyproject_mut.rs | 1682 |
| H | ? | pyproject_mut.rs | 1709 |
| H | ? | pyproject.rs | 1699 |
| H | ? | pyproject.rs | 1700 |
| H | ? | pyproject.rs | 1706 |
| H | ? | pyproject.rs | 1707 |
| H | ? | pyproject.rs | 1708 |
| H | ? | pyproject.rs | 1834 |
| H | ? | pyproject.rs | 1847 |
| H | ? | pyproject.rs | 1873 |
| H | ? | pyproject.rs | 1886 |
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
| H | ? | conflicts.rs | 123 |
| H | ? | conflicts.rs | 132 |
| H | ? | conflicts.rs | 134 |
| H | ? | conflicts.rs | 137 |
| H | ? | conflicts.rs | 148 |
| H | ? | conflicts.rs | 149 |
| H | ? | conflicts.rs | 182 |
| H | ? | conflicts.rs | 184 |
| H | ? | conflicts.rs | 186 |
| H | ? | conflicts.rs | 188 |
| H | ? | conflicts.rs | 210 |
| H | ? | conflicts.rs | 265 |
| H | ? | conflicts.rs | 395 |
| H | ? | conflicts.rs | 482 |
| H | ? | conflicts.rs | 483 |
| H | ? | conflicts.rs | 599 |
| H | ? | conflicts.rs | 602 |
| H | ? | conflicts.rs | 717 |
| H | ? | conflicts.rs | 722 |
| H | ? | conflicts.rs | 723 |
| H | ? | conflicts.rs | 727 |
| H | ? | conflicts.rs | 729 |
| H | ? | conflicts.rs | 738 |
| H | ? | conflicts.rs | 739 |
| H | ? | conflicts.rs | 740 |
| H | ? | conflicts.rs | 867 |
| H | ? | conflicts.rs | 868 |
| H | ? | conflicts.rs | 885 |
| H | ? | lib.rs | 262 |
| H | ? | lib.rs | 303 |
| H | ? | lib.rs | 311 |
| H | ? | lib.rs | 322 |
| H | ? | lib.rs | 1114 |
| H | ? | lib.rs | 1117 |
| H | ? | lib.rs | 1120 |
| H | ? | lib.rs | 1123 |
| H | ? | lib.rs | 1615 |
| H | ? | lib.rs | 6758 |
| H | ? | lib.rs | 6759 |
| H | ? | lib.rs | 6760 |
| H | ? | lib.rs | 6821 |
| H | ? | lib.rs | 6822 |
| H | ? | lib.rs | 6823 |
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
| H | ? | index_url.rs | 27 |
| H | ? | index_url.rs | 66 |
| H | ? | index_url.rs | 114 |
| H | ? | index_url.rs | 304 |
| H | ? | index_url.rs | 544 |
| H | ? | index_url.rs | 547 |
| H | ? | index_url.rs | 681 |
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
| H | ? | index.rs | 550 |
| H | ? | index.rs | 587 |
| H | ? | index.rs | 595 |
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
| H | ? | lib.rs | 456 |
| H | ? | lib.rs | 552 |
| H | ? | lib.rs | 812 |
| H | ? | lib.rs | 823 |
| H | ? | lib.rs | 834 |
| H | ? | lib.rs | 845 |
| H | ? | lib.rs | 846 |
| H | ? | lib.rs | 856 |
| H | ? | lib.rs | 857 |
| H | ? | lib.rs | 866 |
| H | ? | lib.rs | 867 |
| H | ? | lib.rs | 877 |
| H | ? | lib.rs | 878 |
| H | ? | lib.rs | 888 |
| H | ? | lib.rs | 1035 |
| H | ? | lib.rs | 1068 |
| H | ? | lib.rs | 1069 |
| H | ? | lib.rs | 1431 |
| H | ? | lib.rs | 1435 |
| H | ? | lib.rs | 1784 |
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
| H | ? | lib.rs | 1038 |
| H | ? | lib.rs | 1045 |
| H | ? | lib.rs | 1065 |
| H | ? | lib.rs | 1133 |
| H | ? | lib.rs | 1232 |
| H | ? | lib.rs | 1238 |
| H | ? | lib.rs | 1239 |
| H | ? | lib.rs | 1250 |
| H | ? | lib.rs | 1274 |
| H | ? | lib.rs | 1321 |
| H | ? | lib.rs | 1335 |
| H | ? | lib.rs | 1361 |
| H | ? | lib.rs | 1365 |
| H | ? | lib.rs | 1406 |
| H | ? | lib.rs | 1416 |
| H | ? | lib.rs | 1420 |
| H | ? | lib.rs | 1630 |
| H | ? | lib.rs | 1694 |
| H | ? | lib.rs | 1769 |
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
| H | ? | venv.rs | 292 |
| H | ? | venv.rs | 293 |
| H | ? | venv.rs | 339 |
| H | ? | venv.rs | 352 |
| H | ? | build_frontend.rs | 377 |
| H | ? | build_frontend.rs | 416 |
| H | ? | build_frontend.rs | 419 |
| H | ? | build_frontend.rs | 428 |
| H | ? | build_frontend.rs | 441 |
| H | ? | build_frontend.rs | 442 |
| H | ? | build_frontend.rs | 613 |
| H | ? | build_frontend.rs | 614 |
| H | ? | build_frontend.rs | 626 |
| H | ? | build_frontend.rs | 630 |
| H | ? | build_frontend.rs | 648 |
| H | ? | build_frontend.rs | 660 |
| H | ? | build_frontend.rs | 671 |
| H | ? | build_frontend.rs | 673 |
| H | ? | build_frontend.rs | 674 |
| H | ? | build_frontend.rs | 768 |
| H | ? | build_frontend.rs | 1164 |
| H | ? | build_frontend.rs | 1165 |
| H | ? | build_frontend.rs | 1170 |
| H | ? | build_frontend.rs | 1171 |
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
| H | ? | common.rs | 342 |
| H | ? | common.rs | 436 |
| H | ? | common.rs | 437 |
| H | ? | common.rs | 439 |
| H | ? | common.rs | 449 |
| H | ? | common.rs | 453 |
| H | ? | common.rs | 462 |
| H | ? | common.rs | 464 |
| H | ? | common.rs | 478 |
| H | ? | common.rs | 490 |
| H | ? | common.rs | 500 |
| H | ? | common.rs | 501 |
| H | ? | common.rs | 503 |
| H | ? | common.rs | 504 |
| H | ? | common.rs | 510 |
| H | ? | common.rs | 673 |
| H | ? | common.rs | 674 |
| H | ? | common.rs | 791 |
| H | ? | common.rs | 806 |
| H | ? | common.rs | 815 |
| H | ? | common.rs | 819 |
| H | ? | common.rs | 825 |
| H | ? | common.rs | 912 |
| H | ? | common.rs | 939 |
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
| H | ? | install.rs | 159 |
| H | ? | install.rs | 168 |
| H | ? | install.rs | 226 |
| H | ? | install.rs | 227 |
| H | ? | install.rs | 232 |
| H | ? | install.rs | 250 |
| H | ? | install.rs | 251 |
| H | ? | install.rs | 281 |
| H | ? | install.rs | 283 |
| H | ? | install.rs | 285 |
| H | ? | install.rs | 293 |
| H | ? | install.rs | 311 |
| H | ? | install.rs | 316 |
| H | ? | install.rs | 340 |
| H | ? | install.rs | 352 |
| H | ? | install.rs | 373 |
| H | ? | install.rs | 376 |
| H | ? | install.rs | 402 |
| H | ? | install.rs | 413 |
| H | ? | install.rs | 447 |
| H | ? | install.rs | 592 |
| H | ? | install.rs | 618 |
| H | ? | install.rs | 635 |
| H | ? | install.rs | 669 |
| H | ? | install.rs | 705 |
| H | ? | install.rs | 763 |
| H | ? | install.rs | 793 |
| H | ? | install.rs | 795 |
| H | ? | install.rs | 801 |
| H | ? | install.rs | 802 |
| H | ? | install.rs | 803 |
| H | ? | install.rs | 804 |
| H | ? | install.rs | 805 |
| H | ? | install.rs | 808 |
| H | ? | install.rs | 914 |
| H | ? | install.rs | 969 |
| H | ? | upgrade.rs | 78 |
| H | ? | upgrade.rs | 160 |
| H | ? | upgrade.rs | 161 |
| H | ? | upgrade.rs | 322 |
| H | ? | upgrade.rs | 323 |
| H | ? | upgrade.rs | 324 |
| H | ? | upgrade.rs | 326 |
| H | ? | upgrade.rs | 374 |
| H | ? | upgrade.rs | 402 |
| H | ? | upgrade.rs | 439 |
| H | ? | upgrade.rs | 485 |
| H | ? | upgrade.rs | 503 |
| H | ? | upgrade.rs | 515 |
| H | ? | upgrade.rs | 551 |
| H | ? | upgrade.rs | 609 |
| H | ? | upgrade.rs | 642 |
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
| H | ? | install.rs | 328 |
| H | ? | install.rs | 488 |
| H | ? | install.rs | 547 |
| H | ? | install.rs | 644 |
| H | ? | install.rs | 647 |
| H | ? | install.rs | 652 |
| H | ? | install.rs | 658 |
| H | ? | install.rs | 660 |
| H | ? | install.rs | 665 |
| H | ? | install.rs | 723 |
| H | ? | install.rs | 834 |
| H | ? | install.rs | 1021 |
| H | ? | install.rs | 1036 |
| H | ? | install.rs | 1039 |
| H | ? | install.rs | 1041 |
| H | ? | install.rs | 1088 |
| H | ? | install.rs | 1161 |
| H | ? | install.rs | 1175 |
| H | ? | install.rs | 1183 |
| H | ? | install.rs | 1197 |
| H | ? | install.rs | 1200 |
| H | ? | install.rs | 1202 |
| H | ? | install.rs | 1207 |
| H | ? | install.rs | 1218 |
| H | ? | install.rs | 1226 |
| H | ? | uninstall.rs | 108 |
| H | ? | uninstall.rs | 196 |
| H | ? | uninstall.rs | 214 |
| H | ? | uninstall.rs | 216 |
| H | ? | module_owners.rs | 70 |
| H | ? | module_owners.rs | 128 |
| H | ? | module_owners.rs | 148 |
| H | ? | help.rs | 52 |
| H | ? | pylock.rs | 35 |
| H | ? | lock_target.rs | 49 |
| H | ? | lock_target.rs | 261 |
| H | ? | lock_target.rs | 378 |
| H | ? | lock_target.rs | 430 |
| H | ? | lock_target.rs | 448 |
| H | ? | mod.rs | 642 |
| H | ? | mod.rs | 643 |
| H | ? | mod.rs | 651 |
| H | ? | mod.rs | 652 |
| H | ? | mod.rs | 659 |
| H | ? | mod.rs | 660 |
| H | ? | mod.rs | 680 |
| H | ? | mod.rs | 681 |
| H | ? | mod.rs | 687 |
| H | ? | mod.rs | 688 |
| H | ? | mod.rs | 693 |
| H | ? | mod.rs | 694 |
| H | ? | mod.rs | 993 |
| H | ? | mod.rs | 1006 |
| H | ? | mod.rs | 1013 |
| H | ? | mod.rs | 1217 |
| H | ? | mod.rs | 1234 |
| H | ? | mod.rs | 1629 |
| H | ? | mod.rs | 1682 |
| H | ? | mod.rs | 1725 |
| H | ? | mod.rs | 1731 |
| H | ? | mod.rs | 2299 |
| H | ? | mod.rs | 2315 |
| H | ? | mod.rs | 2324 |
| H | ? | mod.rs | 2325 |
| H | ? | mod.rs | 2327 |
| H | ? | mod.rs | 2338 |
| H | ? | mod.rs | 2342 |
| H | ? | mod.rs | 2356 |
| H | ? | mod.rs | 2368 |
| H | ? | mod.rs | 2378 |
| H | ? | mod.rs | 2379 |
| H | ? | mod.rs | 2381 |
| H | ? | mod.rs | 2382 |
| H | ? | mod.rs | 2394 |
| H | ? | mod.rs | 2505 |
| H | ? | mod.rs | 2550 |
| H | ? | mod.rs | 2557 |
| H | ? | mod.rs | 2558 |
| H | ? | mod.rs | 2560 |
| H | ? | mod.rs | 2570 |
| H | ? | mod.rs | 2574 |
| H | ? | mod.rs | 2583 |
| H | ? | mod.rs | 2585 |
| H | ? | mod.rs | 2604 |
| H | ? | mod.rs | 2636 |
| H | ? | mod.rs | 2648 |
| H | ? | mod.rs | 2658 |
| H | ? | mod.rs | 2659 |
| H | ? | mod.rs | 2661 |
| H | ? | mod.rs | 2662 |
| H | ? | mod.rs | 2736 |
| H | ? | mod.rs | 2745 |
| H | ? | mod.rs | 2746 |
| H | ? | mod.rs | 2778 |
| H | ? | mod.rs | 2790 |
| H | ? | mod.rs | 2800 |
| H | ? | mod.rs | 2804 |
| H | ? | mod.rs | 2908 |
| H | ? | mod.rs | 2993 |
| H | ? | mod.rs | 3000 |
| H | ? | mod.rs | 3001 |
| H | ? | mod.rs | 3003 |
| H | ? | mod.rs | 3021 |
| H | ? | mod.rs | 3023 |
| H | ? | mod.rs | 3055 |
| H | ? | mod.rs | 3065 |
| H | ? | mod.rs | 3066 |
| H | ? | mod.rs | 3068 |
| H | ? | mod.rs | 3069 |
| H | ? | mod.rs | 3086 |
| H | ? | mod.rs | 3091 |
| H | ? | mod.rs | 3212 |
| H | ? | mod.rs | 3216 |
| H | ? | mod.rs | 3218 |
| H | ? | mod.rs | 3251 |
| H | ? | mod.rs | 3256 |
| H | ? | mod.rs | 3258 |
| H | ? | mod.rs | 3453 |
| H | ? | version.rs | 275 |
| H | ? | version.rs | 419 |
| H | ? | ty.rs | 48 |
| H | ? | install_target.rs | 360 |
| H | ? | install_target.rs | 361 |
| H | ? | install_target.rs | 364 |
| H | ? | install_target.rs | 366 |
| H | ? | install_target.rs | 377 |
| H | ? | install_target.rs | 421 |
| H | ? | install_target.rs | 443 |
| H | ? | install_target.rs | 446 |
| H | ? | install_target.rs | 455 |
| H | ? | sync.rs | 127 |
| H | ? | sync.rs | 277 |
| H | ? | sync.rs | 282 |
| H | ? | sync.rs | 689 |
| H | ? | sync.rs | 702 |
| H | ? | sync.rs | 703 |
| H | ? | sync.rs | 704 |
| H | ? | sync.rs | 705 |
| H | ? | sync.rs | 706 |
| H | ? | sync.rs | 708 |
| H | ? | sync.rs | 712 |
| H | ? | sync.rs | 713 |
| H | ? | sync.rs | 714 |
| H | ? | sync.rs | 717 |
| H | ? | sync.rs | 735 |
| H | ? | sync.rs | 738 |
| H | ? | sync.rs | 747 |
| H | ? | sync.rs | 748 |
| H | ? | sync.rs | 858 |
| H | ? | sync.rs | 859 |
| H | ? | sync.rs | 899 |
| H | ? | sync.rs | 909 |
| H | ? | sync.rs | 910 |
| H | ? | sync.rs | 912 |
| H | ? | sync.rs | 913 |
| H | ? | sync.rs | 1005 |
| H | ? | sync.rs | 1017 |
| H | ? | sync.rs | 1052 |
| H | ? | sync.rs | 1076 |
| H | ? | sync.rs | 1102 |
| H | ? | sync.rs | 1125 |
| H | ? | sync.rs | 1129 |
| H | ? | sync.rs | 1147 |
| H | ? | sync.rs | 1155 |
| H | ? | sync.rs | 1203 |
| H | ? | sync.rs | 1573 |
| H | ? | check.rs | 92 |
| H | ? | check.rs | 196 |
| H | ? | check.rs | 217 |
| H | ? | check.rs | 228 |
| H | ? | check.rs | 266 |
| H | ? | tree.rs | 246 |
| H | ? | tree.rs | 247 |
| H | ? | tree.rs | 249 |
| H | ? | tree.rs | 252 |
| H | ? | tree.rs | 292 |
| H | ? | lock.rs | 388 |
| H | ? | lock.rs | 390 |
| H | ? | lock.rs | 770 |
| H | ? | lock.rs | 780 |
| H | ? | lock.rs | 783 |
| H | ? | lock.rs | 788 |
| H | ? | lock.rs | 795 |
| H | ? | lock.rs | 796 |
| H | ? | lock.rs | 807 |
| H | ? | lock.rs | 811 |
| H | ? | lock.rs | 830 |
| H | ? | lock.rs | 832 |
| H | ? | lock.rs | 833 |
| H | ? | lock.rs | 856 |
| H | ? | lock.rs | 902 |
| H | ? | lock.rs | 903 |
| H | ? | lock.rs | 905 |
| H | ? | lock.rs | 906 |
| H | ? | lock.rs | 913 |
| H | ? | lock.rs | 1052 |
| H | ? | lock.rs | 1053 |
| H | ? | lock.rs | 1069 |
| H | ? | lock.rs | 1092 |
| H | ? | lock.rs | 1103 |
| H | ? | lock.rs | 1654 |
| H | ? | upgrade.rs | 128 |
| H | ? | upgrade.rs | 129 |
| H | ? | upgrade.rs | 130 |
| H | ? | upgrade.rs | 132 |
| H | ? | upgrade.rs | 136 |
| H | ? | upgrade.rs | 190 |
| H | ? | upgrade.rs | 232 |
| H | ? | upgrade.rs | 293 |
| H | ? | upgrade.rs | 307 |
| H | ? | upgrade.rs | 308 |
| H | ? | upgrade.rs | 314 |
| H | ? | upgrade.rs | 315 |
| H | ? | upgrade.rs | 318 |
| H | ? | upgrade.rs | 319 |
| H | ? | upgrade.rs | 320 |
| H | ? | upgrade.rs | 399 |
| H | ? | upgrade.rs | 401 |
| H | ? | upgrade.rs | 414 |
| H | ? | upgrade.rs | 416 |
| H | ? | upgrade.rs | 424 |
| H | ? | upgrade.rs | 426 |
| H | ? | upgrade.rs | 501 |
| H | ? | upgrade.rs | 732 |
| H | ? | upgrade.rs | 739 |
| H | ? | upgrade.rs | 747 |
| H | ? | upgrade.rs | 764 |
| H | ? | upgrade.rs | 800 |
| H | ? | upgrade.rs | 802 |
| H | ? | toolchain.rs | 48 |
| H | ? | toolchain.rs | 50 |
| H | ? | run.rs | 287 |
| H | ? | run.rs | 411 |
| H | ? | run.rs | 548 |
| H | ? | run.rs | 1051 |
| H | ? | run.rs | 1349 |
| H | ? | run.rs | 1446 |
| H | ? | run.rs | 1547 |
| H | ? | run.rs | 1552 |
| H | ? | run.rs | 1557 |
| H | ? | run.rs | 1588 |
| H | ? | run.rs | 1599 |
| H | ? | run.rs | 1613 |
| H | ? | run.rs | 1626 |
| H | ? | run.rs | 1780 |
| H | ? | run.rs | 1784 |
| H | ? | run.rs | 1811 |
| H | ? | run.rs | 1815 |
| H | ? | add.rs | 155 |
| H | ? | add.rs | 161 |
| H | ? | add.rs | 344 |
| H | ? | add.rs | 396 |
| H | ? | add.rs | 397 |
| H | ? | add.rs | 408 |
| H | ? | add.rs | 412 |
| H | ? | add.rs | 436 |
| H | ? | add.rs | 447 |
| H | ? | add.rs | 453 |
| H | ? | add.rs | 462 |
| H | ? | add.rs | 472 |
| H | ? | add.rs | 477 |
| H | ? | add.rs | 488 |
| H | ? | add.rs | 734 |
| H | ? | add.rs | 767 |
| H | ? | add.rs | 768 |
| H | ? | add.rs | 938 |
| H | ? | add.rs | 965 |
| H | ? | add.rs | 973 |
| H | ? | add.rs | 974 |
| H | ? | add.rs | 975 |
| H | ? | add.rs | 983 |
| H | ? | add.rs | 989 |
| H | ? | add.rs | 993 |
| H | ? | add.rs | 994 |
| H | ? | add.rs | 1163 |
| H | ? | add.rs | 1298 |
| H | ? | add.rs | 1446 |
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
| H | ? | environment.rs | 164 |
| H | ? | environment.rs | 221 |
| H | ? | environment.rs | 282 |
| H | ? | environment.rs | 283 |
| H | ? | environment.rs | 326 |
| H | ? | environment.rs | 395 |
| H | ? | environment.rs | 419 |
| H | ? | environment.rs | 421 |
| H | ? | editable.rs | 37 |
| H | ? | editable.rs | 38 |
| H | ? | editable.rs | 41 |
| H | ? | editable.rs | 43 |
| H | ? | settings.rs | 107 |
| H | ? | settings.rs | 376 |
| H | ? | settings.rs | 382 |
| H | ? | settings.rs | 387 |
| H | ? | settings.rs | 388 |
| H | ? | settings.rs | 389 |
| H | ? | settings.rs | 437 |
| H | ? | settings.rs | 496 |
| H | ? | settings.rs | 765 |
| H | ? | settings.rs | 766 |
| H | ? | settings.rs | 816 |
| H | ? | settings.rs | 960 |
| H | ? | settings.rs | 965 |
| H | ? | settings.rs | 968 |
| H | ? | settings.rs | 1085 |
| H | ? | settings.rs | 1090 |
| H | ? | settings.rs | 1093 |
| H | ? | settings.rs | 1234 |
| H | ? | settings.rs | 1251 |
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
| H | ? | settings.rs | 1946 |
| H | ? | settings.rs | 2020 |
| H | ? | settings.rs | 2021 |
| H | ? | settings.rs | 2072 |
| H | ? | settings.rs | 2073 |
| H | ? | settings.rs | 2078 |
| H | ? | settings.rs | 2128 |
| H | ? | settings.rs | 2129 |
| H | ? | settings.rs | 2305 |
| H | ? | settings.rs | 2350 |
| H | ? | settings.rs | 2510 |
| H | ? | settings.rs | 2511 |
| H | ? | settings.rs | 2602 |
| H | ? | settings.rs | 2603 |
| H | ? | settings.rs | 2699 |
| H | ? | settings.rs | 2700 |
| H | ? | settings.rs | 2724 |
| H | ? | settings.rs | 2841 |
| H | ? | settings.rs | 2842 |
| H | ? | settings.rs | 2887 |
| H | ? | settings.rs | 3040 |
| H | ? | settings.rs | 3041 |
| H | ? | settings.rs | 3080 |
| H | ? | settings.rs | 3153 |
| H | ? | settings.rs | 3154 |
| H | ? | settings.rs | 3159 |
| H | ? | settings.rs | 3185 |
| H | ? | settings.rs | 3190 |
| H | ? | settings.rs | 3236 |
| H | ? | settings.rs | 3242 |
| H | ? | settings.rs | 3341 |
| H | ? | settings.rs | 3357 |
| H | ? | settings.rs | 3366 |
| H | ? | settings.rs | 3378 |
| H | ? | settings.rs | 3386 |
| H | ? | settings.rs | 3646 |
| H | ? | settings.rs | 3662 |
| H | ? | settings.rs | 3671 |
| H | ? | settings.rs | 4109 |
| H | ? | settings.rs | 4115 |
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
| H | ? | settings.rs | 5189 |
| H | ? | lib.rs | 125 |
| H | ? | lib.rs | 302 |
| H | ? | lib.rs | 477 |
| H | ? | lib.rs | 635 |
| H | ? | lib.rs | 642 |
| H | ? | lib.rs | 643 |
| H | ? | lib.rs | 644 |
| H | ? | lib.rs | 741 |
| H | ? | lib.rs | 742 |
| H | ? | lib.rs | 818 |
| H | ? | lib.rs | 860 |
| H | ? | lib.rs | 861 |
| H | ? | lib.rs | 906 |
| H | ? | lib.rs | 1004 |
| H | ? | lib.rs | 1017 |
| H | ? | lib.rs | 1031 |
| H | ? | lib.rs | 1032 |
| H | ? | lib.rs | 1067 |
| H | ? | lib.rs | 1303 |
| H | ? | lib.rs | 1371 |
| H | ? | lib.rs | 1372 |
| H | ? | lib.rs | 1506 |
| H | ? | lib.rs | 1540 |
| H | ? | lib.rs | 1541 |
| H | ? | lib.rs | 1631 |
| H | ? | lib.rs | 1632 |
| H | ? | lib.rs | 1633 |
| H | ? | lib.rs | 1661 |
| H | ? | lib.rs | 2056 |
| H | ? | lib.rs | 2057 |
| H | ? | lib.rs | 2170 |
| H | ? | lib.rs | 2299 |
| H | ? | lib.rs | 2300 |
| H | ? | lib.rs | 2370 |
| H | ? | lib.rs | 2371 |
| H | ? | lib.rs | 2427 |
| H | ? | lib.rs | 2428 |
| H | ? | lib.rs | 2475 |
| H | ? | lib.rs | 2546 |
| H | ? | lib.rs | 2559 |
| H | ? | lib.rs | 2573 |
| H | ? | lib.rs | 2574 |
| H | ? | lib.rs | 2642 |
| H | ? | lib.rs | 2643 |
| H | ? | lib.rs | 2697 |
| H | ? | lib.rs | 2698 |
| H | ? | lib.rs | 2868 |
| H | ? | lib.rs | 2869 |
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
| H | ? | interpreter.rs | 1228 |
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
| H | ? | lib.rs | 1040 |
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
| H | ? | virtualenv.rs | 231 |
| H | ? | virtualenv.rs | 245 |
| H | ? | virtualenv.rs | 248 |
| H | ? | virtualenv.rs | 251 |
| H | ? | virtualenv.rs | 492 |
| H | ? | virtualenv.rs | 541 |
| H | ? | lib.rs | 131 |
| H | ? | generate_scenarios.rs | 85 |
| H | ? | generate_scenarios.rs | 709 |
| H | ? | generate_scenarios.rs | 710 |
| H | ? | generate_scenarios.rs | 896 |
| H | ? | generate_scenarios.rs | 911 |
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
| H | ? | build_requires.rs | 134 |
| H | ? | build_requires.rs | 158 |
| H | ? | build_requires.rs | 210 |
| H | ? | build_requires.rs | 234 |
| H | ? | build_requires.rs | 301 |
| H | ? | build_requires.rs | 329 |
| H | ? | lowering.rs | 101 |
| H | ? | lowering.rs | 110 |
| H | ? | lowering.rs | 118 |
| H | ? | lowering.rs | 126 |
| H | ? | lowering.rs | 134 |
| H | ? | lowering.rs | 147 |
| H | ? | lowering.rs | 177 |
| H | ? | lowering.rs | 256 |
| H | ? | lowering.rs | 265 |
| H | ? | lowering.rs | 270 |
| H | ? | lowering.rs | 273 |
| H | ? | lowering.rs | 307 |
| H | ? | lowering.rs | 308 |
| H | ? | lowering.rs | 312 |
| H | ? | lowering.rs | 373 |
| H | ? | lowering.rs | 444 |
| H | ? | lowering.rs | 453 |
| H | ? | lowering.rs | 487 |
| H | ? | lowering.rs | 488 |
| H | ? | lowering.rs | 492 |
| H | ? | lowering.rs | 627 |
| H | ? | lowering.rs | 717 |
| H | ? | lowering.rs | 755 |
| H | ? | lowering.rs | 770 |
| H | ? | lowering.rs | 771 |
| H | ? | lowering.rs | 801 |
| H | ? | lowering.rs | 836 |
| H | ? | lowering.rs | 875 |
| H | ? | lowering.rs | 883 |
| H | ? | lowering.rs | 998 |
| H | ? | lowering.rs | 1010 |
| H | ? | lowering.rs | 1011 |
| H | ? | lowering.rs | 1024 |
| H | ? | lowering.rs | 1031 |
| H | ? | lowering.rs | 1033 |
| H | ? | lowering.rs | 1034 |
| H | ? | requires_dist.rs | 88 |
| H | ? | requires_dist.rs | 157 |
| H | ? | requires_dist.rs | 181 |
| H | ? | requires_dist.rs | 182 |
| H | ? | requires_dist.rs | 201 |
| H | ? | requires_dist.rs | 225 |
| H | ? | requires_dist.rs | 256 |
| H | ? | requires_dist.rs | 257 |
| H | ? | requires_dist.rs | 267 |
| H | ? | requires_dist.rs | 268 |
| H | ? | requires_dist.rs | 277 |
| H | ? | requires_dist.rs | 278 |
| H | ? | requires_dist.rs | 289 |
| H | ? | requires_dist.rs | 290 |
| H | ? | requires_dist.rs | 385 |
| H | ? | requires_dist.rs | 398 |
| H | ? | requires_dist.rs | 399 |
| H | ? | requires_dist.rs | 400 |
| H | ? | requires_dist.rs | 401 |
| H | ? | requires_dist.rs | 402 |
| H | ? | requires_dist.rs | 432 |
| H | ? | requires_dist.rs | 434 |
| H | ? | requires_dist.rs | 435 |
| H | ? | requires_dist.rs | 436 |
| H | ? | dependency_groups.rs | 153 |
| H | ? | dependency_groups.rs | 177 |
| H | ? | dependency_groups.rs | 178 |
| H | ? | dependency_groups.rs | 209 |
| H | ? | dependency_groups.rs | 210 |
| H | ? | dependency_groups.rs | 221 |
| H | ? | dependency_groups.rs | 222 |
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
| H | ? | error.rs | 422 |
| H | ? | error.rs | 423 |
| H | ? | error.rs | 444 |
| H | ? | error.rs | 445 |
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
| H | ? | lib.rs | 683 |
| H | ? | lib.rs | 758 |
| H | ? | lib.rs | 768 |
| H | ? | lib.rs | 872 |
| H | ? | settings.rs | 2367 |
| H | ? | settings.rs | 2653 |
| H | ? | settings.rs | 2875 |
| H | ? | settings.rs | 2876 |
| H | ? | combine.rs | 256 |
| H | ? | combine.rs | 257 |
| H | ? | lib.rs | 134 |
| H | ? | lib.rs | 286 |
| H | ? | lib.rs | 951 |
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
| H | ? | specification.rs | 517 |
| H | ? | specification.rs | 522 |
| H | ? | specification.rs | 573 |
| H | ? | specification.rs | 574 |
| H | ? | specification.rs | 612 |
| H | ? | specification.rs | 613 |
| H | ? | specification.rs | 639 |
| H | ? | specification.rs | 640 |
| H | ? | specification.rs | 742 |
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
| H | ? | osv.rs | 252 |
| H | ? | osv.rs | 287 |
| H | ? | osv.rs | 301 |
| H | ? | osv.rs | 332 |
| H | ? | osv.rs | 335 |
| H | ? | osv.rs | 381 |
| H | ? | osv.rs | 398 |
| H | ? | osv.rs | 415 |
| H | ? | osv.rs | 451 |
| H | ? | osv.rs | 499 |
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
| H | ? | verbatim_url.rs | 165 |
| H | ? | verbatim_url.rs | 166 |
| H | ? | verbatim_url.rs | 206 |
| H | ? | verbatim_url.rs | 301 |
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
| H | ? | lib.rs | 774 |
| H | ? | lib.rs | 793 |
| H | ? | lib.rs | 799 |
| H | ? | wheel.rs | 219 |
| H | ? | wheel.rs | 624 |
| H | ? | linker.rs | 70 |
| H | ? | linker.rs | 184 |
| H | ? | install.rs | 77 |
| H | ? | install.rs | 80 |
| H | ? | install.rs | 81 |
| H | ? | script.rs | 131 |
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
*Сгенерировано GSC v0.6 · 2026-07-25T04:03:10.488279*