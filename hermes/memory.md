---
tags: [hermes, memory]
updated: 2026-06-24
---

# Техническая память

## Конфиг Hermes (24.06.2026)
- `approvals.mode: auto` — больше никаких pending_approval
- `max_concurrent_sessions: 3` — защита от Broken pipe на DeepSeek
- `cron.max_parallel_jobs: 3` — параллельные cron'ы не душат API
- ⚠️ Рестарт gateway обязателен для применения! `hermes gateway restart`

## Проекты

### bybit-ws
- Сервис: `bybit-ws-async`
- Дашборд v5.0 (порт 9999)
- AGENTS.md: `~/bybit-ws/AGENTS.md`
- **RPC /move_sl (24.06.2026):** добавлен endpoint для передвижения SL без credential scanner
- SUI SL: $0.6307 → $0.58

### PCI Bot (24.06.2026)
- **Остановлен и отключён.** Был бесконечный restart loop (65K раз, нет токена)
- Сервис: system-level `/etc/systemd/system/pci-bot.service`
- Проект: `~/pci-index/` — крипто-индекс, не используется

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
