Создай мобильное приложение для русскоязычных туристов во Вьетнаме. Приложение объединяет каталог проверенных партнёров (экскурсии, еда, обмен валют, трансфер, няни, врачи и др.) с возможностью бронирования и заказа.

## Стек

- Flutter (Dart) — один код под Android + iOS
- Тёмная тема (фон #0D0D0D, карточки #1A1A1A)
- Акцент: оранжевый #FF6B00
- Шрифт: системный sans-serif
- Данные: JSON-файлы → API в будущем
- **Изображения:** используй picsum.photos с сидами для ВСЕХ фото (партнёры, города, hero, блюда). Пример: `https://picsum.photos/seed/vietnam1/800/600`. Создай класс `AppImages` с константами URL — чтобы заменить одной правкой.
- **Погода:** данные о температуре и иконке для хедера брать из мокового поля `weather` в `cities.json`. НЕ подключай Weather API.
- Android minSdk 21, iOS min 13.0, portrait-only

---

## Навигация

5 табов внизу (BottomNavigationBar):

| Таб | Иконка | Название | Куда ведёт |
|-----|--------|----------|-----------|
| 1 | 🏠 дом | Главная | HomeScreen |
| 2 | ⊞ сетка | Услуги | ServicesScreen (отсюда же → Экскурсии, Доставка, Обмен, Трансфер) |
| 3 | 📖 книга | Гайд | GuideScreen |
| 4 | 🎫 календарь | Билеты | TicketsScreen (Авиа/Автобус/Поезд) |
| 5 | 👤 человек | Профиль | ProfileScreen |

Активный таб — оранжевый, остальные — серые.

---

## Header (общий для всех экранов)

- Слева: логотип — красная звезда ★ + "VIET LIVE" (красный жирный) + "SERVICE" (белый мелкий)
- Справа: овальная кнопка с оранжевой обводкой: 📍 "Нячанг" + 🌩 "30°"
- Кнопка города кликабельна → смена города

---

## Экран 1 — Главная

### Hero-карточка
- Полноширинная, border-radius 16px, фон — фото бухты Халонг
- Поверх фото текст (белый):
  - «Всё для отдыха во Вьетнаме» (жирный)
  - «в одном приложении»
  - «Бронируйте экскурсии, заказывайте трансферы, обменивайте валюту и получайте поддержку на русском языке в любое время.»
- Клик → экран Услуг

### Акция
- Тёмно-серая карточка. Слева: красный круглый бейдж «-25%»
- Текст: «Специальное предложение!» (оранжевый), «Скидка 25% для компаний от 4 человек» (белый), «Путешествуйте больше — платите меньше» (серый)
- Справа: оранжевая круглая кнопка →

### 🔥 Сегодня рекомендуем
- Заголовок «🔥 Сегодня рекомендуем в Нячанге»
- Список VIP-партнёров (текущий город). Каждый: название, категория, краткое описание (120 символов), контакт
- Клик → карточка партнёра

### Куда летим?
- Заголовок «Куда летим?» (белый жирный)
- Список городов: Нячанг, Дананг, Фукуок, Хошимин, Ханой, Далат, Муйне
- Каждый город — карточка с иконкой-эмодзи в сером круге слева, название (белый жирный), теги (серый), стрелка →
- Клик → экран города

---

## Экран 2 — Услуги

### Строка поиска
- «Что ищете?» — поле с тёмно-серым фоном, лупа слева
- Поиск по названию и описанию партнёров с синонимами: «кофе»=coffee, «массаж»=massage, «няня»=nanny, «обмен»=exchange, «пляж»=beaches

### Сетка услуг 3×3

| # | Услуга | Цвет фона | Иконка | Подзаголовок |
|---|--------|----------|--------|-------------|
| 1 | Экскурсии | красный | 🌴 пальма | Туры и поездки |
| 2 | Трансфер | синий | 🚗 машина | Авто и такси |
| 3 | Vinpearl | зелёный | 🎡 колесо | Проживание и билеты |
| 4 | Travel Chat | золотой | 💬 облачко | Чат для туристов |
| 5 | Обмен валют | бирюзовый | 💲 $ | Лучший курс |
| 6 | Билеты | фиолетовый | 🎫 билет | Бронь билетов |
| 7 | eSIM | синий | 📱 трубка | Оставайся на связи |
| 8 | Fast Track | красный | ✈ самолёт | Быстрый проход |
| 9 | Доставка еды | оранжевый | 🛵 скутер | Рестораны на дом |

Каждая карточка ведёт на соответствующий список.

### Успей забронировать
- Заголовок + «Смотреть все →» (оранжевый)
- Горизонтальный скролл карточек экскурсий с фото, названием, «Экскурсия», ценой «от 72$»

### Гайд по Нячангу
- Заголовок + «Все категории →» (оранжевый)
- Горизонтальный скролл: Рестораны, Спа, Такси, Детские центры, Спорт

---

## Экран 3 — Гайд

### Все места
- Сетка категорий (5 в ряд, квадратные карточки, тёмно-серые, белая иконка + название):
  Рестораны, Спа, Такси, Детские центры, Спорт, Салоны красоты, Пляжи, Медицина, Торговые центры, Достопримечательности, Рынки
- Клик → список мест категории

### Список мест категории
- Фильтр по городу (пилюли: Нячанг, Дананг, Фукуок, Все)
- Карточки: фото 80×80 слева, название, адрес, ★ рейтинг, расстояние, теги
- Клик → карточка места

---

## Экскурсии (открываются из Таба 2 «Услуги»)

⚠️ ВАЖНО: Экран «Экскурсии» НЕ является табом в BottomNavigationBar. Он открывается из Таба 2 (Услуги) по клику на карточку «Экскурсии» в сетке 3×3. Таб 4 — это «Билеты» (TicketsScreen).

### Фильтр
- Кнопка с красной обводкой: 📍 город + счётчик «16»

### Список
Карточки с фото слева + детали справа:
- Название (белый жирный)
- ★ 5.0 (жёлтая звезда)
- Описание (2 строки, серый, многоточие)
- «Комфортный трансфер · Русский гид» (иконка ◆)
- Цена «от 72$» (оранжевый жирный)
- ♡ избранное (контур сердца, сохраняется локально)

Клик → детальная экскурсия.

---

## ⚙️ Кнопки действий под карточкой партнёра

На ВСЕХ карточках (экскурсии, рестораны, места, услуги) внизу — фиксированная панель с кнопками. **Никаких inline-ссылок в тексте. Только кнопки.**

### Состав по категориям

**Экскурсии, трансфер, отели, медицина, фото, няня, бьюти:**
- «🛍 Заказать» (оранжевая, основная) → deeplink Telegram: `https://t.me/username?text=Здравствуйте! Я из Viet Live, хочу узнать подробнее`
- «📍 На карте» (серая) → Google/Apple Maps
- «💬 Связаться» (серая) → Telegram-чат

**Пляжи и еда (кафе/рестораны):**
- «📍 На карте» — основная
- «Заказать» НЕТ

**Обмен валют, SIM-карты, залог:**
- «🛍 Заказать»
- «📍 На карте» НЕТ

### Навигация (если в категории >1 партнёра)
- «◀ Назад» / «▶ Вперёд» — листать
- «🔙 К списку» — в категорию
- «🔙 В меню» — на главную

### После нажатия «Заказать»
- «📍 На карте» убирается
- Остаются только навигационные

---

## 📝 Формат карточки партнёра

Жёсткие правила из @Vietlivebot:

```
НАЗВАНИЕ
────
Описание. Несколько секций с заголовками и текстом.

Списки через длинное тире:
— пункт 1
— пункт 2

Пустая строка между секциями.

📍 Заказать: нажмите «🛍 Заказать» внизу — менеджер ответит в течение 15 минут.
```

Запрещено: `✅`, `⭐`, `👇`, `•`, `*жирный*`, `_курсив_`, markdown-форматирование, двойные переносы строк. Только чистый текст. Скидка: «Скажи Линь — получи скидку 🎁».

Контакт партнёра в БД: `https://t.me/username||https://maps.google.com/...`

---

## 🏙️ Города и категории

### Города
Нячанг (основной), Дананг, Фукуок, Хошимин, Ханой, Далат, Муйне.

- Город выбирается при первом запуске и в настройках
- После выбора — весь контент фильтруется по городу
- Кнопка «📍 Сменить город» в меню

### 15 категорий
экскурсии, пляжи, еда, няня, массаж, аренда жилья, SIM-карта, кофе, обмен валют, залог, аренда байков, досуг, медицина, фото, бьюти-мастера

Бьюти: подменю «💇 Волосы» / «💅 Ногти»

---

## 🔥 VIP-размещение

- Партнёр покупает VIP (150⭐ / 30 дн → денежный платёж)
- VIP показываются первыми в категории с меткой «🔥»
- На главной: блок «🔥 Сегодня рекомендуем»

---

## 👤 Профиль

### Карточка
- Оранжевый круг с иконкой человека
- «Гость» (белый жирный)
- «Viet Live · Ваш гид по Вьетнаму» (серый)
- «Войдите, чтобы сохранять избранное и оформлять заявки»
- Кнопка Google-входа: белая, логотип G + «Войти через Google»

### Настройки
- 🟦📍 Город → «Сменить >»
- 🟣🌐 Язык → переключатель RU | EN | KZ
- 🟢🎨 Тема → переключатель ☀ | 🌙

### Информация
- ℹ️ О нас
- 💼 Партнёрам
- ⭐ Оставить отзыв

### Футер
«Viet Live» / «Версия 1.0.0»

---

## 📦 Внутренние экраны

### Экран города
- Hero-фото, название, описание
- Счётчик: «16 экскурсий · 23 ресторана · 5 отелей»
- Блоки: услуги, популярные экскурсии, рестораны

### Детальная экскурсия
- Галерея фото (свайп)
- ★ 5.0 (12 отзывов) · Цена «от 72$»
- ────
- Полное описание (3-5 абзацев)
- Что входит: список через «—»
- Что взять: список через «—»
- Продолжительность
- ────
- Кнопка «🛍 Забронировать» (оранжевая, закреплена внизу)
- ♡ в AppBar

### Форма бронирования
- Название экскурсии, дата (календарь), кол-во человек (степпер ±)
- Итого: цена × человек (автопересчёт)
- Поля: Имя, Телефон (маска), Комментарий
- «Отправить заявку» → «✅ Заявка отправлена! Свяжемся в течение 15 минут.»

### Доставка еды
- Список: поиск, фильтры-пилюли по кухням, карточки ресторанов
- Меню: фото, разделы, позиции с «+», корзина внизу
- Заказ: состав, адрес, телефон, оплата (нал/карта) → «✅ Заказ принят! 30-45 минут.»
- Доставка: 30 000₫

### Обмен валют
- Таблица: USD/RUB/EUR/USDT → VND (флаг, покупка, продажа)
- Калькулятор: «У меня есть» → «Я получу» (VND)
- Кнопка «💬 Связаться для обмена» → Telegram
- «Обмен наличных и криптовалют. Доставка по Нячангу.»

### Трансфер
- Форма: Откуда → Куда (автодополнение), дата+время, класс авто (Эконом/Комфорт/Бизнес/Минивэн — пилюли с ценой), пассажиры (±)
- Поля: Имя, Телефон, Рейс
- «Заказать трансфер»

### Билеты
- Вкладки: ✈ Авиа / 🚌 Автобус / 🚂 Поезд
- Поиск: Откуда → Куда, Дата, Пассажиры
- Результаты: карточки маршрутов (перевозчик, время, стыковки, цена)
- Клик → детали → «Купить» (внешняя ссылка)
- Заглушка: «Скоро запуск. Оставьте заявку.»

### Travel Chat
- Интерфейс чата: поддержка слева, пользователь справа
- Приветствие: «👋 Здравствуйте! Я ваш помощник по Вьетнаму...»
- Пилюли-подсказки: Экскурсии, Трансфер, Погода, Обмен валют, Рестораны
- «Скоро AI-помощник. Пока отвечаем вручную в течение 5 минут.»

### Карточка места (гайд)
- Галерея фото, название, ★ рейтинг
- Адрес (→ карты), Часы работы, Телефон
- Описание, Удобства (иконки)
- Кнопки: «📍 На карте», «💬 Связаться»

---

## 🔗 Партнёрская система

### Кабинет партнёра
- Статистика: просмотры, заказы, конверсия (30 дней)
- Редактирование: описание, фото, контакты → модерация админу
- QR-код со ссылкой на карточку

### Рефералы гидов
- Админ создаёт гида: имя + код
- Гид получает ссылку и QR
- При регистрации пользователя записывается какой гид привёл
- При заказе — +1 к статистике гида
- Статистика: регистрации / заказы / конверсия

### Claim-коды
- Каждый партнёр получает код
- Вводит в приложении → активирует кабинет
- Без claim'а заказы не привязываются

---

## 🌐 Языки

- RU (русский, основной)
- EN (английский)
- KZ (казахский)

Переключатель в профиле. Строки в JSON: `ru.json`, `en.json`, `kz.json`.

---

## 📊 Данные для первого запуска

**29 партнёров из @Vietlivebot должны быть в приложении с первого дня.** Структура:

```json
{
  "partners": [
    {
      "id": 1,
      "name": "Обзорная экскурсия по Нячангу",
      "category": "excursions",
      "city": "Нячанг",
      "description": "Полный день...",
      "contact": "https://t.me/main_tour||https://maps.google.com/...",
      "photos": ["url1.jpg", "url2.jpg"],
      "price": 72,
      "rating": 5.0,
      "reviews": 12,
      "discount": "Скажи Линь — получи скидку 🎁",
      "is_vip": true,
      "duration": "1 день / 8:00–18:00",
      "includes": ["Трансфер", "Русский гид", "Обед"],
      "what_to_bring": ["Вода", "Крем от загара", "Удобная обувь"]
    }
  ],
  "cities": ["Нячанг", "Дананг", "Фукуок", "Хошимин", "Ханой", "Далат", "Муйне"],
  "restaurants": [
    {
      "name": "Pho Viet",
      "cuisine": "Вьетнамская",
      "rating": 4.8,
      "delivery_time": "30-45 мин",
      "min_order": 200000,
      "delivery_fee": 30000,
      "menu": [
        {"name": "Фо Бо", "description": "Суп с говядиной", "price": 85000, "category": "Супы", "photo": "pho.jpg"}
      ]
    }
  ]
}
```

---

## 🎨 Тема

- Фон: #0D0D0D
- Карточки: #1A1A1A
- Текст: #FFFFFF (белый), #999999 (серый)
- Акцент: #FF6B00 (оранжевый)
- Рейтинг: #FFD700 (жёлтый)
- Border-radius: 12–16px
- Скроллы плавные, pull-to-refresh на списках
- Избранное: SharedPreferences локально

---

## 🛠️ Технический бриф для Codex

### Что использовать (обязательно)

**Структура проекта:**
```
vietlive/
├── lib/
│   ├── main.dart                    ← точка входа
│   ├── app.dart                     ← MaterialApp + тема + роутинг
│   ├── theme/
│   │   ├── app_theme.dart           ← все цвета, текстовые стили, константы
│   │   └── app_images.dart          ← URL-заглушки picsum.photos для фото
│   ├── models/
│   │   ├── partner.dart             ← Partner, City, Category
│   │   ├── restaurant.dart          ← Restaurant, MenuItem
│   │   └── order.dart               ← Booking, FoodOrder, TransferOrder
│   ├── data/
│   │   ├── partners.json            ← 29 партнёров
│   │   ├── restaurants.json         ← 15-20 ресторанов
│   │   ├── cities.json              ← 7 городов + поле weather
│   │   ├── categories.json          ← 15 категорий
│   │   ├── exchange_rates.json      ← курсы валют (USD/RUB/EUR/USDT → VND)
│   │   ├── responses.json           ← моковые ответы для Travel Chat
│   │   └── i18n/
│   │       ├── ru.json              ← русский основной
│   │       ├── en.json              ← английский
│   │       └── kz.json              ← казахский
│   ├── providers/
│   │   ├── app_state.dart           ← город, язык, тема, избранное
│   │   └── cart_provider.dart       ← корзина доставки еды
│   ├── screens/
│   │   ├── home_screen.dart
│   │   ├── services_screen.dart
│   │   ├── guide_screen.dart
│   │   ├── excursions_screen.dart
│   │   ├── tickets_screen.dart
│   │   ├── profile_screen.dart
│   │   ├── city_screen.dart
│   │   ├── excursion_detail_screen.dart
│   │   ├── booking_screen.dart
│   │   ├── food_delivery/
│   │   │   ├── restaurant_list_screen.dart
│   │   │   ├── menu_screen.dart
│   │   │   └── order_screen.dart
│   │   ├── exchange_screen.dart
│   │   ├── transfer_screen.dart
│   │   ├── travel_chat_screen.dart
│   │   ├── guide_category_screen.dart
│   │   ├── place_detail_screen.dart
│   │   └── partner/
│   │       ├── partner_cabinet_screen.dart   ← Кабинет партнёра (фаза 5)
│   │       ├── referral_screen.dart          ← Рефералы гидов (фаза 5)
│   │       └── claim_code_screen.dart        ← Активация claim-кода (фаза 5)
│   └── widgets/
│       ├── app_header.dart          ← логотип + город-погода
│       ├── partner_card.dart        ← карточка партнёра с кнопками
│       ├── excursion_card.dart      ← карточка экскурсии
│       ├── restaurant_card.dart     ← карточка ресторана
│       ├── city_card.dart           ← карточка города
│       ├── service_grid.dart        ← сетка услуг 3×3
│       ├── promo_banner.dart        ← акция -25%
│       ├── horizontal_scroll.dart   ← «Успей забронировать»
│       ├── star_rating.dart         ← ★ рейтинг
│       └── price_tag.dart           ← ценник
├── assets/
│   ├── images/                      ← фото партнёров, городов, hero
│   └── icons/                       ← SVG-иконки услуг
├── pubspec.yaml
├── README.md
└── AGENTS.md
```

**pubspec.yaml (обязательные пакеты):**
```yaml
dependencies:
  flutter:
    sdk: flutter
  provider: ^6.1.0           # state management
  go_router: ^14.0.0         # навигация
  shared_preferences: ^2.2.0 # избранное, город, язык
  flutter_svg: ^2.0.0        # SVG-иконки
  url_launcher: ^6.2.0       # открытие Telegram, карт
  intl: ^0.19.0              # форматирование валют, дат
  cached_network_image: ^3.3.0 # кеширование фото
  shimmer: ^3.0.0            # скелетоны при загрузке
  flutter_rating_bar: ^4.0.0 # звёзды рейтинга
  carousel_slider: ^4.2.0    # галерея фото (свайп)
  google_sign_in: ^6.2.1     # Google-вход (ТОЛЬКО UI-кнопка в MVP, см. ниже)
  qr_flutter: ^4.1.0         # QR-код в кабинете партнёра
  mask_text_input_formatter: ^2.9.0  # маска телефона в формах
  share_plus: ^7.2.1         # поделиться карточкой партнёра
```

**⚠️ КРИТИЧНО: assets в pubspec.yaml.** Без этого `rootBundle.loadString()` крашнет приложение при старте:
```yaml
flutter:
  uses-material-design: true
  assets:
    - assets/data/
    - assets/data/i18n/
    - assets/icons/
```

**⚠️ Google Sign-In для MVP — упростить:**
- Реализуй ТОЛЬКО UI-кнопку «Войти через Google» (белая, логотип G, чёрный текст)
- При нажатии показывай `SnackBar`: «Авторизация будет доступна в следующем обновлении»
- НЕ вызывай `GoogleSignIn.signIn()` без конфигурации
- НЕ добавляй `google-services.json` (его нет в проекте)
- После «входа» просто меняй «Гость» → «Пользователь» локально в AppState
- Полноценный OAuth — позже через Firebase

**State management:** Provider (один AppState на все настройки + отдельные провайдеры для корзины и брони)

**Роутинг:** GoRouter с именованными маршрутами:
```
/                     → HomeScreen
/services             → ServicesScreen
/guide                → GuideScreen
/excursions           → ExcursionsScreen
/excursions/:id       → ExcursionDetailScreen
/excursions/:id/book  → BookingScreen
/tickets              → TicketsScreen
/profile              → ProfileScreen
/city/:name           → CityScreen
/food                 → RestaurantListScreen
/food/:id             → MenuScreen
/food/:id/order       → OrderScreen
/exchange              → ExchangeScreen
/transfer              → TransferScreen
/chat                  → TravelChatScreen
/guide/:category       → GuideCategoryScreen
/place/:id             → PlaceDetailScreen
```

**Цвета (app_theme.dart):**
```dart
class AppColors {
  static const background = Color(0xFF0D0D0D);
  static const card = Color(0xFF1A1A1A);
  static const text = Color(0xFFFFFFFF);
  static const textSecondary = Color(0xFF999999);
  static const accent = Color(0xFFFF6B00);
  static const star = Color(0xFFFFD700);
  static const red = Color(0xFFE53935);
  static const green = Color(0xFF43A047);
}
```

### Data models (Dart) — полный набор

```dart
class Partner { /* см. выше */ }

class City {
  final String name;
  final String emoji;       // "🏝", "🌴", "🏖"
  final List<String> tags;  // ["Пляжи", "Экскурсии", "Приключения"]
  final String heroImage;   // picsum URL
  final Weather? weather;
}

class Weather {
  final int temperature;    // 30
  final String icon;        // "🌩", "☀️", "🌧"
}

class Category {
  final String id;          // "excursions"
  final String icon;        // "🌴"
  final String color;       // "#E53935"
}

class Booking {
  final int excursionId;
  final DateTime date;
  final int persons;
  final String name;
  final String phone;
  final String? comment;
  final double totalPrice;
}

class FoodOrder {
  final int restaurantId;
  final List<CartItem> items;
  final String address;
  final String phone;
  final String paymentMethod; // "cash" | "card"
  final int deliveryFee;
  final int totalPrice;
}

class CartItem {
  final MenuItem item;
  int quantity;
}

/// Обёртки для JSON (ОБЯЗАТЕЛЬНЫ):
class PartnerList {
  final List<Partner> partners;
  PartnerList({required this.partners});
  factory PartnerList.fromJson(Map<String, dynamic> json) => PartnerList(
    partners: (json['partners'] as List).map((e) => Partner.fromJson(e)).toList(),
  );
}
// Аналогично: RestaurantList, CityList, CategoryList
```

### ⚠️ КРИТИЧНО: CartProvider — структура

```dart
class CartProvider extends ChangeNotifier {
  final SharedPreferences _prefs;
  List<CartItem> _items = [];

  CartProvider({required SharedPreferences prefs}) : _prefs = prefs { _loadCart(); }

  List<CartItem> get items => List.unmodifiable(_items);
  int get totalCount => _items.fold(0, (sum, i) => sum + i.quantity);
  int get totalPrice => _items.fold(0, (sum, i) => sum + (i.item.price * i.quantity));

  void addItem(MenuItem menuItem) {
    final idx = _items.indexWhere((i) => i.item.name == menuItem.name);
    if (idx >= 0) { _items[idx].quantity++; }
    else { _items.add(CartItem(item: menuItem, quantity: 1)); }
    _saveCart();
    notifyListeners();
  }

  void removeItem(MenuItem menuItem) {
    _items.removeWhere((i) => i.item.name == menuItem.name);
    _saveCart();
    notifyListeners();
  }

  void clear() { _items.clear(); _saveCart(); notifyListeners(); }

  void _saveCart() {
    final json = _items.map((i) => {'name': i.item.name, 'price': i.item.price, 'qty': i.quantity}).toList();
    _prefs.setString('cart', jsonEncode(json));
  }

  void _loadCart() {
    final s = _prefs.getString('cart');
    if (s == null) return;
    try {
      final list = jsonDecode(s) as List;
      _items = list.map((j) => CartItem(item: MenuItem(name: j['name'], price: j['price']), quantity: j['qty'])).toList();
    } catch (_) { _items = []; }
  }
}
```

### ⚠️ КРИТИЧНО: Favorite — логика в AppState

Добавить в класс `AppState`:

```dart
Set<int> _favorites = {};
Set<int> get favorites => _favorites;
bool isFavorite(int id) => _favorites.contains(id);

void toggleFavorite(int id) {
  _favorites.contains(id) ? _favorites.remove(id) : _favorites.add(id);
  _prefs.setStringList('favorites', _favorites.map((e) => e.toString()).toList());
  notifyListeners();
}

void _loadFavorites() {
  final list = _prefs.getStringList('favorites');
  if (list != null) _favorites = list.map(int.parse).toSet();
}
```

Вызвать `_loadFavorites()` в конструкторе AppState (после `_loadInitialData()`).

### ⚠️ i18n — простая реализация (БЕЗ генерации .arb)

```dart
class AppLocalizations {
  final Map<String, dynamic> _data;
  AppLocalizations(this._data);

  String t(String key) {
    final keys = key.split('.');
    dynamic val = _data;
    for (final k in keys) {
      if (val is Map) val = val[k];
      else return key;
    }
    return val?.toString() ?? key;
  }

  static AppLocalizations of(BuildContext context) => Localizations.of<AppLocalizations>(context, AppLocalizations)!;
}

class AppLocalizationsDelegate extends LocalizationsDelegate<AppLocalizations> {
  const AppLocalizationsDelegate();

  @override
  bool isSupported(Locale locale) => ['ru', 'en', 'kz'].contains(locale.languageCode);

  @override
  Future<AppLocalizations> load(Locale locale) async {
    final json = await rootBundle.loadString('assets/data/i18n/${locale.languageCode}.json');
    return AppLocalizations(jsonDecode(json));
  }

  @override
  bool shouldReload(covariant LocalizationsDelegate old) => false;
}
```

В MaterialApp:
```dart
localizationsDelegates: const [
  AppLocalizationsDelegate(),
  GlobalMaterialLocalizations.delegate,
  GlobalWidgetsLocalizations.delegate,
  GlobalCupertinoLocalizations.delegate,
],
locale: Locale(appState.language),
supportedLocales: const [Locale('ru'), Locale('en'), Locale('kz')],
```

Использование: `Text(AppLocalizations.of(context).t('home.hero_title'))`
```

### AppConstants (обязательно)

Добавь в `app_theme.dart`. Никаких магических чисел в коде:

```dart
class AppConstants {
  static const double paddingXS = 4.0;
  static const double paddingS = 8.0;
  static const double paddingM = 16.0;
  static const double paddingL = 24.0;
  static const double paddingXL = 32.0;
  static const double radiusS = 8.0;
  static const double radiusM = 12.0;
  static const double radiusL = 16.0;
  static const double cardImageSize = 80.0;
  static const double avatarSize = 64.0;
  static const double iconSize = 24.0;
  static const Duration animationFast = Duration(milliseconds: 200);
  static const Duration animationNormal = Duration(milliseconds: 300);
  static const int maxVipOnHome = 5;
  static const int maxDescriptionLines = 2;
}
```

### ⚠️ КРИТИЧНО: AndroidManifest.xml и Info.plist

Без этого `url_launcher` крашнет приложение на Android 11+ при открытии Telegram и карт:

**android/app/src/main/AndroidManifest.xml** — внутри `<manifest>`:
```xml
<queries>
  <intent>
    <action android:name="android.intent.action.VIEW" />
    <data android:scheme="https" />
  </intent>
  <intent>
    <action android:name="android.intent.action.VIEW" />
    <data android:scheme="tg" />
  </intent>
</queries>
```

**ios/Runner/Info.plist** — внутри `<dict>`:
```xml
<key>LSApplicationQueriesSchemes</key>
<array>
  <string>tg</string>
  <string>https</string>
  <string>http</string>
</array>
```

### ⚠️ КРИТИЧНО: GoRouter ShellRoute

Используй ShellRoute для табов — иначе состояние теряется при переходах.

**⚠️ НЕ создавай внешний GoRoute с path: '/' — это вызовет конфликт с ShellRoute.**

Правильный синтаксис:
- Все 5 табов (`/`, `/services`, `/guide`, `/tickets`, `/profile`) — ВНУТРИ ShellRoute
- Используй `NoTransitionPage` для табов (убирает анимацию переключения)
- Вложенные маршруты (`/excursions`, `/food` и т.д.) — ОТДЕЛЬНО от ShellRoute, без BottomNavigationBar

```dart
final router = GoRouter(
  initialLocation: '/',
  routes: [
    ShellRoute(
      builder: (context, state, child) => MainScaffold(child: child),
      routes: [
        GoRoute(path: '/', pageBuilder: (_, __) => const NoTransitionPage(child: HomeScreen())),
        GoRoute(path: '/services', pageBuilder: (_, __) => const NoTransitionPage(child: ServicesScreen())),
        GoRoute(path: '/guide', pageBuilder: (_, __) => const NoTransitionPage(child: GuideScreen())),
        GoRoute(path: '/tickets', pageBuilder: (_, __) => const NoTransitionPage(child: TicketsScreen())),
        GoRoute(path: '/profile', pageBuilder: (_, __) => const NoTransitionPage(child: ProfileScreen())),
      ],
    ),
    // Вложенные маршруты ОТДЕЛЬНО от ShellRoute (НЕТ BottomNavigationBar):
    GoRoute(path: '/excursions', builder: (_, __) => const ExcursionsScreen()),
    GoRoute(path: '/excursions/:id', builder: (_, state) => ExcursionDetailScreen(id: int.parse(state.pathParameters['id']!))),
    GoRoute(path: '/excursions/:id/book', builder: (_, state) => BookingScreen(id: int.parse(state.pathParameters['id']!))),
    GoRoute(path: '/city/:name', builder: (_, state) => CityScreen(name: state.pathParameters['name']!)),
    // Партнёрские экраны (фаза 5 — UI-заглушки):
    GoRoute(path: '/partner/cabinet', builder: (_, __) => const PartnerCabinetScreen()),
    GoRoute(path: '/partner/referral', builder: (_, __) => const ReferralScreen()),
    GoRoute(path: '/partner/claim', builder: (_, __) => const ClaimCodeScreen()),
    // ... остальные маршруты
  ],
);
```

`MainScaffold` — виджет с `Scaffold` + `BottomNavigationBar`. На детальных экранах BottomNavigationBar скрывается автоматически (они вне ShellRoute).

```dart
class MainScaffold extends StatelessWidget {
  final Widget child;
  const MainScaffold({required this.child});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: child,
      bottomNavigationBar: BottomNavigationBar(
        type: BottomNavigationBarType.fixed,
        backgroundColor: AppColors.background,
        selectedItemColor: AppColors.accent,
        unselectedItemColor: AppColors.textSecondary,
        currentIndex: _calculateSelectedIndex(context),
        onTap: (index) => _onItemTapped(index, context),
        items: const [
          BottomNavigationBarItem(icon: Icon(Icons.home), label: 'Главная'),
          BottomNavigationBarItem(icon: Icon(Icons.grid_view), label: 'Услуги'),
          BottomNavigationBarItem(icon: Icon(Icons.menu_book), label: 'Гайд'),
          BottomNavigationBarItem(icon: Icon(Icons.confirmation_number), label: 'Билеты'),
          BottomNavigationBarItem(icon: Icon(Icons.person), label: 'Профиль'),
        ],
      ),
    );
  }

  int _calculateSelectedIndex(BuildContext context) {
    final location = GoRouterState.of(context).uri.toString();
    if (location == '/') return 0;
    if (location.startsWith('/services')) return 1;
    if (location.startsWith('/guide')) return 2;
    if (location.startsWith('/tickets')) return 3;
    if (location.startsWith('/profile')) return 4;
    return 0;
  }

  void _onItemTapped(int index, BuildContext context) {
    switch (index) {
      case 0: context.go('/'); break;
      case 1: context.go('/services'); break;
      case 2: context.go('/guide'); break;
      case 3: context.go('/tickets'); break;
      case 4: context.go('/profile'); break;
    }
  }
}
```

### ⚠️ КРИТИЧНО: AppState — асинхронная инициализация

JSON загружается асинхронно, MaterialApp строится синхронно. Без этого — пустой экран при старте.

**⚠️ ОБЯЗАТЕЛЬНО инициализируй SharedPreferences ПЕРЕД AppState:**

```dart
// main.dart
void main() async {
  WidgetsFlutterBinding.ensureInitialized();

  // SharedPreferences ДОЛЖЕН быть инициализирован ПЕРЕД AppState
  final prefs = await SharedPreferences.getInstance();

  final appState = AppState(prefs: prefs);
  await appState.loadInitialData();

  runApp(
    MultiProvider(
      providers: [
        ChangeNotifierProvider.value(value: appState),
        ChangeNotifierProvider(create: (_) => CartProvider(prefs: prefs)),
      ],
      child: const VietLiveApp(),
    ),
  );
}

// app_state.dart
class AppState extends ChangeNotifier {
  final SharedPreferences _prefs;

  AppState({required SharedPreferences prefs}) : _prefs = prefs {
    _city = _prefs.getString('city') ?? 'Нячанг';
    _language = _prefs.getString('language') ?? 'ru';
    _theme = _prefs.getString('theme') ?? 'dark';
  }

  Future<void> loadInitialData() async {
    _isLoading = true;
    notifyListeners();
    try {
      final json = await rootBundle.loadString('assets/data/partners.json');
      _partners = PartnerList.fromJson(jsonDecode(json));
      _isLoading = false;
      _hasError = false;
    } catch (e) {
      _isLoading = false;
      _hasError = true;
      _errorMessage = e.toString();
    }
    notifyListeners();
  }

  void setCity(String city) {
    _city = city;
    _prefs.setString('city', city);
    notifyListeners();
  }
}
```

### ⚠️ КРИТИЧНО: json_serializable + build_runner

**1. Добавь в pubspec.yaml:**
```yaml
dev_dependencies:
  flutter_test:
    sdk: flutter
  build_runner: ^2.4.0
  json_serializable: ^6.7.0
```

**2. В моделях используй аннотации:**
```dart
import 'package:json_annotation/json_annotation.dart';

part 'partner.g.dart'; // ОБЯЗАТЕЛЬНО

@JsonSerializable()
class Partner {
  final int id;
  final String name;

  const Partner({required this.id, required this.name});

  factory Partner.fromJson(Map<String, dynamic> json) => _$PartnerFromJson(json);
  Map<String, dynamic> toJson() => _$PartnerToJson(this);
}
```

**3. После создания моделей запусти:**
```bash
flutter pub run build_runner build --delete-conflicting-outputs
```

Это сгенерирует `*.g.dart` файлы. Без них приложение НЕ скомпилируется.

### ⚠️ КРИТИЧНО: Разделение BottomNavigationBar и BottomAppBar

Две панели внизу экрана НЕ должны показываться одновременно:

1. **BottomNavigationBar (табы)** — на главных экранах (Home, Services, Guide, Tickets, Profile). Реализуется через ShellRoute.

2. **BottomAppBar (кнопки действий «Заказать»/«На карте»)** — ТОЛЬКО на детальных экранах (ExcursionDetailScreen, PlaceDetailScreen). НЕ на списках.

3. На детальных экранах BottomNavigationBar скрывается автоматически (они вне ShellRoute).

```dart
class ExcursionDetailScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: const Text('Экскурсия')),
      body: /* галерея + описание */,
      bottomNavigationBar: BottomAppBar(
        child: Row(children: [
          Expanded(child: ElevatedButton(onPressed: _onBook, child: const Text('🛍 Заказать'))),
          const SizedBox(width: 8),
          Expanded(child: OutlinedButton(onPressed: _onMap, child: const Text('📍 На карте'))),
        ]),
      ),
    );
  }
}
```

### ⚠️ КРИТИЧНО: url_launcher fallback для Telegram

Используй `https://` (не `tg://`) — универсальный deeplink:

```dart
Future<void> openTelegram(String username, [String? message]) async {
  final url = message != null
      ? 'https://t.me/$username?text=${Uri.encodeComponent(message)}'
      : 'https://t.me/$username';

  final uri = Uri.parse(url);
  if (await canLaunchUrl(uri)) {
    await launchUrl(uri, mode: LaunchMode.externalApplication);
  } else {
    // Fallback: открыть в браузере
    await launchUrl(uri, mode: LaunchMode.externalApplication);
    if (context.mounted) {
      ScaffoldMessenger.of(context).showSnackBar(
        const SnackBar(content: Text('Установите Telegram для связи')),
      );
    }
  }
}
```

`https://t.me/...` работает даже если Telegram не установлен — откроется в браузере.

### Shimmer — когда использовать

- ✅ ТОЛЬКО для `CachedNetworkImage.placeholder` (удалённые фото грузятся с задержкой)
- ❌ НЕ для JSON-данных (локальные, загружаются мгновенно)
- ❌ НЕ для списков партнёров/ресторанов — показывай сразу данные или empty state

```dart
CachedNetworkImage(
  imageUrl: url,
  placeholder: (_, __) => Shimmer.fromColors(
    baseColor: AppColors.card,
    highlightColor: AppColors.textSecondary.withOpacity(0.1),
    child: Container(color: AppColors.card),
  ),
  errorWidget: (_, __, ___) => const Icon(Icons.broken_image, color: AppColors.textSecondary),
)
```

### Smoke-тесты (минимум 5)

Создай `test/widget_test.dart`:

```dart
void main() {
  testWidgets('App opens and shows HomeScreen', (tester) async {
    await tester.pumpWidget(const VietLiveApp());
    expect(find.text('Главная'), findsOneWidget);
  });

  testWidgets('Bottom navigation has 5 tabs', (tester) async {
    await tester.pumpWidget(const VietLiveApp());
    expect(find.byType(BottomNavigationBar), findsOneWidget);
    expect(find.text('Главная'), findsOneWidget);
    expect(find.text('Услуги'), findsOneWidget);
    expect(find.text('Гайд'), findsOneWidget);
    expect(find.text('Билеты'), findsOneWidget);
    expect(find.text('Профиль'), findsOneWidget);
  });

  testWidgets('City filter works', (tester) async { /* tap city → check filtered content */ });
  testWidgets('Favorite toggle saves', (tester) async { /* tap ♡ → verify SharedPreferences */ });
  testWidgets('Empty state shows when no data', (tester) async { /* verify "Пока ничего нет" */ });
}
```

### README.md и AGENTS.md

**README.md:**
```markdown
# Viet Live
Мобильное приложение для русскоязычных туристов во Вьетнаме.

## Стек
Flutter 3.x | Provider | GoRouter | JSON

## Запуск
flutter pub get && flutter run

## Структура
lib/ (screens, widgets, models, providers, theme, data) | assets/ (data, icons)

## Фазы
1. Каркас → 2. Данные → 3. Главные экраны → 4. Внутренние → 5. Партнёры → 6. MVP
```

**AGENTS.md:**
```markdown
# AI Agent Instructions

## Правила
- Одна фаза = один PR. Не смешивать.
- Максимум 300 строк на файл. Выноси в widgets/.
- Перед коммитом: `flutter analyze` без ошибок.
- Никакого хардкода русского текста — используй i18n.
- JSON-парсинг через json_serializable.

## Стек
Provider | GoRouter | CachedNetworkImage | json_serializable | flutter_rating_bar

## Контакты
По вопросам: @Vietlivebot (Telegram)
```

### Порядок сборки (MVP)

**Фаза 1 — каркас (сделать ПЕРВЫМ):**
1. `flutter create vietlive` + pubspec.yaml
2. `app_theme.dart` — все цвета и стили
3. `main.dart` + `app.dart` — MaterialApp, GoRouter, Provider
4. `app_header.dart` — логотип + город/погода
5. BottomNavigationBar с 5 табами — переключение работает
6. Все 5 экранов — заглушки с заголовками

**Фаза 2 — данные:**
7. JSON-файлы: partners.json, restaurants.json, cities.json
8. Модели: Partner, City, Restaurant, MenuItem
9. AppState — загрузка JSON, фильтрация по городу, язык

**Фаза 3 — экраны:**
10. Главная: Hero, акция, VIP, города
11. Услуги: поиск, сетка 3×3, Успей забронировать, Гайд по Нячангу
12. Гайд: сетка категорий 5 в ряд + список мест
13. Экскурсии: фильтр по городу, список карточек
14. Профиль: карточка, настройки, информация

**Фаза 4 — внутренние экраны:**
15. Экран города
16. Детальная экскурсия + форма бронирования
17. Доставка еды: список → меню → заказ
18. Обмен валют, Трансфер
19. Билеты, Travel Chat

**Фаза 5 — партнёрская система (ТОЛЬКО UI-заглушки):**
20. Кабинет партнёра (статистика с моковыми цифрами, форма редактирования без сохранения)
21. Рефералы гидов (UI с моковыми данными)
22. VIP-логика (моковые данные, фильтр isVip=true в JSON)

**⚠️ ВАЖНО для Фазы 5:** Реализуй ТОЛЬКО UI-интерфейсы с хардкодными данными. НЕ пиши код для бэкенда, claim-кодов, Firebase/Supabase и реальной аналитики. Вся «логика» — чтение флагов из локального JSON. Сохранение, регистрация, учёт статистики — будут позже через API.

### Правила для Codex

1. **Одна фаза — один Pull Request.** Не смешивать.
2. **Каждый экран — отдельный файл.** Не пихать всё в main.dart. Максимум 300 строк на файл — если виджет разрастается, выноси части в `widgets/`.
3. **Сначала каркас и навигация, потом наполнение.** Не рисовать красивый экран без роутинга.
4. **Данные сначала из JSON.** Не делать API-запросы пока нет бэкенда.
5. **Использовать готовые пакеты.** Не изобретать звёзды рейтинга и календарь.
6. **Локализация:** создай скелеты `ru.json`, `en.json`, `kz.json` с вложенностью по экранам. Пример структуры:
   ```json
   {
     "home": {"hero_title": "Всё для отдыха во Вьетнаме", "promo_title": "Специальное предложение!"},
     "services": {"search_hint": "Что ищете?", "grid_1": "Экскурсии"},
     "common": {"btn_order": "Заказать", "btn_map": "На карте", "btn_back": "Назад"}
   }
   ```
   Используй `flutter_localizations` или простой класс `AppLocalizations` с `LocalizationsDelegate`. Никакого хардкода русского текста в Dart.
7. **JSON-парсинг:** используй фабрики `fromJson()` + пакет `json_serializable` с `build_runner`. Не парси JSON руками — опечатки в ключах ломают всё.
8. **Обработка ошибок:** ВСЕ места загрузки данных (даже из локального JSON) оборачивай в try-catch. Если JSON не прочитался — показывай UI-заглушку с кнопкой «Повторить», НЕ крашь приложение (White Screen of Death).
9. **Provider:** никогда не вызывай `notifyListeners()` внутри `build()`. Для асинхронной загрузки используй флаги `isLoading`, `hasError` в AppState + `FutureBuilder` или `Selector`.
10. **Тёмная тема — дефолт.** Светлая опциональна, но не в MVP.
11. **Кнопки под карточкой — как описано.** Панель с кнопками (Заказать, На карте) должна быть зафиксирована внизу экрана в `SafeArea` (через `BottomAppBar` или `bottomSheet`), а НЕ скроллиться вместе с контентом карточки.
12. **Фото — remote URL.** Не тащить изображения в репозиторий.
13. **GoRouter:** при переходе по табам сохраняй состояние скролла. Не сбрасывай ScrollController при пересоздании виджета (используй `AutomaticKeepAliveClientMixin`).
14. **Проверять на Android 13 и iOS 16.** Не ниже.
15. **Поле contact:** парси через `split('||')` → `[0]` = Telegram deeplink, `[1]` = Maps URL. Если часть отсутствует — скрывай соответствующую кнопку.
16. **Deeplink в Telegram:** `final url = 'https://t.me/$username?text=${Uri.encodeComponent(message)}';`
17. **Форма бронирования:** при «Отправить заявку» — формируй deeplink в Telegram менеджера с текстом: `Заявка: [название], [дата], [N чел], [имя], [телефон]`. После открытия — snackbar «✅ Заявка отправлена».
18. **Корзина доставки еды:** иконка в AppBar с бейджем-счётчиком. Клик → bottom sheet со списком позиций, итогом и кнопкой «Оформить». Сохраняется между экранами через `CartProvider` (ChangeNotifier).
19. **Курсы валют:** захардкожены в `exchange_rates.json`. Структура: `{"USD": {"buy": 24500, "sell": 25000}}`. Обновляются раз в день вручную.
20. **Travel Chat:** при отправке сообщения → через 2 сек показывай моковый ответ из `responses.json` (выбирай по ключевым словам).
21. **Автодополнение в трансфере:** используй захардкоженный список локаций Нячанга (аэропорт Камрань, ж/д вокзал, популярные отели). НЕ подключай Google Places API.
22. **Empty states:** если в категории/городе нет данных — центрированный текст «Пока ничего нет 🔍» + кнопка «Сменить город». НЕ показывай пустой белый экран.
23. **VIP на главной:** бери из `partners.json` только тех у кого `is_vip == true` И `city == текущий город`. Лимит — 5 карточек.

### Правила UI (чтобы не накосячить с дизайном)

- **Сетка услуг 3×3:** используй `GridView.count(crossAxisCount: 3)` с `shrinkWrap: true` и `physics: NeverScrollableScrollPhysics()`. Сетка НЕ должна скроллиться отдельно — только общий скролл экрана.
- **Вложенные скроллы:** все `ListView` и `GridView` внутри `SingleChildScrollView` должны иметь `shrinkWrap: true` и `NeverScrollableScrollPhysics`.
- **Текст партнёра:** используй обычный `Text` с `maxLines` и `overflow: TextOverflow.ellipsis`. Для списков (через «—») используй `Column` с `Row` (иконка тире + Expanded текст), чтобы тире не уезжали на новую строку.
- **Разделитель «────»:** используй `Divider` или `Container(height: 1, color: AppColors.textSecondary)` — НЕ строку из тире.

### Что отдавать пользователю после каждой фазы

- APK-файл для установки
- Скриншоты новых экранов
- `flutter analyze` — без ошибок
- `flutter test` — хотя бы smoke-тесты

### Критерии готовности MVP

- [ ] Приложение открывается → Главный экран
- [ ] 5 табов переключаются
- [ ] Города фильтруют контент
- [ ] Экскурсии открываются → детальная → бронирование
- [ ] Доставка еды: ресторан → меню → корзина → заказ
- [ ] Обмен валют: таблица + калькулятор
- [ ] Язык переключается (RU/EN/KZ)
- [ ] Тема переключается (тёмная/светлая)
- [ ] Избранное сохраняется
- [ ] Telegram-кнопки открывают чат
- [ ] 29 партнёров в каталоге
- [ ] Пустые состояния отображаются корректно (не белый экран)
- [ ] Telegram deeplinks открываются с предзаполненным текстом
- [ ] QR-код в кабинете партнёра генерируется и отображается
- [ ] Маска телефона работает (+84 XXX XXX XXX)
- [ ] Google Sign-In открывает окно авторизации (даже без реального логина)
- [ ] Корзина доставки сохраняется при переходе между экранами

---

## 🚀 Как скармливать в Cloud Codex (стратегия ввода)

**Не отправляй весь промт одним сообщением.** AI потеряет фокус и начнёт галлюцинировать.

### Сообщение 1 — Каркас
> «Изучи контекст проекта. Создай: pubspec.yaml, app_theme.dart, app_images.dart, main.dart, app.dart, базовый GoRouter с 5 табами-заглушками, app_header.dart. Проверь `flutter analyze`. Жду подтверждения, что каркас компилируется».

### Сообщение 2 — Данные и модели
> «Создай JSON-файлы (partners, restaurants, cities, categories, exchange_rates, responses, i18n), модели Dart с json_serializable, AppState с загрузкой JSON и фильтрацией по городу. Добавь try-catch везде. Не забудь i18n/ru.json, en.json, kz.json».

### Сообщение 3 — Главные экраны
> «Реализуй HomeScreen, ServicesScreen, GuideScreen, ExcursionsScreen, ProfileScreen. Используй AutomaticKeepAliveClientMixin для табов. Проверь `flutter analyze`».

### Сообщение 4 — Внутренние экраны
> «Реализуй CityScreen, ExcursionDetailScreen, BookingScreen, FoodDelivery (3 экрана), ExchangeScreen, TransferScreen. Deeplink Telegram через Uri.encodeComponent(). Корзина через отдельный CartProvider».

### Сообщение 5 — Дополнительные экраны
> «TicketsScreen, TravelChatScreen (моковые ответы из responses.json через 2 сек), GuideCategoryScreen, PlaceDetailScreen. Empty states обязательны на всех экранах».

### Сообщение 6 — Фаза 5 (UI-заглушки)
> «ТОЛЬКО UI: PartnerCabinetScreen, ReferralScreen, ClaimCodeScreen. Без бэкенда, без Firebase. Моковые данные из JSON. QR-код через qr_flutter».

### После каждой фазы:
- `flutter analyze` — без ошибок
- Скриншоты новых экранов
- APK для тестирования
