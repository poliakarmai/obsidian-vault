---
title: "GSC Audit: /tmp/supplier-product-search"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/supplier-product-search

**Дата:** 10.08.2026 14:02  
**Путь:** `/tmp/supplier-product-search`  
**Всего находок:** 47  
**CRITICAL:** 9 | **HIGH:** 4 | **MEDIUM:** 1 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS015 | 26 |
| GS000-LEGACY | 10 |
| GS019 | 3 |
| GS037-hardcoded_password | 2 |
| GS022 | 2 |
| GS018 | 1 |
| GS009 | 1 |
| GS025-eval_usage | 1 |
| YAML-36ACF0AD | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS000-LEGACY | main.py | 83 | Match:     seller_name: str = Field(min_length=2, max_length |
| CRITICAL | GS000-LEGACY | main.py | 84 | Match:     region: str = Field(min_length=1, max_length=80) |
| CRITICAL | GS000-LEGACY | main.py | 85 | Match:     price_type: str = Field(min_length=1, max_length= |
| CRITICAL | GS000-LEGACY | main.py | 86 | Match:     items: list[BasketItem] = Field(min_length=1, max |
| CRITICAL | GS000-LEGACY | main.py | 98 | Match:     region: str = Field(min_length=1, max_length=80) |
| CRITICAL | GS000-LEGACY | main.py | 99 | Match:     price_type: str = Field(min_length=1, max_length= |
| CRITICAL | GS000-LEGACY | main.py | 100 | Match:     product_ids: list[int] = Field(min_length=1, max_ |
| CRITICAL | GS019 | set_demo_password.py | 21 | Session/JWT secret hardcoded in source. Anyone with code acc |
| CRITICAL | GS019 | set_demo_password.py | 22 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | GS000-LEGACY | build_embeddings.py | 63 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | build_embeddings.py | 64 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | export.py | 134 | File upload without MIME-type validation → malicious file up |
| HIGH | GS019 | main.py | 151 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS018 | export.py | 48 |
| H | GS000-LEGACY | build_embeddings.py | 63 |
| H | GS000-LEGACY | build_embeddings.py | 64 |
| H | GS000-LEGACY | export.py | 134 |
| I | GS015 | main.py | 131 |
| I | GS015 | main.py | 143 |
| I | GS015 | main.py | 150 |
| I | GS015 | main.py | 175 |
| I | GS015 | main.py | 181 |
| I | GS015 | main.py | 198 |
| I | GS015 | main.py | 218 |
| I | GS015 | main.py | 240 |
| I | GS015 | main.py | 131 |
| I | GS015 | main.py | 143 |
| I | GS015 | main.py | 150 |
| I | GS015 | main.py | 175 |
| I | GS015 | main.py | 181 |
| I | GS015 | main.py | 198 |
| I | GS015 | main.py | 218 |
| I | GS015 | main.py | 240 |
| I | GS015 | main.py | 131 |
| I | GS015 | main.py | 143 |
| I | GS015 | main.py | 150 |
| I | GS015 | main.py | 175 |
| I | GS015 | main.py | 181 |
| I | GS015 | main.py | 198 |
| I | GS015 | main.py | 218 |
| I | GS015 | main.py | 240 |
| I | GS015 | main.py | 118 |
| I | GS015 | main.py | 65 |
| ? | GS037-hardcoded_password | set_demo_password.py | 21 |
| ? | GS037-hardcoded_password | set_demo_password.py | 22 |
| C | GS000-LEGACY | main.py | 83 |
| C | GS000-LEGACY | main.py | 84 |
| C | GS000-LEGACY | main.py | 85 |
| C | GS000-LEGACY | main.py | 86 |
| C | GS000-LEGACY | main.py | 98 |
| C | GS000-LEGACY | main.py | 99 |
| C | GS000-LEGACY | main.py | 100 |
| s | GS009 |  | 0 |
| H | GS019 | main.py | 151 |
| C | GS019 | set_demo_password.py | 21 |
| C | GS019 | set_demo_password.py | 22 |
| r | GS022 |  | 529 |
| r | GS022 |  | 536 |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | app.js | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-10T14:02:44.102846*