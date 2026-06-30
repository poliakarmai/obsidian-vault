---
title: "GSC Audit: /tmp/gsc_scan_targets/WebGenerator"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc_scan_targets/WebGenerator

**Дата:** 29.06.2026 14:22  
**Путь:** `/tmp/gsc_scan_targets/WebGenerator`  
**Всего находок:** 80  
**CRITICAL:** 10 | **HIGH:** 10 | **MEDIUM:** 8 | **LOW:** 51

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 51 |
| Хардкод IP адреса | 7 |
| GS001 | 6 |
| Outdated dependency pattern | 4 |
| GS004 | 3 |
| Синхронный код в async | 3 |
| Hardcoded encryption key | 2 |
| GS005 | 2 |
| Bare except: | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | alembic.ini.j2 | 62 | Found: sqlite:///./app.db
{% endif %}

[po |
| CRITICAL | GS001 | env.j2 | 31 | Found: sqlite:///./app.db
{% endif %}

{% if u |
| CRITICAL | GS001 | tests_conftest.py.j2 | 103 | Found: password="testpassword" |
| CRITICAL | GS001 | tests_conftest.py.j2 | 124 | Found: password="testpassword" |
| CRITICAL | GS001 | config_settings.py.j2 | 28 | Found: sqlite:///{{ project_name }}.db |
| CRITICAL | GS001 | env.j2 | 17 | Found: sqlite:///{{ project_name }}.db
{% endif %}

{% if u |
| CRITICAL | ? | tests_conftest.py.j2 | 103 | Match:         password="testpassword", |
| CRITICAL | ? | tests_conftest.py.j2 | 124 | Match:         password="testpassword", |
| CRITICAL | GS005 | main.py | 481 | Line 481: self.title_label.setText(f"正在生成 {project_name} 项目. |
| CRITICAL | GS005 | main.py | 551 | Line 551: self.title_label.setText(f"已生成 {self.project_name} |
| HIGH | ? | requirements.txt.j2 | 36 | Match: flasgger==0.9.7.1 |
| HIGH | ? | env.j2 | 5 | Match: FLASK_HOST=0.0.0.0 |
| HIGH | ? | run.py.j2 | 19 | Match:         host=os.getenv('FLASK_HOST', '0.0.0.0'), |
| HIGH | ? | Dockerfile.j2 | 32 | Match: CMD ["gunicorn", "--bind", "0.0.0.0:5000", "run:app"] |
| HIGH | ? | core_config.py.j2 | 34 | Match:     SERVER_HOST: str = "0.0.0.0" |
| HIGH | ? | run.py.j2 | 17 | Match:         host=os.getenv('API_HOST', '0.0.0.0'), |
| HIGH | ? | Dockerfile.j2 | 31 | Match: CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0",  |
| HIGH | GS004 | build_package.py | 19 | Line 19: result = subprocess.run(cmd, shell=True, cwd=cwd, c |
| HIGH | GS004 | build_windows_cross.py | 17 | Line 17: result = subprocess.run(cmd, shell=True, cwd=cwd, c |
| HIGH | GS004 | build_windows_simple.py | 17 | Line 17: result = subprocess.run(cmd, shell=True, cwd=cwd, c |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | utils_redis_client.py.j2 | 251 |
| C | GS001 | alembic.ini.j2 | 62 |
| C | GS001 | env.j2 | 31 |
| C | GS001 | tests_conftest.py.j2 | 103 |
| C | GS001 | tests_conftest.py.j2 | 124 |
| C | GS001 | config_settings.py.j2 | 28 |
| C | GS001 | env.j2 | 17 |
| L | GS003 | main.py | 623 |
| L | GS003 | main.py | 1293 |
| L | GS003 | main.py | 1295 |
| L | GS003 | main.py | 1296 |
| L | GS003 | main.py | 1334 |
| L | GS003 | main.py | 1345 |
| L | GS003 | main.py | 1351 |
| L | GS003 | build_package.py | 17 |
| L | GS003 | build_package.py | 21 |
| L | GS003 | build_package.py | 23 |
| L | GS003 | build_package.py | 26 |
| L | GS003 | build_package.py | 31 |
| L | GS003 | build_package.py | 54 |
| L | GS003 | build_package.py | 60 |
| L | GS003 | build_package.py | 64 |
| L | GS003 | build_package.py | 68 |
| L | GS003 | build_package.py | 89 |
| L | GS003 | build_package.py | 91 |
| L | GS003 | build_package.py | 110 |
| L | GS003 | build_windows_cross.py | 15 |
| L | GS003 | build_windows_cross.py | 19 |
| L | GS003 | build_windows_cross.py | 21 |
| L | GS003 | build_windows_cross.py | 24 |
| L | GS003 | build_windows_cross.py | 29 |
| L | GS003 | build_windows_cross.py | 34 |
| L | GS003 | build_windows_cross.py | 39 |
| L | GS003 | build_windows_simple.py | 15 |
| L | GS003 | build_windows_simple.py | 19 |
| L | GS003 | build_windows_simple.py | 21 |
| L | GS003 | build_windows_simple.py | 24 |
| L | GS003 | build_windows_simple.py | 29 |
| L | GS003 | build_windows_simple.py | 33 |
| L | GS003 | build_windows_simple.py | 34 |
| L | GS003 | build_windows_simple.py | 41 |
| L | GS003 | build_windows_simple.py | 43 |
| L | GS003 | build_windows_simple.py | 47 |
| L | GS003 | build_windows_simple.py | 52 |
| L | GS003 | build_windows_simple.py | 55 |
| L | GS003 | build_windows_simple.py | 58 |
| L | GS003 | build_windows_simple.py | 70 |
| L | GS003 | build_windows_simple.py | 76 |
| L | GS003 | build_windows_simple.py | 77 |
| L | GS003 | build_windows_simple.py | 78 |
| L | GS003 | build_windows_simple.py | 86 |
| L | GS003 | build_windows_simple.py | 88 |
| L | GS003 | build_windows_simple.py | 89 |
| L | GS003 | build_windows_simple.py | 90 |
| L | GS003 | build_windows_simple.py | 91 |
| L | GS003 | build_windows_simple.py | 95 |
| L | GS003 | build_windows_simple.py | 101 |
| L | GS003 | build_windows_simple.py | 103 |
| H | ? | requirements.txt.j2 | 36 |
| H | ? | env.j2 | 5 |
| H | ? | run.py.j2 | 19 |
| H | ? | Dockerfile.j2 | 32 |
| H | ? | core_config.py.j2 | 34 |
| H | ? | run.py.j2 | 17 |
| H | ? | Dockerfile.j2 | 31 |
| C | ? | tests_conftest.py.j2 | 103 |
| C | ? | tests_conftest.py.j2 | 124 |
| M | ? | main.py | 609 |
| M | ? | base_generator.py | 285 |
| M | ? | base_generator.py | 286 |
| M | ? | base_generator.py | 292 |
| H | GS004 | build_package.py | 19 |
| H | GS004 | build_windows_cross.py | 17 |
| H | GS004 | build_windows_simple.py | 17 |
| C | GS005 | main.py | 481 |
| C | GS005 | main.py | 551 |
| s | GS009 |  | 0 |
| M | ? | build_package.py | 19 |
| M | ? | build_windows_cross.py | 17 |
| M | ? | build_windows_simple.py | 17 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:22:07.546683*