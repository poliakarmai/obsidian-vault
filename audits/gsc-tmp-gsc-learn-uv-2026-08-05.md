---
title: "GSC Audit: /tmp/gsc-learn/uv"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/uv

**Дата:** 05.08.2026 04:03  
**Путь:** `/tmp/gsc-learn/uv`  
**Всего находок:** 3617  
**CRITICAL:** 119 | **HIGH:** 3204 | **MEDIUM:** 100 | **LOW:** 187

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 3092 |
| GS003 | 185 |
| Хардкод IP адреса | 104 |
| GS001 | 95 |
| Синхронный код в async | 47 |
| Python: assert in production | 29 |
| Hardcoded encryption key | 24 |
| Outdated dependency pattern | 24 |
| GS022 | 4 |
| GS002 | 2 |
| GS014 | 2 |
| GS017 | 2 |
| CVE-2026-56233: Path traversal | 1 |
| World-readable file: uv.schema.json (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: mkdocs.yml (664) | 1 |
| GS007 | 1 |
| GS009 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | login.rs | 142 | Found: password: ";
                uv_console::password(pro |
| CRITICAL | GS001 | publish.rs | 600 | Found: password: ";
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
| CRITICAL | GS001 | registry_client.rs | 2091 | Found: password = "password" |
| CRITICAL | GS001 | registry_client.rs | 2147 | Found: password = "password" |
| CRITICAL | GS001 | registry_client.rs | 2197 | Found: password = "password" |
| CRITICAL | GS001 | mock.rs | 246 | Found: password = "test ascii password" |
| CRITICAL | GS001 | secret_service.rs | 64 | Found: Password: " pass
    echo -n " |
| CRITICAL | GS001 | secret_service.rs | 771 | Found: password = "password in new collection" |
| CRITICAL | GS001 | windows.rs | 751 | Found: password = "test get password" |
| CRITICAL | GS001 | abi_tag.rs | 504 | Found: "cp37m" |
| CRITICAL | GS001 | abi_tag.rs | 505 | Found: "cp37m" |
| CRITICAL | GS001 | abi_tag.rs | 508 | Found: "cp313t" |
| CRITICAL | GS001 | abi_tag.rs | 509 | Found: "cp313t" |
| CRITICAL | GS001 | abi_tag.rs | 523 | Found: "cp39y" |
| CRITICAL | GS001 | abi_tag.rs | 526 | Found: "cp39dd" |
| CRITICAL | GS001 | tags.rs | 3012 | Found: "cp314" |
| CRITICAL | GS001 | tags.rs | 3013 | Found: "cp314d" |
| CRITICAL | GS001 | tags.rs | 3017 | Found: "cp314" |
| CRITICAL | GS001 | tags.rs | 3018 | Found: "cp314" |
| CRITICAL | GS001 | tags.rs | 3039 | Found: "cp314" |
| CRITICAL | GS001 | tags.rs | 3040 | Found: "cp314" |
| CRITICAL | GS001 | ruff.toml | 6 | Found: "UP036" |
| CRITICAL | GS001 | ruff.toml | 8 | Found: "UP031" |
| CRITICAL | GS001 | ruff.toml | 8 | Found: "UP037" |
| CRITICAL | GS001 | discovery.rs | 3927 | Found: "pp310" |
| CRITICAL | GS001 | discovery.rs | 3941 | Found: "gp310" |
| CRITICAL | GS001 | backend.rs | 947 | Found: "cu132" |
| CRITICAL | GS001 | backend.rs | 948 | Found: "cu130" |
| CRITICAL | GS001 | backend.rs | 949 | Found: "cu129" |
| CRITICAL | GS001 | backend.rs | 950 | Found: "cu128" |
| CRITICAL | GS001 | backend.rs | 951 | Found: "cu126" |
| CRITICAL | GS001 | backend.rs | 952 | Found: "cu125" |
| CRITICAL | GS001 | backend.rs | 953 | Found: "cu124" |
| CRITICAL | GS001 | backend.rs | 954 | Found: "cu123" |
| CRITICAL | GS001 | backend.rs | 955 | Found: "cu122" |
| CRITICAL | GS001 | backend.rs | 956 | Found: "cu121" |
| CRITICAL | GS001 | backend.rs | 957 | Found: "cu120" |
| CRITICAL | GS001 | backend.rs | 958 | Found: "cu118" |
| CRITICAL | GS001 | backend.rs | 959 | Found: "cu117" |
| CRITICAL | GS001 | backend.rs | 960 | Found: "cu116" |
| CRITICAL | GS001 | backend.rs | 961 | Found: "cu115" |
| CRITICAL | GS001 | backend.rs | 962 | Found: "cu114" |
| CRITICAL | GS001 | backend.rs | 963 | Found: "cu113" |
| CRITICAL | GS001 | backend.rs | 964 | Found: "cu112" |
| CRITICAL | GS001 | backend.rs | 965 | Found: "cu111" |
| CRITICAL | GS001 | backend.rs | 966 | Found: "cu110" |
| CRITICAL | GS001 | backend.rs | 967 | Found: "cu102" |
| CRITICAL | GS001 | backend.rs | 968 | Found: "cu101" |
| CRITICAL | GS001 | backend.rs | 969 | Found: "cu100" |
| CRITICAL | GS001 | ruff.toml | 1 | Found: "py312" |
| CRITICAL | GS001 | ruff.toml | 20 | Found: "FA100" |
| CRITICAL | GS001 | ruff.toml | 20 | Found: "UP036" |
| CRITICAL | GS001 | uv.schema.json | 2563 | Found: "cu132" |
| CRITICAL | GS001 | uv.schema.json | 2568 | Found: "cu130" |
| CRITICAL | GS001 | uv.schema.json | 2573 | Found: "cu129" |
| CRITICAL | GS001 | uv.schema.json | 2578 | Found: "cu128" |
| CRITICAL | GS001 | uv.schema.json | 2583 | Found: "cu126" |
| CRITICAL | GS001 | uv.schema.json | 2588 | Found: "cu125" |
| CRITICAL | GS001 | uv.schema.json | 2593 | Found: "cu124" |
| CRITICAL | GS001 | uv.schema.json | 2598 | Found: "cu123" |
| CRITICAL | GS001 | uv.schema.json | 2603 | Found: "cu122" |
| CRITICAL | GS001 | uv.schema.json | 2608 | Found: "cu121" |
| CRITICAL | GS001 | uv.schema.json | 2613 | Found: "cu120" |
| CRITICAL | GS001 | uv.schema.json | 2618 | Found: "cu118" |
| CRITICAL | GS001 | uv.schema.json | 2623 | Found: "cu117" |
| CRITICAL | GS001 | uv.schema.json | 2628 | Found: "cu116" |
| CRITICAL | GS001 | uv.schema.json | 2633 | Found: "cu115" |
| CRITICAL | GS001 | uv.schema.json | 2638 | Found: "cu114" |
| CRITICAL | GS001 | uv.schema.json | 2643 | Found: "cu113" |
| CRITICAL | GS001 | uv.schema.json | 2648 | Found: "cu112" |
| CRITICAL | GS001 | uv.schema.json | 2653 | Found: "cu111" |
| CRITICAL | GS001 | uv.schema.json | 2658 | Found: "cu110" |
| CRITICAL | GS001 | uv.schema.json | 2663 | Found: "cu102" |
| CRITICAL | GS001 | uv.schema.json | 2668 | Found: "cu101" |
| CRITICAL | GS001 | uv.schema.json | 2673 | Found: "cu100" |
| CRITICAL | ? | registry_client.rs | 2091 | Match:         let password = "password"; |
| CRITICAL | ? | registry_client.rs | 2147 | Match:         let password = "password"; |
| CRITICAL | ? | registry_client.rs | 2197 | Match:         let password = "password"; |
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
| HIGH | ? | lib.rs | 1333 | Match:         let listener = std::net::TcpListener::bind("1 |
| HIGH | ? | pyproject_mut.rs | 2076 | Match:             ("0.0.0.1", "==0.0.0.1"), |
| HIGH | ? | pyproject_mut.rs | 2080 | Match:             ("1.2.3.4", "==1.2.3.4"), |
| HIGH | ? | pyproject_mut.rs | 2081 | Match:             ("1.2.3.4a1.post1", "==1.2.3.4a1.post1"), |
| HIGH | ? | pyproject_mut.rs | 2100 | Match:             ("0.0.0.1", ">=0.0.0.1"), |
| HIGH | ? | pyproject_mut.rs | 2105 | Match:             ("1.2.3.4", ">=1.2.3.4"), |
| HIGH | ? | pyproject_mut.rs | 2106 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1"), |
| HIGH | ? | pyproject_mut.rs | 2123 | Match:             ("0.0.0.0", ">=0.0.0.0, <0.1.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2126 | Match:             ("0.0.1.1", ">=0.0.1.1, <0.0.2.0"), |
| HIGH | ? | pyproject_mut.rs | 2127 | Match:             ("0.0.0.1", ">=0.0.0.1, <0.0.0.2"), |
| HIGH | ? | pyproject_mut.rs | 2132 | Match:             ("1.2.3.4", ">=1.2.3.4, <2.0.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2133 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1, < |
| HIGH | ? | pyproject_mut.rs | 2150 | Match:             ("0.0.0.0", ">=0.0.0.0, <0.0.1.0"), |
| HIGH | ? | pyproject_mut.rs | 2153 | Match:             ("0.0.1.1", ">=0.0.1.1, <0.0.2.0"), |
| HIGH | ? | pyproject_mut.rs | 2154 | Match:             ("0.0.0.1", ">=0.0.0.1, <0.0.0.2"), |
| HIGH | ? | pyproject_mut.rs | 2159 | Match:             ("1.2.3.4", ">=1.2.3.4, <1.3.0.0"), |
| HIGH | ? | pyproject_mut.rs | 2160 | Match:             ("1.2.3.4a1.post1", ">=1.2.3.4a1.post1, < |
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
| HIGH | ? | tree.rs | 2782 | Match:             ("3.9.0.0.*", "3.9", "3.9.*"), |
| HIGH | ? | tree.rs | 2799 | Match:         let cases_false = ["3.9.1.*", "3.9.1.0.*", "3 |
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
| HIGH | GS017 | check-release-artifact-sboms.sh | 29 | Password length = 1 chars. |
| HIGH | GS017 | registries-test.py | 109 | Password length = 4 chars. |
| HIGH | ? | lib.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | candidate_selector.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | candidate_selector.rs | 902 | Clone in performance-critical code — consider references |
| HIGH | ? | candidate_selector.rs | 904 | Clone in performance-critical code — consider references |
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
| HIGH | ? | flat_index.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 139 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 476 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 583 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 722 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 740 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 863 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 868 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 897 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 926 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 927 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 949 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 950 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1000 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1072 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1075 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1091 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1109 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1128 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1130 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1173 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1186 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1187 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1188 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1201 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1203 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1216 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1218 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1229 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1231 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1258 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1259 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1271 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2131 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2139 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2198 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2398 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2413 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2568 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2586 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2719 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2807 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2873 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2874 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3042 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3224 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3231 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3234 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3253 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3259 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3268 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3278 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3301 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3306 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3714 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3853 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3871 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3943 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3964 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3976 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3979 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3984 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3994 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4009 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4016 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4017 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4022 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4027 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4035 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4042 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4049 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4069 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4080 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4084 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4088 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4092 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4097 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4103 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4143 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4152 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4160 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4171 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4183 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4195 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4212 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4221 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4230 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4231 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4236 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4239 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4246 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4247 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4251 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4254 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4264 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4273 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4279 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4280 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4284 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4286 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4306 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4307 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4312 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4316 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4324 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4329 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4339 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4340 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4363 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4379 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4380 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4388 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4392 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4400 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4416 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4417 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4526 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4530 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4532 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4544 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4608 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4666 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4670 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4671 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4684 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4751 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4753 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4789 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4793 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4799 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4807 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4933 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5011 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5036 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5055 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5059 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5116 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5320 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5774 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5792 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5810 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 5856 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6065 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6110 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6118 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6123 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6131 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6136 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6146 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6152 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6165 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6175 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6193 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6216 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6226 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6330 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6500 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6647 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6658 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6666 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6667 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6691 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6702 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6710 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6711 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6817 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6818 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6957 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6981 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 6997 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 7001 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 89 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 92 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 97 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 140 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 497 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 551 | Clone in performance-critical code — consider references |
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
| HIGH | ? | pylock_toml.rs | 418 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 470 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 480 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 521 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 538 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 542 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 615 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 701 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 754 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 865 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 871 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 906 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 910 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 921 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 949 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 971 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1103 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1105 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1113 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1114 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1115 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1130 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1134 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1137 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1142 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1146 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1149 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1153 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1157 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1162 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1165 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1183 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1203 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1252 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1266 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1269 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1272 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1274 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1277 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1283 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1430 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1435 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1451 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1458 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1463 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1485 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1489 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1498 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1506 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1540 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1556 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1561 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1568 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1575 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1586 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1587 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1591 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1593 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1607 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1613 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1617 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1648 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1652 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1661 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1669 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1679 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1703 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1726 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1737 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1745 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1746 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1752 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1753 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1754 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1756 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1762 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1774 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1782 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock_toml.rs | 1787 | Clone in performance-critical code — consider references |
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
| HIGH | ? | installable.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 471 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 533 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 635 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 718 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 719 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 720 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 721 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 790 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 853 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 854 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 911 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 917 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 975 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 982 | Clone in performance-critical code — consider references |
| HIGH | ? | installable.rs | 1431 | Clone in performance-critical code — consider references |
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
| HIGH | ? | report.rs | 1372 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1373 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1388 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1389 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1395 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1396 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1794 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1801 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1802 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1854 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1864 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1866 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1971 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 1992 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2011 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2081 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2474 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2486 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2487 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2520 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2522 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2525 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2526 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2535 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2541 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2785 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2787 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2789 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2790 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2793 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2794 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2795 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2796 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2817 | Clone in performance-critical code — consider references |
| HIGH | ? | report.rs | 2819 | Clone in performance-critical code — consider references |
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
| HIGH | ? | version_map.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 689 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 704 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 752 | Clone in performance-critical code — consider references |
| HIGH | ? | version_map.rs | 806 | Clone in performance-critical code — consider references |
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
| HIGH | ? | prerelease.rs | 208 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 234 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 250 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 338 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 339 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 340 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 345 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 377 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 457 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 878 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 881 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 938 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 999 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1003 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1012 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1014 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1018 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1019 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1067 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1069 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1070 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1071 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1105 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1119 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1124 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1154 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1169 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1215 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1229 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1237 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1239 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1276 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1289 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1306 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1308 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1314 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1338 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1346 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1353 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1359 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1365 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1396 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1399 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1442 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1485 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1540 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1587 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1588 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1711 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1713 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1716 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1718 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1746 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1747 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1755 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1779 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1788 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1889 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1909 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1932 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1935 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1943 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1945 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1954 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2011 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2016 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2039 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2044 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2065 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2067 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2070 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2150 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2171 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2172 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2173 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2174 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2175 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2203 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2205 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2206 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2207 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2282 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2380 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2381 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2382 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2383 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2384 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2417 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2418 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2419 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2420 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2421 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2566 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2595 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2596 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2611 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2612 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2636 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2643 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2650 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2695 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2701 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2705 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2754 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2766 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2775 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2808 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2821 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2823 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2849 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2858 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2861 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2886 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2909 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2916 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2929 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2933 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2934 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2935 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2936 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2943 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2944 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2945 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3217 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3218 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3222 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3228 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3248 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3395 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3409 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3535 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3540 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3541 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3544 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3545 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3567 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3572 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3573 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3599 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3604 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3605 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3608 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3617 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3622 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3623 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3649 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3654 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3655 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3659 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3683 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3684 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3685 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3752 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3872 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3914 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3943 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3962 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3983 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3989 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4000 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4007 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4047 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4104 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4116 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 4325 | Clone in performance-critical code — consider references |
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
| HIGH | ? | flat_index.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 178 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 217 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 223 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | flat_index.rs | 378 | Clone in performance-critical code — consider references |
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
| HIGH | ? | registry_client.rs | 1097 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1129 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1136 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1144 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1147 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1208 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1215 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1221 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1240 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1242 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1243 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1246 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1251 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1266 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1282 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1294 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1304 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1376 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1575 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1646 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1711 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1779 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1797 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1798 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 1827 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 2126 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 2176 | Clone in performance-critical code — consider references |
| HIGH | ? | registry_client.rs | 2226 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 456 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 476 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 485 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 487 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 495 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 512 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 516 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 518 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 531 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 625 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 668 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 690 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 698 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 700 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 712 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 803 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 953 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1088 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1194 | Clone in performance-critical code — consider references |
| HIGH | ? | base_client.rs | 1200 | Clone in performance-critical code — consider references |
| HIGH | ? | retry.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | middleware.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 110 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 295 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 387 | Clone in performance-critical code — consider references |
| HIGH | ? | tls.rs | 417 | Clone in performance-critical code — consider references |
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
| HIGH | ? | compile.rs | 517 | Clone in performance-critical code — consider references |
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
| HIGH | ? | source_dist.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 211 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 212 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 493 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | source_dist.rs | 514 | Clone in performance-critical code — consider references |
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
| HIGH | ? | package_options.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | package_options.rs | 188 | Clone in performance-critical code — consider references |
| HIGH | ? | package_options.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | package_options.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | constraints.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | constraints.rs | 78 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 557 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 620 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 673 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 795 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 810 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 836 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1212 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1215 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1251 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1353 | Clone in performance-critical code — consider references |
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
| HIGH | ? | pyproject_mut.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 556 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 594 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 597 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1410 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1556 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1582 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1596 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1602 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1689 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject_mut.rs | 1716 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1698 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1699 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1705 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1706 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1707 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1834 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1847 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1873 | Clone in performance-critical code — consider references |
| HIGH | ? | pyproject.rs | 1886 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 679 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 683 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 689 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 696 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | parsed_url.rs | 728 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1128 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1131 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1134 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1137 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1629 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6230 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6231 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6232 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6293 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6294 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 6295 | Clone in performance-critical code — consider references |
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
| HIGH | ? | prioritized_distribution.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | prioritized_distribution.rs | 543 | Clone in performance-critical code — consider references |
| HIGH | ? | prioritized_distribution.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | prioritized_distribution.rs | 568 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 526 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | index_url.rs | 774 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 818 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 840 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 851 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 852 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 862 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 863 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 872 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 873 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 883 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 884 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 894 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1041 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1074 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1075 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1437 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1441 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1790 | Clone in performance-critical code — consider references |
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
| HIGH | ? | sync.rs | 326 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 327 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 405 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 427 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 452 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 470 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 475 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 523 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 527 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 364 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 466 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 509 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 513 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 523 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 550 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 566 | Clone in performance-critical code — consider references |
| HIGH | ? | compile.rs | 588 | Clone in performance-critical code — consider references |
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
| HIGH | ? | install.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 455 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 457 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 515 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 526 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 528 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 547 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 572 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 596 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 646 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 656 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 660 | Clone in performance-critical code — consider references |
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
| HIGH | ? | build_frontend.rs | 775 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1170 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1171 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1176 | Clone in performance-critical code — consider references |
| HIGH | ? | build_frontend.rs | 1177 | Clone in performance-critical code — consider references |
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
| HIGH | ? | publish.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 276 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 278 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 646 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 661 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 670 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 682 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 695 | Clone in performance-critical code — consider references |
| HIGH | ? | publish.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 138 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 342 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 437 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 439 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 462 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 490 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 500 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 501 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 510 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 674 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 792 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 807 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 816 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 820 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 826 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 913 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 940 | Clone in performance-critical code — consider references |
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
| HIGH | ? | audit.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 211 | Clone in performance-critical code — consider references |
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
| HIGH | ? | install.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 637 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 645 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 651 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 653 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 716 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1014 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1029 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1032 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1034 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1081 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1154 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1168 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1176 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1190 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1193 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1195 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1200 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1211 | Clone in performance-critical code — consider references |
| HIGH | ? | install.rs | 1219 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 108 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | uninstall.rs | 216 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 128 | Clone in performance-critical code — consider references |
| HIGH | ? | module_owners.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | help.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | pylock.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 53 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 398 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | lock_target.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 658 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 659 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 668 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 675 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 696 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 697 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 703 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 704 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 709 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 710 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1009 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1022 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1029 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1233 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1250 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1645 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1698 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1741 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1747 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2315 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2331 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2340 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2341 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2343 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2354 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2358 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2372 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2384 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2394 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2395 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2397 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2398 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2410 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2521 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2566 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2573 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2574 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2576 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2586 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2590 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2597 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2599 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2601 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2620 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2652 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2664 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2674 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2675 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2677 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2678 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2752 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2761 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2762 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2794 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2806 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2816 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2820 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2924 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3009 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3016 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3017 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3019 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3035 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3037 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3039 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3071 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3081 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3082 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3084 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3085 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3102 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3107 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3228 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3232 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3234 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3267 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3272 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3274 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3469 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 275 | Clone in performance-critical code — consider references |
| HIGH | ? | version.rs | 419 | Clone in performance-critical code — consider references |
| HIGH | ? | ty.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 480 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 575 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | install_target.rs | 584 | Clone in performance-critical code — consider references |
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
| HIGH | ? | check.rs | 93 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 197 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 229 | Clone in performance-critical code — consider references |
| HIGH | ? | check.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 246 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 292 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 772 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 782 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 785 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 790 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 797 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 798 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 809 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 813 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 830 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 832 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 835 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 858 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 904 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 905 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 907 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 908 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 915 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1060 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1061 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1077 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1100 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1111 | Clone in performance-critical code — consider references |
| HIGH | ? | lock.rs | 1690 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 280 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 351 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 469 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 473 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 474 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 475 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 479 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 484 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 636 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 640 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 642 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 655 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 657 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 664 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 669 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 695 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 781 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 987 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 988 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 1024 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 1031 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 1039 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 1056 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 1092 | Clone in performance-critical code — consider references |
| HIGH | ? | upgrade.rs | 1094 | Clone in performance-critical code — consider references |
| HIGH | ? | toolchain.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | toolchain.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 288 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 412 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1052 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1350 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1447 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1537 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1542 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1547 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1578 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1589 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1603 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1616 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1770 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1774 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1801 | Clone in performance-critical code — consider references |
| HIGH | ? | run.rs | 1805 | Clone in performance-critical code — consider references |
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
| HIGH | ? | export.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | export.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 463 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | init.rs | 545 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 54 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 55 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 65 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 66 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 195 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 334 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | sarif.rs | 382 | Clone in performance-critical code — consider references |
| HIGH | ? | json.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | json.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | json.rs | 199 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 304 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 307 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 313 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 319 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | audit.rs | 350 | Clone in performance-critical code — consider references |
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
| HIGH | ? | settings.rs | 109 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 447 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 504 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 748 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 749 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 799 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 944 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 949 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 952 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1069 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1074 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1077 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1204 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1221 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1324 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1439 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1440 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1441 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1450 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1456 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1462 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1529 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1620 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1734 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1790 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1890 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1891 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 1989 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2063 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2064 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2112 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2113 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2122 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2174 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2175 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2392 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2450 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2554 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2555 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2647 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2648 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2748 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2749 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2773 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2889 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2890 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2935 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3089 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3090 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3127 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3203 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3204 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3209 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3235 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3240 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3282 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3288 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3387 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3403 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3412 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3424 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3432 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3698 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3714 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 3723 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4164 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4170 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4415 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4418 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4421 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4433 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4529 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4544 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4547 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4550 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4833 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 4942 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 5066 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 5274 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 148 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 308 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 483 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 739 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 815 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 858 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 859 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 904 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1003 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1016 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1030 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1031 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1066 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1309 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1377 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1378 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1510 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1544 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1545 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1635 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1636 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1637 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 1665 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2084 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2085 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2198 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2314 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2315 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2385 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2386 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2442 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2443 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2490 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2562 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2575 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2589 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2590 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2658 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2659 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2713 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2714 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2884 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 2885 | Clone in performance-critical code — consider references |
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
| HIGH | ? | lib.rs | 1043 | Clone in performance-critical code — consider references |
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
| HIGH | ? | virtualenv.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 235 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 238 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 241 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 482 | Clone in performance-critical code — consider references |
| HIGH | ? | virtualenv.rs | 542 | Clone in performance-critical code — consider references |
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
| HIGH | ? | hash.rs | 224 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 393 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 394 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 477 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 478 | Clone in performance-critical code — consider references |
| HIGH | ? | hash.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | builds.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 88 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 204 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 232 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 239 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 270 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 277 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 297 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 309 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 335 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 353 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 371 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 454 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 467 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 588 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 638 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 781 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 789 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 817 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 992 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1000 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1028 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1111 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1118 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1128 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1135 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1140 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1147 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1195 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1200 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1205 | Clone in performance-critical code — consider references |
| HIGH | ? | distribution_database.rs | 1212 | Clone in performance-critical code — consider references |
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
| HIGH | ? | mod.rs | 997 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1003 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1039 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1328 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1449 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1509 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1565 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1588 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1617 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1653 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1684 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1703 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1754 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1762 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1862 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 1972 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2139 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2198 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2331 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2367 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2405 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2433 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2462 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2500 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2531 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2588 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2790 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2802 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 2804 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3036 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3084 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3175 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3185 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3196 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3197 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3525 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3526 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3532 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3534 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3535 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3547 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3548 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3554 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 3555 | Clone in performance-critical code — consider references |
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
| HIGH | ? | uv.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 379 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 380 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 399 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 465 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 503 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 548 | Clone in performance-critical code — consider references |
| HIGH | ? | uv.rs | 567 | Clone in performance-critical code — consider references |
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
| HIGH | ? | stream.rs | 124 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 207 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 222 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 279 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 396 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 403 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 413 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 424 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 436 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 460 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 468 | Clone in performance-critical code — consider references |
| HIGH | ? | stream.rs | 540 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 61 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 104 | Clone in performance-critical code — consider references |
| HIGH | ? | sync.rs | 112 | Clone in performance-critical code — consider references |
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
| HIGH | ? | settings.rs | 2465 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2757 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2980 | Clone in performance-critical code — consider references |
| HIGH | ? | settings.rs | 2981 | Clone in performance-critical code — consider references |
| HIGH | ? | combine.rs | 271 | Clone in performance-critical code — consider references |
| HIGH | ? | combine.rs | 272 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 134 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 286 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 955 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 254 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | backend.rs | 267 | Clone in performance-critical code — consider references |
| HIGH | ? | unnamed.rs | 306 | Clone in performance-critical code — consider references |
| HIGH | ? | unnamed.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 146 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 149 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 169 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 175 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 183 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 198 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 266 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 305 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 311 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 314 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 337 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 347 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 357 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 372 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 494 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 499 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 576 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 616 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 617 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 644 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 645 | Clone in performance-critical code — consider references |
| HIGH | ? | specification.rs | 748 | Clone in performance-critical code — consider references |
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
| HIGH | ? | tree.rs | 1190 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 3666 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 3671 | Clone in performance-critical code — consider references |
| HIGH | ? | tree.rs | 3678 | Clone in performance-critical code — consider references |
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
| HIGH | ? | unnamed.rs | 400 | Clone in performance-critical code — consider references |
| HIGH | ? | unnamed.rs | 411 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 165 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | verbatim_url.rs | 301 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | cursor.rs | 85 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 730 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 741 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 946 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 974 | Clone in performance-critical code — consider references |
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
| HIGH | ? | wheel.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | wheel.rs | 699 | Clone in performance-critical code — consider references |
| HIGH | ? | linker.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | linker.rs | 185 | Clone in performance-critical code — consider references |
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
| C | GS001 | publish.rs | 600 |
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
| C | GS001 | registry_client.rs | 2091 |
| C | GS001 | registry_client.rs | 2147 |
| C | GS001 | registry_client.rs | 2197 |
| C | GS001 | mock.rs | 246 |
| C | GS001 | secret_service.rs | 64 |
| C | GS001 | secret_service.rs | 771 |
| C | GS001 | windows.rs | 751 |
| C | GS001 | abi_tag.rs | 504 |
| C | GS001 | abi_tag.rs | 505 |
| C | GS001 | abi_tag.rs | 508 |
| C | GS001 | abi_tag.rs | 509 |
| C | GS001 | abi_tag.rs | 523 |
| C | GS001 | abi_tag.rs | 526 |
| C | GS001 | tags.rs | 3012 |
| C | GS001 | tags.rs | 3013 |
| C | GS001 | tags.rs | 3017 |
| C | GS001 | tags.rs | 3018 |
| C | GS001 | tags.rs | 3039 |
| C | GS001 | tags.rs | 3040 |
| C | GS001 | ruff.toml | 6 |
| C | GS001 | ruff.toml | 8 |
| C | GS001 | ruff.toml | 8 |
| C | GS001 | discovery.rs | 3927 |
| C | GS001 | discovery.rs | 3941 |
| C | GS001 | backend.rs | 947 |
| C | GS001 | backend.rs | 948 |
| C | GS001 | backend.rs | 949 |
| C | GS001 | backend.rs | 950 |
| C | GS001 | backend.rs | 951 |
| C | GS001 | backend.rs | 952 |
| C | GS001 | backend.rs | 953 |
| C | GS001 | backend.rs | 954 |
| C | GS001 | backend.rs | 955 |
| C | GS001 | backend.rs | 956 |
| C | GS001 | backend.rs | 957 |
| C | GS001 | backend.rs | 958 |
| C | GS001 | backend.rs | 959 |
| C | GS001 | backend.rs | 960 |
| C | GS001 | backend.rs | 961 |
| C | GS001 | backend.rs | 962 |
| C | GS001 | backend.rs | 963 |
| C | GS001 | backend.rs | 964 |
| C | GS001 | backend.rs | 965 |
| C | GS001 | backend.rs | 966 |
| C | GS001 | backend.rs | 967 |
| C | GS001 | backend.rs | 968 |
| C | GS001 | backend.rs | 969 |
| C | GS001 | ruff.toml | 1 |
| C | GS001 | ruff.toml | 20 |
| C | GS001 | ruff.toml | 20 |
| C | GS001 | uv.schema.json | 2563 |
| C | GS001 | uv.schema.json | 2568 |
| C | GS001 | uv.schema.json | 2573 |
| C | GS001 | uv.schema.json | 2578 |
| C | GS001 | uv.schema.json | 2583 |
| C | GS001 | uv.schema.json | 2588 |
| C | GS001 | uv.schema.json | 2593 |
| C | GS001 | uv.schema.json | 2598 |
| C | GS001 | uv.schema.json | 2603 |
| C | GS001 | uv.schema.json | 2608 |
| C | GS001 | uv.schema.json | 2613 |
| C | GS001 | uv.schema.json | 2618 |
| C | GS001 | uv.schema.json | 2623 |
| C | GS001 | uv.schema.json | 2628 |
| C | GS001 | uv.schema.json | 2633 |
| C | GS001 | uv.schema.json | 2638 |
| C | GS001 | uv.schema.json | 2643 |
| C | GS001 | uv.schema.json | 2648 |
| C | GS001 | uv.schema.json | 2653 |
| C | GS001 | uv.schema.json | 2658 |
| C | GS001 | uv.schema.json | 2663 |
| C | GS001 | uv.schema.json | 2668 |
| C | GS001 | uv.schema.json | 2673 |
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
| L | GS003 | prune_cargo_workspace_cache.py | 109 |
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
| L | GS003 | settings.rs | 5261 |
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
| L | GS003 | wheel_metadata.rs | 57 |
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
| L | GS003 | lib.rs | 2200 |
| L | GS003 | lib.rs | 2201 |
| L | GS003 | lib.rs | 2206 |
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
| H | ? | lib.rs | 1333 |
| H | ? | pyproject_mut.rs | 2076 |
| H | ? | pyproject_mut.rs | 2080 |
| H | ? | pyproject_mut.rs | 2081 |
| H | ? | pyproject_mut.rs | 2100 |
| H | ? | pyproject_mut.rs | 2105 |
| H | ? | pyproject_mut.rs | 2106 |
| H | ? | pyproject_mut.rs | 2123 |
| H | ? | pyproject_mut.rs | 2126 |
| H | ? | pyproject_mut.rs | 2127 |
| H | ? | pyproject_mut.rs | 2132 |
| H | ? | pyproject_mut.rs | 2133 |
| H | ? | pyproject_mut.rs | 2150 |
| H | ? | pyproject_mut.rs | 2153 |
| H | ? | pyproject_mut.rs | 2154 |
| H | ? | pyproject_mut.rs | 2159 |
| H | ? | pyproject_mut.rs | 2160 |
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
| H | ? | tree.rs | 2782 |
| H | ? | tree.rs | 2799 |
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
| C | ? | registry_client.rs | 2091 |
| C | ? | registry_client.rs | 2147 |
| C | ? | registry_client.rs | 2197 |
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
| I | GS007 | get_interpreter_info.py | 21 |
| s | GS009 |  | 0 |
| L | GS014 | credentials.rs | 1 |
| L | GS014 | credentials.rs | 1 |
| H | GS017 | check-release-artifact-sboms.sh | 29 |
| H | GS017 | registries-test.py | 109 |
| s | GS021 |  | 80 |
| r | GS022 |  | 67 |
| r | GS022 |  | 76 |
| r | GS022 |  | 49 |
| r | GS022 |  | 212 |
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
| H | ? | candidate_selector.rs | 344 |
| H | ? | candidate_selector.rs | 902 |
| H | ? | candidate_selector.rs | 904 |
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
| H | ? | flat_index.rs | 138 |
| H | ? | flat_index.rs | 139 |
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
| H | ? | mod.rs | 444 |
| H | ? | mod.rs | 447 |
| H | ? | mod.rs | 476 |
| H | ? | mod.rs | 478 |
| H | ? | mod.rs | 583 |
| H | ? | mod.rs | 598 |
| H | ? | mod.rs | 603 |
| H | ? | mod.rs | 722 |
| H | ? | mod.rs | 740 |
| H | ? | mod.rs | 863 |
| H | ? | mod.rs | 868 |
| H | ? | mod.rs | 897 |
| H | ? | mod.rs | 926 |
| H | ? | mod.rs | 927 |
| H | ? | mod.rs | 949 |
| H | ? | mod.rs | 950 |
| H | ? | mod.rs | 1000 |
| H | ? | mod.rs | 1072 |
| H | ? | mod.rs | 1075 |
| H | ? | mod.rs | 1091 |
| H | ? | mod.rs | 1109 |
| H | ? | mod.rs | 1128 |
| H | ? | mod.rs | 1130 |
| H | ? | mod.rs | 1173 |
| H | ? | mod.rs | 1174 |
| H | ? | mod.rs | 1186 |
| H | ? | mod.rs | 1187 |
| H | ? | mod.rs | 1188 |
| H | ? | mod.rs | 1201 |
| H | ? | mod.rs | 1202 |
| H | ? | mod.rs | 1203 |
| H | ? | mod.rs | 1216 |
| H | ? | mod.rs | 1218 |
| H | ? | mod.rs | 1229 |
| H | ? | mod.rs | 1231 |
| H | ? | mod.rs | 1258 |
| H | ? | mod.rs | 1259 |
| H | ? | mod.rs | 1271 |
| H | ? | mod.rs | 2131 |
| H | ? | mod.rs | 2139 |
| H | ? | mod.rs | 2198 |
| H | ? | mod.rs | 2398 |
| H | ? | mod.rs | 2413 |
| H | ? | mod.rs | 2568 |
| H | ? | mod.rs | 2586 |
| H | ? | mod.rs | 2655 |
| H | ? | mod.rs | 2719 |
| H | ? | mod.rs | 2807 |
| H | ? | mod.rs | 2873 |
| H | ? | mod.rs | 2874 |
| H | ? | mod.rs | 3042 |
| H | ? | mod.rs | 3224 |
| H | ? | mod.rs | 3231 |
| H | ? | mod.rs | 3234 |
| H | ? | mod.rs | 3253 |
| H | ? | mod.rs | 3259 |
| H | ? | mod.rs | 3268 |
| H | ? | mod.rs | 3278 |
| H | ? | mod.rs | 3301 |
| H | ? | mod.rs | 3306 |
| H | ? | mod.rs | 3714 |
| H | ? | mod.rs | 3853 |
| H | ? | mod.rs | 3871 |
| H | ? | mod.rs | 3943 |
| H | ? | mod.rs | 3964 |
| H | ? | mod.rs | 3976 |
| H | ? | mod.rs | 3979 |
| H | ? | mod.rs | 3984 |
| H | ? | mod.rs | 3994 |
| H | ? | mod.rs | 4009 |
| H | ? | mod.rs | 4016 |
| H | ? | mod.rs | 4017 |
| H | ? | mod.rs | 4022 |
| H | ? | mod.rs | 4027 |
| H | ? | mod.rs | 4035 |
| H | ? | mod.rs | 4042 |
| H | ? | mod.rs | 4049 |
| H | ? | mod.rs | 4069 |
| H | ? | mod.rs | 4080 |
| H | ? | mod.rs | 4084 |
| H | ? | mod.rs | 4088 |
| H | ? | mod.rs | 4092 |
| H | ? | mod.rs | 4097 |
| H | ? | mod.rs | 4103 |
| H | ? | mod.rs | 4143 |
| H | ? | mod.rs | 4152 |
| H | ? | mod.rs | 4159 |
| H | ? | mod.rs | 4160 |
| H | ? | mod.rs | 4171 |
| H | ? | mod.rs | 4183 |
| H | ? | mod.rs | 4195 |
| H | ? | mod.rs | 4212 |
| H | ? | mod.rs | 4221 |
| H | ? | mod.rs | 4230 |
| H | ? | mod.rs | 4231 |
| H | ? | mod.rs | 4236 |
| H | ? | mod.rs | 4239 |
| H | ? | mod.rs | 4246 |
| H | ? | mod.rs | 4247 |
| H | ? | mod.rs | 4251 |
| H | ? | mod.rs | 4254 |
| H | ? | mod.rs | 4264 |
| H | ? | mod.rs | 4273 |
| H | ? | mod.rs | 4279 |
| H | ? | mod.rs | 4280 |
| H | ? | mod.rs | 4284 |
| H | ? | mod.rs | 4286 |
| H | ? | mod.rs | 4306 |
| H | ? | mod.rs | 4307 |
| H | ? | mod.rs | 4312 |
| H | ? | mod.rs | 4316 |
| H | ? | mod.rs | 4324 |
| H | ? | mod.rs | 4329 |
| H | ? | mod.rs | 4339 |
| H | ? | mod.rs | 4340 |
| H | ? | mod.rs | 4363 |
| H | ? | mod.rs | 4379 |
| H | ? | mod.rs | 4380 |
| H | ? | mod.rs | 4388 |
| H | ? | mod.rs | 4392 |
| H | ? | mod.rs | 4400 |
| H | ? | mod.rs | 4416 |
| H | ? | mod.rs | 4417 |
| H | ? | mod.rs | 4526 |
| H | ? | mod.rs | 4530 |
| H | ? | mod.rs | 4532 |
| H | ? | mod.rs | 4544 |
| H | ? | mod.rs | 4608 |
| H | ? | mod.rs | 4666 |
| H | ? | mod.rs | 4670 |
| H | ? | mod.rs | 4671 |
| H | ? | mod.rs | 4684 |
| H | ? | mod.rs | 4751 |
| H | ? | mod.rs | 4753 |
| H | ? | mod.rs | 4789 |
| H | ? | mod.rs | 4793 |
| H | ? | mod.rs | 4799 |
| H | ? | mod.rs | 4807 |
| H | ? | mod.rs | 4933 |
| H | ? | mod.rs | 5011 |
| H | ? | mod.rs | 5036 |
| H | ? | mod.rs | 5055 |
| H | ? | mod.rs | 5059 |
| H | ? | mod.rs | 5116 |
| H | ? | mod.rs | 5320 |
| H | ? | mod.rs | 5774 |
| H | ? | mod.rs | 5792 |
| H | ? | mod.rs | 5810 |
| H | ? | mod.rs | 5856 |
| H | ? | mod.rs | 6065 |
| H | ? | mod.rs | 6110 |
| H | ? | mod.rs | 6118 |
| H | ? | mod.rs | 6123 |
| H | ? | mod.rs | 6131 |
| H | ? | mod.rs | 6136 |
| H | ? | mod.rs | 6146 |
| H | ? | mod.rs | 6152 |
| H | ? | mod.rs | 6165 |
| H | ? | mod.rs | 6175 |
| H | ? | mod.rs | 6193 |
| H | ? | mod.rs | 6216 |
| H | ? | mod.rs | 6226 |
| H | ? | mod.rs | 6330 |
| H | ? | mod.rs | 6500 |
| H | ? | mod.rs | 6647 |
| H | ? | mod.rs | 6658 |
| H | ? | mod.rs | 6666 |
| H | ? | mod.rs | 6667 |
| H | ? | mod.rs | 6691 |
| H | ? | mod.rs | 6702 |
| H | ? | mod.rs | 6710 |
| H | ? | mod.rs | 6711 |
| H | ? | mod.rs | 6817 |
| H | ? | mod.rs | 6818 |
| H | ? | mod.rs | 6957 |
| H | ? | mod.rs | 6981 |
| H | ? | mod.rs | 6997 |
| H | ? | mod.rs | 7001 |
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
| H | ? | mod.rs | 89 |
| H | ? | mod.rs | 92 |
| H | ? | mod.rs | 97 |
| H | ? | mod.rs | 119 |
| H | ? | mod.rs | 140 |
| H | ? | mod.rs | 497 |
| H | ? | mod.rs | 501 |
| H | ? | mod.rs | 529 |
| H | ? | mod.rs | 551 |
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
| H | ? | pylock_toml.rs | 418 |
| H | ? | pylock_toml.rs | 449 |
| H | ? | pylock_toml.rs | 465 |
| H | ? | pylock_toml.rs | 470 |
| H | ? | pylock_toml.rs | 480 |
| H | ? | pylock_toml.rs | 487 |
| H | ? | pylock_toml.rs | 521 |
| H | ? | pylock_toml.rs | 531 |
| H | ? | pylock_toml.rs | 538 |
| H | ? | pylock_toml.rs | 542 |
| H | ? | pylock_toml.rs | 543 |
| H | ? | pylock_toml.rs | 553 |
| H | ? | pylock_toml.rs | 563 |
| H | ? | pylock_toml.rs | 569 |
| H | ? | pylock_toml.rs | 582 |
| H | ? | pylock_toml.rs | 589 |
| H | ? | pylock_toml.rs | 615 |
| H | ? | pylock_toml.rs | 625 |
| H | ? | pylock_toml.rs | 701 |
| H | ? | pylock_toml.rs | 717 |
| H | ? | pylock_toml.rs | 754 |
| H | ? | pylock_toml.rs | 801 |
| H | ? | pylock_toml.rs | 865 |
| H | ? | pylock_toml.rs | 871 |
| H | ? | pylock_toml.rs | 884 |
| H | ? | pylock_toml.rs | 906 |
| H | ? | pylock_toml.rs | 910 |
| H | ? | pylock_toml.rs | 921 |
| H | ? | pylock_toml.rs | 949 |
| H | ? | pylock_toml.rs | 971 |
| H | ? | pylock_toml.rs | 1103 |
| H | ? | pylock_toml.rs | 1105 |
| H | ? | pylock_toml.rs | 1113 |
| H | ? | pylock_toml.rs | 1114 |
| H | ? | pylock_toml.rs | 1115 |
| H | ? | pylock_toml.rs | 1130 |
| H | ? | pylock_toml.rs | 1134 |
| H | ? | pylock_toml.rs | 1137 |
| H | ? | pylock_toml.rs | 1142 |
| H | ? | pylock_toml.rs | 1146 |
| H | ? | pylock_toml.rs | 1149 |
| H | ? | pylock_toml.rs | 1153 |
| H | ? | pylock_toml.rs | 1157 |
| H | ? | pylock_toml.rs | 1162 |
| H | ? | pylock_toml.rs | 1165 |
| H | ? | pylock_toml.rs | 1183 |
| H | ? | pylock_toml.rs | 1203 |
| H | ? | pylock_toml.rs | 1252 |
| H | ? | pylock_toml.rs | 1266 |
| H | ? | pylock_toml.rs | 1269 |
| H | ? | pylock_toml.rs | 1272 |
| H | ? | pylock_toml.rs | 1274 |
| H | ? | pylock_toml.rs | 1277 |
| H | ? | pylock_toml.rs | 1283 |
| H | ? | pylock_toml.rs | 1430 |
| H | ? | pylock_toml.rs | 1435 |
| H | ? | pylock_toml.rs | 1451 |
| H | ? | pylock_toml.rs | 1458 |
| H | ? | pylock_toml.rs | 1463 |
| H | ? | pylock_toml.rs | 1485 |
| H | ? | pylock_toml.rs | 1489 |
| H | ? | pylock_toml.rs | 1498 |
| H | ? | pylock_toml.rs | 1506 |
| H | ? | pylock_toml.rs | 1540 |
| H | ? | pylock_toml.rs | 1556 |
| H | ? | pylock_toml.rs | 1561 |
| H | ? | pylock_toml.rs | 1568 |
| H | ? | pylock_toml.rs | 1575 |
| H | ? | pylock_toml.rs | 1586 |
| H | ? | pylock_toml.rs | 1587 |
| H | ? | pylock_toml.rs | 1591 |
| H | ? | pylock_toml.rs | 1593 |
| H | ? | pylock_toml.rs | 1607 |
| H | ? | pylock_toml.rs | 1613 |
| H | ? | pylock_toml.rs | 1617 |
| H | ? | pylock_toml.rs | 1648 |
| H | ? | pylock_toml.rs | 1652 |
| H | ? | pylock_toml.rs | 1661 |
| H | ? | pylock_toml.rs | 1669 |
| H | ? | pylock_toml.rs | 1679 |
| H | ? | pylock_toml.rs | 1703 |
| H | ? | pylock_toml.rs | 1726 |
| H | ? | pylock_toml.rs | 1737 |
| H | ? | pylock_toml.rs | 1745 |
| H | ? | pylock_toml.rs | 1746 |
| H | ? | pylock_toml.rs | 1752 |
| H | ? | pylock_toml.rs | 1753 |
| H | ? | pylock_toml.rs | 1754 |
| H | ? | pylock_toml.rs | 1756 |
| H | ? | pylock_toml.rs | 1762 |
| H | ? | pylock_toml.rs | 1774 |
| H | ? | pylock_toml.rs | 1782 |
| H | ? | pylock_toml.rs | 1787 |
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
| H | ? | installable.rs | 119 |
| H | ? | installable.rs | 123 |
| H | ? | installable.rs | 422 |
| H | ? | installable.rs | 468 |
| H | ? | installable.rs | 471 |
| H | ? | installable.rs | 530 |
| H | ? | installable.rs | 533 |
| H | ? | installable.rs | 569 |
| H | ? | installable.rs | 635 |
| H | ? | installable.rs | 718 |
| H | ? | installable.rs | 719 |
| H | ? | installable.rs | 720 |
| H | ? | installable.rs | 721 |
| H | ? | installable.rs | 790 |
| H | ? | installable.rs | 853 |
| H | ? | installable.rs | 854 |
| H | ? | installable.rs | 911 |
| H | ? | installable.rs | 917 |
| H | ? | installable.rs | 975 |
| H | ? | installable.rs | 982 |
| H | ? | installable.rs | 1431 |
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
| H | ? | report.rs | 1372 |
| H | ? | report.rs | 1373 |
| H | ? | report.rs | 1388 |
| H | ? | report.rs | 1389 |
| H | ? | report.rs | 1395 |
| H | ? | report.rs | 1396 |
| H | ? | report.rs | 1794 |
| H | ? | report.rs | 1801 |
| H | ? | report.rs | 1802 |
| H | ? | report.rs | 1854 |
| H | ? | report.rs | 1864 |
| H | ? | report.rs | 1866 |
| H | ? | report.rs | 1971 |
| H | ? | report.rs | 1992 |
| H | ? | report.rs | 2011 |
| H | ? | report.rs | 2081 |
| H | ? | report.rs | 2474 |
| H | ? | report.rs | 2486 |
| H | ? | report.rs | 2487 |
| H | ? | report.rs | 2520 |
| H | ? | report.rs | 2522 |
| H | ? | report.rs | 2525 |
| H | ? | report.rs | 2526 |
| H | ? | report.rs | 2535 |
| H | ? | report.rs | 2541 |
| H | ? | report.rs | 2785 |
| H | ? | report.rs | 2787 |
| H | ? | report.rs | 2789 |
| H | ? | report.rs | 2790 |
| H | ? | report.rs | 2793 |
| H | ? | report.rs | 2794 |
| H | ? | report.rs | 2795 |
| H | ? | report.rs | 2796 |
| H | ? | report.rs | 2817 |
| H | ? | report.rs | 2819 |
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
| H | ? | version_map.rs | 94 |
| H | ? | version_map.rs | 674 |
| H | ? | version_map.rs | 689 |
| H | ? | version_map.rs | 703 |
| H | ? | version_map.rs | 704 |
| H | ? | version_map.rs | 707 |
| H | ? | version_map.rs | 752 |
| H | ? | version_map.rs | 806 |
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
| H | ? | prerelease.rs | 208 |
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
| H | ? | mod.rs | 188 |
| H | ? | mod.rs | 234 |
| H | ? | mod.rs | 235 |
| H | ? | mod.rs | 236 |
| H | ? | mod.rs | 249 |
| H | ? | mod.rs | 250 |
| H | ? | mod.rs | 252 |
| H | ? | mod.rs | 254 |
| H | ? | mod.rs | 270 |
| H | ? | mod.rs | 290 |
| H | ? | mod.rs | 293 |
| H | ? | mod.rs | 335 |
| H | ? | mod.rs | 336 |
| H | ? | mod.rs | 338 |
| H | ? | mod.rs | 339 |
| H | ? | mod.rs | 340 |
| H | ? | mod.rs | 344 |
| H | ? | mod.rs | 345 |
| H | ? | mod.rs | 348 |
| H | ? | mod.rs | 377 |
| H | ? | mod.rs | 454 |
| H | ? | mod.rs | 455 |
| H | ? | mod.rs | 457 |
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
| H | ? | mod.rs | 878 |
| H | ? | mod.rs | 881 |
| H | ? | mod.rs | 938 |
| H | ? | mod.rs | 999 |
| H | ? | mod.rs | 1003 |
| H | ? | mod.rs | 1012 |
| H | ? | mod.rs | 1014 |
| H | ? | mod.rs | 1018 |
| H | ? | mod.rs | 1019 |
| H | ? | mod.rs | 1067 |
| H | ? | mod.rs | 1069 |
| H | ? | mod.rs | 1070 |
| H | ? | mod.rs | 1071 |
| H | ? | mod.rs | 1105 |
| H | ? | mod.rs | 1119 |
| H | ? | mod.rs | 1124 |
| H | ? | mod.rs | 1154 |
| H | ? | mod.rs | 1169 |
| H | ? | mod.rs | 1215 |
| H | ? | mod.rs | 1229 |
| H | ? | mod.rs | 1237 |
| H | ? | mod.rs | 1239 |
| H | ? | mod.rs | 1276 |
| H | ? | mod.rs | 1289 |
| H | ? | mod.rs | 1306 |
| H | ? | mod.rs | 1308 |
| H | ? | mod.rs | 1314 |
| H | ? | mod.rs | 1338 |
| H | ? | mod.rs | 1346 |
| H | ? | mod.rs | 1353 |
| H | ? | mod.rs | 1359 |
| H | ? | mod.rs | 1365 |
| H | ? | mod.rs | 1396 |
| H | ? | mod.rs | 1399 |
| H | ? | mod.rs | 1442 |
| H | ? | mod.rs | 1485 |
| H | ? | mod.rs | 1540 |
| H | ? | mod.rs | 1587 |
| H | ? | mod.rs | 1588 |
| H | ? | mod.rs | 1655 |
| H | ? | mod.rs | 1711 |
| H | ? | mod.rs | 1713 |
| H | ? | mod.rs | 1716 |
| H | ? | mod.rs | 1718 |
| H | ? | mod.rs | 1746 |
| H | ? | mod.rs | 1747 |
| H | ? | mod.rs | 1755 |
| H | ? | mod.rs | 1779 |
| H | ? | mod.rs | 1788 |
| H | ? | mod.rs | 1889 |
| H | ? | mod.rs | 1909 |
| H | ? | mod.rs | 1932 |
| H | ? | mod.rs | 1935 |
| H | ? | mod.rs | 1943 |
| H | ? | mod.rs | 1945 |
| H | ? | mod.rs | 1954 |
| H | ? | mod.rs | 2011 |
| H | ? | mod.rs | 2016 |
| H | ? | mod.rs | 2039 |
| H | ? | mod.rs | 2044 |
| H | ? | mod.rs | 2065 |
| H | ? | mod.rs | 2067 |
| H | ? | mod.rs | 2070 |
| H | ? | mod.rs | 2150 |
| H | ? | mod.rs | 2171 |
| H | ? | mod.rs | 2172 |
| H | ? | mod.rs | 2173 |
| H | ? | mod.rs | 2174 |
| H | ? | mod.rs | 2175 |
| H | ? | mod.rs | 2203 |
| H | ? | mod.rs | 2205 |
| H | ? | mod.rs | 2206 |
| H | ? | mod.rs | 2207 |
| H | ? | mod.rs | 2282 |
| H | ? | mod.rs | 2380 |
| H | ? | mod.rs | 2381 |
| H | ? | mod.rs | 2382 |
| H | ? | mod.rs | 2383 |
| H | ? | mod.rs | 2384 |
| H | ? | mod.rs | 2417 |
| H | ? | mod.rs | 2418 |
| H | ? | mod.rs | 2419 |
| H | ? | mod.rs | 2420 |
| H | ? | mod.rs | 2421 |
| H | ? | mod.rs | 2566 |
| H | ? | mod.rs | 2595 |
| H | ? | mod.rs | 2596 |
| H | ? | mod.rs | 2611 |
| H | ? | mod.rs | 2612 |
| H | ? | mod.rs | 2636 |
| H | ? | mod.rs | 2643 |
| H | ? | mod.rs | 2650 |
| H | ? | mod.rs | 2695 |
| H | ? | mod.rs | 2701 |
| H | ? | mod.rs | 2705 |
| H | ? | mod.rs | 2754 |
| H | ? | mod.rs | 2766 |
| H | ? | mod.rs | 2775 |
| H | ? | mod.rs | 2808 |
| H | ? | mod.rs | 2821 |
| H | ? | mod.rs | 2823 |
| H | ? | mod.rs | 2849 |
| H | ? | mod.rs | 2858 |
| H | ? | mod.rs | 2861 |
| H | ? | mod.rs | 2886 |
| H | ? | mod.rs | 2909 |
| H | ? | mod.rs | 2916 |
| H | ? | mod.rs | 2929 |
| H | ? | mod.rs | 2933 |
| H | ? | mod.rs | 2934 |
| H | ? | mod.rs | 2935 |
| H | ? | mod.rs | 2936 |
| H | ? | mod.rs | 2943 |
| H | ? | mod.rs | 2944 |
| H | ? | mod.rs | 2945 |
| H | ? | mod.rs | 3217 |
| H | ? | mod.rs | 3218 |
| H | ? | mod.rs | 3222 |
| H | ? | mod.rs | 3228 |
| H | ? | mod.rs | 3248 |
| H | ? | mod.rs | 3395 |
| H | ? | mod.rs | 3409 |
| H | ? | mod.rs | 3535 |
| H | ? | mod.rs | 3540 |
| H | ? | mod.rs | 3541 |
| H | ? | mod.rs | 3544 |
| H | ? | mod.rs | 3545 |
| H | ? | mod.rs | 3567 |
| H | ? | mod.rs | 3572 |
| H | ? | mod.rs | 3573 |
| H | ? | mod.rs | 3599 |
| H | ? | mod.rs | 3604 |
| H | ? | mod.rs | 3605 |
| H | ? | mod.rs | 3608 |
| H | ? | mod.rs | 3617 |
| H | ? | mod.rs | 3622 |
| H | ? | mod.rs | 3623 |
| H | ? | mod.rs | 3649 |
| H | ? | mod.rs | 3654 |
| H | ? | mod.rs | 3655 |
| H | ? | mod.rs | 3659 |
| H | ? | mod.rs | 3683 |
| H | ? | mod.rs | 3684 |
| H | ? | mod.rs | 3685 |
| H | ? | mod.rs | 3752 |
| H | ? | mod.rs | 3872 |
| H | ? | mod.rs | 3914 |
| H | ? | mod.rs | 3943 |
| H | ? | mod.rs | 3962 |
| H | ? | mod.rs | 3983 |
| H | ? | mod.rs | 3989 |
| H | ? | mod.rs | 4000 |
| H | ? | mod.rs | 4007 |
| H | ? | mod.rs | 4047 |
| H | ? | mod.rs | 4104 |
| H | ? | mod.rs | 4116 |
| H | ? | mod.rs | 4325 |
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
| H | ? | flat_index.rs | 175 |
| H | ? | flat_index.rs | 178 |
| H | ? | flat_index.rs | 212 |
| H | ? | flat_index.rs | 217 |
| H | ? | flat_index.rs | 223 |
| H | ? | flat_index.rs | 226 |
| H | ? | flat_index.rs | 229 |
| H | ? | flat_index.rs | 269 |
| H | ? | flat_index.rs | 306 |
| H | ? | flat_index.rs | 378 |
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
| H | ? | registry_client.rs | 1097 |
| H | ? | registry_client.rs | 1129 |
| H | ? | registry_client.rs | 1136 |
| H | ? | registry_client.rs | 1144 |
| H | ? | registry_client.rs | 1147 |
| H | ? | registry_client.rs | 1208 |
| H | ? | registry_client.rs | 1215 |
| H | ? | registry_client.rs | 1221 |
| H | ? | registry_client.rs | 1240 |
| H | ? | registry_client.rs | 1242 |
| H | ? | registry_client.rs | 1243 |
| H | ? | registry_client.rs | 1246 |
| H | ? | registry_client.rs | 1251 |
| H | ? | registry_client.rs | 1266 |
| H | ? | registry_client.rs | 1282 |
| H | ? | registry_client.rs | 1294 |
| H | ? | registry_client.rs | 1304 |
| H | ? | registry_client.rs | 1376 |
| H | ? | registry_client.rs | 1575 |
| H | ? | registry_client.rs | 1646 |
| H | ? | registry_client.rs | 1711 |
| H | ? | registry_client.rs | 1779 |
| H | ? | registry_client.rs | 1797 |
| H | ? | registry_client.rs | 1798 |
| H | ? | registry_client.rs | 1827 |
| H | ? | registry_client.rs | 2126 |
| H | ? | registry_client.rs | 2176 |
| H | ? | registry_client.rs | 2226 |
| H | ? | base_client.rs | 456 |
| H | ? | base_client.rs | 464 |
| H | ? | base_client.rs | 469 |
| H | ? | base_client.rs | 476 |
| H | ? | base_client.rs | 485 |
| H | ? | base_client.rs | 487 |
| H | ? | base_client.rs | 495 |
| H | ? | base_client.rs | 500 |
| H | ? | base_client.rs | 507 |
| H | ? | base_client.rs | 512 |
| H | ? | base_client.rs | 513 |
| H | ? | base_client.rs | 516 |
| H | ? | base_client.rs | 518 |
| H | ? | base_client.rs | 531 |
| H | ? | base_client.rs | 553 |
| H | ? | base_client.rs | 625 |
| H | ? | base_client.rs | 636 |
| H | ? | base_client.rs | 653 |
| H | ? | base_client.rs | 668 |
| H | ? | base_client.rs | 690 |
| H | ? | base_client.rs | 698 |
| H | ? | base_client.rs | 700 |
| H | ? | base_client.rs | 710 |
| H | ? | base_client.rs | 712 |
| H | ? | base_client.rs | 803 |
| H | ? | base_client.rs | 953 |
| H | ? | base_client.rs | 1088 |
| H | ? | base_client.rs | 1194 |
| H | ? | base_client.rs | 1200 |
| H | ? | retry.rs | 149 |
| H | ? | middleware.rs | 46 |
| H | ? | tls.rs | 110 |
| H | ? | tls.rs | 295 |
| H | ? | tls.rs | 387 |
| H | ? | tls.rs | 417 |
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
| H | ? | compile.rs | 517 |
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
| H | ? | source_dist.rs | 36 |
| H | ? | source_dist.rs | 37 |
| H | ? | source_dist.rs | 51 |
| H | ? | source_dist.rs | 64 |
| H | ? | source_dist.rs | 65 |
| H | ? | source_dist.rs | 211 |
| H | ? | source_dist.rs | 212 |
| H | ? | source_dist.rs | 246 |
| H | ? | source_dist.rs | 458 |
| H | ? | source_dist.rs | 493 |
| H | ? | source_dist.rs | 507 |
| H | ? | source_dist.rs | 514 |
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
| H | ? | package_options.rs | 181 |
| H | ? | package_options.rs | 188 |
| H | ? | package_options.rs | 202 |
| H | ? | package_options.rs | 301 |
| H | ? | constraints.rs | 27 |
| H | ? | constraints.rs | 78 |
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
| H | ? | lib.rs | 557 |
| H | ? | lib.rs | 620 |
| H | ? | lib.rs | 673 |
| H | ? | lib.rs | 795 |
| H | ? | lib.rs | 799 |
| H | ? | lib.rs | 810 |
| H | ? | lib.rs | 836 |
| H | ? | lib.rs | 1212 |
| H | ? | lib.rs | 1215 |
| H | ? | lib.rs | 1251 |
| H | ? | lib.rs | 1353 |
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
| H | ? | pyproject_mut.rs | 553 |
| H | ? | pyproject_mut.rs | 556 |
| H | ? | pyproject_mut.rs | 572 |
| H | ? | pyproject_mut.rs | 575 |
| H | ? | pyproject_mut.rs | 594 |
| H | ? | pyproject_mut.rs | 597 |
| H | ? | pyproject_mut.rs | 1410 |
| H | ? | pyproject_mut.rs | 1556 |
| H | ? | pyproject_mut.rs | 1582 |
| H | ? | pyproject_mut.rs | 1596 |
| H | ? | pyproject_mut.rs | 1602 |
| H | ? | pyproject_mut.rs | 1689 |
| H | ? | pyproject_mut.rs | 1716 |
| H | ? | pyproject.rs | 1698 |
| H | ? | pyproject.rs | 1699 |
| H | ? | pyproject.rs | 1705 |
| H | ? | pyproject.rs | 1706 |
| H | ? | pyproject.rs | 1707 |
| H | ? | pyproject.rs | 1834 |
| H | ? | pyproject.rs | 1847 |
| H | ? | pyproject.rs | 1873 |
| H | ? | pyproject.rs | 1886 |
| H | ? | parsed_url.rs | 350 |
| H | ? | parsed_url.rs | 504 |
| H | ? | parsed_url.rs | 559 |
| H | ? | parsed_url.rs | 574 |
| H | ? | parsed_url.rs | 591 |
| H | ? | parsed_url.rs | 674 |
| H | ? | parsed_url.rs | 679 |
| H | ? | parsed_url.rs | 683 |
| H | ? | parsed_url.rs | 689 |
| H | ? | parsed_url.rs | 696 |
| H | ? | parsed_url.rs | 703 |
| H | ? | parsed_url.rs | 716 |
| H | ? | parsed_url.rs | 728 |
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
| H | ? | lib.rs | 266 |
| H | ? | lib.rs | 307 |
| H | ? | lib.rs | 315 |
| H | ? | lib.rs | 326 |
| H | ? | lib.rs | 1128 |
| H | ? | lib.rs | 1131 |
| H | ? | lib.rs | 1134 |
| H | ? | lib.rs | 1137 |
| H | ? | lib.rs | 1629 |
| H | ? | lib.rs | 6230 |
| H | ? | lib.rs | 6231 |
| H | ? | lib.rs | 6232 |
| H | ? | lib.rs | 6293 |
| H | ? | lib.rs | 6294 |
| H | ? | lib.rs | 6295 |
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
| H | ? | prioritized_distribution.rs | 540 |
| H | ? | prioritized_distribution.rs | 543 |
| H | ? | prioritized_distribution.rs | 559 |
| H | ? | prioritized_distribution.rs | 568 |
| H | ? | index_url.rs | 27 |
| H | ? | index_url.rs | 66 |
| H | ? | index_url.rs | 114 |
| H | ? | index_url.rs | 304 |
| H | ? | index_url.rs | 526 |
| H | ? | index_url.rs | 529 |
| H | ? | index_url.rs | 774 |
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
| H | ? | lib.rs | 469 |
| H | ? | lib.rs | 569 |
| H | ? | lib.rs | 818 |
| H | ? | lib.rs | 829 |
| H | ? | lib.rs | 840 |
| H | ? | lib.rs | 851 |
| H | ? | lib.rs | 852 |
| H | ? | lib.rs | 862 |
| H | ? | lib.rs | 863 |
| H | ? | lib.rs | 872 |
| H | ? | lib.rs | 873 |
| H | ? | lib.rs | 883 |
| H | ? | lib.rs | 884 |
| H | ? | lib.rs | 894 |
| H | ? | lib.rs | 1041 |
| H | ? | lib.rs | 1074 |
| H | ? | lib.rs | 1075 |
| H | ? | lib.rs | 1437 |
| H | ? | lib.rs | 1441 |
| H | ? | lib.rs | 1790 |
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
| H | ? | sync.rs | 326 |
| H | ? | sync.rs | 327 |
| H | ? | sync.rs | 329 |
| H | ? | sync.rs | 372 |
| H | ? | sync.rs | 380 |
| H | ? | sync.rs | 392 |
| H | ? | sync.rs | 402 |
| H | ? | sync.rs | 403 |
| H | ? | sync.rs | 405 |
| H | ? | sync.rs | 406 |
| H | ? | sync.rs | 427 |
| H | ? | sync.rs | 452 |
| H | ? | sync.rs | 455 |
| H | ? | sync.rs | 470 |
| H | ? | sync.rs | 475 |
| H | ? | sync.rs | 513 |
| H | ? | sync.rs | 523 |
| H | ? | sync.rs | 527 |
| H | ? | compile.rs | 199 |
| H | ? | compile.rs | 364 |
| H | ? | compile.rs | 463 |
| H | ? | compile.rs | 464 |
| H | ? | compile.rs | 466 |
| H | ? | compile.rs | 509 |
| H | ? | compile.rs | 513 |
| H | ? | compile.rs | 523 |
| H | ? | compile.rs | 528 |
| H | ? | compile.rs | 550 |
| H | ? | compile.rs | 554 |
| H | ? | compile.rs | 563 |
| H | ? | compile.rs | 566 |
| H | ? | compile.rs | 588 |
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
| H | ? | install.rs | 247 |
| H | ? | install.rs | 454 |
| H | ? | install.rs | 455 |
| H | ? | install.rs | 457 |
| H | ? | install.rs | 500 |
| H | ? | install.rs | 515 |
| H | ? | install.rs | 525 |
| H | ? | install.rs | 526 |
| H | ? | install.rs | 528 |
| H | ? | install.rs | 529 |
| H | ? | install.rs | 547 |
| H | ? | install.rs | 572 |
| H | ? | install.rs | 575 |
| H | ? | install.rs | 591 |
| H | ? | install.rs | 596 |
| H | ? | install.rs | 646 |
| H | ? | install.rs | 656 |
| H | ? | install.rs | 660 |
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
| H | ? | build_frontend.rs | 775 |
| H | ? | build_frontend.rs | 1170 |
| H | ? | build_frontend.rs | 1171 |
| H | ? | build_frontend.rs | 1176 |
| H | ? | build_frontend.rs | 1177 |
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
| H | ? | publish.rs | 226 |
| H | ? | publish.rs | 276 |
| H | ? | publish.rs | 278 |
| H | ? | publish.rs | 348 |
| H | ? | publish.rs | 382 |
| H | ? | publish.rs | 646 |
| H | ? | publish.rs | 653 |
| H | ? | publish.rs | 661 |
| H | ? | publish.rs | 670 |
| H | ? | publish.rs | 682 |
| H | ? | publish.rs | 695 |
| H | ? | publish.rs | 707 |
| H | ? | common.rs | 138 |
| H | ? | common.rs | 221 |
| H | ? | common.rs | 264 |
| H | ? | common.rs | 342 |
| H | ? | common.rs | 436 |
| H | ? | common.rs | 437 |
| H | ? | common.rs | 439 |
| H | ? | common.rs | 449 |
| H | ? | common.rs | 453 |
| H | ? | common.rs | 460 |
| H | ? | common.rs | 462 |
| H | ? | common.rs | 464 |
| H | ? | common.rs | 478 |
| H | ? | common.rs | 490 |
| H | ? | common.rs | 500 |
| H | ? | common.rs | 501 |
| H | ? | common.rs | 503 |
| H | ? | common.rs | 504 |
| H | ? | common.rs | 510 |
| H | ? | common.rs | 674 |
| H | ? | common.rs | 675 |
| H | ? | common.rs | 792 |
| H | ? | common.rs | 807 |
| H | ? | common.rs | 816 |
| H | ? | common.rs | 820 |
| H | ? | common.rs | 826 |
| H | ? | common.rs | 913 |
| H | ? | common.rs | 940 |
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
| H | ? | audit.rs | 198 |
| H | ? | audit.rs | 206 |
| H | ? | audit.rs | 207 |
| H | ? | audit.rs | 211 |
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
| H | ? | install.rs | 540 |
| H | ? | install.rs | 637 |
| H | ? | install.rs | 640 |
| H | ? | install.rs | 645 |
| H | ? | install.rs | 651 |
| H | ? | install.rs | 653 |
| H | ? | install.rs | 658 |
| H | ? | install.rs | 716 |
| H | ? | install.rs | 827 |
| H | ? | install.rs | 1014 |
| H | ? | install.rs | 1029 |
| H | ? | install.rs | 1032 |
| H | ? | install.rs | 1034 |
| H | ? | install.rs | 1081 |
| H | ? | install.rs | 1154 |
| H | ? | install.rs | 1168 |
| H | ? | install.rs | 1176 |
| H | ? | install.rs | 1190 |
| H | ? | install.rs | 1193 |
| H | ? | install.rs | 1195 |
| H | ? | install.rs | 1200 |
| H | ? | install.rs | 1211 |
| H | ? | install.rs | 1219 |
| H | ? | uninstall.rs | 108 |
| H | ? | uninstall.rs | 196 |
| H | ? | uninstall.rs | 214 |
| H | ? | uninstall.rs | 216 |
| H | ? | module_owners.rs | 70 |
| H | ? | module_owners.rs | 128 |
| H | ? | module_owners.rs | 148 |
| H | ? | help.rs | 52 |
| H | ? | pylock.rs | 35 |
| H | ? | lock_target.rs | 53 |
| H | ? | lock_target.rs | 160 |
| H | ? | lock_target.rs | 162 |
| H | ? | lock_target.rs | 169 |
| H | ? | lock_target.rs | 306 |
| H | ? | lock_target.rs | 398 |
| H | ? | lock_target.rs | 450 |
| H | ? | lock_target.rs | 468 |
| H | ? | mod.rs | 658 |
| H | ? | mod.rs | 659 |
| H | ? | mod.rs | 667 |
| H | ? | mod.rs | 668 |
| H | ? | mod.rs | 675 |
| H | ? | mod.rs | 676 |
| H | ? | mod.rs | 696 |
| H | ? | mod.rs | 697 |
| H | ? | mod.rs | 703 |
| H | ? | mod.rs | 704 |
| H | ? | mod.rs | 709 |
| H | ? | mod.rs | 710 |
| H | ? | mod.rs | 1009 |
| H | ? | mod.rs | 1022 |
| H | ? | mod.rs | 1029 |
| H | ? | mod.rs | 1233 |
| H | ? | mod.rs | 1250 |
| H | ? | mod.rs | 1645 |
| H | ? | mod.rs | 1698 |
| H | ? | mod.rs | 1741 |
| H | ? | mod.rs | 1747 |
| H | ? | mod.rs | 2315 |
| H | ? | mod.rs | 2331 |
| H | ? | mod.rs | 2340 |
| H | ? | mod.rs | 2341 |
| H | ? | mod.rs | 2343 |
| H | ? | mod.rs | 2354 |
| H | ? | mod.rs | 2358 |
| H | ? | mod.rs | 2372 |
| H | ? | mod.rs | 2384 |
| H | ? | mod.rs | 2394 |
| H | ? | mod.rs | 2395 |
| H | ? | mod.rs | 2397 |
| H | ? | mod.rs | 2398 |
| H | ? | mod.rs | 2410 |
| H | ? | mod.rs | 2521 |
| H | ? | mod.rs | 2566 |
| H | ? | mod.rs | 2573 |
| H | ? | mod.rs | 2574 |
| H | ? | mod.rs | 2576 |
| H | ? | mod.rs | 2586 |
| H | ? | mod.rs | 2590 |
| H | ? | mod.rs | 2597 |
| H | ? | mod.rs | 2599 |
| H | ? | mod.rs | 2601 |
| H | ? | mod.rs | 2620 |
| H | ? | mod.rs | 2652 |
| H | ? | mod.rs | 2664 |
| H | ? | mod.rs | 2674 |
| H | ? | mod.rs | 2675 |
| H | ? | mod.rs | 2677 |
| H | ? | mod.rs | 2678 |
| H | ? | mod.rs | 2752 |
| H | ? | mod.rs | 2761 |
| H | ? | mod.rs | 2762 |
| H | ? | mod.rs | 2794 |
| H | ? | mod.rs | 2806 |
| H | ? | mod.rs | 2816 |
| H | ? | mod.rs | 2820 |
| H | ? | mod.rs | 2924 |
| H | ? | mod.rs | 3009 |
| H | ? | mod.rs | 3016 |
| H | ? | mod.rs | 3017 |
| H | ? | mod.rs | 3019 |
| H | ? | mod.rs | 3035 |
| H | ? | mod.rs | 3037 |
| H | ? | mod.rs | 3039 |
| H | ? | mod.rs | 3071 |
| H | ? | mod.rs | 3081 |
| H | ? | mod.rs | 3082 |
| H | ? | mod.rs | 3084 |
| H | ? | mod.rs | 3085 |
| H | ? | mod.rs | 3102 |
| H | ? | mod.rs | 3107 |
| H | ? | mod.rs | 3228 |
| H | ? | mod.rs | 3232 |
| H | ? | mod.rs | 3234 |
| H | ? | mod.rs | 3267 |
| H | ? | mod.rs | 3272 |
| H | ? | mod.rs | 3274 |
| H | ? | mod.rs | 3469 |
| H | ? | version.rs | 275 |
| H | ? | version.rs | 419 |
| H | ? | ty.rs | 61 |
| H | ? | install_target.rs | 463 |
| H | ? | install_target.rs | 464 |
| H | ? | install_target.rs | 467 |
| H | ? | install_target.rs | 469 |
| H | ? | install_target.rs | 480 |
| H | ? | install_target.rs | 575 |
| H | ? | install_target.rs | 577 |
| H | ? | install_target.rs | 584 |
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
| H | ? | check.rs | 93 |
| H | ? | check.rs | 197 |
| H | ? | check.rs | 218 |
| H | ? | check.rs | 229 |
| H | ? | check.rs | 267 |
| H | ? | tree.rs | 246 |
| H | ? | tree.rs | 247 |
| H | ? | tree.rs | 249 |
| H | ? | tree.rs | 252 |
| H | ? | tree.rs | 292 |
| H | ? | lock.rs | 392 |
| H | ? | lock.rs | 394 |
| H | ? | lock.rs | 772 |
| H | ? | lock.rs | 782 |
| H | ? | lock.rs | 785 |
| H | ? | lock.rs | 790 |
| H | ? | lock.rs | 797 |
| H | ? | lock.rs | 798 |
| H | ? | lock.rs | 809 |
| H | ? | lock.rs | 813 |
| H | ? | lock.rs | 830 |
| H | ? | lock.rs | 832 |
| H | ? | lock.rs | 834 |
| H | ? | lock.rs | 835 |
| H | ? | lock.rs | 858 |
| H | ? | lock.rs | 904 |
| H | ? | lock.rs | 905 |
| H | ? | lock.rs | 907 |
| H | ? | lock.rs | 908 |
| H | ? | lock.rs | 915 |
| H | ? | lock.rs | 1060 |
| H | ? | lock.rs | 1061 |
| H | ? | lock.rs | 1077 |
| H | ? | lock.rs | 1100 |
| H | ? | lock.rs | 1111 |
| H | ? | lock.rs | 1690 |
| H | ? | upgrade.rs | 149 |
| H | ? | upgrade.rs | 150 |
| H | ? | upgrade.rs | 151 |
| H | ? | upgrade.rs | 279 |
| H | ? | upgrade.rs | 280 |
| H | ? | upgrade.rs | 281 |
| H | ? | upgrade.rs | 289 |
| H | ? | upgrade.rs | 290 |
| H | ? | upgrade.rs | 291 |
| H | ? | upgrade.rs | 293 |
| H | ? | upgrade.rs | 297 |
| H | ? | upgrade.rs | 351 |
| H | ? | upgrade.rs | 444 |
| H | ? | upgrade.rs | 468 |
| H | ? | upgrade.rs | 469 |
| H | ? | upgrade.rs | 473 |
| H | ? | upgrade.rs | 474 |
| H | ? | upgrade.rs | 475 |
| H | ? | upgrade.rs | 479 |
| H | ? | upgrade.rs | 483 |
| H | ? | upgrade.rs | 484 |
| H | ? | upgrade.rs | 636 |
| H | ? | upgrade.rs | 640 |
| H | ? | upgrade.rs | 642 |
| H | ? | upgrade.rs | 655 |
| H | ? | upgrade.rs | 657 |
| H | ? | upgrade.rs | 664 |
| H | ? | upgrade.rs | 667 |
| H | ? | upgrade.rs | 669 |
| H | ? | upgrade.rs | 695 |
| H | ? | upgrade.rs | 781 |
| H | ? | upgrade.rs | 987 |
| H | ? | upgrade.rs | 988 |
| H | ? | upgrade.rs | 1024 |
| H | ? | upgrade.rs | 1031 |
| H | ? | upgrade.rs | 1039 |
| H | ? | upgrade.rs | 1056 |
| H | ? | upgrade.rs | 1092 |
| H | ? | upgrade.rs | 1094 |
| H | ? | toolchain.rs | 48 |
| H | ? | toolchain.rs | 50 |
| H | ? | run.rs | 288 |
| H | ? | run.rs | 412 |
| H | ? | run.rs | 549 |
| H | ? | run.rs | 1052 |
| H | ? | run.rs | 1350 |
| H | ? | run.rs | 1447 |
| H | ? | run.rs | 1537 |
| H | ? | run.rs | 1542 |
| H | ? | run.rs | 1547 |
| H | ? | run.rs | 1578 |
| H | ? | run.rs | 1589 |
| H | ? | run.rs | 1603 |
| H | ? | run.rs | 1616 |
| H | ? | run.rs | 1770 |
| H | ? | run.rs | 1774 |
| H | ? | run.rs | 1801 |
| H | ? | run.rs | 1805 |
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
| H | ? | export.rs | 114 |
| H | ? | export.rs | 126 |
| H | ? | init.rs | 463 |
| H | ? | init.rs | 478 |
| H | ? | init.rs | 545 |
| H | ? | sarif.rs | 54 |
| H | ? | sarif.rs | 55 |
| H | ? | sarif.rs | 65 |
| H | ? | sarif.rs | 66 |
| H | ? | sarif.rs | 195 |
| H | ? | sarif.rs | 334 |
| H | ? | sarif.rs | 347 |
| H | ? | sarif.rs | 379 |
| H | ? | sarif.rs | 382 |
| H | ? | json.rs | 164 |
| H | ? | json.rs | 165 |
| H | ? | json.rs | 199 |
| H | ? | audit.rs | 304 |
| H | ? | audit.rs | 306 |
| H | ? | audit.rs | 307 |
| H | ? | audit.rs | 308 |
| H | ? | audit.rs | 313 |
| H | ? | audit.rs | 319 |
| H | ? | audit.rs | 343 |
| H | ? | audit.rs | 350 |
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
| H | ? | settings.rs | 109 |
| H | ? | settings.rs | 380 |
| H | ? | settings.rs | 386 |
| H | ? | settings.rs | 391 |
| H | ? | settings.rs | 392 |
| H | ? | settings.rs | 393 |
| H | ? | settings.rs | 447 |
| H | ? | settings.rs | 504 |
| H | ? | settings.rs | 748 |
| H | ? | settings.rs | 749 |
| H | ? | settings.rs | 799 |
| H | ? | settings.rs | 944 |
| H | ? | settings.rs | 949 |
| H | ? | settings.rs | 952 |
| H | ? | settings.rs | 1069 |
| H | ? | settings.rs | 1074 |
| H | ? | settings.rs | 1077 |
| H | ? | settings.rs | 1204 |
| H | ? | settings.rs | 1221 |
| H | ? | settings.rs | 1324 |
| H | ? | settings.rs | 1439 |
| H | ? | settings.rs | 1440 |
| H | ? | settings.rs | 1441 |
| H | ? | settings.rs | 1450 |
| H | ? | settings.rs | 1456 |
| H | ? | settings.rs | 1462 |
| H | ? | settings.rs | 1529 |
| H | ? | settings.rs | 1620 |
| H | ? | settings.rs | 1734 |
| H | ? | settings.rs | 1790 |
| H | ? | settings.rs | 1890 |
| H | ? | settings.rs | 1891 |
| H | ? | settings.rs | 1989 |
| H | ? | settings.rs | 2063 |
| H | ? | settings.rs | 2064 |
| H | ? | settings.rs | 2112 |
| H | ? | settings.rs | 2113 |
| H | ? | settings.rs | 2122 |
| H | ? | settings.rs | 2174 |
| H | ? | settings.rs | 2175 |
| H | ? | settings.rs | 2392 |
| H | ? | settings.rs | 2450 |
| H | ? | settings.rs | 2554 |
| H | ? | settings.rs | 2555 |
| H | ? | settings.rs | 2647 |
| H | ? | settings.rs | 2648 |
| H | ? | settings.rs | 2748 |
| H | ? | settings.rs | 2749 |
| H | ? | settings.rs | 2773 |
| H | ? | settings.rs | 2889 |
| H | ? | settings.rs | 2890 |
| H | ? | settings.rs | 2935 |
| H | ? | settings.rs | 3089 |
| H | ? | settings.rs | 3090 |
| H | ? | settings.rs | 3127 |
| H | ? | settings.rs | 3203 |
| H | ? | settings.rs | 3204 |
| H | ? | settings.rs | 3209 |
| H | ? | settings.rs | 3235 |
| H | ? | settings.rs | 3240 |
| H | ? | settings.rs | 3282 |
| H | ? | settings.rs | 3288 |
| H | ? | settings.rs | 3387 |
| H | ? | settings.rs | 3403 |
| H | ? | settings.rs | 3412 |
| H | ? | settings.rs | 3424 |
| H | ? | settings.rs | 3432 |
| H | ? | settings.rs | 3698 |
| H | ? | settings.rs | 3714 |
| H | ? | settings.rs | 3723 |
| H | ? | settings.rs | 4164 |
| H | ? | settings.rs | 4170 |
| H | ? | settings.rs | 4415 |
| H | ? | settings.rs | 4418 |
| H | ? | settings.rs | 4421 |
| H | ? | settings.rs | 4433 |
| H | ? | settings.rs | 4529 |
| H | ? | settings.rs | 4544 |
| H | ? | settings.rs | 4547 |
| H | ? | settings.rs | 4550 |
| H | ? | settings.rs | 4833 |
| H | ? | settings.rs | 4942 |
| H | ? | settings.rs | 5066 |
| H | ? | settings.rs | 5274 |
| H | ? | lib.rs | 76 |
| H | ? | lib.rs | 83 |
| H | ? | lib.rs | 84 |
| H | ? | lib.rs | 85 |
| H | ? | lib.rs | 88 |
| H | ? | lib.rs | 148 |
| H | ? | lib.rs | 308 |
| H | ? | lib.rs | 483 |
| H | ? | lib.rs | 738 |
| H | ? | lib.rs | 739 |
| H | ? | lib.rs | 815 |
| H | ? | lib.rs | 858 |
| H | ? | lib.rs | 859 |
| H | ? | lib.rs | 904 |
| H | ? | lib.rs | 1003 |
| H | ? | lib.rs | 1016 |
| H | ? | lib.rs | 1030 |
| H | ? | lib.rs | 1031 |
| H | ? | lib.rs | 1066 |
| H | ? | lib.rs | 1309 |
| H | ? | lib.rs | 1377 |
| H | ? | lib.rs | 1378 |
| H | ? | lib.rs | 1510 |
| H | ? | lib.rs | 1544 |
| H | ? | lib.rs | 1545 |
| H | ? | lib.rs | 1635 |
| H | ? | lib.rs | 1636 |
| H | ? | lib.rs | 1637 |
| H | ? | lib.rs | 1665 |
| H | ? | lib.rs | 2084 |
| H | ? | lib.rs | 2085 |
| H | ? | lib.rs | 2198 |
| H | ? | lib.rs | 2314 |
| H | ? | lib.rs | 2315 |
| H | ? | lib.rs | 2385 |
| H | ? | lib.rs | 2386 |
| H | ? | lib.rs | 2442 |
| H | ? | lib.rs | 2443 |
| H | ? | lib.rs | 2490 |
| H | ? | lib.rs | 2562 |
| H | ? | lib.rs | 2575 |
| H | ? | lib.rs | 2589 |
| H | ? | lib.rs | 2590 |
| H | ? | lib.rs | 2658 |
| H | ? | lib.rs | 2659 |
| H | ? | lib.rs | 2713 |
| H | ? | lib.rs | 2714 |
| H | ? | lib.rs | 2884 |
| H | ? | lib.rs | 2885 |
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
| H | ? | lib.rs | 1043 |
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
| H | ? | virtualenv.rs | 221 |
| H | ? | virtualenv.rs | 235 |
| H | ? | virtualenv.rs | 238 |
| H | ? | virtualenv.rs | 241 |
| H | ? | virtualenv.rs | 482 |
| H | ? | virtualenv.rs | 542 |
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
| H | ? | hash.rs | 224 |
| H | ? | hash.rs | 360 |
| H | ? | hash.rs | 393 |
| H | ? | hash.rs | 394 |
| H | ? | hash.rs | 402 |
| H | ? | hash.rs | 403 |
| H | ? | hash.rs | 477 |
| H | ? | hash.rs | 478 |
| H | ? | hash.rs | 481 |
| H | ? | builds.rs | 72 |
| H | ? | distribution_database.rs | 88 |
| H | ? | distribution_database.rs | 150 |
| H | ? | distribution_database.rs | 152 |
| H | ? | distribution_database.rs | 204 |
| H | ? | distribution_database.rs | 220 |
| H | ? | distribution_database.rs | 232 |
| H | ? | distribution_database.rs | 239 |
| H | ? | distribution_database.rs | 270 |
| H | ? | distribution_database.rs | 277 |
| H | ? | distribution_database.rs | 297 |
| H | ? | distribution_database.rs | 309 |
| H | ? | distribution_database.rs | 316 |
| H | ? | distribution_database.rs | 335 |
| H | ? | distribution_database.rs | 346 |
| H | ? | distribution_database.rs | 353 |
| H | ? | distribution_database.rs | 371 |
| H | ? | distribution_database.rs | 454 |
| H | ? | distribution_database.rs | 467 |
| H | ? | distribution_database.rs | 498 |
| H | ? | distribution_database.rs | 520 |
| H | ? | distribution_database.rs | 588 |
| H | ? | distribution_database.rs | 638 |
| H | ? | distribution_database.rs | 781 |
| H | ? | distribution_database.rs | 789 |
| H | ? | distribution_database.rs | 817 |
| H | ? | distribution_database.rs | 992 |
| H | ? | distribution_database.rs | 1000 |
| H | ? | distribution_database.rs | 1028 |
| H | ? | distribution_database.rs | 1111 |
| H | ? | distribution_database.rs | 1118 |
| H | ? | distribution_database.rs | 1128 |
| H | ? | distribution_database.rs | 1135 |
| H | ? | distribution_database.rs | 1140 |
| H | ? | distribution_database.rs | 1147 |
| H | ? | distribution_database.rs | 1195 |
| H | ? | distribution_database.rs | 1200 |
| H | ? | distribution_database.rs | 1205 |
| H | ? | distribution_database.rs | 1212 |
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
| H | ? | mod.rs | 997 |
| H | ? | mod.rs | 1003 |
| H | ? | mod.rs | 1039 |
| H | ? | mod.rs | 1328 |
| H | ? | mod.rs | 1449 |
| H | ? | mod.rs | 1509 |
| H | ? | mod.rs | 1565 |
| H | ? | mod.rs | 1588 |
| H | ? | mod.rs | 1617 |
| H | ? | mod.rs | 1653 |
| H | ? | mod.rs | 1684 |
| H | ? | mod.rs | 1703 |
| H | ? | mod.rs | 1754 |
| H | ? | mod.rs | 1762 |
| H | ? | mod.rs | 1862 |
| H | ? | mod.rs | 1972 |
| H | ? | mod.rs | 2139 |
| H | ? | mod.rs | 2198 |
| H | ? | mod.rs | 2331 |
| H | ? | mod.rs | 2367 |
| H | ? | mod.rs | 2405 |
| H | ? | mod.rs | 2433 |
| H | ? | mod.rs | 2462 |
| H | ? | mod.rs | 2500 |
| H | ? | mod.rs | 2531 |
| H | ? | mod.rs | 2588 |
| H | ? | mod.rs | 2790 |
| H | ? | mod.rs | 2802 |
| H | ? | mod.rs | 2804 |
| H | ? | mod.rs | 3036 |
| H | ? | mod.rs | 3084 |
| H | ? | mod.rs | 3175 |
| H | ? | mod.rs | 3185 |
| H | ? | mod.rs | 3196 |
| H | ? | mod.rs | 3197 |
| H | ? | mod.rs | 3525 |
| H | ? | mod.rs | 3526 |
| H | ? | mod.rs | 3532 |
| H | ? | mod.rs | 3534 |
| H | ? | mod.rs | 3535 |
| H | ? | mod.rs | 3547 |
| H | ? | mod.rs | 3548 |
| H | ? | mod.rs | 3554 |
| H | ? | mod.rs | 3555 |
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
| H | ? | uv.rs | 283 |
| H | ? | uv.rs | 369 |
| H | ? | uv.rs | 379 |
| H | ? | uv.rs | 380 |
| H | ? | uv.rs | 391 |
| H | ? | uv.rs | 399 |
| H | ? | uv.rs | 400 |
| H | ? | uv.rs | 465 |
| H | ? | uv.rs | 503 |
| H | ? | uv.rs | 541 |
| H | ? | uv.rs | 548 |
| H | ? | uv.rs | 567 |
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
| H | ? | stream.rs | 124 |
| H | ? | stream.rs | 134 |
| H | ? | stream.rs | 145 |
| H | ? | stream.rs | 207 |
| H | ? | stream.rs | 222 |
| H | ? | stream.rs | 236 |
| H | ? | stream.rs | 252 |
| H | ? | stream.rs | 261 |
| H | ? | stream.rs | 279 |
| H | ? | stream.rs | 286 |
| H | ? | stream.rs | 296 |
| H | ? | stream.rs | 305 |
| H | ? | stream.rs | 314 |
| H | ? | stream.rs | 336 |
| H | ? | stream.rs | 395 |
| H | ? | stream.rs | 396 |
| H | ? | stream.rs | 403 |
| H | ? | stream.rs | 413 |
| H | ? | stream.rs | 424 |
| H | ? | stream.rs | 436 |
| H | ? | stream.rs | 460 |
| H | ? | stream.rs | 468 |
| H | ? | stream.rs | 540 |
| H | ? | sync.rs | 33 |
| H | ? | sync.rs | 34 |
| H | ? | sync.rs | 61 |
| H | ? | sync.rs | 104 |
| H | ? | sync.rs | 112 |
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
| H | ? | settings.rs | 2465 |
| H | ? | settings.rs | 2757 |
| H | ? | settings.rs | 2980 |
| H | ? | settings.rs | 2981 |
| H | ? | combine.rs | 271 |
| H | ? | combine.rs | 272 |
| H | ? | lib.rs | 134 |
| H | ? | lib.rs | 286 |
| H | ? | lib.rs | 955 |
| H | ? | backend.rs | 253 |
| H | ? | backend.rs | 254 |
| H | ? | backend.rs | 260 |
| H | ? | backend.rs | 267 |
| H | ? | unnamed.rs | 306 |
| H | ? | unnamed.rs | 316 |
| H | ? | specification.rs | 146 |
| H | ? | specification.rs | 149 |
| H | ? | specification.rs | 164 |
| H | ? | specification.rs | 169 |
| H | ? | specification.rs | 175 |
| H | ? | specification.rs | 183 |
| H | ? | specification.rs | 190 |
| H | ? | specification.rs | 198 |
| H | ? | specification.rs | 260 |
| H | ? | specification.rs | 266 |
| H | ? | specification.rs | 305 |
| H | ? | specification.rs | 311 |
| H | ? | specification.rs | 314 |
| H | ? | specification.rs | 337 |
| H | ? | specification.rs | 347 |
| H | ? | specification.rs | 357 |
| H | ? | specification.rs | 369 |
| H | ? | specification.rs | 372 |
| H | ? | specification.rs | 494 |
| H | ? | specification.rs | 499 |
| H | ? | specification.rs | 520 |
| H | ? | specification.rs | 525 |
| H | ? | specification.rs | 576 |
| H | ? | specification.rs | 577 |
| H | ? | specification.rs | 616 |
| H | ? | specification.rs | 617 |
| H | ? | specification.rs | 644 |
| H | ? | specification.rs | 645 |
| H | ? | specification.rs | 748 |
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
| H | ? | tree.rs | 1190 |
| H | ? | tree.rs | 3666 |
| H | ? | tree.rs | 3671 |
| H | ? | tree.rs | 3678 |
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
| H | ? | unnamed.rs | 400 |
| H | ? | unnamed.rs | 411 |
| H | ? | verbatim_url.rs | 165 |
| H | ? | verbatim_url.rs | 166 |
| H | ? | verbatim_url.rs | 206 |
| H | ? | verbatim_url.rs | 301 |
| H | ? | cursor.rs | 45 |
| H | ? | cursor.rs | 50 |
| H | ? | cursor.rs | 85 |
| H | ? | lib.rs | 453 |
| H | ? | lib.rs | 730 |
| H | ? | lib.rs | 741 |
| H | ? | lib.rs | 946 |
| H | ? | lib.rs | 974 |
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
| H | ? | wheel.rs | 289 |
| H | ? | wheel.rs | 699 |
| H | ? | linker.rs | 71 |
| H | ? | linker.rs | 185 |
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
*Сгенерировано GSC v0.6 · 2026-08-05T04:03:58.646530*