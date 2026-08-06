# Obsidian Vault — Personal Knowledge Base

[![Obsidian](https://img.shields.io/badge/Obsidian-1.5%2B-7C3AED)](https://obsidian.md)
[![Notes](https://img.shields.io/badge/notes-129%2B-blue)](.)

**Personal knowledge base** — заметки, проекты, идеи. Синхронизируется через Git.

## Что внутри

| Директория | Содержание |
|-----------|-----------|
| `projects/` | Документация активных проектов (bybit-ws, GSC, VPN, PCI) |
| `hermes/` | Hermes Agent: конфигурация, инсайты, метрики |
| `admin/` | Административные заметки, тенанты, инфраструктура |
| `inbox/` | Входящие: идеи, ссылки, черновики |
| `daily/` | Ежедневные заметки |

## Использование

```bash
git clone https://github.com/poliakarmai/obsidian-vault.git
# Открыть в Obsidian как vault
```

## Инструменты

- **Knowledge Graph:** `~/.hermes/scripts/kg.py` — граф [[wikilinks]]
- **Reflect:** `~/.hermes/scripts/reflect.py` — ночной цикл инсайтов
- **BM25 поиск:** `~/.hermes/scripts/obsidian_search.py`

## Ссылки

- [Obsidian](https://obsidian.md) — приложение для заметок
- [Hermes Agent](https://github.com/nousresearch/hermes-agent) — AI-оркестратор
