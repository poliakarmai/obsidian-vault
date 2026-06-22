# Жадная память — Windsurf Pattern

> «Save immediately. Don't wait for task completion. Context window is limited — everything not saved will be lost.»

## Ключевые факты (сохранены 12.06.2026)

### Инфраструктура
- Hermes multi-tenant: 4 тенанта, 148 скиллов
- Gateway: systemd, авто-рестарт
- Дашборд: http://2.27.48.142:9999/dashboard.html
- Резервный чат: http://2.27.48.142:9999/chat.html
- VPN: VLESS+REALITY, Xray
- bybit-ws: systemd, RPC 8766, GridSignal бот отдельно

### GitHub
- Аккаунт: poliakarmai
- 2FA: TOTP (Google Authenticator)
- Recovery codes: `hermes/github-recovery-codes.md`
- Репа bybit-ws: публичная, но профиль скрыт (user_view_type: private)
- Звёзды поставлены, issue создан — ждём разблокировку

### Скиллы (новые)
- `agent-best-patterns` — выжимка из Claude Code, Cursor, Windsurf
- `human-style-writer` — обход AI-детекторов (промпт DoctorGPT)

### Принятые решения (12.06.2026)
- Внедрены 5 паттернов из топ-3 AI-агентов
- «Не коммитить без спроса» зафиксировано в конституции
- Память включена в config.yaml (memory_enabled: true)
- Жадное сохранение контекста через Obsidian
