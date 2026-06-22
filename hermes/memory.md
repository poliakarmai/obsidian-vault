---
tags: [hermes, memory]
updated: 2026-06-19
---

# Техническая память

## Проекты (актуальное состояние)

### bybit-ws
- Фаза 3 завершена: backtest, ML scorer, partial TP, funding rotation, trailing_sl_x10
- Сервис: `bybit-ws-async` (НЕ `bybit-ws.service` — вырублен)
- Тесты: 45/45 PASS
- Дашборд v5.0 (порт 9999)
- AGENTS.md в репо (`~/bybit-ws/AGENTS.md`) — навигация для AI

### Multi-tenant Hermes
- 7 профилей: default (Море), demo, user_1148002325, user_2115597720 (Колесников), user_308591502, user_470549555 (Илья), user_5529208670
- Cron для тенантов: ✳️ папок cron/ у тенантов нет — работают в рамках gateway с disabled_toolsets
- Gateway: active since Jun 17

### VPN
- Xray: скорее всего через другой механизм (не systemd user unit)
- VPN-бот: masked (выключен намеренно)

### Промышленная тема
- Претензия по линейке: составлена, сохранена в `акты-бнгкм/`
- Кейсбук «ИИ в ТЭК»: сохранён в Obsidian
- Тезисы-2026: в работе

## LLM & Инструменты
- DeepSeek V4 Pro (deepseek-v4-pro) для всех вызовов
- Judge: прямой вызов DeepSeek API, max_tokens=2000, timeout=30с
- FreeLLMAPI: ~/freellmapi, port 3001, systemd
- TTS: всегда русский, голос Дмитрий (ru-RU-DmitryNeural)

## Сервер
- Хельсинки, Финляндия (2.27.48.142)
- SSH: порт 2091, пользователь openclaw, password auth ✅
- 1.9GB RAM, своп 2GB — критично экономить память
- Все systemd-сервисы — user-level

## Веб-интерфейсы Hermes
- **Dashboard:** `http://127.0.0.1:9119` (сервис hermes-dashboard, enabled, автостарт)
  - Скиллы, конфиг, API-ключи, сессии, статус компонентов
  - Доступ снаружи: `ssh -L 9119:127.0.0.1:9119 -p 2091 openclaw@2.27.48.142`
- **Command Center (свой):** `http://2.27.48.142:9998/chat.html` (чат) и `/dashboard.html` (устарел)
  - Сервис hermes-chat, порт 9998, слушает 0.0.0.0
- **Веб-чат (fallback):** `http://2.27.48.142:9999/chat.html` (bybit-ws дашборд)

## Отправка файлов
- MEDIA:/path в тексте ответа — доставляет в текущий чат
- send_message — только когда явно сказано «отправь в канал X»

## Правила пользователя
- Не слать approved-запросы — исполнять без подтверждений
- GitHub push только через cron github-weekly-push (пн 10:00), не вручную
- **memory() Hermes ОТКЛЮЧЕНА НАВСЕГДА** — только Obsidian vault через write_file/patch

## Онбординг новых клиентов — ОБЯЗАТЕЛЬНАЯ ПРОВЕРКА
После `hermes-tenant onboard` всегда проверять:
1. `TELEGRAM_ALLOWED_USERS` в `.env` — добавить новый tg_id
2. `channel_profiles` в `config.yaml` — маппинг tg_id → профиль
3. `channel_prompts` в `config.yaml` — системный промпт
4. После правок — `systemctl --user restart hermes-gateway`
