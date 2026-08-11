---
tags: [hermes, memory]
updated: 2026-08-11
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

## Доступы

### GitHub (10.08.2026 — НЕ ЗАБЫВАТЬ)
- **Ты подключён к GitHub!** Аккаунт `poliakarmai` (Alexey Polyakov, Armyanao@gmail.com)
- `gh` CLI авторизован, токен с полным скоупом (repo, workflow, admin:org, copilot, ...)
- `GITHUB_TOKEN` в `~/.hermes/.env`
- GSC, bybit-ws, hermes-orchestration, obsidian-vault — все репы под этим аккаунтом
- Никогда не спрашивать «подключён ли ты к GitHub» — ты подключён всегда

### Системные (27.06.2026)
- **sudo NOPASSWD** — `openclaw ALL=(ALL) NOPASSWD: ALL` в `/etc/sudoers.d/openclaw`
- iptables, systemctl restart, правка конфигов — без пароля

## Проекты

### bybit-ws
- Сервис: `bybit-ws-async`
- Дашборд v5.0 (порт 9999)
- AGENTS.md: `~/bybit-ws/AGENTS.md`
- **RPC /move_sl (24.06.2026):** добавлен endpoint для передвижения SL без credential scanner
- SUI SL: $0.6307 → $0.58
- **⚠️ RPC-токен ОБЯЗАТЕЛЕН (10.08.2026):** ВСЕ запросы к `http://127.0.0.1:8766` требуют Bearer-токен. Токен: `sqlite3 ~/.local/share/bybit-ws/state.db "SELECT value FROM kv_store WHERE key='rpc_auth_token';"`. Без токена — 401 и пустой ответ. Никогда не докладывать «0 позиций» без проверки с токеном — врать будешь.

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
- Cron: 61 джоба (28 no_agent), доставка в супергруппу `-1004317245467` по топикам 4-7. Сокращено с 69 (09.08.2026): GSC 6→4, Vietnam 5→3, Backups 4→2.
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

## GSC — статус (09.08.2026)
- **Hall of Fame:** 3 реальные находки — aiohttp-security#1005 (CWE-384), django-ca#202 (CWE-918), Baobab#1401 (CWE-798)
- **Precision-hunt:** 32 активных детектора, 1 disabled (GS000), 6 review-only. Hunter v4 с edu-layer
- **PyPI:** `pip install gsc-security` — v1.3.0 опубликован. Имя `gsc` было занято.
- **VS Code:** расширение готово (gsc-security-1.0.0.vsix), ждёт Azure PAT для Marketplace
- **Самообучение:** batch revalidate 50 находок/ночь + federated submit (DP ε=1.0) — nightly cron в 04:00
- **Охотник:** cron e6e3dc0016ef, 07:00 MSK, v4 Educational — PR с what/why/when/how
- **DB:** `~/.hermes/state/gsc_audit.db` — 461K findings, 217 проектов, 237 ревалидировано
- **Скиллы Hermes:** architectural-audit, antivibe (из AntiVibe)

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
- **memory() Hermes ОТКЛЮЧЕНА 09.08.2026** — только Obsidian vault. `memory_enabled: false`, `user_profile_enabled: false`
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

## 2026-08-10

- **Отчёт аудита системы и тенантов**: пользователь провёл детальный аудит, выявил и задокументировал проблемы/решения по тенантам (детали не сохранены, но факт аудита зафиксирован).
- **Курс по AI-агентам**: проходил обучение с «подвохом» — вероятно, разбор ошибок/ловушек в агентах; предпочтение — практические кейсы с разбором.
- **Открытые торговые позиции**: вёл анализ/управление торговыми позициями (вероятно, крипто/акции), решения по сделкам принимались в этой сессии.
- **GSC Cloud**: подтверждена полная готовность конфигурации GSC Cloud (Google Search Console?) — финальная проверка пройдена, система работает.
- **Проверка системы и контекста**: выполнена диагностика окружения, подтверждена работоспособность контекста (без критичных багов).

## 2026-08-11

### Системный аудит
- Диск 68%, RAM 1.9G free, Swap 1.8/4G. 19 сервисов running, 0 failed.
- Docker: 4 контейнера healthy (cloud-api, gsc-api, cloud-redis, cloud-postgres).
- GSC API v1.3.0 живой на порту 8001 (не 8081!), 36 детекторов.
- VPN: порты слушают, 12 активных подключений. НО vpn-seller-bot inactive.
- Трейдинг: 5 LONG, все в минусе (-$88 суммарно). Self-learn: 170 трейдов, WR 19.8%, PnL -$143.

### GSC — фикс реакций (коммит f771fd9, запушен)
- **Проблема:** gsc_reactions.py падал с 404 — comment_id всегда был 0.
- **Корень:** хантер постит сканы в тело PR (не в комментарий). `upsert_comment()` возвращал ID, но никто не ловил. `upsert_published_comment()` — мёртвый код.
- **Фикс 1:** `gsc_github_adapter.py:544` — ловим comment_id, пишем в БД.
- **Фикс 2:** `gsc_reactions.py` — для comment_id=0 → reactions самого PR/issue вместо /comments/0/reactions.
- **Крон:** 6e812dc603d8, 04:30 MSK — подхватит завтра.

### VPN
- Xray конфиг: 4 клиента (включая Алексея), порты 4443 и 8445.
- **SNI mismatch:** Xray inbound 4443 → amazon.com, ключ Алексея → cloudflare.com. Гонка ротации.
- vpn-seller-bot inactive — требует поднятия для выдачи новых ключей.

### Возможности агента
- DeepSeek V4 Pro через API пишет эротические рассказы — проверено, работает.
