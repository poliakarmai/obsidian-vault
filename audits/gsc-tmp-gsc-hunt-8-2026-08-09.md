---
title: "GSC Audit: /tmp/gsc-hunt-8"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-8

**Дата:** 09.08.2026 09:53  
**Путь:** `/tmp/gsc-hunt-8`  
**Всего находок:** 37  
**CRITICAL:** 2 | **HIGH:** 9 | **MEDIUM:** 0 | **LOW:** 7

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 10 |
| GS012 | 6 |
| GS036-redos | 5 |
| GS015 | 3 |
| GS025-eval_usage | 3 |
| YAML-36ACF0AD | 3 |
| GS022 | 2 |
| GS001 | 1 |
| GS003 | 1 |
| GS020 | 1 |
| GS036-high_risk | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | secret_settings.template | 8 | Found: PASSWORD = '<MySQL user password>' |
| CRITICAL | GS000-LEGACY | fields.py | 102 | Match:         super(UncertainDateFormField, self).__init__( |
| HIGH | GS000-LEGACY | views.py | 457 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 474 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 490 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | forms.py | 85 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | forms.py | 105 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 63 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 443 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 449 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 452 | File upload without MIME-type validation → malicious file up |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS000-LEGACY | views.py | 457 |
| H | GS000-LEGACY | views.py | 474 |
| H | GS000-LEGACY | views.py | 490 |
| H | GS000-LEGACY | forms.py | 85 |
| H | GS000-LEGACY | forms.py | 105 |
| H | GS000-LEGACY | models.py | 63 |
| H | GS000-LEGACY | models.py | 443 |
| H | GS000-LEGACY | models.py | 449 |
| H | GS000-LEGACY | models.py | 452 |
| C | GS001 | secret_settings.template | 8 |
| L | GS003 | jquery.tablesorter.min.js | 3 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 10 |
| i | GS020 |  | 4 |
| ? | GS036-redos | jquery.tablesorter.min.js | 4 |
| ? | GS036-redos | jquery.tablesorter.min.js | 4 |
| ? | GS036-redos | jquery.tablesorter.min.js | 4 |
| ? | GS036-redos | jquery.tablesorter.min.js | 4 |
| ? | GS036-redos | jquery.tablesorter.min.js | 4 |
| ? | GS036-high_risk | jquery.tablesorter.min.js | 1 |
| C | GS000-LEGACY | fields.py | 102 |
| s | GS009 |  | 0 |
| L | GS012 | forms.py | 105 |
| L | GS012 | models.py | 449 |
| L | GS012 | models.py | 452 |
| L | GS012 | views.py | 457 |
| L | GS012 | views.py | 474 |
| L | GS012 | views.py | 490 |
| r | GS022 |  | 65 |
| r | GS022 |  | 393 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | jquery.tablesorter.min.js | ? |
| ? | YAML-36ACF0AD | jquery.tagcloud.js | ? |
| ? | YAML-36ACF0AD | tablesorterextra.js | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-09T09:53:57.398916*