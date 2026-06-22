---
tags: [project, bug-hunting, bug-bounty]
created: 2026-06-16
status: active
---

# Проект: Поиск багов (Bug Bounty)

Платформы и программы bug bounty, в которых участвуем.

## Активные кампании

### 🎲 TheOriginals.io — OG Bug Hunt
- **Платформа:** https://theoriginals.io
- **Тип:** UI/UX bug bounty ($10-$1000)
- **Подача:** Twitter @theoriginalsio + #OnlyOriginals ИЛИ чат поддержки
- **Статус:** найдено 4 бага, отчёт готов, ждём скрины и подачу

**Находки (2026-06-16):**

| # | Severity | Описание | Оценка |
|---|----------|----------|--------|
| 1 | HIGH | i18n ключи вместо текста на легальных страницах (/legal/privacy, /legal/responsible-gaming, /game/limbo) | $100-300 |
| 2 | HIGH | Ноль security-заголовков (CSP, X-Frame-Options, HSTS) | $200-500 |
| 3 | MEDIUM | blob:http://localhost в проде (/game/hyperdrive) | $30-50 |
| 4 | LOW | Опечатка «provenably» → «provably» fair | $10 |

**Отчёт:** `obsidian-vault/hermes/og-bug-hunt-report-2026-06-16.md`
**Осталось сделать:** скриншоты → подача в Twitter или саппорт

## Архив (завершённые)

_Пока пусто_
