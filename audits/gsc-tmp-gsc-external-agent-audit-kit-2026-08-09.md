---
title: "GSC Audit: /tmp/gsc-external/agent-audit-kit"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-external/agent-audit-kit

**Дата:** 09.08.2026 06:07  
**Путь:** `/tmp/gsc-external/agent-audit-kit`  
**Всего находок:** 609  
**CRITICAL:** 14 | **HIGH:** 89 | **MEDIUM:** 116 | **LOW:** 169

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 266 |
| GS021 | 67 |
| GS025-eval_usage | 50 |
| GS003 | 45 |
| YAML-36ACF0AD | 41 |
| GS025 | 31 |
| GS022 | 29 |
| GS008 | 19 |
| GS020 | 14 |
| Синхронный код в async | 13 |
| GS025-wildcard_bind | 6 |
| GS018 | 4 |
| GS025-permissive_cors | 3 |
| GS025-hardcoded_secret | 3 |
| GS001 | 2 |
| GS007 | 2 |
| GS029 | 2 |
| GS032-override_instruction | 2 |
| GS032-system_prompt_override | 2 |
| GS032-role_hijack | 1 |
| GS032-high_density | 1 |
| GS037-yaml_unsafe_load | 1 |
| GS037-command_injection_shell_true | 1 |
| GS009 | 1 |
| GS016 | 1 |
| YAML-B39DC08C | 1 |
| Deep analysis requires OpenRouter API key | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS025 | builtin.py | 1403 |  |
| CRITICAL | GS025 | builtin.py | 3215 |  |
| CRITICAL | GS025 | builtin.py | 4262 |  |
| CRITICAL | GS025 | builtin.py | 4516 |  |
| CRITICAL | GS025 | builtin.py | 5429 |  |
| CRITICAL | GS025 | crewai.py | 116 |  |
| CRITICAL | GS025 | stdio_injection.py | 74 |  |
| CRITICAL | GS025 | argv_toctou.py | 120 |  |
| CRITICAL | GS025 | skill_untrusted_exec_path.py | 201 |  |
| CRITICAL | GS025 | crewai_rce_chain.py | 183 |  |
| CRITICAL | GS025 | mcp_atlassian.py | 130 |  |
| CRITICAL | GS001 | tsconfig.json | 4 | Found: "ES2020" |
| CRITICAL | GS001 | tsconfig.json | 5 | Found: "ES2020" |
| CRITICAL | GS007 | builtin.py | 1473 | Match:     "A @tool function parameter is passed to pickle.l |
| HIGH | GS025 | index_builder.py | 171 |  |
| HIGH | GS025 | builtin.py | 4652 |  |
| HIGH | GS025 | builtin.py | 5281 |  |
| HIGH | GS025 | builtin.py | 5498 |  |
| HIGH | GS025 | mcp_config.py | 231 |  |
| HIGH | GS025 | supply_chain.py | 124 |  |
| HIGH | GS025 | builtin.py | 864 |  |
| HIGH | GS025 | ide_task_rce.py | 60 |  |
| HIGH | GS025 | hook_injection.py | 51 |  |
| HIGH | GS025 | builtin.py | 3828 |  |
| HIGH | GS000-LEGACY | findings.sarif | 292 | Match:             "text": "An MCP server uses HTTP transpor |
| HIGH | GS000-LEGACY | findings.sarif | 329 | Match:             "text": "The MCP server URL points to loc |
| HIGH | GS000-LEGACY | findings.sarif | 733 | Match:             "text": "An MCP server URL uses HTTP inst |
| HIGH | GS000-LEGACY | sample_03_no_auth.json | 10 | Match:       "url": "http://192.168.1.100:3000/sse", |
| HIGH | GS000-LEGACY | demo.cast | 57 | Match: [2.3592, "o", " rotate immediately, use environment v |
| HIGH | GS000-LEGACY | demo.cast | 59 | Match: [2.35923, "o", "nces or a secrets manager.\r\n    \u0 |
| HIGH | GS000-LEGACY | builtin.py | 489 | Match:     "CIDR that covers the public internet (0.0.0.0/0, |
| HIGH | GS000-LEGACY | builtin.py | 1963 | Match:     "127.0.0.1/localhost/::1, reaching internal servi |
| HIGH | GS000-LEGACY | builtin.py | 1976 | Match:     "An MCP tool accepts URLs that can reach 169.254. |
| HIGH | GS000-LEGACY | builtin.py | 1981 | Match:     "Block 169.254.0.0/16 and metadata.google.interna |
| HIGH | GS000-LEGACY | builtin.py | 3438 | Match:     "did not normalise IPv4-mapped IPv6 (`::ffff:127. |
| HIGH | GS000-LEGACY | builtin.py | 3625 | Match:     "custom domain to 127.0.0.1 via DNS rebinding and |
| HIGH | GS000-LEGACY | builtin.py | 3756 | Match:     "default 0.0.0.0 bind + zero authentication on SS |
| HIGH | GS000-LEGACY | builtin.py | 3762 | Match:     "bind the server to 127.0.0.1 and front it with a |
| HIGH | GS000-LEGACY | builtin.py | 3818 | Match:     "`http://169.254.169.254/...`, `http://localhost` |
| HIGH | GS000-LEGACY | builtin.py | 5305 | Match:     "interfaces (`0.0.0.0` / `::`) or serving a wildc |
| HIGH | GS000-LEGACY | builtin.py | 5312 | Match:     "`0.0.0.0` with wildcard CORS. Generalises the Az |
| HIGH | GS000-LEGACY | builtin.py | 5317 | Match:     "`command`/`args`), Docker `--host 0.0.0.0` / `-p |
| HIGH | GS000-LEGACY | builtin.py | 5319 | Match:     "interface (`0.0.0.0` / `::` / a routable IP) wit |
| HIGH | GS000-LEGACY | builtin.py | 5325 | Match:     "an HTTP MCP server bound to `0.0.0.0:8080` with  |
| HIGH | GS000-LEGACY | builtin.py | 5335 | Match:     "empty. Bind the listener to `127.0.0.1` (or behi |
| HIGH | GS000-LEGACY | builtin.py | 5336 | Match:     "reverse proxy) instead of `0.0.0.0`, never pass  |
| HIGH | GS000-LEGACY | builtin.py | 5469 | Match:     "the server binds a non-loopback interface (`0.0. |
| HIGH | GS000-LEGACY | builtin.py | 5480 | Match:     "constant-time check, bind to `127.0.0.1` behind  |
| HIGH | GS000-LEGACY | builtin.py | 5698 | Match:     "(also reject RFC 1918, 127.0.0.0/8, 169.254.0.0/ |
| HIGH | GS000-LEGACY | builtin.py | 5786 | Match:     "`ROOM_SECRET` is unset on a local 127.0.0.1 bind |
| HIGH | GS000-LEGACY | builtin.py | 5975 | Match:     "pinned below it is exposed to all of them. Defau |
| HIGH | GS000-LEGACY | builtin.py | 6014 | Match:     "`@penpot/mcp` before 2.15.0 binds its ReplServer |
| HIGH | GS000-LEGACY | builtin.py | 6274 | Match:     "127.0.0.1:8080 with no authentication and no Hos |
| HIGH | GS000-LEGACY | crewai.py | 28 | Match:     "192.168.", "0.0.0.0", |
| HIGH | GS000-LEGACY | mcp_http_noauth_server.py | 175 | Match:         bind = "0.0.0.0/::" |
| HIGH | GS000-LEGACY | mcp_http_noauth_server.py | 252 | Match:             exposure = "binds 0.0.0.0/::" if _BIND_AL |
| HIGH | GS000-LEGACY | mcp_http_noauth_server.py | 264 | Match:                     f"127.0.0.1." |
| HIGH | GS000-LEGACY | mcp_http_noauth_server.py | 266 | Match:                 find_line_number(raw, "0.0.0.0") or f |
| HIGH | GS000-LEGACY | mcp_http_noauth_server.py | 285 | Match:                 f"Bind 127.0.0.1 or require a bearer  |
| HIGH | GS000-LEGACY | ssrf_patterns.py | 103 | Match:             if ip in {"169.254.169.254", "metadata.go |
| HIGH | GS000-LEGACY | ssrf_patterns.py | 112 | Match:             elif ip in {"127.0.0.1", "localhost", ":: |
| HIGH | GS000-LEGACY | mcp_tunnel.py | 198 | Match: _PUBLIC_INTERNET_CIDRS_V4: tuple[str, ...] = ("0.0.0. |
| HIGH | GS000-LEGACY | interceptor.py | 130 | Match:         self._server_socket.bind(("127.0.0.1", p)) |
| HIGH | GS000-LEGACY | engine.py | 96 | Match:     ("mcp_http_noauth_server", "Unauthenticated MCP H |
| HIGH | GS000-LEGACY | scanners.json | 142 | Match:       "name": "Unauthenticated MCP HTTP/SSE server on |
| HIGH | GS000-LEGACY | rules.json | 821 | Match:       "description": "The upstream MCP Python, Java,  |
| HIGH | GS000-LEGACY | rules.json | 959 | Match:       "description": "Project depends on `excel-mcp-s |
| HIGH | GS000-LEGACY | rules.json | 969 | Match:       "remediation": "Upgrade `excel-mcp-server` to 0 |
| HIGH | GS000-LEGACY | rules.json | 992 | Match:       "description": "Package manifest depends on `fl |
| HIGH | GS000-LEGACY | rules.json | 1808 | Match:       "description": "A function calls a known SSRF g |
| HIGH | GS000-LEGACY | rules.json | 3104 | Match:       "description": "The Cline (`cline`) Hub dashboa |
| HIGH | GS000-LEGACY | rules.json | 3493 | Match:       "description": "A repository publishes an MCP s |
| HIGH | GS000-LEGACY | rules.json | 3501 | Match:       "remediation": "Require an inbound credential o |
| HIGH | GS000-LEGACY | rules.json | 3853 | Match:       "description": "An MCP server ships an authenti |
| HIGH | GS000-LEGACY | rules.json | 3861 | Match:       "remediation": "Fail closed: reject every reque |
| HIGH | GS000-LEGACY | rules.json | 3969 | Match:       "description": "`@penpot/mcp` before 2.15.0 bin |
| HIGH | GS000-LEGACY | rules.json | 3998 | Match:       "description": "PraisonAI before 4.6.78 exposes |
| HIGH | GS000-LEGACY | rules.json | 4217 | Match:       "remediation": "Deny by default: before fetchin |
| HIGH | GS000-LEGACY | rules.json | 4598 | Match:       "description": "An MCP Tunnels gateway-proxy co |
| HIGH | GS000-LEGACY | rules.json | 4680 | Match:       "description": "The WhatsApp MCP Server's `what |
| HIGH | GS000-LEGACY | rules.json | 6065 | Match:       "description": "An MCP tool handler forwards us |
| HIGH | GS000-LEGACY | rules.json | 6089 | Match:       "description": "An MCP tool accepts URLs that c |
| HIGH | GS000-LEGACY | rules.json | 6097 | Match:       "remediation": "Block 169.254.0.0/16 and metada |
| HIGH | GS008 | builtin.py | 1417 | Match:     "A @tool function parameter flows to eval(), exec |
| HIGH | GS008 | builtin.py | 4809 | Match:     "Unsafe eval()/exec()/compile() inside @mcp.tool  |
| HIGH | GS008 | builtin.py | 4811 | Match:     "`eval()`, `exec()`, `compile()`, `__import__()`, |
| HIGH | GS008 | builtin.py | 4825 | Match:     "Replace `eval(expr)` with `ast.literal_eval(expr |
| HIGH | GS008 | builtin.py | 4903 | Match:     "MCP Calculate Server eval() RCE (CVE-2026-44717, |
| HIGH | GS008 | builtin.py | 4906 | Match:     "expression is routed through `eval()` (SymPy-bac |
| HIGH | GS008 | builtin.py | 4913 | Match:     "broader source-detector for the unsafe-`eval()`  |
| HIGH | GS008 | builtin.py | 4920 | Match:     "If you maintain a similar MCP server, replace `e |
| HIGH | GS008 | typescript_pattern_scan.py | 44 | Match:         "eval() call detected in MCP server file", |
| HIGH | GS008 | mcp_tool_unsafe_eval.py | 145 | Match:                 title="Unsafe eval()/exec()/compile() |
| HIGH | GS008 | mcp_tool_unsafe_eval.py | 148 | Match:                     "`eval()`, `exec()`, `compile()`, |
| HIGH | GS008 | mcp_tool_unsafe_eval.py | 162 | Match:                     "Replace `eval(expr)` with `ast.l |
| HIGH | GS008 | hook_rce.py | 41 | Match:     r"""(?:subprocess\.(?:run|call|Popen|check_output |
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .agent-audit-kit.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | mkdocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | scanners.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | action.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | rules.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .pre-commit-hooks.yaml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS025 | builtin.py | 1403 |
| C | GS025 | builtin.py | 3215 |
| C | GS025 | builtin.py | 4262 |
| C | GS025 | builtin.py | 4516 |
| C | GS025 | builtin.py | 5429 |
| C | GS025 | crewai.py | 116 |
| C | GS025 | stdio_injection.py | 74 |
| C | GS025 | argv_toctou.py | 120 |
| C | GS025 | skill_untrusted_exec_path.py | 201 |
| C | GS025 | crewai_rce_chain.py | 183 |
| C | GS025 | mcp_atlassian.py | 130 |
| C | GS001 | tsconfig.json | 4 |
| C | GS001 | tsconfig.json | 5 |
| C | GS007 | builtin.py | 1473 |
| H | GS025 | index_builder.py | 171 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| L | GS000-LEGACY | mcp_toolgate_asymmetry.py | 151 |
| L | GS000-LEGACY | watch_csa_mcp_baseline.py | 101 |
| M | GS018 | baseline.py | 78 |
| M | GS018 | builtin.py | 5145 |
| M | GS018 | project_deal_drift.py | 131 |
| M | GS018 | compliance.py | 443 |
| M | GS025 | gen_coverage.py | 148 |
| M | GS025 | gen_coverage.py | 154 |
| M | GS025 | gen_coverage.py | 161 |
| M | GS007 | builtin.py | 1473 |
| H | GS025 | builtin.py | 4652 |
| H | GS025 | builtin.py | 5281 |
| H | GS025 | builtin.py | 5498 |
| H | GS025 | mcp_config.py | 231 |
| H | GS025 | supply_chain.py | 124 |
| H | GS025 | builtin.py | 864 |
| H | GS025 | ide_task_rce.py | 60 |
| H | GS025 | hook_injection.py | 51 |
| H | GS025 | builtin.py | 3828 |
| M | GS020 | builtin.py | 2788 |
| M | GS020 | builtin.py | 2797 |
| M | GS020 | mcp_apps_ui.py | 79 |
| M | GS029 | cli.py | 1238 |
| M | GS029 | cli.py | 1250 |
| L | GS003 | crawler.py | 464 |
| L | GS003 | crawler.py | 465 |
| L | GS003 | crawler.py | 466 |
| L | GS003 | crawler.py | 467 |
| L | GS003 | crawler.py | 468 |
| L | GS003 | crawler.py | 469 |
| L | GS003 | crawler.py | 470 |
| L | GS003 | crawler.py | 471 |
| L | GS003 | crawler.py | 474 |
| L | GS003 | crawler.py | 475 |
| L | GS003 | crawler.py | 476 |
| L | GS003 | crawler.py | 477 |
| L | GS003 | crawler.py | 478 |
| L | GS003 | crawler.py | 480 |
| L | GS003 | crawler.py | 482 |
| L | GS003 | crawler.py | 483 |
| L | GS003 | run.py | 197 |
| L | GS003 | run.py | 199 |
| L | GS003 | run.py | 202 |
| L | GS003 | corpus.py | 123 |
| L | GS003 | corpus.py | 124 |
| L | GS003 | corpus.py | 125 |
| L | GS003 | corpus.py | 126 |
| L | GS003 | run.py | 153 |
| L | GS003 | run.py | 154 |
| L | GS003 | run.py | 165 |
| L | GS003 | run.py | 167 |
| L | GS003 | index_builder.py | 509 |
| L | GS003 | baseline.py | 457 |
| L | GS003 | baseline.py | 474 |
| L | GS003 | fetch_registry.py | 156 |
| L | GS003 | fetch_registry.py | 189 |
| L | GS003 | run_report.py | 331 |
| L | GS003 | gen_coverage.py | 156 |
| L | GS003 | gen_coverage.py | 172 |
| L | GS003 | generate_lockfile.py | 65 |
| L | GS003 | generate_lockfile.py | 68 |
| L | GS003 | generate_lockfile.py | 76 |
| L | GS003 | mcp_2026_07_28_readiness.py | 88 |
| L | GS003 | mcp_2026_07_28_readiness.py | 90 |
| L | GS003 | mcp_2026_07_28_readiness.py | 92 |
| L | GS003 | mcp_2026_07_28_readiness.py | 93 |
| L | GS003 | mcp_2026_07_28_readiness.py | 95 |
| L | GS003 | mcp_2026_07_28_readiness.py | 97 |
| L | GS003 | mcp_2026_07_28_readiness.py | 101 |
| L | GS008 | cli.py | 25 |
| L | GS008 | _helpers.py | 12 |
| L | GS008 | mcp_middleware.py | 46 |
| L | GS008 | pin_drift.py | 20 |
| L | GS008 | stdio_injection.py | 44 |
| L | GS008 | crawler.py | 38 |
| i | GS020 |  | 390 |
| i | GS020 |  | 56 |
| i | GS020 |  | 59 |
| i | GS020 |  | 79 |
| i | GS020 |  | 82 |
| i | GS020 |  | 2789 |
| i | GS020 |  | 2798 |
| i | GS020 |  | 21 |
| i | GS020 |  | 82 |
| i | GS020 |  | 294 |
| i | GS020 |  | 298 |
| ? | GS032-override_instruction | builtin.py | 1329 |
| ? | GS032-override_instruction | builtin.py | 4239 |
| ? | GS032-role_hijack | builtin.py | 2884 |
| ? | GS032-system_prompt_override | builtin.py | 1329 |
| ? | GS032-system_prompt_override | builtin.py | 4239 |
| ? | GS032-high_density | builtin.py | 1 |
| ? | GS037-yaml_unsafe_load | builtin.py | 1473 |
| ? | GS037-command_injection_shell_true | mcp_stdio_params.py | 13 |
| H | GS000-LEGACY | findings.sarif | 292 |
| H | GS000-LEGACY | findings.sarif | 329 |
| H | GS000-LEGACY | findings.sarif | 733 |
| H | GS000-LEGACY | sample_03_no_auth.json | 10 |
| H | GS000-LEGACY | demo.cast | 57 |
| H | GS000-LEGACY | demo.cast | 59 |
| H | GS000-LEGACY | builtin.py | 489 |
| H | GS000-LEGACY | builtin.py | 1963 |
| H | GS000-LEGACY | builtin.py | 1976 |
| H | GS000-LEGACY | builtin.py | 1981 |
| H | GS000-LEGACY | builtin.py | 3438 |
| H | GS000-LEGACY | builtin.py | 3625 |
| H | GS000-LEGACY | builtin.py | 3756 |
| H | GS000-LEGACY | builtin.py | 3762 |
| H | GS000-LEGACY | builtin.py | 3818 |
| H | GS000-LEGACY | builtin.py | 5305 |
| H | GS000-LEGACY | builtin.py | 5312 |
| H | GS000-LEGACY | builtin.py | 5317 |
| H | GS000-LEGACY | builtin.py | 5319 |
| H | GS000-LEGACY | builtin.py | 5325 |
| H | GS000-LEGACY | builtin.py | 5335 |
| H | GS000-LEGACY | builtin.py | 5336 |
| H | GS000-LEGACY | builtin.py | 5469 |
| H | GS000-LEGACY | builtin.py | 5480 |
| H | GS000-LEGACY | builtin.py | 5698 |
| H | GS000-LEGACY | builtin.py | 5786 |
| H | GS000-LEGACY | builtin.py | 5975 |
| H | GS000-LEGACY | builtin.py | 6014 |
| H | GS000-LEGACY | builtin.py | 6274 |
| H | GS000-LEGACY | crewai.py | 28 |
| H | GS000-LEGACY | mcp_http_noauth_server.py | 175 |
| H | GS000-LEGACY | mcp_http_noauth_server.py | 252 |
| H | GS000-LEGACY | mcp_http_noauth_server.py | 264 |
| H | GS000-LEGACY | mcp_http_noauth_server.py | 266 |
| H | GS000-LEGACY | mcp_http_noauth_server.py | 285 |
| H | GS000-LEGACY | ssrf_patterns.py | 103 |
| H | GS000-LEGACY | ssrf_patterns.py | 112 |
| H | GS000-LEGACY | mcp_tunnel.py | 198 |
| H | GS000-LEGACY | interceptor.py | 130 |
| H | GS000-LEGACY | engine.py | 96 |
| H | GS000-LEGACY | scanners.json | 142 |
| H | GS000-LEGACY | rules.json | 821 |
| H | GS000-LEGACY | rules.json | 959 |
| H | GS000-LEGACY | rules.json | 969 |
| H | GS000-LEGACY | rules.json | 992 |
| H | GS000-LEGACY | rules.json | 1808 |
| H | GS000-LEGACY | rules.json | 3104 |
| H | GS000-LEGACY | rules.json | 3493 |
| H | GS000-LEGACY | rules.json | 3501 |
| H | GS000-LEGACY | rules.json | 3853 |
| H | GS000-LEGACY | rules.json | 3861 |
| H | GS000-LEGACY | rules.json | 3969 |
| H | GS000-LEGACY | rules.json | 3998 |
| H | GS000-LEGACY | rules.json | 4217 |
| H | GS000-LEGACY | rules.json | 4598 |
| H | GS000-LEGACY | rules.json | 4680 |
| H | GS000-LEGACY | rules.json | 6065 |
| H | GS000-LEGACY | rules.json | 6089 |
| H | GS000-LEGACY | rules.json | 6097 |
| M | GS000-LEGACY | builtin.py | 1183 |
| M | GS000-LEGACY | builtin.py | 3353 |
| M | GS000-LEGACY | builtin.py | 3354 |
| M | GS000-LEGACY | builtin.py | 3655 |
| M | GS000-LEGACY | builtin.py | 3656 |
| M | GS000-LEGACY | builtin.py | 4097 |
| M | GS000-LEGACY | builtin.py | 4349 |
| M | GS000-LEGACY | builtin.py | 4647 |
| M | GS000-LEGACY | builtin.py | 4912 |
| M | GS000-LEGACY | builtin.py | 4939 |
| M | GS000-LEGACY | builtin.py | 5022 |
| M | GS000-LEGACY | builtin.py | 5023 |
| M | GS000-LEGACY | builtin.py | 5056 |
| M | GS000-LEGACY | builtin.py | 5079 |
| M | GS000-LEGACY | builtin.py | 5096 |
| M | GS000-LEGACY | builtin.py | 6477 |
| M | GS000-LEGACY | builtin.py | 6503 |
| M | GS000-LEGACY | fix.py | 184 |
| M | GS000-LEGACY | fix.py | 188 |
| M | GS000-LEGACY | fix.py | 205 |
| M | GS000-LEGACY | stdio_injection.py | 336 |
| M | GS000-LEGACY | log_token_leak.py | 204 |
| M | GS000-LEGACY | log_token_leak.py | 205 |
| M | GS000-LEGACY | log_token_leak.py | 209 |
| M | GS000-LEGACY | log_token_leak.py | 211 |
| M | GS000-LEGACY | log_token_leak.py | 229 |
| M | GS000-LEGACY | log_token_leak.py | 233 |
| M | GS000-LEGACY | mcp_deprecated_features.py | 45 |
| M | GS000-LEGACY | ssrf_redirect.py | 299 |
| M | GS000-LEGACY | ssrf_redirect.py | 300 |
| M | GS000-LEGACY | ssrf_toctou.py | 222 |
| M | GS000-LEGACY | ssrf_toctou.py | 223 |
| M | GS000-LEGACY | mcp_sampling_capability.py | 106 |
| M | GS000-LEGACY | mcp_sampling_capability.py | 114 |
| M | GS000-LEGACY | mcp_sampling_capability.py | 131 |
| M | GS000-LEGACY | mcp_sampling_capability.py | 142 |
| M | GS000-LEGACY | neo4j_cve.py | 28 |
| M | GS000-LEGACY | oauth_surface.py | 177 |
| M | GS000-LEGACY | oauth_surface.py | 186 |
| M | GS000-LEGACY | oauth_surface.py | 220 |
| M | GS000-LEGACY | oauth_surface.py | 224 |
| M | GS000-LEGACY | marketplace_manifest.py | 191 |
| M | GS000-LEGACY | marketplace_manifest.py | 193 |
| M | GS000-LEGACY | marketplace_manifest.py | 207 |
| M | GS000-LEGACY | marketplace_manifest.py | 209 |
| M | GS000-LEGACY | supply_chain.py | 206 |
| M | GS000-LEGACY | supply_chain.py | 208 |
| M | GS000-LEGACY | supply_chain.py | 244 |
| M | GS000-LEGACY | supply_chain.py | 254 |
| M | GS000-LEGACY | supply_chain.py | 257 |
| M | GS000-LEGACY | supply_chain.py | 267 |
| M | GS000-LEGACY | supply_chain.py | 290 |
| M | GS000-LEGACY | supply_chain.py | 446 |
| M | GS000-LEGACY | supply_chain.py | 447 |
| M | GS000-LEGACY | supply_chain.py | 590 |
| M | GS000-LEGACY | supply_chain.py | 644 |
| M | GS000-LEGACY | supply_chain.py | 645 |
| M | GS000-LEGACY | supply_chain.py | 705 |
| M | GS000-LEGACY | supply_chain.py | 706 |
| M | GS000-LEGACY | supply_chain.py | 763 |
| M | GS000-LEGACY | supply_chain.py | 764 |
| M | GS000-LEGACY | supply_chain.py | 825 |
| M | GS000-LEGACY | supply_chain.py | 1025 |
| M | GS000-LEGACY | mcp_cve_pins_2026_07.py | 271 |
| M | GS000-LEGACY | mcp_cve_pins_2026_07.py | 272 |
| M | GS000-LEGACY | mcp_sdk_hardening.py | 80 |
| M | GS000-LEGACY | mcp_sdk_hardening.py | 88 |
| M | GS000-LEGACY | mcp_sdk_hardening.py | 102 |
| M | GS000-LEGACY | mcp_sdk_hardening.py | 113 |
| M | GS000-LEGACY | legal_compliance.py | 25 |
| M | GS000-LEGACY | legal_compliance.py | 28 |
| M | GS000-LEGACY | legal_compliance.py | 32 |
| M | GS000-LEGACY | legal_compliance.py | 55 |
| M | GS000-LEGACY | mcp_stateless_migration.py | 82 |
| M | GS000-LEGACY | mcp_stateless_migration.py | 90 |
| M | GS000-LEGACY | mcp_stateless_migration.py | 107 |
| M | GS000-LEGACY | mcp_stateless_migration.py | 118 |
| M | GS000-LEGACY | dns_rebind.py | 146 |
| M | GS000-LEGACY | dns_rebind.py | 151 |
| M | GS000-LEGACY | dns_rebind.py | 160 |
| M | GS000-LEGACY | langchain_vuln.py | 25 |
| M | GS000-LEGACY | langchain_vuln.py | 28 |
| M | GS000-LEGACY | langchain_vuln.py | 62 |
| M | GS000-LEGACY | langchain_vuln.py | 66 |
| M | GS000-LEGACY | langchain_vuln.py | 175 |
| M | GS000-LEGACY | sbom.py | 96 |
| M | GS000-LEGACY | sbom.py | 154 |
| M | GS000-LEGACY | sync_repo_metadata.py | 35 |
| M | GS000-LEGACY | gen_owasp_coverage.py | 54 |
| H | GS008 | builtin.py | 1417 |
| H | GS008 | builtin.py | 4809 |
| H | GS008 | builtin.py | 4811 |
| H | GS008 | builtin.py | 4825 |
| H | GS008 | builtin.py | 4903 |
| H | GS008 | builtin.py | 4906 |
| H | GS008 | builtin.py | 4913 |
| H | GS008 | builtin.py | 4920 |
| H | GS008 | typescript_pattern_scan.py | 44 |
| H | GS008 | mcp_tool_unsafe_eval.py | 145 |
| H | GS008 | mcp_tool_unsafe_eval.py | 148 |
| H | GS008 | mcp_tool_unsafe_eval.py | 162 |
| H | GS008 | hook_rce.py | 41 |
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS025 | .agent-audit-kit.yml | 0 |
| H | GS025 | mkdocs.yml | 0 |
| H | GS025 | scanners.json | 0 |
| H | GS025 | action.yml | 0 |
| H | GS025 | rules.json | 0 |
| H | GS025 | .pre-commit-hooks.yaml | 0 |
| s | GS009 |  | 0 |
| M | GS016 | skill_untrusted_exec_path.py | 70 |
| s | GS021 |  | 146 |
| s | GS021 |  | 96 |
| s | GS021 |  | 26 |
| s | GS021 |  | 29 |
| s | GS021 |  | 18 |
| s | GS021 |  | 9 |
| s | GS021 |  | 9 |
| s | GS021 |  | 5 |
| s | GS021 |  | 8 |
| s | GS021 |  | 433 |
| s | GS021 |  | 434 |
| s | GS021 |  | 439 |
| s | GS021 |  | 489 |
| s | GS021 |  | 1961 |
| s | GS021 |  | 1963 |
| s | GS021 |  | 1963 |
| s | GS021 |  | 2084 |
| s | GS021 |  | 3438 |
| s | GS021 |  | 3625 |
| s | GS021 |  | 3756 |
| s | GS021 |  | 3762 |
| s | GS021 |  | 3818 |
| s | GS021 |  | 3855 |
| s | GS021 |  | 5305 |
| s | GS021 |  | 5312 |
| s | GS021 |  | 5317 |
| s | GS021 |  | 5317 |
| s | GS021 |  | 5319 |
| s | GS021 |  | 5325 |
| s | GS021 |  | 5335 |
| s | GS021 |  | 5336 |
| s | GS021 |  | 5336 |
| s | GS021 |  | 5469 |
| s | GS021 |  | 5480 |
| s | GS021 |  | 5786 |
| s | GS021 |  | 5975 |
| s | GS021 |  | 6014 |
| s | GS021 |  | 6274 |
| s | GS021 |  | 1976 |
| s | GS021 |  | 3818 |
| s | GS021 |  | 1977 |
| s | GS021 |  | 1981 |
| s | GS021 |  | 28 |
| s | GS021 |  | 5 |
| s | GS021 |  | 175 |
| s | GS021 |  | 252 |
| s | GS021 |  | 264 |
| s | GS021 |  | 266 |
| s | GS021 |  | 285 |
| s | GS021 |  | 11 |
| s | GS021 |  | 19 |
| s | GS021 |  | 38 |
| s | GS021 |  | 22 |
| s | GS021 |  | 23 |
| s | GS021 |  | 72 |
| s | GS021 |  | 31 |
| s | GS021 |  | 36 |
| s | GS021 |  | 112 |
| s | GS021 |  | 112 |
| s | GS021 |  | 112 |
| s | GS021 |  | 103 |
| s | GS021 |  | 103 |
| s | GS021 |  | 42 |
| s | GS021 |  | 198 |
| s | GS021 |  | 130 |
| s | GS021 |  | 164 |
| s | GS021 |  | 71 |
| r | GS022 |  | 11 |
| r | GS022 |  | 24 |
| r | GS022 |  | 3 |
| r | GS022 |  | 14 |
| r | GS022 |  | 5 |
| r | GS022 |  | 7 |
| r | GS022 |  | 4 |
| r | GS022 |  | 9 |
| r | GS022 |  | 4 |
| r | GS022 |  | 9 |
| r | GS022 |  | 4 |
| r | GS022 |  | 9 |
| r | GS022 |  | 7 |
| r | GS022 |  | 12 |
| r | GS022 |  | 36 |
| r | GS022 |  | 62 |
| r | GS022 |  | 65 |
| r | GS022 |  | 2058 |
| r | GS022 |  | 4566 |
| r | GS022 |  | 21 |
| r | GS022 |  | 77 |
| r | GS022 |  | 83 |
| r | GS022 |  | 4 |
| r | GS022 |  | 6 |
| r | GS022 |  | 37 |
| r | GS022 |  | 75 |
| r | GS022 |  | 220 |
| r | GS022 |  | 53 |
| r | GS022 |  | 41 |
| ? | GS025-permissive_cors |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-permissive_cors |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-permissive_cors |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | builtin.py | ? |
| ? | YAML-36ACF0AD | hook_rce.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | mcp_tool_unsafe_eval.py | ? |
| ? | YAML-36ACF0AD | supply_chain.py | ? |
| ? | YAML-36ACF0AD | supply_chain.py | ? |
| ? | YAML-36ACF0AD | supply_chain.py | ? |
| ? | YAML-36ACF0AD | taint_analysis.py | ? |
| ? | YAML-36ACF0AD | typescript_pattern_scan.py | ? |
| ? | YAML-36ACF0AD | typescript_pattern_scan.py | ? |
| ? | YAML-36ACF0AD | typescript_pattern_scan.py | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-36ACF0AD | rules.json | ? |
| ? | YAML-B39DC08C | crawler.py | ? |
| M | ? | crawler.py | 264 |
| M | ? | diff.py | 23 |
| M | ? | builtin.py | 2247 |
| M | ? | builtin.py | 3223 |
| M | ? | builtin.py | 4262 |
| M | ? | builtin.py | 5428 |
| M | ? | stdio_injection.py | 72 |
| M | ? | toxic_flow_pairs.yml | 52 |
| M | ? | advisories.py | 143 |
| M | ? | rules.json | 1405 |
| M | ? | rules.json | 2794 |
| M | ? | rules.json | 2848 |
| M | ? | rules.json | 6258 |
| I | ? |  | 0 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T06:07:02.811540*