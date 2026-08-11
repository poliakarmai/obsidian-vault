---
title: "GSC Audit: /home/openclaw/gsc/enterprise"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc/enterprise

**Дата:** 08.08.2026 04:08  
**Путь:** `/home/openclaw/gsc/enterprise`  
**Всего находок:** 24  
**CRITICAL:** 21 | **HIGH:** 1 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS001 | 18 |
| GS005 | 3 |
| GS010 | 1 |
| GS009 | 1 |
| GS019 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS019" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS029" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS001" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS005" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS030" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS031" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS028" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS001" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS005" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS017" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS019" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS029" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS030" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS030" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS031" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS028" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS019" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS029" |
| CRITICAL | GS005 | tenancy.py | 13 | Line 13: conn.execute(f"ALTER TABLE {t} ENABLE ROW LEVEL SEC |
| CRITICAL | GS005 | tenancy.py | 14 | Line 14: conn.execute(f"ALTER TABLE {t} FORCE ROW LEVEL SECU |
| CRITICAL | GS005 | tenancy.py | 15 | Line 15: conn.execute(f"CREATE POLICY tenant_isolation_{t} O |
| HIGH | GS019 | sso.py | 37 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS010 | sso.py | 22 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS005 | tenancy.py | 13 |
| C | GS005 | tenancy.py | 14 |
| C | GS005 | tenancy.py | 15 |
| s | GS009 |  | 0 |
| H | GS019 | sso.py | 37 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T04:08:58.815487*