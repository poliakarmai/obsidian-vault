---
status: active
as_of: 2026-08-14
tags: [gsc, roadmap, maturity, release]
---

# GSC Roadmap Maturity — завершён

Дорожная карта зрелости (`GSC_ROADMAP.pdf`, baseline `f542fe6`) закрыта полностью.
Все волны A/B/C/D + due-diligence v2 + низкоприоритетная добивка.

## Итог по волнам

| Волна | Задачи | Результат |
|-------|--------|-----------|
| **A** | 3.9 header-only API key · 3.8 JWT fail-closed · 3.5 StageOutcome · 2.7 динамический standalone · 4.9 `/ready` | ✅ |
| **B** | 3.2 web PoC в контейнере · 3.10 security tests · 4.7 request-scoped DB | ✅ |
| **C** | 4.8 out-of-process worker · 5.1 no import side effects · 5.4 release manifest · 6.3 markers · 6.10 conftest | ✅ |
| **D** | THREAT_MODEL · ARCHITECTURE · DEPLOYMENT · PILOT_GUIDE · KNOWN_LIMITATIONS · openapi.json · «does NOT do» | ✅ |
| **Низкоприоритет** | 7.1 README gen · 7.5 CHANGELOG · 4.11 backup drill · 5.5/5.8/6.8 CI | ✅ |

## Ключевые цифры (SSOT `gsc_meta.py`)

- **Детекторы:** 41 (37 registry + 4 движка)
- **Schema:** v32
- **Модули:** 109
- **Тесты:** 188 passed, 5 skipped

## Due-diligence v2 (закрыт)

- P0/P1/P2 + шаги 4–6: immutable base image (digest), SBOM (CycloneDX),
  tenant-isolation тест, README disclosure про verification strength.

## Что осталось (не блокирует pilot)

- 🟡 5.2 env/XDG paths · 5.7 SBOM в CI · 6.7 skip policy · 7.10 inline comments
- ⬜ 6.5 hardcoded path · 6.6 coverage gate · 6.9 отделить smoke · 5.9 apps/ wheel

## Статус

**Готов к limited single-tenant pilot.** Push-состояние на 2026-08-14:
последний push `66bcfc7`, локальные коммиты добивки зафиксированы (push по команде).

См. также: [[gsc-cloud-launch|GSC Cloud Launch]], [[gsc-status-2026-08-11|GSC Status 08-11]]
