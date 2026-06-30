---
title: "GSC Audit: apolaibot"
date: 2026-06-26
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — apolaibot

**Дата:** 26.06.2026 08:42  
**Путь:** `/home/openclaw/projects/hermes-agent-orchestration`  
**Всего находок:** 137  
**CRITICAL:** 1 | **HIGH:** 7 | **MEDIUM:** 15 | **LOW:** 114

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 114 |
| Синхронный код в async | 15 |
| Хардкод IP адреса | 3 |
| Python: File upload without content-type validation | 2 |
| eval() or exec() usage | 2 |
| SQL injection risk: f-string in query | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | tenant-audit.py | 63 | OWASP A03: Injection |
| HIGH | ? | apolaibot-demo.py | 485 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | apolaibot-demo.py | 791 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | hermes-tenant | 149 | Match:          "-d", "127.0.0.0/8", "-j", "DROP"], |
| HIGH | ? | hermes-tenant | 160 | Match:         print(f"   👉 Ручками: sudo iptables -A OUTPUT |
| HIGH | ? | hermes-tenant | 168 | Match:          "-d", "127.0.0.0/8", "-j", "DROP"], |
| HIGH | ? | skill-validate.py | 86 | Match:         (r'\beval\s*\(', "eval() call detected"), |
| HIGH | ? | skill-validate.py | 87 | Match:         (r'\bexec\s*\(', "exec() call detected"), |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | tenant-audit.py | 63 |
| H | ? | apolaibot-demo.py | 485 |
| H | ? | apolaibot-demo.py | 791 |
| L | GS003 | apolaibot-demo.py | 80 |
| L | GS003 | apolaibot-demo.py | 90 |
| L | GS003 | miropolbot.py | 55 |
| L | GS003 | miropolbot.py | 56 |
| L | GS003 | miropolbot.py | 59 |
| L | GS003 | miropolbot.py | 64 |
| L | GS003 | miropolbot.py | 73 |
| L | GS003 | miropolbot.py | 74 |
| L | GS003 | miropolbot.py | 83 |
| L | GS003 | deepseek-balance-monitor.py | 99 |
| L | GS003 | deepseek-balance-monitor.py | 115 |
| L | GS003 | deepseek-balance-monitor.py | 119 |
| L | GS003 | deepseek-balance-monitor.py | 121 |
| L | GS003 | deepseek-balance-monitor.py | 128 |
| L | GS003 | deepseek-balance-monitor.py | 139 |
| L | GS003 | deprovision.py | 53 |
| L | GS003 | deprovision.py | 55 |
| L | GS003 | deprovision.py | 57 |
| L | GS003 | deprovision.py | 65 |
| L | GS003 | deprovision.py | 69 |
| L | GS003 | generate-tenant-dashboard.py | 365 |
| L | GS003 | rate_limiter.py | 272 |
| L | GS003 | rate_limiter.py | 277 |
| L | GS003 | rate_limiter.py | 280 |
| L | GS003 | skill-sync.py | 114 |
| L | GS003 | skill-sync.py | 145 |
| L | GS003 | skill-sync.py | 158 |
| L | GS003 | skill-sync.py | 162 |
| L | GS003 | skill-sync.py | 163 |
| L | GS003 | skill-sync.py | 165 |
| L | GS003 | skill-sync.py | 168 |
| L | GS003 | skill-sync.py | 186 |
| L | GS003 | skill-sync.py | 190 |
| L | GS003 | skill-sync.py | 194 |
| L | GS003 | skill-sync.py | 197 |
| L | GS003 | skill-sync.py | 208 |
| L | GS003 | skill-sync.py | 212 |
| L | GS003 | skill-sync.py | 213 |
| L | GS003 | skill-sync.py | 217 |
| L | GS003 | skill-sync.py | 228 |
| L | GS003 | skill-sync.py | 264 |
| L | GS003 | skill-sync.py | 266 |
| L | GS003 | skill-sync.py | 269 |
| L | GS003 | skill-sync.py | 273 |
| L | GS003 | skill-sync.py | 281 |
| L | GS003 | skill-sync.py | 293 |
| L | GS003 | skill-sync.py | 295 |
| L | GS003 | skill-sync.py | 301 |
| L | GS003 | skill-sync.py | 304 |
| L | GS003 | skill-sync.py | 308 |
| L | GS003 | skill-sync.py | 311 |
| L | GS003 | skill-sync.py | 315 |
| L | GS003 | skill-sync.py | 317 |
| L | GS003 | skill-sync.py | 320 |
| L | GS003 | skill-sync.py | 322 |
| L | GS003 | skill-sync.py | 325 |
| L | GS003 | skill-sync.py | 326 |
| L | GS003 | skill-sync.py | 333 |
| L | GS003 | skill-sync.py | 337 |
| L | GS003 | skill-sync.py | 340 |
| L | GS003 | skill-sync.py | 343 |
| L | GS003 | skill-sync.py | 350 |
| L | GS003 | skill-sync.py | 360 |
| L | GS003 | skill-sync.py | 363 |
| L | GS003 | skill-sync.py | 371 |
| L | GS003 | skill-sync.py | 380 |
| L | GS003 | skill-sync.py | 381 |
| L | GS003 | skill-sync.py | 387 |
| L | GS003 | skill-sync.py | 388 |
| L | GS003 | skill-sync.py | 393 |
| L | GS003 | skill-sync.py | 412 |
| L | GS003 | skill-sync.py | 414 |
| L | GS003 | skill-sync.py | 420 |
| L | GS003 | skill-sync.py | 425 |
| L | GS003 | skill-sync.py | 436 |
| L | GS003 | skill-sync.py | 443 |
| L | GS003 | skill-sync.py | 453 |
| L | GS003 | skill-sync.py | 457 |
| L | GS003 | skill-sync.py | 460 |
| L | GS003 | skill-sync.py | 466 |
| L | GS003 | skill-sync.py | 472 |
| L | GS003 | skill-sync.py | 488 |
| L | GS003 | skill-sync.py | 507 |
| L | GS003 | skill-sync.py | 515 |
| L | GS003 | skill-validate.py | 139 |
| L | GS003 | skill-validate.py | 146 |
| L | GS003 | skill-validate.py | 149 |
| L | GS003 | skill-validate.py | 151 |
| L | GS003 | skill-validate.py | 153 |
| L | GS003 | skill-validate.py | 155 |
| L | GS003 | stars-activator.py | 54 |
| L | GS003 | stars-activator.py | 67 |
| L | GS003 | stars-activator.py | 69 |
| L | GS003 | stars-activator.py | 71 |
| L | GS003 | tenant-audit.py | 128 |
| L | GS003 | tenant-audit.py | 129 |
| L | GS003 | tenant-audit.py | 130 |
| L | GS003 | tenant-audit.py | 131 |
| L | GS003 | tenant-audit.py | 132 |
| L | GS003 | tenant-audit.py | 139 |
| L | GS003 | tenant-audit.py | 142 |
| L | GS003 | tenant-audit.py | 146 |
| L | GS003 | tenant-audit.py | 147 |
| L | GS003 | tenant-audit.py | 152 |
| L | GS003 | tenant-audit.py | 156 |
| L | GS003 | tenant-audit.py | 157 |
| L | GS003 | tenant-backup.py | 35 |
| L | GS003 | tenant-backup.py | 42 |
| L | GS003 | tenant-backup.py | 61 |
| L | GS003 | tenant-backup.py | 68 |
| L | GS003 | tenant-rate-watch.py | 106 |
| L | GS003 | tenant-rate-watch.py | 121 |
| L | GS003 | tenant-rate-watch.py | 123 |
| L | GS003 | tenant-rate-watch.py | 135 |
| H | ? | hermes-tenant | 149 |
| H | ? | hermes-tenant | 160 |
| H | ? | hermes-tenant | 168 |
| H | ? | skill-validate.py | 86 |
| H | ? | skill-validate.py | 87 |
| M | ? | stars-activator.py | 63 |
| M | ? | hermes-tenant | 130 |
| M | ? | hermes-tenant | 155 |
| M | ? | hermes-tenant | 174 |
| M | ? | hermes-tenant | 189 |
| M | ? | hermes-tenant | 196 |
| M | ? | hermes-tenant | 350 |
| M | ? | hermes-tenant | 354 |
| M | ? | hermes-tenant | 408 |
| M | ? | hermes-tenant | 432 |
| M | ? | deprovision.py | 49 |
| M | ? | skill-sync.py | 67 |
| M | ? | skill-sync.py | 149 |
| M | ? | skill-sync.py | 172 |
| M | ? | skill-sync.py | 200 |

---
*Сгенерировано GSC v0.6 · 2026-06-26T08:42:32.253344*