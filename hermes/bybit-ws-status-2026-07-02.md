# bybit-ws — статус на 02.07.2026

## Версия
- **v7.7** (commit 036eabf на master)
- BE-SL: вариант Б (активация при +3%, SL = entry×1.01 LONG / entry×0.99 SHORT)
- tight trailing для SHORT
- Исправлены дубликаты fetch_positions(), корреляции abs(r), NameError new_positions

## Сервис
- bybit-ws-async: active ✅
- Циклы каждые ~5 минут
- Telegram fallback работает (ntfy.sh исчерпал дневной лимит)

## Трейдинг на 02.07
- 4 позиции LONG, unrealized PnL -$107.48
- STG, MOVE, DOT — старые позиции (до стратегии), ждут закрытия
- WLFIUSDT — новый вход по текущей стратегии
- За день закрыто: DASH +$2.81, ACH +$1.53, DOGE -$0.46

## Что сделано с 30.06
- BE-SL исправлен (вариант Б, tight trailing SHORT)
- Устранены дубликаты REST-вызовов
- Корреляции исправлены (abs → знаковая проверка)
- NameError new_positions исправлен
- Все LLM-кроны переведены на deepseek-v4-pro
