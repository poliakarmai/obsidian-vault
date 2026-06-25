# 23.06.2026 — Аудит и чистка оркестрации

## Что сделано

### Факт-чек документации
- Обнаружены расхождения: 1690 сессий (реально 22), admin 42 скилла (реально 117), skill-sync «сломан» (ошибка подсчёта — 13 dirs = 42 leaf-скилла)
- SIGTERM-хук найден в user systemd (не system), работает
- 3 итерации правок документации (v3.0 → v3.3)

### Чистка профилей
- Удалены лишние скиллы: Илья 83→42, Марина 83→42, боты 97-100→42
- Все тенанты: 42 base-скилла, без trading
- Админ: 117 скиллов (42 base + 46 admin_only + 21 opt_in + 8 extra)

### Утечка trading/
- session-summarizer писал `trading/sessions/` всем тенантам
- Удалено из 5 vault'ов
- Скилл исправлен: админ → trading/sessions/, тенанты → sessions/

### 42 base-скилла
- Задокументированы: creative(2), email(1), fire-safety(1), github(5), mcp(1), media(3), meta(3), note-taking(2), productivity(14), research(4), security(1), software-dev(4), tools(1)

### Коммиты
- hermes-orchestrator: `bc45c1a` — session-summarizer fix
