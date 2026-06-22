# 3-Echelon Audit: Hermes Orchestrator — 2026-06-14

**Вердикт:** 🔴 **FAIL** — 9 CRITICAL, 10 HIGH, 13 MEDIUM, 10 LOW = **42 находки**

---

## Сводка по эшелонам

| Эшелон | Проверяющий | Вердикт | C | H | M | L |
|--------|------------|---------|---|---|---|---|
| 🔍 Source-Driven | Аудитор документации | ❌ FAIL | 1 | 2 | 6 | 5 |
| 🔒 Security | Security-аудитор | ❌ FAIL | 5 | 3 | 3 | 2 |
| ⚔️ Adversarial | Adversarial-ревьюер | ❌ FAIL | 3 | 5 | 4 | 3 |
| **ИТОГО** | | | **9** | **10** | **13** | **10** |

---

## 🔴 CRITICAL (9)

### C1 ✦ Source: cost-tracker цены V3 вместо V4 (ошибка до 19×)
`cost-tracker-v2.py` использует цены DeepSeek V3 ($0.07 cache-hit), а актуальные V4 Pro — $0.003625. Cache-hit завышен в **19 раз**.

### C2 ✦ Security: нет `.gitignore` в `~/.hermes/`
`hermes.key`, `.env`, `profiles/*/.env` — ничем не защищены от случайного `git add .`

### C3 ✦ Security: `*.key` и `*.bak` не в `.gitignore`
`hermes-agent/.gitignore` не включает `*.key` и `*.bak`

### C4 ✦ Security: утечка TELEGRAM_BOT_TOKEN в бекапе логов
`errors.log.1-2026060900.backup` содержит префикс токена (`TELEGRAM_BOT_TOKEN=807899...`), права 664

### C5 ✦ Security: `.env.enc` тенанта имеет права 664
`user_308591502/.env.enc` world-readable — можно скопировать для офлайн-брутфорса

### C6 ✦ Security: бекап логов ошибок имеет права 664
`errors.log.1-2026060900.backup` доступен всем на чтение с утёкшим токеном

### C7 ✦ Adversarial: терминал-команды от openclaw, не от tenant
iptables привязаны к UID tenant'ов, но Hermes выполняет все команды как `openclaw` → изоляция на уровне промпта, не ядра

### C8 ✦ Adversarial: `except: pass` — молчаливый отказ disabled_toolsets
При ошибке загрузки профиля тенант получает **полный доступ админа** (148 скиллов, delegation, cron)

### C9 ✦ Adversarial: потеря `hermes.key` = полный отказ системы
Нет бэкапа, shamir sharing, fallback. Все `.env.enc` становятся нечитаемы, gateway не стартует

---

## 🟠 HIGH (10)

| ID | Эшелон | Суть |
|----|--------|------|
| H1 | Source | `fact-checker.py`: temperature=0 молча игнорируется DeepSeek V4 (thinking mode по умолчанию) |
| H2 | Source | Ноль ссылок на официальную документацию API (age, DeepSeek, Telegram, iptables, systemd) |
| H3 | Security | `user_5529208670/config.yaml` — права 644 (карта изоляции для атакующего) |
| H4 | Security | Бекапы логов ошибок с правами 664 |
| H5 | Security | 13 упоминаний имён чувствительных переменных в бекапе логов |
| H6 | Adversarial | Gateway-патч теряется после `git pull` — до 7 дней без изоляции |
| H7 | Adversarial | cronjob разрешён 2/3 тенантов, процесс openclaw — tenant может читать ключи админа |
| H8 | Adversarial | Утечка `.env` между тенантами через авто-обнаружение в fact-checker, judge, decrypt |
| H9 | Adversarial | Race condition: DELETE+INSERT без транзакции в cost-tracker |
| H10 | Adversarial | skill-sync затирает правки тенанта без бэкапа и предупреждения |

---

## 🟡 MEDIUM (13)

- M1: Неканонический `/v1` префикс в DeepSeek URL (6 файлов)
- M2: cost-tracker — хардкод цен без валидации
- M3: health_check.py — непоследовательный HTTP-клиент (urllib vs requests)
- M4: SKILL.md — размножение неверной цифры стоимости ($0.00143 вместо $0.00115)
- M5: tenant-health-check — проверка age-заголовка без ссылки на спек
- M6: config.yaml — `/v1` в base_url
- M7: cost-tracker — хардкод unlimited для tenant 470549555 (Илья)
- M8: Децентрализованное чтение DEEPSEEK_API_KEY (5 скриптов, разная логика)
- M9: cronjob не отключён у user_470549555 (в отличие от других)
- M10: telegram-watchdog — только 200 строк лога
- M11: decrypt_env — нет блокировки при конкурентном запуске
- M12: Веб-чат без HTTPS (http://2.27.48.142:9999/chat.html)
- M13: audit_logger не интегрирован в gateway

---

## 🟢 LOW (10)

- L1: hermes-tenant: хрупкий grep для публичного ключа age
- L2: fact-checker: недокументированная схема кэша
- L3: decrypt_env: нет обработки ошибок формата age
- L4: SKILL.md: send_message vs sendMessage naming
- L5: config.yaml: хардкод freellmapi ключа
- L6: `*.bak` не в .gitignore
- L7: audit.log и fallback.log не проверены на секреты
- L8: iptables для новых тенантов — ручное добавление
- L9: health_check.py — ключ в HTTP-заголовках, риск утечки в логи
- L10: hermes-tenant onboard не добавляет iptables автоматически

---

## 🔧 Приоритетные исправления (топ-5)

1. **Создать `.gitignore`** — защитить `hermes.key`, `.env`, `profiles/*/.env` от коммита
2. **Исправить права** — chmod 600 на `.env.enc`, `config.yaml`, бекапы логов
3. **Очистить утечку токена** — удалить строку с `TELEGRAM_BOT_TOKEN=807899` из бекапа
4. **Исправить цены** — cost-tracker: DeepSeek V4 Pro вместо V3
5. **Добавить `thinking: disabled`** — fact-checker для детерминированной сверки

### Корневая проблема (архитектурная)

**Процесс Hermes работает как `openclaw`, а не от tenant-пользователя.** Три слоя изоляции полагаются на промпт-уровень, а не на уровень ядра. Тенант через terminal может читать ключи админа и чужие `.env`.

---

*Аудит: 3 эшелона параллельно, 14.06.2026*
*Эшелон 1: аудитор документации (DeepSeek V4)*
*Эшелон 2: security-аудитор (DeepSeek V4)*
*Эшелон 3: adversarial-ревьюер (DeepSeek V4)*
