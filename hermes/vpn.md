---
tags: [vpn, infra]
---

# VPN Инфраструктура

## Сервер
- Хельсинки, 2.27.48.142
- VLESS+REALITY: порты 4443, 8445
- WireGuard: порт 443/UDP, клиент 10.88.0.2/24

## Xray
- VLESS без flow (flow ломает XKeen)
- Mux enabled: коннекты 10K→100, память 294→27MB
- Конфиг: /opt/vpn-core/conf/config.json
- Снапшот: /opt/vpn-core/snapshots/latest.json

## V2RayTun (iOS)
- allowInsecure=1, encryption=none, spx=%2F

## Мониторинг
- vpn-watch.py: cron каждые 5 мин
- Пишет в /opt/vpn-core/conf/vpn-watch-status.json (НЕ в /tmp!)
- Conntrack overflow: >500 conn + <10% ESTABLISHED → авто-рестарт
- Синхронизация: cp /opt/vpn-core/vpn-watch.py ~/.hermes/scripts/vpn-watch.py
- Systemd: ReadWritePaths включает /opt/vpn-core/conf

## Бот @Poliakarbot
- aiogram 3.x, юзер vpn-bot
- MTProto ($0.50), VLESS+WG ключи
- /opt/vpn-seller-bot/bot.py
- Бэкапы: /opt/vpn-seller-bot/backups/
- Пользователь Поляков: VLESS UUID=e03dffcd-c2a3-49d4-a2a0-dbcc292db8ab (активна)
