---
title: "GSC Audit: /tmp/gsc-hunt-2"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-2

**Дата:** 09.08.2026 12:01  
**Путь:** `/tmp/gsc-hunt-2`  
**Всего находок:** 71  
**CRITICAL:** 3 | **HIGH:** 6 | **MEDIUM:** 6 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 31 |
| GS021 | 16 |
| GS000-LEGACY | 7 |
| GS025-hardcoded_secret | 5 |
| GS005 | 3 |
| GS025-no_rate_limit_auth | 3 |
| GS025 | 2 |
| GS007 | 2 |
| GS009 | 1 |
| GS019 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | sqlite.py | 62 | OWASP A03: Injection |
| CRITICAL | GS005 | sqlite.py | 62 |  |
| CRITICAL | GS005 | sqlite.py | 62 | Line 62: cursor.execute(f"DELETE FROM {table_name}") |
| HIGH | GS000-LEGACY | additional.py | 212 | File upload without MIME-type validation → malicious file up |
| HIGH | GS025 | .env | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | clipbin.db | 0 | Permissions 664 — should be 600 |
| HIGH | GS007 | app.py | 95 | Line 95: data = db.execute("SELECT uri FROM twoFA WHERE user |
| HIGH | GS007 | app.py | 647 | Line 647: data = db.execute("SELECT uri FROM twoFA WHERE use |
| HIGH | GS019 | app.py | 585 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | sqlite.py | 62 |
| H | GS000-LEGACY | additional.py | 212 |
| M | GS000-LEGACY | app.py | 261 |
| M | GS000-LEGACY | app.py | 470 |
| M | GS000-LEGACY | app.py | 480 |
| M | GS000-LEGACY | app.py | 484 |
| M | GS000-LEGACY | app.py | 490 |
| M | GS000-LEGACY | app.py | 516 |
| C | GS005 | sqlite.py | 62 |
| I | GS015 | app.py | 142 |
| I | GS015 | app.py | 267 |
| I | GS015 | app.py | 268 |
| I | GS015 | app.py | 369 |
| I | GS015 | app.py | 370 |
| I | GS015 | app.py | 413 |
| I | GS015 | app.py | 432 |
| I | GS015 | app.py | 438 |
| I | GS015 | app.py | 444 |
| I | GS015 | app.py | 523 |
| I | GS015 | app.py | 142 |
| I | GS015 | app.py | 267 |
| I | GS015 | app.py | 268 |
| I | GS015 | app.py | 369 |
| I | GS015 | app.py | 370 |
| I | GS015 | app.py | 413 |
| I | GS015 | app.py | 432 |
| I | GS015 | app.py | 438 |
| I | GS015 | app.py | 444 |
| I | GS015 | app.py | 523 |
| I | GS015 | app.py | 142 |
| I | GS015 | app.py | 267 |
| I | GS015 | app.py | 268 |
| I | GS015 | app.py | 369 |
| I | GS015 | app.py | 370 |
| I | GS015 | app.py | 413 |
| I | GS015 | app.py | 432 |
| I | GS015 | app.py | 438 |
| I | GS015 | app.py | 444 |
| I | GS015 | app.py | 523 |
| I | GS015 | app.py | 36 |
| H | GS025 | .env | 0 |
| H | GS025 | clipbin.db | 0 |
| C | GS005 | sqlite.py | 62 |
| H | GS007 | app.py | 95 |
| H | GS007 | app.py | 647 |
| s | GS009 |  | 0 |
| H | GS019 | app.py | 585 |
| c | GS021 |  | 142 |
| c | GS021 |  | 267 |
| c | GS021 |  | 268 |
| c | GS021 |  | 369 |
| c | GS021 |  | 370 |
| c | GS021 |  | 413 |
| c | GS021 |  | 444 |
| c | GS021 |  | 541 |
| c | GS021 |  | 584 |
| c | GS021 |  | 626 |
| c | GS021 |  | 668 |
| c | GS021 |  | 750 |
| c | GS021 |  | 785 |
| c | GS021 |  | 841 |
| c | GS021 |  | 888 |
| c | GS021 |  | 1003 |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-09T12:01:49.004748*