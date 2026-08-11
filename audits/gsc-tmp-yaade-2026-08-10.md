---
title: "GSC Audit: /tmp/yaade"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/yaade

**Дата:** 10.08.2026 14:23  
**Путь:** `/tmp/yaade`  
**Всего находок:** 309  
**CRITICAL:** 14 | **HIGH:** 131 | **MEDIUM:** 30 | **LOW:** 69

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 169 |
| GS003 | 53 |
| GS022 | 31 |
| YAML-36ACF0AD | 18 |
| GS001 | 14 |
| GS025-eval_usage | 10 |
| GS012 | 5 |
| GS010 | 2 |
| GS021 | 2 |
| GS020 | 1 |
| GS034-typo_squatting | 1 |
| GS009 | 1 |
| GS025-insecure_random | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| CRITICAL | GS001 | bundle.js | 2 | Found: 4503599627370496 |
| HIGH | GS000-LEGACY | AuthTab.tsx | 144 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | AuthTab.tsx | 196 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | RequestPanel.tsx | 212 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | RequestSender.tsx | 436 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | RequestSender.tsx | 500 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | KVEditor.tsx | 11 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | KVEditor.tsx | 44 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | KVEditor.tsx | 45 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | KVEditor.tsx | 50 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | KVEditor.tsx | 52 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | KVEditorRow.tsx | 128 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | BodyTextEditor.tsx | 22 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | BodyEditor.tsx | 14 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | BodyEditor.tsx | 15 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | BodyEditor.tsx | 18 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | BodyEditor.tsx | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | BodyKVEditor.tsx | 6 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionScript.tsx | 28 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionScript.tsx | 41 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ScriptPanel.tsx | 176 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UriBar.tsx | 25 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UriBar.tsx | 27 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Sidebar.tsx | 34 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Sidebar.tsx | 44 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Sidebar.tsx | 45 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Sidebar.tsx | 46 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | LogsTab.tsx | 31 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CmdPalette.tsx | 12 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Editor.tsx | 21 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionRequest.tsx | 28 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionRequest.tsx | 42 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | GenerateCodeTab.tsx | 165 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | GenerateCodeTab.tsx | 213 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionSettingsTab.tsx | 30 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionSettingsTab.tsx | 39 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionPanel.tsx | 123 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EnvironmentsTab.tsx | 122 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EnvironmentsTab.tsx | 172 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EnvironmentsTab.tsx | 202 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EnvironmentsTab.tsx | 520 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EnvironmentsTab.tsx | 587 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableScript.tsx | 17 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableScript.tsx | 180 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableHeader.tsx | 51 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableHeader.tsx | 52 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableHeader.tsx | 53 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableHeader.tsx | 70 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableHeader.tsx | 321 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableHeader.tsx | 351 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableRequest.tsx | 17 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MoveableRequest.tsx | 180 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionView.tsx | 54 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionView.tsx | 55 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CollectionView.tsx | 56 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UserSettings.tsx | 22 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UserSettings.tsx | 23 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ExternalProviderTab.tsx | 13 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ExternalProviderTab.tsx | 14 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | AccountSettings.tsx | 95 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | SettingsTab.tsx | 8 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | AdminSettings.tsx | 20 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Collections.tsx | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Collections.tsx | 20 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | WebsocketHandler.tsx | 95 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | WebsocketHandler.tsx | 223 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | WebsocketHandler.tsx | 237 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | WebsocketHandler.tsx | 288 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | WebsocketPanel.tsx | 265 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | currentCollection.tsx | 34 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | currentCollection.tsx | 59 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | currentScript.tsx | 34 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | currentScript.tsx | 59 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 45 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 68 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 107 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 211 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 331 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 361 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 396 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | collections.tsx | 473 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Dashboard.tsx | 302 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Dashboard.tsx | 798 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 3 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 7 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 8 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 11 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 15 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 31 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 38 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseReport.ts | 54 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | jasmine.d.ts | 1 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | envhover.d.ts | 1 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | envhover.d.ts | 2 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 25 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 26 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 27 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 28 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 57 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 63 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 72 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 84 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 85 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 86 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 105 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 111 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | script.tsx | 116 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | parseResponseEvent.tsx | 16 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | websocket.ts | 5 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | httpsnippet.tsx | 34 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | httpsnippet.tsx | 37 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | httpsnippet.tsx | 38 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | httpsnippet.tsx | 54 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | httpsnippet.tsx | 55 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | httpsnippet.tsx | 63 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 13 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 21 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 46 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 56 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 13 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 14 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 75 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 78 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 79 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 80 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 109 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | interpolate.tsx | 129 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | extension.ts | 5 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | extension.ts | 15 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | User.tsx | 4 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | bundle.js | 2 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS010 | index.js | 47 |
| M | GS010 | index.js | 48 |
| H | GS000-LEGACY | AuthTab.tsx | 144 |
| H | GS000-LEGACY | AuthTab.tsx | 196 |
| H | GS000-LEGACY | RequestPanel.tsx | 212 |
| H | GS000-LEGACY | RequestSender.tsx | 436 |
| H | GS000-LEGACY | RequestSender.tsx | 500 |
| H | GS000-LEGACY | KVEditor.tsx | 11 |
| H | GS000-LEGACY | KVEditor.tsx | 44 |
| H | GS000-LEGACY | KVEditor.tsx | 45 |
| H | GS000-LEGACY | KVEditor.tsx | 50 |
| H | GS000-LEGACY | KVEditor.tsx | 52 |
| H | GS000-LEGACY | KVEditorRow.tsx | 128 |
| H | GS000-LEGACY | BodyTextEditor.tsx | 22 |
| H | GS000-LEGACY | BodyEditor.tsx | 14 |
| H | GS000-LEGACY | BodyEditor.tsx | 15 |
| H | GS000-LEGACY | BodyEditor.tsx | 18 |
| H | GS000-LEGACY | BodyEditor.tsx | 19 |
| H | GS000-LEGACY | BodyKVEditor.tsx | 6 |
| H | GS000-LEGACY | CollectionScript.tsx | 28 |
| H | GS000-LEGACY | CollectionScript.tsx | 41 |
| H | GS000-LEGACY | ScriptPanel.tsx | 176 |
| H | GS000-LEGACY | UriBar.tsx | 25 |
| H | GS000-LEGACY | UriBar.tsx | 27 |
| H | GS000-LEGACY | Sidebar.tsx | 34 |
| H | GS000-LEGACY | Sidebar.tsx | 44 |
| H | GS000-LEGACY | Sidebar.tsx | 45 |
| H | GS000-LEGACY | Sidebar.tsx | 46 |
| H | GS000-LEGACY | LogsTab.tsx | 31 |
| H | GS000-LEGACY | CmdPalette.tsx | 12 |
| H | GS000-LEGACY | Editor.tsx | 21 |
| H | GS000-LEGACY | CollectionRequest.tsx | 28 |
| H | GS000-LEGACY | CollectionRequest.tsx | 42 |
| H | GS000-LEGACY | GenerateCodeTab.tsx | 165 |
| H | GS000-LEGACY | GenerateCodeTab.tsx | 213 |
| H | GS000-LEGACY | CollectionSettingsTab.tsx | 30 |
| H | GS000-LEGACY | CollectionSettingsTab.tsx | 39 |
| H | GS000-LEGACY | CollectionPanel.tsx | 123 |
| H | GS000-LEGACY | EnvironmentsTab.tsx | 122 |
| H | GS000-LEGACY | EnvironmentsTab.tsx | 172 |
| H | GS000-LEGACY | EnvironmentsTab.tsx | 202 |
| H | GS000-LEGACY | EnvironmentsTab.tsx | 520 |
| H | GS000-LEGACY | EnvironmentsTab.tsx | 587 |
| H | GS000-LEGACY | MoveableScript.tsx | 17 |
| H | GS000-LEGACY | MoveableScript.tsx | 180 |
| H | GS000-LEGACY | MoveableHeader.tsx | 51 |
| H | GS000-LEGACY | MoveableHeader.tsx | 52 |
| H | GS000-LEGACY | MoveableHeader.tsx | 53 |
| H | GS000-LEGACY | MoveableHeader.tsx | 70 |
| H | GS000-LEGACY | MoveableHeader.tsx | 321 |
| H | GS000-LEGACY | MoveableHeader.tsx | 351 |
| H | GS000-LEGACY | MoveableRequest.tsx | 17 |
| H | GS000-LEGACY | MoveableRequest.tsx | 180 |
| H | GS000-LEGACY | CollectionView.tsx | 54 |
| H | GS000-LEGACY | CollectionView.tsx | 55 |
| H | GS000-LEGACY | CollectionView.tsx | 56 |
| H | GS000-LEGACY | UserSettings.tsx | 22 |
| H | GS000-LEGACY | UserSettings.tsx | 23 |
| H | GS000-LEGACY | ExternalProviderTab.tsx | 13 |
| H | GS000-LEGACY | ExternalProviderTab.tsx | 14 |
| H | GS000-LEGACY | AccountSettings.tsx | 95 |
| H | GS000-LEGACY | SettingsTab.tsx | 8 |
| H | GS000-LEGACY | AdminSettings.tsx | 20 |
| H | GS000-LEGACY | Collections.tsx | 19 |
| H | GS000-LEGACY | Collections.tsx | 20 |
| H | GS000-LEGACY | WebsocketHandler.tsx | 95 |
| H | GS000-LEGACY | WebsocketHandler.tsx | 223 |
| H | GS000-LEGACY | WebsocketHandler.tsx | 237 |
| H | GS000-LEGACY | WebsocketHandler.tsx | 288 |
| H | GS000-LEGACY | WebsocketPanel.tsx | 265 |
| H | GS000-LEGACY | currentCollection.tsx | 34 |
| H | GS000-LEGACY | currentCollection.tsx | 59 |
| H | GS000-LEGACY | currentScript.tsx | 34 |
| H | GS000-LEGACY | currentScript.tsx | 59 |
| H | GS000-LEGACY | collections.tsx | 45 |
| H | GS000-LEGACY | collections.tsx | 68 |
| H | GS000-LEGACY | collections.tsx | 107 |
| H | GS000-LEGACY | collections.tsx | 211 |
| H | GS000-LEGACY | collections.tsx | 331 |
| H | GS000-LEGACY | collections.tsx | 361 |
| H | GS000-LEGACY | collections.tsx | 396 |
| H | GS000-LEGACY | collections.tsx | 473 |
| H | GS000-LEGACY | Dashboard.tsx | 302 |
| H | GS000-LEGACY | Dashboard.tsx | 798 |
| H | GS000-LEGACY | parseReport.ts | 3 |
| H | GS000-LEGACY | parseReport.ts | 7 |
| H | GS000-LEGACY | parseReport.ts | 8 |
| H | GS000-LEGACY | parseReport.ts | 11 |
| H | GS000-LEGACY | parseReport.ts | 15 |
| H | GS000-LEGACY | parseReport.ts | 19 |
| H | GS000-LEGACY | parseReport.ts | 31 |
| H | GS000-LEGACY | parseReport.ts | 38 |
| H | GS000-LEGACY | parseReport.ts | 54 |
| H | GS000-LEGACY | jasmine.d.ts | 1 |
| H | GS000-LEGACY | envhover.d.ts | 1 |
| H | GS000-LEGACY | envhover.d.ts | 2 |
| H | GS000-LEGACY | script.tsx | 25 |
| H | GS000-LEGACY | script.tsx | 26 |
| H | GS000-LEGACY | script.tsx | 27 |
| H | GS000-LEGACY | script.tsx | 28 |
| H | GS000-LEGACY | script.tsx | 57 |
| H | GS000-LEGACY | script.tsx | 63 |
| H | GS000-LEGACY | script.tsx | 72 |
| H | GS000-LEGACY | script.tsx | 84 |
| H | GS000-LEGACY | script.tsx | 85 |
| H | GS000-LEGACY | script.tsx | 86 |
| H | GS000-LEGACY | script.tsx | 105 |
| H | GS000-LEGACY | script.tsx | 111 |
| H | GS000-LEGACY | script.tsx | 116 |
| H | GS000-LEGACY | parseResponseEvent.tsx | 16 |
| H | GS000-LEGACY | websocket.ts | 5 |
| H | GS000-LEGACY | httpsnippet.tsx | 34 |
| H | GS000-LEGACY | httpsnippet.tsx | 37 |
| H | GS000-LEGACY | httpsnippet.tsx | 38 |
| H | GS000-LEGACY | httpsnippet.tsx | 54 |
| H | GS000-LEGACY | httpsnippet.tsx | 55 |
| H | GS000-LEGACY | httpsnippet.tsx | 63 |
| H | GS000-LEGACY | index.tsx | 13 |
| H | GS000-LEGACY | index.tsx | 21 |
| H | GS000-LEGACY | index.tsx | 46 |
| H | GS000-LEGACY | index.tsx | 56 |
| H | GS000-LEGACY | interpolate.tsx | 13 |
| H | GS000-LEGACY | interpolate.tsx | 14 |
| H | GS000-LEGACY | interpolate.tsx | 75 |
| H | GS000-LEGACY | interpolate.tsx | 78 |
| H | GS000-LEGACY | interpolate.tsx | 79 |
| H | GS000-LEGACY | interpolate.tsx | 80 |
| H | GS000-LEGACY | interpolate.tsx | 109 |
| H | GS000-LEGACY | interpolate.tsx | 129 |
| H | GS000-LEGACY | extension.ts | 5 |
| H | GS000-LEGACY | extension.ts | 15 |
| H | GS000-LEGACY | User.tsx | 4 |
| M | GS000-LEGACY | Login.tsx | 60 |
| M | GS000-LEGACY | Login.tsx | 72 |
| M | GS000-LEGACY | Dashboard.tsx | 184 |
| M | GS000-LEGACY | Dashboard.tsx | 422 |
| M | GS000-LEGACY | script.tsx | 58 |
| M | GS000-LEGACY | script.tsx | 64 |
| M | GS000-LEGACY | script.tsx | 106 |
| M | GS000-LEGACY | script.tsx | 112 |
| M | GS000-LEGACY | index.tsx | 284 |
| M | GS000-LEGACY | index.tsx | 294 |
| M | GS000-LEGACY | interpolate.tsx | 35 |
| M | GS000-LEGACY | interpolate.tsx | 36 |
| M | GS000-LEGACY | interpolate.tsx | 37 |
| M | GS000-LEGACY | interpolate.tsx | 38 |
| M | GS000-LEGACY | interpolate.tsx | 58 |
| M | GS000-LEGACY | interpolate.tsx | 59 |
| M | GS000-LEGACY | interpolate.tsx | 67 |
| M | GS000-LEGACY | interpolate.tsx | 68 |
| M | GS000-LEGACY | interpolate.tsx | 82 |
| M | GS000-LEGACY | interpolate.tsx | 83 |
| M | GS000-LEGACY | interpolate.tsx | 102 |
| M | GS000-LEGACY | interpolate.tsx | 103 |
| M | GS000-LEGACY | interpolate.tsx | 119 |
| M | GS000-LEGACY | interpolate.tsx | 120 |
| M | GS000-LEGACY | interpolate.tsx | 121 |
| M | GS000-LEGACY | interpolate.tsx | 132 |
| M | GS000-LEGACY | interpolate.tsx | 133 |
| M | GS000-LEGACY | interpolate.tsx | 134 |
| L | GS000-LEGACY | CollectionElement.java | 130 |
| L | GS000-LEGACY | AuthDeserializer.java | 50 |
| L | GS000-LEGACY | AuthDeserializer.java | 57 |
| L | GS000-LEGACY | RequestBody.java | 186 |
| L | GS000-LEGACY | BodyElement.java | 126 |
| L | GS000-LEGACY | BodyElement.java | 224 |
| L | GS000-LEGACY | BodyElement.java | 248 |
| L | GS000-LEGACY | Url.java | 731 |
| L | GS000-LEGACY | ItemGroup.java | 65 |
| L | GS000-LEGACY | Collection.java | 392 |
| L | GS000-LEGACY | Collection.java | 418 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| C | GS001 | bundle.js | 2 |
| L | GS003 | jasmine.js | 7507 |
| L | GS003 | jasmine.js | 8417 |
| L | GS003 | jasmine.js | 8463 |
| L | GS003 | jasmine.js | 8480 |
| L | GS003 | jasmine.js | 8483 |
| L | GS003 | jasmine.js | 8489 |
| L | GS003 | jasmine.js | 8494 |
| L | GS003 | jasmine.js | 8508 |
| L | GS003 | jasmine.js | 8511 |
| L | GS003 | jasmine.js | 8519 |
| L | GS003 | jasmine.js | 8522 |
| L | GS003 | background.js | 192 |
| L | GS003 | background.js | 198 |
| L | GS003 | background.js | 207 |
| L | GS003 | background.js | 210 |
| L | GS003 | contentScript.js | 27 |
| L | GS003 | bundle.js | 2 |
| L | GS003 | bundle.js | 2 |
| L | GS003 | bundle.js | 2 |
| L | GS003 | bundle.js | 2 |
| L | GS003 | bundle.js | 2 |
| L | GS003 | bundle.js | 2 |
| L | GS003 | bundle.js | 2 |
| L | GS003 | interpolate.js | 75 |
| L | GS003 | interpolate.js | 76 |
| L | GS003 | interpolate.js | 77 |
| L | GS003 | interpolate.js | 78 |
| L | GS003 | interpolate.js | 101 |
| L | GS003 | interpolate.js | 102 |
| L | GS003 | interpolate.js | 110 |
| L | GS003 | interpolate.js | 111 |
| L | GS003 | interpolate.js | 125 |
| L | GS003 | interpolate.js | 126 |
| L | GS003 | interpolate.js | 145 |
| L | GS003 | interpolate.js | 146 |
| L | GS003 | interpolate.js | 164 |
| L | GS003 | interpolate.js | 165 |
| L | GS003 | interpolate.js | 166 |
| L | GS003 | interpolate.js | 177 |
| L | GS003 | interpolate.js | 178 |
| L | GS003 | interpolate.js | 179 |
| L | GS003 | interpolate.js | 9 |
| L | GS003 | jasmine.js | 7690 |
| L | GS003 | jasmine.js | 8598 |
| L | GS003 | jasmine.js | 8644 |
| L | GS003 | jasmine.js | 8658 |
| L | GS003 | jasmine.js | 8659 |
| L | GS003 | jasmine.js | 8663 |
| L | GS003 | jasmine.js | 8664 |
| L | GS003 | jasmine.js | 8672 |
| L | GS003 | jasmine.js | 8673 |
| L | GS003 | jasmine.js | 8678 |
| L | GS003 | jasmine.js | 8679 |
| i | GS020 |  | 188 |
| ? | GS034-typo_squatting | package.json | 32 |
| s | GS009 |  | 0 |
| L | GS012 | bundle.js | 2 |
| L | GS012 | bundle.js | 2 |
| L | GS012 | bundle.js | 2 |
| L | GS012 | bundle.js | 2 |
| L | GS012 | bundle.js | 2 |
| s | GS021 |  | 21 |
| s | GS021 |  | 26 |
| r | GS022 |  | 82 |
| r | GS022 |  | 82 |
| r | GS022 |  | 97 |
| r | GS022 |  | 134 |
| r | GS022 |  | 134 |
| r | GS022 |  | 168 |
| r | GS022 |  | 178 |
| r | GS022 |  | 179 |
| r | GS022 |  | 200 |
| r | GS022 |  | 61 |
| r | GS022 |  | 237 |
| r | GS022 |  | 321 |
| r | GS022 |  | 332 |
| r | GS022 |  | 380 |
| r | GS022 |  | 695 |
| r | GS022 |  | 726 |
| r | GS022 |  | 728 |
| r | GS022 |  | 734 |
| r | GS022 |  | 438 |
| r | GS022 |  | 515 |
| r | GS022 |  | 189 |
| r | GS022 |  | 190 |
| r | GS022 |  | 4966 |
| r | GS022 |  | 4966 |
| r | GS022 |  | 4 |
| r | GS022 |  | 5094 |
| r | GS022 |  | 5094 |
| r | GS022 |  | 86 |
| r | GS022 |  | 55 |
| r | GS022 |  | 327 |
| r | GS022 |  | 379 |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-insecure_random |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | jasmine.js | ? |
| ? | YAML-36ACF0AD | jasmine.js | ? |
| ? | YAML-36ACF0AD | jasmine.js | ? |
| ? | YAML-36ACF0AD | ScriptRunner.kt | ? |
| ? | YAML-36ACF0AD | ScriptRunner.kt | ? |
| ? | YAML-36ACF0AD | ScriptRunner.kt | ? |
| ? | YAML-36ACF0AD | ScriptRunner.kt | ? |
| ? | YAML-36ACF0AD | ScriptRuntimeBuilder.kt | ? |
| ? | YAML-36ACF0AD | ScriptRuntimeBuilder.kt | ? |
| ? | YAML-36ACF0AD | ScriptRuntimeBuilder.kt | ? |
| ? | YAML-36ACF0AD | ScriptRuntimeBuilder.kt | ? |
| ? | YAML-36ACF0AD | bundle.js | ? |
| ? | YAML-36ACF0AD | bundle.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | jasmine.js | ? |
| ? | YAML-36ACF0AD | jasmine.js | ? |
| ? | YAML-36ACF0AD | jasmine.js | ? |
| H | ? | bundle.js | 2 |

---
*Сгенерировано GSC v0.6 · 2026-08-10T14:23:56.975629*