# Аудит оркестрации — 22.06.2026

## Проблемы найдены
- `channel_profiles` отсутствовал в config.yaml → все тенанты без изоляции
- `channel_prompts` пустые → tenant'ы не знали своих песочниц
- 9 профилей без age-шифрования .env
- 7 cron-джоб с избыточной частотой (≤5 мин)
- `skill-sync.py --install` сломан (cmd_install без def)
- 32 несуществующих скилла в tiers
- 2 дублирующих watchdog'а (bybit, telegram)

## Исправлено
- channel_profiles: восстановлен из снапшота 21.06.2026 (7 tg_id)
- channel_prompts: 7 кастомных инструкций
- Age-шифрование: 4 профиля (apolai, demo, morearbot, 696238708)
- skill-sync fix: добавлен `def cmd_install()`
- Tiers: 54→41 base, 62→46 admin, 24→21 opt-in
- Cron: 7 джоб урезаны (−67% запусков)
- Watchdog'и: bybit + telegram отключены
- Gateway: рестарт в 17:00

## Онбординг D.V. (696238708)
- hermes-dv uid=1007
- Песочница /home/hermes-dv/ (770)
- iptables 3 правила
- Obsidian vault
- ≈194 скилла (без trading)
- pro tier (20M токенов)

## Реестр тенантов (22.06.2026)
| tg_id | Кто | Профиль | Linux user | UID | Tier |
|---|---|---|---|---|---|
| 319665243 | Поляков Алексей | poliakarm | openclaw | 1000 | pro |
| 5529208670 | Cryptos | user_5529208670 | hermes-cryptos | 1002 | demo |
| 470549555 | Илья | user_470549555 | hermes-ilya | 1003 | demo |
| 308591502 | Марина | user_308591502 | hermes-marina | 1004 | demo |
| 2115597720 | Колесников | user_2115597720 | hermes-kolesnikov | 1005 | demo |
| 1148002325 | Костя Илларионов | user_1148002325 | hermes-illarionov | 1006 | demo |
| 696238708 | D.V. (@mr_yk3) | user_696238708 | hermes-dv | 1007 | pro |

Боты: @Apolaibot (apolai), @Morearbot (morearbot), demo-бот (demo)

## В бэклоге
- Cron per-profile изоляция (тул не пробрасывает профиль)
- Платёжный флоу Stars (не протестирован — нет платежей)
- 3 скилла не в базе: openhue, tezisy-polyakov-2026, ideation
