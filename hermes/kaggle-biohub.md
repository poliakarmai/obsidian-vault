---
tags: [kaggle, ml, cell-tracking, todo]
created: 2026-06-30
status: waiting
---

# Kaggle Biohub — Cell Tracking

**Ссылка:** https://kaggle.com/competitions/biohub-cell-tracking
**Приз:** $60,000
**Дедлайн:** 22 сентября 2026
**Проект:** ~/kaggle-cell-tracking/

## Что сделано

- ✅ Проект создан: README, requirements.txt, get_data.py, eda.ipynb, baseline.py
- ✅ Бейзлайн: CellPose → IoU-трекинг → lineage
- ⏳ Ждёт: Kaggle API-ключ для скачивания данных

## Что нужно

1. Зайти на https://kaggle.com/settings/account
2. Create New API Token → скачать kaggle.json
3. Передать агенту → положить в ~/.kaggle/kaggle.json
4. Агент скачает данные и запустит бейзлайн

## Метрика

TRA (Tracking Accuracy) = SEG + DET + TRA + lineage accuracy
