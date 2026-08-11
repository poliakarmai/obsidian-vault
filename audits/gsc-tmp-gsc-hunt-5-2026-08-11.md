---
title: "GSC Audit: /tmp/gsc-hunt-5"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-5

**Дата:** 11.08.2026 07:06  
**Путь:** `/tmp/gsc-hunt-5`  
**Всего находок:** 311  
**CRITICAL:** 8 | **HIGH:** 18 | **MEDIUM:** 7 | **LOW:** 214

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 180 |
| GS022 | 21 |
| GS008 | 20 |
| GS020 | 19 |
| GS025 | 7 |
| GS007 | 7 |
| GS001 | 5 |
| GS014 | 4 |
| GS021 | 4 |
| GS025-debug_mode | 4 |
| GS003 | 3 |
| GS032-fake_tool_call_execute | 3 |
| GS029 | 2 |
| Systemd: NoNewPrivileges= not set | 2 |
| Systemd: ProtectSystem= not set | 2 |
| Systemd: ProtectHome= not set | 2 |
| Systemd: PrivateTmp= not set | 2 |
| Systemd: ProtectProc= not set | 2 |
| Systemd: MemoryDenyWriteExecute= not set | 2 |
| Systemd: RestrictRealtime= not set | 2 |
| Systemd: RemoveIPC= not set | 2 |
| Systemd: LockPersonality= not set | 2 |
| Systemd: RestrictSUIDSGID= not set | 2 |
| GS002 | 2 |
| YAML-B39DC08C | 2 |
| GS037-command_injection_shell_true | 1 |
| GS004 | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS017 | 1 |
| GS019 | 1 |
| YAML-ECB85AD8 | 1 |
| YAML-SSTI001 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS025 | manage.py | 120 |  |
| CRITICAL | GS001 | consul_config.py.ctmpl | 34 | Found: postgresql://{{template  |
| CRITICAL | GS001 | consul_config.py.ctmpl | 35 | Found: postgresql://{{template  |
| CRITICAL | GS001 | default_config.py | 7 | Found: postgresql://critiquebrainz:critiquebrainz@db:5432/cr |
| CRITICAL | GS001 | default_config.py | 11 | Found: postgresql://bookbrainz:bookbrainz@db:5432/bookbrainz |
| CRITICAL | GS001 | develop.sh | 3 | Found: postgresql://critiquebrainz:critiquebrainz@db/critiqu |
| CRITICAL | GS025 | Dockerfile | 83 | Match: RUN chmod 0644 /etc/cron.d/critiquebrainz |
| CRITICAL | GS019 | default_config.py | 4 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | GS029 | default_config.py | 4 | Hacking APIs (No Starch Press) |
| HIGH | GS000-LEGACY | default_config.py | 7 | Redteam Kit |
| HIGH | GS000-LEGACY | default_config.py | 11 | Redteam Kit |
| HIGH | GS000-LEGACY | default_config.py | 14 | Redteam Kit |
| HIGH | GS025 | package-lock.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | package.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | uwsgi.service | 0 | NoNewPrivileges= not set |
| HIGH | ? | cron-config.service | 0 | NoNewPrivileges= not set |
| HIGH | GS002 | consul-template-cron-config.conf | 0 | File consul-template-cron-config.conf has permissions -rw-rw |
| HIGH | GS002 | consul-template-uwsgi.conf | 0 | File consul-template-uwsgi.conf has permissions -rw-rw-r-- — |
| HIGH | GS004 | manage.py | 120 | Line 120: return subprocess.check_call(command, shell=True) |
| HIGH | GS011 | default_config.py | 4 | Found JWT secret in code: 'CHANGE_T...'. JWT secrets must be |
| HIGH | GS014 | default_config.py | 7 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | default_config.py | 11 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | default_config.py | 14 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | develop.sh | 3 | Database URL contains password in plaintext. Use environment |
| HIGH | GS017 | exceptions.py | 69 | Password length = 4 chars. |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| L | GS000-LEGACY | release_group.py | 52 |
| L | GS000-LEGACY | artist.py | 86 |
| L | GS000-LEGACY | label.py | 73 |
| H | GS029 | default_config.py | 4 |
| H | GS000-LEGACY | default_config.py | 7 |
| H | GS000-LEGACY | default_config.py | 11 |
| H | GS000-LEGACY | default_config.py | 14 |
| M | GS025 | default_config.py | 4 |
| M | GS025 | testing.py | 35 |
| C | GS025 | manage.py | 120 |
| M | GS029 | testing.py | 35 |
| C | GS001 | consul_config.py.ctmpl | 34 |
| C | GS001 | consul_config.py.ctmpl | 35 |
| C | GS001 | default_config.py | 7 |
| C | GS001 | default_config.py | 11 |
| C | GS001 | develop.sh | 3 |
| L | GS003 | fixtures.py | 16 |
| L | GS003 | fixtures.py | 18 |
| L | GS003 | utils.py | 98 |
| L | GS008 | default_config.py | 3 |
| L | GS008 | default_config.py | 7 |
| L | GS008 | default_config.py | 8 |
| L | GS008 | default_config.py | 11 |
| L | GS008 | default_config.py | 14 |
| L | GS008 | default_config.py | 17 |
| L | GS008 | default_config.py | 18 |
| L | GS008 | default_config.py | 19 |
| L | GS008 | default_config.py | 23 |
| L | GS008 | default_config.py | 27 |
| L | GS008 | default_config.py | 28 |
| L | GS008 | default_config.py | 29 |
| L | GS008 | default_config.py | 31 |
| L | GS008 | default_config.py | 35 |
| L | GS008 | default_config.py | 53 |
| L | GS008 | default_config.py | 56 |
| L | GS008 | default_config.py | 59 |
| L | GS008 | default_config.py | 62 |
| L | GS008 | default_config.py | 63 |
| L | GS008 | default_config.py | 64 |
| i | GS020 |  | 31 |
| i | GS020 |  | 2 |
| i | GS020 |  | 21 |
| i | GS020 |  | 40 |
| i | GS020 |  | 50 |
| i | GS020 |  | 19 |
| i | GS020 |  | 43 |
| i | GS020 |  | 26 |
| i | GS020 |  | 33 |
| i | GS020 |  | 24 |
| i | GS020 |  | 10 |
| i | GS020 |  | 14 |
| i | GS020 |  | 36 |
| i | GS020 |  | 51 |
| i | GS020 |  | 52 |
| i | GS020 |  | 63 |
| i | GS020 |  | 64 |
| i | GS020 |  | 17 |
| i | GS020 |  | 17 |
| ? | GS032-fake_tool_call_execute | manage.py | 50 |
| ? | GS032-fake_tool_call_execute | manage.py | 63 |
| ? | GS032-fake_tool_call_execute | manage.py | 76 |
| ? | GS037-command_injection_shell_true | dump_manager.py | 124 |
| C | GS025 | Dockerfile | 83 |
| H | GS025 | package-lock.json | 0 |
| H | GS025 | package.json | 0 |
| H | GS025 | .readthedocs.yaml | 0 |
| H | ? | uwsgi.service | 0 |
| M | ? | uwsgi.service | 0 |
| M | ? | uwsgi.service | 0 |
| L | ? | uwsgi.service | 0 |
| L | ? | uwsgi.service | 0 |
| L | ? | uwsgi.service | 0 |
| L | ? | uwsgi.service | 0 |
| L | ? | uwsgi.service | 0 |
| L | ? | uwsgi.service | 0 |
| L | ? | uwsgi.service | 0 |
| H | ? | cron-config.service | 0 |
| M | ? | cron-config.service | 0 |
| M | ? | cron-config.service | 0 |
| L | ? | cron-config.service | 0 |
| L | ? | cron-config.service | 0 |
| L | ? | cron-config.service | 0 |
| L | ? | cron-config.service | 0 |
| L | ? | cron-config.service | 0 |
| L | ? | cron-config.service | 0 |
| L | ? | cron-config.service | 0 |
| H | GS002 | consul-template-cron-config.conf | 0 |
| H | GS002 | consul-template-uwsgi.conf | 0 |
| H | GS004 | manage.py | 120 |
| I | GS007 | 11.sql | 13 |
| I | GS007 | 5.sql | 11 |
| I | GS007 | create_tables.sql | 13 |
| I | GS007 | create_tables.sql | 26 |
| I | GS007 | create_tables.sql | 46 |
| I | GS007 | create_tables.sql | 56 |
| I | GS007 | create_tables.sql | 86 |
| s | GS009 |  | 0 |
| H | GS011 | default_config.py | 4 |
| H | GS014 | default_config.py | 7 |
| H | GS014 | default_config.py | 11 |
| H | GS014 | default_config.py | 14 |
| H | GS014 | develop.sh | 3 |
| H | GS017 | exceptions.py | 69 |
| C | GS019 | default_config.py | 4 |
| s | GS021 |  | 27 |
| s | GS021 |  | 27 |
| s | GS021 |  | 8 |
| s | GS021 |  | 11 |
| r | GS022 |  | 15 |
| r | GS022 |  | 16 |
| r | GS022 |  | 71 |
| r | GS022 |  | 82 |
| r | GS022 |  | 17 |
| r | GS022 |  | 20 |
| r | GS022 |  | 22 |
| r | GS022 |  | 78 |
| r | GS022 |  | 28 |
| r | GS022 |  | 36 |
| r | GS022 |  | 12 |
| r | GS022 |  | 16 |
| r | GS022 |  | 31 |
| r | GS022 |  | 11 |
| r | GS022 |  | 23 |
| r | GS022 |  | 14 |
| r | GS022 |  | 29 |
| r | GS022 |  | 45 |
| r | GS022 |  | 12 |
| r | GS022 |  | 16 |
| r | GS022 |  | 32 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | YAML-ECB85AD8 | custom_config.py.example | ? |
| ? | YAML-B39DC08C | fixtures.py | ? |
| ? | YAML-B39DC08C | fixtures.py | ? |
| ? | YAML-SSTI001 | base.html | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-11T07:06:39.211395*