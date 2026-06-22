---
tags: [api, research, infrastructure, trading, product]
created: 2026-06-18
source: https://github.com/public-api-lists/public-api-lists
---

# Public API Lists — анализ для проектов Hermes

> **Источник:** [public-api-lists/public-api-lists](https://github.com/public-api-lists/public-api-lists) — 14.8K ⭐  
> **Формат:** 775+ бесплатных API в 48 категориях, JSON API, веб-поиск  
> **API:** `https://public-api-lists.github.io/public-api-lists/api/all.json`

---

## 🥇 Приоритетные для внедрения

| # | API | Категория | Для чего | Проект |
|---|-----|-----------|----------|--------|
| 1 | **CoinGecko / Coinpaprika** | Cryptocurrency | Мультибиржевой арбитраж, фундаментал | bybit-ws |
| 2 | **Finlight** | News | Realtime financial news + sentiment | bybit-ws |
| 3 | **HaveIBeenPwned** | Security | Проверка утечек ключей/email | Hermes-инфра |
| 4 | **VirusTotal** | Anti-Malware | Сканирование файлов перед деплоем | Hermes-инфра |
| 5 | **AbuseIPDB** | Anti-Malware | Репутация IP (VPN-клиенты, атакующие) | VPN, Hermes |
| 6 | **Clearbit Logo** | Business | Логотипы компаний для дашбордов | Продуктизация |
| 7 | **Mailgun / Mailjet** | Business | Транзакционные письма, онбординг | Продуктизация |
| 8 | **IPASIS** | Fraud Prevention | Детект прокси/VPN/ботов | VPN, безопасность |
| 9 | **CurrencyFreaks** | Currency Exchange | Конвертация PnL в RUB/USDT | bybit-ws |
| 10 | **Cloudmersive** | ML + Documents | NLP, OCR, HTML→PDF, валидация | MCP, продукт |

---

## 📊 По проектам

### bybit-ws (трейдинг) — 63 API

**Cryptocurrency (29):**
- CoinGecko, CoinMarketCap, Coinpaprika, CryptoCompare — фундаментал, мультибиржа
- Binance, Bitmex API — данные других бирж для арбитража
- Bitquery — on-chain данные (40+ сетей), money flow

**Finance (22):**
- Alpha Vantage — акции, forex, крипта
- Yahoo Finance, IEX Cloud — фундаментальные данные
- Earnings Feed — SEC filings, insider trades
- Finlight — financial news + sentiment

**Currency Exchange (12):**
- CurrencyFreaks, Currencylayer — курсы валют
- 1Forge — forex market data

### Hermes-инфраструктура — 114 API

**Security (12):**
- HaveIBeenPwned — утечки паролей
- Shodan — поиск устройств в интернете
- National Vulnerability Database — CVE

**Anti-Malware (5):**
- VirusTotal — сканирование файлов/URL
- AbuseIPDB — репутация IP
- Google Safe Browsing — фишинг/малваре

**Development (87):**
- Abstract API — email validation, IP geolocation, phone validation
- JSONPlaceholder — mock API для тестов
- IPify, ipapi — геолокация по IP

**Cloud Storage (7):**
- Google Drive, Dropbox API — бэкапы
- Box, OneDrive, Mega.nz

### VPN-сервер — 20 API

**Fraud Prevention (3):**
- **IPASIS** — proxy/VPN detection, email validation, bot detection
- FraudLabs Pro — AI fraud screening
- Jumio — identity verification, KYC/AML

**Security (12):**
- HaveIBeenPwned, Shodan, AbuseIPDB
- National Vulnerability Database

### MCP-серверы / разработка — 115 API

**Machine Learning (11):**
- AI Engine — 36+ endpoints: OCR, face detection, background removal, NSFW
- Cloudmersive — image captioning, face recognition, NLP
- CrowdSorcerer — web research, document parsing, LLM generation
- HOL Registry Broker — search/verify AI agents & MCP servers

**Data Validation (17):**
- Cloudmersive Validate — email, phone, VAT, domain
- Kiprio Email Validation — MX, disposable, role, typo detection
- Lob.com — US address verification

### Продуктизация — 34 API

**Business (16):**
- Clearbit Logo — логотипы компаний
- Mailgun, Mailjet — email сервис
- Gmail API, Google Analytics
- Tomba — email finder для B2B
- Domainsdb.info — поиск доменов

**Documents & Productivity (18):**
- Cloudmersive — HTML→PDF, Office→PDF
- DynamicDocs — JSON→PDF (LaTeX)
- File.io — file sharing
- CustomJS — HTML to PDF/PNG

### Telegram-боты — 40 API

**News (10):**
- Currents — новости из блогов/форумов
- Feedbin — RSS reader
- Finlight — financial news + sentiment
- Associated Press

**Social (25):**
- Discord API, Facebook, Buffer
- BulkPublish — 11 соцсетей + scheduling + AI agent support

**URL Shorteners (5):**
- Bitly, Rebrandly, T.LY

### Мониторинг — 13 API

Скромно. Основной мониторинг через:
- Health (6): Nutritionix, Diabetes — нерелевантно
- Events (4): Eventbrite, Ticketmaster — нерелевантно
- Tracking (3): Let's Count — счётчики

**Вывод:** для мониторинга лучше использовать специализированные сервисы (Prometheus, Grafana, UptimeRobot), а не general-purpose API.

---

## 🔴 Что НЕ брать

- **Животные, Аниме, Игры** — не для наших проектов
- **Транспорт, Погода, Спорт** — нецелевое
- **Образование, Патенты** — мимо
- **Музыка, Видео, Фотография** — не приоритет

---

## 📝 План внедрения

### Этап 1: Быстрые победы ✅ (18.06.2026)
- [x] **HaveIBeenPwned** → `~/.hermes/scripts/hibp-check.py` + cron `hibp-daily-check` (ежедневно 09:00)
- [x] **AbuseIPDB** → `~/.hermes/scripts/abuseipdb-check.py` + cron `abuseipdb-vpn-check` (каждые 6ч)
- [x] **VirusTotal** → `~/.hermes/scripts/vt-scan.py` + интеграция в `deploy.sh` (pre-deploy scan)
- [ ] **API-ключи** → заполнить `HIBP_API_KEY`, `ABUSEIPDB_API_KEY`, `VT_API_KEY` в `~/.hermes/secrets.env`

### Этап 2: Трейдинг (3-5 дней)
- [ ] **CoinGecko API** → мультибиржевые данные в bybit-ws
- [ ] **Finlight** → sentiment analysis для входов
- [ ] **CurrencyFreaks** → конвертация PnL в RUB

### Этап 3: Продуктизация (в рамках MVP)
- [ ] **Mailgun** → транзакционные письма
- [ ] **Clearbit Logo** → дашборды
- [ ] **Cloudmersive** → HTML→PDF для отчетов

---

## 🔧 Реализация (18.06.2026)

### Созданные файлы

| Файл | Назначение |
|------|-----------|
| `~/.hermes/scripts/hibp-check.py` | Проверка email на утечки (HIBP API v3) |
| `~/.hermes/scripts/abuseipdb-check.py` | Репутация IP VPN-клиентов (AbuseIPDB v2) |
| `~/.hermes/scripts/vt-scan.py` | Сканирование файлов перед деплоем (VT API v3) |

### Cron-джобы

| Job ID | Имя | Расписание |
|--------|-----|-----------|
| `372eb5eb1f88` | `hibp-daily-check` | Ежедневно 09:00 |
| `5d30df424e7f` | `abuseipdb-vpn-check` | Каждые 6 часов |

### Интеграция в deploy.sh

VT-скан добавлен в `bybit-ws/deploy.sh` (шаг 2, перед атомарным swap).  
При обнаружении — деплой блокируется. Флаг `SKIP_VT_SCAN=1` для принудительного пропуска.

### API-ключи

| Переменная | Нужен? | Где получить |
|-----------|--------|-------------|
| `HIBP_API_KEY` | 🟢 Опционально | https://haveibeenpwned.com/API/Key |
| `ABUSEIPDB_API_KEY` | 🔴 Обязателен | https://www.abuseipdb.com/account/api |
| `VT_API_KEY` | 🔴 Обязателен | https://www.virustotal.com/gui/my-apikey |

**HIBP работает без ключа:** отслеживание глобальных брешей + проверка паролей (k-anonymity).  
Ключ нужен только для проверки конкретных email'ов.

---

## Связанные заметки

- [[hermes/bybit-ws-development-plan|План развития bybit-ws]]
- [[hermes/bybit-ws-full|Документация bybit-ws]]
- [[roadmap-aegis-ai-engine|Roadmap Aegis AI Engine]]
