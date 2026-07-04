# DeepSeek V4 — Official Release (июль 2026)

**Источник:** официальный анонс DeepSeek
**Дата:** 30 июня 2026
**Релиз:** середина июля 2026

## Текущее vs Будущее

| Параметр | Сейчас (Preview) | Июль (Official) |
|----------|:--:|:--:|
| Версия | Preview | V4 Pro + V4 Flash |
| Фичи | Базовые | +оптимизации, +перформанс |
| Ценообразование | Фикс | Peak/Off-peak |
| AI Studio | ❌ | ❌ |

## Тарифы (после релиза)

### deepseek-v4-pro (основная модель)
| | Обычная | Пик (×2) |
|---|---:|---:|
| Input (cache hit) / 1M | $0.0036 | $0.0072 |
| Input (cache miss) / 1M | $0.435 | $0.87 |
| **Output / 1M** | **$0.87** | **$1.74** |

### deepseek-v4-flash (быстрая/дешёвая)
| | Обычная | Пик (×2) |
|---|---:|---:|
| Input (cache hit) / 1M | $0.0028 | $0.0056 |
| Input (cache miss) / 1M | $0.14 | $0.28 |
| **Output / 1M** | **$0.28** | **$0.56** |

## Стратегия для Hermes

| Тип задач | Модель | Почему |
|-----------|--------|-------|
| Основные сессии (Поляков) | v4-pro | Качество важнее цены |
| Cron-дайджесты, health-check | v4-flash | Механика, не нужен Pro |
| Саб-агенты (delegate_task) | v4-flash | Много вызовов, короткие ответы |
| Code review, анализ кода | v4-pro | Сложный reasoning |
| VPN-бот, простые ответы | v4-flash | 3× дешевле |

## Риски

1. **Цена ×2 в пик.** Если основная сессия попадёт в пик — output $1.74/M. При 100K output/сессия = $0.17 вместо $0.09.
2. **Breaking changes.** Preview → Official может сломать API.
3. **Flash качество.** Может не хватать для сложного reasoning. Тестировать на некритичных задачах.
4. **Нет AI Studio.** Нельзя тестировать промпты в веб-интерфейсе. Только через API.

## Мониторинг

- Следить за анонсами DeepSeek
- После релиза: протестировать Flash на cron-джобах
- Сравнить качество ответов Pro vs Flash на одних и тех же запросах
- Настроить переключение пик/не-пик если API позволит

## Конфиг для Hermes (после релиза)

```yaml
# ~/.hermes/config.yaml
models:
  default: deepseek-v4-pro
  providers:
    deepseek:
      deepseek-v4-pro:
        provider: custom:deepseek
        model: deepseek-v4-pro
        cost_per_million_output: 0.87
      deepseek-v4-flash:
        provider: custom:deepseek
        model: deepseek-v4-flash
        cost_per_million_output: 0.28
```
