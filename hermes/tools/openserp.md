---
tags: [tools, search, serp, self-hosted, docker]
created: 2026-06-23
source: https://github.com/karust/openserp
stars: 791
status: deployed
---

# OpenSERP — self-hosted поисковый API

Бесплатный SERP API. Google, Yandex, Baidu, Bing, DuckDuckGo, Ecosia.

## Установка

```bash
docker run -d --name openserp -p 127.0.0.1:7000:7000 karust/openserp:latest serve -a 0.0.0.0 -p 7000
```

## Использование

```bash
# Одиночный поиск
curl "http://localhost:7000/yandex/search?text=запрос&limit=5"

# Мега-поиск (все движки сразу)
curl "http://localhost:7000/mega/search?engines=google,yandex,bing&text=запрос"

# С извлечением контента (для RAG)
curl "http://localhost:7000/yandex/search?text=запрос&extract=1"
```

## Что работает

| Движок | Статус |
|--------|--------|
| Yandex | ✅ работает |
| Google | 🟡 0 результатов (нужен тюнинг) |
| Baidu | ⬜ не проверен |
| Bing | ⬜ не проверен |
| DuckDuckGo | ⬜ не проверен |

## Применимость к Hermes

- Замена `web_search` (который отключён)
- RAG-пайплайн: поиск → extract → кормим LLM
- Русскоязычный поиск (Yandex) — для ГОСТов, нормативки
- `/mega/search` — агрегация результатов с дедупликацией

## Порт

`127.0.0.1:7000` — только локально
