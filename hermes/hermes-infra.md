---
tags: [hermes, infra, multi-tenant]
---

# Hermes Infrastructure

## Версия
- v0.16.0 (upstream 56236b16)
- Streaming + typing indicator для Telegram

## Архитектурное решение (22.06.2026)
- **Demo-тенант → @Apolaibot:** кастомный скрипт-бот (621 строка, 62MB RAM, DeepSeek API)
- **Продакшен (Morearbot):** полноценный Hermes-гейтвей (~200MB)
- **Причина:** 90% лидам нужен только чат + /upgrade, незачем тащить MCP, терминал

### Цепочка ботов
```
Пользователь → @Apolaibot (demo, 62MB) → 10 команд
                                            → /upgrade → @miropolbot (оплата Stars, 10MB)
                                            → авто-онбординг (stars-activator, cron 2min)
                                            → @Morearbot (полный Hermes, 200MB)
```

| Бот | Тип | RAM | Функция |
|-----|-----|-----|---------|
| @Apolaibot | Скрипт (python-telegram-bot) | 62MB | Демо: каталог, онбординг, 2FA, summarize, export, temp, tools, feedback |
| @miropolbot | Скрипт (polling) | 10MB | Оплата Telegram Stars |
| @Morearbot | Hermes Gateway | 200MB | Полный доступ (Pro) |

## Новые скрипты (22.06.2026)

| Скрипт | Фаза | Назначение |
|--------|------|-----------|
| `agent_fs.py` | 1 | Агентская ФС: версионирование, локинг, audit trail |
| `skill_sandbox.py` | 1 | Podman-песочница для кода |
| `billing.py` | 2 | 4 тарифа, организации, промокоды |
| `tenant_features.py` | 2 | Каталог, фидбек, бюджет для тенантов |
| `user_skills.py` | 3 | Пользовательские скиллы |
| `team_vault.py` | 3 | Командный vault + BM25-поиск |
| `doc_export.py` | 3 | MD→PDF/DOCX/XLSX |
| `agent_queue.py` | 4 | Очередь агентов FIFO |
| `cloud_mirror.py` | 4 | Облачное зеркало папки |
| `health_dashboard.py` | 5 | Мониторинг сервисов |
| `whitelabel.py` | 5 | Брендинг тенантов |

## Multi-tenant
- ОДИН агент, ОДИН бот, ОДИН процесс (продакшен)
- Роутинг: channel_prompts + channel_profiles в config.yaml
- Профили в ~/.hermes/profiles/<name>/
- Изоляция: 5 слоёв (терминал, статика, код, рантайм, аудит)

## Патч gateway/run.py (06.06.2026)
- profile-specific disabled_toolsets
- Файл: ~/.hermes/hermes-agent/gateway/run.py
- Строка: "profile-specific disabled_toolsets"
- При обновлении Hermes может слететь — переприменить

## Cron
- Canary-watch: раз в 12ч, silent
- Cost-tracking: pnl-morning 09:00, cost-weekly пн 10:00
- GitHub push: пн 10:00
- tenant-health-check

## Профили
- default (Поляков) — полный доступ
- user_470549555 (Илья) — disabled: delegation, code_execution
- user_5529208670 (Cryptos)
- user_308591502, user_2115597720, user_1148002325
- poliakarm, apolai, demo, morearbot
