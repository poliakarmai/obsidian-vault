# Бэклог: завтра

## 1. Диск (быстрое заполнение)
- Авто-очистка pip cache после установок
- state.db VACUUM по расписанию (cron)
- Алерт при >80%
- whisper → Groq API (−5GB диска)

## 2. SHORT-стратегия: SL 10% + задержка 20 мин
**Сейчас:** SL +5-7%, мгновенно при входе
**Надо:** SL +10% выше входа, с задержкой 20 мин

**Что менять:**
1. `bybit-ws/config.py`: `sl_tier_ab: 0.05→0.10`, `sl_tier_cd: 0.07→0.10`
2. `bybit-ws/auto_short.py:556`: убрать мгновенный trading-stop, сохранить `sl_pending_until = now + 1200`
3. `bybit-ws/auto_sl.py`: добавить проверку `sl_pending_until` → выставить SL

**Деплой:** `bash ~/bybit-ws/deploy.sh` + `systemctl --user restart bybit-ws-async`
