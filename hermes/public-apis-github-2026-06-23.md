---
tags: [api, open-source, github, infrastructure, development]
created: 2026-06-23
source: https://ai-uchi.ru/news/public-apis-besplatnye-api-github/
original: https://github.com/public-apis/public-apis
---

# Public APIs: 1400+ бесплатных API

**Источник:** AI-Uchi, 22 июня 2026
**Оригинал:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — 300K+ ⭐, MIT

---

## Суть

Крупнейший кураторский каталог бесплатных публичных API на GitHub. 1400+ сервисов в 50+ категориях. Каждая запись: название, описание, тип аутентификации (apiKey/OAuth/без ключа), HTTPS, CORS.

## Структура записи

```python
import requests
resp = requests.get("https://dogapi.dog/api/v2/facts")
data = resp.json()
print(data["data"][0]["attributes"]["body"])
```

Большинство API без авторизации — можно дёргать сразу.

## Ключевые категории

| Категория | Примеры | Доступ |
|-----------|---------|--------|
| Animals | Dog Facts, HTTP Cat, eBird | Без ключа / apiKey |
| Machine Learning | Несколько ML-сервисов | apiKey |
| Anti-Malware | VirusTotal, URLScan.io | apiKey |
| Anime | Jikan, AniList, Studio Ghibli | OAuth / без ключа |
| Art & Design | Met Museum, Rijksmuseum | Без ключа / apiKey |
| Cryptocurrency | Множество крипто-источников | apiKey |
| Games & Comics | Игровые и комикс-базы | Разный |

## Связь с APILayer

Курируется сообществом + командой APILayer (маркетплейс API). Коммерческие версии: IPstack, Marketstack, Weatherstack, Fixer, Aviationstack.

## Важно

- ⚠️ Часть API устаревшие/мёртвые — проверять документацию перед интеграцией
- Pull request'ы от сообщества → каталог живёт и пополняется
- Лицензия MIT — можно использовать в коммерческих проектах

## Применимость к Hermes

| Концепция | У них | У нас |
|-----------|-------|-------|
| Крипто-данные | Множество API | bybit-ws + CoinGecko |
| Погода | Open-Meteo, Weatherstack | Нет (можно для вахты) |
| ML-сервисы | Несколько | DSPy на DeepSeek |
| Безопасность | VirusTotal | skill-security-scan |

Вердикт: полезный справочник для прототипирования, но не для продакшн-зависимостей.
