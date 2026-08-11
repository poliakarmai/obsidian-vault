---
title: "GSC Audit: /tmp/gsc-external/carnivore"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/carnivore

**Дата:** 09.08.2026 06:12  
**Путь:** `/tmp/gsc-external/carnivore`  
**Всего находок:** 57  
**CRITICAL:** 1 | **HIGH:** 4 | **MEDIUM:** 0 | **LOW:** 22

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 18 |
| GS022 | 16 |
| GS021 | 6 |
| GS000-LEGACY | 4 |
| GS008 | 4 |
| GS015 | 3 |
| GS020 | 2 |
| GS025 | 1 |
| GS009 | 1 |
| GS025-hardcoded_secret | 1 |
| Deep analysis requires OpenRouter API key | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS025 | Dockerfile | 72 | Match:     chmod 0755 /usr/local/bin/monolith; \ |
| HIGH | GS000-LEGACY | github_upload.py | 40 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | github_upload.py | 53 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | render.py | 43 | Match:     " (KHTML, like Gecko) Chrome/131.0.0.0 Safari/537 |
| HIGH | GS000-LEGACY | lib.py | 62 | Match: USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X  |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS025 | Dockerfile | 72 |
| H | GS000-LEGACY | github_upload.py | 40 |
| H | GS000-LEGACY | github_upload.py | 53 |
| H | GS000-LEGACY | render.py | 43 |
| H | GS000-LEGACY | lib.py | 62 |
| L | GS003 | main.py | 71 |
| L | GS003 | main.py | 83 |
| L | GS003 | main.py | 88 |
| L | GS003 | main.py | 90 |
| L | GS003 | main.py | 19 |
| L | GS003 | main.py | 24 |
| L | GS003 | main.py | 33 |
| L | GS003 | main.py | 35 |
| L | GS003 | main.py | 36 |
| L | GS003 | cli.py | 63 |
| L | GS003 | cli.py | 75 |
| L | GS003 | cli.py | 77 |
| L | GS003 | cli.py | 83 |
| L | GS003 | cli.py | 93 |
| L | GS003 | frontmatter.py | 71 |
| L | GS003 | frontmatter.py | 74 |
| L | GS003 | github_upload.py | 91 |
| L | GS003 | index.mjs | 29 |
| L | GS008 | models.py | 5 |
| L | GS008 | models.py | 6 |
| L | GS008 | models.py | 18 |
| L | GS008 | render.py | 36 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 81 |
| i | GS020 |  | 105 |
| i | GS020 |  | 118 |
| s | GS009 |  | 0 |
| s | GS021 |  | 11 |
| s | GS021 |  | 15 |
| s | GS021 |  | 186 |
| s | GS021 |  | 56 |
| s | GS021 |  | 60 |
| s | GS021 |  | 53 |
| r | GS022 |  | 23 |
| r | GS022 |  | 28 |
| r | GS022 |  | 33 |
| r | GS022 |  | 55 |
| r | GS022 |  | 238 |
| r | GS022 |  | 358 |
| r | GS022 |  | 476 |
| r | GS022 |  | 92 |
| r | GS022 |  | 148 |
| r | GS022 |  | 313 |
| r | GS022 |  | 432 |
| r | GS022 |  | 442 |
| r | GS022 |  | 450 |
| r | GS022 |  | 496 |
| r | GS022 |  | 502 |
| r | GS022 |  | 556 |
| ? | GS025-hardcoded_secret |  | ? |
| I | ? |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T06:12:37.028471*