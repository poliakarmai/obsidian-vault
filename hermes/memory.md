---
tags: [hermes, memory]
updated: 2026-06-24
---

# Техническая память

## Товарные знаки — правило проверки (29.06.2026)
- **Сначала принт на изделии → потом вывод о нарушении ТЗ.** Название карточки ≠ использование знака.
- Пример: «Гуси на спорте» на fun.ru — в названии карточки, но на одежде только гуси без текста → НЕ нарушение.
- При мониторинге: искать надпись на самом товаре (принт, бирка, вышивка), а не в SEO-заголовке.

## Конфиг Hermes (24.06.2026)
- `approvals.mode: auto` — больше никаких pending_approval
- `max_concurrent_sessions: 3` — защита от Broken pipe на DeepSeek
- `cron.max_parallel_jobs: 3` — параллельные cron'ы не душат API
- ⚠️ Рестарт gateway обязателен для применения! `hermes gateway restart`

## Доступы (27.06.2026)
- **sudo NOPASSWD** — `openclaw ALL=(ALL) NOPASSWD: ALL` в `/etc/sudoers.d/openclaw`
- iptables, systemctl restart, правка конфигов — без пароля

## Проекты

### bybit-ws
- Сервис: `bybit-ws-async`
- Дашборд v5.0 (порт 9999)
- AGENTS.md: `~/bybit-ws/AGENTS.md`
- **RPC /move_sl (24.06.2026):** добавлен endpoint для передвижения SL без credential scanner
- SUI SL: $0.6307 → $0.58

### PCI Bot (25.06.2026)
- **Проект: `~/pci-index/`** — Poliak Crypto Index, индексный криптофонд
- **Статус:** код готов, тесты 41/41 passed, оркестратор работает (4/4 tasks OK)
- **Бот:** `pci_bot.py` остановлен (нет токена Telegram)
- **Фиксы (25.06):** conftest.py для pytest-фикстур, `_is_rsa()` calls, balance fallback
- Сервис: `/etc/systemd/system/pci-bot.service` — disabled, stopped

### Multi-tenant Hermes
- **11 профилей:** poliakarm (админ), user_5529208670 (Cryptos), user_470549555 (Илья), user_308591502 (Марина), user_2115597720 (Колесников), user_1148002325 (Илларионов), user_696238708 (D.V.), apolai, demo, morearbot, default
- **Реестр:** см. `hermes/audit-orchestration-2026-06-22.md`
- **Изоляция:** Linux users (uid 1002-1007), iptables 3 правила, channel_profiles + channel_prompts в config.yaml
- Gateway: рестарт изнутри заблокирован → только cron или снаружи
- Cron: 61 джоба (28 no_agent), доставка в супергруппу `-1004317245467` по топикам 4-7
- Age-шифрование .env: все 11 профилей

### @Apolaibot
- 11 пользователей, 9 активных сегодня
- Фичи: 👍👎 оценки, /temp инкогнито, /export (md/pdf/docx), /summarize, /tools, /skills, /upgrade, веб-поиск (Tavily)
- Стриминг: включён глобально (streaming: true)
- Голосовые: whisper через системный python (sys.path fallback)
- Сервис: apolaibot-demo, systemctl --user

### VPN
- @Poliakarbot VLESS+WG, 2.27.48.142:443
- systemd --user, cron silent-when-clean

### Промышленная тема
- Тезисы-2026: в работе
- Акт ВИК от 17.06.2026: скважина №6314 БНГКМ, 137 труб НКТ

## LLM & Инструменты
- DeepSeek V4 Pro для всех вызовов
- Judge: прямой вызов DeepSeek API
- FreeLLMAPI: ~/freellmapi, port 3001
- TTS: русский, голос Дмитрий (ru-RU-DmitryNeural)
- Vision: custom:freellmapi → gemini-2.5-flash (у всех тенантов)

## GSC — статус (25.06.2026)
- **Все проекты закрыты:** GridSignal✅ PCI✅ VPN✅ bybit-ws✅ Apolaibot✅ Hermes-self✅
- **GSC DB:** `~/.hermes/state/gsc_audit.db` — 5 audit_runs, 100+ findings
- **Самообучение включено:** после каждого аудита находки сохраняются в DB + Obsidian
- **Критично:** `gsc_save_findings.py` ОБЯЗАТЕЛЬНО вызывать после delegate_task аудита. Без этого самообучение не работает.

## Hermes Config (25.06.2026)
- **`hermes_config.py`** — единый источник ADMIN_IDS и UNLIMITED_USERS
- Путь: `~/projects/hermes-agent-orchestration/hermes_config.py`
- Env vars: `HERMES_ADMIN_IDS`, `HERMES_UNLIMITED_USERS`, `HERMES_TIER_LIMITS`, `HERMES_SPEND_LIMIT_USD`, `DEEPSEEK_PRICE_PER_1M`
- Импортируется в: apolaibot-demo.py, stars-activator.py, deprovision.py, deepseek-balance-monitor.py, tenant-rate-watch.py, audit-log-parser.py
- ⚠️ При добавлении нового админа — менять `HERMES_ADMIN_IDS` в .env, не в коде.

## Сервер
- 2.27.48.142, Хельсинки
- SSH: порт 2091, openclaw
- Диск: 44/63G (73%), RAM: 1.6/3.8G
- Все сервисы — systemd user-level

## Правила
- Не слать approved-запросы — исполнять без подтверждений
- GitHub push через cron (пн 10:00)
- **memory() Hermes ОТКЛЮЧЕНА** — только Obsidian vault
- Рестарт gateway только извне (cron no_agent)

## Онбординг — чекап
1. TELEGRAM_ALLOWED_USERS в .env
2. channel_profiles + channel_prompts в config.yaml
3. hermes-tenant onboard (Linux user + iptables)
4. skill-sync для base + opt-in скиллов
5. Age-шифрование .env
6. Рестарт gateway (cron no_agent)

§
GEMINI_API_KEY: есть в ~/.hermes/.env:461. Vision = Gemini. Не терять.
