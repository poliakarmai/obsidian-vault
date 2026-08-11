---
title: "GSC Audit: /home/openclaw/gsc"
date: 2026-08-06
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc

**Дата:** 06.08.2026 21:47  
**Путь:** `/home/openclaw/gsc`  
**Всего находок:** 1323  
**CRITICAL:** 306 | **HIGH:** 104 | **MEDIUM:** 114 | **LOW:** 682

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 432 |
| GS001 | 191 |
| Синхронный код в async | 82 |
| GS008 | 73 |
| GS005 | 61 |
| GS007 | 58 |
| GS021 | 25 |
| GS025-eval_usage | 20 |
| SQL injection risk: f-string in query | 16 |
| GS020 | 16 |
| CVE-2026-55721: SQL injection | 15 |
| CVE-2026-56233: Privilege escalation | 15 |
| Хардкод IP адреса | 15 |
| eval() or exec() usage | 11 |
| GS022 | 11 |
| CVE-2026-56413: Command injection | 10 |
| Bare except: | 8 |
| CVE-2026-56356: Cross-site scripting (XSS) | 8 |
| GS024 | 6 |
| TS: any type escape hatch | 5 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 5 |
| Python: raw string concatenation in SQL | 4 |
| CVE-2026-56219: Authentication bypass | 4 |
| GS014 | 4 |
| GS025-hardcoded_secret | 4 |
| Generic code smell #24 | 3 |
| Generic code smell #27 | 3 |
| Generic code smell #30 | 3 |
| Generic code smell #33 | 3 |
| Generic code smell #36 | 3 |
| Generic code smell #39 | 3 |
| Generic code smell #42 | 3 |
| Generic code smell #45 | 3 |
| Generic code smell #48 | 3 |
| Generic code smell #51 | 3 |
| Generic code smell #54 | 3 |
| Generic code smell #57 | 3 |
| Generic code smell #60 | 3 |
| Generic code smell #63 | 3 |
| Generic code smell #66 | 3 |
| Generic code smell #69 | 3 |
| Generic code smell #72 | 3 |
| Generic code smell #75 | 3 |
| Generic code smell #78 | 3 |
| Generic code smell #81 | 3 |
| Generic code smell #84 | 3 |
| Generic code smell #87 | 3 |
| Generic code smell #90 | 3 |
| Generic code smell #93 | 3 |
| Generic code smell #96 | 3 |
| Generic code smell #99 | 3 |
| Generic code smell #102 | 3 |
| Generic code smell #105 | 3 |
| Generic code smell #108 | 3 |
| Generic code smell #111 | 3 |
| Generic code smell #114 | 3 |
| Generic code smell #117 | 3 |
| Generic code smell #120 | 3 |
| Generic code smell #123 | 3 |
| Generic code smell #126 | 3 |
| Generic code smell #129 | 3 |
| Generic code smell #132 | 3 |
| Generic code smell #135 | 3 |
| Generic code smell #138 | 3 |
| Generic code smell #141 | 3 |
| Generic code smell #144 | 3 |
| Generic code smell #147 | 3 |
| Generic code smell #150 | 3 |
| Generic code smell #153 | 3 |
| Generic code smell #156 | 3 |
| Generic code smell #159 | 3 |
| Generic code smell #162 | 3 |
| Generic code smell #165 | 3 |
| Generic code smell #168 | 3 |
| Generic code smell #171 | 3 |
| Generic code smell #174 | 3 |
| Generic code smell #177 | 3 |
| Generic code smell #180 | 3 |
| Generic code smell #183 | 3 |
| Generic code smell #186 | 3 |
| Generic code smell #189 | 3 |
| Generic code smell #192 | 3 |
| Generic code smell #195 | 3 |
| Generic code smell #198 | 3 |
| Python: SSRF via requests without URL validation | 3 |
| CVE-2026-54696: Buffer overflow | 3 |
| CVE-2026-55223: Insecure deserialization | 3 |
| flipkart-incubator/Astra: modules/jwt_attack.py | 3 |
| User-controlled URL in request | 3 |
| GS004 | 3 |
| CVE-2026-56233: Path traversal | 2 |
| sileht/bird-lg: lg.py | 2 |
| poliakarmai/gsc: gsc_collect_light.py | 2 |
| CVE-2026-37270: Hardcoded credential | 2 |
| os.system() without sanitization | 2 |
| Systemd: EnvironmentFile without quotes → word splitting | 2 |
| Systemd: Type=forking without PIDFile | 2 |
| GS012 | 2 |
| Python: File upload without content-type validation | 1 |
| FastAPI: **body spread | 1 |
| Postgres URL with password | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| Systemd: User=root or absent → runs as root | 1 |
| Systemd: AmbientCapabilities with ALL caps | 1 |
| World-readable file: .mcp.json (664) | 1 |
| GS009 | 1 |
| GS016 | 1 |
| GS019 | 1 |
| GS025-debug_mode | 1 |
| Go: sync.Mutex copy | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | gsc_metrics.py | 31 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 8 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 12 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 15 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 19 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 20 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 23 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 28 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 31 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 37 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 39 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 43 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 46 | OWASP A03: Injection |
| CRITICAL | ? | gs018_payment_abuse.py | 215 | OWASP A03: Injection |
| CRITICAL | ? | gs020_llm_sqli.py | 126 | OWASP A03: Injection |
| CRITICAL | ? | gs020_llm_sqli.py | 230 | OWASP A03: Injection |
| CRITICAL | ? | corpus_gs005_python.py | 11 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | corpus_gs005_python.py | 16 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | corpus_gs005_python.py | 24 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | corpus_gs005_python.py | 25 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | gsc_metrics.py | 31 |  |
| CRITICAL | ? | corpus_gs005_python.py | 8 |  |
| CRITICAL | ? | corpus_gs005_python.py | 12 |  |
| CRITICAL | ? | corpus_gs005_python.py | 15 |  |
| CRITICAL | ? | corpus_gs005_python.py | 19 |  |
| CRITICAL | ? | corpus_gs005_python.py | 20 |  |
| CRITICAL | ? | corpus_gs005_python.py | 23 |  |
| CRITICAL | ? | corpus_gs005_python.py | 28 |  |
| CRITICAL | ? | corpus_gs005_python.py | 31 |  |
| CRITICAL | ? | corpus_gs005_python.py | 37 |  |
| CRITICAL | ? | corpus_gs005_python.py | 39 |  |
| CRITICAL | ? | corpus_gs005_python.py | 43 |  |
| CRITICAL | ? | corpus_gs005_python.py | 46 |  |
| CRITICAL | ? | gs020_llm_sqli.py | 126 |  |
| CRITICAL | ? | gs020_llm_sqli.py | 230 |  |
| CRITICAL | ? | _cron_collect.py | 141 |  |
| CRITICAL | ? | gsc_pdf.py | 15 |  |
| CRITICAL | ? | gsc.py | 1264 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 38 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 43 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 48 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 115 |  |
| CRITICAL | ? | gsc_collect_light.py | 212 |  |
| CRITICAL | ? | gsc_vuln_spider.py | 29 |  |
| CRITICAL | ? | gsc_vuln_spider.py | 187 |  |
| CRITICAL | ? | _cron_collect.py | 139 |  |
| CRITICAL | ? | gsc_collect_light.py | 210 |  |
| CRITICAL | ? | _cron_collect.py | 140 |  |
| CRITICAL | ? | gsc_collect_light.py | 211 |  |
| CRITICAL | ? | gsc_vuln_spider.py | 39 |  |
| CRITICAL | GS001 | _cron_collect.py | 17 | Found: "GS001" |
| CRITICAL | GS001 | _cron_collect.py | 20 | Found: "GS005" |
| CRITICAL | GS001 | _cron_collect.py | 23 | Found: "GS004" |
| CRITICAL | GS001 | _cron_collect.py | 29 | Found: "GS004" |
| CRITICAL | GS001 | _cron_collect.py | 38 | Found: "GS011" |
| CRITICAL | GS001 | _cron_collect.py | 46 | Found: "GS014" |
| CRITICAL | GS001 | _cron_collect.py | 49 | Found: "GS014" |
| CRITICAL | GS001 | _cron_collect.py | 139 | Found: "GS001" |
| CRITICAL | GS001 | _cron_collect.py | 140 | Found: "GS011" |
| CRITICAL | GS001 | _cron_collect.py | 141 | Found: "GS004" |
| CRITICAL | GS001 | _cron_collect.py | 142 | Found: "GS005" |
| CRITICAL | GS001 | _cron_collect.py | 143 | Found: "GS014" |
| CRITICAL | GS001 | _cron_nvd.py | 15 | Found: "GS001" |
| CRITICAL | GS001 | _cron_nvd.py | 18 | Found: "GS005" |
| CRITICAL | GS001 | _cron_nvd.py | 21 | Found: "GS004" |
| CRITICAL | GS001 | _cron_nvd.py | 27 | Found: "GS004" |
| CRITICAL | GS001 | _cron_nvd.py | 36 | Found: "GS011" |
| CRITICAL | GS001 | _cron_nvd.py | 44 | Found: "GS014" |
| CRITICAL | GS001 | _cron_nvd.py | 47 | Found: "GS014" |
| CRITICAL | GS001 | click.json | 9 | Found: "GS001" |
| CRITICAL | GS001 | flask-jwt-auth.json | 7 | Found: "GS011" |
| CRITICAL | GS001 | flask-jwt-auth.json | 8 | Found: "GS019" |
| CRITICAL | GS001 | github_auth.py | 40 | Found: "RS256" |
| CRITICAL | GS001 | manifest.json | 249 | Found: "bb0744740ba2e343a19f4d77f388842a" |
| CRITICAL | GS001 | manifest.json | 250 | Found: "bb0744740ba2e343a19f4d77f388842a" |
| CRITICAL | GS001 | manifest.json | 289 | Found: "dd648e75e997d21b11471747b746a2f0" |
| CRITICAL | GS001 | manifest.json | 290 | Found: "dd648e75e997d21b11471747b746a2f0" |
| CRITICAL | GS001 | manifest.json | 339 | Found: "cc350016c2c90504944929ddcae40500" |
| CRITICAL | GS001 | manifest.json | 340 | Found: "cc350016c2c90504944929ddcae40500" |
| CRITICAL | GS001 | manifest.json | 344 | Found: "df82b30c519a4adb8fa80b6fd3b3990f" |
| CRITICAL | GS001 | manifest.json | 345 | Found: "df82b30c519a4adb8fa80b6fd3b3990f" |
| CRITICAL | GS001 | gsc_blocking.py | 55 | Found: "GS028" |
| CRITICAL | GS001 | gsc_chain_composer.py | 26 | Found: "GS001" |
| CRITICAL | GS001 | gsc_chain_composer.py | 26 | Found: "GS004" |
| CRITICAL | GS001 | gsc_chain_composer.py | 26 | Found: "GS005" |
| CRITICAL | GS001 | gsc_chain_composer.py | 27 | Found: "GS007" |
| CRITICAL | GS001 | gsc_chain_composer.py | 27 | Found: "GS012" |
| CRITICAL | GS001 | gsc_chain_composer.py | 28 | Found: "GS014" |
| CRITICAL | GS001 | gsc_chain_composer.py | 29 | Found: "GS019" |
| CRITICAL | GS001 | gsc_chain_composer.py | 29 | Found: "GS011" |
| CRITICAL | GS001 | gsc_chain_composer.py | 30 | Found: "GS022" |
| CRITICAL | GS001 | gsc_chain_composer.py | 30 | Found: "GS021" |
| CRITICAL | GS001 | gsc_chain_composer.py | 31 | Found: "GS020" |
| CRITICAL | GS001 | gsc_chain_composer.py | 32 | Found: "GS024" |
| CRITICAL | GS001 | gsc_chain_composer.py | 38 | Found: "GS010" |
| CRITICAL | GS001 | gsc_chain_composer.py | 38 | Found: "GS016" |
| CRITICAL | GS001 | gsc_collect_light.py | 44 | Found: "GS001" |
| CRITICAL | GS001 | gsc_collect_light.py | 47 | Found: "GS005" |
| CRITICAL | GS001 | gsc_collect_light.py | 50 | Found: "GS004" |
| CRITICAL | GS001 | gsc_collect_light.py | 56 | Found: "GS004" |
| CRITICAL | GS001 | gsc_collect_light.py | 65 | Found: "GS011" |
| CRITICAL | GS001 | gsc_collect_light.py | 73 | Found: "GS014" |
| CRITICAL | GS001 | gsc_collect_light.py | 76 | Found: "GS014" |
| CRITICAL | GS001 | gsc_collect_light.py | 210 | Found: "GS001" |
| CRITICAL | GS001 | gsc_collect_light.py | 211 | Found: "GS011" |
| CRITICAL | GS001 | gsc_collect_light.py | 212 | Found: "GS004" |
| CRITICAL | GS001 | gsc_collect_light.py | 213 | Found: "GS005" |
| CRITICAL | GS001 | gsc_collect_light.py | 214 | Found: "GS014" |
| CRITICAL | GS001 | gs001_hardcoded_secret.py | 20 | Found: "GS001" |
| CRITICAL | GS001 | gs001_hardcoded_secret.py | 98 | Found: "GS001" |
| CRITICAL | GS001 | gs002_world_readable.py | 18 | Found: "GS002" |
| CRITICAL | GS001 | gs002_world_readable.py | 45 | Found: "GS002" |
| CRITICAL | GS001 | gs003_debug_prints.py | 17 | Found: "GS003" |
| CRITICAL | GS001 | gs003_debug_prints.py | 58 | Found: "GS003" |
| CRITICAL | GS001 | gs004_dangerous_subprocess.py | 21 | Found: "GS004" |
| CRITICAL | GS001 | gs004_dangerous_subprocess.py | 86 | Found: "GS004" |
| CRITICAL | GS001 | gs005_sql_injection.py | 32 | Found: "GS005" |
| CRITICAL | GS001 | gs007_idor.py | 25 | Found: "GS007" |
| CRITICAL | GS001 | gs007_idor.py | 153 | Found: "GS007" |
| CRITICAL | GS001 | gs008_dead_code.py | 23 | Found: "GS008" |
| CRITICAL | GS001 | gs008_dead_code.py | 73 | Found: "GS008" |
| CRITICAL | GS001 | gs009_supply_chain.py | 24 | Found: "GS009" |
| CRITICAL | GS001 | gs010_ssh_hardening.py | 24 | Found: "GS010" |
| CRITICAL | GS001 | gs010_ssh_hardening.py | 30 | Found: "GS010" |
| CRITICAL | GS001 | gs011_jwt_vulnerabilities.py | 22 | Found: "GS011" |
| CRITICAL | GS001 | gs011_jwt_vulnerabilities.py | 56 | Found: "GS011" |
| CRITICAL | GS001 | gs012_mass_assignment.py | 22 | Found: "GS012" |
| CRITICAL | GS001 | gs012_mass_assignment.py | 82 | Found: "GS012" |
| CRITICAL | GS001 | gs013_graphql_security.py | 23 | Found: "GS013" |
| CRITICAL | GS001 | gs013_graphql_security.py | 89 | Found: "GS013" |
| CRITICAL | GS001 | gs014_credential_exposure.py | 27 | Found: "GS014" |
| CRITICAL | GS001 | gs014_credential_exposure.py | 113 | Found: "GS014" |
| CRITICAL | GS001 | gs015_entry_points.py | 19 | Found: "GS015" |
| CRITICAL | GS001 | gs015_entry_points.py | 87 | Found: "GS015" |
| CRITICAL | GS001 | gs016_linux_priv_esc.py | 24 | Found: "GS016" |
| CRITICAL | GS001 | gs017_weak_passwords.py | 23 | Found: "GS017" |
| CRITICAL | GS001 | gs017_weak_passwords.py | 109 | Found: "GS017" |
| CRITICAL | GS001 | gs018_payment_abuse.py | 28 | Found: "GS018" |
| CRITICAL | GS001 | gs018_payment_abuse.py | 137 | Found: "GS018" |
| CRITICAL | GS001 | gs019_auth_session.py | 29 | Found: "GS019" |
| CRITICAL | GS001 | gs019_auth_session.py | 173 | Found: "GS019" |
| CRITICAL | GS001 | gs020_llm_sqli.py | 26 | Found: "GS024" |
| CRITICAL | GS001 | gs020_xss_injection.py | 24 | Found: "GS020" |
| CRITICAL | GS001 | gs021_csrf_ssrf.py | 22 | Found: "GS021" |
| CRITICAL | GS001 | gs022_open_redirect.py | 23 | Found: "GS022" |
| CRITICAL | GS001 | gs023_race_conditions.py | 24 | Found: "GS023" |
| CRITICAL | GS001 | gs025_ai_provenance.py | 68 | Found: "GS025" |
| CRITICAL | GS001 | gs025_ai_provenance.py | 125 | Found: "GS025" |
| CRITICAL | GS001 | gs028_invariants.py | 21 | Found: "GS028" |
| CRITICAL | GS001 | multi_lang.py | 21 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 22 | Found: "GS002" |
| CRITICAL | GS001 | multi_lang.py | 25 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 26 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 28 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 31 | Found: "GS002" |
| CRITICAL | GS001 | multi_lang.py | 32 | Found: "GS015" |
| CRITICAL | GS001 | multi_lang.py | 39 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 41 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 44 | Found: "GS017" |
| CRITICAL | GS001 | multi_lang.py | 46 | Found: "GS020" |
| CRITICAL | GS001 | multi_lang.py | 47 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 48 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 51 | Found: "GS018" |
| CRITICAL | GS001 | multi_lang.py | 52 | Found: "GS019" |
| CRITICAL | GS001 | multi_lang.py | 59 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 62 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 64 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 65 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 68 | Found: "GS002" |
| CRITICAL | GS001 | multi_lang.py | 69 | Found: "GS015" |
| CRITICAL | GS001 | multi_lang.py | 76 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 80 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 82 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 83 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 84 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 88 | Found: "GS008" |
| CRITICAL | GS001 | multi_lang.py | 91 | Found: "GS019" |
| CRITICAL | GS001 | registry.py | 225 | Found: "GS024" |
| CRITICAL | GS001 | gsc_external.py | 58 | Found: "GS003" |
| CRITICAL | GS001 | gsc_external.py | 58 | Found: "GS008" |
| CRITICAL | GS001 | gsc_external.py | 58 | Found: "GS015" |
| CRITICAL | GS001 | gsc_external.py | 59 | Found: "GS007" |
| CRITICAL | GS001 | gsc_external.py | 59 | Found: "GS012" |
| CRITICAL | GS001 | gsc_external.py | 59 | Found: "GS013" |
| CRITICAL | GS001 | gsc_external.py | 59 | Found: "GS018" |
| CRITICAL | GS001 | gsc_external.py | 59 | Found: "GS019" |
| CRITICAL | GS001 | gsc_external.py | 59 | Found: "GS023" |
| CRITICAL | GS001 | gsc_external.py | 75 | Found: "GS003" |
| CRITICAL | GS001 | gsc_external.py | 75 | Found: "GS008" |
| CRITICAL | GS001 | gsc_external.py | 75 | Found: "GS015" |
| CRITICAL | GS001 | gsc_external.py | 75 | Found: "GS023" |
| CRITICAL | GS001 | gsc_external.py | 76 | Found: "GS007" |
| CRITICAL | GS001 | gsc_external.py | 76 | Found: "GS012" |
| CRITICAL | GS001 | gsc_external.py | 76 | Found: "GS013" |
| CRITICAL | GS001 | gsc_external.py | 76 | Found: "GS018" |
| CRITICAL | GS001 | gsc_external.py | 76 | Found: "GS019" |
| CRITICAL | GS001 | gsc_external.py | 107 | Found: "GS003" |
| CRITICAL | GS001 | gsc_external.py | 107 | Found: "GS008" |
| CRITICAL | GS001 | gsc_external.py | 107 | Found: "GS015" |
| CRITICAL | GS001 | gsc_external.py | 107 | Found: "GS023" |
| CRITICAL | GS001 | gsc_external.py | 108 | Found: "GS007" |
| CRITICAL | GS001 | gsc_external.py | 108 | Found: "GS012" |
| CRITICAL | GS001 | gsc_external.py | 108 | Found: "GS013" |
| CRITICAL | GS001 | gsc_external.py | 108 | Found: "GS018" |
| CRITICAL | GS001 | gsc_external.py | 108 | Found: "GS019" |
| CRITICAL | GS001 | gsc_external.py | 108 | Found: "GS021" |
| CRITICAL | GS001 | gsc_external.py | 108 | Found: "GS022" |
| CRITICAL | GS001 | gsc_external.py | 454 | Found: "GS001" |
| CRITICAL | GS001 | gsc_external.py | 456 | Found: "GS005" |
| CRITICAL | GS001 | gsc_external.py | 458 | Found: "GS020" |
| CRITICAL | GS001 | gsc_poc_generator.py | 40 | Found: "GS001" |
| CRITICAL | GS001 | gsc_poc_generator.py | 41 | Found: "GS003" |
| CRITICAL | GS001 | gsc_poc_generator.py | 42 | Found: "GS007" |
| CRITICAL | GS001 | gsc_poc_generator.py | 43 | Found: "GS012" |
| CRITICAL | GS001 | gsc_poc_generator.py | 44 | Found: "GS019" |
| CRITICAL | GS001 | gsc_poc_generator.py | 45 | Found: "GS022" |
| CRITICAL | GS001 | gsc_poc_generator.py | 46 | Found: "GS024" |
| CRITICAL | GS001 | gsc_scan_modes.py | 29 | Found: "GS002" |
| CRITICAL | GS001 | gsc_scan_modes.py | 29 | Found: "GS003" |
| CRITICAL | GS001 | gsc_scan_modes.py | 29 | Found: "GS007" |
| CRITICAL | GS001 | gsc_scan_modes.py | 29 | Found: "GS008" |
| CRITICAL | GS001 | gsc_scan_modes.py | 29 | Found: "GS012" |
| CRITICAL | GS001 | gsc_scan_modes.py | 29 | Found: "GS013" |
| CRITICAL | GS001 | gsc_scan_modes.py | 30 | Found: "GS015" |
| CRITICAL | GS001 | gsc_scan_modes.py | 30 | Found: "GS018" |
| CRITICAL | GS001 | gsc_scan_modes.py | 30 | Found: "GS019" |
| CRITICAL | GS001 | gsc_scan_modes.py | 30 | Found: "GS022" |
| CRITICAL | GS001 | gsc_scan_modes.py | 30 | Found: "GS023" |
| CRITICAL | GS001 | gsc_scan_modes.py | 30 | Found: "GS025" |
| CRITICAL | GS001 | gsc_scan_modes.py | 45 | Found: "GS003" |
| CRITICAL | GS001 | gsc_scan_modes.py | 45 | Found: "GS008" |
| CRITICAL | GS001 | gsc_scan_modes.py | 45 | Found: "GS015" |
| CRITICAL | GS001 | gsc_selfhealing.py | 63 | Found: "GS001" |
| CRITICAL | GS001 | gsc_selfhealing.py | 63 | Found: "GS004" |
| CRITICAL | GS001 | gsc_selfhealing.py | 63 | Found: "GS005" |
| CRITICAL | GS001 | gsc_selfhealing.py | 63 | Found: "GS017" |
| CRITICAL | GS001 | gsc_selfhealing.py | 63 | Found: "GS020" |
| CRITICAL | GS001 | gsc_selfhealing.py | 63 | Found: "GS021" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 16 | Found: SECRET: "change-me-in-sealed-secret" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 14 | Found: REDIS_URL: "redis://redis:6379/0" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 25 | Found: DATABASE_URL: "postgresql://gsc_app:CHANGE_ME@postgre |
| CRITICAL | ? | systemd.json | 78 | Match:     "detail": "AmbientCapabilities=CAP_ALL grants all |
| CRITICAL | GS005 | corpus_gs005_javascript.js | 10 | Line 10: await sequelize.query("SELECT * FROM logs WHERE use |
| CRITICAL | GS005 | corpus_gs005_javascript.js | 14 | Line 14: await knex.raw("SELECT * FROM sessions WHERE token  |
| CRITICAL | GS005 | corpus_gs005_javascript.js | 17 | Line 17: pool.query("SELECT * FROM users WHERE email = '" +  |
| CRITICAL | GS005 | corpus_gs005_javascript.js | 20 | Line 20: db.collection.find({ $where: `this.name == '${req.q |
| CRITICAL | GS005 | corpus_gs005_php.php | 6 | Line 6: mysqli_query($conn, "SELECT * FROM users WHERE id =  |
| CRITICAL | GS005 | corpus_gs005_php.php | 7 | Line 7: mysqli_query($conn, "SELECT * FROM orders WHERE stat |
| CRITICAL | GS005 | corpus_gs005_php.php | 10 | Line 10: $pdo->query("SELECT * FROM orders WHERE status = '" |
| CRITICAL | GS005 | corpus_gs005_php.php | 11 | Line 11: $pdo->query("SELECT * FROM users WHERE email = '{$e |
| CRITICAL | GS005 | corpus_gs005_php.php | 14 | Line 14: pg_query($conn, "SELECT * FROM data WHERE key = '"  |
| CRITICAL | GS005 | corpus_gs005_php.php | 17 | Line 17: DB::table('users')->whereRaw("email = '{$email}'")- |
| CRITICAL | GS005 | corpus_gs005_php.php | 18 | Line 18: DB::select("SELECT * FROM logs WHERE user_id = {$us |
| CRITICAL | GS005 | corpus_gs005_python.py | 8 | Line 8: cursor.execute(f"SELECT * FROM users WHERE id = {use |
| CRITICAL | GS005 | corpus_gs005_python.py | 9 | Line 9: cursor.execute("SELECT * FROM users WHERE name = '%s |
| CRITICAL | GS005 | corpus_gs005_python.py | 10 | Line 10: cursor.execute("SELECT * FROM products WHERE catego |
| CRITICAL | GS005 | corpus_gs005_python.py | 11 | Line 11: cursor.execute("SELECT * FROM orders WHERE id = " + |
| CRITICAL | GS005 | corpus_gs005_python.py | 12 | Line 12: cursor.executemany(f"INSERT INTO log VALUES ({data} |
| CRITICAL | GS005 | corpus_gs005_python.py | 15 | Line 15: cursor.execute(f"SELECT name FROM users WHERE id =  |
| CRITICAL | GS005 | corpus_gs005_python.py | 16 | Line 16: cursor.execute("SELECT * FROM products WHERE cat =  |
| CRITICAL | GS005 | corpus_gs005_python.py | 16 | Line 16: cursor.execute("SELECT * FROM products WHERE cat =  |
| CRITICAL | GS005 | corpus_gs005_python.py | 16 | Line 16: cursor.execute("SELECT * FROM products WHERE cat =  |
| CRITICAL | GS005 | corpus_gs005_python.py | 19 | Line 19: cursor.execute(f"SELECT * FROM users WHERE name = ' |
| CRITICAL | GS005 | corpus_gs005_python.py | 19 | Line 19: cursor.execute(f"SELECT * FROM users WHERE name = ' |
| CRITICAL | GS005 | corpus_gs005_python.py | 20 | Line 20: cursor.execute(f"SELECT * FROM items WHERE id = {it |
| CRITICAL | GS005 | corpus_gs005_python.py | 20 | Line 20: cursor.execute(f"SELECT * FROM items WHERE id = {it |
| CRITICAL | GS005 | corpus_gs005_python.py | 23 | Line 23: cursor.execute(f"SELECT * FROM users WHERE id = {ui |
| CRITICAL | GS005 | corpus_gs005_python.py | 24 | Line 24: cursor.execute("SELECT * FROM data WHERE key = '" + |
| CRITICAL | GS005 | corpus_gs005_python.py | 24 | Line 24: cursor.execute("SELECT * FROM data WHERE key = '" + |
| CRITICAL | GS005 | corpus_gs005_python.py | 24 | Line 24: cursor.execute("SELECT * FROM data WHERE key = '" + |
| CRITICAL | GS005 | corpus_gs005_python.py | 25 | Line 25: cursor.execute("SELECT * FROM dbo.users WHERE name  |
| CRITICAL | GS005 | corpus_gs005_python.py | 25 | Line 25: cursor.execute("SELECT * FROM dbo.users WHERE name  |
| CRITICAL | GS005 | corpus_gs005_python.py | 28 | Line 28: cursor.execute(f"SELECT * FROM users WHERE id = {ui |
| CRITICAL | GS005 | corpus_gs005_python.py | 31 | Line 31: User.objects.raw(f"SELECT * FROM users WHERE name = |
| CRITICAL | GS005 | corpus_gs005_python.py | 32 | Line 32: User.objects.raw("SELECT * FROM users WHERE id = %s |
| CRITICAL | GS005 | corpus_gs005_python.py | 33 | Line 33: User.objects.extra(where=f"name = '{name}' AND acti |
| CRITICAL | GS005 | corpus_gs005_python.py | 34 | Line 34: User.objects.annotate(full_name=RawSQL(f"first_name |
| CRITICAL | GS005 | corpus_gs005_python.py | 34 | Line 34: User.objects.annotate(full_name=RawSQL(f"first_name |
| CRITICAL | GS005 | corpus_gs005_python.py | 37 | Line 37: session.execute(text(f"SELECT * FROM users WHERE id |
| CRITICAL | GS005 | corpus_gs005_python.py | 38 | Line 38: session.execute(text("SELECT * FROM users WHERE ema |
| CRITICAL | GS005 | corpus_gs005_python.py | 39 | Line 39: engine.execute(text(f"DELETE FROM sessions WHERE to |
| CRITICAL | GS005 | corpus_gs005_python.py | 39 | Line 39: engine.execute(text(f"DELETE FROM sessions WHERE to |
| CRITICAL | GS005 | corpus_gs005_python.py | 43 | Line 43: cursor.execute(f"SELECT * FROM audit WHERE user = ' |
| CRITICAL | GS005 | corpus_gs005_python.py | 43 | Line 43: cursor.execute(f"SELECT * FROM audit WHERE user = ' |
| CRITICAL | GS005 | corpus_gs005_python.py | 50 | Line 50: table.query(KeyConditionExpression=f"pk = '{partiti |
| CRITICAL | GS005 | corpus_gs005_ruby.rb | 5 | Line 5: User.where("name = '#{params[:name]}' AND active = 1 |
| CRITICAL | GS005 | corpus_gs005_ruby.rb | 6 | Line 6: User.find_by_sql("SELECT * FROM users WHERE email =  |
| CRITICAL | GS005 | corpus_gs005_ruby.rb | 7 | Line 7: ActiveRecord::Base.connection.execute("SELECT * FROM |
| CRITICAL | GS005 | corpus_gs005_ruby.rb | 8 | Line 8: User.select_all("SELECT * FROM products WHERE sku =  |
| CRITICAL | GS005 | gsc_db_backend.py | 60 | Line 60: self.conn.execute(f"SET app.tenant_id = {int(tenant |
| CRITICAL | GS005 | gs020_llm_sqli.py | 126 | Line 126: - f-string with user-controlled input: cursor.exec |
| CRITICAL | GS005 | gs020_llm_sqli.py | 230 | Line 230: cursor.execute(f"SELECT * FROM users WHERE id = {u |
| CRITICAL | GS005 | gsc_metrics.py | 31 | Line 31: total = conn.execute(f"SELECT COUNT(*) FROM finding |
| CRITICAL | GS005 | gsc_metrics.py | 34 | Line 34: tp = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 40 | Line 40: fp = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 46 | Line 46: open_f = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 52 | Line 52: reval_total = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 74 | Line 74: det_rows = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 101 | Line 101: worst = conn.execute(f""" |
| CRITICAL | GS016 | gs016_linux_priv_esc.py | 35 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS024 | corpus_gs005_python.py | 8 | LLM confidence: 100%. The code uses f-strings, string format |
| CRITICAL | GS024 | corpus_gs005_python.py | 9 | LLM confidence: 100%. The code uses f-strings, % formatting, |
| CRITICAL | GS024 | corpus_gs005_python.py | 15 | LLM confidence: 100%. All lines use string interpolation or  |
| CRITICAL | GS024 | gs020_llm_sqli.py | 230 | LLM confidence: 100%. The code uses an f-string to interpola |
| CRITICAL | GS024 | gsc_metrics.py | 31 | LLM confidence: 95%. The 'project' variable is interpolated  |
| CRITICAL | GS024 | gsc_metrics.py | 34 | LLM confidence: 95%. The 'project' variable is interpolated  |
| HIGH | ? | api.ts | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | api.ts | 24 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | api.ts | 26 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | api.ts | 27 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | page.tsx | 23 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | ? | user_auth.py | 60 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | sso.py | 36 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | gsc_issue.py | 74 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | fastapi_support.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | gs012_mass_assignment.py | 44 | Hacking APIs Ch.11 |
| HIGH | ? | gsc_vuln_spider.py | 47 | Redteam Kit |
| HIGH | ? | _cron_collect.py | 140 |  |
| HIGH | ? | gs011_jwt_vulnerabilities.py | 41 |  |
| HIGH | ? | gsc_collect_light.py | 211 |  |
| HIGH | ? | gsc_vuln_spider.py | 39 |  |
| HIGH | ? | gsc.py | 299 |  |
| HIGH | ? | gs005_sql_injection.py | 135 |  |
| HIGH | ? | _cron_collect.py | 47 |  |
| HIGH | ? | _cron_nvd.py | 45 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 27 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 40 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 41 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 95 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 129 |  |
| HIGH | ? | gs014_credential_exposure.py | 29 |  |
| HIGH | ? | gs014_credential_exposure.py | 91 |  |
| HIGH | ? | gs014_credential_exposure.py | 92 |  |
| HIGH | ? | gs014_credential_exposure.py | 93 |  |
| HIGH | ? | gs014_credential_exposure.py | 94 |  |
| HIGH | ? | gs014_credential_exposure.py | 98 |  |
| HIGH | ? | gs014_credential_exposure.py | 99 |  |
| HIGH | ? | gsc_collect_light.py | 74 |  |
| HIGH | ? | user_auth.py | 60 |  |
| HIGH | ? | sso.py | 36 |  |
| HIGH | ? | gsc_issue.py | 74 |  |
| HIGH | ? | gsc_collect_light.py | 113 |  |
| HIGH | ? | gsc_collect_light.py | 126 |  |
| HIGH | ? | _cron_collect.py | 141 |  |
| HIGH | ? | gsc_collect_light.py | 212 |  |
| HIGH | ? | gsc_external.py | 174 | Match:     "standard default", "localhost", "loopback", "127 |
| HIGH | ? | gsc_external.py | 1307 | Match: RULES: localhost/127.0.0.1 defaults → false-positive. |
| HIGH | ? | bughunter.json | 45 | Match:     "fix": "Validate URL against allowlist. Block int |
| HIGH | ? | terraform.json | 3 | Match:   {"echelon": 2, "category": "HIGH", "title": "Terraf |
| HIGH | ? | docker.json | 6 | Match:   {"echelon": 2, "category": "MEDIUM", "title": "Dock |
| HIGH | ? | Dockerfile | 18 | Match: CMD ["uvicorn", "cloud.api:app", "--host", "0.0.0.0", |
| HIGH | ? | docker-compose.yml | 35 | Match:     command: uvicorn cloud.api:app --host 0.0.0.0 --p |
| HIGH | ? | sso.yaml | 14 | Match:     http_address = "0.0.0.0:4180" |
| HIGH | ? | gsc.py | 1887 | Match:     api.add_argument('--host', default='127.0.0.1', h |
| HIGH | ? | gsc_proofoffix.py | 31 | Match:     "HTTP_PROXY": "http://127.0.0.1:9", |
| HIGH | ? | gsc_proofoffix.py | 32 | Match:     "HTTPS_PROXY": "http://127.0.0.1:9", |
| HIGH | ? | gsc_proofoffix.py | 33 | Match:     "http_proxy": "http://127.0.0.1:9", |
| HIGH | ? | gsc_proofoffix.py | 34 | Match:     "https_proxy": "http://127.0.0.1:9", |
| HIGH | ? | gsc_api.py | 413 | Match:     p.add_argument("--host", default="127.0.0.1") |
| HIGH | ? | gs010_ssh_hardening.py | 85 | Match:                         references=["SSH Hardening &  |
| HIGH | ? | user_auth.py | 60 | Match:     user = requests.get(f"{GH_API}/user", |
| HIGH | ? | sso.py | 36 | Match:     resp = requests.get(f"{issuer_url.rstrip('/')}/.w |
| HIGH | ? | gsc_issue.py | 74 | Match:     r = requests.post(f"{jira_url}/rest/api/2/issue", |
| HIGH | ? | framework_aware.py | 21 | Match:     "eval() usage": { |
| HIGH | ? | framework_aware.py | 167 | Match:         {"title": "eval() usage", "category": "HIGH", |
| HIGH | ? | gsc.py | 703 | Match:             "Req 6": ["SQL injection", "eval()", "pic |
| HIGH | ? | gsc.py | 712 | Match:             "CC6.8": ["eval()", "pickle.load"], |
| HIGH | ? | gsc.py | 1262 | Match:         (2, "HIGH", "eval() or exec() usage", "regex" |
| HIGH | ? | gs004_dangerous_subprocess.py | 72 | Match:         "eval() with dynamic input — code injection", |
| HIGH | ? | gs004_dangerous_subprocess.py | 73 | Match:         "Never use eval() on user input. Use ast.lite |
| HIGH | ? | gs004_dangerous_subprocess.py | 78 | Match:         "exec() on variable — code injection risk", |
| HIGH | ? | gs004_dangerous_subprocess.py | 79 | Match:         "Avoid exec(); use explicit function calls or |
| HIGH | ? | gs020_xss_injection.py | 38 | Match:     (r'eval\s*\(\s*[\"\'`]', "DOM XSS: eval() with st |
| HIGH | ? | gsc_vuln_spider.py | 31 | Match:         ('"eval(" "request" language:python stars:<20 |
| HIGH | ? | gsc_pdf.py | 15 | Match:     os.system(f"python3 {os.path.dirname(__file__)}/g |
| HIGH | ? | gs004_dangerous_subprocess.py | 48 | Match:         "os.system() with .format() — command injecti |
| HIGH | ? | systemd.json | 23 | Match:     "title": "Systemd: User=root or absent → runs as  |
| HIGH | ? | .mcp.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 54 | Line 54: "os.popen() — deprecated, uses shell", |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 60 | Line 60: "commands.getoutput() — deprecated shell wrapper", |
| HIGH | GS004 | gsc_pdf.py | 15 | Line 15: os.system(f"python3 {os.path.dirname(__file__)}/gsc |
| HIGH | GS005 | corpus_gs005_javascript.js | 20 | Line 20: db.collection.find({ $where: `this.name == '${req.q |
| HIGH | GS005 | corpus_gs005_javascript.js | 21 | Line 21: db.collection.find({ name: { $regex: req.params.sea |
| HIGH | GS005 | corpus_gs005_python.py | 46 | Line 46: pd.read_sql(f"SELECT * FROM sales WHERE region = '{ |
| HIGH | GS005 | corpus_gs005_python.py | 49 | Line 49: table.scan(FilterExpression=f"username = '{user}'") |
| HIGH | GS007 | api.py | 65 | Line 65: @app.get("/api/v2/scans/{scan_id}") |
| HIGH | GS007 | user_auth.py | 123 | Line 123: SELECT tenant_id FROM memberships WHERE user_id =  |
| HIGH | GS007 | corpus_gs005_javascript.js | 10 | Line 10: await sequelize.query("SELECT * FROM logs WHERE use |
| HIGH | GS007 | corpus_gs005_javascript.js | 13 | Line 13: await knex.raw(`SELECT * FROM logs WHERE user_id =  |
| HIGH | GS007 | corpus_gs005_php.php | 18 | Line 18: DB::select("SELECT * FROM logs WHERE user_id = {$us |
| HIGH | GS007 | batch_and_override.py | 31 | Line 31: Order.objects.bulk_create(  # GS007: batch operatio |
| HIGH | GS007 | batch_and_override.py | 39 | Line 39: HTTP_METHOD_OVERRIDE = "X-HTTP-Method-Override"  #  |
| HIGH | GS007 | batch_and_override.py | 39 | Line 39: HTTP_METHOD_OVERRIDE = "X-HTTP-Method-Override"  #  |
| HIGH | GS007 | batch_and_override.py | 44 | Line 44: _method = request.POST.get("_method", request.metho |
| HIGH | GS007 | batch_and_override.py | 44 | Line 44: _method = request.POST.get("_method", request.metho |
| HIGH | GS007 | batch_and_override.py | 45 | Line 45: if _method == "DELETE": |
| HIGH | GS007 | express_files.js | 17 | Line 17: Ticket.findById(req.params.id).then(ticket => {  // |
| HIGH | GS007 | express_files.js | 12 | Line 12: res.sendFile(`/uploads/${req.params.fileId}`);  //  |
| HIGH | GS007 | fastapi_support.py | 35 | Line 35: @app.get("/attachments/{file_id}")  # GS007: file e |
| HIGH | GS007 | laravel_tickets.php | 29 | Line 29: $ticket->add_subscriber($request->user());  // GS00 |
| HIGH | GS007 | schema.sql | 12 | Line 12: SELECT * FROM tickets WHERE user_id = $1;  -- GS007 |
| HIGH | GS007 | gs007_idor.py | 101 | Line 101: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP- |
| HIGH | GS007 | gs007_idor.py | 101 | Line 101: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP- |
| HIGH | GS007 | gs007_idor.py | 101 | Line 101: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP- |
| HIGH | GS012 | gs012_mass_assignment.py | 44 | Unpacking request body directly into model enables field inj |
| HIGH | GS014 | docker-compose.yml | 37 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | docker-compose.yml | 62 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | gsc_vuln_spider.py | 47 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | 00-namespace-config.yaml | 25 | Database URL contains password in plaintext. Use environment |
| HIGH | ? | rust.json | 7 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | ? | gsc_metrics.py | 31 |
| C | ? | corpus_gs005_python.py | 8 |
| C | ? | corpus_gs005_python.py | 12 |
| C | ? | corpus_gs005_python.py | 15 |
| C | ? | corpus_gs005_python.py | 19 |
| C | ? | corpus_gs005_python.py | 20 |
| C | ? | corpus_gs005_python.py | 23 |
| C | ? | corpus_gs005_python.py | 28 |
| C | ? | corpus_gs005_python.py | 31 |
| C | ? | corpus_gs005_python.py | 37 |
| C | ? | corpus_gs005_python.py | 39 |
| C | ? | corpus_gs005_python.py | 43 |
| C | ? | corpus_gs005_python.py | 46 |
| C | ? | gs018_payment_abuse.py | 215 |
| C | ? | gs020_llm_sqli.py | 126 |
| C | ? | gs020_llm_sqli.py | 230 |
| M | ? | pre-commit | 22 |
| M | ? | gsc_nlpolicy.py | 130 |
| M | ? | gsc_doctor.py | 16 |
| M | ? | gsc_doctor.py | 33 |
| M | ? | framework_aware.py | 31 |
| M | ? | framework_aware.py | 165 |
| M | ? | gsc.py | 60 |
| M | ? | gsc.py | 1261 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| L | ? | gsc_external.py | 144 |
| L | ? | gs001_hardcoded_secret.py | 89 |
| L | ? | gs025_ai_provenance.py | 28 |
| H | ? | api.ts | 19 |
| H | ? | api.ts | 24 |
| H | ? | api.ts | 26 |
| H | ? | api.ts | 27 |
| H | ? | page.tsx | 23 |
| C | ? | corpus_gs005_python.py | 11 |
| C | ? | corpus_gs005_python.py | 16 |
| C | ? | corpus_gs005_python.py | 24 |
| C | ? | corpus_gs005_python.py | 25 |
| H | ? | user_auth.py | 60 |
| H | ? | sso.py | 36 |
| H | ? | gsc_issue.py | 74 |
| H | ? | fastapi_support.py | 38 |
| H | ? | gs012_mass_assignment.py | 44 |
| H | ? | gsc_vuln_spider.py | 47 |
| M | ? | _cron_collect.py | 42 |
| M | ? | _cron_nvd.py | 40 |
| M | ? | gsc_collect_light.py | 69 |
| M | ? | gsc.py | 703 |
| M | ? | gsc.py | 712 |
| M | ? | gsc_vuln_spider.py | 191 |
| C | ? | gsc_metrics.py | 31 |
| C | ? | corpus_gs005_python.py | 8 |
| C | ? | corpus_gs005_python.py | 12 |
| C | ? | corpus_gs005_python.py | 15 |
| C | ? | corpus_gs005_python.py | 19 |
| C | ? | corpus_gs005_python.py | 20 |
| C | ? | corpus_gs005_python.py | 23 |
| C | ? | corpus_gs005_python.py | 28 |
| C | ? | corpus_gs005_python.py | 31 |
| C | ? | corpus_gs005_python.py | 37 |
| C | ? | corpus_gs005_python.py | 39 |
| C | ? | corpus_gs005_python.py | 43 |
| C | ? | corpus_gs005_python.py | 46 |
| C | ? | gs020_llm_sqli.py | 126 |
| C | ? | gs020_llm_sqli.py | 230 |
| H | ? | _cron_collect.py | 140 |
| H | ? | gs011_jwt_vulnerabilities.py | 41 |
| H | ? | gsc_collect_light.py | 211 |
| H | ? | gsc_vuln_spider.py | 39 |
| H | ? | gsc.py | 299 |
| H | ? | gs005_sql_injection.py | 135 |
| H | ? | _cron_collect.py | 47 |
| H | ? | _cron_nvd.py | 45 |
| H | ? | gs016_linux_priv_esc.py | 27 |
| H | ? | gs016_linux_priv_esc.py | 40 |
| H | ? | gs016_linux_priv_esc.py | 41 |
| H | ? | gs016_linux_priv_esc.py | 95 |
| H | ? | gs016_linux_priv_esc.py | 129 |
| H | ? | gs014_credential_exposure.py | 29 |
| H | ? | gs014_credential_exposure.py | 91 |
| H | ? | gs014_credential_exposure.py | 92 |
| H | ? | gs014_credential_exposure.py | 93 |
| H | ? | gs014_credential_exposure.py | 94 |
| H | ? | gs014_credential_exposure.py | 98 |
| H | ? | gs014_credential_exposure.py | 99 |
| H | ? | gsc_collect_light.py | 74 |
| H | ? | user_auth.py | 60 |
| H | ? | sso.py | 36 |
| H | ? | gsc_issue.py | 74 |
| H | ? | gsc_collect_light.py | 113 |
| H | ? | gsc_collect_light.py | 126 |
| M | ? | corpus_gs005_python.py | 39 |
| M | ? | _cron_collect.py | 33 |
| M | ? | _cron_nvd.py | 31 |
| M | ? | multi_lang.py | 45 |
| M | ? | multi_lang.py | 46 |
| M | ? | gs020_xss_injection.py | 33 |
| M | ? | gs020_xss_injection.py | 36 |
| M | ? | gs020_xss_injection.py | 50 |
| M | ? | gsc_collect_light.py | 60 |
| C | ? | _cron_collect.py | 141 |
| C | ? | gsc_pdf.py | 15 |
| C | ? | gsc.py | 1264 |
| C | ? | gs004_dangerous_subprocess.py | 38 |
| C | ? | gs004_dangerous_subprocess.py | 43 |
| C | ? | gs004_dangerous_subprocess.py | 48 |
| C | ? | gs004_dangerous_subprocess.py | 115 |
| C | ? | gsc_collect_light.py | 212 |
| C | ? | gsc_vuln_spider.py | 29 |
| C | ? | gsc_vuln_spider.py | 187 |
| C | ? | _cron_collect.py | 139 |
| C | ? | gsc_collect_light.py | 210 |
| C | ? | _cron_collect.py | 140 |
| C | ? | gsc_collect_light.py | 211 |
| C | ? | gsc_vuln_spider.py | 39 |
| H | ? | _cron_collect.py | 141 |
| H | ? | gsc_collect_light.py | 212 |
| M | ? | corpus_gs005_python.py | 24 |
| M | ? | corpus_gs005_python.py | 39 |
| C | GS001 | _cron_collect.py | 17 |
| C | GS001 | _cron_collect.py | 20 |
| C | GS001 | _cron_collect.py | 23 |
| C | GS001 | _cron_collect.py | 29 |
| C | GS001 | _cron_collect.py | 38 |
| C | GS001 | _cron_collect.py | 46 |
| C | GS001 | _cron_collect.py | 49 |
| C | GS001 | _cron_collect.py | 139 |
| C | GS001 | _cron_collect.py | 140 |
| C | GS001 | _cron_collect.py | 141 |
| C | GS001 | _cron_collect.py | 142 |
| C | GS001 | _cron_collect.py | 143 |
| C | GS001 | _cron_nvd.py | 15 |
| C | GS001 | _cron_nvd.py | 18 |
| C | GS001 | _cron_nvd.py | 21 |
| C | GS001 | _cron_nvd.py | 27 |
| C | GS001 | _cron_nvd.py | 36 |
| C | GS001 | _cron_nvd.py | 44 |
| C | GS001 | _cron_nvd.py | 47 |
| C | GS001 | click.json | 9 |
| C | GS001 | flask-jwt-auth.json | 7 |
| C | GS001 | flask-jwt-auth.json | 8 |
| C | GS001 | github_auth.py | 40 |
| C | GS001 | manifest.json | 249 |
| C | GS001 | manifest.json | 250 |
| C | GS001 | manifest.json | 289 |
| C | GS001 | manifest.json | 290 |
| C | GS001 | manifest.json | 339 |
| C | GS001 | manifest.json | 340 |
| C | GS001 | manifest.json | 344 |
| C | GS001 | manifest.json | 345 |
| C | GS001 | gsc_blocking.py | 55 |
| C | GS001 | gsc_chain_composer.py | 26 |
| C | GS001 | gsc_chain_composer.py | 26 |
| C | GS001 | gsc_chain_composer.py | 26 |
| C | GS001 | gsc_chain_composer.py | 27 |
| C | GS001 | gsc_chain_composer.py | 27 |
| C | GS001 | gsc_chain_composer.py | 28 |
| C | GS001 | gsc_chain_composer.py | 29 |
| C | GS001 | gsc_chain_composer.py | 29 |
| C | GS001 | gsc_chain_composer.py | 30 |
| C | GS001 | gsc_chain_composer.py | 30 |
| C | GS001 | gsc_chain_composer.py | 31 |
| C | GS001 | gsc_chain_composer.py | 32 |
| C | GS001 | gsc_chain_composer.py | 38 |
| C | GS001 | gsc_chain_composer.py | 38 |
| C | GS001 | gsc_collect_light.py | 44 |
| C | GS001 | gsc_collect_light.py | 47 |
| C | GS001 | gsc_collect_light.py | 50 |
| C | GS001 | gsc_collect_light.py | 56 |
| C | GS001 | gsc_collect_light.py | 65 |
| C | GS001 | gsc_collect_light.py | 73 |
| C | GS001 | gsc_collect_light.py | 76 |
| C | GS001 | gsc_collect_light.py | 210 |
| C | GS001 | gsc_collect_light.py | 211 |
| C | GS001 | gsc_collect_light.py | 212 |
| C | GS001 | gsc_collect_light.py | 213 |
| C | GS001 | gsc_collect_light.py | 214 |
| C | GS001 | gs001_hardcoded_secret.py | 20 |
| C | GS001 | gs001_hardcoded_secret.py | 98 |
| C | GS001 | gs002_world_readable.py | 18 |
| C | GS001 | gs002_world_readable.py | 45 |
| C | GS001 | gs003_debug_prints.py | 17 |
| C | GS001 | gs003_debug_prints.py | 58 |
| C | GS001 | gs004_dangerous_subprocess.py | 21 |
| C | GS001 | gs004_dangerous_subprocess.py | 86 |
| C | GS001 | gs005_sql_injection.py | 32 |
| C | GS001 | gs007_idor.py | 25 |
| C | GS001 | gs007_idor.py | 153 |
| C | GS001 | gs008_dead_code.py | 23 |
| C | GS001 | gs008_dead_code.py | 73 |
| C | GS001 | gs009_supply_chain.py | 24 |
| C | GS001 | gs010_ssh_hardening.py | 24 |
| C | GS001 | gs010_ssh_hardening.py | 30 |
| C | GS001 | gs011_jwt_vulnerabilities.py | 22 |
| C | GS001 | gs011_jwt_vulnerabilities.py | 56 |
| C | GS001 | gs012_mass_assignment.py | 22 |
| C | GS001 | gs012_mass_assignment.py | 82 |
| C | GS001 | gs013_graphql_security.py | 23 |
| C | GS001 | gs013_graphql_security.py | 89 |
| C | GS001 | gs014_credential_exposure.py | 27 |
| C | GS001 | gs014_credential_exposure.py | 113 |
| C | GS001 | gs015_entry_points.py | 19 |
| C | GS001 | gs015_entry_points.py | 87 |
| C | GS001 | gs016_linux_priv_esc.py | 24 |
| C | GS001 | gs017_weak_passwords.py | 23 |
| C | GS001 | gs017_weak_passwords.py | 109 |
| C | GS001 | gs018_payment_abuse.py | 28 |
| C | GS001 | gs018_payment_abuse.py | 137 |
| C | GS001 | gs019_auth_session.py | 29 |
| C | GS001 | gs019_auth_session.py | 173 |
| C | GS001 | gs020_llm_sqli.py | 26 |
| C | GS001 | gs020_xss_injection.py | 24 |
| C | GS001 | gs021_csrf_ssrf.py | 22 |
| C | GS001 | gs022_open_redirect.py | 23 |
| C | GS001 | gs023_race_conditions.py | 24 |
| C | GS001 | gs025_ai_provenance.py | 68 |
| C | GS001 | gs025_ai_provenance.py | 125 |
| C | GS001 | gs028_invariants.py | 21 |
| C | GS001 | multi_lang.py | 21 |
| C | GS001 | multi_lang.py | 22 |
| C | GS001 | multi_lang.py | 25 |
| C | GS001 | multi_lang.py | 26 |
| C | GS001 | multi_lang.py | 28 |
| C | GS001 | multi_lang.py | 31 |
| C | GS001 | multi_lang.py | 32 |
| C | GS001 | multi_lang.py | 39 |
| C | GS001 | multi_lang.py | 41 |
| C | GS001 | multi_lang.py | 44 |
| C | GS001 | multi_lang.py | 46 |
| C | GS001 | multi_lang.py | 47 |
| C | GS001 | multi_lang.py | 48 |
| C | GS001 | multi_lang.py | 51 |
| C | GS001 | multi_lang.py | 52 |
| C | GS001 | multi_lang.py | 59 |
| C | GS001 | multi_lang.py | 62 |
| C | GS001 | multi_lang.py | 64 |
| C | GS001 | multi_lang.py | 65 |
| C | GS001 | multi_lang.py | 68 |
| C | GS001 | multi_lang.py | 69 |
| C | GS001 | multi_lang.py | 76 |
| C | GS001 | multi_lang.py | 80 |
| C | GS001 | multi_lang.py | 82 |
| C | GS001 | multi_lang.py | 83 |
| C | GS001 | multi_lang.py | 84 |
| C | GS001 | multi_lang.py | 88 |
| C | GS001 | multi_lang.py | 91 |
| C | GS001 | registry.py | 225 |
| C | GS001 | gsc_external.py | 58 |
| C | GS001 | gsc_external.py | 58 |
| C | GS001 | gsc_external.py | 58 |
| C | GS001 | gsc_external.py | 59 |
| C | GS001 | gsc_external.py | 59 |
| C | GS001 | gsc_external.py | 59 |
| C | GS001 | gsc_external.py | 59 |
| C | GS001 | gsc_external.py | 59 |
| C | GS001 | gsc_external.py | 59 |
| C | GS001 | gsc_external.py | 75 |
| C | GS001 | gsc_external.py | 75 |
| C | GS001 | gsc_external.py | 75 |
| C | GS001 | gsc_external.py | 75 |
| C | GS001 | gsc_external.py | 76 |
| C | GS001 | gsc_external.py | 76 |
| C | GS001 | gsc_external.py | 76 |
| C | GS001 | gsc_external.py | 76 |
| C | GS001 | gsc_external.py | 76 |
| C | GS001 | gsc_external.py | 107 |
| C | GS001 | gsc_external.py | 107 |
| C | GS001 | gsc_external.py | 107 |
| C | GS001 | gsc_external.py | 107 |
| C | GS001 | gsc_external.py | 108 |
| C | GS001 | gsc_external.py | 108 |
| C | GS001 | gsc_external.py | 108 |
| C | GS001 | gsc_external.py | 108 |
| C | GS001 | gsc_external.py | 108 |
| C | GS001 | gsc_external.py | 108 |
| C | GS001 | gsc_external.py | 108 |
| C | GS001 | gsc_external.py | 454 |
| C | GS001 | gsc_external.py | 456 |
| C | GS001 | gsc_external.py | 458 |
| C | GS001 | gsc_poc_generator.py | 40 |
| C | GS001 | gsc_poc_generator.py | 41 |
| C | GS001 | gsc_poc_generator.py | 42 |
| C | GS001 | gsc_poc_generator.py | 43 |
| C | GS001 | gsc_poc_generator.py | 44 |
| C | GS001 | gsc_poc_generator.py | 45 |
| C | GS001 | gsc_poc_generator.py | 46 |
| C | GS001 | gsc_scan_modes.py | 29 |
| C | GS001 | gsc_scan_modes.py | 29 |
| C | GS001 | gsc_scan_modes.py | 29 |
| C | GS001 | gsc_scan_modes.py | 29 |
| C | GS001 | gsc_scan_modes.py | 29 |
| C | GS001 | gsc_scan_modes.py | 29 |
| C | GS001 | gsc_scan_modes.py | 30 |
| C | GS001 | gsc_scan_modes.py | 30 |
| C | GS001 | gsc_scan_modes.py | 30 |
| C | GS001 | gsc_scan_modes.py | 30 |
| C | GS001 | gsc_scan_modes.py | 30 |
| C | GS001 | gsc_scan_modes.py | 30 |
| C | GS001 | gsc_scan_modes.py | 45 |
| C | GS001 | gsc_scan_modes.py | 45 |
| C | GS001 | gsc_scan_modes.py | 45 |
| C | GS001 | gsc_selfhealing.py | 63 |
| C | GS001 | gsc_selfhealing.py | 63 |
| C | GS001 | gsc_selfhealing.py | 63 |
| C | GS001 | gsc_selfhealing.py | 63 |
| C | GS001 | gsc_selfhealing.py | 63 |
| C | GS001 | gsc_selfhealing.py | 63 |
| C | GS001 | 00-namespace-config.yaml | 16 |
| C | GS001 | 00-namespace-config.yaml | 14 |
| C | GS001 | 00-namespace-config.yaml | 25 |
| L | GS003 | _cron_collect.py | 68 |
| L | GS003 | _cron_collect.py | 82 |
| L | GS003 | _cron_collect.py | 93 |
| L | GS003 | _cron_collect.py | 99 |
| L | GS003 | _cron_collect.py | 125 |
| L | GS003 | _cron_collect.py | 128 |
| L | GS003 | _cron_collect.py | 145 |
| L | GS003 | _cron_collect.py | 150 |
| L | GS003 | _cron_collect.py | 166 |
| L | GS003 | _cron_collect.py | 169 |
| L | GS003 | _cron_collect.py | 174 |
| L | GS003 | _cron_collect.py | 191 |
| L | GS003 | _cron_collect.py | 196 |
| L | GS003 | _cron_collect.py | 197 |
| L | GS003 | _cron_collect.py | 212 |
| L | GS003 | _cron_collect.py | 232 |
| L | GS003 | _cron_collect.py | 259 |
| L | GS003 | _cron_collect.py | 260 |
| L | GS003 | _cron_collect.py | 261 |
| L | GS003 | _cron_nvd.py | 62 |
| L | GS003 | _cron_nvd.py | 68 |
| L | GS003 | _cron_nvd.py | 96 |
| L | GS003 | _cron_nvd.py | 112 |
| L | GS003 | _cron_nvd.py | 139 |
| L | GS003 | _cron_nvd.py | 141 |
| L | GS003 | runner.py | 37 |
| L | GS003 | runner.py | 42 |
| L | GS003 | runner.py | 91 |
| L | GS003 | runner.py | 113 |
| L | GS003 | manage.py | 41 |
| L | GS003 | manage.py | 42 |
| L | GS003 | django_cross_org.py | 33 |
| L | GS003 | gsc.py | 81 |
| L | GS003 | gsc.py | 86 |
| L | GS003 | gsc.py | 87 |
| L | GS003 | gsc.py | 88 |
| L | GS003 | gsc.py | 95 |
| L | GS003 | gsc.py | 146 |
| L | GS003 | gsc.py | 149 |
| L | GS003 | gsc.py | 170 |
| L | GS003 | gsc.py | 172 |
| L | GS003 | gsc.py | 609 |
| L | GS003 | gsc.py | 724 |
| L | GS003 | gsc.py | 726 |
| L | GS003 | gsc.py | 729 |
| L | GS003 | gsc.py | 737 |
| L | GS003 | gsc.py | 740 |
| L | GS003 | gsc.py | 743 |
| L | GS003 | gsc.py | 745 |
| L | GS003 | gsc.py | 779 |
| L | GS003 | gsc.py | 807 |
| L | GS003 | gsc.py | 891 |
| L | GS003 | gsc.py | 933 |
| L | GS003 | gsc.py | 935 |
| L | GS003 | gsc.py | 936 |
| L | GS003 | gsc.py | 937 |
| L | GS003 | gsc.py | 938 |
| L | GS003 | gsc.py | 939 |
| L | GS003 | gsc.py | 942 |
| L | GS003 | gsc.py | 944 |
| L | GS003 | gsc.py | 1014 |
| L | GS003 | gsc.py | 1015 |
| L | GS003 | gsc.py | 1019 |
| L | GS003 | gsc.py | 1134 |
| L | GS003 | gsc.py | 1205 |
| L | GS003 | gsc.py | 1228 |
| L | GS003 | gsc.py | 1288 |
| L | GS003 | gsc.py | 1299 |
| L | GS003 | gsc.py | 1300 |
| L | GS003 | gsc.py | 1308 |
| L | GS003 | gsc.py | 1316 |
| L | GS003 | gsc.py | 1318 |
| L | GS003 | gsc.py | 1332 |
| L | GS003 | gsc.py | 1344 |
| L | GS003 | gsc.py | 1345 |
| L | GS003 | gsc.py | 1347 |
| L | GS003 | gsc.py | 1360 |
| L | GS003 | gsc.py | 1362 |
| L | GS003 | gsc.py | 1392 |
| L | GS003 | gsc.py | 1393 |
| L | GS003 | gsc.py | 1400 |
| L | GS003 | gsc.py | 1407 |
| L | GS003 | gsc.py | 1417 |
| L | GS003 | gsc.py | 1424 |
| L | GS003 | gsc.py | 1445 |
| L | GS003 | gsc.py | 1455 |
| L | GS003 | gsc.py | 1458 |
| L | GS003 | gsc.py | 1476 |
| L | GS003 | gsc.py | 1482 |
| L | GS003 | gsc.py | 1493 |
| L | GS003 | gsc.py | 1504 |
| L | GS003 | gsc.py | 1508 |
| L | GS003 | gsc.py | 1509 |
| L | GS003 | gsc.py | 1510 |
| L | GS003 | gsc.py | 1511 |
| L | GS003 | gsc.py | 1513 |
| L | GS003 | gsc.py | 1520 |
| L | GS003 | gsc.py | 1527 |
| L | GS003 | gsc.py | 1537 |
| L | GS003 | gsc.py | 1546 |
| L | GS003 | gsc.py | 1548 |
| L | GS003 | gsc.py | 1549 |
| L | GS003 | gsc.py | 1589 |
| L | GS003 | gsc.py | 1617 |
| L | GS003 | gsc.py | 1619 |
| L | GS003 | gsc.py | 1622 |
| L | GS003 | gsc.py | 1650 |
| L | GS003 | gsc.py | 1653 |
| L | GS003 | gsc.py | 1655 |
| L | GS003 | gsc.py | 1656 |
| L | GS003 | gsc.py | 1666 |
| L | GS003 | gsc.py | 1671 |
| L | GS003 | gsc.py | 1674 |
| L | GS003 | gsc.py | 1688 |
| L | GS003 | gsc.py | 1690 |
| L | GS003 | gsc.py | 1691 |
| L | GS003 | gsc.py | 1692 |
| L | GS003 | gsc.py | 1696 |
| L | GS003 | gsc.py | 2046 |
| L | GS003 | gsc.py | 2078 |
| L | GS003 | gsc.py | 2079 |
| L | GS003 | gsc.py | 2121 |
| L | GS003 | gsc.py | 2126 |
| L | GS003 | gsc.py | 2128 |
| L | GS003 | gsc.py | 2134 |
| L | GS003 | gsc.py | 2137 |
| L | GS003 | gsc_api.py | 30 |
| L | GS003 | gsc_api.py | 415 |
| L | GS003 | gsc_api.py | 417 |
| L | GS003 | gsc_api.py | 418 |
| L | GS003 | gsc_archaeology.py | 279 |
| L | GS003 | gsc_archaeology.py | 283 |
| L | GS003 | gsc_archaeology.py | 287 |
| L | GS003 | gsc_archaeology.py | 290 |
| L | GS003 | gsc_chain_composer.py | 88 |
| L | GS003 | gsc_chain_composer.py | 95 |
| L | GS003 | gsc_collect_light.py | 107 |
| L | GS003 | gsc_collect_light.py | 115 |
| L | GS003 | gsc_collect_light.py | 118 |
| L | GS003 | gsc_collect_light.py | 128 |
| L | GS003 | gsc_collect_light.py | 132 |
| L | GS003 | gsc_collect_light.py | 136 |
| L | GS003 | gsc_collect_light.py | 186 |
| L | GS003 | gsc_collect_light.py | 216 |
| L | GS003 | gsc_collect_light.py | 221 |
| L | GS003 | gsc_collect_light.py | 237 |
| L | GS003 | gsc_collect_light.py | 240 |
| L | GS003 | gsc_collect_light.py | 245 |
| L | GS003 | gsc_collect_light.py | 267 |
| L | GS003 | gsc_collect_light.py | 271 |
| L | GS003 | gsc_collect_light.py | 304 |
| L | GS003 | gsc_collect_light.py | 365 |
| L | GS003 | gsc_collect_light.py | 376 |
| L | GS003 | gsc_collect_light.py | 377 |
| L | GS003 | gsc_collect_light.py | 378 |
| L | GS003 | gsc_collect_light.py | 379 |
| L | GS003 | gsc_collect_light.py | 393 |
| L | GS003 | gsc_collect_light.py | 395 |
| L | GS003 | gsc_collect_light.py | 397 |
| L | GS003 | gsc_collector.py | 44 |
| L | GS003 | gsc_collector.py | 52 |
| L | GS003 | gsc_collector.py | 53 |
| L | GS003 | gsc_collector.py | 54 |
| L | GS003 | gsc_collector.py | 58 |
| L | GS003 | gsc_collector.py | 62 |
| L | GS003 | gsc_crossrepo_secrets.py | 149 |
| L | GS003 | gsc_crossrepo_secrets.py | 151 |
| L | GS003 | gsc_crossrepo_secrets.py | 155 |
| L | GS003 | gsc_db.py | 275 |
| L | GS003 | multi_lang.py | 188 |
| L | GS003 | multi_lang.py | 194 |
| L | GS003 | multi_lang.py | 196 |
| L | GS003 | multi_lang.py | 198 |
| L | GS003 | multi_lang.py | 200 |
| L | GS003 | gsc_external.py | 950 |
| L | GS003 | gsc_external.py | 977 |
| L | GS003 | gsc_external.py | 985 |
| L | GS003 | gsc_external.py | 1013 |
| L | GS003 | gsc_external.py | 1015 |
| L | GS003 | gsc_external.py | 1016 |
| L | GS003 | gsc_external.py | 1019 |
| L | GS003 | gsc_external.py | 1034 |
| L | GS003 | gsc_external.py | 1040 |
| L | GS003 | gsc_external.py | 1071 |
| L | GS003 | gsc_external.py | 1100 |
| L | GS003 | gsc_external.py | 1106 |
| L | GS003 | gsc_external.py | 1116 |
| L | GS003 | gsc_external.py | 1145 |
| L | GS003 | gsc_external.py | 1147 |
| L | GS003 | gsc_external.py | 1184 |
| L | GS003 | gsc_external.py | 1190 |
| L | GS003 | gsc_external.py | 1193 |
| L | GS003 | gsc_external.py | 1198 |
| L | GS003 | gsc_external.py | 1200 |
| L | GS003 | gsc_external.py | 1209 |
| L | GS003 | gsc_external.py | 1386 |
| L | GS003 | gsc_external.py | 1390 |
| L | GS003 | gsc_external.py | 1396 |
| L | GS003 | gsc_external.py | 1397 |
| L | GS003 | gsc_external.py | 1400 |
| L | GS003 | gsc_external.py | 1402 |
| L | GS003 | gsc_external.py | 1404 |
| L | GS003 | gsc_external.py | 1409 |
| L | GS003 | gsc_external.py | 1429 |
| L | GS003 | gsc_external.py | 1431 |
| L | GS003 | gsc_external.py | 1451 |
| L | GS003 | gsc_forecast.py | 270 |
| L | GS003 | gsc_forecast.py | 272 |
| L | GS003 | gsc_forecast.py | 273 |
| L | GS003 | gsc_forecast.py | 274 |
| L | GS003 | gsc_forecast.py | 275 |
| L | GS003 | gsc_forecast.py | 278 |
| L | GS003 | gsc_forecast.py | 286 |
| L | GS003 | gsc_forecast.py | 300 |
| L | GS003 | gsc_github_adapter.py | 76 |
| L | GS003 | gsc_github_adapter.py | 98 |
| L | GS003 | gsc_github_adapter.py | 255 |
| L | GS003 | gsc_github_adapter.py | 256 |
| L | GS003 | gsc_github_adapter.py | 267 |
| L | GS003 | gsc_github_adapter.py | 276 |
| L | GS003 | gsc_github_adapter.py | 278 |
| L | GS003 | gsc_github_adapter.py | 280 |
| L | GS003 | gsc_github_adapter.py | 307 |
| L | GS003 | gsc_github_adapter.py | 310 |
| L | GS003 | gsc_github_adapter.py | 326 |
| L | GS003 | gsc_github_adapter.py | 328 |
| L | GS003 | gsc_github_adapter.py | 330 |
| L | GS003 | gsc_github_adapter.py | 433 |
| L | GS003 | gsc_github_adapter.py | 434 |
| L | GS003 | gsc_github_adapter.py | 437 |
| L | GS003 | gsc_github_adapter.py | 438 |
| L | GS003 | gsc_github_adapter.py | 439 |
| L | GS003 | gsc_github_adapter.py | 440 |
| L | GS003 | gsc_github_adapter.py | 441 |
| L | GS003 | gsc_github_adapter.py | 442 |
| L | GS003 | gsc_github_adapter.py | 443 |
| L | GS003 | gsc_github_adapter.py | 444 |
| L | GS003 | gsc_github_adapter.py | 446 |
| L | GS003 | gsc_github_adapter.py | 448 |
| L | GS003 | gsc_github_adapter.py | 449 |
| L | GS003 | gsc_github_adapter.py | 477 |
| L | GS003 | gsc_github_adapter.py | 479 |
| L | GS003 | gsc_github_adapter.py | 480 |
| L | GS003 | gsc_github_adapter.py | 494 |
| L | GS003 | gsc_github_adapter.py | 531 |
| L | GS003 | gsc_github_adapter.py | 536 |
| L | GS003 | gsc_github_adapter.py | 561 |
| L | GS003 | gsc_github_adapter.py | 679 |
| L | GS003 | gsc_github_dorks.py | 120 |
| L | GS003 | gsc_github_dorks.py | 122 |
| L | GS003 | gsc_github_dorks.py | 124 |
| L | GS003 | gsc_github_dorks.py | 127 |
| L | GS003 | gsc_github_dorks.py | 133 |
| L | GS003 | gsc_github_dorks.py | 134 |
| L | GS003 | gsc_github_dorks.py | 143 |
| L | GS003 | gsc_github_dorks.py | 151 |
| L | GS003 | gsc_github_dorks.py | 160 |
| L | GS003 | gsc_github_dorks.py | 162 |
| L | GS003 | gsc_github_dorks.py | 165 |
| L | GS003 | gsc_github_dorks.py | 173 |
| L | GS003 | gsc_github_dorks.py | 175 |
| L | GS003 | gsc_github_dorks.py | 176 |
| L | GS003 | gsc_github_dorks.py | 177 |
| L | GS003 | gsc_github_dorks.py | 182 |
| L | GS003 | gsc_github_dorks.py | 201 |
| L | GS003 | gsc_github_dorks.py | 208 |
| L | GS003 | gsc_nlpolicy.py | 59 |
| L | GS003 | gsc_nlpolicy.py | 175 |
| L | GS003 | gsc_nlpolicy.py | 179 |
| L | GS003 | gsc_nlpolicy.py | 184 |
| L | GS003 | gsc_nlpolicy.py | 203 |
| L | GS003 | gsc_nlpolicy.py | 205 |
| L | GS003 | gsc_nlpolicy.py | 206 |
| L | GS003 | gsc_nlpolicy.py | 207 |
| L | GS003 | gsc_nlpolicy.py | 214 |
| L | GS003 | gsc_nlpolicy.py | 216 |
| L | GS003 | gsc_nlpolicy.py | 218 |
| L | GS003 | gsc_nlpolicy.py | 221 |
| L | GS003 | gsc_nlpolicy.py | 258 |
| L | GS003 | gsc_nlpolicy.py | 260 |
| L | GS003 | gsc_nlpolicy.py | 261 |
| L | GS003 | gsc_nlpolicy.py | 263 |
| L | GS003 | gsc_nlpolicy.py | 265 |
| L | GS003 | gsc_nlpolicy.py | 273 |
| L | GS003 | gsc_nlpolicy.py | 277 |
| L | GS003 | gsc_nlpolicy.py | 285 |
| L | GS003 | gsc_nlpolicy.py | 300 |
| L | GS003 | gsc_poc_generator.py | 77 |
| L | GS003 | gsc_poc_generator.py | 85 |
| L | GS003 | gsc_proofoffix.py | 63 |
| L | GS003 | gsc_proofoffix.py | 289 |
| L | GS003 | gsc_proofoffix.py | 299 |
| L | GS003 | gsc_proofoffix.py | 308 |
| L | GS003 | gsc_proofoffix.py | 316 |
| L | GS003 | gsc_proofoffix.py | 372 |
| L | GS003 | gsc_proofoffix.py | 373 |
| L | GS003 | gsc_selfhealing.py | 81 |
| L | GS003 | gsc_selfhealing.py | 83 |
| L | GS003 | gsc_selfhealing.py | 98 |
| L | GS003 | gsc_selfhealing.py | 123 |
| L | GS003 | gsc_selfhealing.py | 125 |
| L | GS003 | gsc_selfhealing.py | 130 |
| L | GS003 | gsc_selfhealing.py | 186 |
| L | GS003 | gsc_selfhealing.py | 187 |
| L | GS003 | gsc_selfhealing.py | 188 |
| L | GS003 | gsc_selfhealing.py | 189 |
| L | GS003 | gsc_selfhealing.py | 190 |
| L | GS003 | gsc_selfhealing.py | 211 |
| L | GS003 | gsc_selfhealing.py | 214 |
| L | GS003 | gsc_selfhealing.py | 234 |
| L | GS003 | gsc_selfhealing.py | 235 |
| L | GS003 | ci_report.py | 13 |
| L | GS003 | ci_report.py | 14 |
| L | GS003 | ci_report.py | 15 |
| L | GS003 | ci_report.py | 16 |
| L | GS003 | ci_report.py | 17 |
| L | GS003 | ci_report.py | 18 |
| L | GS003 | ci_report.py | 19 |
| L | GS003 | ci_report.py | 22 |
| L | GS003 | ci_report.py | 24 |
| L | GS003 | ci_report.py | 27 |
| L | GS003 | ci_report.py | 29 |
| L | GS003 | ci_report.py | 32 |
| L | GS003 | ci_report.py | 33 |
| L | GS003 | db_encrypt.py | 49 |
| L | GS003 | db_encrypt.py | 53 |
| L | GS003 | db_encrypt.py | 66 |
| L | GS003 | db_encrypt.py | 76 |
| L | GS003 | db_encrypt.py | 85 |
| L | GS003 | db_encrypt.py | 114 |
| L | GS003 | db_encrypt.py | 116 |
| L | GS003 | db_encrypt.py | 117 |
| L | GS003 | db_encrypt.py | 119 |
| L | GS003 | e4_llm.py | 347 |
| L | GS003 | e4_llm.py | 349 |
| L | GS003 | framework_aware.py | 153 |
| L | GS003 | framework_aware.py | 174 |
| L | GS003 | gsc_backfill_fingerprints.py | 17 |
| L | GS003 | gsc_backfill_fingerprints.py | 39 |
| L | GS003 | gsc_backfill_fingerprints.py | 41 |
| L | GS003 | gsc_baseline.py | 12 |
| L | GS003 | gsc_baseline.py | 48 |
| L | GS003 | gsc_baseline.py | 56 |
| L | GS003 | gsc_baseline.py | 63 |
| L | GS003 | gsc_baseline.py | 81 |
| L | GS003 | gsc_baseline.py | 85 |
| L | GS003 | gsc_baseline.py | 96 |
| L | GS003 | gsc_calibration.py | 86 |
| L | GS003 | gsc_calibration.py | 111 |
| L | GS003 | gsc_calibration.py | 224 |
| L | GS003 | gsc_calibration.py | 227 |
| L | GS003 | gsc_calibration.py | 251 |
| L | GS003 | gsc_calibration.py | 254 |
| L | GS003 | gsc_calibration.py | 255 |
| L | GS003 | gsc_calibration.py | 256 |
| L | GS003 | gsc_calibration.py | 257 |
| L | GS003 | gsc_calibration.py | 258 |
| L | GS003 | gsc_calibration.py | 259 |
| L | GS003 | gsc_calibration.py | 260 |
| L | GS003 | gsc_calibration.py | 261 |
| L | GS003 | gsc_calibration.py | 264 |
| L | GS003 | gsc_config.py | 28 |
| L | GS003 | gsc_config.py | 31 |
| L | GS003 | gsc_config.py | 36 |
| L | GS003 | gsc_config.py | 49 |
| L | GS003 | gsc_config.py | 53 |
| L | GS003 | gsc_config.py | 65 |
| L | GS003 | gsc_config.py | 66 |
| L | GS003 | gsc_doctor.py | 7 |
| L | GS003 | gsc_doctor.py | 8 |
| L | GS003 | gsc_doctor.py | 74 |
| L | GS003 | gsc_dryrun_summary.py | 34 |
| L | GS003 | gsc_issue.py | 54 |
| L | GS003 | gsc_issue.py | 77 |
| L | GS003 | gsc_issue.py | 79 |
| L | GS003 | gsc_issue.py | 87 |
| L | GS003 | gsc_issue.py | 125 |
| L | GS003 | gsc_issue.py | 127 |
| L | GS003 | gsc_issue.py | 132 |
| L | GS003 | gsc_issue.py | 133 |
| L | GS003 | gsc_issue.py | 140 |
| L | GS003 | gsc_issue.py | 141 |
| L | GS003 | gsc_issue.py | 146 |
| L | GS003 | gsc_issue.py | 151 |
| L | GS003 | gsc_marketplace.py | 45 |
| L | GS003 | gsc_marketplace.py | 56 |
| L | GS003 | gsc_metrics.py | 20 |
| L | GS003 | gsc_pdf.py | 10 |
| L | GS003 | gsc_pdf.py | 19 |
| L | GS003 | gsc_pr_comment.py | 68 |
| L | GS003 | gsc_pr_comment.py | 99 |
| L | GS003 | gsc_pr_comment.py | 101 |
| L | GS003 | gsc_pr_feedback.py | 52 |
| L | GS003 | gsc_pr_feedback.py | 98 |
| L | GS003 | gsc_pr_feedback.py | 101 |
| L | GS003 | gsc_pr_feedback.py | 104 |
| L | GS003 | gsc_pr_scanner.py | 61 |
| L | GS003 | gsc_pr_scanner.py | 124 |
| L | GS003 | gsc_pr_scanner.py | 130 |
| L | GS003 | gsc_pr_scanner.py | 134 |
| L | GS003 | gsc_pr_scanner.py | 138 |
| L | GS003 | gsc_pr_scanner.py | 142 |
| L | GS003 | gsc_pr_scanner.py | 144 |
| L | GS003 | gsc_reachability.py | 91 |
| L | GS003 | gsc_reachability.py | 96 |
| L | GS003 | gsc_reachability.py | 106 |
| L | GS003 | gsc_reachability.py | 108 |
| L | GS003 | gsc_reachability.py | 110 |
| L | GS003 | gsc_reactions.py | 42 |
| L | GS003 | gsc_redact_report.py | 43 |
| L | GS003 | gsc_report.py | 10 |
| L | GS003 | gsc_report.py | 73 |
| L | GS003 | gsc_report_dryrun.py | 10 |
| L | GS003 | gsc_report_dryrun.py | 31 |
| L | GS003 | gsc_rollout_metrics.py | 94 |
| L | GS003 | gsc_rollout_metrics.py | 95 |
| L | GS003 | gsc_rollout_metrics.py | 96 |
| L | GS003 | gsc_rollout_metrics.py | 97 |
| L | GS003 | gsc_rollout_metrics.py | 98 |
| L | GS003 | gsc_rollout_metrics.py | 100 |
| L | GS003 | gsc_rollout_metrics.py | 102 |
| L | GS003 | gsc_rollout_metrics.py | 103 |
| L | GS003 | gsc_rollout_metrics.py | 104 |
| L | GS003 | gsc_rollout_metrics.py | 107 |
| L | GS003 | gsc_rollout_metrics.py | 108 |
| L | GS003 | gsc_rollout_metrics.py | 110 |
| L | GS003 | gsc_rollout_metrics.py | 113 |
| L | GS003 | gsc_rollout_metrics.py | 114 |
| L | GS003 | gsc_rollout_metrics.py | 128 |
| L | GS003 | gsc_rollout_metrics.py | 130 |
| L | GS003 | gsc_rollout_metrics.py | 132 |
| L | GS003 | gsc_rollout_metrics.py | 143 |
| L | GS008 | session.py | 47 |
| L | GS008 | batch_and_override.py | 39 |
| L | GS008 | gsc.py | 46 |
| L | GS008 | gsc.py | 59 |
| L | GS008 | gsc_chain_composer.py | 23 |
| L | GS008 | settings.py | 5 |
| L | GS008 | settings.py | 6 |
| L | GS008 | settings.py | 7 |
| L | GS008 | settings.py | 10 |
| L | GS008 | settings.py | 11 |
| L | GS008 | settings.py | 12 |
| L | GS008 | settings.py | 13 |
| L | GS008 | settings.py | 14 |
| L | GS008 | settings.py | 17 |
| L | GS008 | settings.py | 24 |
| L | GS008 | settings.py | 25 |
| L | GS008 | settings.py | 29 |
| L | GS008 | settings.py | 33 |
| L | GS008 | settings.py | 34 |
| L | GS008 | settings.py | 37 |
| L | GS008 | gs001_hardcoded_secret.py | 21 |
| L | GS008 | gs002_world_readable.py | 19 |
| L | GS008 | gs003_debug_prints.py | 18 |
| L | GS008 | gs004_dangerous_subprocess.py | 22 |
| L | GS008 | gs005_sql_injection.py | 33 |
| L | GS008 | gs005_sql_injection.py | 34 |
| L | GS008 | gs005_sql_injection.py | 63 |
| L | GS008 | gs007_idor.py | 26 |
| L | GS008 | gs007_idor.py | 27 |
| L | GS008 | gs008_dead_code.py | 24 |
| L | GS008 | gs009_supply_chain.py | 26 |
| L | GS008 | gs010_ssh_hardening.py | 25 |
| L | GS008 | gs011_jwt_vulnerabilities.py | 23 |
| L | GS008 | gs012_mass_assignment.py | 23 |
| L | GS008 | gs013_graphql_security.py | 24 |
| L | GS008 | gs014_credential_exposure.py | 28 |
| L | GS008 | gs015_entry_points.py | 20 |
| L | GS008 | gs016_linux_priv_esc.py | 25 |
| L | GS008 | gs016_linux_priv_esc.py | 26 |
| L | GS008 | gs017_weak_passwords.py | 24 |
| L | GS008 | gs017_weak_passwords.py | 25 |
| L | GS008 | gs018_payment_abuse.py | 29 |
| L | GS008 | gs018_payment_abuse.py | 30 |
| L | GS008 | gs018_payment_abuse.py | 39 |
| L | GS008 | gs018_payment_abuse.py | 54 |
| L | GS008 | gs018_payment_abuse.py | 61 |
| L | GS008 | gs018_payment_abuse.py | 81 |
| L | GS008 | gs018_payment_abuse.py | 97 |
| L | GS008 | gs018_payment_abuse.py | 109 |
| L | GS008 | gs018_payment_abuse.py | 118 |
| L | GS008 | gs019_auth_session.py | 30 |
| L | GS008 | gs019_auth_session.py | 31 |
| L | GS008 | gs019_auth_session.py | 46 |
| L | GS008 | gs019_auth_session.py | 59 |
| L | GS008 | gs019_auth_session.py | 68 |
| L | GS008 | gs019_auth_session.py | 87 |
| L | GS008 | gs019_auth_session.py | 111 |
| L | GS008 | gs019_auth_session.py | 139 |
| L | GS008 | gs020_llm_sqli.py | 28 |
| L | GS008 | gs020_llm_sqli.py | 29 |
| L | GS008 | gs020_xss_injection.py | 26 |
| L | GS008 | gs021_csrf_ssrf.py | 24 |
| L | GS008 | gs022_open_redirect.py | 25 |
| L | GS008 | gs023_race_conditions.py | 26 |
| L | GS008 | gs025_ai_provenance.py | 125 |
| L | GS008 | gs025_ai_provenance.py | 126 |
| L | GS008 | gs025_ai_provenance.py | 127 |
| L | GS008 | registry.py | 239 |
| L | GS008 | registry.py | 240 |
| L | GS008 | gsc_github_adapter.py | 34 |
| L | GS008 | gsc_nlpolicy.py | 137 |
| L | GS008 | gsc_proofoffix.py | 27 |
| L | GS008 | gsc_pr_commands.py | 10 |
| i | GS020 |  | 135 |
| i | GS020 |  | 184 |
| i | GS020 |  | 192 |
| i | GS020 |  | 267 |
| i | GS020 |  | 126 |
| i | GS020 |  | 45 |
| i | GS020 |  | 46 |
| i | GS020 |  | 10 |
| i | GS020 |  | 34 |
| i | GS020 |  | 34 |
| i | GS020 |  | 36 |
| i | GS020 |  | 45 |
| i | GS020 |  | 65 |
| i | GS020 |  | 65 |
| i | GS020 |  | 65 |
| i | GS020 |  | 31 |
| H | ? | gsc_external.py | 174 |
| H | ? | gsc_external.py | 1307 |
| H | ? | bughunter.json | 45 |
| H | ? | terraform.json | 3 |
| H | ? | docker.json | 6 |
| H | ? | Dockerfile | 18 |
| H | ? | docker-compose.yml | 35 |
| H | ? | sso.yaml | 14 |
| H | ? | gsc.py | 1887 |
| H | ? | gsc_proofoffix.py | 31 |
| H | ? | gsc_proofoffix.py | 32 |
| H | ? | gsc_proofoffix.py | 33 |
| H | ? | gsc_proofoffix.py | 34 |
| H | ? | gsc_api.py | 413 |
| H | ? | gs010_ssh_hardening.py | 85 |
| H | ? | user_auth.py | 60 |
| H | ? | sso.py | 36 |
| H | ? | gsc_issue.py | 74 |
| H | ? | framework_aware.py | 21 |
| H | ? | framework_aware.py | 167 |
| H | ? | gsc.py | 703 |
| H | ? | gsc.py | 712 |
| H | ? | gsc.py | 1262 |
| H | ? | gs004_dangerous_subprocess.py | 72 |
| H | ? | gs004_dangerous_subprocess.py | 73 |
| H | ? | gs004_dangerous_subprocess.py | 78 |
| H | ? | gs004_dangerous_subprocess.py | 79 |
| H | ? | gs020_xss_injection.py | 38 |
| H | ? | gsc_vuln_spider.py | 31 |
| H | ? | gsc_pdf.py | 15 |
| H | ? | gs004_dangerous_subprocess.py | 48 |
| M | ? | systemd.json | 18 |
| M | ? | systemd.json | 19 |
| H | ? | systemd.json | 23 |
| M | ? | systemd.json | 63 |
| M | ? | systemd.json | 68 |
| C | ? | systemd.json | 78 |
| H | ? | .mcp.json | 0 |
| H | GS004 | gs004_dangerous_subprocess.py | 54 |
| H | GS004 | gs004_dangerous_subprocess.py | 60 |
| H | GS004 | gsc_pdf.py | 15 |
| C | GS005 | corpus_gs005_javascript.js | 10 |
| C | GS005 | corpus_gs005_javascript.js | 14 |
| C | GS005 | corpus_gs005_javascript.js | 17 |
| C | GS005 | corpus_gs005_javascript.js | 20 |
| H | GS005 | corpus_gs005_javascript.js | 20 |
| H | GS005 | corpus_gs005_javascript.js | 21 |
| C | GS005 | corpus_gs005_php.php | 6 |
| C | GS005 | corpus_gs005_php.php | 7 |
| C | GS005 | corpus_gs005_php.php | 10 |
| C | GS005 | corpus_gs005_php.php | 11 |
| C | GS005 | corpus_gs005_php.php | 14 |
| C | GS005 | corpus_gs005_php.php | 17 |
| C | GS005 | corpus_gs005_php.php | 18 |
| C | GS005 | corpus_gs005_python.py | 8 |
| C | GS005 | corpus_gs005_python.py | 9 |
| C | GS005 | corpus_gs005_python.py | 10 |
| C | GS005 | corpus_gs005_python.py | 11 |
| C | GS005 | corpus_gs005_python.py | 12 |
| C | GS005 | corpus_gs005_python.py | 15 |
| C | GS005 | corpus_gs005_python.py | 16 |
| C | GS005 | corpus_gs005_python.py | 16 |
| C | GS005 | corpus_gs005_python.py | 16 |
| C | GS005 | corpus_gs005_python.py | 19 |
| C | GS005 | corpus_gs005_python.py | 19 |
| C | GS005 | corpus_gs005_python.py | 20 |
| C | GS005 | corpus_gs005_python.py | 20 |
| C | GS005 | corpus_gs005_python.py | 23 |
| C | GS005 | corpus_gs005_python.py | 24 |
| C | GS005 | corpus_gs005_python.py | 24 |
| C | GS005 | corpus_gs005_python.py | 24 |
| C | GS005 | corpus_gs005_python.py | 25 |
| C | GS005 | corpus_gs005_python.py | 25 |
| C | GS005 | corpus_gs005_python.py | 28 |
| C | GS005 | corpus_gs005_python.py | 31 |
| C | GS005 | corpus_gs005_python.py | 32 |
| C | GS005 | corpus_gs005_python.py | 33 |
| C | GS005 | corpus_gs005_python.py | 34 |
| C | GS005 | corpus_gs005_python.py | 34 |
| C | GS005 | corpus_gs005_python.py | 37 |
| C | GS005 | corpus_gs005_python.py | 38 |
| C | GS005 | corpus_gs005_python.py | 39 |
| C | GS005 | corpus_gs005_python.py | 39 |
| C | GS005 | corpus_gs005_python.py | 43 |
| C | GS005 | corpus_gs005_python.py | 43 |
| H | GS005 | corpus_gs005_python.py | 46 |
| H | GS005 | corpus_gs005_python.py | 49 |
| C | GS005 | corpus_gs005_python.py | 50 |
| C | GS005 | corpus_gs005_ruby.rb | 5 |
| C | GS005 | corpus_gs005_ruby.rb | 6 |
| C | GS005 | corpus_gs005_ruby.rb | 7 |
| C | GS005 | corpus_gs005_ruby.rb | 8 |
| C | GS005 | gsc_db_backend.py | 60 |
| C | GS005 | gs020_llm_sqli.py | 126 |
| C | GS005 | gs020_llm_sqli.py | 230 |
| C | GS005 | gsc_metrics.py | 31 |
| C | GS005 | gsc_metrics.py | 34 |
| C | GS005 | gsc_metrics.py | 40 |
| C | GS005 | gsc_metrics.py | 46 |
| C | GS005 | gsc_metrics.py | 52 |
| C | GS005 | gsc_metrics.py | 74 |
| C | GS005 | gsc_metrics.py | 101 |
| H | GS007 | api.py | 65 |
| I | GS007 | schema_s1.sql | 3 |
| I | GS007 | schema_s1.sql | 12 |
| I | GS007 | schema_s1.sql | 21 |
| I | GS007 | schema_s1.sql | 29 |
| I | GS007 | schema_s1.sql | 44 |
| I | GS007 | schema_s1.sql | 58 |
| I | GS007 | schema_s2.sql | 4 |
| I | GS007 | schema_s2.sql | 27 |
| I | GS007 | schema_s2.sql | 40 |
| I | GS007 | schema_s2.sql | 51 |
| I | GS007 | schema_s2.sql | 64 |
| I | GS007 | schema_s2.sql | 77 |
| I | GS007 | schema_s3.sql | 4 |
| I | GS007 | schema_s3.sql | 14 |
| I | GS007 | schema_s3.sql | 31 |
| I | GS007 | schema_s4.sql | 5 |
| I | GS007 | schema_s4.sql | 46 |
| I | GS007 | schema_s5.sql | 4 |
| I | GS007 | schema_s5.sql | 15 |
| I | GS007 | schema_s5.sql | 27 |
| H | GS007 | user_auth.py | 123 |
| H | GS007 | corpus_gs005_javascript.js | 10 |
| H | GS007 | corpus_gs005_javascript.js | 13 |
| H | GS007 | corpus_gs005_php.php | 18 |
| H | GS007 | batch_and_override.py | 31 |
| H | GS007 | batch_and_override.py | 39 |
| H | GS007 | batch_and_override.py | 39 |
| H | GS007 | batch_and_override.py | 44 |
| H | GS007 | batch_and_override.py | 44 |
| H | GS007 | batch_and_override.py | 45 |
| I | GS007 | django_cross_org.py | 13 |
| H | GS007 | express_files.js | 17 |
| H | GS007 | express_files.js | 12 |
| H | GS007 | fastapi_support.py | 35 |
| H | GS007 | laravel_tickets.php | 29 |
| I | GS007 | schema.sql | 6 |
| I | GS007 | schema.sql | 6 |
| I | GS007 | schema.sql | 6 |
| H | GS007 | schema.sql | 12 |
| I | GS007 | gsc_crossrepo_secrets.py | 55 |
| I | GS007 | gsc_db.py | 50 |
| I | GS007 | gsc_db.py | 90 |
| I | GS007 | gsc_db.py | 103 |
| I | GS007 | gsc_db.py | 150 |
| I | GS007 | gsc_db.py | 167 |
| I | GS007 | gs007_idor.py | 54 |
| I | GS007 | gs007_idor.py | 54 |
| I | GS007 | gs007_idor.py | 56 |
| I | GS007 | gs007_idor.py | 56 |
| I | GS007 | gs007_idor.py | 56 |
| I | GS007 | gs007_idor.py | 185 |
| H | GS007 | gs007_idor.py | 101 |
| H | GS007 | gs007_idor.py | 101 |
| H | GS007 | gs007_idor.py | 101 |
| I | GS007 | gsc_workspace.py | 39 |
| I | GS007 | gsc_workspace.py | 46 |
| I | GS007 | gsc_workspace.py | 54 |
| s | GS009 |  | 0 |
| H | GS012 | gs012_mass_assignment.py | 44 |
| M | GS012 | gsc_issue.py | 90 |
| H | GS014 | docker-compose.yml | 37 |
| H | GS014 | docker-compose.yml | 62 |
| H | GS014 | gsc_vuln_spider.py | 47 |
| H | GS014 | 00-namespace-config.yaml | 25 |
| C | GS016 | gs016_linux_priv_esc.py | 35 |
| M | GS019 | gs021_csrf_ssrf.py | 37 |
| s | GS021 |  | 81 |
| s | GS021 |  | 174 |
| s | GS021 |  | 174 |
| s | GS021 |  | 1307 |
| s | GS021 |  | 1307 |
| s | GS021 |  | 71 |
| s | GS021 |  | 1014 |
| s | GS021 |  | 1887 |
| s | GS021 |  | 1887 |
| s | GS021 |  | 31 |
| s | GS021 |  | 32 |
| s | GS021 |  | 33 |
| s | GS021 |  | 34 |
| s | GS021 |  | 413 |
| s | GS021 |  | 119 |
| s | GS021 |  | 28 |
| c | GS021 |  | 31 |
| c | GS021 |  | 31 |
| c | GS021 |  | 39 |
| c | GS021 |  | 41 |
| s | GS021 |  | 53 |
| s | GS021 |  | 53 |
| s | GS021 |  | 10 |
| s | GS021 |  | 55 |
| s | GS021 |  | 55 |
| r | GS022 |  | 19 |
| r | GS022 |  | 6 |
| r | GS022 |  | 142 |
| r | GS022 |  | 668 |
| r | GS022 |  | 23 |
| r | GS022 |  | 24 |
| r | GS022 |  | 53 |
| r | GS022 |  | 18 |
| r | GS022 |  | 29 |
| r | GS022 |  | 34 |
| r | GS022 |  | 45 |
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
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| C | GS024 | corpus_gs005_python.py | 8 |
| C | GS024 | corpus_gs005_python.py | 9 |
| C | GS024 | corpus_gs005_python.py | 15 |
| C | GS024 | gs020_llm_sqli.py | 230 |
| C | GS024 | gsc_metrics.py | 31 |
| C | GS024 | gsc_metrics.py | 34 |
| M | ? | gsc_external.py | 732 |
| M | ? | gsc_external.py | 737 |
| M | ? | gsc_external.py | 762 |
| M | ? | gsc_external.py | 764 |
| M | ? | gsc_external.py | 775 |
| M | ? | gsc_external.py | 794 |
| M | ? | gsc_external.py | 796 |
| M | ? | gsc_external.py | 916 |
| M | ? | gsc_external.py | 920 |
| M | ? | gsc_external.py | 966 |
| M | ? | gsc_external.py | 972 |
| M | ? | gsc_external.py | 979 |
| M | ? | gsc_external.py | 1022 |
| M | ? | bughunter.json | 32 |
| M | ? | bughunter.json | 33 |
| M | ? | python_async.json | 42 |
| M | ? | python_async.json | 53 |
| M | ? | python_async.json | 74 |
| M | ? | python_async.json | 75 |
| M | ? | github_worker.py | 35 |
| M | ? | github_worker.py | 38 |
| M | ? | github_worker.py | 58 |
| M | ? | worker.py | 46 |
| M | ? | gsc_github_dorks.py | 94 |
| M | ? | gsc_evidence_pack.py | 25 |
| M | ? | gsc_evidence_pack.py | 32 |
| M | ? | gsc_pr_scanner.py | 46 |
| M | ? | gsc_pr_scanner.py | 117 |
| M | ? | gsc_calibration.py | 131 |
| M | ? | gsc_calibration.py | 134 |
| M | ? | gsc_doctor.py | 21 |
| M | ? | gsc_doctor.py | 31 |
| M | ? | e4_llm.py | 307 |
| M | ? | gsc_github_adapter.py | 488 |
| M | ? | gsc_github_adapter.py | 489 |
| M | ? | gsc_github_adapter.py | 511 |
| M | ? | gsc_github_adapter.py | 565 |
| M | ? | gsc_revalidate.py | 78 |
| M | ? | gsc_revalidate.py | 91 |
| M | ? | gsc.py | 94 |
| M | ? | gsc.py | 402 |
| M | ? | gsc.py | 445 |
| M | ? | gsc.py | 562 |
| M | ? | gsc.py | 1195 |
| M | ? | gsc.py | 1197 |
| M | ? | gsc.py | 1199 |
| M | ? | gsc.py | 1973 |
| M | ? | gsc.py | 1985 |
| M | ? | gsc.py | 1995 |
| M | ? | gsc.py | 2003 |
| M | ? | gsc.py | 2008 |
| M | ? | gsc.py | 2011 |
| M | ? | gsc.py | 2014 |
| M | ? | gsc.py | 2027 |
| M | ? | gsc.py | 2029 |
| M | ? | gsc.py | 2054 |
| M | ? | gsc.py | 2060 |
| M | ? | gsc.py | 2069 |
| M | ? | gsc.py | 2073 |
| M | ? | gsc.py | 2098 |
| M | ? | gsc.py | 2101 |
| M | ? | gsc.py | 2111 |
| M | ? | gsc_archaeology.py | 70 |
| M | ? | gsc_archaeology.py | 92 |
| M | ? | runner.py | 88 |
| M | ? | gsc_forecast.py | 35 |
| M | ? | gsc_forecast.py | 48 |
| M | ? | gsc_forecast.py | 69 |
| M | ? | gsc_forecast.py | 223 |
| M | ? | gsc_proofoffix.py | 209 |
| M | ? | gsc_proofoffix.py | 246 |
| M | ? | gsc_selfhealing.py | 184 |
| M | ? | gsc_selfhealing.py | 194 |
| M | ? | gsc_selfhealing.py | 195 |
| M | ? | gsc_selfhealing.py | 196 |
| M | ? | gsc_selfhealing.py | 200 |
| M | ? | gsc_selfhealing.py | 202 |
| M | ? | gs009_supply_chain.py | 79 |
| M | ? | gs004_dangerous_subprocess.py | 39 |
| M | ? | gs004_dangerous_subprocess.py | 44 |
| M | ? | gs004_dangerous_subprocess.py | 49 |
| M | ? | gs004_dangerous_subprocess.py | 61 |
| M | ? | go.json | 9 |
| H | ? | rust.json | 7 |

---
*Сгенерировано GSC v0.6 · 2026-08-06T21:47:48.312445*