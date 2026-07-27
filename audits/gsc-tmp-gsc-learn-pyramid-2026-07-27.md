---
title: "GSC Audit: /tmp/gsc-learn/pyramid"
date: 2026-07-27
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/pyramid

**Дата:** 27.07.2026 04:05  
**Путь:** `/tmp/gsc-learn/pyramid`  
**Всего находок:** 153  
**CRITICAL:** 5 | **HIGH:** 5 | **MEDIUM:** 15 | **LOW:** 126

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 8 |
| CVE-2026-37270: Hardcoded credential | 7 |
| CVE-2026-56318: Information disclosure | 5 |
| Хардкод IP адреса | 3 |
| Hardcoded encryption key | 3 |
| Generic code smell #24 | 2 |
| Generic code smell #27 | 2 |
| Generic code smell #30 | 2 |
| Generic code smell #33 | 2 |
| Generic code smell #36 | 2 |
| Generic code smell #39 | 2 |
| Generic code smell #42 | 2 |
| Generic code smell #45 | 2 |
| Generic code smell #48 | 2 |
| Generic code smell #51 | 2 |
| Generic code smell #54 | 2 |
| Generic code smell #57 | 2 |
| Generic code smell #60 | 2 |
| Generic code smell #63 | 2 |
| Generic code smell #66 | 2 |
| Generic code smell #69 | 2 |
| Generic code smell #72 | 2 |
| Generic code smell #75 | 2 |
| Generic code smell #78 | 2 |
| Generic code smell #81 | 2 |
| Generic code smell #84 | 2 |
| Generic code smell #87 | 2 |
| Generic code smell #90 | 2 |
| Generic code smell #93 | 2 |
| Generic code smell #96 | 2 |
| Generic code smell #99 | 2 |
| Generic code smell #102 | 2 |
| Generic code smell #105 | 2 |
| Generic code smell #108 | 2 |
| Generic code smell #111 | 2 |
| Generic code smell #114 | 2 |
| Generic code smell #117 | 2 |
| Generic code smell #120 | 2 |
| Generic code smell #123 | 2 |
| Generic code smell #126 | 2 |
| Generic code smell #129 | 2 |
| Generic code smell #132 | 2 |
| Generic code smell #135 | 2 |
| Generic code smell #138 | 2 |
| Generic code smell #141 | 2 |
| Generic code smell #144 | 2 |
| Generic code smell #147 | 2 |
| Generic code smell #150 | 2 |
| Generic code smell #153 | 2 |
| Generic code smell #156 | 2 |
| Generic code smell #159 | 2 |
| Generic code smell #162 | 2 |
| Generic code smell #165 | 2 |
| Generic code smell #168 | 2 |
| Generic code smell #171 | 2 |
| Generic code smell #174 | 2 |
| Generic code smell #177 | 2 |
| Generic code smell #180 | 2 |
| Generic code smell #183 | 2 |
| Generic code smell #186 | 2 |
| Generic code smell #189 | 2 |
| Generic code smell #192 | 2 |
| Generic code smell #195 | 2 |
| Generic code smell #198 | 2 |
| Python: assert in production | 2 |
| CVE-2026-55223: Insecure deserialization | 1 |
| GS001 | 1 |
| GS015 | 1 |
| pickle.load() — unsafe deserialization | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| GS009 | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | testing.py | 261 | Found: token = '0123456789012345678901234567890123456789' |
| CRITICAL | ? | viewderivers.py | 486 | Match:         token = 'csrf_token' |
| CRITICAL | ? | csrf.py | 194 | Match:     request, token='csrf_token', header='X-CSRF-Token |
| CRITICAL | ? | security.py | 261 | Match:         token='csrf_token', |
| CRITICAL | ? | session.py | 70 | Match:             return pickle.loads(bstruct) |
| HIGH | ? | authentication.py | 1060 | Match:             remote_addr = '0.0.0.0' |
| HIGH | ? | authentication.py | 1148 | Match:             remote_addr = '0.0.0.0' |
| HIGH | ? | pserve.py | 332 | Match:         127.0.0.1, which is not a public interface. |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | viewderivers.py | 455 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| L | ? | session.py | 264 |
| L | ? | predicates.py | 151 |
| M | ? | actions.py | 74 |
| M | ? | registry.py | 228 |
| M | ? | session.py | 70 |
| M | ? | viewderivers.py | 486 |
| M | ? | testing.py | 261 |
| M | ? | csrf.py | 194 |
| M | ? | csrf.py | 229 |
| M | ? | security.py | 261 |
| M | ? | viewderivers.py | 486 |
| M | ? | testing.py | 261 |
| M | ? | authentication.py | 408 |
| M | ? | csrf.py | 70 |
| M | ? | csrf.py | 194 |
| M | ? | csrf.py | 229 |
| M | ? | security.py | 261 |
| C | GS001 | testing.py | 261 |
| L | GS008 | authorization.py | 46 |
| L | GS008 | predicates.py | 11 |
| L | GS008 | interfaces.py | 1644 |
| L | GS008 | interfaces.py | 1645 |
| L | GS008 | interfaces.py | 1646 |
| L | GS008 | interfaces.py | 1647 |
| L | GS008 | security.py | 14 |
| L | GS008 | tweens.py | 51 |
| I | GS015 | wsgi.py | 1 |
| H | ? | authentication.py | 1060 |
| H | ? | authentication.py | 1148 |
| H | ? | pserve.py | 332 |
| C | ? | viewderivers.py | 486 |
| C | ? | csrf.py | 194 |
| C | ? | security.py | 261 |
| C | ? | session.py | 70 |
| H | ? | .readthedocs.yaml | 0 |
| s | GS009 |  | 0 |
| H | ? | viewderivers.py | 455 |

---
*Сгенерировано GSC v0.6 · 2026-07-27T04:05:08.513956*