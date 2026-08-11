---
title: "GSC Audit: /tmp/gsc-learn/pyramid"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pyramid

**Дата:** 07.08.2026 04:06  
**Путь:** `/tmp/gsc-learn/pyramid`  
**Всего находок:** 536  
**CRITICAL:** 11 | **HIGH:** 9 | **MEDIUM:** 19 | **LOW:** 493

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 13 |
| Хардкод IP адреса | 9 |
| Generic code smell #24 | 8 |
| Generic code smell #27 | 8 |
| Generic code smell #30 | 8 |
| Generic code smell #33 | 8 |
| Generic code smell #36 | 8 |
| Generic code smell #39 | 8 |
| Generic code smell #42 | 8 |
| Generic code smell #45 | 8 |
| Generic code smell #48 | 8 |
| Generic code smell #51 | 8 |
| Generic code smell #54 | 8 |
| Generic code smell #57 | 8 |
| Generic code smell #60 | 8 |
| Generic code smell #63 | 8 |
| Generic code smell #66 | 8 |
| Generic code smell #69 | 8 |
| Generic code smell #72 | 8 |
| Generic code smell #75 | 8 |
| Generic code smell #78 | 8 |
| Generic code smell #81 | 8 |
| Generic code smell #84 | 8 |
| Generic code smell #87 | 8 |
| Generic code smell #90 | 8 |
| Generic code smell #93 | 8 |
| Generic code smell #96 | 8 |
| Generic code smell #99 | 8 |
| Generic code smell #102 | 8 |
| Generic code smell #105 | 8 |
| Generic code smell #108 | 8 |
| Generic code smell #111 | 8 |
| Generic code smell #114 | 8 |
| Generic code smell #117 | 8 |
| Generic code smell #120 | 8 |
| Generic code smell #123 | 8 |
| Generic code smell #126 | 8 |
| Generic code smell #129 | 8 |
| Generic code smell #132 | 8 |
| Generic code smell #135 | 8 |
| Generic code smell #138 | 8 |
| Generic code smell #141 | 8 |
| Generic code smell #144 | 8 |
| Generic code smell #147 | 8 |
| Generic code smell #150 | 8 |
| Generic code smell #153 | 8 |
| Generic code smell #156 | 8 |
| Generic code smell #159 | 8 |
| Generic code smell #162 | 8 |
| Generic code smell #165 | 8 |
| Generic code smell #168 | 8 |
| Generic code smell #171 | 8 |
| Generic code smell #174 | 8 |
| Generic code smell #177 | 8 |
| Generic code smell #180 | 8 |
| Generic code smell #183 | 8 |
| Generic code smell #186 | 8 |
| Generic code smell #189 | 8 |
| Generic code smell #192 | 8 |
| Generic code smell #195 | 8 |
| Generic code smell #198 | 8 |
| CVE-2026-37270: Hardcoded credential | 8 |
| GS008 | 8 |
| CVE-2026-56318: Information disclosure | 6 |
| GS001 | 6 |
| Hardcoded encryption key | 5 |
| Python: assert in production | 4 |
| GS020 | 2 |
| CVE-2026-55223: Insecure deserialization | 1 |
| GS015 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | pyproject.toml | 106 | Found: 'py310' |
| CRITICAL | GS001 | pyproject.toml | 106 | Found: 'py311' |
| CRITICAL | GS001 | pyproject.toml | 106 | Found: 'py312' |
| CRITICAL | GS001 | pyproject.toml | 106 | Found: 'py313' |
| CRITICAL | GS001 | pyproject.toml | 106 | Found: 'py314' |
| CRITICAL | GS001 | testing.py | 261 | Found: token = '0123456789012345678901234567890123456789' |
| CRITICAL | ? | viewderivers.py | 486 | Match:         token = 'csrf_token' |
| CRITICAL | ? | testing.py | 261 | Match:         token = '012345678901234567890123456789012345 |
| CRITICAL | ? | authentication.py | 408 | Match:     def __init__(self, environ_key='REMOTE_USER', cal |
| CRITICAL | ? | csrf.py | 194 | Match:     request, token='csrf_token', header='X-CSRF-Token |
| CRITICAL | ? | security.py | 261 | Match:         token='csrf_token', |
| HIGH | ? | authentication.py | 1060 | Match:             remote_addr = '0.0.0.0' |
| HIGH | ? | authentication.py | 1148 | Match:             remote_addr = '0.0.0.0' |
| HIGH | ? | pserve.py | 178 | Match:             return 'http://127.0.0.1:{port}'.format(* |
| HIGH | ? | pserve.py | 297 | Match:     host = kw.get('host', '0.0.0.0') |
| HIGH | ? | pserve.py | 308 | Match:     host='127.0.0.1', |
| HIGH | ? | pserve.py | 332 | Match:         127.0.0.1, which is not a public interface. |
| HIGH | ? | pserve.py | 417 | Match:         if host == '0.0.0.0': |
| HIGH | ? | pserve.py | 419 | Match:                 'serving on 0.0.0.0:%s view at %s://1 |
| HIGH | ? | prequest.py | 184 | Match:             'REMOTE_ADDR': '127.0.0.1', |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| L | ? | viewderivers.py | 337 |
| L | ? | session.py | 264 |
| L | ? | views.py | 1092 |
| L | ? | predicates.py | 151 |
| L | ? | security.py | 139 |
| L | ? | httpexceptions.py | 481 |
| L | ? | httpexceptions.py | 614 |
| L | ? | static.py | 193 |
| M | ? | testing.py | 118 |
| M | ? | actions.py | 74 |
| M | ? | registry.py | 228 |
| M | ? | pserve.py | 202 |
| M | ? | session.py | 70 |
| M | ? | viewderivers.py | 486 |
| M | ? | testing.py | 261 |
| M | ? | csrf.py | 194 |
| M | ? | csrf.py | 229 |
| M | ? | security.py | 261 |
| M | ? | security.py | 35 |
| M | ? | viewderivers.py | 486 |
| M | ? | testing.py | 261 |
| M | ? | authentication.py | 408 |
| M | ? | csrf.py | 70 |
| M | ? | csrf.py | 194 |
| M | ? | csrf.py | 229 |
| M | ? | security.py | 261 |
| M | ? | security.py | 35 |
| C | GS001 | pyproject.toml | 106 |
| C | GS001 | pyproject.toml | 106 |
| C | GS001 | pyproject.toml | 106 |
| C | GS001 | pyproject.toml | 106 |
| C | GS001 | pyproject.toml | 106 |
| C | GS001 | testing.py | 261 |
| L | GS003 | events.py | 41 |
| L | GS003 | events.py | 52 |
| L | GS003 | events.py | 287 |
| L | GS003 | path.py | 195 |
| L | GS003 | prequest.py | 132 |
| L | GS003 | proutes.py | 305 |
| L | GS003 | pserve.py | 146 |
| L | GS003 | pserve.py | 300 |
| L | GS003 | pserve.py | 418 |
| L | GS003 | pserve.py | 424 |
| L | GS003 | pshell.py | 123 |
| L | GS003 | ptweens.py | 68 |
| L | GS003 | pviews.py | 69 |
| L | GS008 | authorization.py | 46 |
| L | GS008 | predicates.py | 11 |
| L | GS008 | interfaces.py | 1644 |
| L | GS008 | interfaces.py | 1645 |
| L | GS008 | interfaces.py | 1646 |
| L | GS008 | interfaces.py | 1647 |
| L | GS008 | security.py | 14 |
| L | GS008 | tweens.py | 51 |
| I | GS015 | wsgi.py | 1 |
| i | GS020 |  | 17 |
| i | GS020 |  | 14 |
| H | ? | authentication.py | 1060 |
| H | ? | authentication.py | 1148 |
| H | ? | pserve.py | 178 |
| H | ? | pserve.py | 297 |
| H | ? | pserve.py | 308 |
| H | ? | pserve.py | 332 |
| H | ? | pserve.py | 417 |
| H | ? | pserve.py | 419 |
| H | ? | prequest.py | 184 |
| C | ? | viewderivers.py | 486 |
| C | ? | testing.py | 261 |
| C | ? | authentication.py | 408 |
| C | ? | csrf.py | 194 |
| C | ? | security.py | 261 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T04:06:14.377733*