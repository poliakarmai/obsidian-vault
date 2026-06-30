---
title: "GSC Audit: /tmp/gsc_scan_targets/ssh-key-manager"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/ssh-key-manager

**Дата:** 29.06.2026 14:21  
**Путь:** `/tmp/gsc_scan_targets/ssh-key-manager`  
**Всего находок:** 10  
**CRITICAL:** 0 | **HIGH:** 2 | **MEDIUM:** 0 | **LOW:** 7

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 7 |
| os.system() without sanitization | 1 |
| GS004 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | ssh_mgr.py | 24 | Match:     os.system(f'ssh-keygen -t {key_type} -f {key_path |
| HIGH | GS004 | ssh_mgr.py | 24 | Line 24: os.system(f'ssh-keygen -t {key_type} -f {key_path}  |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| L | GS003 | ssh_mgr.py | 23 |
| L | GS003 | ssh_mgr.py | 32 |
| L | GS003 | ssh_mgr.py | 41 |
| L | GS003 | ssh_mgr.py | 45 |
| L | GS003 | ssh_mgr.py | 47 |
| L | GS003 | ssh_mgr.py | 48 |
| L | GS003 | ssh_mgr.py | 50 |
| H | ? | ssh_mgr.py | 24 |
| H | GS004 | ssh_mgr.py | 24 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:21:56.929725*