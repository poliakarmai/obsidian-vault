---
title: "GSC Audit: /tmp/gsc-hunt-3/quiet-riot"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-3/quiet-riot

**Дата:** 09.08.2026 08:02  
**Путь:** `/tmp/gsc-hunt-3/quiet-riot`  
**Всего находок:** 193  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 140

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 118 |
| GS015 | 33 |
| GS003 | 21 |
| GS020 | 14 |
| GS021 | 2 |
| GS025 | 1 |
| GS002 | 1 |
| GS009 | 1 |
| GS014 | 1 |
| Deep analysis requires OpenRouter API key | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | secretsmanagerenum.py | 0 | File secretsmanagerenum.py has permissions -rw-rw-r-- — read |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS002 | secretsmanagerenum.py | 0 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS000-LEGACY | s3enum.py | 28 |
| L | GS000-LEGACY | s3enum.py | 31 |
| L | GS003 | codeartifactenum.py | 30 |
| L | GS003 | codeartifactenum.py | 33 |
| L | GS003 | iamassumeroleenum.py | 20 |
| L | GS003 | iamassumeroleenum.py | 22 |
| L | GS003 | lambdaenum.py | 19 |
| L | GS003 | s3enum.py | 33 |
| L | GS003 | app.js | 157 |
| L | GS003 | app.js | 161 |
| L | GS003 | app.js | 166 |
| L | GS003 | app.js | 184 |
| L | GS003 | app.js | 195 |
| L | GS003 | app.js | 199 |
| L | GS003 | app.js | 202 |
| L | GS003 | app.js | 207 |
| L | GS003 | app.js | 219 |
| L | GS003 | app.js | 233 |
| L | GS003 | app.js | 235 |
| L | GS003 | app.js | 251 |
| L | GS003 | app.js | 254 |
| L | GS003 | app.js | 257 |
| L | GS003 | app.js | 261 |
| I | GS015 | server.py | 154 |
| I | GS015 | server.py | 161 |
| I | GS015 | server.py | 220 |
| I | GS015 | server.py | 265 |
| I | GS015 | server.py | 288 |
| I | GS015 | server.py | 478 |
| I | GS015 | server.py | 499 |
| I | GS015 | server.py | 515 |
| I | GS015 | server.py | 610 |
| I | GS015 | server.py | 743 |
| I | GS015 | server.py | 154 |
| I | GS015 | server.py | 161 |
| I | GS015 | server.py | 220 |
| I | GS015 | server.py | 265 |
| I | GS015 | server.py | 288 |
| I | GS015 | server.py | 478 |
| I | GS015 | server.py | 499 |
| I | GS015 | server.py | 515 |
| I | GS015 | server.py | 610 |
| I | GS015 | server.py | 743 |
| I | GS015 | server.py | 154 |
| I | GS015 | server.py | 161 |
| I | GS015 | server.py | 220 |
| I | GS015 | server.py | 265 |
| I | GS015 | server.py | 288 |
| I | GS015 | server.py | 478 |
| I | GS015 | server.py | 499 |
| I | GS015 | server.py | 515 |
| I | GS015 | server.py | 610 |
| I | GS015 | server.py | 743 |
| I | GS015 | server.py | 155 |
| I | GS015 | server.py | 99 |
| I | GS015 | main.py | 1 |
| i | GS020 |  | 46 |
| i | GS020 |  | 54 |
| i | GS020 |  | 108 |
| i | GS020 |  | 25 |
| i | GS020 |  | 56 |
| i | GS020 |  | 66 |
| i | GS020 |  | 76 |
| i | GS020 |  | 84 |
| i | GS020 |  | 15 |
| i | GS020 |  | 27 |
| i | GS020 |  | 40 |
| i | GS020 |  | 43 |
| i | GS020 |  | 142 |
| i | GS020 |  | 142 |
| s | GS009 |  | 0 |
| L | GS014 | aws_credentials.py | 1 |
| s | GS021 |  | 69 |
| s | GS021 |  | 836 |
| I | ? |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T08:02:29.803477*