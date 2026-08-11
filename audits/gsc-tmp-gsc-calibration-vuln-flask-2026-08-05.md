---
title: "GSC Audit: /tmp/gsc-calibration/vuln-flask"
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/vuln-flask

**Дата:** 05.08.2026 07:47  
**Путь:** `/tmp/gsc-calibration/vuln-flask`  
**Всего находок:** 74  
**CRITICAL:** 5 | **HIGH:** 5 | **MEDIUM:** 3 | **LOW:** 6

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 31 |
| GS021 | 12 |
| GS020 | 9 |
| GS003 | 4 |
| GS011 | 4 |
| CVE-2026-37270: Hardcoded credential | 2 |
| GS001 | 2 |
| GS019 | 2 |
| GS022 | 2 |
| Rust: .clone() in hot path | 2 |
| JWT: verify=False | 1 |
| CVE-2026-56219: Authentication bypass | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | app.py | 97 | Hacking APIs (No Starch Press) |
| CRITICAL | GS001 | app.py | 63 | Found: password = 'admin123' |
| CRITICAL | GS001 | app.py | 86 | Found: 'HS256' |
| CRITICAL | GS011 | app.py | 86 | Detected: jwt.decode(token, app.config['SECRET_KEY_HMAC'], v |
| CRITICAL | GS019 | app.py | 28 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | ? | app.py | 97 |  |
| HIGH | GS011 | app.py | 28 | Found JWT secret in code: 'F12Zr47j...'. JWT secrets must be |
| HIGH | GS019 | app.py | 171 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | ? | loader.js | 30 | Clone in performance-critical code — consider references |
| HIGH | ? | loader.js | 109 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | app.py | 97 |
| H | ? | app.py | 97 |
| M | ? | app.py | 63 |
| M | ? | app.py | 28 |
| M | ? | app.py | 63 |
| C | GS001 | app.py | 63 |
| C | GS001 | app.py | 86 |
| L | GS003 | app.py | 87 |
| L | GS003 | app.py | 90 |
| L | GS003 | app.py | 93 |
| L | GS003 | app.py | 98 |
| I | GS015 | app.py | 121 |
| I | GS015 | app.py | 134 |
| I | GS015 | app.py | 150 |
| I | GS015 | app.py | 170 |
| I | GS015 | app.py | 196 |
| I | GS015 | app.py | 221 |
| I | GS015 | app.py | 246 |
| I | GS015 | app.py | 284 |
| I | GS015 | app.py | 290 |
| I | GS015 | app.py | 310 |
| I | GS015 | app.py | 121 |
| I | GS015 | app.py | 134 |
| I | GS015 | app.py | 150 |
| I | GS015 | app.py | 170 |
| I | GS015 | app.py | 196 |
| I | GS015 | app.py | 221 |
| I | GS015 | app.py | 246 |
| I | GS015 | app.py | 284 |
| I | GS015 | app.py | 290 |
| I | GS015 | app.py | 310 |
| I | GS015 | app.py | 121 |
| I | GS015 | app.py | 134 |
| I | GS015 | app.py | 150 |
| I | GS015 | app.py | 170 |
| I | GS015 | app.py | 196 |
| I | GS015 | app.py | 221 |
| I | GS015 | app.py | 246 |
| I | GS015 | app.py | 284 |
| I | GS015 | app.py | 290 |
| I | GS015 | app.py | 310 |
| I | GS015 | app.py | 24 |
| i | GS020 |  | 50 |
| i | GS020 |  | 153 |
| i | GS020 |  | 153 |
| i | GS020 |  | 20 |
| i | GS020 |  | 153 |
| i | GS020 |  | 23 |
| i | GS020 |  | 33 |
| i | GS020 |  | 114 |
| i | GS020 |  | 281 |
| s | GS009 |  | 0 |
| H | GS011 | app.py | 28 |
| C | GS011 | app.py | 86 |
| L | GS011 | app.py | 86 |
| L | GS011 | app.py | 97 |
| H | GS019 | app.py | 171 |
| C | GS019 | app.py | 28 |
| s | GS021 |  | 9 |
| s | GS021 |  | 11 |
| s | GS021 |  | 12 |
| s | GS021 |  | 54 |
| s | GS021 |  | 55 |
| c | GS021 |  | 134 |
| c | GS021 |  | 150 |
| c | GS021 |  | 170 |
| c | GS021 |  | 196 |
| c | GS021 |  | 246 |
| c | GS021 |  | 290 |
| c | GS021 |  | 315 |
| r | GS022 |  | 133 |
| r | GS022 |  | 133 |
| H | ? | loader.js | 30 |
| H | ? | loader.js | 109 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T07:47:07.611177*