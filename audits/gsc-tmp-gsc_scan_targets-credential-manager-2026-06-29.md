---
title: "GSC Audit: /tmp/gsc_scan_targets/credential-manager"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/credential-manager

**Дата:** 29.06.2026 14:21  
**Путь:** `/tmp/gsc_scan_targets/credential-manager`  
**Всего находок:** 8  
**CRITICAL:** 7 | **HIGH:** 0 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS001 | 6 |
| Hardcoded encryption key | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | credential-manager | 170 | Found: password = "<decryption error>" |
| CRITICAL | GS001 | credential-manager | 435 | Found: password: ")
        confirmation = safe_getpass(" |
| CRITICAL | GS001 | credential-manager | 436 | Found: password: ")
        if password == confirmation:
    |
| CRITICAL | GS001 | credential-manager | 451 | Found: password: ")
    key = derive_key(entered, salt)

    |
| CRITICAL | GS001 | credential-manager | 602 | Found: password: ")
        confirm = safe_getpass(" |
| CRITICAL | GS001 | credential-manager | 603 | Found: password: ")
        
        if master != confirm:
  |
| CRITICAL | ? | credential-manager | 170 | Match:                 password = "<decryption error>" |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | credential-manager | 170 |
| C | GS001 | credential-manager | 435 |
| C | GS001 | credential-manager | 436 |
| C | GS001 | credential-manager | 451 |
| C | GS001 | credential-manager | 602 |
| C | GS001 | credential-manager | 603 |
| C | ? | credential-manager | 170 |
| s | GS009 |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:21:52.352629*