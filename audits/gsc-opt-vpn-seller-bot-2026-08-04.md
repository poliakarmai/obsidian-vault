---
title: "GSC Audit: /opt/vpn-seller-bot"
date: 2026-08-04
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /opt/vpn-seller-bot

**Дата:** 04.08.2026 22:26  
**Путь:** `/opt/vpn-seller-bot`  
**Всего находок:** 627  
**CRITICAL:** 2 | **HIGH:** 19 | **MEDIUM:** 52 | **LOW:** 21

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS022 | 460 |
| GS021 | 49 |
| Синхронный код в async | 48 |
| GS020 | 23 |
| GS003 | 21 |
| Хардкод IP адреса | 7 |
| CVE-2026-56233: Privilege escalation | 6 |
| GS018 | 3 |
| CVE-2026-37270: Hardcoded credential | 2 |
| Hardcoded encryption key | 2 |
| Bare except: | 1 |
| Python: File upload without content-type validation | 1 |
| CVE-2026-56233: Path traversal | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| World-readable file: bot.db (644) | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | bot.py.bak_v1 | 1820 | Match:         msg_key = "lang_set_ru" if new_lang == "ru" e |
| CRITICAL | ? | bot.py.bak.audit-20260611 | 1713 | Match:         msg_key = "lang_set_ru" if new_lang == "ru" e |
| HIGH | ? | bot.py | 1177 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | bot.py | 293 |  |
| HIGH | ? | bot.py | 917 |  |
| HIGH | ? | bot.py | 952 |  |
| HIGH | ? | bot.py | 962 |  |
| HIGH | ? | admin_key_v2.py | 97 |  |
| HIGH | ? | admin_key_v2.py | 111 |  |
| HIGH | ? | admin_key.py | 159 |  |
| HIGH | ? | bot.py.bak_v1 | 997 | Match: DNS = 1.1.1.1, 8.8.8.8 |
| HIGH | ? | bot.py.bak_v1 | 1013 | Match: AllowedIPs = 0.0.0.0/0 |
| HIGH | ? | bot.py.bak.audit-20260611 | 173 | Match:     "proxy_access":         {"ru": "🔑 Твой MTProto пр |
| HIGH | ? | bot.py.bak.audit-20260611 | 934 | Match: DNS = 1.1.1.1, 8.8.8.8 |
| HIGH | ? | bot.py.bak.audit-20260611 | 950 | Match: AllowedIPs = 0.0.0.0/0 |
| HIGH | ? | bot.py | 1000 | Match: DNS = 1.1.1.1, 8.8.8.8 |
| HIGH | ? | bot.py | 1016 | Match: AllowedIPs = 0.0.0.0/0 |
| HIGH | ? | bot.db | 0 | Permissions 644 — should be 600 for sensitive files |
| HIGH | GS018 | bot.py | 640 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | bot.py | 785 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | GS018 | bot.py | 1860 | Float arithmetic for money leads to rounding errors exploita |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | admin_key_v2.py | 42 |
| H | ? | bot.py | 1177 |
| H | ? | bot.py | 293 |
| H | ? | bot.py | 917 |
| H | ? | bot.py | 952 |
| H | ? | bot.py | 962 |
| H | ? | admin_key_v2.py | 97 |
| H | ? | admin_key_v2.py | 111 |
| H | ? | admin_key.py | 159 |
| M | ? | bot.py | 1276 |
| M | ? | bot.py | 1276 |
| M | ? | bot.py | 1835 |
| L | GS003 | admin_key.py | 155 |
| L | GS003 | admin_key.py | 175 |
| L | GS003 | admin_key.py | 182 |
| L | GS003 | admin_key.py | 183 |
| L | GS003 | admin_key.py | 189 |
| L | GS003 | admin_key.py | 190 |
| L | GS003 | admin_key.py | 191 |
| L | GS003 | admin_key.py | 192 |
| L | GS003 | admin_key.py | 193 |
| L | GS003 | admin_key.py | 195 |
| L | GS003 | admin_key_v2.py | 96 |
| L | GS003 | admin_key_v2.py | 113 |
| L | GS003 | admin_key_v2.py | 121 |
| L | GS003 | admin_key_v2.py | 122 |
| L | GS003 | admin_key_v2.py | 123 |
| L | GS003 | admin_key_v2.py | 128 |
| L | GS003 | admin_key_v2.py | 129 |
| L | GS003 | admin_key_v2.py | 131 |
| L | GS003 | admin_key_v2.py | 137 |
| L | GS003 | admin_key_v2.py | 145 |
| L | GS003 | admin_key_v2.py | 150 |
| i | GS020 |  | 116 |
| i | GS020 |  | 21 |
| i | GS020 |  | 15 |
| i | GS020 |  | 22 |
| i | GS020 |  | 23 |
| i | GS020 |  | 175 |
| i | GS020 |  | 711 |
| i | GS020 |  | 507 |
| i | GS020 |  | 1014 |
| i | GS020 |  | 1022 |
| i | GS020 |  | 1022 |
| i | GS020 |  | 1058 |
| i | GS020 |  | 15 |
| i | GS020 |  | 68 |
| i | GS020 |  | 1429 |
| i | GS020 |  | 1435 |
| i | GS020 |  | 1436 |
| i | GS020 |  | 1438 |
| i | GS020 |  | 1449 |
| i | GS020 |  | 1450 |
| i | GS020 |  | 1453 |
| i | GS020 |  | 1 |
| i | GS020 |  | 194 |
| H | ? | bot.py.bak_v1 | 997 |
| H | ? | bot.py.bak_v1 | 1013 |
| H | ? | bot.py.bak.audit-20260611 | 173 |
| H | ? | bot.py.bak.audit-20260611 | 934 |
| H | ? | bot.py.bak.audit-20260611 | 950 |
| H | ? | bot.py | 1000 |
| H | ? | bot.py | 1016 |
| C | ? | bot.py.bak_v1 | 1820 |
| C | ? | bot.py.bak.audit-20260611 | 1713 |
| H | ? | bot.db | 0 |
| s | GS009 |  | 0 |
| H | GS018 | bot.py | 640 |
| H | GS018 | bot.py | 785 |
| H | GS018 | bot.py | 1860 |
| s | GS021 |  | 1016 |
| s | GS021 |  | 783 |
| s | GS021 |  | 783 |
| s | GS021 |  | 811 |
| s | GS021 |  | 811 |
| s | GS021 |  | 111 |
| s | GS021 |  | 570 |
| s | GS021 |  | 245 |
| s | GS021 |  | 250 |
| s | GS021 |  | 258 |
| s | GS021 |  | 258 |
| s | GS021 |  | 289 |
| s | GS021 |  | 305 |
| s | GS021 |  | 498 |
| s | GS021 |  | 236 |
| s | GS021 |  | 209 |
| s | GS021 |  | 137 |
| s | GS021 |  | 3514 |
| s | GS021 |  | 3514 |
| s | GS021 |  | 3514 |
| s | GS021 |  | 209 |
| s | GS021 |  | 216 |
| s | GS021 |  | 248 |
| s | GS021 |  | 721 |
| s | GS021 |  | 225 |
| s | GS021 |  | 118 |
| s | GS021 |  | 294 |
| s | GS021 |  | 392 |
| s | GS021 |  | 468 |
| s | GS021 |  | 71 |
| s | GS021 |  | 36 |
| s | GS021 |  | 556 |
| s | GS021 |  | 679 |
| s | GS021 |  | 526 |
| s | GS021 |  | 549 |
| s | GS021 |  | 79 |
| s | GS021 |  | 86 |
| s | GS021 |  | 128 |
| s | GS021 |  | 147 |
| s | GS021 |  | 84 |
| s | GS021 |  | 82 |
| s | GS021 |  | 106 |
| s | GS021 |  | 128 |
| s | GS021 |  | 147 |
| s | GS021 |  | 84 |
| s | GS021 |  | 82 |
| s | GS021 |  | 106 |
| s | GS021 |  | 297 |
| s | GS021 |  | 490 |
| r | GS022 |  | 24 |
| r | GS022 |  | 164 |
| r | GS022 |  | 168 |
| r | GS022 |  | 228 |
| r | GS022 |  | 231 |
| r | GS022 |  | 238 |
| r | GS022 |  | 377 |
| r | GS022 |  | 377 |
| r | GS022 |  | 385 |
| r | GS022 |  | 385 |
| r | GS022 |  | 441 |
| r | GS022 |  | 1221 |
| r | GS022 |  | 1223 |
| r | GS022 |  | 1249 |
| r | GS022 |  | 1251 |
| r | GS022 |  | 51 |
| r | GS022 |  | 164 |
| r | GS022 |  | 178 |
| r | GS022 |  | 179 |
| r | GS022 |  | 266 |
| r | GS022 |  | 271 |
| r | GS022 |  | 322 |
| r | GS022 |  | 158 |
| r | GS022 |  | 96 |
| r | GS022 |  | 99 |
| r | GS022 |  | 165 |
| r | GS022 |  | 237 |
| r | GS022 |  | 249 |
| r | GS022 |  | 254 |
| r | GS022 |  | 415 |
| r | GS022 |  | 401 |
| r | GS022 |  | 847 |
| r | GS022 |  | 856 |
| r | GS022 |  | 959 |
| r | GS022 |  | 74 |
| r | GS022 |  | 265 |
| r | GS022 |  | 280 |
| r | GS022 |  | 619 |
| r | GS022 |  | 623 |
| r | GS022 |  | 284 |
| r | GS022 |  | 378 |
| r | GS022 |  | 379 |
| r | GS022 |  | 452 |
| r | GS022 |  | 454 |
| r | GS022 |  | 463 |
| r | GS022 |  | 465 |
| r | GS022 |  | 509 |
| r | GS022 |  | 543 |
| r | GS022 |  | 546 |
| r | GS022 |  | 662 |
| r | GS022 |  | 667 |
| r | GS022 |  | 1063 |
| r | GS022 |  | 1068 |
| r | GS022 |  | 231 |
| r | GS022 |  | 293 |
| r | GS022 |  | 451 |
| r | GS022 |  | 827 |
| r | GS022 |  | 188 |
| r | GS022 |  | 391 |
| r | GS022 |  | 258 |
| r | GS022 |  | 2 |
| r | GS022 |  | 136 |
| r | GS022 |  | 151 |
| r | GS022 |  | 157 |
| r | GS022 |  | 162 |
| r | GS022 |  | 202 |
| r | GS022 |  | 207 |
| r | GS022 |  | 213 |
| r | GS022 |  | 299 |
| r | GS022 |  | 314 |
| r | GS022 |  | 329 |
| r | GS022 |  | 348 |
| r | GS022 |  | 370 |
| r | GS022 |  | 375 |
| r | GS022 |  | 381 |
| r | GS022 |  | 239 |
| r | GS022 |  | 332 |
| r | GS022 |  | 532 |
| r | GS022 |  | 179 |
| r | GS022 |  | 267 |
| r | GS022 |  | 274 |
| r | GS022 |  | 275 |
| r | GS022 |  | 345 |
| r | GS022 |  | 370 |
| r | GS022 |  | 375 |
| r | GS022 |  | 460 |
| r | GS022 |  | 496 |
| r | GS022 |  | 503 |
| r | GS022 |  | 762 |
| r | GS022 |  | 1005 |
| r | GS022 |  | 1508 |
| r | GS022 |  | 1753 |
| r | GS022 |  | 324 |
| r | GS022 |  | 329 |
| r | GS022 |  | 331 |
| r | GS022 |  | 336 |
| r | GS022 |  | 338 |
| r | GS022 |  | 340 |
| r | GS022 |  | 345 |
| r | GS022 |  | 347 |
| r | GS022 |  | 349 |
| r | GS022 |  | 354 |
| r | GS022 |  | 356 |
| r | GS022 |  | 370 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 15 |
| r | GS022 |  | 43 |
| r | GS022 |  | 45 |
| r | GS022 |  | 50 |
| r | GS022 |  | 52 |
| r | GS022 |  | 59 |
| r | GS022 |  | 59 |
| r | GS022 |  | 60 |
| r | GS022 |  | 61 |
| r | GS022 |  | 95 |
| r | GS022 |  | 115 |
| r | GS022 |  | 174 |
| r | GS022 |  | 177 |
| r | GS022 |  | 180 |
| r | GS022 |  | 183 |
| r | GS022 |  | 201 |
| r | GS022 |  | 204 |
| r | GS022 |  | 207 |
| r | GS022 |  | 210 |
| r | GS022 |  | 226 |
| r | GS022 |  | 226 |
| r | GS022 |  | 227 |
| r | GS022 |  | 249 |
| r | GS022 |  | 266 |
| r | GS022 |  | 314 |
| r | GS022 |  | 322 |
| r | GS022 |  | 334 |
| r | GS022 |  | 349 |
| r | GS022 |  | 354 |
| r | GS022 |  | 374 |
| r | GS022 |  | 380 |
| r | GS022 |  | 380 |
| r | GS022 |  | 386 |
| r | GS022 |  | 329 |
| r | GS022 |  | 561 |
| r | GS022 |  | 40 |
| r | GS022 |  | 45 |
| r | GS022 |  | 189 |
| r | GS022 |  | 195 |
| r | GS022 |  | 214 |
| r | GS022 |  | 231 |
| r | GS022 |  | 268 |
| r | GS022 |  | 345 |
| r | GS022 |  | 355 |
| r | GS022 |  | 504 |
| r | GS022 |  | 346 |
| r | GS022 |  | 347 |
| r | GS022 |  | 348 |
| r | GS022 |  | 349 |
| r | GS022 |  | 350 |
| r | GS022 |  | 351 |
| r | GS022 |  | 352 |
| r | GS022 |  | 352 |
| r | GS022 |  | 353 |
| r | GS022 |  | 354 |
| r | GS022 |  | 355 |
| r | GS022 |  | 366 |
| r | GS022 |  | 367 |
| r | GS022 |  | 368 |
| r | GS022 |  | 369 |
| r | GS022 |  | 370 |
| r | GS022 |  | 169 |
| r | GS022 |  | 335 |
| r | GS022 |  | 28 |
| r | GS022 |  | 29 |
| r | GS022 |  | 36 |
| r | GS022 |  | 37 |
| r | GS022 |  | 66 |
| r | GS022 |  | 2458 |
| r | GS022 |  | 26 |
| r | GS022 |  | 26 |
| r | GS022 |  | 70 |
| r | GS022 |  | 38 |
| r | GS022 |  | 189 |
| r | GS022 |  | 1614 |
| r | GS022 |  | 20 |
| r | GS022 |  | 46 |
| r | GS022 |  | 104 |
| r | GS022 |  | 22 |
| r | GS022 |  | 76 |
| r | GS022 |  | 78 |
| r | GS022 |  | 191 |
| r | GS022 |  | 196 |
| r | GS022 |  | 206 |
| r | GS022 |  | 218 |
| r | GS022 |  | 219 |
| r | GS022 |  | 246 |
| r | GS022 |  | 348 |
| r | GS022 |  | 566 |
| r | GS022 |  | 705 |
| r | GS022 |  | 771 |
| r | GS022 |  | 792 |
| r | GS022 |  | 873 |
| r | GS022 |  | 892 |
| r | GS022 |  | 363 |
| r | GS022 |  | 110 |
| r | GS022 |  | 518 |
| r | GS022 |  | 660 |
| r | GS022 |  | 491 |
| r | GS022 |  | 498 |
| r | GS022 |  | 499 |
| r | GS022 |  | 643 |
| r | GS022 |  | 1083 |
| r | GS022 |  | 1100 |
| r | GS022 |  | 303 |
| r | GS022 |  | 314 |
| r | GS022 |  | 378 |
| r | GS022 |  | 497 |
| r | GS022 |  | 534 |
| r | GS022 |  | 544 |
| r | GS022 |  | 555 |
| r | GS022 |  | 853 |
| r | GS022 |  | 77 |
| r | GS022 |  | 85 |
| r | GS022 |  | 84 |
| r | GS022 |  | 168 |
| r | GS022 |  | 365 |
| r | GS022 |  | 464 |
| r | GS022 |  | 151 |
| r | GS022 |  | 50 |
| r | GS022 |  | 97 |
| r | GS022 |  | 105 |
| r | GS022 |  | 17 |
| r | GS022 |  | 183 |
| r | GS022 |  | 86 |
| r | GS022 |  | 368 |
| r | GS022 |  | 410 |
| r | GS022 |  | 434 |
| r | GS022 |  | 436 |
| r | GS022 |  | 445 |
| r | GS022 |  | 455 |
| r | GS022 |  | 457 |
| r | GS022 |  | 594 |
| r | GS022 |  | 15 |
| r | GS022 |  | 38 |
| r | GS022 |  | 44 |
| r | GS022 |  | 49 |
| r | GS022 |  | 56 |
| r | GS022 |  | 199 |
| r | GS022 |  | 17 |
| r | GS022 |  | 129 |
| r | GS022 |  | 130 |
| r | GS022 |  | 176 |
| r | GS022 |  | 200 |
| r | GS022 |  | 204 |
| r | GS022 |  | 209 |
| r | GS022 |  | 316 |
| r | GS022 |  | 323 |
| r | GS022 |  | 49 |
| r | GS022 |  | 230 |
| r | GS022 |  | 642 |
| r | GS022 |  | 774 |
| r | GS022 |  | 837 |
| r | GS022 |  | 869 |
| r | GS022 |  | 987 |
| r | GS022 |  | 1010 |
| r | GS022 |  | 1016 |
| r | GS022 |  | 1062 |
| r | GS022 |  | 30 |
| r | GS022 |  | 214 |
| r | GS022 |  | 226 |
| r | GS022 |  | 344 |
| r | GS022 |  | 346 |
| r | GS022 |  | 351 |
| r | GS022 |  | 354 |
| r | GS022 |  | 355 |
| r | GS022 |  | 356 |
| r | GS022 |  | 370 |
| r | GS022 |  | 385 |
| r | GS022 |  | 390 |
| r | GS022 |  | 427 |
| r | GS022 |  | 456 |
| r | GS022 |  | 459 |
| r | GS022 |  | 82 |
| r | GS022 |  | 111 |
| r | GS022 |  | 132 |
| r | GS022 |  | 143 |
| r | GS022 |  | 146 |
| r | GS022 |  | 333 |
| r | GS022 |  | 344 |
| r | GS022 |  | 348 |
| r | GS022 |  | 349 |
| r | GS022 |  | 350 |
| r | GS022 |  | 351 |
| r | GS022 |  | 352 |
| r | GS022 |  | 353 |
| r | GS022 |  | 357 |
| r | GS022 |  | 419 |
| r | GS022 |  | 434 |
| r | GS022 |  | 179 |
| r | GS022 |  | 358 |
| r | GS022 |  | 359 |
| r | GS022 |  | 360 |
| r | GS022 |  | 361 |
| r | GS022 |  | 362 |
| r | GS022 |  | 363 |
| r | GS022 |  | 364 |
| r | GS022 |  | 364 |
| r | GS022 |  | 365 |
| r | GS022 |  | 366 |
| r | GS022 |  | 367 |
| r | GS022 |  | 380 |
| r | GS022 |  | 381 |
| r | GS022 |  | 382 |
| r | GS022 |  | 383 |
| r | GS022 |  | 384 |
| r | GS022 |  | 180 |
| r | GS022 |  | 80 |
| r | GS022 |  | 294 |
| r | GS022 |  | 448 |
| r | GS022 |  | 23 |
| r | GS022 |  | 42 |
| r | GS022 |  | 282 |
| r | GS022 |  | 298 |
| r | GS022 |  | 305 |
| r | GS022 |  | 339 |
| r | GS022 |  | 350 |
| r | GS022 |  | 353 |
| r | GS022 |  | 399 |
| r | GS022 |  | 495 |
| r | GS022 |  | 30 |
| r | GS022 |  | 82 |
| r | GS022 |  | 92 |
| r | GS022 |  | 57 |
| r | GS022 |  | 67 |
| r | GS022 |  | 320 |
| r | GS022 |  | 327 |
| r | GS022 |  | 449 |
| r | GS022 |  | 452 |
| r | GS022 |  | 464 |
| r | GS022 |  | 464 |
| r | GS022 |  | 526 |
| r | GS022 |  | 611 |
| r | GS022 |  | 80 |
| r | GS022 |  | 88 |
| r | GS022 |  | 109 |
| r | GS022 |  | 80 |
| r | GS022 |  | 349 |
| r | GS022 |  | 376 |
| r | GS022 |  | 379 |
| r | GS022 |  | 16 |
| r | GS022 |  | 22 |
| r | GS022 |  | 33 |
| r | GS022 |  | 34 |
| r | GS022 |  | 63 |
| r | GS022 |  | 73 |
| r | GS022 |  | 83 |
| r | GS022 |  | 471 |
| r | GS022 |  | 524 |
| r | GS022 |  | 552 |
| r | GS022 |  | 560 |
| r | GS022 |  | 564 |
| r | GS022 |  | 568 |
| r | GS022 |  | 571 |
| r | GS022 |  | 573 |
| r | GS022 |  | 580 |
| r | GS022 |  | 608 |
| r | GS022 |  | 609 |
| r | GS022 |  | 127 |
| r | GS022 |  | 354 |
| r | GS022 |  | 204 |
| r | GS022 |  | 206 |
| r | GS022 |  | 700 |
| r | GS022 |  | 104 |
| r | GS022 |  | 289 |
| r | GS022 |  | 299 |
| r | GS022 |  | 309 |
| r | GS022 |  | 313 |
| r | GS022 |  | 332 |
| r | GS022 |  | 344 |
| r | GS022 |  | 133 |
| r | GS022 |  | 173 |
| r | GS022 |  | 282 |
| r | GS022 |  | 350 |
| r | GS022 |  | 435 |
| r | GS022 |  | 62 |
| r | GS022 |  | 238 |
| r | GS022 |  | 243 |
| r | GS022 |  | 784 |
| r | GS022 |  | 80 |
| r | GS022 |  | 92 |
| r | GS022 |  | 116 |
| r | GS022 |  | 140 |
| r | GS022 |  | 164 |
| r | GS022 |  | 168 |
| r | GS022 |  | 391 |
| r | GS022 |  | 440 |
| r | GS022 |  | 596 |
| r | GS022 |  | 190 |
| r | GS022 |  | 207 |
| r | GS022 |  | 138 |
| r | GS022 |  | 167 |
| r | GS022 |  | 175 |
| r | GS022 |  | 238 |
| r | GS022 |  | 275 |
| r | GS022 |  | 327 |
| r | GS022 |  | 371 |
| r | GS022 |  | 373 |
| r | GS022 |  | 379 |
| r | GS022 |  | 482 |
| r | GS022 |  | 52 |
| r | GS022 |  | 82 |
| r | GS022 |  | 107 |
| r | GS022 |  | 119 |
| r | GS022 |  | 132 |
| r | GS022 |  | 424 |
| r | GS022 |  | 60 |
| r | GS022 |  | 70 |
| r | GS022 |  | 10 |
| r | GS022 |  | 19 |
| r | GS022 |  | 20 |
| r | GS022 |  | 24 |
| r | GS022 |  | 28 |
| r | GS022 |  | 279 |
| r | GS022 |  | 89 |
| r | GS022 |  | 96 |
| r | GS022 |  | 3750 |
| r | GS022 |  | 8 |
| r | GS022 |  | 89 |
| r | GS022 |  | 120 |
| r | GS022 |  | 133 |
| r | GS022 |  | 212 |
| r | GS022 |  | 220 |
| r | GS022 |  | 50 |
| r | GS022 |  | 166 |
| r | GS022 |  | 171 |
| r | GS022 |  | 275 |
| r | GS022 |  | 286 |
| r | GS022 |  | 289 |
| r | GS022 |  | 311 |
| r | GS022 |  | 399 |
| r | GS022 |  | 405 |
| r | GS022 |  | 416 |
| r | GS022 |  | 431 |
| r | GS022 |  | 439 |
| r | GS022 |  | 554 |
| r | GS022 |  | 154 |
| r | GS022 |  | 181 |
| r | GS022 |  | 222 |
| r | GS022 |  | 295 |
| r | GS022 |  | 321 |
| r | GS022 |  | 362 |
| r | GS022 |  | 164 |
| r | GS022 |  | 32 |
| r | GS022 |  | 64 |
| r | GS022 |  | 126 |
| r | GS022 |  | 193 |
| r | GS022 |  | 273 |
| r | GS022 |  | 164 |
| r | GS022 |  | 32 |
| r | GS022 |  | 64 |
| r | GS022 |  | 126 |
| r | GS022 |  | 193 |
| r | GS022 |  | 273 |
| M | ? | bot.py.bak_v1 | 858 |
| M | ? | bot.py.bak_v1 | 914 |
| M | ? | bot.py.bak_v1 | 944 |
| M | ? | bot.py.bak_v1 | 949 |
| M | ? | bot.py.bak_v1 | 959 |
| M | ? | bot.py.bak_v1 | 984 |
| M | ? | bot.py.bak_v1 | 985 |
| M | ? | bot.py.bak_v1 | 1103 |
| M | ? | bot.py.bak_v1 | 1604 |
| M | ? | bot.py.bak_v1 | 1679 |
| M | ? | bot.py.bak_v1 | 2160 |
| M | ? | bot.py.bak_v1 | 2504 |
| M | ? | bot.py.bak_v1 | 2550 |
| M | ? | bot.py.bak_v1 | 2579 |
| M | ? | bot.py.bak.audit-20260611 | 791 |
| M | ? | bot.py.bak.audit-20260611 | 847 |
| M | ? | bot.py.bak.audit-20260611 | 863 |
| M | ? | bot.py.bak.audit-20260611 | 883 |
| M | ? | bot.py.bak.audit-20260611 | 888 |
| M | ? | bot.py.bak.audit-20260611 | 898 |
| M | ? | bot.py.bak.audit-20260611 | 922 |
| M | ? | bot.py.bak.audit-20260611 | 923 |
| M | ? | bot.py.bak.audit-20260611 | 1040 |
| M | ? | bot.py.bak.audit-20260611 | 1495 |
| M | ? | bot.py.bak.audit-20260611 | 1572 |
| M | ? | bot.py.bak.audit-20260611 | 1998 |
| M | ? | bot.py.bak.audit-20260611 | 2305 |
| M | ? | bot.py.bak.audit-20260611 | 2351 |
| M | ? | bot.py.bak.audit-20260611 | 2380 |
| M | ? | bot.py | 861 |
| M | ? | bot.py | 917 |
| M | ? | bot.py | 947 |
| M | ? | bot.py | 952 |
| M | ? | bot.py | 962 |
| M | ? | bot.py | 987 |
| M | ? | bot.py | 988 |
| M | ? | bot.py | 1112 |
| M | ? | bot.py | 1619 |
| M | ? | bot.py | 1694 |
| M | ? | bot.py | 2175 |
| M | ? | bot.py | 2519 |
| M | ? | bot.py | 2565 |
| M | ? | bot.py | 2594 |
| M | ? | admin_key_v2.py | 93 |
| M | ? | admin_key_v2.py | 97 |
| M | ? | admin_key_v2.py | 111 |
| M | ? | admin_key.py | 147 |
| M | ? | admin_key.py | 159 |

---
*Сгенерировано GSC v0.6 · 2026-08-04T22:26:14.042912*