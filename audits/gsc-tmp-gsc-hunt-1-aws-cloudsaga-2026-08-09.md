---
title: "GSC Audit: /tmp/gsc-hunt-1/aws-cloudsaga"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-1/aws-cloudsaga

**Дата:** 09.08.2026 08:05  
**Путь:** `/tmp/gsc-hunt-1/aws-cloudsaga`  
**Всего находок:** 24  
**CRITICAL:** 4 | **HIGH:** 1 | **MEDIUM:** 0 | **LOW:** 13

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 12 |
| GS025 | 4 |
| GS032-fake_tool_call_execute | 4 |
| GS000-LEGACY | 1 |
| GS009 | 1 |
| GS014 | 1 |
| GS021 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS025 | imds_reveal.py | 58 |  |
| CRITICAL | GS025 | imds_reveal.py | 62 |  |
| CRITICAL | GS025 | imds_reveal.py | 63 |  |
| CRITICAL | GS025 | imds_reveal.py | 65 |  |
| HIGH | GS000-LEGACY | imds_reveal.py | 62 | Match:         os.system("curl http://{ip}/?url=http://169.2 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS025 | imds_reveal.py | 58 |
| C | GS025 | imds_reveal.py | 62 |
| C | GS025 | imds_reveal.py | 63 |
| C | GS025 | imds_reveal.py | 65 |
| L | GS003 | cloudsaga.py | 35 |
| L | GS003 | cloudsaga.py | 78 |
| L | GS003 | cloudsaga.py | 89 |
| L | GS003 | cloudsaga.py | 101 |
| L | GS003 | cloudsaga.py | 112 |
| L | GS003 | cloudsaga.py | 124 |
| L | GS003 | cloudsaga.py | 133 |
| L | GS003 | imds_reveal.py | 46 |
| L | GS003 | imds_reveal.py | 50 |
| L | GS003 | public_resources.py | 69 |
| L | GS003 | public_resources.py | 72 |
| L | GS003 | public_resources.py | 76 |
| ? | GS032-fake_tool_call_execute | imds_reveal.py | 58 |
| ? | GS032-fake_tool_call_execute | imds_reveal.py | 62 |
| ? | GS032-fake_tool_call_execute | imds_reveal.py | 63 |
| ? | GS032-fake_tool_call_execute | imds_reveal.py | 65 |
| H | GS000-LEGACY | imds_reveal.py | 62 |
| s | GS009 |  | 0 |
| L | GS014 | iam_credentials.py | 1 |
| s | GS021 |  | 62 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T08:05:38.577325*