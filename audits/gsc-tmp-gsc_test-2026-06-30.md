---
title: "GSC Audit: /tmp/gsc_test"
date: 2026-06-30
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_test

**Дата:** 30.06.2026 08:28  
**Путь:** `/tmp/gsc_test`  
**Всего находок:** 7  
**CRITICAL:** 3 | **HIGH:** 2 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS016 | 5 |
| chmod: World-readable configs | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | dangerous.sh | 3 | Match: chmod 4777 /usr/bin/bash |
| CRITICAL | GS016 | dangerous.sh | 3 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS016 | dangerous.sh | 4 | SUID binary outside standard system paths — potential privil |
| HIGH | GS016 | dangerous.sh | 8 | eval/exec with untrusted input — arbitrary code execution |
| HIGH | GS016 | dangerous.sh | 9 | Dangerous Linux capability on binary — container escape or p |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | dangerous.sh | 3 |
| s | GS009 |  | 0 |
| C | GS016 | dangerous.sh | 3 |
| C | GS016 | dangerous.sh | 4 |
| M | GS016 | dangerous.sh | 7 |
| H | GS016 | dangerous.sh | 8 |
| H | GS016 | dangerous.sh | 9 |

---
*Сгенерировано GSC v0.6 · 2026-06-30T08:28:51.369292*