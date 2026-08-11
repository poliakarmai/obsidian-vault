---
title: "GSC Audit: /tmp/django-bolt"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/django-bolt

**Дата:** 10.08.2026 14:31  
**Путь:** `/tmp/django-bolt`  
**Всего находок:** 572  
**CRITICAL:** 25 | **HIGH:** 210 | **MEDIUM:** 94 | **LOW:** 54

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Rust: .clone() in hot path | 138 |
| GS018 | 88 |
| GS000-LEGACY | 83 |
| GS021 | 68 |
| GS003 | 51 |
| GS025-debug_mode | 38 |
| GS025-hardcoded_secret | 33 |
| GS020 | 17 |
| GS022 | 14 |
| YAML-B39DC08C | 9 |
| GS025 | 7 |
| GS019 | 5 |
| GS015 | 3 |
| GS011 | 3 |
| YAML-ECB85AD8 | 3 |
| GS029 | 2 |
| GS037-hardcoded_password | 2 |
| GS004 | 2 |
| GS005 | 2 |
| GS008 | 1 |
| GS037-debug_true | 1 |
| GS009 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 89 | Match:     name: Annotated[str, Meta(min_length=2)] |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 98 | Match:     name: str = Field(..., min_length=2) |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 110 | Match:     user_name: Annotated[str, Meta(min_length=2)] |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 119 | Match:     user_name: str = Field(..., min_length=2, alias=" |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 144 | Match:     name: Annotated[str, Meta(min_length=2)] |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 161 | Match:     name: str = Field(..., min_length=2) |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 254 | Match:     name: Annotated[str, Meta(min_length=1, max_lengt |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 264 | Match:     name: str = Field(..., min_length=1, max_length=1 |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 319 | Match:     name: str = Field(..., min_length=1) |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 331 | Match:     name: Annotated[str, Meta(min_length=1, max_lengt |
| CRITICAL | GS000-LEGACY | benchmark_serializer.py | 344 | Match:     name: str = Field(..., min_length=1, max_length=1 |
| CRITICAL | GS000-LEGACY | api.py | 23 | Match:     name: Annotated[str, Meta(min_length=1, max_lengt |
| CRITICAL | GS000-LEGACY | api.py | 35 | Match:     name: Annotated[str, Meta(min_length=1, max_lengt |
| CRITICAL | GS000-LEGACY | api.py | 118 | Match:     name: Annotated[str, Meta(min_length=1, max_lengt |
| CRITICAL | GS000-LEGACY | api.py | 119 | Match:     role: Annotated[str, Meta(min_length=1, max_lengt |
| CRITICAL | GS000-LEGACY | api.py | 161 | Match:     username: Annotated[str, Meta(min_length=2, max_l |
| CRITICAL | GS000-LEGACY | api.py | 1341 | Match:     name: Annotated[str, Meta(min_length=2)] |
| CRITICAL | GS000-LEGACY | api.py | 1350 | Match:     name: Annotated[str, Meta(min_length=2)] |
| CRITICAL | GS000-LEGACY | types.py | 368 | Match:         min_length=3, |
| CRITICAL | GS000-LEGACY | types.py | 380 | Match:         min_length=2, |
| CRITICAL | GS000-LEGACY | types.py | 392 | Match:         min_length=2, |
| CRITICAL | GS000-LEGACY | types.py | 476 | Match:     Meta(min_length=1, description="Non-empty string" |
| CRITICAL | GS005 | api.py | 1622 | Line 1622: return PlainText(f"Header: {x}") |
| CRITICAL | GS005 | api.py | 1631 | Line 1631: return PlainText(f"Cookie: {val}") |
| CRITICAL | GS019 | settings.py | 23 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | GS000-LEGACY | tests.py | 187 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 188 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 204 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 205 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 364 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 51 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 68 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 948 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 950 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 2763 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 2764 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 2812 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 2813 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | typing.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | typing.py | 274 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | typing.py | 289 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 25 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 215 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 226 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 255 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 273 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 341 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 345 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 346 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 366 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 377 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 385 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 390 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 392 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 525 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 536 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 538 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 540 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 541 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 542 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 545 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 547 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 548 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 549 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 575 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 577 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 579 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 580 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 581 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 584 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 586 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 587 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | extractors.py | 588 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 27 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 74 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 83 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 175 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 261 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 310 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 642 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 818 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 819 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 834 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 940 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model.py | 941 | File upload without MIME-type validation → malicious file up |
| HIGH | GS025 | ws_load.py | 153 |  |
| HIGH | GS025 | sse_load.py | 130 |  |
| HIGH | GS025 | cli.py | 16 |  |
| HIGH | GS025 | renovate.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | _worker_loop.py | 725 | Line 725: async def subprocess_exec(self, protocol_factory,  |
| HIGH | GS004 | _worker_loop.py | 727 | Line 727: self._selector_loop.subprocess_exec(protocol_facto |
| HIGH | GS011 | token.py | 60 | Detected: secret="my-secret" |
| HIGH | GS019 | config.py | 16 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | config.py | 119 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | views.py | 79 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | responses.py | 140 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | ? | server.rs | 289 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 667 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 707 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 717 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 726 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 759 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 760 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 780 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 781 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 805 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 806 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 837 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 880 | Clone in performance-critical code — consider references |
| HIGH | ? | server.rs | 1107 | Clone in performance-critical code — consider references |
| HIGH | ? | worker_loop.rs | 83 | Clone in performance-critical code — consider references |
| HIGH | ? | worker_loop.rs | 106 | Clone in performance-critical code — consider references |
| HIGH | ? | worker_loop.rs | 316 | Clone in performance-critical code — consider references |
| HIGH | ? | form_parsing.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | form_parsing.rs | 415 | Clone in performance-critical code — consider references |
| HIGH | ? | static_files.rs | 150 | Clone in performance-critical code — consider references |
| HIGH | ? | static_files.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | request.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | request.rs | 392 | Clone in performance-critical code — consider references |
| HIGH | ? | request.rs | 406 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | metadata.rs | 769 | Clone in performance-critical code — consider references |
| HIGH | ? | type_coercion.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | type_coercion.rs | 167 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 176 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 296 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 333 | Clone in performance-critical code — consider references |
| HIGH | ? | streaming.rs | 453 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 75 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 481 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 525 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 551 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 553 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 554 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 556 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 557 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 562 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 576 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 579 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 580 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 582 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 583 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 589 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 590 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 595 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 596 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 613 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 631 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 645 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 732 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 1087 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 1205 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 1206 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 1207 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 1279 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 1363 | Clone in performance-critical code — consider references |
| HIGH | ? | testing.rs | 1478 | Clone in performance-critical code — consider references |
| HIGH | ? | response_builder.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 203 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 261 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 269 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 290 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 309 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 343 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 563 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 603 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 608 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 618 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 619 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 663 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 1086 | Clone in performance-critical code — consider references |
| HIGH | ? | permissions.rs | 196 | Clone in performance-critical code — consider references |
| HIGH | ? | permissions.rs | 369 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | registry.rs | 236 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 200 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 206 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 103 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 114 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 205 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 247 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 294 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 317 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 479 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 486 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 574 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 585 | Clone in performance-critical code — consider references |
| HIGH | ? | handler.rs | 607 | Clone in performance-critical code — consider references |
| HIGH | ? | state_codec.rs | 137 | Clone in performance-critical code — consider references |
| HIGH | ? | request_pipeline.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | request_pipeline.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | responses.rs | 33 | Clone in performance-critical code — consider references |
| HIGH | ? | responses.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | responses.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | cors.rs | 39 | Clone in performance-critical code — consider references |
| HIGH | ? | cors.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | cors.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | cors.rs | 115 | Clone in performance-critical code — consider references |
| HIGH | ? | cors.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | cors.rs | 123 | Clone in performance-critical code — consider references |
| HIGH | ? | auth.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | auth.rs | 80 | Clone in performance-critical code — consider references |
| HIGH | ? | auth.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | auth.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | auth.rs | 320 | Clone in performance-critical code — consider references |
| HIGH | ? | auth.rs | 660 | Clone in performance-critical code — consider references |
| HIGH | ? | auth.rs | 676 | Clone in performance-critical code — consider references |
| HIGH | ? | compression.rs | 76 | Clone in performance-critical code — consider references |
| HIGH | ? | compression.rs | 174 | Clone in performance-critical code — consider references |
| HIGH | ? | compression.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | rate_limit.rs | 86 | Clone in performance-critical code — consider references |
| HIGH | ? | rate_limit.rs | 87 | Clone in performance-critical code — consider references |
| HIGH | ? | cors.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | dev_reload.rs | 348 | Clone in performance-critical code — consider references |
| HIGH | ? | asgi_http.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | asgi_http.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | asgi_http.rs | 126 | Clone in performance-critical code — consider references |
| HIGH | ? | asgi_http.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | asgi_http.rs | 449 | Clone in performance-critical code — consider references |
| HIGH | ? | asgi_http.rs | 458 | Clone in performance-critical code — consider references |
| HIGH | ? | asgi_http.rs | 459 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | GS018 | tests.py | 36 |
| M | GS018 | tests.py | 37 |
| M | GS018 | tests.py | 45 |
| M | GS018 | tests.py | 47 |
| M | GS018 | tests.py | 48 |
| M | GS018 | tests.py | 49 |
| M | GS018 | tests.py | 50 |
| M | GS018 | tests.py | 55 |
| M | GS018 | tests.py | 60 |
| M | GS018 | tests.py | 65 |
| M | GS018 | tests.py | 70 |
| M | GS018 | tests.py | 83 |
| M | GS018 | tests.py | 85 |
| M | GS018 | tests.py | 86 |
| M | GS018 | tests.py | 91 |
| M | GS018 | tests.py | 101 |
| M | GS018 | tests.py | 102 |
| M | GS018 | tests.py | 105 |
| M | GS018 | tests.py | 115 |
| M | GS018 | tests.py | 125 |
| M | GS018 | tests.py | 129 |
| M | GS018 | tests.py | 138 |
| M | GS018 | tests.py | 140 |
| M | GS018 | tests.py | 155 |
| M | GS018 | tests.py | 157 |
| M | GS018 | tests.py | 158 |
| M | GS018 | tests.py | 159 |
| M | GS018 | tests.py | 169 |
| M | GS018 | tests.py | 178 |
| M | GS018 | tests.py | 180 |
| M | GS018 | tests.py | 196 |
| M | GS018 | tests.py | 198 |
| M | GS018 | tests.py | 199 |
| M | GS018 | tests.py | 200 |
| M | GS018 | tests.py | 201 |
| M | GS018 | tests.py | 202 |
| M | GS018 | tests.py | 216 |
| M | GS018 | tests.py | 218 |
| M | GS018 | tests.py | 220 |
| M | GS018 | tests.py | 221 |
| M | GS018 | tests.py | 230 |
| M | GS018 | tests.py | 242 |
| M | GS018 | tests.py | 244 |
| M | GS018 | tests.py | 245 |
| M | GS018 | tests.py | 246 |
| M | GS018 | tests.py | 256 |
| M | GS018 | tests.py | 258 |
| M | GS018 | tests.py | 259 |
| M | GS018 | tests.py | 260 |
| M | GS018 | tests.py | 273 |
| M | GS018 | tests.py | 275 |
| M | GS018 | tests.py | 276 |
| M | GS018 | tests.py | 277 |
| M | GS018 | tests.py | 285 |
| M | GS018 | tests.py | 287 |
| M | GS018 | tests.py | 288 |
| M | GS018 | tests.py | 293 |
| M | GS018 | tests.py | 306 |
| M | GS018 | tests.py | 308 |
| M | GS018 | tests.py | 309 |
| M | GS018 | tests.py | 314 |
| M | GS018 | tests.py | 316 |
| M | GS018 | tests.py | 317 |
| M | GS018 | tests.py | 325 |
| M | GS018 | tests.py | 327 |
| M | GS018 | tests.py | 328 |
| M | GS018 | tests.py | 338 |
| M | GS018 | tests.py | 339 |
| M | GS018 | tests.py | 346 |
| M | GS018 | tests.py | 352 |
| M | GS018 | tests.py | 353 |
| M | GS018 | tests.py | 360 |
| M | GS018 | tests.py | 361 |
| M | GS018 | tests.py | 362 |
| M | GS018 | tests.py | 372 |
| M | GS018 | tests.py | 374 |
| M | GS018 | tests.py | 375 |
| M | GS018 | tests.py | 378 |
| M | GS018 | tests.py | 385 |
| M | GS018 | tests.py | 386 |
| M | GS018 | tests.py | 389 |
| M | GS018 | tests.py | 390 |
| M | GS018 | tests.py | 395 |
| M | GS018 | tests.py | 396 |
| M | GS018 | mcp_oauth_client_demo.py | 167 |
| M | GS018 | mcp_oauth_client_demo.py | 168 |
| M | GS018 | api.py | 1393 |
| M | GS018 | api.py | 1394 |
| H | GS000-LEGACY | tests.py | 187 |
| H | GS000-LEGACY | tests.py | 188 |
| H | GS000-LEGACY | tests.py | 204 |
| H | GS000-LEGACY | tests.py | 205 |
| H | GS000-LEGACY | tests.py | 364 |
| H | GS000-LEGACY | api.py | 51 |
| H | GS000-LEGACY | api.py | 68 |
| H | GS000-LEGACY | api.py | 948 |
| H | GS000-LEGACY | api.py | 950 |
| H | GS000-LEGACY | api.py | 2763 |
| H | GS000-LEGACY | api.py | 2764 |
| H | GS000-LEGACY | api.py | 2812 |
| H | GS000-LEGACY | api.py | 2813 |
| H | GS000-LEGACY | typing.py | 38 |
| H | GS000-LEGACY | typing.py | 274 |
| H | GS000-LEGACY | typing.py | 289 |
| H | GS000-LEGACY | extractors.py | 25 |
| H | GS000-LEGACY | extractors.py | 215 |
| H | GS000-LEGACY | extractors.py | 226 |
| H | GS000-LEGACY | extractors.py | 255 |
| H | GS000-LEGACY | extractors.py | 273 |
| H | GS000-LEGACY | extractors.py | 341 |
| H | GS000-LEGACY | extractors.py | 345 |
| H | GS000-LEGACY | extractors.py | 346 |
| H | GS000-LEGACY | extractors.py | 366 |
| H | GS000-LEGACY | extractors.py | 377 |
| H | GS000-LEGACY | extractors.py | 385 |
| H | GS000-LEGACY | extractors.py | 390 |
| H | GS000-LEGACY | extractors.py | 392 |
| H | GS000-LEGACY | extractors.py | 525 |
| H | GS000-LEGACY | extractors.py | 536 |
| H | GS000-LEGACY | extractors.py | 538 |
| H | GS000-LEGACY | extractors.py | 540 |
| H | GS000-LEGACY | extractors.py | 541 |
| H | GS000-LEGACY | extractors.py | 542 |
| H | GS000-LEGACY | extractors.py | 545 |
| H | GS000-LEGACY | extractors.py | 547 |
| H | GS000-LEGACY | extractors.py | 548 |
| H | GS000-LEGACY | extractors.py | 549 |
| H | GS000-LEGACY | extractors.py | 575 |
| H | GS000-LEGACY | extractors.py | 577 |
| H | GS000-LEGACY | extractors.py | 579 |
| H | GS000-LEGACY | extractors.py | 580 |
| H | GS000-LEGACY | extractors.py | 581 |
| H | GS000-LEGACY | extractors.py | 584 |
| H | GS000-LEGACY | extractors.py | 586 |
| H | GS000-LEGACY | extractors.py | 587 |
| H | GS000-LEGACY | extractors.py | 588 |
| H | GS000-LEGACY | model.py | 27 |
| H | GS000-LEGACY | model.py | 74 |
| H | GS000-LEGACY | model.py | 83 |
| H | GS000-LEGACY | model.py | 175 |
| H | GS000-LEGACY | model.py | 261 |
| H | GS000-LEGACY | model.py | 310 |
| H | GS000-LEGACY | model.py | 642 |
| H | GS000-LEGACY | model.py | 818 |
| H | GS000-LEGACY | model.py | 819 |
| H | GS000-LEGACY | model.py | 834 |
| H | GS000-LEGACY | model.py | 940 |
| H | GS000-LEGACY | model.py | 941 |
| H | GS025 | ws_load.py | 153 |
| H | GS025 | sse_load.py | 130 |
| H | GS025 | cli.py | 16 |
| M | GS025 | settings.py | 23 |
| M | GS025 | tokens.py | 327 |
| M | GS029 | schema_generator.py | 1056 |
| M | GS029 | tokens.py | 327 |
| L | GS003 | admin_detection.py | 106 |
| L | GS003 | admin_detection.py | 194 |
| L | GS003 | admin_detection.py | 204 |
| L | GS003 | admin_detection.py | 216 |
| L | GS003 | backends.py | 417 |
| L | GS003 | api.py | 139 |
| L | GS003 | api.py | 55 |
| L | GS003 | api.py | 59 |
| L | GS003 | api.py | 1701 |
| L | GS003 | middleware_demo.py | 30 |
| L | GS003 | middleware_demo.py | 223 |
| L | GS003 | t.py | 33 |
| L | GS003 | cookies.rs | 23 |
| L | GS003 | cookies.rs | 32 |
| L | GS003 | cookies.rs | 45 |
| L | GS003 | dev_reload.rs | 63 |
| L | GS003 | metadata.rs | 168 |
| L | GS003 | metadata.rs | 773 |
| L | GS003 | rate_limit.rs | 107 |
| L | GS003 | server.rs | 69 |
| L | GS003 | server.rs | 76 |
| L | GS003 | server.rs | 127 |
| L | GS003 | server.rs | 136 |
| L | GS003 | server.rs | 143 |
| L | GS003 | server.rs | 156 |
| L | GS003 | server.rs | 415 |
| L | GS003 | server.rs | 482 |
| L | GS003 | server.rs | 493 |
| L | GS003 | server.rs | 518 |
| L | GS003 | server.rs | 574 |
| L | GS003 | server.rs | 657 |
| L | GS003 | server.rs | 658 |
| L | GS003 | server.rs | 661 |
| L | GS003 | server.rs | 693 |
| L | GS003 | server.rs | 749 |
| L | GS003 | server.rs | 1012 |
| L | GS003 | server.rs | 1031 |
| L | GS003 | streaming.rs | 327 |
| L | GS003 | streaming.rs | 415 |
| L | GS003 | streaming.rs | 436 |
| L | GS003 | streaming.rs | 448 |
| L | GS003 | actor.rs | 86 |
| L | GS003 | actor.rs | 166 |
| L | GS003 | actor.rs | 194 |
| L | GS003 | actor.rs | 241 |
| L | GS003 | handler.rs | 387 |
| L | GS003 | handler.rs | 405 |
| L | GS003 | handler.rs | 487 |
| L | GS003 | handler.rs | 669 |
| L | GS003 | handler.rs | 681 |
| L | GS003 | handler.rs | 697 |
| L | GS008 | benchmark_serializer.py | 72 |
| I | GS015 | server.py | 1 |
| I | GS015 | server.py | 1 |
| I | GS015 | urls.py | 1 |
| i | GS020 |  | 46 |
| i | GS020 |  | 30 |
| i | GS020 |  | 31 |
| i | GS020 |  | 62 |
| i | GS020 |  | 555 |
| i | GS020 |  | 41 |
| i | GS020 |  | 20 |
| i | GS020 |  | 34 |
| i | GS020 |  | 32 |
| i | GS020 |  | 40 |
| i | GS020 |  | 42 |
| i | GS020 |  | 31 |
| i | GS020 |  | 26 |
| i | GS020 |  | 28 |
| i | GS020 |  | 20 |
| i | GS020 |  | 37 |
| i | GS020 |  | 55 |
| ? | GS037-hardcoded_password | token.py | 60 |
| ? | GS037-debug_true | error_handlers.py | 319 |
| ? | GS037-hardcoded_password | base.py | 391 |
| M | GS000-LEGACY | cli.py | 16 |
| C | GS000-LEGACY | benchmark_serializer.py | 89 |
| C | GS000-LEGACY | benchmark_serializer.py | 98 |
| C | GS000-LEGACY | benchmark_serializer.py | 110 |
| C | GS000-LEGACY | benchmark_serializer.py | 119 |
| C | GS000-LEGACY | benchmark_serializer.py | 144 |
| C | GS000-LEGACY | benchmark_serializer.py | 161 |
| C | GS000-LEGACY | benchmark_serializer.py | 254 |
| C | GS000-LEGACY | benchmark_serializer.py | 264 |
| C | GS000-LEGACY | benchmark_serializer.py | 319 |
| C | GS000-LEGACY | benchmark_serializer.py | 331 |
| C | GS000-LEGACY | benchmark_serializer.py | 344 |
| C | GS000-LEGACY | api.py | 23 |
| C | GS000-LEGACY | api.py | 35 |
| C | GS000-LEGACY | api.py | 118 |
| C | GS000-LEGACY | api.py | 119 |
| C | GS000-LEGACY | api.py | 161 |
| C | GS000-LEGACY | api.py | 1341 |
| C | GS000-LEGACY | api.py | 1350 |
| C | GS000-LEGACY | types.py | 368 |
| C | GS000-LEGACY | types.py | 380 |
| C | GS000-LEGACY | types.py | 392 |
| C | GS000-LEGACY | types.py | 476 |
| H | GS025 | renovate.json | 0 |
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS004 | _worker_loop.py | 725 |
| H | GS004 | _worker_loop.py | 727 |
| C | GS005 | api.py | 1622 |
| C | GS005 | api.py | 1631 |
| s | GS009 |  | 0 |
| L | GS011 | tokens.py | 69 |
| L | GS011 | token.py | 244 |
| H | GS011 | token.py | 60 |
| H | GS019 | config.py | 16 |
| H | GS019 | config.py | 119 |
| H | GS019 | views.py | 79 |
| H | GS019 | responses.py | 140 |
| C | GS019 | settings.py | 23 |
| s | GS021 |  | 91 |
| s | GS021 |  | 288 |
| s | GS021 |  | 289 |
| s | GS021 |  | 235 |
| s | GS021 |  | 236 |
| s | GS021 |  | 16 |
| s | GS021 |  | 25 |
| s | GS021 |  | 43 |
| s | GS021 |  | 82 |
| s | GS021 |  | 2839 |
| s | GS021 |  | 27 |
| s | GS021 |  | 323 |
| s | GS021 |  | 123 |
| s | GS021 |  | 197 |
| s | GS021 |  | 228 |
| s | GS021 |  | 237 |
| s | GS021 |  | 256 |
| s | GS021 |  | 355 |
| s | GS021 |  | 358 |
| s | GS021 |  | 387 |
| s | GS021 |  | 391 |
| s | GS021 |  | 412 |
| s | GS021 |  | 418 |
| s | GS021 |  | 457 |
| s | GS021 |  | 12 |
| s | GS021 |  | 183 |
| s | GS021 |  | 756 |
| s | GS021 |  | 780 |
| s | GS021 |  | 797 |
| s | GS021 |  | 816 |
| s | GS021 |  | 845 |
| s | GS021 |  | 874 |
| s | GS021 |  | 908 |
| s | GS021 |  | 1290 |
| s | GS021 |  | 1454 |
| s | GS021 |  | 1455 |
| s | GS021 |  | 1475 |
| s | GS021 |  | 1479 |
| s | GS021 |  | 1503 |
| s | GS021 |  | 1504 |
| s | GS021 |  | 1682 |
| s | GS021 |  | 1713 |
| s | GS021 |  | 152 |
| s | GS021 |  | 153 |
| c | GS021 |  | 289 |
| c | GS021 |  | 324 |
| c | GS021 |  | 347 |
| s | GS021 |  | 187 |
| s | GS021 |  | 221 |
| s | GS021 |  | 300 |
| s | GS021 |  | 333 |
| s | GS021 |  | 353 |
| s | GS021 |  | 386 |
| s | GS021 |  | 412 |
| s | GS021 |  | 449 |
| s | GS021 |  | 515 |
| s | GS021 |  | 549 |
| s | GS021 |  | 234 |
| s | GS021 |  | 17 |
| s | GS021 |  | 835 |
| s | GS021 |  | 101 |
| s | GS021 |  | 102 |
| s | GS021 |  | 534 |
| s | GS021 |  | 534 |
| s | GS021 |  | 411 |
| s | GS021 |  | 135 |
| s | GS021 |  | 33 |
| s | GS021 |  | 45 |
| r | GS022 |  | 322 |
| r | GS022 |  | 325 |
| r | GS022 |  | 341 |
| r | GS022 |  | 375 |
| r | GS022 |  | 50 |
| r | GS022 |  | 409 |
| r | GS022 |  | 719 |
| r | GS022 |  | 829 |
| r | GS022 |  | 1063 |
| r | GS022 |  | 77 |
| r | GS022 |  | 100 |
| r | GS022 |  | 15 |
| r | GS022 |  | 42 |
| r | GS022 |  | 64 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | YAML-ECB85AD8 | error_handlers.py | ? |
| ? | YAML-ECB85AD8 | api.py | ? |
| ? | YAML-ECB85AD8 | state.rs | ? |
| ? | YAML-B39DC08C | mcp_oauth_client_demo.py | ? |
| ? | YAML-B39DC08C | mcp_oauth_client_demo.py | ? |
| ? | YAML-B39DC08C | mcp_oauth_client_demo.py | ? |
| ? | YAML-B39DC08C | mcp_oauth_client_demo.py | ? |
| ? | YAML-B39DC08C | benchmark.sh | ? |
| ? | YAML-B39DC08C | benchmark_compare.py | ? |
| ? | YAML-B39DC08C | benchmark_compare.py | ? |
| ? | YAML-B39DC08C | benchmark_compare.py | ? |
| ? | YAML-B39DC08C | benchmark_compare.py | ? |
| M | ? | workers.py | 59 |
| H | ? | server.rs | 289 |
| H | ? | server.rs | 667 |
| H | ? | server.rs | 676 |
| H | ? | server.rs | 707 |
| H | ? | server.rs | 717 |
| H | ? | server.rs | 726 |
| H | ? | server.rs | 759 |
| H | ? | server.rs | 760 |
| H | ? | server.rs | 780 |
| H | ? | server.rs | 781 |
| H | ? | server.rs | 800 |
| H | ? | server.rs | 805 |
| H | ? | server.rs | 806 |
| H | ? | server.rs | 837 |
| H | ? | server.rs | 880 |
| H | ? | server.rs | 1107 |
| H | ? | worker_loop.rs | 83 |
| H | ? | worker_loop.rs | 106 |
| H | ? | worker_loop.rs | 316 |
| H | ? | form_parsing.rs | 391 |
| H | ? | form_parsing.rs | 415 |
| H | ? | static_files.rs | 150 |
| H | ? | static_files.rs | 162 |
| H | ? | request.rs | 259 |
| H | ? | request.rs | 392 |
| H | ? | request.rs | 406 |
| H | ? | metadata.rs | 163 |
| H | ? | metadata.rs | 769 |
| H | ? | type_coercion.rs | 161 |
| H | ? | type_coercion.rs | 167 |
| H | ? | streaming.rs | 126 |
| H | ? | streaming.rs | 172 |
| H | ? | streaming.rs | 176 |
| H | ? | streaming.rs | 264 |
| H | ? | streaming.rs | 296 |
| H | ? | streaming.rs | 320 |
| H | ? | streaming.rs | 333 |
| H | ? | streaming.rs | 453 |
| H | ? | testing.rs | 75 |
| H | ? | testing.rs | 481 |
| H | ? | testing.rs | 525 |
| H | ? | testing.rs | 551 |
| H | ? | testing.rs | 552 |
| H | ? | testing.rs | 553 |
| H | ? | testing.rs | 554 |
| H | ? | testing.rs | 556 |
| H | ? | testing.rs | 557 |
| H | ? | testing.rs | 562 |
| H | ? | testing.rs | 563 |
| H | ? | testing.rs | 576 |
| H | ? | testing.rs | 579 |
| H | ? | testing.rs | 580 |
| H | ? | testing.rs | 581 |
| H | ? | testing.rs | 582 |
| H | ? | testing.rs | 583 |
| H | ? | testing.rs | 589 |
| H | ? | testing.rs | 590 |
| H | ? | testing.rs | 595 |
| H | ? | testing.rs | 596 |
| H | ? | testing.rs | 608 |
| H | ? | testing.rs | 613 |
| H | ? | testing.rs | 631 |
| H | ? | testing.rs | 645 |
| H | ? | testing.rs | 732 |
| H | ? | testing.rs | 1087 |
| H | ? | testing.rs | 1205 |
| H | ? | testing.rs | 1206 |
| H | ? | testing.rs | 1207 |
| H | ? | testing.rs | 1279 |
| H | ? | testing.rs | 1363 |
| H | ? | testing.rs | 1478 |
| H | ? | response_builder.rs | 95 |
| H | ? | handler.rs | 203 |
| H | ? | handler.rs | 261 |
| H | ? | handler.rs | 269 |
| H | ? | handler.rs | 290 |
| H | ? | handler.rs | 309 |
| H | ? | handler.rs | 343 |
| H | ? | handler.rs | 563 |
| H | ? | handler.rs | 603 |
| H | ? | handler.rs | 608 |
| H | ? | handler.rs | 618 |
| H | ? | handler.rs | 619 |
| H | ? | handler.rs | 663 |
| H | ? | handler.rs | 1086 |
| H | ? | permissions.rs | 196 |
| H | ? | permissions.rs | 369 |
| H | ? | registry.rs | 145 |
| H | ? | registry.rs | 236 |
| H | ? | mod.rs | 200 |
| H | ? | mod.rs | 206 |
| H | ? | handler.rs | 50 |
| H | ? | handler.rs | 103 |
| H | ? | handler.rs | 114 |
| H | ? | handler.rs | 205 |
| H | ? | handler.rs | 247 |
| H | ? | handler.rs | 281 |
| H | ? | handler.rs | 294 |
| H | ? | handler.rs | 317 |
| H | ? | handler.rs | 479 |
| H | ? | handler.rs | 486 |
| H | ? | handler.rs | 559 |
| H | ? | handler.rs | 574 |
| H | ? | handler.rs | 585 |
| H | ? | handler.rs | 607 |
| H | ? | state_codec.rs | 137 |
| H | ? | request_pipeline.rs | 52 |
| H | ? | request_pipeline.rs | 86 |
| H | ? | responses.rs | 33 |
| H | ? | responses.rs | 47 |
| H | ? | responses.rs | 84 |
| H | ? | cors.rs | 39 |
| H | ? | cors.rs | 50 |
| H | ? | cors.rs | 105 |
| H | ? | cors.rs | 115 |
| H | ? | cors.rs | 119 |
| H | ? | cors.rs | 123 |
| H | ? | auth.rs | 73 |
| H | ? | auth.rs | 80 |
| H | ? | auth.rs | 99 |
| H | ? | auth.rs | 151 |
| H | ? | auth.rs | 320 |
| H | ? | auth.rs | 660 |
| H | ? | auth.rs | 676 |
| H | ? | compression.rs | 76 |
| H | ? | compression.rs | 174 |
| H | ? | compression.rs | 179 |
| H | ? | rate_limit.rs | 86 |
| H | ? | rate_limit.rs | 87 |
| H | ? | cors.rs | 95 |
| H | ? | dev_reload.rs | 348 |
| H | ? | asgi_http.rs | 43 |
| H | ? | asgi_http.rs | 44 |
| H | ? | asgi_http.rs | 126 |
| H | ? | asgi_http.rs | 443 |
| H | ? | asgi_http.rs | 449 |
| H | ? | asgi_http.rs | 458 |
| H | ? | asgi_http.rs | 459 |

---
*Сгенерировано GSC v0.6 · 2026-08-10T14:31:27.172137*