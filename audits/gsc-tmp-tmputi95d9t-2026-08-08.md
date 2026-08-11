---
title: "GSC Audit: /tmp/tmputi95d9t"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmputi95d9t

**Дата:** 08.08.2026 11:52  
**Путь:** `/tmp/tmputi95d9t`  
**Всего находок:** 52  
**CRITICAL:** 0 | **HIGH:** 15 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS021 | 25 |
| GS000-LEGACY | 13 |
| GS022 | 7 |
| GS020 | 2 |
| GS025 | 2 |
| GS025-eval_usage | 2 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | GS000-LEGACY | app.listen.js | 29 | Match:     const server = app.listen(0, '127.0.0.1', 5, func |
| HIGH | GS000-LEGACY | app.listen.js | 31 | Match:       assert.strictEqual(address, '127.0.0.1'); |
| HIGH | GS000-LEGACY | req.host.js | 93 | Match:         app.set('trust proxy', '10.0.0.1'); |
| HIGH | GS000-LEGACY | req.hostname.js | 93 | Match:         app.set('trust proxy', '10.0.0.1'); |
| HIGH | GS000-LEGACY | req.subdomains.js | 31 | Match:         .set('Host', '127.0.0.1') |
| HIGH | GS000-LEGACY | req.subdomains.js | 121 | Match:           .set('Host', '127.0.0.1') |
| HIGH | GS000-LEGACY | req.subdomains.js | 122 | Match:           .expect(200, ['127.0.0.1'], done); |
| HIGH | GS000-LEGACY | req.protocol.js | 54 | Match:         app.set('trust proxy', '10.0.0.1'); |
| HIGH | GS000-LEGACY | req.ip.js | 43 | Match:           app.set('trust proxy', '10.0.0.1, 10.0.0.2, |
| HIGH | GS000-LEGACY | req.ip.js | 51 | Match:             .set('X-Forwarded-For', '10.0.0.2, 10.0.0 |
| HIGH | GS000-LEGACY | req.ip.js | 52 | Match:             .expect('10.0.0.3', done) |
| HIGH | GS000-LEGACY | req.ip.js | 111 | Match:     ? '::ffff:127.0.0.1' |
| HIGH | GS000-LEGACY | req.ip.js | 112 | Match:     : '127.0.0.1'; |
| HIGH | GS025 | package.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .eslintrc.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| i | GS020 |  | 115 |
| i | GS020 |  | 116 |
| H | GS000-LEGACY | app.listen.js | 29 |
| H | GS000-LEGACY | app.listen.js | 31 |
| H | GS000-LEGACY | req.host.js | 93 |
| H | GS000-LEGACY | req.hostname.js | 93 |
| H | GS000-LEGACY | req.subdomains.js | 31 |
| H | GS000-LEGACY | req.subdomains.js | 121 |
| H | GS000-LEGACY | req.subdomains.js | 122 |
| H | GS000-LEGACY | req.protocol.js | 54 |
| H | GS000-LEGACY | req.ip.js | 43 |
| H | GS000-LEGACY | req.ip.js | 51 |
| H | GS000-LEGACY | req.ip.js | 52 |
| H | GS000-LEGACY | req.ip.js | 111 |
| H | GS000-LEGACY | req.ip.js | 112 |
| H | GS025 | package.json | 0 |
| H | GS025 | .eslintrc.yml | 0 |
| s | GS009 |  | 0 |
| s | GS021 |  | 29 |
| s | GS021 |  | 31 |
| s | GS021 |  | 85 |
| s | GS021 |  | 101 |
| s | GS021 |  | 103 |
| s | GS021 |  | 133 |
| s | GS021 |  | 150 |
| s | GS021 |  | 152 |
| s | GS021 |  | 85 |
| s | GS021 |  | 101 |
| s | GS021 |  | 103 |
| s | GS021 |  | 133 |
| s | GS021 |  | 149 |
| s | GS021 |  | 165 |
| s | GS021 |  | 182 |
| s | GS021 |  | 184 |
| s | GS021 |  | 31 |
| s | GS021 |  | 121 |
| s | GS021 |  | 122 |
| s | GS021 |  | 43 |
| s | GS021 |  | 111 |
| s | GS021 |  | 112 |
| s | GS021 |  | 14 |
| s | GS021 |  | 15 |
| s | GS021 |  | 16 |
| r | GS022 |  | 798 |
| r | GS022 |  | 115 |
| r | GS022 |  | 130 |
| r | GS022 |  | 158 |
| r | GS022 |  | 159 |
| r | GS022 |  | 282 |
| r | GS022 |  | 634 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-08T11:52:41.198734*