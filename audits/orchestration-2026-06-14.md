# Automation Audit — Оркестрация агентов — 2026-06-14

**Время:** 14:30 EEST
**Исполнитель:** Море (главный оркестратор)

---

## 📊 Inventory

### 1. Cron Jobs (29)

| Джоб | Расписание | Режим | Статус |
|------|-----------|--------|--------|
| Daily Bollinger Scan | 10:00 daily | LLM | ✅ ok |
| Scoring Scan | 11:00 daily | LLM | ✅ ok |
| Утренний скан LONG | 05:00 daily | LLM | ✅ ok |
| M5/M3 авто-сканер | каждые 4ч | no_agent | ✅ ok |
| PnL morning | 09:00 daily | LLM | ✅ ok |
| Weekly PnL | 09:00 пн | no_agent | ✅ ok |
| Cost daily collect | каждые 3ч | LLM | ✅ ok |
| Cost weekly | 10:00 пн | LLM | ✅ ok |
| Crypto Daily Digest | 06:00 daily | LLM | ✅ ok |
| Newswatch | 08:00, 20:00 | LLM | ✅ ok |
| VPN DB backup | 03:00 daily | no_agent | ✅ ok |
| VPN snapshot | 02:55 daily | no_agent | ✅ ok |
| VPN watch | каждые 5м | no_agent | ✅ ok |
| System backup | каждые 4 дня | no_agent | ✅ ok |
| Memory consolidate | 02:00 daily | no_agent | ✅ ok |
| Memory prune | 08:00 daily | no_agent | ✅ ok |
| Session prune | 04:00 daily | no_agent | ✅ ok |
| Tenant health | 10:00 пн | no_agent | ✅ ok |
| Tenant health daily | 09:00 daily | no_agent | ✅ ok |
| Telegram watchdog | каждую минуту | no_agent | ✅ ok |
| Dashboard refresh | каждые 15м | no_agent | ✅ ok |
| Gmail автосортировка | каждые 10м | no_agent | ✅ ok |
| GitHub weekly push | 10:00 пн | no_agent | ✅ ok |
| Вахта: дедлайны | 06:00 daily | no_agent | ✅ ok |
| Утренняя цитата | 07:00 daily | no_agent | ✅ ok |
| Morning Session Health | 04:00 daily | LLM | ✅ ok |
| **SkillOpt weekly tuning** | **04:00 пн** | **LLM** | **❌ error** |
| Weekly Project Audit | 09:00 вс | LLM | ⏳ первый 21.06 |
| PCI Bybit Key Reminder | 09.07 12:00 | no_agent | ⏳ ждёт |

### 2. Systemd Services (8)

| Сервис | Тип | Статус |
|--------|-----|--------|
| `hermes-gateway` | user | ✅ running |
| `hermes-chat` | user | ✅ running |
| `command-center` | user | ✅ running |
| `bybit-ws` | user | ✅ running |
| `freellmapi` | user | ✅ running |
| `vpn-seller-bot` | system | ✅ running |
| `vpn-core-xray` | system | ✅ running |

### 3. MCP Servers

| Сервер | Args формат | Статус |
|--------|------------|--------|
| bybit-ws | ✅ YAML-список | OK |
| tavily | ✅ YAML-список | OK |
| dexscreener | ✅ YAML-список | OK |
| osint-tools | ✅ YAML-список | OK |

### 4. Tenant Health

```
✅ iptables: DNS изоляция для cryptos, ilya, marina
✅ home dirs: права 700/770
✅ env encryption: всё зашифровано
✅ gateway-patch: на месте
✅ Профили: poliakarm, user_308591502, user_470549555, user_5529208670
```

### 5. Config Health

- `cdp_url`: пусто (нет спама Connection refused) ✅
- `fallback_model`: не установлен ✅
- MCP args: YAML-список ✅

---

## 🔴 Findings

### ❌ SkillOpt weekly tuning — error
- **Джоб:** `e68d5ed40e95`, 04:00 пн
- **Последний запуск:** 08.06.2026 — error
- **Причина:** вероятно SkillOpt скрипт упал (нужно проверить логи)

### ⚠️ 29 cron-джобов — высокая плотность
- 7 джобов в 09:00-10:00 окне (пн: 09:00 weekly-pnl, 09:00 tenant-health-daily, 09:00 pnl-morning, 10:00 cost-weekly, 10:00 github-push, 10:00 tenant-health, 10:00 bollinger-scan)
- 5 джобов в 04:00-05:00: session-prune + morning-health + skillopt + утренний LONG

### ⚠️ VPN watch каждые 5 минут = 288/день
- Согласно принципам automation-audit: silent-when-clean скрипты с частотой 5м — кандидаты на увеличение интервала

---

## 📋 Recommendations

| Действие | Что | Почему |
|----------|-----|--------|
| **FIX NEXT** | SkillOpt tuning | error при последнем запуске |
| **MERGE** | tenant-health-check + tenant-health-daily | два джоба с разной периодичностью делают одно и то же |
| **KEEP** | Всё остальное | работает, не дублируется |
| **CUT** | — | удалять нечего |

---

## ✅ Tenant Health — подробно

- **Пользователи:** 3 tenant'а (cryptos UID=1002, ilya UID=1003, marina UID=1004)
- **Изоляция:** iptables DNS-only, home dirs 700/770
- **Шифрование:** все .env зашифрованы через age
- **Gateway патч:** profile-level disabled_toolsets на месте
- **Obsidian vaults:** per-tenant (авто-создание при онбординге)

---

*Следующий авто-аудит: 21.06.2026 09:00 (cron ce4940b0e05a)*
*Tenant health: 15.06.2026 10:00 (cron 7049e70d0967)*
