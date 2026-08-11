---
title: "GSC Audit: ."
date: 2026-08-05
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — .

**Дата:** 05.08.2026 14:11  
**Путь:** `/home/openclaw/gsc`  
**Всего находок:** 1126  
**CRITICAL:** 279 | **HIGH:** 81 | **MEDIUM:** 86 | **LOW:** 604

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 358 |
| GS001 | 165 |
| GS008 | 69 |
| GS005 | 60 |
| Синхронный код в async | 55 |
| GS007 | 28 |
| GS025-eval_usage | 20 |
| GS021 | 19 |
| SQL injection risk: f-string in query | 16 |
| GS020 | 16 |
| CVE-2026-55721: SQL injection | 15 |
| CVE-2026-56233: Privilege escalation | 15 |
| eval() or exec() usage | 11 |
| CVE-2026-56413: Command injection | 10 |
| Хардкод IP адреса | 9 |
| CVE-2026-56356: Cross-site scripting (XSS) | 8 |
| Bare except: | 7 |
| GS024 | 6 |
| Python: raw string concatenation in SQL | 4 |
| CVE-2026-56219: Authentication bypass | 4 |
| GS022 | 4 |
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
| CVE-2026-54696: Buffer overflow | 3 |
| CVE-2026-55223: Insecure deserialization | 3 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 3 |
| flipkart-incubator/Astra: modules/jwt_attack.py | 3 |
| GS004 | 3 |
| CVE-2026-56233: Path traversal | 2 |
| sileht/bird-lg: lg.py | 2 |
| poliakarmai/gsc: gsc_collect_light.py | 2 |
| CVE-2026-37270: Hardcoded credential | 2 |
| os.system() without sanitization | 2 |
| Systemd: EnvironmentFile without quotes → word splitting | 2 |
| Systemd: Type=forking without PIDFile | 2 |
| GS012 | 2 |
| Python: SSRF via requests without URL validation | 1 |
| Python: File upload without content-type validation | 1 |
| FastAPI: **body spread | 1 |
| Postgres URL with password | 1 |
| CVE-2026-56318: Information disclosure | 1 |
| User-controlled URL in request | 1 |
| Systemd: User=root or absent → runs as root | 1 |
| Systemd: AmbientCapabilities with ALL caps | 1 |
| GS009 | 1 |
| GS014 | 1 |
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
| CRITICAL | ? | gs018_payment_abuse.py | 211 | OWASP A03: Injection |
| CRITICAL | ? | gs020_llm_sqli.py | 122 | OWASP A03: Injection |
| CRITICAL | ? | gs020_llm_sqli.py | 226 | OWASP A03: Injection |
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
| CRITICAL | ? | gs020_llm_sqli.py | 122 |  |
| CRITICAL | ? | gs020_llm_sqli.py | 226 |  |
| CRITICAL | ? | _cron_collect.py | 141 |  |
| CRITICAL | ? | gsc_pdf.py | 15 |  |
| CRITICAL | ? | gsc.py | 1258 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 34 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 39 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 44 |  |
| CRITICAL | ? | gs004_dangerous_subprocess.py | 111 |  |
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
| CRITICAL | GS001 | manifest.json | 249 | Found: "bb0744740ba2e343a19f4d77f388842a" |
| CRITICAL | GS001 | manifest.json | 250 | Found: "bb0744740ba2e343a19f4d77f388842a" |
| CRITICAL | GS001 | manifest.json | 289 | Found: "dd648e75e997d21b11471747b746a2f0" |
| CRITICAL | GS001 | manifest.json | 290 | Found: "dd648e75e997d21b11471747b746a2f0" |
| CRITICAL | GS001 | manifest.json | 339 | Found: "cc350016c2c90504944929ddcae40500" |
| CRITICAL | GS001 | manifest.json | 340 | Found: "cc350016c2c90504944929ddcae40500" |
| CRITICAL | GS001 | manifest.json | 344 | Found: "df82b30c519a4adb8fa80b6fd3b3990f" |
| CRITICAL | GS001 | manifest.json | 345 | Found: "df82b30c519a4adb8fa80b6fd3b3990f" |
| CRITICAL | GS001 | gsc_chain_composer.py | 22 | Found: "GS001" |
| CRITICAL | GS001 | gsc_chain_composer.py | 22 | Found: "GS004" |
| CRITICAL | GS001 | gsc_chain_composer.py | 22 | Found: "GS005" |
| CRITICAL | GS001 | gsc_chain_composer.py | 23 | Found: "GS007" |
| CRITICAL | GS001 | gsc_chain_composer.py | 23 | Found: "GS012" |
| CRITICAL | GS001 | gsc_chain_composer.py | 24 | Found: "GS014" |
| CRITICAL | GS001 | gsc_chain_composer.py | 25 | Found: "GS019" |
| CRITICAL | GS001 | gsc_chain_composer.py | 25 | Found: "GS011" |
| CRITICAL | GS001 | gsc_chain_composer.py | 26 | Found: "GS022" |
| CRITICAL | GS001 | gsc_chain_composer.py | 26 | Found: "GS021" |
| CRITICAL | GS001 | gsc_chain_composer.py | 27 | Found: "GS020" |
| CRITICAL | GS001 | gsc_chain_composer.py | 28 | Found: "GS024" |
| CRITICAL | GS001 | gsc_chain_composer.py | 34 | Found: "GS010" |
| CRITICAL | GS001 | gsc_chain_composer.py | 34 | Found: "GS016" |
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
| CRITICAL | GS001 | gs001_hardcoded_secret.py | 16 | Found: "GS001" |
| CRITICAL | GS001 | gs001_hardcoded_secret.py | 94 | Found: "GS001" |
| CRITICAL | GS001 | gs002_world_readable.py | 14 | Found: "GS002" |
| CRITICAL | GS001 | gs002_world_readable.py | 41 | Found: "GS002" |
| CRITICAL | GS001 | gs003_debug_prints.py | 13 | Found: "GS003" |
| CRITICAL | GS001 | gs003_debug_prints.py | 54 | Found: "GS003" |
| CRITICAL | GS001 | gs004_dangerous_subprocess.py | 17 | Found: "GS004" |
| CRITICAL | GS001 | gs004_dangerous_subprocess.py | 82 | Found: "GS004" |
| CRITICAL | GS001 | gs005_sql_injection.py | 28 | Found: "GS005" |
| CRITICAL | GS001 | gs007_idor.py | 21 | Found: "GS007" |
| CRITICAL | GS001 | gs007_idor.py | 149 | Found: "GS007" |
| CRITICAL | GS001 | gs008_dead_code.py | 19 | Found: "GS008" |
| CRITICAL | GS001 | gs008_dead_code.py | 69 | Found: "GS008" |
| CRITICAL | GS001 | gs009_supply_chain.py | 20 | Found: "GS009" |
| CRITICAL | GS001 | gs010_ssh_hardening.py | 20 | Found: "GS010" |
| CRITICAL | GS001 | gs010_ssh_hardening.py | 26 | Found: "GS010" |
| CRITICAL | GS001 | gs011_jwt_vulnerabilities.py | 18 | Found: "GS011" |
| CRITICAL | GS001 | gs011_jwt_vulnerabilities.py | 52 | Found: "GS011" |
| CRITICAL | GS001 | gs012_mass_assignment.py | 18 | Found: "GS012" |
| CRITICAL | GS001 | gs012_mass_assignment.py | 78 | Found: "GS012" |
| CRITICAL | GS001 | gs013_graphql_security.py | 19 | Found: "GS013" |
| CRITICAL | GS001 | gs013_graphql_security.py | 85 | Found: "GS013" |
| CRITICAL | GS001 | gs014_credential_exposure.py | 23 | Found: "GS014" |
| CRITICAL | GS001 | gs014_credential_exposure.py | 109 | Found: "GS014" |
| CRITICAL | GS001 | gs015_entry_points.py | 15 | Found: "GS015" |
| CRITICAL | GS001 | gs015_entry_points.py | 83 | Found: "GS015" |
| CRITICAL | GS001 | gs016_linux_priv_esc.py | 20 | Found: "GS016" |
| CRITICAL | GS001 | gs017_weak_passwords.py | 19 | Found: "GS017" |
| CRITICAL | GS001 | gs017_weak_passwords.py | 105 | Found: "GS017" |
| CRITICAL | GS001 | gs018_payment_abuse.py | 24 | Found: "GS018" |
| CRITICAL | GS001 | gs018_payment_abuse.py | 133 | Found: "GS018" |
| CRITICAL | GS001 | gs019_auth_session.py | 25 | Found: "GS019" |
| CRITICAL | GS001 | gs019_auth_session.py | 169 | Found: "GS019" |
| CRITICAL | GS001 | gs020_llm_sqli.py | 22 | Found: "GS024" |
| CRITICAL | GS001 | gs020_xss_injection.py | 20 | Found: "GS020" |
| CRITICAL | GS001 | gs021_csrf_ssrf.py | 18 | Found: "GS021" |
| CRITICAL | GS001 | gs022_open_redirect.py | 19 | Found: "GS022" |
| CRITICAL | GS001 | gs023_race_conditions.py | 20 | Found: "GS023" |
| CRITICAL | GS001 | gs025_ai_provenance.py | 64 | Found: "GS025" |
| CRITICAL | GS001 | gs025_ai_provenance.py | 121 | Found: "GS025" |
| CRITICAL | GS001 | gs028_invariants.py | 17 | Found: "GS028" |
| CRITICAL | GS001 | multi_lang.py | 17 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 18 | Found: "GS002" |
| CRITICAL | GS001 | multi_lang.py | 21 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 22 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 24 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 27 | Found: "GS002" |
| CRITICAL | GS001 | multi_lang.py | 28 | Found: "GS015" |
| CRITICAL | GS001 | multi_lang.py | 35 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 37 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 40 | Found: "GS017" |
| CRITICAL | GS001 | multi_lang.py | 42 | Found: "GS020" |
| CRITICAL | GS001 | multi_lang.py | 43 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 44 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 47 | Found: "GS018" |
| CRITICAL | GS001 | multi_lang.py | 48 | Found: "GS019" |
| CRITICAL | GS001 | multi_lang.py | 55 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 58 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 60 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 61 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 64 | Found: "GS002" |
| CRITICAL | GS001 | multi_lang.py | 65 | Found: "GS015" |
| CRITICAL | GS001 | multi_lang.py | 72 | Found: "GS001" |
| CRITICAL | GS001 | multi_lang.py | 76 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 78 | Found: "GS005" |
| CRITICAL | GS001 | multi_lang.py | 79 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 80 | Found: "GS004" |
| CRITICAL | GS001 | multi_lang.py | 84 | Found: "GS008" |
| CRITICAL | GS001 | multi_lang.py | 87 | Found: "GS019" |
| CRITICAL | GS001 | registry.py | 221 | Found: "GS024" |
| CRITICAL | GS001 | gsc_external.py | 52 | Found: "GS003" |
| CRITICAL | GS001 | gsc_external.py | 52 | Found: "GS008" |
| CRITICAL | GS001 | gsc_external.py | 52 | Found: "GS015" |
| CRITICAL | GS001 | gsc_external.py | 53 | Found: "GS007" |
| CRITICAL | GS001 | gsc_external.py | 53 | Found: "GS012" |
| CRITICAL | GS001 | gsc_external.py | 53 | Found: "GS013" |
| CRITICAL | GS001 | gsc_external.py | 53 | Found: "GS018" |
| CRITICAL | GS001 | gsc_external.py | 53 | Found: "GS019" |
| CRITICAL | GS001 | gsc_external.py | 53 | Found: "GS023" |
| CRITICAL | GS001 | gsc_external.py | 69 | Found: "GS003" |
| CRITICAL | GS001 | gsc_external.py | 69 | Found: "GS008" |
| CRITICAL | GS001 | gsc_external.py | 69 | Found: "GS015" |
| CRITICAL | GS001 | gsc_external.py | 69 | Found: "GS023" |
| CRITICAL | GS001 | gsc_external.py | 70 | Found: "GS007" |
| CRITICAL | GS001 | gsc_external.py | 70 | Found: "GS012" |
| CRITICAL | GS001 | gsc_external.py | 70 | Found: "GS013" |
| CRITICAL | GS001 | gsc_external.py | 70 | Found: "GS018" |
| CRITICAL | GS001 | gsc_external.py | 70 | Found: "GS019" |
| CRITICAL | GS001 | gsc_external.py | 101 | Found: "GS003" |
| CRITICAL | GS001 | gsc_external.py | 101 | Found: "GS008" |
| CRITICAL | GS001 | gsc_external.py | 101 | Found: "GS015" |
| CRITICAL | GS001 | gsc_external.py | 101 | Found: "GS023" |
| CRITICAL | GS001 | gsc_external.py | 102 | Found: "GS007" |
| CRITICAL | GS001 | gsc_external.py | 102 | Found: "GS012" |
| CRITICAL | GS001 | gsc_external.py | 102 | Found: "GS013" |
| CRITICAL | GS001 | gsc_external.py | 102 | Found: "GS018" |
| CRITICAL | GS001 | gsc_external.py | 102 | Found: "GS019" |
| CRITICAL | GS001 | gsc_external.py | 102 | Found: "GS021" |
| CRITICAL | GS001 | gsc_external.py | 102 | Found: "GS022" |
| CRITICAL | GS001 | gsc_external.py | 446 | Found: "GS001" |
| CRITICAL | GS001 | gsc_external.py | 448 | Found: "GS005" |
| CRITICAL | GS001 | gsc_external.py | 450 | Found: "GS020" |
| CRITICAL | GS001 | gsc_poc_generator.py | 36 | Found: "GS001" |
| CRITICAL | GS001 | gsc_poc_generator.py | 37 | Found: "GS003" |
| CRITICAL | GS001 | gsc_poc_generator.py | 38 | Found: "GS007" |
| CRITICAL | GS001 | gsc_poc_generator.py | 39 | Found: "GS012" |
| CRITICAL | GS001 | gsc_poc_generator.py | 40 | Found: "GS019" |
| CRITICAL | GS001 | gsc_poc_generator.py | 41 | Found: "GS022" |
| CRITICAL | GS001 | gsc_poc_generator.py | 42 | Found: "GS024" |
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
| CRITICAL | GS005 | gs020_llm_sqli.py | 122 | Line 122: - f-string with user-controlled input: cursor.exec |
| CRITICAL | GS005 | gs020_llm_sqli.py | 226 | Line 226: cursor.execute(f"SELECT * FROM users WHERE id = {u |
| CRITICAL | GS005 | gsc_metrics.py | 31 | Line 31: total = conn.execute(f"SELECT COUNT(*) FROM finding |
| CRITICAL | GS005 | gsc_metrics.py | 34 | Line 34: tp = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 40 | Line 40: fp = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 46 | Line 46: open_f = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 52 | Line 52: reval_total = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 74 | Line 74: det_rows = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 101 | Line 101: worst = conn.execute(f""" |
| CRITICAL | GS016 | gs016_linux_priv_esc.py | 31 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS024 | corpus_gs005_python.py | 8 | LLM confidence: 100%. The code uses f-strings, string format |
| CRITICAL | GS024 | corpus_gs005_python.py | 9 | LLM confidence: 100%. The code contains multiple SQL injecti |
| CRITICAL | GS024 | corpus_gs005_python.py | 15 | LLM confidence: 100%. All lines use unsafe string interpolat |
| CRITICAL | GS024 | gs020_llm_sqli.py | 226 | LLM confidence: 100%. The f-string directly interpolates use |
| CRITICAL | GS024 | gsc_metrics.py | 31 | LLM confidence: 100%. The f-string in line 28 directly inter |
| CRITICAL | GS024 | gsc_metrics.py | 34 | LLM confidence: 95%. The 'project' variable is interpolated  |
| HIGH | ? | gsc_issue.py | 74 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | fastapi_support.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | gs012_mass_assignment.py | 40 | Hacking APIs Ch.11 |
| HIGH | ? | gsc_vuln_spider.py | 47 | Redteam Kit |
| HIGH | ? | _cron_collect.py | 140 |  |
| HIGH | ? | gs011_jwt_vulnerabilities.py | 37 |  |
| HIGH | ? | gsc_collect_light.py | 211 |  |
| HIGH | ? | gsc_vuln_spider.py | 39 |  |
| HIGH | ? | gsc.py | 293 |  |
| HIGH | ? | gs005_sql_injection.py | 131 |  |
| HIGH | ? | _cron_collect.py | 47 |  |
| HIGH | ? | _cron_nvd.py | 45 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 23 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 36 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 37 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 91 |  |
| HIGH | ? | gs016_linux_priv_esc.py | 125 |  |
| HIGH | ? | gs014_credential_exposure.py | 25 |  |
| HIGH | ? | gs014_credential_exposure.py | 87 |  |
| HIGH | ? | gs014_credential_exposure.py | 88 |  |
| HIGH | ? | gs014_credential_exposure.py | 89 |  |
| HIGH | ? | gs014_credential_exposure.py | 90 |  |
| HIGH | ? | gs014_credential_exposure.py | 94 |  |
| HIGH | ? | gs014_credential_exposure.py | 95 |  |
| HIGH | ? | gsc_collect_light.py | 74 |  |
| HIGH | ? | gsc_issue.py | 74 |  |
| HIGH | ? | gsc_collect_light.py | 113 |  |
| HIGH | ? | gsc_collect_light.py | 126 |  |
| HIGH | ? | _cron_collect.py | 141 |  |
| HIGH | ? | gsc_collect_light.py | 212 |  |
| HIGH | ? | gsc_external.py | 168 | Match:     "standard default", "localhost", "loopback", "127 |
| HIGH | ? | gsc_external.py | 1275 | Match: RULES: localhost/127.0.0.1 defaults → false-positive. |
| HIGH | ? | bughunter.json | 45 | Match:     "fix": "Validate URL against allowlist. Block int |
| HIGH | ? | terraform.json | 3 | Match:   {"echelon": 2, "category": "HIGH", "title": "Terraf |
| HIGH | ? | docker.json | 6 | Match:   {"echelon": 2, "category": "MEDIUM", "title": "Dock |
| HIGH | ? | sso.yaml | 14 | Match:     http_address = "0.0.0.0:4180" |
| HIGH | ? | gsc.py | 1794 | Match:     api.add_argument('--host', default='127.0.0.1', h |
| HIGH | ? | gsc_api.py | 334 | Match:     p.add_argument("--host", default="127.0.0.1") |
| HIGH | ? | gs010_ssh_hardening.py | 81 | Match:                         references=["SSH Hardening &  |
| HIGH | ? | gsc_issue.py | 74 | Match:     r = requests.post(f"{jira_url}/rest/api/2/issue", |
| HIGH | ? | framework_aware.py | 21 | Match:     "eval() usage": { |
| HIGH | ? | framework_aware.py | 167 | Match:         {"title": "eval() usage", "category": "HIGH", |
| HIGH | ? | gsc.py | 697 | Match:             "Req 6": ["SQL injection", "eval()", "pic |
| HIGH | ? | gsc.py | 706 | Match:             "CC6.8": ["eval()", "pickle.load"], |
| HIGH | ? | gsc.py | 1256 | Match:         (2, "HIGH", "eval() or exec() usage", "regex" |
| HIGH | ? | gs004_dangerous_subprocess.py | 68 | Match:         "eval() with dynamic input — code injection", |
| HIGH | ? | gs004_dangerous_subprocess.py | 69 | Match:         "Never use eval() on user input. Use ast.lite |
| HIGH | ? | gs004_dangerous_subprocess.py | 74 | Match:         "exec() on variable — code injection risk", |
| HIGH | ? | gs004_dangerous_subprocess.py | 75 | Match:         "Avoid exec(); use explicit function calls or |
| HIGH | ? | gs020_xss_injection.py | 34 | Match:     (r'eval\s*\(\s*[\"\'`]', "DOM XSS: eval() with st |
| HIGH | ? | gsc_vuln_spider.py | 31 | Match:         ('"eval(" "request" language:python stars:<20 |
| HIGH | ? | gsc_pdf.py | 15 | Match:     os.system(f"python3 {os.path.dirname(__file__)}/g |
| HIGH | ? | gs004_dangerous_subprocess.py | 44 | Match:         "os.system() with .format() — command injecti |
| HIGH | ? | systemd.json | 23 | Match:     "title": "Systemd: User=root or absent → runs as  |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 50 | Line 50: "os.popen() — deprecated, uses shell", |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 56 | Line 56: "commands.getoutput() — deprecated shell wrapper", |
| HIGH | GS004 | gsc_pdf.py | 15 | Line 15: os.system(f"python3 {os.path.dirname(__file__)}/gsc |
| HIGH | GS005 | corpus_gs005_javascript.js | 20 | Line 20: db.collection.find({ $where: `this.name == '${req.q |
| HIGH | GS005 | corpus_gs005_javascript.js | 21 | Line 21: db.collection.find({ name: { $regex: req.params.sea |
| HIGH | GS005 | corpus_gs005_python.py | 46 | Line 46: pd.read_sql(f"SELECT * FROM sales WHERE region = '{ |
| HIGH | GS005 | corpus_gs005_python.py | 49 | Line 49: table.scan(FilterExpression=f"username = '{user}'") |
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
| HIGH | GS007 | gs007_idor.py | 97 | Line 97: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP-M |
| HIGH | GS007 | gs007_idor.py | 97 | Line 97: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP-M |
| HIGH | GS007 | gs007_idor.py | 97 | Line 97: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP-M |
| HIGH | GS012 | gs012_mass_assignment.py | 40 | Unpacking request body directly into model enables field inj |
| HIGH | GS014 | gsc_vuln_spider.py | 47 | Database URL contains password in plaintext. Use environment |
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
| C | ? | gs018_payment_abuse.py | 211 |
| C | ? | gs020_llm_sqli.py | 122 |
| C | ? | gs020_llm_sqli.py | 226 |
| M | ? | pre-commit | 22 |
| M | ? | gsc_doctor.py | 16 |
| M | ? | gsc_doctor.py | 33 |
| M | ? | framework_aware.py | 31 |
| M | ? | framework_aware.py | 165 |
| M | ? | gsc.py | 54 |
| M | ? | gsc.py | 1255 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| L | ? | gsc_external.py | 138 |
| L | ? | gs001_hardcoded_secret.py | 85 |
| L | ? | gs025_ai_provenance.py | 24 |
| C | ? | corpus_gs005_python.py | 11 |
| C | ? | corpus_gs005_python.py | 16 |
| C | ? | corpus_gs005_python.py | 24 |
| C | ? | corpus_gs005_python.py | 25 |
| H | ? | gsc_issue.py | 74 |
| H | ? | fastapi_support.py | 38 |
| H | ? | gs012_mass_assignment.py | 40 |
| H | ? | gsc_vuln_spider.py | 47 |
| M | ? | _cron_collect.py | 42 |
| M | ? | _cron_nvd.py | 40 |
| M | ? | gsc_collect_light.py | 69 |
| M | ? | gsc.py | 697 |
| M | ? | gsc.py | 706 |
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
| C | ? | gs020_llm_sqli.py | 122 |
| C | ? | gs020_llm_sqli.py | 226 |
| H | ? | _cron_collect.py | 140 |
| H | ? | gs011_jwt_vulnerabilities.py | 37 |
| H | ? | gsc_collect_light.py | 211 |
| H | ? | gsc_vuln_spider.py | 39 |
| H | ? | gsc.py | 293 |
| H | ? | gs005_sql_injection.py | 131 |
| H | ? | _cron_collect.py | 47 |
| H | ? | _cron_nvd.py | 45 |
| H | ? | gs016_linux_priv_esc.py | 23 |
| H | ? | gs016_linux_priv_esc.py | 36 |
| H | ? | gs016_linux_priv_esc.py | 37 |
| H | ? | gs016_linux_priv_esc.py | 91 |
| H | ? | gs016_linux_priv_esc.py | 125 |
| H | ? | gs014_credential_exposure.py | 25 |
| H | ? | gs014_credential_exposure.py | 87 |
| H | ? | gs014_credential_exposure.py | 88 |
| H | ? | gs014_credential_exposure.py | 89 |
| H | ? | gs014_credential_exposure.py | 90 |
| H | ? | gs014_credential_exposure.py | 94 |
| H | ? | gs014_credential_exposure.py | 95 |
| H | ? | gsc_collect_light.py | 74 |
| H | ? | gsc_issue.py | 74 |
| H | ? | gsc_collect_light.py | 113 |
| H | ? | gsc_collect_light.py | 126 |
| M | ? | corpus_gs005_python.py | 39 |
| M | ? | _cron_collect.py | 33 |
| M | ? | _cron_nvd.py | 31 |
| M | ? | multi_lang.py | 41 |
| M | ? | multi_lang.py | 42 |
| M | ? | gs020_xss_injection.py | 29 |
| M | ? | gs020_xss_injection.py | 32 |
| M | ? | gs020_xss_injection.py | 46 |
| M | ? | gsc_collect_light.py | 60 |
| C | ? | _cron_collect.py | 141 |
| C | ? | gsc_pdf.py | 15 |
| C | ? | gsc.py | 1258 |
| C | ? | gs004_dangerous_subprocess.py | 34 |
| C | ? | gs004_dangerous_subprocess.py | 39 |
| C | ? | gs004_dangerous_subprocess.py | 44 |
| C | ? | gs004_dangerous_subprocess.py | 111 |
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
| C | GS001 | manifest.json | 249 |
| C | GS001 | manifest.json | 250 |
| C | GS001 | manifest.json | 289 |
| C | GS001 | manifest.json | 290 |
| C | GS001 | manifest.json | 339 |
| C | GS001 | manifest.json | 340 |
| C | GS001 | manifest.json | 344 |
| C | GS001 | manifest.json | 345 |
| C | GS001 | gsc_chain_composer.py | 22 |
| C | GS001 | gsc_chain_composer.py | 22 |
| C | GS001 | gsc_chain_composer.py | 22 |
| C | GS001 | gsc_chain_composer.py | 23 |
| C | GS001 | gsc_chain_composer.py | 23 |
| C | GS001 | gsc_chain_composer.py | 24 |
| C | GS001 | gsc_chain_composer.py | 25 |
| C | GS001 | gsc_chain_composer.py | 25 |
| C | GS001 | gsc_chain_composer.py | 26 |
| C | GS001 | gsc_chain_composer.py | 26 |
| C | GS001 | gsc_chain_composer.py | 27 |
| C | GS001 | gsc_chain_composer.py | 28 |
| C | GS001 | gsc_chain_composer.py | 34 |
| C | GS001 | gsc_chain_composer.py | 34 |
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
| C | GS001 | gs001_hardcoded_secret.py | 16 |
| C | GS001 | gs001_hardcoded_secret.py | 94 |
| C | GS001 | gs002_world_readable.py | 14 |
| C | GS001 | gs002_world_readable.py | 41 |
| C | GS001 | gs003_debug_prints.py | 13 |
| C | GS001 | gs003_debug_prints.py | 54 |
| C | GS001 | gs004_dangerous_subprocess.py | 17 |
| C | GS001 | gs004_dangerous_subprocess.py | 82 |
| C | GS001 | gs005_sql_injection.py | 28 |
| C | GS001 | gs007_idor.py | 21 |
| C | GS001 | gs007_idor.py | 149 |
| C | GS001 | gs008_dead_code.py | 19 |
| C | GS001 | gs008_dead_code.py | 69 |
| C | GS001 | gs009_supply_chain.py | 20 |
| C | GS001 | gs010_ssh_hardening.py | 20 |
| C | GS001 | gs010_ssh_hardening.py | 26 |
| C | GS001 | gs011_jwt_vulnerabilities.py | 18 |
| C | GS001 | gs011_jwt_vulnerabilities.py | 52 |
| C | GS001 | gs012_mass_assignment.py | 18 |
| C | GS001 | gs012_mass_assignment.py | 78 |
| C | GS001 | gs013_graphql_security.py | 19 |
| C | GS001 | gs013_graphql_security.py | 85 |
| C | GS001 | gs014_credential_exposure.py | 23 |
| C | GS001 | gs014_credential_exposure.py | 109 |
| C | GS001 | gs015_entry_points.py | 15 |
| C | GS001 | gs015_entry_points.py | 83 |
| C | GS001 | gs016_linux_priv_esc.py | 20 |
| C | GS001 | gs017_weak_passwords.py | 19 |
| C | GS001 | gs017_weak_passwords.py | 105 |
| C | GS001 | gs018_payment_abuse.py | 24 |
| C | GS001 | gs018_payment_abuse.py | 133 |
| C | GS001 | gs019_auth_session.py | 25 |
| C | GS001 | gs019_auth_session.py | 169 |
| C | GS001 | gs020_llm_sqli.py | 22 |
| C | GS001 | gs020_xss_injection.py | 20 |
| C | GS001 | gs021_csrf_ssrf.py | 18 |
| C | GS001 | gs022_open_redirect.py | 19 |
| C | GS001 | gs023_race_conditions.py | 20 |
| C | GS001 | gs025_ai_provenance.py | 64 |
| C | GS001 | gs025_ai_provenance.py | 121 |
| C | GS001 | gs028_invariants.py | 17 |
| C | GS001 | multi_lang.py | 17 |
| C | GS001 | multi_lang.py | 18 |
| C | GS001 | multi_lang.py | 21 |
| C | GS001 | multi_lang.py | 22 |
| C | GS001 | multi_lang.py | 24 |
| C | GS001 | multi_lang.py | 27 |
| C | GS001 | multi_lang.py | 28 |
| C | GS001 | multi_lang.py | 35 |
| C | GS001 | multi_lang.py | 37 |
| C | GS001 | multi_lang.py | 40 |
| C | GS001 | multi_lang.py | 42 |
| C | GS001 | multi_lang.py | 43 |
| C | GS001 | multi_lang.py | 44 |
| C | GS001 | multi_lang.py | 47 |
| C | GS001 | multi_lang.py | 48 |
| C | GS001 | multi_lang.py | 55 |
| C | GS001 | multi_lang.py | 58 |
| C | GS001 | multi_lang.py | 60 |
| C | GS001 | multi_lang.py | 61 |
| C | GS001 | multi_lang.py | 64 |
| C | GS001 | multi_lang.py | 65 |
| C | GS001 | multi_lang.py | 72 |
| C | GS001 | multi_lang.py | 76 |
| C | GS001 | multi_lang.py | 78 |
| C | GS001 | multi_lang.py | 79 |
| C | GS001 | multi_lang.py | 80 |
| C | GS001 | multi_lang.py | 84 |
| C | GS001 | multi_lang.py | 87 |
| C | GS001 | registry.py | 221 |
| C | GS001 | gsc_external.py | 52 |
| C | GS001 | gsc_external.py | 52 |
| C | GS001 | gsc_external.py | 52 |
| C | GS001 | gsc_external.py | 53 |
| C | GS001 | gsc_external.py | 53 |
| C | GS001 | gsc_external.py | 53 |
| C | GS001 | gsc_external.py | 53 |
| C | GS001 | gsc_external.py | 53 |
| C | GS001 | gsc_external.py | 53 |
| C | GS001 | gsc_external.py | 69 |
| C | GS001 | gsc_external.py | 69 |
| C | GS001 | gsc_external.py | 69 |
| C | GS001 | gsc_external.py | 69 |
| C | GS001 | gsc_external.py | 70 |
| C | GS001 | gsc_external.py | 70 |
| C | GS001 | gsc_external.py | 70 |
| C | GS001 | gsc_external.py | 70 |
| C | GS001 | gsc_external.py | 70 |
| C | GS001 | gsc_external.py | 101 |
| C | GS001 | gsc_external.py | 101 |
| C | GS001 | gsc_external.py | 101 |
| C | GS001 | gsc_external.py | 101 |
| C | GS001 | gsc_external.py | 102 |
| C | GS001 | gsc_external.py | 102 |
| C | GS001 | gsc_external.py | 102 |
| C | GS001 | gsc_external.py | 102 |
| C | GS001 | gsc_external.py | 102 |
| C | GS001 | gsc_external.py | 102 |
| C | GS001 | gsc_external.py | 102 |
| C | GS001 | gsc_external.py | 446 |
| C | GS001 | gsc_external.py | 448 |
| C | GS001 | gsc_external.py | 450 |
| C | GS001 | gsc_poc_generator.py | 36 |
| C | GS001 | gsc_poc_generator.py | 37 |
| C | GS001 | gsc_poc_generator.py | 38 |
| C | GS001 | gsc_poc_generator.py | 39 |
| C | GS001 | gsc_poc_generator.py | 40 |
| C | GS001 | gsc_poc_generator.py | 41 |
| C | GS001 | gsc_poc_generator.py | 42 |
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
| L | GS003 | django_cross_org.py | 33 |
| L | GS003 | gsc.py | 75 |
| L | GS003 | gsc.py | 80 |
| L | GS003 | gsc.py | 81 |
| L | GS003 | gsc.py | 82 |
| L | GS003 | gsc.py | 89 |
| L | GS003 | gsc.py | 140 |
| L | GS003 | gsc.py | 143 |
| L | GS003 | gsc.py | 164 |
| L | GS003 | gsc.py | 166 |
| L | GS003 | gsc.py | 603 |
| L | GS003 | gsc.py | 718 |
| L | GS003 | gsc.py | 720 |
| L | GS003 | gsc.py | 723 |
| L | GS003 | gsc.py | 731 |
| L | GS003 | gsc.py | 734 |
| L | GS003 | gsc.py | 737 |
| L | GS003 | gsc.py | 739 |
| L | GS003 | gsc.py | 773 |
| L | GS003 | gsc.py | 801 |
| L | GS003 | gsc.py | 885 |
| L | GS003 | gsc.py | 927 |
| L | GS003 | gsc.py | 929 |
| L | GS003 | gsc.py | 930 |
| L | GS003 | gsc.py | 931 |
| L | GS003 | gsc.py | 932 |
| L | GS003 | gsc.py | 933 |
| L | GS003 | gsc.py | 936 |
| L | GS003 | gsc.py | 938 |
| L | GS003 | gsc.py | 1008 |
| L | GS003 | gsc.py | 1009 |
| L | GS003 | gsc.py | 1013 |
| L | GS003 | gsc.py | 1128 |
| L | GS003 | gsc.py | 1199 |
| L | GS003 | gsc.py | 1222 |
| L | GS003 | gsc.py | 1282 |
| L | GS003 | gsc.py | 1293 |
| L | GS003 | gsc.py | 1294 |
| L | GS003 | gsc.py | 1302 |
| L | GS003 | gsc.py | 1310 |
| L | GS003 | gsc.py | 1312 |
| L | GS003 | gsc.py | 1326 |
| L | GS003 | gsc.py | 1338 |
| L | GS003 | gsc.py | 1339 |
| L | GS003 | gsc.py | 1341 |
| L | GS003 | gsc.py | 1354 |
| L | GS003 | gsc.py | 1356 |
| L | GS003 | gsc.py | 1386 |
| L | GS003 | gsc.py | 1387 |
| L | GS003 | gsc.py | 1394 |
| L | GS003 | gsc.py | 1401 |
| L | GS003 | gsc.py | 1411 |
| L | GS003 | gsc.py | 1418 |
| L | GS003 | gsc.py | 1439 |
| L | GS003 | gsc.py | 1449 |
| L | GS003 | gsc.py | 1452 |
| L | GS003 | gsc.py | 1470 |
| L | GS003 | gsc.py | 1476 |
| L | GS003 | gsc.py | 1487 |
| L | GS003 | gsc.py | 1498 |
| L | GS003 | gsc.py | 1502 |
| L | GS003 | gsc.py | 1503 |
| L | GS003 | gsc.py | 1504 |
| L | GS003 | gsc.py | 1505 |
| L | GS003 | gsc.py | 1507 |
| L | GS003 | gsc.py | 1514 |
| L | GS003 | gsc.py | 1521 |
| L | GS003 | gsc.py | 1531 |
| L | GS003 | gsc.py | 1540 |
| L | GS003 | gsc.py | 1542 |
| L | GS003 | gsc.py | 1543 |
| L | GS003 | gsc.py | 1583 |
| L | GS003 | gsc.py | 1611 |
| L | GS003 | gsc.py | 1613 |
| L | GS003 | gsc.py | 1616 |
| L | GS003 | gsc.py | 1644 |
| L | GS003 | gsc.py | 1647 |
| L | GS003 | gsc.py | 1649 |
| L | GS003 | gsc.py | 1650 |
| L | GS003 | gsc.py | 1660 |
| L | GS003 | gsc.py | 1665 |
| L | GS003 | gsc.py | 1668 |
| L | GS003 | gsc.py | 1682 |
| L | GS003 | gsc.py | 1684 |
| L | GS003 | gsc.py | 1685 |
| L | GS003 | gsc.py | 1686 |
| L | GS003 | gsc.py | 1690 |
| L | GS003 | gsc.py | 1907 |
| L | GS003 | gsc.py | 1908 |
| L | GS003 | gsc.py | 1950 |
| L | GS003 | gsc.py | 1955 |
| L | GS003 | gsc.py | 1957 |
| L | GS003 | gsc.py | 1963 |
| L | GS003 | gsc.py | 1966 |
| L | GS003 | gsc_api.py | 30 |
| L | GS003 | gsc_api.py | 336 |
| L | GS003 | gsc_api.py | 338 |
| L | GS003 | gsc_api.py | 339 |
| L | GS003 | gsc_chain_composer.py | 84 |
| L | GS003 | gsc_chain_composer.py | 91 |
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
| L | GS003 | gsc_db.py | 139 |
| L | GS003 | multi_lang.py | 184 |
| L | GS003 | multi_lang.py | 190 |
| L | GS003 | multi_lang.py | 192 |
| L | GS003 | multi_lang.py | 194 |
| L | GS003 | multi_lang.py | 196 |
| L | GS003 | gsc_external.py | 952 |
| L | GS003 | gsc_external.py | 960 |
| L | GS003 | gsc_external.py | 988 |
| L | GS003 | gsc_external.py | 990 |
| L | GS003 | gsc_external.py | 991 |
| L | GS003 | gsc_external.py | 994 |
| L | GS003 | gsc_external.py | 1009 |
| L | GS003 | gsc_external.py | 1015 |
| L | GS003 | gsc_external.py | 1046 |
| L | GS003 | gsc_external.py | 1075 |
| L | GS003 | gsc_external.py | 1081 |
| L | GS003 | gsc_external.py | 1091 |
| L | GS003 | gsc_external.py | 1112 |
| L | GS003 | gsc_external.py | 1129 |
| L | GS003 | gsc_external.py | 1131 |
| L | GS003 | gsc_external.py | 1152 |
| L | GS003 | gsc_external.py | 1158 |
| L | GS003 | gsc_external.py | 1161 |
| L | GS003 | gsc_external.py | 1166 |
| L | GS003 | gsc_external.py | 1168 |
| L | GS003 | gsc_external.py | 1177 |
| L | GS003 | gsc_external.py | 1352 |
| L | GS003 | gsc_external.py | 1356 |
| L | GS003 | gsc_external.py | 1362 |
| L | GS003 | gsc_external.py | 1363 |
| L | GS003 | gsc_external.py | 1366 |
| L | GS003 | gsc_external.py | 1368 |
| L | GS003 | gsc_external.py | 1370 |
| L | GS003 | gsc_external.py | 1375 |
| L | GS003 | gsc_external.py | 1395 |
| L | GS003 | gsc_external.py | 1397 |
| L | GS003 | gsc_external.py | 1417 |
| L | GS003 | gsc_github_adapter.py | 72 |
| L | GS003 | gsc_github_adapter.py | 94 |
| L | GS003 | gsc_github_adapter.py | 251 |
| L | GS003 | gsc_github_adapter.py | 252 |
| L | GS003 | gsc_github_adapter.py | 263 |
| L | GS003 | gsc_github_adapter.py | 272 |
| L | GS003 | gsc_github_adapter.py | 274 |
| L | GS003 | gsc_github_adapter.py | 276 |
| L | GS003 | gsc_github_adapter.py | 299 |
| L | GS003 | gsc_github_adapter.py | 302 |
| L | GS003 | gsc_github_adapter.py | 318 |
| L | GS003 | gsc_github_adapter.py | 320 |
| L | GS003 | gsc_github_adapter.py | 322 |
| L | GS003 | gsc_github_adapter.py | 425 |
| L | GS003 | gsc_github_adapter.py | 426 |
| L | GS003 | gsc_github_adapter.py | 429 |
| L | GS003 | gsc_github_adapter.py | 430 |
| L | GS003 | gsc_github_adapter.py | 431 |
| L | GS003 | gsc_github_adapter.py | 432 |
| L | GS003 | gsc_github_adapter.py | 433 |
| L | GS003 | gsc_github_adapter.py | 434 |
| L | GS003 | gsc_github_adapter.py | 435 |
| L | GS003 | gsc_github_adapter.py | 436 |
| L | GS003 | gsc_github_adapter.py | 438 |
| L | GS003 | gsc_github_adapter.py | 440 |
| L | GS003 | gsc_github_adapter.py | 441 |
| L | GS003 | gsc_github_adapter.py | 469 |
| L | GS003 | gsc_github_adapter.py | 471 |
| L | GS003 | gsc_github_adapter.py | 472 |
| L | GS003 | gsc_github_adapter.py | 486 |
| L | GS003 | gsc_github_adapter.py | 523 |
| L | GS003 | gsc_github_adapter.py | 528 |
| L | GS003 | gsc_github_adapter.py | 553 |
| L | GS003 | gsc_github_adapter.py | 671 |
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
| L | GS003 | gsc_poc_generator.py | 73 |
| L | GS003 | gsc_poc_generator.py | 81 |
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
| L | GS003 | gsc_report.py | 10 |
| L | GS003 | gsc_report.py | 73 |
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
| L | GS008 | batch_and_override.py | 39 |
| L | GS008 | gsc.py | 40 |
| L | GS008 | gsc.py | 53 |
| L | GS008 | gsc_chain_composer.py | 19 |
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
| L | GS008 | gs001_hardcoded_secret.py | 17 |
| L | GS008 | gs002_world_readable.py | 15 |
| L | GS008 | gs003_debug_prints.py | 14 |
| L | GS008 | gs004_dangerous_subprocess.py | 18 |
| L | GS008 | gs005_sql_injection.py | 29 |
| L | GS008 | gs005_sql_injection.py | 30 |
| L | GS008 | gs005_sql_injection.py | 59 |
| L | GS008 | gs007_idor.py | 22 |
| L | GS008 | gs007_idor.py | 23 |
| L | GS008 | gs008_dead_code.py | 20 |
| L | GS008 | gs009_supply_chain.py | 22 |
| L | GS008 | gs010_ssh_hardening.py | 21 |
| L | GS008 | gs011_jwt_vulnerabilities.py | 19 |
| L | GS008 | gs012_mass_assignment.py | 19 |
| L | GS008 | gs013_graphql_security.py | 20 |
| L | GS008 | gs014_credential_exposure.py | 24 |
| L | GS008 | gs015_entry_points.py | 16 |
| L | GS008 | gs016_linux_priv_esc.py | 21 |
| L | GS008 | gs016_linux_priv_esc.py | 22 |
| L | GS008 | gs017_weak_passwords.py | 20 |
| L | GS008 | gs017_weak_passwords.py | 21 |
| L | GS008 | gs018_payment_abuse.py | 25 |
| L | GS008 | gs018_payment_abuse.py | 26 |
| L | GS008 | gs018_payment_abuse.py | 35 |
| L | GS008 | gs018_payment_abuse.py | 50 |
| L | GS008 | gs018_payment_abuse.py | 57 |
| L | GS008 | gs018_payment_abuse.py | 77 |
| L | GS008 | gs018_payment_abuse.py | 93 |
| L | GS008 | gs018_payment_abuse.py | 105 |
| L | GS008 | gs018_payment_abuse.py | 114 |
| L | GS008 | gs019_auth_session.py | 26 |
| L | GS008 | gs019_auth_session.py | 27 |
| L | GS008 | gs019_auth_session.py | 42 |
| L | GS008 | gs019_auth_session.py | 55 |
| L | GS008 | gs019_auth_session.py | 64 |
| L | GS008 | gs019_auth_session.py | 83 |
| L | GS008 | gs019_auth_session.py | 107 |
| L | GS008 | gs019_auth_session.py | 135 |
| L | GS008 | gs020_llm_sqli.py | 24 |
| L | GS008 | gs020_llm_sqli.py | 25 |
| L | GS008 | gs020_xss_injection.py | 22 |
| L | GS008 | gs021_csrf_ssrf.py | 20 |
| L | GS008 | gs022_open_redirect.py | 21 |
| L | GS008 | gs023_race_conditions.py | 22 |
| L | GS008 | gs025_ai_provenance.py | 121 |
| L | GS008 | gs025_ai_provenance.py | 122 |
| L | GS008 | gs025_ai_provenance.py | 123 |
| L | GS008 | registry.py | 235 |
| L | GS008 | registry.py | 236 |
| L | GS008 | gsc_github_adapter.py | 30 |
| i | GS020 |  | 122 |
| i | GS020 |  | 41 |
| i | GS020 |  | 42 |
| i | GS020 |  | 6 |
| i | GS020 |  | 30 |
| i | GS020 |  | 30 |
| i | GS020 |  | 32 |
| i | GS020 |  | 41 |
| i | GS020 |  | 61 |
| i | GS020 |  | 61 |
| i | GS020 |  | 61 |
| i | GS020 |  | 31 |
| i | GS020 |  | 135 |
| i | GS020 |  | 184 |
| i | GS020 |  | 192 |
| i | GS020 |  | 267 |
| H | ? | gsc_external.py | 168 |
| H | ? | gsc_external.py | 1275 |
| H | ? | bughunter.json | 45 |
| H | ? | terraform.json | 3 |
| H | ? | docker.json | 6 |
| H | ? | sso.yaml | 14 |
| H | ? | gsc.py | 1794 |
| H | ? | gsc_api.py | 334 |
| H | ? | gs010_ssh_hardening.py | 81 |
| H | ? | gsc_issue.py | 74 |
| H | ? | framework_aware.py | 21 |
| H | ? | framework_aware.py | 167 |
| H | ? | gsc.py | 697 |
| H | ? | gsc.py | 706 |
| H | ? | gsc.py | 1256 |
| H | ? | gs004_dangerous_subprocess.py | 68 |
| H | ? | gs004_dangerous_subprocess.py | 69 |
| H | ? | gs004_dangerous_subprocess.py | 74 |
| H | ? | gs004_dangerous_subprocess.py | 75 |
| H | ? | gs020_xss_injection.py | 34 |
| H | ? | gsc_vuln_spider.py | 31 |
| H | ? | gsc_pdf.py | 15 |
| H | ? | gs004_dangerous_subprocess.py | 44 |
| M | ? | systemd.json | 18 |
| M | ? | systemd.json | 19 |
| H | ? | systemd.json | 23 |
| M | ? | systemd.json | 63 |
| M | ? | systemd.json | 68 |
| C | ? | systemd.json | 78 |
| H | GS004 | gs004_dangerous_subprocess.py | 50 |
| H | GS004 | gs004_dangerous_subprocess.py | 56 |
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
| C | GS005 | gs020_llm_sqli.py | 122 |
| C | GS005 | gs020_llm_sqli.py | 226 |
| C | GS005 | gsc_metrics.py | 31 |
| C | GS005 | gsc_metrics.py | 34 |
| C | GS005 | gsc_metrics.py | 40 |
| C | GS005 | gsc_metrics.py | 46 |
| C | GS005 | gsc_metrics.py | 52 |
| C | GS005 | gsc_metrics.py | 74 |
| C | GS005 | gsc_metrics.py | 101 |
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
| I | GS007 | gsc_db.py | 45 |
| I | GS007 | gs007_idor.py | 50 |
| I | GS007 | gs007_idor.py | 50 |
| I | GS007 | gs007_idor.py | 52 |
| I | GS007 | gs007_idor.py | 52 |
| I | GS007 | gs007_idor.py | 52 |
| I | GS007 | gs007_idor.py | 181 |
| H | GS007 | gs007_idor.py | 97 |
| H | GS007 | gs007_idor.py | 97 |
| H | GS007 | gs007_idor.py | 97 |
| s | GS009 |  | 0 |
| H | GS012 | gs012_mass_assignment.py | 40 |
| M | GS012 | gsc_issue.py | 90 |
| H | GS014 | gsc_vuln_spider.py | 47 |
| C | GS016 | gs016_linux_priv_esc.py | 31 |
| M | GS019 | gs021_csrf_ssrf.py | 33 |
| s | GS021 |  | 77 |
| s | GS021 |  | 168 |
| s | GS021 |  | 168 |
| s | GS021 |  | 1275 |
| s | GS021 |  | 1275 |
| s | GS021 |  | 67 |
| s | GS021 |  | 1008 |
| s | GS021 |  | 1794 |
| s | GS021 |  | 1794 |
| s | GS021 |  | 334 |
| c | GS021 |  | 27 |
| c | GS021 |  | 27 |
| c | GS021 |  | 35 |
| c | GS021 |  | 37 |
| s | GS021 |  | 49 |
| s | GS021 |  | 49 |
| s | GS021 |  | 6 |
| s | GS021 |  | 51 |
| s | GS021 |  | 51 |
| r | GS022 |  | 138 |
| r | GS022 |  | 660 |
| r | GS022 |  | 30 |
| r | GS022 |  | 41 |
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
| C | GS024 | gs020_llm_sqli.py | 226 |
| C | GS024 | gsc_metrics.py | 31 |
| C | GS024 | gsc_metrics.py | 34 |
| M | ? | gsc_external.py | 724 |
| M | ? | gsc_external.py | 729 |
| M | ? | gsc_external.py | 754 |
| M | ? | gsc_external.py | 756 |
| M | ? | gsc_external.py | 767 |
| M | ? | gsc_external.py | 786 |
| M | ? | gsc_external.py | 788 |
| M | ? | gsc_external.py | 908 |
| M | ? | gsc_external.py | 912 |
| M | ? | gsc_external.py | 941 |
| M | ? | gsc_external.py | 947 |
| M | ? | gsc_external.py | 954 |
| M | ? | gsc_external.py | 997 |
| M | ? | bughunter.json | 32 |
| M | ? | bughunter.json | 33 |
| M | ? | python_async.json | 42 |
| M | ? | python_async.json | 53 |
| M | ? | python_async.json | 74 |
| M | ? | python_async.json | 75 |
| M | ? | gsc_github_dorks.py | 94 |
| M | ? | gsc_pr_scanner.py | 46 |
| M | ? | gsc_pr_scanner.py | 117 |
| M | ? | gsc_calibration.py | 131 |
| M | ? | gsc_calibration.py | 134 |
| M | ? | gsc_doctor.py | 21 |
| M | ? | gsc_doctor.py | 31 |
| M | ? | e4_llm.py | 307 |
| M | ? | gsc_github_adapter.py | 480 |
| M | ? | gsc_github_adapter.py | 481 |
| M | ? | gsc_github_adapter.py | 503 |
| M | ? | gsc_github_adapter.py | 557 |
| M | ? | gsc_revalidate.py | 74 |
| M | ? | gsc_revalidate.py | 87 |
| M | ? | gsc.py | 88 |
| M | ? | gsc.py | 396 |
| M | ? | gsc.py | 439 |
| M | ? | gsc.py | 556 |
| M | ? | gsc.py | 1189 |
| M | ? | gsc.py | 1191 |
| M | ? | gsc.py | 1193 |
| M | ? | gsc.py | 1870 |
| M | ? | gsc.py | 1873 |
| M | ? | gsc.py | 1876 |
| M | ? | gsc.py | 1889 |
| M | ? | gsc.py | 1891 |
| M | ? | gsc.py | 1898 |
| M | ? | gsc.py | 1902 |
| M | ? | gsc.py | 1927 |
| M | ? | gsc.py | 1930 |
| M | ? | gsc.py | 1940 |
| M | ? | gs009_supply_chain.py | 75 |
| M | ? | gs004_dangerous_subprocess.py | 35 |
| M | ? | gs004_dangerous_subprocess.py | 40 |
| M | ? | gs004_dangerous_subprocess.py | 45 |
| M | ? | gs004_dangerous_subprocess.py | 57 |
| M | ? | go.json | 9 |
| H | ? | rust.json | 7 |

---
*Сгенерировано GSC v0.6 · 2026-08-05T14:11:42.003561*