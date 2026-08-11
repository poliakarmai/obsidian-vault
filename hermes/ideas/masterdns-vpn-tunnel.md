---
tags: [vpn, idea, dns-tunnel]
created: 2026-08-03
status: planned
---

# MasterDnsVPN — DNS-туннель (альтернативный транспорт)

## Источник
Статья на Хабре: [Немного извращений из мира прокси и VPN](https://habr.com/ru/articles/1036100/) (MiracleUsr, 66K просмотров)

## Что это
**MasterDnsVPN** — DNS-туннель нового поколения на Go. Трафик через DNS-запросы к публичным резолверам. В 9× быстрее DNSTT, в 3.6× быстрее SlipStream. Выжил 88 дней полного отключения интернета в Иране.

GitHub: [masterking32/MasterDnsVPN](https://github.com/masterking32/MasterDnsVPN) ⭐6873

## Что нужно для запуска
1. **Купить дешёвый домен** (короткий `.xyz` ~$1/год на Namecheap — важен короткий домен для MTU!)
2. **DNS-записи:**
   - `A` → `ns` → `2.27.48.142`
   - `NS` → `v` → `ns.домен.xyz`
3. **Запустить авто-скрипт на сервере:**
   ```bash
   bash <(curl -Ls https://raw.githubusercontent.com/masterking32/MasterDnsVPN/main/server_linux_install.sh)
   ```
4. **Клиенты:** консольный (Win/Linux/Mac/Android), Android GUI (`RevocGG/MasterDnsVPN-AndroidGG`)

## Плюсы для нас
- Работает даже если режут ICMP, TCP, UDP — только DNS (53/UDP) должен ходить
- Отказоустойчивость: несколько резолверов, авто-восстановление
- Может использоваться как SOCKS5 прокси или TCP-туннель (совместим с VLESS/Shadowsocks)
- Не конфликтует с существующим Xray (разные порты)

## Статус
⏸️ Отложено — нужен домен. Следующий шаг: купить .xyz домен, скинуть мне имя.
