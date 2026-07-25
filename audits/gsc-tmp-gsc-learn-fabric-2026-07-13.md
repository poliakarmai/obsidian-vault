---
title: "GSC Audit: /tmp/gsc-learn/fabric"
date: 2026-07-13
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/fabric

**Дата:** 13.07.2026 04:10  
**Путь:** `/tmp/gsc-learn/fabric`  
**Всего находок:** 160  
**CRITICAL:** 2 | **HIGH:** 24 | **MEDIUM:** 70 | **LOW:** 62

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: assert in production | 68 |
| CVE-2026-56233: Privilege escalation | 18 |
| GS003 | 3 |
| Хардкод IP адреса | 3 |
| GS001 | 2 |
| Generic code smell #24 | 1 |
| Generic code smell #27 | 1 |
| Generic code smell #30 | 1 |
| Generic code smell #33 | 1 |
| Generic code smell #36 | 1 |
| Generic code smell #39 | 1 |
| Generic code smell #42 | 1 |
| Generic code smell #45 | 1 |
| Generic code smell #48 | 1 |
| Generic code smell #51 | 1 |
| Generic code smell #54 | 1 |
| Generic code smell #57 | 1 |
| Generic code smell #60 | 1 |
| Generic code smell #63 | 1 |
| Generic code smell #66 | 1 |
| Generic code smell #69 | 1 |
| Generic code smell #72 | 1 |
| Generic code smell #75 | 1 |
| Generic code smell #78 | 1 |
| Generic code smell #81 | 1 |
| Generic code smell #84 | 1 |
| Generic code smell #87 | 1 |
| Generic code smell #90 | 1 |
| Generic code smell #93 | 1 |
| Generic code smell #96 | 1 |
| Generic code smell #99 | 1 |
| Generic code smell #102 | 1 |
| Generic code smell #105 | 1 |
| Generic code smell #108 | 1 |
| Generic code smell #111 | 1 |
| Generic code smell #114 | 1 |
| Generic code smell #117 | 1 |
| Generic code smell #120 | 1 |
| Generic code smell #123 | 1 |
| Generic code smell #126 | 1 |
| Generic code smell #129 | 1 |
| Generic code smell #132 | 1 |
| Generic code smell #135 | 1 |
| Generic code smell #138 | 1 |
| Generic code smell #141 | 1 |
| Generic code smell #144 | 1 |
| Generic code smell #147 | 1 |
| Generic code smell #150 | 1 |
| Generic code smell #153 | 1 |
| Generic code smell #156 | 1 |
| Generic code smell #159 | 1 |
| Generic code smell #162 | 1 |
| Generic code smell #165 | 1 |
| Generic code smell #168 | 1 |
| Generic code smell #171 | 1 |
| Generic code smell #174 | 1 |
| Generic code smell #177 | 1 |
| Generic code smell #180 | 1 |
| Generic code smell #183 | 1 |
| Generic code smell #186 | 1 |
| Generic code smell #189 | 1 |
| Generic code smell #192 | 1 |
| Generic code smell #195 | 1 |
| Generic code smell #198 | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| CVE-2026-37270: Hardcoded credential | 1 |
| GS015 | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .codecov.yml (664) | 1 |
| GS009 | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | auth.py | 191 | Found: password: ")
        # Then password.
        yield P |
| CRITICAL | GS001 | tasks.py | 36 | Found: password = "sikrit" |
| HIGH | ? | tasks.py | 45 |  |
| HIGH | ? | connection.py | 98 |  |
| HIGH | ? | connection.py | 104 |  |
| HIGH | ? | connection.py | 108 |  |
| HIGH | ? | connection.py | 113 |  |
| HIGH | ? | connection.py | 115 |  |
| HIGH | ? | connection.py | 122 |  |
| HIGH | ? | config.py | 75 |  |
| HIGH | ? | config.py | 90 |  |
| HIGH | ? | config.py | 94 |  |
| HIGH | ? | config.py | 95 |  |
| HIGH | ? | config.py | 96 |  |
| HIGH | ? | group.py | 118 |  |
| HIGH | ? | group.py | 127 |  |
| HIGH | ? | connection.py | 775 |  |
| HIGH | ? | connection.py | 777 |  |
| HIGH | ? | connection.py | 780 |  |
| HIGH | ? | connection.py | 835 |  |
| HIGH | ? | group.py | 9 | Match:         group = Group("localhost", "127.0.0.1") |
| HIGH | ? | group.py | 15 | Match:         group = Group("localhost", "127.0.0.1") |
| HIGH | ? | connection.py | 1063 | Match:             connections. Default: ``127.0.0.1`` (i.e. |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | connection.py | 525 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| L | ? | transfer.py | 11 |
| M | ? | tasks.py | 42 |
| M | ? | tasks.py | 43 |
| M | ? | tasks.py | 44 |
| M | ? | tasks.py | 45 |
| M | ? | tasks.py | 46 |
| M | ? | tasks.py | 47 |
| M | ? | tasks.py | 48 |
| M | ? | concurrency.py | 41 |
| M | ? | concurrency.py | 42 |
| M | ? | concurrency.py | 43 |
| M | ? | concurrency.py | 44 |
| M | ? | concurrency.py | 46 |
| M | ? | concurrency.py | 90 |
| M | ? | transfer.py | 27 |
| M | ? | transfer.py | 28 |
| M | ? | transfer.py | 30 |
| M | ? | transfer.py | 31 |
| M | ? | transfer.py | 32 |
| M | ? | transfer.py | 33 |
| M | ? | transfer.py | 38 |
| M | ? | transfer.py | 39 |
| M | ? | transfer.py | 40 |
| M | ? | transfer.py | 50 |
| M | ? | transfer.py | 66 |
| M | ? | transfer.py | 67 |
| M | ? | transfer.py | 69 |
| M | ? | transfer.py | 70 |
| M | ? | transfer.py | 71 |
| M | ? | transfer.py | 72 |
| M | ? | transfer.py | 79 |
| M | ? | transfer.py | 80 |
| M | ? | transfer.py | 81 |
| M | ? | transfer.py | 91 |
| M | ? | group.py | 12 |
| M | ? | group.py | 23 |
| M | ? | group.py | 25 |
| M | ? | group.py | 33 |
| M | ? | group.py | 35 |
| M | ? | connection.py | 25 |
| M | ? | connection.py | 26 |
| M | ? | connection.py | 34 |
| M | ? | connection.py | 35 |
| M | ? | connection.py | 43 |
| M | ? | connection.py | 44 |
| M | ? | connection.py | 45 |
| M | ? | connection.py | 58 |
| M | ? | connection.py | 60 |
| M | ? | connection.py | 61 |
| M | ? | connection.py | 71 |
| M | ? | connection.py | 72 |
| M | ? | connection.py | 73 |
| M | ? | connection.py | 74 |
| M | ? | connection.py | 75 |
| M | ? | connection.py | 83 |
| M | ? | connection.py | 84 |
| M | ? | connection.py | 92 |
| M | ? | connection.py | 93 |
| M | ? | connection.py | 95 |
| M | ? | connection.py | 96 |
| M | ? | connection.py | 113 |
| M | ? | connection.py | 121 |
| M | ? | connection.py | 122 |
| M | ? | connection.py | 137 |
| M | ? | connection.py | 144 |
| M | ? | connection.py | 151 |
| M | ? | connection.py | 154 |
| M | ? | base.py | 336 |
| M | ? | base.py | 340 |
| H | ? | tasks.py | 45 |
| H | ? | connection.py | 98 |
| H | ? | connection.py | 104 |
| H | ? | connection.py | 108 |
| H | ? | connection.py | 113 |
| H | ? | connection.py | 115 |
| H | ? | connection.py | 122 |
| H | ? | config.py | 75 |
| H | ? | config.py | 90 |
| H | ? | config.py | 94 |
| H | ? | config.py | 95 |
| H | ? | config.py | 96 |
| H | ? | group.py | 118 |
| H | ? | group.py | 127 |
| H | ? | connection.py | 775 |
| H | ? | connection.py | 777 |
| H | ? | connection.py | 780 |
| H | ? | connection.py | 835 |
| M | ? | tasks.py | 36 |
| M | ? | tasks.py | 36 |
| C | GS001 | auth.py | 191 |
| C | GS001 | tasks.py | 36 |
| L | GS003 | main.py | 21 |
| L | GS003 | main.py | 22 |
| L | GS003 | main.py | 172 |
| I | GS015 | main.py | 1 |
| H | ? | group.py | 9 |
| H | ? | group.py | 15 |
| H | ? | connection.py | 1063 |
| H | ? | codecov.yml | 0 |
| H | ? | .codecov.yml | 0 |
| s | GS009 |  | 0 |
| H | ? | connection.py | 525 |

---
*Сгенерировано GSC v0.6 · 2026-07-13T04:10:44.332942*