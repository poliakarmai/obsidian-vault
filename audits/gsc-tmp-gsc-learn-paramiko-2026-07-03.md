---
title: "GSC Audit: /tmp/gsc-learn/paramiko"
date: 2026-07-03
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/paramiko

**Дата:** 03.07.2026 04:04  
**Путь:** `/tmp/gsc-learn/paramiko`  
**Всего находок:** 116  
**CRITICAL:** 1 | **HIGH:** 4 | **MEDIUM:** 20 | **LOW:** 89

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS008 | 24 |
| Bare except: | 11 |
| Python: assert in production | 9 |
| GS003 | 6 |
| Хардкод IP адреса | 2 |
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
| GS001 | 1 |
| GS015 | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: .codecov.yml (664) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | common.py | 166 | Found: TOKEN: "userauth-gssapi-token" |
| HIGH | ? | pipe.py | 82 | Match:         serv.bind(("127.0.0.1", 0)) |
| HIGH | ? | pipe.py | 87 | Match:         self._rsock.connect(("127.0.0.1", serv.getsoc |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .codecov.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | channel.py | 139 |
| M | ? | pkey.py | 639 |
| M | ? | sftp_file.py | 534 |
| M | ? | transport.py | 2169 |
| M | ? | agent.py | 148 |
| M | ? | agent.py | 203 |
| M | ? | agent.py | 231 |
| M | ? | client.py | 362 |
| M | ? | sftp_server.py | 159 |
| M | ? | primes.py | 121 |
| M | ? | server.py | 622 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| L | ? | client.py | 438 |
| M | ? | channel.py | 401 |
| M | ? | channel.py | 1218 |
| M | ? | hostkeys.py | 299 |
| M | ? | rsakey.py | 222 |
| M | ? | ed25519key.py | 152 |
| M | ? | common.py | 31 |
| M | ? | common.py | 36 |
| M | ? | _winapi.py | 172 |
| M | ? | _winapi.py | 398 |
| C | GS001 | common.py | 166 |
| L | GS003 | transport.py | 1668 |
| L | GS003 | transport.py | 1670 |
| L | GS003 | transport.py | 1672 |
| L | GS003 | transport.py | 3298 |
| L | GS003 | transport.py | 3300 |
| L | GS003 | transport.py | 3302 |
| L | GS008 | _winapi.py | 89 |
| L | GS008 | _winapi.py | 206 |
| L | GS008 | _winapi.py | 221 |
| L | GS008 | _winapi.py | 223 |
| L | GS008 | _winapi.py | 240 |
| L | GS008 | _winapi.py | 246 |
| L | GS008 | _winapi.py | 258 |
| L | GS008 | common.py | 72 |
| L | GS008 | common.py | 128 |
| L | GS008 | common.py | 188 |
| L | GS008 | common.py | 232 |
| L | GS008 | common.py | 233 |
| L | GS008 | common.py | 238 |
| L | GS008 | common.py | 242 |
| L | GS008 | common.py | 245 |
| L | GS008 | sftp.py | 53 |
| L | GS008 | sftp.py | 65 |
| L | GS008 | sftp.py | 77 |
| L | GS008 | sftp.py | 78 |
| L | GS008 | sftp.py | 79 |
| L | GS008 | sftp.py | 80 |
| L | GS008 | sftp.py | 81 |
| L | GS008 | sftp.py | 82 |
| L | GS008 | sftp.py | 88 |
| I | GS015 | server.py | 1 |
| H | ? | pipe.py | 82 |
| H | ? | pipe.py | 87 |
| H | ? | codecov.yml | 0 |
| H | ? | .codecov.yml | 0 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-07-03T04:04:21.667374*