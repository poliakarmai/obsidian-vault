---
title: "GSC Audit: /tmp/gsc-external/cyberbro"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/cyberbro

**Дата:** 08.08.2026 19:21  
**Путь:** `/tmp/gsc-external/cyberbro`  
**Всего находок:** 193  
**CRITICAL:** 1 | **HIGH:** 17 | **MEDIUM:** 0 | **LOW:** 83

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 65 |
| GS015 | 30 |
| GS003 | 23 |
| GS022 | 23 |
| GS020 | 19 |
| GS025-hardcoded_secret | 13 |
| GS025 | 10 |
| GS021 | 5 |
| GS001 | 1 |
| GS036-redos | 1 |
| GS002 | 1 |
| GS009 | 1 |
| GS011 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | app.py | 94 | Found: sqlite:///{DATA_DIR /  |
| HIGH | GS025 | chrome_extension.py | 29 |  |
| HIGH | GS025 | microsoft_defender_for_endpoint.py | 81 |  |
| HIGH | GS025 | alienvault.py | 118 |  |
| HIGH | GS025 | ipquery.py | 28 |  |
| HIGH | GS025 | base_engine.py | 98 |  |
| HIGH | GS025 | app.py | 179 |  |
| HIGH | GS000-LEGACY | config.py | 31 | Match:     flask_host: str = "127.0.0.1" |
| HIGH | GS000-LEGACY | utils.py | 169 | Match:     ::(ffff(:0{1,4}){0,1}:){0,1}                      |
| HIGH | GS000-LEGACY | utils.py | 172 | Match:     ([0-9a-fA-F]{1,4}:){1,4}:                         |
| HIGH | GS000-LEGACY | index.html | 6 | Match: 1.2.3.4 |
| HIGH | GS000-LEGACY | docker-compose.yml | 22 | Match:       - FLASK_HOST=0.0.0.0 |
| HIGH | GS000-LEGACY | docker-compose.yml | 64 | Match:           "python -c \"import os,urllib.request; port |
| HIGH | GS025 | .bandit.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | secrets_json_to_env.py | 0 | File secrets_json_to_env.py has permissions -rw-rw-r-- — rea |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| L | GS000-LEGACY | spur_us.py | 29 |
| H | GS025 | chrome_extension.py | 29 |
| H | GS025 | microsoft_defender_for_endpoint.py | 81 |
| H | GS025 | alienvault.py | 118 |
| H | GS025 | ipquery.py | 28 |
| H | GS025 | base_engine.py | 98 |
| H | GS025 | app.py | 179 |
| C | GS001 | app.py | 94 |
| L | GS003 | app.py | 157 |
| L | GS003 | config.py | 111 |
| L | GS003 | config.py | 196 |
| L | GS003 | config.py | 211 |
| L | GS003 | history.js | 92 |
| L | GS003 | history.js | 118 |
| L | GS003 | history.js | 143 |
| L | GS003 | json-viewer.js | 6 |
| L | GS003 | json-viewer.js | 13 |
| L | GS003 | json-viewer.js | 22 |
| L | GS003 | json-viewer.js | 25 |
| L | GS003 | json-viewer.js | 28 |
| L | GS003 | json-viewer.js | 57 |
| L | GS003 | json-viewer.js | 103 |
| L | GS003 | json-viewer.js | 135 |
| L | GS003 | json-viewer.js | 148 |
| L | GS003 | json-viewer.js | 176 |
| L | GS003 | json-viewer.js | 184 |
| L | GS003 | json-viewer.js | 246 |
| L | GS003 | json-viewer.js | 353 |
| L | GS003 | json-viewer.js | 409 |
| L | GS003 | table-row-expansion.js | 26 |
| L | GS003 | table-row-expansion.js | 27 |
| I | GS015 | app.py | 218 |
| I | GS015 | app.py | 233 |
| I | GS015 | app.py | 272 |
| I | GS015 | app.py | 289 |
| I | GS015 | app.py | 296 |
| I | GS015 | app.py | 311 |
| I | GS015 | app.py | 339 |
| I | GS015 | app.py | 389 |
| I | GS015 | app.py | 396 |
| I | GS015 | app.py | 402 |
| I | GS015 | app.py | 218 |
| I | GS015 | app.py | 233 |
| I | GS015 | app.py | 272 |
| I | GS015 | app.py | 289 |
| I | GS015 | app.py | 296 |
| I | GS015 | app.py | 311 |
| I | GS015 | app.py | 339 |
| I | GS015 | app.py | 389 |
| I | GS015 | app.py | 396 |
| I | GS015 | app.py | 402 |
| I | GS015 | app.py | 218 |
| I | GS015 | app.py | 233 |
| I | GS015 | app.py | 272 |
| I | GS015 | app.py | 289 |
| I | GS015 | app.py | 296 |
| I | GS015 | app.py | 311 |
| I | GS015 | app.py | 339 |
| I | GS015 | app.py | 389 |
| I | GS015 | app.py | 396 |
| I | GS015 | app.py | 402 |
| i | GS020 |  | 148 |
| i | GS020 |  | 282 |
| i | GS020 |  | 286 |
| i | GS020 |  | 394 |
| i | GS020 |  | 448 |
| i | GS020 |  | 14 |
| i | GS020 |  | 20 |
| i | GS020 |  | 65 |
| i | GS020 |  | 154 |
| i | GS020 |  | 50 |
| i | GS020 |  | 50 |
| i | GS020 |  | 105 |
| i | GS020 |  | 35 |
| i | GS020 |  | 43 |
| i | GS020 |  | 46 |
| i | GS020 |  | 80 |
| i | GS020 |  | 86 |
| i | GS020 |  | 92 |
| i | GS020 |  | 83 |
| ? | GS036-redos | history.js | 50 |
| H | GS000-LEGACY | config.py | 31 |
| H | GS000-LEGACY | utils.py | 169 |
| H | GS000-LEGACY | utils.py | 172 |
| H | GS000-LEGACY | index.html | 6 |
| H | GS000-LEGACY | docker-compose.yml | 22 |
| H | GS000-LEGACY | docker-compose.yml | 64 |
| H | GS025 | .bandit.yml | 0 |
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS025 | mkdocs.yml | 0 |
| H | GS002 | secrets_json_to_env.py | 0 |
| s | GS009 |  | 0 |
| L | GS011 | microsoft_defender_for_endpoint.py | 38 |
| c | GS021 |  | 233 |
| c | GS021 |  | 411 |
| s | GS021 |  | 31 |
| s | GS021 |  | 28 |
| s | GS021 |  | 164 |
| r | GS022 |  | 24 |
| r | GS022 |  | 3 |
| r | GS022 |  | 45 |
| r | GS022 |  | 4 |
| r | GS022 |  | 31 |
| r | GS022 |  | 27 |
| r | GS022 |  | 69 |
| r | GS022 |  | 127 |
| r | GS022 |  | 29 |
| r | GS022 |  | 108 |
| r | GS022 |  | 111 |
| r | GS022 |  | 225 |
| r | GS022 |  | 232 |
| r | GS022 |  | 93 |
| r | GS022 |  | 132 |
| r | GS022 |  | 69 |
| r | GS022 |  | 128 |
| r | GS022 |  | 56 |
| r | GS022 |  | 67 |
| r | GS022 |  | 78 |
| r | GS022 |  | 54 |
| r | GS022 |  | 64 |
| r | GS022 |  | 75 |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-08T19:21:07.322786*