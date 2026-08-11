---
title: "GSC Audit: /tmp/gsc-learn/redis-py"
date: 2026-08-02
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/redis-py

**Дата:** 02.08.2026 04:01  
**Путь:** `/tmp/gsc-learn/redis-py`  
**Всего находок:** 136  
**CRITICAL:** 0 | **HIGH:** 15 | **MEDIUM:** 13 | **LOW:** 107

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 84 |
| GS008 | 19 |
| CVE-2026-54696: Buffer overflow | 8 |
| eval() or exec() usage | 8 |
| GS002 | 2 |
| GS012 | 2 |
| Синхронный код в async | 2 |
| Bare except: | 1 |
| Python: assert in production | 1 |
| Хардкод IP адреса | 1 |
| Outdated dependency pattern | 1 |
| World-readable file: codecov.yml (664) | 1 |
| World-readable file: docker-compose.yml (664) | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| GS007 | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS014 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| HIGH | ? | docker-compose.yml | 170 | Match:       LISTEN_HOST: "0.0.0.0" |
| HIGH | ? | cluster.py | 3714 | Match:     def eval(self): |
| HIGH | ? | cluster.py | 3716 | Match:         return self._execution_strategy.eval() |
| HIGH | ? | cluster.py | 3998 | Match:     def eval(self): |
| HIGH | ? | cluster.py | 4102 | Match:     def eval(self): |
| HIGH | ? | cluster.py | 4104 | Match:         raise RedisClusterException("method eval() is |
| HIGH | ? | core.py | 11195 | Match:     def eval( |
| HIGH | ? | core.py | 11203 | Match:     def eval( |
| HIGH | ? | core.py | 11210 | Match:     def eval( |
| HIGH | ? | codecov.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | sentinel.conf | 0 | File sentinel.conf has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | credentials.py | 0 | File credentials.py has permissions -rw-rw-r-- — readable by |
| HIGH | GS007 | hybrid_query.py | 228 | Line 228: self._method = method |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | CHANGES | 545 |
| M | ? | connection.py | 1348 |
| M | ? | hiredis.py | 233 |
| M | ? | hiredis.py | 235 |
| M | ? | hiredis.py | 240 |
| M | ? | hiredis.py | 242 |
| M | ? | hiredis.py | 353 |
| M | ? | hiredis.py | 355 |
| M | ? | hiredis.py | 360 |
| M | ? | hiredis.py | 362 |
| L | GS003 | basic_operations.py | 55 |
| L | GS003 | basic_operations.py | 56 |
| L | GS003 | basic_operations.py | 57 |
| L | GS003 | basic_operations.py | 58 |
| L | GS003 | cluster_async.py | 181 |
| L | GS003 | cluster_async.py | 189 |
| L | GS003 | cluster_async.py | 191 |
| L | GS003 | cluster_async.py | 192 |
| L | GS003 | cluster_async.py | 193 |
| L | GS003 | cluster_async.py | 194 |
| L | GS003 | cluster_async.py | 195 |
| L | GS003 | cluster_async.py | 196 |
| L | GS003 | cluster_async.py | 198 |
| L | GS003 | cluster_async.py | 199 |
| L | GS003 | cluster_async.py | 200 |
| L | GS003 | cluster_async.py | 201 |
| L | GS003 | cluster_async.py | 218 |
| L | GS003 | cluster_async.py | 219 |
| L | GS003 | cluster_async.py | 229 |
| L | GS003 | cluster_async.py | 230 |
| L | GS003 | cluster_async.py | 243 |
| L | GS003 | cluster_async.py | 244 |
| L | GS003 | cluster_async_pipeline.py | 66 |
| L | GS003 | cluster_async_pipeline.py | 67 |
| L | GS003 | cluster_async_pipeline.py | 77 |
| L | GS003 | cluster_async_pipeline.py | 78 |
| L | GS003 | cluster_async_pipeline.py | 91 |
| L | GS003 | cluster_async_pipeline.py | 92 |
| L | GS003 | otel_benchmark.py | 294 |
| L | GS003 | otel_benchmark.py | 333 |
| L | GS003 | otel_benchmark.py | 596 |
| L | GS003 | otel_benchmark.py | 633 |
| L | GS003 | otel_benchmark.py | 704 |
| L | GS003 | otel_benchmark.py | 705 |
| L | GS003 | otel_benchmark.py | 706 |
| L | GS003 | otel_benchmark.py | 708 |
| L | GS003 | otel_benchmark.py | 709 |
| L | GS003 | otel_benchmark.py | 710 |
| L | GS003 | otel_benchmark.py | 711 |
| L | GS003 | otel_benchmark.py | 712 |
| L | GS003 | otel_benchmark.py | 713 |
| L | GS003 | otel_benchmark.py | 714 |
| L | GS003 | otel_benchmark.py | 715 |
| L | GS003 | otel_benchmark.py | 716 |
| L | GS003 | otel_benchmark.py | 717 |
| L | GS003 | otel_benchmark.py | 718 |
| L | GS003 | otel_benchmark.py | 720 |
| L | GS003 | otel_benchmark.py | 723 |
| L | GS003 | otel_benchmark.py | 725 |
| L | GS003 | otel_benchmark.py | 727 |
| L | GS003 | otel_benchmark.py | 729 |
| L | GS003 | otel_benchmark.py | 731 |
| L | GS003 | otel_benchmark.py | 732 |
| L | GS003 | otel_benchmark.py | 860 |
| L | GS003 | otel_benchmark.py | 867 |
| L | GS003 | otel_benchmark.py | 880 |
| L | GS003 | otel_benchmark.py | 916 |
| L | GS003 | otel_benchmark.py | 923 |
| L | GS003 | otel_benchmark.py | 936 |
| L | GS003 | otel_benchmark.py | 1159 |
| L | GS003 | otel_benchmark.py | 1170 |
| L | GS003 | otel_benchmark.py | 1171 |
| L | GS003 | otel_benchmark.py | 1175 |
| L | GS003 | otel_benchmark.py | 1176 |
| L | GS003 | otel_benchmark.py | 1178 |
| L | GS003 | otel_benchmark.py | 1180 |
| L | GS003 | otel_benchmark.py | 1181 |
| L | GS003 | otel_benchmark.py | 1182 |
| L | GS003 | otel_benchmark.py | 1183 |
| L | GS003 | otel_benchmark.py | 1184 |
| L | GS003 | otel_benchmark.py | 1185 |
| L | GS003 | otel_benchmark.py | 1186 |
| L | GS003 | otel_benchmark.py | 1187 |
| L | GS003 | otel_benchmark.py | 1200 |
| L | GS003 | otel_benchmark.py | 1206 |
| L | GS003 | otel_benchmark.py | 1219 |
| L | GS003 | otel_benchmark.py | 1224 |
| L | GS003 | otel_benchmark.py | 1230 |
| L | GS003 | otel_benchmark.py | 1237 |
| L | GS003 | otel_benchmark.py | 1248 |
| L | GS003 | otel_benchmark.py | 1253 |
| L | GS003 | otel_benchmark.py | 1259 |
| L | GS003 | otel_benchmark.py | 1266 |
| L | GS003 | tasks.py | 90 |
| L | GS008 | _defaults.py | 8 |
| L | GS008 | _defaults.py | 9 |
| L | GS008 | _defaults.py | 37 |
| L | GS008 | _defaults.py | 38 |
| L | GS008 | _defaults.py | 39 |
| L | GS008 | connection.py | 124 |
| L | GS008 | http_client.py | 8 |
| L | GS008 | http_client.py | 9 |
| L | GS008 | http_client.py | 10 |
| L | GS008 | healthcheck.py | 44 |
| L | GS008 | client.py | 104 |
| L | GS008 | commands.py | 46 |
| L | GS008 | dialect.py | 3 |
| L | GS008 | himport.py | 47 |
| L | GS008 | himport.py | 49 |
| L | GS008 | himport.py | 50 |
| L | GS008 | circuit.py | 7 |
| L | GS008 | attributes.py | 52 |
| L | GS008 | attributes.py | 53 |
| H | ? | docker-compose.yml | 170 |
| M | ? | tasks.py | 30 |
| H | ? | cluster.py | 3714 |
| H | ? | cluster.py | 3716 |
| H | ? | cluster.py | 3998 |
| H | ? | cluster.py | 4102 |
| H | ? | cluster.py | 4104 |
| H | ? | core.py | 11195 |
| H | ? | core.py | 11203 |
| H | ? | core.py | 11210 |
| H | ? | codecov.yml | 0 |
| H | ? | docker-compose.yml | 0 |
| H | ? | .readthedocs.yml | 0 |
| H | GS002 | sentinel.conf | 0 |
| H | GS002 | credentials.py | 0 |
| H | GS007 | hybrid_query.py | 228 |
| s | GS009 |  | 0 |
| L | GS011 | token.py | 89 |
| L | GS012 | cluster.py | 3952 |
| L | GS012 | cluster.py | 3226 |
| L | GS014 | credentials.py | 1 |
| M | ? | otel_benchmark.py | 862 |
| M | ? | otel_benchmark.py | 918 |

---
*Сгенерировано GSC v0.6 · 2026-08-02T04:01:11.387210*