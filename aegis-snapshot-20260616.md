# Aegis AI Engine — Снапшот 16.06.2026

## Состояние гейтвеев

| Гейтвей | Бот | Модель | Доступ | Статус |
|---------|-----|--------|--------|--------|
| Production | @Morearbot | custom (DeepSeek) | 4 доверенных | ✅ Жив |
| Demo | @Apolaibot | DeepSeek (custom_provider) | Открыт всем | ✅ Жив |

## Demo-гейтвей

- **Профиль:** `/home/openclaw/.hermes/profiles/demo/`
- **Модель:** `deepseek-v4-pro` через `custom_providers.deepseek`
- **System prompt:** Aegis AI Engine — 4 УТП, лимиты (50/день, 131K контекст), прайсинг Pro
- **Онбординг:** `profile_build: ask`, `GATEWAY_ALLOW_ALL_USERS: true`
- **Disabled toolsets:** delegation, cronjob, send_message, code_exec, skill_manage
- **Тестер:** Cloud (6290772314) — сын Алексея

## Production-гейтвей

- **Профиль:** `/home/openclaw/.hermes/`
- **Модель:** `custom` → DeepSeek API
- **ALLOWED_USERS:** 319665243,5529208670,1148002325,470549555
- **Онбординг:** `profile_build: ask`

## Бекап

- **Файл:** `~/.hermes/backups/manual/aegis-project-20260616-0958.tar.gz` (76 MB)
- **Санация:** .env удалены из бекапа
- **Что внутри:** config.yaml, skills, cron, scripts, demo-профиль, Obsidian vault, aegis-landing.html

## Известные проблемы

1. Cron `incident-response` (f30b5e0f0817) — падает с Broken pipe (каждые 5 мин)
2. `TERMINAL_CWD` в demo/.env — deprecated, предупреждение в логах

## Следующие шаги (роадмэп)

- Фаза 1B: Лендинг на GitHub Pages
- Фаза 2: Whitepaper + Sales Kit
