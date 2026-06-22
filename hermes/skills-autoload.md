
## Graphify Context (добавлен 17.06.2026)

При старте сессии, связанной с bybit-ws — загружать `graphify-context` skill.

**Что даёт:**
- 900 узлов, 1817 рёбер, 70 сообществ — полная карта bybit-ws
- Первые 150 строк GRAPH_REPORT.md заменяют чтение ~30 файлов для ориентации
- god-узлы: log_event() (69 связей), bybit() (57 связей)

**Обновление графа:**
```bash
cd ~/bybit-ws && graphify update .        # бесплатно (только AST)
cd ~/bybit-ws && graphify . --backend deepseek  # полная пересборка (~$0.01)
```

**Файлы:**
- `~/bybit-ws/graphify-out/GRAPH_REPORT.md` — текстовый отчёт
- `~/bybit-ws/graphify-out/graph.json` — полный граф (jq для поиска)
- `~/bybit-ws/graphify-out/graph.html` — интерактивная визуализация

**Построен:** 17.06.2026, коммит d5fe27b3, стоимость $0.0123
