---
tags: [vpn, audit, ponytail]
created: 2026-06-15
source: /opt/vpn-seller-bot/bot.py (2753 строки, 128K)
---

# Ponytail-аудит VPN-бота (2026-06-15)

Полный разбор `bot.py` (vpn-seller-bot) по методологии @ponytail — ленивый сеньор-разработчик матерится, но по делу.

## Оценка: 6.2/10

| Что | Оценка |
|-----|--------|
| Работает | ✅ Да |
| Не падает | ✅ В целом |
| Читаемо | 🟡 Местами |
| Расширяемо | ❌ Монолит |
| Безопасно | 🟡 Race condition в промо |
| Идиоматично | ❌ `__import__`, импорты в телах |

---

## 🔴 КРИТИЧНОЕ (надо чинить сразу)

### 1. Двойной health-check в `cmd_health_handler` (стр. 1651–1674)

```python
async def cmd_health_handler(message: Message):
    # ...
    await cmd_admin(message)  # ← вызывает /admin health, который уже делает ВСЁ
    # А потом делает то же самое ещё раз ↓
    with db() as conn:
        active = conn.execute("SELECT COUNT(*) ...").fetchone()[0]
    # ...
```

**Это баг.** При `/health` админ получает двойной ответ: сначала от `cmd_admin` (subcmd=health), потом от `cmd_health_handler` с тем же самым. Для не-админа логика тоже странная — сначала отказ в `cmd_admin` (админ-денид), потом свой хелс-чек.

**Фикс:** удалить `await cmd_admin(message)` из `cmd_health_handler` — либо оставить только его для админов, либо оставить только свой код.

### 2. Race condition в промокодах (стр. 734–763)

```python
ok, msg_key = promo_can_redeem(message.from_user.id, code)  # CHECK
if not ok:
    ...
promo_redeem(message.from_user.id, code)  # THEN ACT
```

В асинхронном боте два одновременных вызова `/promo XXXX` от одного юзера могут оба пройти проверку и оба применить промокод. **Check-then-act — классическая гонка.**

**Фикс:** заменить на `INSERT OR IGNORE` с атомарной проверкой в одной транзакции БД.

---

## 🟡 СЕРЬЁЗНОЕ (техдолг, копится)

### 3. Монолит на 2753 строки
Весь бот — один файл. Никакого разделения на `handlers.py`, `db.py`, `xray.py`, `i18n.py`. При росте функционала станет неуправляемым. Плюс `admin_key.py` (197 строк) дублирует часть логики.

### 4. Импорты внутри тел функций (антипаттерн)
- `import json` — 6 раз в разных функциях (стр. 1001, 1236, 1306, 1856, 2265, 2689)
- `import urllib.parse` — 2 раза
- `import shutil` — 2 раза
- `from aiogram.types import ...` — в горячих коллбэках

Каждый `import` делает поиск в `sys.modules`, замедляя горячие пути (особенно `on_callback` — 1515 строк).

**Фикс:** все импорты — наверх файла.

### 5. `__import__('socket')` (стр. 2508, 2523) — wtf

```python
sock = __import__('socket').socket(__import__('socket').AF_INET, ...)
```

`__import__` — это CPython-интернал, не для прикладного кода. Просто `import socket` наверх.

### 6. Дубликат `build_vless_link`
- `bot.py` (стр. 1000–1025): берёт параметры из `VLESS_*` env-переменных
- `admin_key.py` (стр. 59–97): читает из `xray_config.json`

Разная логика → бот может сгенерировать **невалидную ссылку**, если конфиг изменился через админку.

**Фикс:** единая функция, читающая из конфига, в общем модуле.

### 7. Синхронный SQLite блокирует event loop (стр. 396)
```python
def db() -> sqlite3.Connection:
    conn = sqlite3.connect(DB_PATH)
    # WAL, sync=NORMAL — хорошо, но...
```
Все `with db() as conn:` вызовы — синхронные. Под нагрузкой (50+ пользователей жмут кнопки) SQLite I/O заблокирует asyncio event loop.

**Фикс:** `aiosqlite` или `asyncio.to_thread()` для всех обращений к БД.

### 8. `on_callback` — 1515 строк (стр. 1787–2301)
Одна гигантская функция с 20+ `if data == ...`. Каждое условие — копипаста паттерна:
```python
await upsert_main_message(...)
await clear_keyboard(...)
await bot.send_message(...)
```

**Фикс:** разнести по отдельным handler'ам с aiogram Router.

---

## 🟢 МЕЛОЧИ (бесят, но не убивают)

### 9. Глобальный mutable state
```python
AUTO_CHECK_TASKS: dict[int, asyncio.Task] = {}  # стр. 336
_rate_cache: dict = {"ton_usd": 0.0, ...}        # стр. 345
_last_backup_ts = 0                               # стр. 2379
```
Работает пока один инстанс. Мины замедленного действия при скейлинге.

### 10. Словарь переводов `T` инлайном (стр. 34–297)
260+ строк питонячьего словаря в теле модуля. Должен быть в JSON/YAML.

### 11. Молчаливое проглатывание ошибок
```python
try:
    await bot.edit_message_text(...)
except Exception:
    pass  # стр. 1393 — даже не логируется
```
```python
try:
    lang = get_lang(_conn, tg_id)
except Exception:
    pass  # стр. 2703
```
Хотя бы `log.debug()` добавить, чтобы при дебаге видеть, что сломалось.

### 12. Hardcoded пути
`/opt/vpn-core/`, `/opt/vpn-seller-bot/backups`, `./data/bot.lock` — разбросаны по всему коду. Вынести в config/`.env`.

---

## Сопутствующие файлы

- `admin_key.py` (197 строк): инструмент управления админ-ключами, дублирует `build_vless_link`, использует другой подход к `rebuild_xray`
- `.env`: конфиг (токены, цены, пути)

---

## План исправлений (на завтра)

1. 🔴 `cmd_health_handler` — убрать двойной вызов
2. 🔴 `promo` — атомарный redeem через `INSERT OR IGNORE`
3. 🟡 Все импорты — наверх файла
4. 🟡 `build_vless_link` — в общий модуль, чтение из конфига
5. 🟡 `on_callback` — разбить на handler'ы с Router
6. 🟢 `T`-словарь — в отдельный JSON
