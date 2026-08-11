---
title: "GSC Audit: /tmp/gsc-external/fastadmin"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/fastadmin

**Дата:** 08.08.2026 19:18  
**Путь:** `/tmp/gsc-external/fastadmin`  
**Всего находок:** 584  
**CRITICAL:** 10 | **HIGH:** 291 | **MEDIUM:** 10 | **LOW:** 16

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 271 |
| GS025-eval_usage | 84 |
| GS020 | 75 |
| GS022 | 48 |
| GS021 | 36 |
| Rust: .clone() in hot path | 19 |
| GS003 | 15 |
| GS001 | 7 |
| GS019 | 6 |
| GS025 | 3 |
| GS015 | 3 |
| GS036-redos | 3 |
| GS025-insecure_random | 3 |
| GS005 | 2 |
| GS032-exfil_env_send | 1 |
| GS034-token_collector | 1 |
| GS029 | 1 |
| GS007 | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS025-debug_mode | 1 |
| GS025-wildcard_bind | 1 |
| TS: useEffect missing deps | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | index.min.js | 9 | OWASP A03: Injection |
| CRITICAL | GS005 | index.min.js | 395 | OWASP A03: Injection |
| CRITICAL | GS001 | service.py | 68 | Found: "HS256" |
| CRITICAL | GS001 | service.py | 198 | Found: "HS256" |
| CRITICAL | GS001 | tsconfig.json | 6 | Found: "ES2020" |
| CRITICAL | GS001 | tsconfig.json | 8 | Found: "ES2020" |
| CRITICAL | GS001 | vite.config.ts | 46 | Found: "es2015" |
| CRITICAL | GS001 | pyproject.toml | 93 | Found: "py312" |
| CRITICAL | GS001 | pyproject.toml | 139 | Found: "UP042" |
| CRITICAL | GS029 | index.min.js | 250 | Match:           &${r}-slide-up-leave${r}-slide-up-leave-act |
| HIGH | GS000-LEGACY | index.test.tsx | 65 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 66 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 182 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 234 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 315 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 354 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 433 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 454 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 455 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 500 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 112 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 164 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 180 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 205 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 231 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 266 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 297 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 304 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 312 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 316 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 477 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 23 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 110 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 114 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 122 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 153 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 176 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 215 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 276 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 288 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 294 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 305 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 100 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 111 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 251 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 310 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 374 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 451 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 34 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 36 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 38 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 45 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 46 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 54 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 60 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 95 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 111 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 112 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 113 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 114 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 115 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 116 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 120 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 110 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 201 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 235 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 24 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 26 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 80 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 156 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 172 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 185 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 234 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 152 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 153 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 30 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 32 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 54 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 75 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 7 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 9 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 159 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 160 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 42 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 53 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 237 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 297 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 44 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 69 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 140 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 141 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 143 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 145 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 303 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 9 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 13 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 23 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 35 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 90 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 99 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 45 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 47 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 49 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 61 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 66 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 12 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 14 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 16 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 31 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 43 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 42 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 87 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 139 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 173 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 224 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 237 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 268 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 289 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 290 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 40 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 42 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 101 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 118 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 130 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 133 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 137 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 157 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 175 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 179 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 212 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 222 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 228 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 7 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 9 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 32 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 54 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 9 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 11 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 8 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 10 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 62 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 96 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 118 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 119 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 121 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 397 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 137 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 214 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 233 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.test.ts | 6 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.test.ts | 32 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.test.ts | 55 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.test.ts | 76 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.test.ts | 93 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.test.ts | 123 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | widgets.ts | 24 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | widgets.test.ts | 52 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.ts | 4 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.ts | 16 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.ts | 31 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | forms.ts | 48 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 67 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 84 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 93 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 109 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 115 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 122 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 149 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 151 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 156 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 225 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.tsx | 249 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | configuration.test.ts | 67 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.test.tsx | 207 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.test.tsx | 212 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.test.tsx | 217 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.test.tsx | 218 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.test.tsx | 284 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.test.tsx | 294 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | transform.test.tsx | 314 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | configuration.ts | 68 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | configuration.ts | 110 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | configuration.ts | 117 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | configuration.ts | 125 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | configuration.ts | 199 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 136 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 140 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 160 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 164 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 26 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 35 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 235 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 269 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 307 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 348 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 396 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 423 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 424 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 425 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 498 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 77 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 98 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 130 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 124 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 155 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 202 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 279 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 365 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 412 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 424 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 425 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 469 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 101 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 128 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 166 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 199 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 206 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 351 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 163 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.test.tsx | 177 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 46 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 58 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 59 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useIsMobile.test.ts | 36 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 25 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 27 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 29 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 31 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 33 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 34 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 67 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 74 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 93 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 132 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.tsx | 156 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 86 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 142 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 206 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 216 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 217 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 218 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 277 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 290 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableColumns.test.tsx | 309 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableQuery.ts | 17 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableQuery.ts | 18 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableQuery.ts | 25 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableQuery.ts | 60 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableQuery.ts | 61 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | useTableQuery.ts | 62 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | provider.tsx | 29 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | service.py | 394 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | service.py | 416 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | service.py | 417 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | service.py | 419 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | service.py | 421 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | service.py | 430 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | service.py | 431 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 252 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 253 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 277 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 247 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 248 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 269 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 9 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 304 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 326 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | urls.py | 21 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | urls.py | 39 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | base.py | 642 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | django.py | 312 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | yaraorm.py | 301 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tortoise.py | 323 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | index.min.js | 121 | Match: `,df=e=>{let{csp:t,prefixCls:n,layer:r,zeroRuntime:i} |
| HIGH | GS000-LEGACY | index.min.js | 313 | Match:           }`)}});K();var abe=[`id`,`prefixCls`,`class |
| HIGH | GS000-LEGACY | index.min.js | 387 | Match: Please change the parent <Route path="${e}"> to <Rout |
| HIGH | GS000-LEGACY | index.min.js | 395 | Match: `+n)}}catch(e){}}throw e}})()}_request(e,t){typeof e= |
| HIGH | GS000-LEGACY | Makefile | 46 | Match: 	@exec yarn run dev --host 0.0.0.0 --port 3030 |
| HIGH | GS025 | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS007 | api.py | 247 | Line 247: @router.post("/upload-file/{model}/{field_name}") |
| HIGH | GS019 | base.py | 814 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | ? | index.min.js | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 218 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 298 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 395 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 397 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 530 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 532 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 577 | Clone in performance-critical code — consider references |
| HIGH | ? | index.min.js | 586 | Clone in performance-critical code — consider references |
| HIGH | ? | worker-C151k0-L.js | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | worker-MF2p-l5_.js | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | worker-C9KPOOKD.js | 9 | Clone in performance-critical code — consider references |
| HIGH | ? | worker-DRNcaZ-V.js | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | worker-D1fCgYB7.js | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | worker-6Z7niv9l.js | 13 | Clone in performance-critical code — consider references |
| HIGH | ? | worker-D3TWcJOI.js | 13 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | index.min.js | 9 |
| C | GS005 | index.min.js | 395 |
| H | GS000-LEGACY | index.test.tsx | 65 |
| H | GS000-LEGACY | index.test.tsx | 66 |
| H | GS000-LEGACY | index.test.tsx | 182 |
| H | GS000-LEGACY | index.test.tsx | 234 |
| H | GS000-LEGACY | index.test.tsx | 315 |
| H | GS000-LEGACY | index.test.tsx | 354 |
| H | GS000-LEGACY | index.test.tsx | 433 |
| H | GS000-LEGACY | index.test.tsx | 454 |
| H | GS000-LEGACY | index.test.tsx | 455 |
| H | GS000-LEGACY | index.test.tsx | 500 |
| H | GS000-LEGACY | index.tsx | 112 |
| H | GS000-LEGACY | index.tsx | 164 |
| H | GS000-LEGACY | index.tsx | 180 |
| H | GS000-LEGACY | index.tsx | 205 |
| H | GS000-LEGACY | index.tsx | 231 |
| H | GS000-LEGACY | index.tsx | 266 |
| H | GS000-LEGACY | index.tsx | 297 |
| H | GS000-LEGACY | index.tsx | 304 |
| H | GS000-LEGACY | index.tsx | 312 |
| H | GS000-LEGACY | index.tsx | 316 |
| H | GS000-LEGACY | index.tsx | 477 |
| H | GS000-LEGACY | index.test.tsx | 23 |
| H | GS000-LEGACY | index.test.tsx | 110 |
| H | GS000-LEGACY | index.test.tsx | 114 |
| H | GS000-LEGACY | index.test.tsx | 122 |
| H | GS000-LEGACY | index.test.tsx | 153 |
| H | GS000-LEGACY | index.test.tsx | 176 |
| H | GS000-LEGACY | index.test.tsx | 215 |
| H | GS000-LEGACY | index.test.tsx | 276 |
| H | GS000-LEGACY | index.test.tsx | 288 |
| H | GS000-LEGACY | index.test.tsx | 294 |
| H | GS000-LEGACY | index.test.tsx | 305 |
| H | GS000-LEGACY | index.tsx | 100 |
| H | GS000-LEGACY | index.tsx | 111 |
| H | GS000-LEGACY | index.tsx | 251 |
| H | GS000-LEGACY | index.tsx | 310 |
| H | GS000-LEGACY | index.tsx | 374 |
| H | GS000-LEGACY | index.tsx | 451 |
| H | GS000-LEGACY | index.tsx | 34 |
| H | GS000-LEGACY | index.tsx | 36 |
| H | GS000-LEGACY | index.tsx | 38 |
| H | GS000-LEGACY | index.tsx | 45 |
| H | GS000-LEGACY | index.tsx | 46 |
| H | GS000-LEGACY | index.tsx | 54 |
| H | GS000-LEGACY | index.tsx | 60 |
| H | GS000-LEGACY | index.tsx | 95 |
| H | GS000-LEGACY | index.tsx | 111 |
| H | GS000-LEGACY | index.tsx | 112 |
| H | GS000-LEGACY | index.tsx | 113 |
| H | GS000-LEGACY | index.tsx | 114 |
| H | GS000-LEGACY | index.tsx | 115 |
| H | GS000-LEGACY | index.tsx | 116 |
| H | GS000-LEGACY | index.tsx | 120 |
| H | GS000-LEGACY | index.test.tsx | 110 |
| H | GS000-LEGACY | index.test.tsx | 201 |
| H | GS000-LEGACY | index.test.tsx | 235 |
| H | GS000-LEGACY | index.tsx | 24 |
| H | GS000-LEGACY | index.tsx | 26 |
| H | GS000-LEGACY | index.tsx | 80 |
| H | GS000-LEGACY | index.tsx | 156 |
| H | GS000-LEGACY | index.tsx | 172 |
| H | GS000-LEGACY | index.tsx | 185 |
| H | GS000-LEGACY | index.tsx | 234 |
| H | GS000-LEGACY | index.test.tsx | 152 |
| H | GS000-LEGACY | index.test.tsx | 153 |
| H | GS000-LEGACY | index.tsx | 30 |
| H | GS000-LEGACY | index.tsx | 32 |
| H | GS000-LEGACY | index.tsx | 54 |
| H | GS000-LEGACY | index.tsx | 75 |
| H | GS000-LEGACY | index.tsx | 7 |
| H | GS000-LEGACY | index.tsx | 9 |
| H | GS000-LEGACY | index.test.tsx | 159 |
| H | GS000-LEGACY | index.test.tsx | 160 |
| H | GS000-LEGACY | index.tsx | 42 |
| H | GS000-LEGACY | index.tsx | 53 |
| H | GS000-LEGACY | index.test.tsx | 237 |
| H | GS000-LEGACY | index.test.tsx | 297 |
| H | GS000-LEGACY | index.tsx | 44 |
| H | GS000-LEGACY | index.tsx | 69 |
| H | GS000-LEGACY | index.tsx | 140 |
| H | GS000-LEGACY | index.tsx | 141 |
| H | GS000-LEGACY | index.tsx | 143 |
| H | GS000-LEGACY | index.tsx | 145 |
| H | GS000-LEGACY | index.tsx | 303 |
| H | GS000-LEGACY | index.test.tsx | 9 |
| H | GS000-LEGACY | index.test.tsx | 13 |
| H | GS000-LEGACY | index.test.tsx | 23 |
| H | GS000-LEGACY | index.test.tsx | 35 |
| H | GS000-LEGACY | index.test.tsx | 90 |
| H | GS000-LEGACY | index.test.tsx | 99 |
| H | GS000-LEGACY | index.tsx | 19 |
| H | GS000-LEGACY | index.tsx | 45 |
| H | GS000-LEGACY | index.tsx | 47 |
| H | GS000-LEGACY | index.tsx | 49 |
| H | GS000-LEGACY | index.tsx | 61 |
| H | GS000-LEGACY | index.tsx | 66 |
| H | GS000-LEGACY | index.tsx | 12 |
| H | GS000-LEGACY | index.tsx | 14 |
| H | GS000-LEGACY | index.tsx | 16 |
| H | GS000-LEGACY | index.tsx | 31 |
| H | GS000-LEGACY | index.tsx | 43 |
| H | GS000-LEGACY | index.test.tsx | 42 |
| H | GS000-LEGACY | index.test.tsx | 87 |
| H | GS000-LEGACY | index.test.tsx | 139 |
| H | GS000-LEGACY | index.test.tsx | 173 |
| H | GS000-LEGACY | index.test.tsx | 224 |
| H | GS000-LEGACY | index.test.tsx | 237 |
| H | GS000-LEGACY | index.test.tsx | 268 |
| H | GS000-LEGACY | index.test.tsx | 289 |
| H | GS000-LEGACY | index.test.tsx | 290 |
| H | GS000-LEGACY | index.tsx | 40 |
| H | GS000-LEGACY | index.tsx | 42 |
| H | GS000-LEGACY | index.tsx | 101 |
| H | GS000-LEGACY | index.tsx | 118 |
| H | GS000-LEGACY | index.tsx | 130 |
| H | GS000-LEGACY | index.tsx | 133 |
| H | GS000-LEGACY | index.tsx | 137 |
| H | GS000-LEGACY | index.tsx | 157 |
| H | GS000-LEGACY | index.tsx | 175 |
| H | GS000-LEGACY | index.tsx | 179 |
| H | GS000-LEGACY | index.tsx | 212 |
| H | GS000-LEGACY | index.tsx | 222 |
| H | GS000-LEGACY | index.tsx | 228 |
| H | GS000-LEGACY | index.tsx | 7 |
| H | GS000-LEGACY | index.tsx | 9 |
| H | GS000-LEGACY | index.test.tsx | 32 |
| H | GS000-LEGACY | index.test.tsx | 54 |
| H | GS000-LEGACY | index.tsx | 9 |
| H | GS000-LEGACY | index.tsx | 11 |
| H | GS000-LEGACY | index.tsx | 8 |
| H | GS000-LEGACY | index.tsx | 10 |
| H | GS000-LEGACY | index.tsx | 62 |
| H | GS000-LEGACY | index.tsx | 96 |
| H | GS000-LEGACY | index.tsx | 118 |
| H | GS000-LEGACY | index.tsx | 119 |
| H | GS000-LEGACY | index.tsx | 121 |
| H | GS000-LEGACY | index.tsx | 397 |
| H | GS000-LEGACY | index.test.tsx | 137 |
| H | GS000-LEGACY | index.test.tsx | 214 |
| H | GS000-LEGACY | index.test.tsx | 233 |
| H | GS000-LEGACY | forms.test.ts | 6 |
| H | GS000-LEGACY | forms.test.ts | 32 |
| H | GS000-LEGACY | forms.test.ts | 55 |
| H | GS000-LEGACY | forms.test.ts | 76 |
| H | GS000-LEGACY | forms.test.ts | 93 |
| H | GS000-LEGACY | forms.test.ts | 123 |
| H | GS000-LEGACY | widgets.ts | 24 |
| H | GS000-LEGACY | widgets.test.ts | 52 |
| H | GS000-LEGACY | forms.ts | 4 |
| H | GS000-LEGACY | forms.ts | 16 |
| H | GS000-LEGACY | forms.ts | 31 |
| H | GS000-LEGACY | forms.ts | 48 |
| H | GS000-LEGACY | transform.tsx | 67 |
| H | GS000-LEGACY | transform.tsx | 84 |
| H | GS000-LEGACY | transform.tsx | 93 |
| H | GS000-LEGACY | transform.tsx | 109 |
| H | GS000-LEGACY | transform.tsx | 115 |
| H | GS000-LEGACY | transform.tsx | 122 |
| H | GS000-LEGACY | transform.tsx | 149 |
| H | GS000-LEGACY | transform.tsx | 151 |
| H | GS000-LEGACY | transform.tsx | 156 |
| H | GS000-LEGACY | transform.tsx | 225 |
| H | GS000-LEGACY | transform.tsx | 249 |
| H | GS000-LEGACY | configuration.test.ts | 67 |
| H | GS000-LEGACY | transform.test.tsx | 207 |
| H | GS000-LEGACY | transform.test.tsx | 212 |
| H | GS000-LEGACY | transform.test.tsx | 217 |
| H | GS000-LEGACY | transform.test.tsx | 218 |
| H | GS000-LEGACY | transform.test.tsx | 284 |
| H | GS000-LEGACY | transform.test.tsx | 294 |
| H | GS000-LEGACY | transform.test.tsx | 314 |
| H | GS000-LEGACY | configuration.ts | 68 |
| H | GS000-LEGACY | configuration.ts | 110 |
| H | GS000-LEGACY | configuration.ts | 117 |
| H | GS000-LEGACY | configuration.ts | 125 |
| H | GS000-LEGACY | configuration.ts | 199 |
| H | GS000-LEGACY | index.test.tsx | 136 |
| H | GS000-LEGACY | index.test.tsx | 140 |
| H | GS000-LEGACY | index.test.tsx | 160 |
| H | GS000-LEGACY | index.test.tsx | 164 |
| H | GS000-LEGACY | index.tsx | 26 |
| H | GS000-LEGACY | index.tsx | 35 |
| H | GS000-LEGACY | index.test.tsx | 235 |
| H | GS000-LEGACY | index.test.tsx | 269 |
| H | GS000-LEGACY | index.test.tsx | 307 |
| H | GS000-LEGACY | index.test.tsx | 348 |
| H | GS000-LEGACY | index.test.tsx | 396 |
| H | GS000-LEGACY | index.test.tsx | 423 |
| H | GS000-LEGACY | index.test.tsx | 424 |
| H | GS000-LEGACY | index.test.tsx | 425 |
| H | GS000-LEGACY | index.test.tsx | 498 |
| H | GS000-LEGACY | index.tsx | 77 |
| H | GS000-LEGACY | index.tsx | 98 |
| H | GS000-LEGACY | index.tsx | 130 |
| H | GS000-LEGACY | index.test.tsx | 124 |
| H | GS000-LEGACY | index.test.tsx | 155 |
| H | GS000-LEGACY | index.test.tsx | 202 |
| H | GS000-LEGACY | index.test.tsx | 279 |
| H | GS000-LEGACY | index.test.tsx | 365 |
| H | GS000-LEGACY | index.test.tsx | 412 |
| H | GS000-LEGACY | index.test.tsx | 424 |
| H | GS000-LEGACY | index.test.tsx | 425 |
| H | GS000-LEGACY | index.test.tsx | 469 |
| H | GS000-LEGACY | index.tsx | 101 |
| H | GS000-LEGACY | index.tsx | 128 |
| H | GS000-LEGACY | index.tsx | 166 |
| H | GS000-LEGACY | index.tsx | 199 |
| H | GS000-LEGACY | index.tsx | 206 |
| H | GS000-LEGACY | index.tsx | 351 |
| H | GS000-LEGACY | index.test.tsx | 163 |
| H | GS000-LEGACY | index.test.tsx | 177 |
| H | GS000-LEGACY | index.tsx | 46 |
| H | GS000-LEGACY | index.tsx | 58 |
| H | GS000-LEGACY | index.tsx | 59 |
| H | GS000-LEGACY | useIsMobile.test.ts | 36 |
| H | GS000-LEGACY | useTableColumns.tsx | 25 |
| H | GS000-LEGACY | useTableColumns.tsx | 27 |
| H | GS000-LEGACY | useTableColumns.tsx | 29 |
| H | GS000-LEGACY | useTableColumns.tsx | 31 |
| H | GS000-LEGACY | useTableColumns.tsx | 33 |
| H | GS000-LEGACY | useTableColumns.tsx | 34 |
| H | GS000-LEGACY | useTableColumns.tsx | 67 |
| H | GS000-LEGACY | useTableColumns.tsx | 74 |
| H | GS000-LEGACY | useTableColumns.tsx | 93 |
| H | GS000-LEGACY | useTableColumns.tsx | 132 |
| H | GS000-LEGACY | useTableColumns.tsx | 156 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 86 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 142 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 206 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 216 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 217 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 218 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 277 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 290 |
| H | GS000-LEGACY | useTableColumns.test.tsx | 309 |
| H | GS000-LEGACY | useTableQuery.ts | 17 |
| H | GS000-LEGACY | useTableQuery.ts | 18 |
| H | GS000-LEGACY | useTableQuery.ts | 25 |
| H | GS000-LEGACY | useTableQuery.ts | 60 |
| H | GS000-LEGACY | useTableQuery.ts | 61 |
| H | GS000-LEGACY | useTableQuery.ts | 62 |
| H | GS000-LEGACY | provider.tsx | 29 |
| H | GS000-LEGACY | service.py | 394 |
| H | GS000-LEGACY | service.py | 416 |
| H | GS000-LEGACY | service.py | 417 |
| H | GS000-LEGACY | service.py | 419 |
| H | GS000-LEGACY | service.py | 421 |
| H | GS000-LEGACY | service.py | 430 |
| H | GS000-LEGACY | service.py | 431 |
| H | GS000-LEGACY | api.py | 252 |
| H | GS000-LEGACY | api.py | 253 |
| H | GS000-LEGACY | api.py | 277 |
| H | GS000-LEGACY | api.py | 247 |
| H | GS000-LEGACY | api.py | 248 |
| H | GS000-LEGACY | api.py | 269 |
| H | GS000-LEGACY | api.py | 9 |
| H | GS000-LEGACY | api.py | 304 |
| H | GS000-LEGACY | api.py | 326 |
| H | GS000-LEGACY | urls.py | 21 |
| H | GS000-LEGACY | urls.py | 39 |
| H | GS000-LEGACY | base.py | 642 |
| H | GS000-LEGACY | django.py | 312 |
| H | GS000-LEGACY | yaraorm.py | 301 |
| H | GS000-LEGACY | tortoise.py | 323 |
| M | GS025 | yaraorm.py | 47 |
| M | GS025 | yaraorm.py | 200 |
| C | GS001 | service.py | 68 |
| C | GS001 | service.py | 198 |
| C | GS001 | tsconfig.json | 6 |
| C | GS001 | tsconfig.json | 8 |
| C | GS001 | vite.config.ts | 46 |
| C | GS001 | pyproject.toml | 93 |
| C | GS001 | pyproject.toml | 139 |
| L | GS003 | worker-6Z7niv9l.js | 13 |
| L | GS003 | worker-C151k0-L.js | 13 |
| L | GS003 | worker-C9KPOOKD.js | 9 |
| L | GS003 | worker-D1fCgYB7.js | 13 |
| L | GS003 | worker-D3TWcJOI.js | 13 |
| L | GS003 | worker-DRNcaZ-V.js | 13 |
| L | GS003 | worker-MF2p-l5_.js | 13 |
| L | GS003 | index.min.js | 524 |
| L | GS003 | index.min.js | 577 |
| L | GS003 | index.min.js | 590 |
| L | GS003 | index.min.js | 592 |
| L | GS003 | index.min.js | 520 |
| L | GS003 | index.min.js | 520 |
| L | GS003 | index.min.js | 524 |
| L | GS003 | index.min.js | 524 |
| I | GS015 | urls.py | 1 |
| I | GS015 | app.py | 13 |
| I | GS015 | app.py | 22 |
| i | GS020 |  | 8 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 67 |
| i | GS020 |  | 67 |
| i | GS020 |  | 408 |
| i | GS020 |  | 419 |
| i | GS020 |  | 435 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 438 |
| i | GS020 |  | 518 |
| i | GS020 |  | 518 |
| i | GS020 |  | 520 |
| i | GS020 |  | 520 |
| i | GS020 |  | 520 |
| i | GS020 |  | 524 |
| i | GS020 |  | 524 |
| i | GS020 |  | 524 |
| i | GS020 |  | 524 |
| i | GS020 |  | 524 |
| i | GS020 |  | 524 |
| i | GS020 |  | 530 |
| i | GS020 |  | 530 |
| i | GS020 |  | 530 |
| i | GS020 |  | 577 |
| i | GS020 |  | 593 |
| i | GS020 |  | 649 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 387 |
| i | GS020 |  | 8 |
| i | GS020 |  | 9 |
| i | GS020 |  | 435 |
| i | GS020 |  | 438 |
| i | GS020 |  | 518 |
| i | GS020 |  | 520 |
| i | GS020 |  | 524 |
| i | GS020 |  | 530 |
| i | GS020 |  | 577 |
| i | GS020 |  | 649 |
| i | GS020 |  | 385 |
| i | GS020 |  | 387 |
| i | GS020 |  | 432 |
| i | GS020 |  | 432 |
| i | GS020 |  | 524 |
| i | GS020 |  | 524 |
| i | GS020 |  | 395 |
| i | GS020 |  | 395 |
| i | GS020 |  | 518 |
| i | GS020 |  | 49 |
| i | GS020 |  | 10 |
| i | GS020 |  | 10 |
| i | GS020 |  | 13 |
| i | GS020 |  | 112 |
| i | GS020 |  | 19 |
| i | GS020 |  | 19 |
| ? | GS032-exfil_env_send | index.min.js | 395 |
| ? | GS034-token_collector | index.min.js | 150 |
| ? | GS036-redos | index.min.js | 395 |
| ? | GS036-redos | index.min.js | 519 |
| ? | GS036-redos | index.min.js | 524 |
| H | GS000-LEGACY | index.min.js | 121 |
| H | GS000-LEGACY | index.min.js | 313 |
| H | GS000-LEGACY | index.min.js | 387 |
| H | GS000-LEGACY | index.min.js | 395 |
| H | GS000-LEGACY | Makefile | 46 |
| C | GS029 | index.min.js | 250 |
| M | GS000-LEGACY | usePageMeta.test.tsx | 10 |
| M | GS000-LEGACY | usePageMeta.test.tsx | 15 |
| H | GS025 | mkdocs.yml | 0 |
| H | GS007 | api.py | 247 |
| s | GS009 |  | 0 |
| L | GS011 | service.py | 68 |
| M | GS019 | api.py | 252 |
| M | GS019 | api.py | 198 |
| M | GS019 | api.py | 198 |
| M | GS019 | service.py | 321 |
| H | GS019 | base.py | 814 |
| M | GS019 | base.py | 823 |
| c | GS021 |  | 77 |
| c | GS021 |  | 109 |
| c | GS021 |  | 130 |
| c | GS021 |  | 157 |
| c | GS021 |  | 204 |
| c | GS021 |  | 229 |
| c | GS021 |  | 251 |
| c | GS021 |  | 276 |
| c | GS021 |  | 303 |
| c | GS021 |  | 340 |
| c | GS021 |  | 379 |
| c | GS021 |  | 408 |
| c | GS021 |  | 442 |
| c | GS021 |  | 471 |
| s | GS021 |  | 7 |
| s | GS021 |  | 8 |
| s | GS021 |  | 467 |
| s | GS021 |  | 467 |
| s | GS021 |  | 152 |
| s | GS021 |  | 152 |
| s | GS021 |  | 458 |
| s | GS021 |  | 458 |
| s | GS021 |  | 464 |
| s | GS021 |  | 464 |
| s | GS021 |  | 464 |
| s | GS021 |  | 544 |
| s | GS021 |  | 544 |
| s | GS021 |  | 32 |
| s | GS021 |  | 33 |
| s | GS021 |  | 365 |
| s | GS021 |  | 385 |
| s | GS021 |  | 389 |
| s | GS021 |  | 524 |
| s | GS021 |  | 150 |
| s | GS021 |  | 385 |
| s | GS021 |  | 389 |
| r | GS022 |  | 468 |
| r | GS022 |  | 49 |
| r | GS022 |  | 50 |
| r | GS022 |  | 78 |
| r | GS022 |  | 82 |
| r | GS022 |  | 120 |
| r | GS022 |  | 449 |
| r | GS022 |  | 610 |
| r | GS022 |  | 626 |
| r | GS022 |  | 629 |
| r | GS022 |  | 8 |
| r | GS022 |  | 387 |
| r | GS022 |  | 150 |
| r | GS022 |  | 298 |
| r | GS022 |  | 310 |
| r | GS022 |  | 313 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 387 |
| r | GS022 |  | 387 |
| r | GS022 |  | 387 |
| r | GS022 |  | 389 |
| r | GS022 |  | 389 |
| r | GS022 |  | 389 |
| r | GS022 |  | 395 |
| r | GS022 |  | 395 |
| r | GS022 |  | 395 |
| r | GS022 |  | 395 |
| r | GS022 |  | 432 |
| r | GS022 |  | 518 |
| r | GS022 |  | 518 |
| r | GS022 |  | 518 |
| r | GS022 |  | 520 |
| r | GS022 |  | 520 |
| r | GS022 |  | 520 |
| r | GS022 |  | 520 |
| r | GS022 |  | 524 |
| r | GS022 |  | 524 |
| r | GS022 |  | 549 |
| r | GS022 |  | 649 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-insecure_random |  | ? |
| M | ? | index.min.js | 310 |
| H | ? | index.min.js | 35 |
| H | ? | index.min.js | 143 |
| H | ? | index.min.js | 218 |
| H | ? | index.min.js | 298 |
| H | ? | index.min.js | 350 |
| H | ? | index.min.js | 395 |
| H | ? | index.min.js | 397 |
| H | ? | index.min.js | 530 |
| H | ? | index.min.js | 532 |
| H | ? | index.min.js | 549 |
| H | ? | index.min.js | 577 |
| H | ? | index.min.js | 586 |
| H | ? | worker-C151k0-L.js | 13 |
| H | ? | worker-MF2p-l5_.js | 13 |
| H | ? | worker-C9KPOOKD.js | 9 |
| H | ? | worker-DRNcaZ-V.js | 13 |
| H | ? | worker-D1fCgYB7.js | 13 |
| H | ? | worker-6Z7niv9l.js | 13 |
| H | ? | worker-D3TWcJOI.js | 13 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T19:18:41.474701*