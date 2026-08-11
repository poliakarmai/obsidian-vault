---
title: "GSC Audit: /home/openclaw/gsc/cloud"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc/cloud

**Дата:** 08.08.2026 04:09  
**Путь:** `/home/openclaw/gsc/cloud`  
**Всего находок:** 52  
**CRITICAL:** 1 | **HIGH:** 12 | **MEDIUM:** 5 | **LOW:** 5

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS007 | 23 |
| GS000-LEGACY | 6 |
| GS022 | 5 |
| Синхронный код в async | 5 |
| GS003 | 3 |
| GS025 | 2 |
| GS014 | 2 |
| GS021 | 2 |
| GS001 | 1 |
| GS008 | 1 |
| GS009 | 1 |
| GS011 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | github_auth.py | 40 | Found: "RS256" |
| HIGH | GS000-LEGACY | user_auth.py | 60 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | sso.py | 36 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS025 | user_auth.py | 60 |  |
| HIGH | GS025 | sso.py | 36 |  |
| HIGH | GS000-LEGACY | Dockerfile | 18 | Match: CMD ["uvicorn", "cloud.api:app", "--host", "0.0.0.0", |
| HIGH | GS000-LEGACY | docker-compose.yml | 35 | Match:     command: uvicorn cloud.api:app --host 0.0.0.0 --p |
| HIGH | GS000-LEGACY | user_auth.py | 60 | Match:     user = requests.get(f"{GH_API}/user", |
| HIGH | GS000-LEGACY | sso.py | 36 | Match:     resp = requests.get(f"{issuer_url.rstrip('/')}/.w |
| HIGH | GS007 | api.py | 65 | Line 65: @app.get("/api/v2/scans/{scan_id}") |
| HIGH | GS007 | user_auth.py | 123 | Line 123: SELECT tenant_id FROM memberships WHERE user_id =  |
| HIGH | GS014 | docker-compose.yml | 37 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | docker-compose.yml | 62 | Database URL contains password in plaintext. Use environment |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS000-LEGACY | user_auth.py | 60 |
| H | GS000-LEGACY | sso.py | 36 |
| H | GS025 | user_auth.py | 60 |
| H | GS025 | sso.py | 36 |
| C | GS001 | github_auth.py | 40 |
| L | GS003 | manage.py | 41 |
| L | GS003 | manage.py | 42 |
| L | GS003 | workers.py | 173 |
| L | GS008 | session.py | 47 |
| H | GS000-LEGACY | Dockerfile | 18 |
| H | GS000-LEGACY | docker-compose.yml | 35 |
| H | GS000-LEGACY | user_auth.py | 60 |
| H | GS000-LEGACY | sso.py | 36 |
| H | GS007 | api.py | 65 |
| I | GS007 | federated_server.py | 16 |
| I | GS007 | schema_s1.sql | 3 |
| I | GS007 | schema_s1.sql | 12 |
| I | GS007 | schema_s1.sql | 21 |
| I | GS007 | schema_s1.sql | 29 |
| I | GS007 | schema_s1.sql | 44 |
| I | GS007 | schema_s1.sql | 58 |
| I | GS007 | schema_s2.sql | 4 |
| I | GS007 | schema_s2.sql | 27 |
| I | GS007 | schema_s2.sql | 40 |
| I | GS007 | schema_s2.sql | 51 |
| I | GS007 | schema_s2.sql | 64 |
| I | GS007 | schema_s2.sql | 77 |
| I | GS007 | schema_s3.sql | 4 |
| I | GS007 | schema_s3.sql | 14 |
| I | GS007 | schema_s3.sql | 31 |
| I | GS007 | schema_s4.sql | 5 |
| I | GS007 | schema_s4.sql | 46 |
| I | GS007 | schema_s5.sql | 4 |
| I | GS007 | schema_s5.sql | 15 |
| I | GS007 | schema_s5.sql | 27 |
| H | GS007 | user_auth.py | 123 |
| s | GS009 |  | 0 |
| L | GS011 | sso.py | 107 |
| H | GS014 | docker-compose.yml | 37 |
| H | GS014 | docker-compose.yml | 62 |
| s | GS021 |  | 119 |
| s | GS021 |  | 28 |
| r | GS022 |  | 23 |
| r | GS022 |  | 24 |
| r | GS022 |  | 53 |
| r | GS022 |  | 18 |
| r | GS022 |  | 29 |
| M | ? | github_worker.py | 35 |
| M | ? | github_worker.py | 38 |
| M | ? | github_worker.py | 58 |
| M | ? | workers.py | 135 |
| M | ? | worker.py | 46 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:09:07.402711*