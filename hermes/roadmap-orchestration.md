---
tags: [hermes, roadmap, orchestration]
created: 2026-06-16
updated: 2026-06-23
---

# Roadmap: Оркестрация Hermes

## ✅ Фаза 1: Базовая оркестрация (16 июня 2026)

| # | Что | Статус |
|---|-----|--------|
| 1 | Вариант В: demo-бот → лёгкий скрипт (86 строк, DeepSeek API) | ✅ |
| 2 | Цепочка ботов: @Apolaibot → @miropolbot → @Morearbot | ✅ |
| 3 | Авто-онбординг после оплаты Stars | ✅ |
| 4 | Skill-sync v3: двухсторонняя + трёхэтапное ревью | ✅ |
| 5 | `hermes-tenant` авто-добавление в `TELEGRAM_ALLOWED_USERS` | ✅ |
| 6 | `memory-preload` + `obsidian-context` | ✅ |
| 7 | Приватный GitHub: `hermes-agent-orchestration` | ✅ |
| 8 | 5 tenant'ов в проде | ✅ |
| 9 | Skill-sync новым тенантам при онбординге | ✅ |
| 10 | Отключение `hermes-gateway-demo` (−155MB RAM) | ✅ |
| 11 | Авто-депровижнинг Pro через 30 дней | ✅ |
| 12 | Алерт админу при новом клиенте | ✅ |
| 13 | Per-tenant rate limiting | ✅ |
| 14 | Панель управления тенантами (HTML дашборд) | ✅ |
| 15 | Аудит-трейл действий тенантов | ✅ |
| 16 | Webhook miropolbot → мгновенный онбординг | ✅ |

## ✅ Фаза 2: Изоляция и надёжность (22-23 июня 2026)

| # | Что | Статус |
|---|-----|--------|
| 17 | Systemd resource limits (MemoryMax/CPUQuota/TasksMax) | ✅ |
| 18 | Token budget (demo=1M, pro=5M, admin=∞) | ✅ |
| 19 | DeepSeek balance monitor | ✅ |
| 20 | Observability: метрики тенантов + дашборд | ✅ |
| 21 | CI/CD для скиллов (4-stage review: validate→security→judge→adversarial) | ✅ |
| 22 | Авто-бэкап профилей тенантов (ежедневно, ротация 7д) | ✅ |
| 23 | Аудит оркестрации: channel_profiles восстановлены, tenant-registry | ✅ |
| 24 | Онбординг D.V. (696238708, uid=1007, песочница, iptables, vault) | ✅ |
| 25 | Cron-оптимизация: 64→59 (−5 мусорных) | ✅ |
| 26 | Age-шифрование 4 профилей, tier cleanup (32 несуществующих скилла) | ✅ |
| 27 | Аудит изоляции: 6 тенантов — 41 skill, tavily+tutu, disabled_toolsets | ✅ |
| 28 | Default-профиль: config.yaml + 41 skill (был 0 — дыра) | ✅ |
| 29 | Публичный лендинг Aegis AI Engine (Linear dark theme) | ✅ |
| 30 | Стриминг включён глобально | ✅ |

## ✅ Фаза 3: Сессии, инварианты, self-healing (23 июня 2026)

| # | Что | Статус |
|---|-----|--------|
| 31 | SIGTERM-хук: авто-сохранение всех сессий в Obsidian перед рестартом | ✅ |
| 32 | Инвариант-чек при старте (tenant-aware, 12 проверок админ / 3 тенант) | ✅ |
| 33 | `memory-preload` → tenant-aware (админ/тенант, загрузка trading/sessions/) | ✅ |
| 34 | `session-summarizer` → тенант-секции (запросы/контекст вместо сделок) | ✅ |
| 35 | `trading/sessions/` во всех 6 tenant vault'ах | ✅ |
| 36 | Cron: `vault-vs-reality-check` (ежедневно 08:00) | ✅ |
| 37 | Meilisearch: `filterableAttributes: [path]`, tenant_prefix изоляция | ✅ |
| 38 | GitHub: `poliakarmai/hermes-orchestrator`, 2 коммита, документация | ✅ |
| 39 | Tenant skills: полный цикл (создание→pull→4-stage review→import→sync) | ✅ |
| 40 | Judge fix: OSError на длинных строках | ✅ |
| 41 | Adversarial review: tenant-aware (не блокирует доменные скиллы) | ✅ |
| 42 | Диск: авто-очистка (бэкапы >7д, pip cache, audio >3д, journal vacuum) | ✅ |
| 43 | DSPy skill-evolution: конфиг + evolve_skill на DeepSeek V4 Pro | ✅ |
| 44 | SHORT SL: +10% + задержка 20 мин (config + auto_short + auto_sl) | ✅ |

## 🔜 Фаза 4: Ближайшие (июль 2026)

| # | Что | Приоритет |
|---|-----|-----------|
| 45 | Тестирование платёжного флоу (реальная оплата Stars → авто-онбординг) | 🥇 |
| 46 | White-label: кастомные боты для B2B-клиентов | 🥈 |
| 47 | Шардинг: горизонтальное масштабирование на 100+ тенантов | 🥉 |
| 48 | Tenant migration: перенос тенанта между серверами | 🥉 |
| 49 | OpenRath-подобный Session объект (fork/merge/replay для multi-agent) | 🔮 |

## 🔮 Бэклог

| # | Что | Метрика |
|---|-----|---------|
| 50 | Grafana/Prometheus для gateway | Мониторинг |
| 51 | Биллинг: автоматические инвойсы, история платежей | Монетизация |
| 52 | CI/CD для скиллов: авто-тестирование при импорте от тенантов | Качество |
| 53 | Публичная документация для продвижения | Рост |
| 54 | RAG: open-notebook (Docker fix) | Продукт |
| 55 | DSPy: переход на GPT-4.1 для реального эффекта оптимизации | ML |

## Архитектурные решения (зафиксированы)

1. **Demo = вариант В** — лёгкий скрипт, не Hermes. Не пересматривать.
2. **Продакшен = один Hermes-гейтвей** — не плодить инстансы без шардинга.
3. **Оплата = Telegram Stars** — не подключать внешние платёжки без явной команды.
4. **Изоляция = 3 слоя** — disabled_toolsets + channel_prompts + Linux users.
5. **Память = Obsidian vault** — не `memory()` Hermes, tenant-aware изоляция.
6. **Сессии = SIGTERM-хук + invariant-check + vault-vs-reality** — самовосстанавливающиеся.
7. **SHORT SL = +10% + задержка 20 мин** — SL не ставится при входе, активируется auto_sl.

## Метрики успеха (цели Q3 2026)

- 20 активных тенантов
- Время онбординга: < 3 минут от оплаты до «/start в @Morearbot»
- Uptime gateway: 99.5%
- Средний расход на тенанта: < $0.03/день
- 0 утечек данных между тенантами
- Сессии не теряются при рестарте
