---
tags: [security, github, dorks, bugbounty, gsc]
source: https://spy-soft.net/github-dorks/
created: 2026-06-30
---

# GitHub Dorks

Поисковые запросы для нахождения секретов и уязвимостей в публичных репозиториях GitHub.

## Основные операторы

| Оператор | Пример | Ищет |
|----------|--------|------|
| `language:` | `language:python` | По языку |
| `filename:` | `filename:.env` | По имени файла |
| `extension:` | `extension:pem` | По расширению |
| `created:` | `created:>2026-06-25` | Свежие репы |
| `org:` | `org:company` | По организации |

## Категории дорков

- **API-ключи и токены:** `filename:.env password`, `extension:pem private`
- **Бекапы:** `filename:backup`, `filename:dump.sql`
- **Пароли:** `filename:config password`, `filename:credentials`
- **Internal endpoints:** `"api_key" language:python`, `"secret_token"`

## Инструменты

- **gdorklinks.sh** — генератор ссылок по компании
- **GitDorker** — 513 дорков + GitHub Search API (нужен токен)
- **truffleHog** — сканирование репозиториев на секреты

## Интеграция с GSC

Можно добавить как источник паттернов для GS001 (Hardcoded Secrets) или сделать модуль `gsc_dork_scan` для поиска по внешним репозиториям конкурентов/партнёров.
