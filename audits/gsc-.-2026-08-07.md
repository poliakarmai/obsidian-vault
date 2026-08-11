---
title: "GSC Audit: ."
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — .

**Дата:** 07.08.2026 14:48  
**Путь:** `/home/openclaw/gsc`  
**Всего находок:** 1542  
**CRITICAL:** 410 | **HIGH:** 109 | **MEDIUM:** 142 | **LOW:** 736

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 486 |
| GS001 | 279 |
| GS000-LEGACY | 225 |
| GS005 | 103 |
| Синхронный код в async | 93 |
| GS008 | 85 |
| GS007 | 70 |
| GS025 | 43 |
| GS021 | 33 |
| GS020 | 28 |
| GS025-eval_usage | 22 |
| GS010 | 18 |
| GS022 | 15 |
| GS029 | 8 |
| GS025-hardcoded_secret | 7 |
| GS024 | 7 |
| GS004 | 4 |
| GS014 | 4 |
| GS012 | 2 |
| GS019 | 2 |
| GS018 | 1 |
| GS031 | 1 |
| GS009 | 1 |
| GS016 | 1 |
| GS017 | 1 |
| GS025-debug_mode | 1 |
| Go: sync.Mutex copy | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | gsc_metrics.py | 31 | OWASP A03: Injection |
| CRITICAL | GS005 | gsc_setup_calibration.py | 8 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 8 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 12 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 15 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 19 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 20 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 23 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 28 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 31 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 37 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 39 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 43 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 46 | OWASP A03: Injection |
| CRITICAL | GS005 | gs018_payment_abuse.py | 215 | OWASP A03: Injection |
| CRITICAL | GS005 | gs020_llm_sqli.py | 126 | OWASP A03: Injection |
| CRITICAL | GS005 | gs020_llm_sqli.py | 230 | OWASP A03: Injection |
| CRITICAL | GS005 | corpus_gs005_python.py | 11 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | corpus_gs005_python.py | 16 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | corpus_gs005_python.py | 24 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | corpus_gs005_python.py | 25 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | gsc_epss.py | 97 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | gsc_metrics.py | 31 |  |
| CRITICAL | GS005 | gsc_setup_calibration.py | 8 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 8 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 12 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 15 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 19 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 20 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 23 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 28 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 31 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 37 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 39 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 43 |  |
| CRITICAL | GS005 | corpus_gs005_python.py | 46 |  |
| CRITICAL | GS005 | gs020_llm_sqli.py | 126 |  |
| CRITICAL | GS005 | gs020_llm_sqli.py | 230 |  |
| CRITICAL | GS025 | _cron_collect.py | 141 |  |
| CRITICAL | GS025 | gsc_pdf.py | 15 |  |
| CRITICAL | GS025 | gsc.py | 1308 |  |
| CRITICAL | GS025 | gsc_proofoffix.py | 447 |  |
| CRITICAL | GS025 | gs004_dangerous_subprocess.py | 38 |  |
| CRITICAL | GS025 | gs004_dangerous_subprocess.py | 43 |  |
| CRITICAL | GS025 | gs004_dangerous_subprocess.py | 48 |  |
| CRITICAL | GS025 | gs004_dangerous_subprocess.py | 115 |  |
| CRITICAL | GS025 | gsc_collect_light.py | 212 |  |
| CRITICAL | GS025 | gsc_vuln_spider.py | 29 |  |
| CRITICAL | GS025 | gsc_vuln_spider.py | 187 |  |
| CRITICAL | GS000-LEGACY | _cron_collect.py | 139 |  |
| CRITICAL | GS000-LEGACY | gsc_collect_light.py | 210 |  |
| CRITICAL | GS000-LEGACY | _cron_collect.py | 140 |  |
| CRITICAL | GS000-LEGACY | gsc_collect_light.py | 211 |  |
| CRITICAL | GS000-LEGACY | gsc_vuln_spider.py | 39 |  |
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
| CRITICAL | GS001 | cwe_map.py | 28 | Found: "GS004" |
| CRITICAL | GS001 | click.json | 9 | Found: "GS001" |
| CRITICAL | GS001 | flask-jwt-auth.json | 7 | Found: "GS011" |
| CRITICAL | GS001 | flask-jwt-auth.json | 8 | Found: "GS019" |
| CRITICAL | GS001 | main.tf | 5 | Found: access_key = "AKIAIOSFODNN7EXAMPLE" |
| CRITICAL | GS001 | main.tf | 5 | Found: AKIAIOSFODNN7EXAMPLE |
| CRITICAL | GS001 | config.py | 2 | Found: AKIAIOSFODNN7EXAMPLE |
| CRITICAL | GS001 | config.py | 3 | Found: DATABASE_URL = "mysql://admin:secret@localhost/db" |
| CRITICAL | GS001 | github_auth.py | 40 | Found: "RS256" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS019" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS029" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS001" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS005" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS030" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS031" |
| CRITICAL | GS001 | compliance.py | 5 | Found: "GS028" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS001" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS005" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS017" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS019" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS029" |
| CRITICAL | GS001 | compliance.py | 6 | Found: "GS030" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS030" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS031" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS028" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS019" |
| CRITICAL | GS001 | compliance.py | 7 | Found: "GS029" |
| CRITICAL | GS001 | manifest.json | 249 | Found: "bb0744740ba2e343a19f4d77f388842a" |
| CRITICAL | GS001 | manifest.json | 250 | Found: "bb0744740ba2e343a19f4d77f388842a" |
| CRITICAL | GS001 | manifest.json | 289 | Found: "dd648e75e997d21b11471747b746a2f0" |
| CRITICAL | GS001 | manifest.json | 290 | Found: "dd648e75e997d21b11471747b746a2f0" |
| CRITICAL | GS001 | manifest.json | 339 | Found: "cc350016c2c90504944929ddcae40500" |
| CRITICAL | GS001 | manifest.json | 340 | Found: "cc350016c2c90504944929ddcae40500" |
| CRITICAL | GS001 | manifest.json | 344 | Found: "df82b30c519a4adb8fa80b6fd3b3990f" |
| CRITICAL | GS001 | manifest.json | 345 | Found: "df82b30c519a4adb8fa80b6fd3b3990f" |
| CRITICAL | GS001 | tsconfig.json | 4 | Found: "ES2022" |
| CRITICAL | GS001 | gsc.py | 401 | Found: "GS005" |
| CRITICAL | GS001 | gsc.py | 402 | Found: "GS020" |
| CRITICAL | GS001 | gsc.py | 403 | Found: "GS029" |
| CRITICAL | GS001 | gsc.py | 404 | Found: "GS008" |
| CRITICAL | GS001 | gsc.py | 405 | Found: "GS007" |
| CRITICAL | GS001 | gsc.py | 406 | Found: "GS010" |
| CRITICAL | GS001 | gsc.py | 407 | Found: "GS018" |
| CRITICAL | GS001 | gsc.py | 408 | Found: "GS031" |
| CRITICAL | GS001 | gsc.py | 409 | Found: "GS025" |
| CRITICAL | GS001 | gsc.py | 410 | Found: "GS025" |
| CRITICAL | GS001 | gsc.py | 415 | Found: "GS025" |
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
| CRITICAL | GS001 | gsc_compliance.py | 18 | Found: "GS001" |
| CRITICAL | GS001 | gsc_compliance.py | 19 | Found: "GS003" |
| CRITICAL | GS001 | gsc_compliance.py | 20 | Found: "GS005" |
| CRITICAL | GS001 | gsc_compliance.py | 22 | Found: "GS007" |
| CRITICAL | GS001 | gsc_compliance.py | 23 | Found: "GS019" |
| CRITICAL | GS001 | gsc_compliance.py | 25 | Found: "GS014" |
| CRITICAL | GS001 | gsc_compliance.py | 26 | Found: "GS017" |
| CRITICAL | GS001 | gsc_compliance.py | 28 | Found: "GS022" |
| CRITICAL | GS001 | gsc_compliance.py | 29 | Found: "GS021" |
| CRITICAL | GS001 | gsc_compliance.py | 31 | Found: "GS009" |
| CRITICAL | GS001 | gsc_compliance.py | 33 | Found: "GS024" |
| CRITICAL | GS001 | gsc_compliance.py | 34 | Found: "GS025" |
| CRITICAL | GS001 | gsc_compliance.py | 36 | Found: "GS028" |
| CRITICAL | GS001 | gsc_compliance.py | 38 | Found: "GS030" |
| CRITICAL | GS001 | gsc_compliance.py | 40 | Found: "GS029" |
| CRITICAL | GS001 | gsc_compliance.py | 42 | Found: "GS004" |
| CRITICAL | GS001 | gsc_compliance.py | 44 | Found: "GS020" |
| CRITICAL | GS001 | gsc_compliance.py | 46 | Found: "GS002" |
| CRITICAL | GS001 | gsc_compliance.py | 47 | Found: "GS008" |
| CRITICAL | GS001 | gsc_compliance.py | 48 | Found: "GS010" |
| CRITICAL | GS001 | gsc_compliance.py | 49 | Found: "GS011" |
| CRITICAL | GS001 | gsc_compliance.py | 50 | Found: "GS012" |
| CRITICAL | GS001 | gsc_compliance.py | 51 | Found: "GS013" |
| CRITICAL | GS001 | gsc_compliance.py | 52 | Found: "GS015" |
| CRITICAL | GS001 | gsc_compliance.py | 53 | Found: "GS016" |
| CRITICAL | GS001 | gsc_compliance.py | 54 | Found: "GS018" |
| CRITICAL | GS001 | gsc_compliance.py | 55 | Found: "GS023" |
| CRITICAL | GS001 | base.py | 20 | Found: "GS000" |
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
| CRITICAL | GS001 | gs029_secrets.py | 41 | Found: "GS029" |
| CRITICAL | GS001 | gs030_sca.py | 10 | Found: "GS030" |
| CRITICAL | GS001 | gs031_iac.py | 6 | Found: "GS031" |
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
| CRITICAL | GS001 | gsc_epss.py | 135 | Found: "GS030" |
| CRITICAL | GS001 | gsc_epss.py | 146 | Found: "GS030" |
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
| CRITICAL | GS001 | gsc_nuclei_export.py | 157 | Found: 'GS000' |
| CRITICAL | GS001 | gsc_poc_generator.py | 43 | Found: "GS001" |
| CRITICAL | GS001 | gsc_poc_generator.py | 44 | Found: "GS003" |
| CRITICAL | GS001 | gsc_poc_generator.py | 45 | Found: "GS007" |
| CRITICAL | GS001 | gsc_poc_generator.py | 46 | Found: "GS012" |
| CRITICAL | GS001 | gsc_poc_generator.py | 47 | Found: "GS019" |
| CRITICAL | GS001 | gsc_poc_generator.py | 48 | Found: "GS022" |
| CRITICAL | GS001 | gsc_poc_generator.py | 49 | Found: "GS024" |
| CRITICAL | GS001 | gsc_proofoffix.py | 445 | Found: "GS001" |
| CRITICAL | GS001 | gsc_proofoffix.py | 446 | Found: "GS001" |
| CRITICAL | GS001 | gsc_proofoffix.py | 447 | Found: "GS004" |
| CRITICAL | GS001 | gsc_proofoffix.py | 448 | Found: "GS004" |
| CRITICAL | GS001 | gsc_proofoffix.py | 449 | Found: "GS005" |
| CRITICAL | GS001 | gsc_proofoffix.py | 450 | Found: "GS005" |
| CRITICAL | GS001 | gsc_proofoffix.py | 451 | Found: "GS017" |
| CRITICAL | GS001 | gsc_proofoffix.py | 452 | Found: "GS017" |
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
| CRITICAL | GS001 | gsc_selfhealing.py | 28 | Found: "GS001" |
| CRITICAL | GS001 | gsc_selfhealing.py | 28 | Found: "GS004" |
| CRITICAL | GS001 | gsc_selfhealing.py | 28 | Found: "GS005" |
| CRITICAL | GS001 | gsc_selfhealing.py | 28 | Found: "GS017" |
| CRITICAL | GS001 | gsc_selfhealing.py | 28 | Found: "GS020" |
| CRITICAL | GS001 | gsc_selfhealing.py | 28 | Found: "GS021" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 16 | Found: SECRET: "change-me-in-sealed-secret" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 14 | Found: REDIS_URL: "redis://redis:6379/0" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 25 | Found: DATABASE_URL: "postgresql://gsc_app:CHANGE_ME@postgre |
| CRITICAL | GS001 | gsc_setup_calibration.py | 15 | Found: TOKEN="ghp_abc123def456" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 10 | Found: password = "SuperSecret123!" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 8 | Found: "GS005" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 9 | Found: "GS017" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 10 | Found: "GS029" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 11 | Found: "GS008" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 12 | Found: "GS007" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 13 | Found: "GS010" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 14 | Found: "GS018" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 15 | Found: "GS029" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 16 | Found: "GS031" |
| CRITICAL | GS029 | gsc_setup_calibration.py | 10 | Match:     "secrets-demo": ("py", 'password = "SuperSecret12 |
| CRITICAL | GS029 | gsc_setup_calibration.py | 15 | Match:     "hardcoded-secret": ("py", 'API_TOKEN="ghp_abc123 |
| CRITICAL | GS029 | main.tf | 5 | Match: access_key = "AKIAIOSFODNN7EXAMPLE" |
| CRITICAL | GS007 | gsc_setup_calibration.py | 12 | Match:     "pickle-demo": ("py", 'import pickle\ndef load(x) |
| CRITICAL | GS031 | Dockerfile | 1 | Match: FROM node:latest |
| CRITICAL | GS029 | main.tf | 5 | Match: access_key = "AKIAIOSFODNN7EXAMPLE" |
| CRITICAL | GS000-LEGACY | systemd.json | 78 | Match:     "detail": "AmbientCapabilities=CAP_ALL grants all |
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
| CRITICAL | GS005 | tenancy.py | 13 | Line 13: conn.execute(f"ALTER TABLE {t} ENABLE ROW LEVEL SEC |
| CRITICAL | GS005 | tenancy.py | 14 | Line 14: conn.execute(f"ALTER TABLE {t} FORCE ROW LEVEL SECU |
| CRITICAL | GS005 | tenancy.py | 15 | Line 15: conn.execute(f"CREATE POLICY tenant_isolation_{t} O |
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
| CRITICAL | GS005 | gsc_setup_calibration.py | 8 | Line 8: "sqli-demo": ("py", 'def q(x):\n    return db.execut |
| CRITICAL | GS016 | gs016_linux_priv_esc.py | 35 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS017 | config.py | 3 | Weak DB password in connection string: mysql://admin:secret@ |
| CRITICAL | GS024 | corpus_gs005_python.py | 8 | LLM confidence: 100%. All lines use string interpolation or  |
| CRITICAL | GS024 | corpus_gs005_python.py | 9 | LLM confidence: 100%. The code contains multiple SQL injecti |
| CRITICAL | GS024 | corpus_gs005_python.py | 15 | LLM confidence: 100%. All lines use unsafe string interpolat |
| CRITICAL | GS024 | gs020_llm_sqli.py | 230 | LLM confidence: 100%. The code uses an f-string to interpola |
| CRITICAL | GS024 | gsc_metrics.py | 31 | LLM confidence: 100%. The 'project' variable is interpolated |
| CRITICAL | GS024 | gsc_metrics.py | 34 | LLM confidence: 100%. The 'project' variable is interpolated |
| CRITICAL | GS024 | gsc_setup_calibration.py | 8 | LLM confidence: 100%. The code contains an f-string SQL quer |
| HIGH | GS000-LEGACY | api.ts | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 24 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 26 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 27 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | page.tsx | 23 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | user_auth.py | 60 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | sso.py | 36 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | gsc_issue.py | 74 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | fastapi_support.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | gs012_mass_assignment.py | 44 | Hacking APIs Ch.11 |
| HIGH | GS000-LEGACY | gsc_vuln_spider.py | 47 | Redteam Kit |
| HIGH | GS025 | _cron_collect.py | 140 |  |
| HIGH | GS025 | gs011_jwt_vulnerabilities.py | 41 |  |
| HIGH | GS025 | gsc_collect_light.py | 211 |  |
| HIGH | GS025 | gsc_vuln_spider.py | 39 |  |
| HIGH | GS025 | gsc.py | 315 |  |
| HIGH | GS025 | gs005_sql_injection.py | 135 |  |
| HIGH | GS025 | _cron_collect.py | 47 |  |
| HIGH | GS025 | _cron_nvd.py | 45 |  |
| HIGH | GS025 | gs016_linux_priv_esc.py | 27 |  |
| HIGH | GS025 | gs016_linux_priv_esc.py | 40 |  |
| HIGH | GS025 | gs016_linux_priv_esc.py | 41 |  |
| HIGH | GS025 | gs016_linux_priv_esc.py | 95 |  |
| HIGH | GS025 | gs016_linux_priv_esc.py | 129 |  |
| HIGH | GS025 | gs014_credential_exposure.py | 29 |  |
| HIGH | GS025 | gs014_credential_exposure.py | 91 |  |
| HIGH | GS025 | gs014_credential_exposure.py | 92 |  |
| HIGH | GS025 | gs014_credential_exposure.py | 93 |  |
| HIGH | GS025 | gs014_credential_exposure.py | 94 |  |
| HIGH | GS025 | gs014_credential_exposure.py | 98 |  |
| HIGH | GS025 | gs014_credential_exposure.py | 99 |  |
| HIGH | GS025 | gsc_collect_light.py | 74 |  |
| HIGH | GS025 | user_auth.py | 60 |  |
| HIGH | GS025 | sso.py | 36 |  |
| HIGH | GS025 | gsc_issue.py | 74 |  |
| HIGH | GS025 | gsc_collect_light.py | 113 |  |
| HIGH | GS025 | gsc_collect_light.py | 126 |  |
| HIGH | GS000-LEGACY | _cron_collect.py | 141 |  |
| HIGH | GS000-LEGACY | gsc_collect_light.py | 212 |  |
| HIGH | GS000-LEGACY | gsc_external.py | 174 | Match:     "standard default", "localhost", "loopback", "127 |
| HIGH | GS000-LEGACY | gsc_external.py | 1310 | Match: RULES: localhost/127.0.0.1 defaults → false-positive. |
| HIGH | GS000-LEGACY | bughunter.json | 45 | Match:     "fix": "Validate URL against allowlist. Block int |
| HIGH | GS000-LEGACY | terraform.json | 3 | Match:   {"echelon": 2, "category": "HIGH", "title": "Terraf |
| HIGH | GS000-LEGACY | docker.json | 6 | Match:   {"echelon": 2, "category": "MEDIUM", "title": "Dock |
| HIGH | GS000-LEGACY | Dockerfile | 18 | Match: CMD ["uvicorn", "cloud.api:app", "--host", "0.0.0.0", |
| HIGH | GS000-LEGACY | docker-compose.yml | 35 | Match:     command: uvicorn cloud.api:app --host 0.0.0.0 --p |
| HIGH | GS000-LEGACY | sso.yaml | 14 | Match:     http_address = "0.0.0.0:4180" |
| HIGH | GS000-LEGACY | gsc_iac.py | 99 | Match:     ("GS031-TF-SG-OPEN", re.compile(r'cidr_blocks\s*= |
| HIGH | GS000-LEGACY | gsc.py | 2058 | Match:     api.add_argument('--host', default='127.0.0.1', h |
| HIGH | GS000-LEGACY | gsc_proofoffix.py | 38 | Match:     "http_proxy": "http://127.0.0.1:9", |
| HIGH | GS000-LEGACY | gsc_proofoffix.py | 39 | Match:     "https_proxy": "http://127.0.0.1:9", |
| HIGH | GS000-LEGACY | gsc_proofoffix.py | 40 | Match:     "HTTP_PROXY": "http://127.0.0.1:9", |
| HIGH | GS000-LEGACY | gsc_proofoffix.py | 41 | Match:     "HTTPS_PROXY": "http://127.0.0.1:9", |
| HIGH | GS000-LEGACY | gsc_api.py | 413 | Match:     p.add_argument("--host", default="127.0.0.1") |
| HIGH | GS000-LEGACY | gs010_ssh_hardening.py | 85 | Match:                         references=["SSH Hardening &  |
| HIGH | GS000-LEGACY | user_auth.py | 60 | Match:     user = requests.get(f"{GH_API}/user", |
| HIGH | GS000-LEGACY | sso.py | 36 | Match:     resp = requests.get(f"{issuer_url.rstrip('/')}/.w |
| HIGH | GS000-LEGACY | gsc_issue.py | 74 | Match:     r = requests.post(f"{jira_url}/rest/api/2/issue", |
| HIGH | GS008 | gsc_setup_calibration.py | 11 | Match:     "eval-demo": ("py", 'def exec(u): return eval(u)\ |
| HIGH | GS008 | framework_aware.py | 21 | Match:     "eval() usage": { |
| HIGH | GS008 | framework_aware.py | 167 | Match:         {"title": "eval() usage", "category": "HIGH", |
| HIGH | GS008 | gsc.py | 747 | Match:             "Req 6": ["SQL injection", "eval()", "pic |
| HIGH | GS008 | gsc.py | 756 | Match:             "CC6.8": ["eval()", "pickle.load"], |
| HIGH | GS008 | gsc.py | 1306 | Match:         (2, "HIGH", "eval() or exec() usage", "regex" |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 72 | Match:         "eval() with dynamic input — code injection", |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 73 | Match:         "Never use eval() on user input. Use ast.lite |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 78 | Match:         "exec() on variable — code injection risk", |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 79 | Match:         "Avoid exec(); use explicit function calls or |
| HIGH | GS008 | gs020_xss_injection.py | 38 | Match:     (r'eval\s*\(\s*[\"\'`]', "DOM XSS: eval() with st |
| HIGH | GS008 | gsc_vuln_spider.py | 31 | Match:         ('"eval(" "request" language:python stars:<20 |
| HIGH | GS000-LEGACY | gsc_pdf.py | 15 | Match:     os.system(f"python3 {os.path.dirname(__file__)}/g |
| HIGH | GS000-LEGACY | gs004_dangerous_subprocess.py | 48 | Match:         "os.system() with .format() — command injecti |
| HIGH | GS000-LEGACY | main.tf | 3 | Match:   acl    = "public-read" |
| HIGH | GS000-LEGACY | systemd.json | 23 | Match:     "title": "Systemd: User=root or absent → runs as  |
| HIGH | GS025 | .mcp.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 54 | Line 54: "os.popen() — deprecated, uses shell", |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 60 | Line 60: "commands.getoutput() — deprecated shell wrapper", |
| HIGH | GS004 | gsc_pdf.py | 15 | Line 15: os.system(f"python3 {os.path.dirname(__file__)}/gsc |
| HIGH | GS004 | gsc_setup_calibration.py | 11 | Line 11: "eval-demo": ("py", 'def exec(u): return eval(u)\n' |
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
| HIGH | GS019 | sso.py | 37 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | ? | rust.json | 7 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | gsc_metrics.py | 31 |
| C | GS005 | gsc_setup_calibration.py | 8 |
| C | GS005 | corpus_gs005_python.py | 8 |
| C | GS005 | corpus_gs005_python.py | 12 |
| C | GS005 | corpus_gs005_python.py | 15 |
| C | GS005 | corpus_gs005_python.py | 19 |
| C | GS005 | corpus_gs005_python.py | 20 |
| C | GS005 | corpus_gs005_python.py | 23 |
| C | GS005 | corpus_gs005_python.py | 28 |
| C | GS005 | corpus_gs005_python.py | 31 |
| C | GS005 | corpus_gs005_python.py | 37 |
| C | GS005 | corpus_gs005_python.py | 39 |
| C | GS005 | corpus_gs005_python.py | 43 |
| C | GS005 | corpus_gs005_python.py | 46 |
| C | GS005 | gs018_payment_abuse.py | 215 |
| C | GS005 | gs020_llm_sqli.py | 126 |
| C | GS005 | gs020_llm_sqli.py | 230 |
| M | GS010 | sso.py | 22 |
| M | GS010 | gsc_orchestrator.py | 32 |
| M | GS010 | gsc_orchestrator.py | 49 |
| M | GS010 | gsc_orchestrator.py | 57 |
| M | GS010 | pre-commit | 22 |
| M | GS010 | gsc_meta.py | 32 |
| M | GS010 | gsc_setup_calibration.py | 13 |
| M | GS010 | gsc_audit_detectors.py | 35 |
| M | GS010 | gsc_reconcile.py | 14 |
| M | GS010 | gsc_reconcile.py | 25 |
| M | GS010 | gsc_doctor.py | 16 |
| M | GS010 | gsc_doctor.py | 33 |
| M | GS010 | framework_aware.py | 31 |
| M | GS010 | framework_aware.py | 165 |
| M | GS010 | gsc.py | 60 |
| M | GS010 | gsc.py | 175 |
| M | GS010 | gsc.py | 1305 |
| M | GS010 | gsc.py | 1750 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 144 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| H | GS000-LEGACY | api.ts | 19 |
| H | GS000-LEGACY | api.ts | 24 |
| H | GS000-LEGACY | api.ts | 26 |
| H | GS000-LEGACY | api.ts | 27 |
| H | GS000-LEGACY | page.tsx | 23 |
| M | GS018 | gsc_setup_calibration.py | 14 |
| C | GS005 | corpus_gs005_python.py | 11 |
| C | GS005 | corpus_gs005_python.py | 16 |
| C | GS005 | corpus_gs005_python.py | 24 |
| C | GS005 | corpus_gs005_python.py | 25 |
| C | GS005 | gsc_epss.py | 97 |
| H | GS000-LEGACY | user_auth.py | 60 |
| H | GS000-LEGACY | sso.py | 36 |
| H | GS000-LEGACY | gsc_issue.py | 74 |
| H | GS000-LEGACY | fastapi_support.py | 38 |
| H | GS000-LEGACY | gs012_mass_assignment.py | 44 |
| H | GS000-LEGACY | gsc_vuln_spider.py | 47 |
| M | GS025 | _cron_collect.py | 42 |
| M | GS025 | _cron_nvd.py | 40 |
| M | GS025 | gsc_collect_light.py | 69 |
| M | GS007 | gsc_setup_calibration.py | 12 |
| M | GS007 | gsc.py | 747 |
| M | GS007 | gsc.py | 756 |
| M | GS007 | gsc_vuln_spider.py | 191 |
| C | GS005 | gsc_metrics.py | 31 |
| C | GS005 | gsc_setup_calibration.py | 8 |
| C | GS005 | corpus_gs005_python.py | 8 |
| C | GS005 | corpus_gs005_python.py | 12 |
| C | GS005 | corpus_gs005_python.py | 15 |
| C | GS005 | corpus_gs005_python.py | 19 |
| C | GS005 | corpus_gs005_python.py | 20 |
| C | GS005 | corpus_gs005_python.py | 23 |
| C | GS005 | corpus_gs005_python.py | 28 |
| C | GS005 | corpus_gs005_python.py | 31 |
| C | GS005 | corpus_gs005_python.py | 37 |
| C | GS005 | corpus_gs005_python.py | 39 |
| C | GS005 | corpus_gs005_python.py | 43 |
| C | GS005 | corpus_gs005_python.py | 46 |
| C | GS005 | gs020_llm_sqli.py | 126 |
| C | GS005 | gs020_llm_sqli.py | 230 |
| H | GS025 | _cron_collect.py | 140 |
| H | GS025 | gs011_jwt_vulnerabilities.py | 41 |
| H | GS025 | gsc_collect_light.py | 211 |
| H | GS025 | gsc_vuln_spider.py | 39 |
| H | GS025 | gsc.py | 315 |
| H | GS025 | gs005_sql_injection.py | 135 |
| H | GS025 | _cron_collect.py | 47 |
| H | GS025 | _cron_nvd.py | 45 |
| H | GS025 | gs016_linux_priv_esc.py | 27 |
| H | GS025 | gs016_linux_priv_esc.py | 40 |
| H | GS025 | gs016_linux_priv_esc.py | 41 |
| H | GS025 | gs016_linux_priv_esc.py | 95 |
| H | GS025 | gs016_linux_priv_esc.py | 129 |
| H | GS025 | gs014_credential_exposure.py | 29 |
| H | GS025 | gs014_credential_exposure.py | 91 |
| H | GS025 | gs014_credential_exposure.py | 92 |
| H | GS025 | gs014_credential_exposure.py | 93 |
| H | GS025 | gs014_credential_exposure.py | 94 |
| H | GS025 | gs014_credential_exposure.py | 98 |
| H | GS025 | gs014_credential_exposure.py | 99 |
| H | GS025 | gsc_collect_light.py | 74 |
| H | GS025 | user_auth.py | 60 |
| H | GS025 | sso.py | 36 |
| H | GS025 | gsc_issue.py | 74 |
| H | GS025 | gsc_collect_light.py | 113 |
| H | GS025 | gsc_collect_light.py | 126 |
| M | GS025 | gsc_setup_calibration.py | 10 |
| M | GS025 | corpus_gs005_python.py | 39 |
| M | GS020 | _cron_collect.py | 33 |
| M | GS020 | _cron_nvd.py | 31 |
| M | GS020 | multi_lang.py | 45 |
| M | GS020 | multi_lang.py | 46 |
| M | GS020 | gs020_xss_injection.py | 33 |
| M | GS020 | gs020_xss_injection.py | 36 |
| M | GS020 | gs020_xss_injection.py | 50 |
| M | GS020 | gsc_collect_light.py | 60 |
| C | GS025 | _cron_collect.py | 141 |
| C | GS025 | gsc_pdf.py | 15 |
| C | GS025 | gsc.py | 1308 |
| C | GS025 | gsc_proofoffix.py | 447 |
| C | GS025 | gs004_dangerous_subprocess.py | 38 |
| C | GS025 | gs004_dangerous_subprocess.py | 43 |
| C | GS025 | gs004_dangerous_subprocess.py | 48 |
| C | GS025 | gs004_dangerous_subprocess.py | 115 |
| C | GS025 | gsc_collect_light.py | 212 |
| C | GS025 | gsc_vuln_spider.py | 29 |
| C | GS025 | gsc_vuln_spider.py | 187 |
| C | GS000-LEGACY | _cron_collect.py | 139 |
| C | GS000-LEGACY | gsc_collect_light.py | 210 |
| C | GS000-LEGACY | _cron_collect.py | 140 |
| C | GS000-LEGACY | gsc_collect_light.py | 211 |
| C | GS000-LEGACY | gsc_vuln_spider.py | 39 |
| H | GS000-LEGACY | _cron_collect.py | 141 |
| H | GS000-LEGACY | gsc_collect_light.py | 212 |
| M | GS029 | gsc_setup_calibration.py | 10 |
| M | GS029 | gsc_setup_calibration.py | 15 |
| M | GS029 | corpus_gs005_python.py | 24 |
| M | GS029 | corpus_gs005_python.py | 39 |
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
| C | GS001 | cwe_map.py | 28 |
| C | GS001 | click.json | 9 |
| C | GS001 | flask-jwt-auth.json | 7 |
| C | GS001 | flask-jwt-auth.json | 8 |
| C | GS001 | main.tf | 5 |
| C | GS001 | main.tf | 5 |
| C | GS001 | config.py | 2 |
| C | GS001 | config.py | 3 |
| C | GS001 | github_auth.py | 40 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 5 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 6 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | compliance.py | 7 |
| C | GS001 | manifest.json | 249 |
| C | GS001 | manifest.json | 250 |
| C | GS001 | manifest.json | 289 |
| C | GS001 | manifest.json | 290 |
| C | GS001 | manifest.json | 339 |
| C | GS001 | manifest.json | 340 |
| C | GS001 | manifest.json | 344 |
| C | GS001 | manifest.json | 345 |
| C | GS001 | tsconfig.json | 4 |
| C | GS001 | gsc.py | 401 |
| C | GS001 | gsc.py | 402 |
| C | GS001 | gsc.py | 403 |
| C | GS001 | gsc.py | 404 |
| C | GS001 | gsc.py | 405 |
| C | GS001 | gsc.py | 406 |
| C | GS001 | gsc.py | 407 |
| C | GS001 | gsc.py | 408 |
| C | GS001 | gsc.py | 409 |
| C | GS001 | gsc.py | 410 |
| C | GS001 | gsc.py | 415 |
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
| C | GS001 | gsc_compliance.py | 18 |
| C | GS001 | gsc_compliance.py | 19 |
| C | GS001 | gsc_compliance.py | 20 |
| C | GS001 | gsc_compliance.py | 22 |
| C | GS001 | gsc_compliance.py | 23 |
| C | GS001 | gsc_compliance.py | 25 |
| C | GS001 | gsc_compliance.py | 26 |
| C | GS001 | gsc_compliance.py | 28 |
| C | GS001 | gsc_compliance.py | 29 |
| C | GS001 | gsc_compliance.py | 31 |
| C | GS001 | gsc_compliance.py | 33 |
| C | GS001 | gsc_compliance.py | 34 |
| C | GS001 | gsc_compliance.py | 36 |
| C | GS001 | gsc_compliance.py | 38 |
| C | GS001 | gsc_compliance.py | 40 |
| C | GS001 | gsc_compliance.py | 42 |
| C | GS001 | gsc_compliance.py | 44 |
| C | GS001 | gsc_compliance.py | 46 |
| C | GS001 | gsc_compliance.py | 47 |
| C | GS001 | gsc_compliance.py | 48 |
| C | GS001 | gsc_compliance.py | 49 |
| C | GS001 | gsc_compliance.py | 50 |
| C | GS001 | gsc_compliance.py | 51 |
| C | GS001 | gsc_compliance.py | 52 |
| C | GS001 | gsc_compliance.py | 53 |
| C | GS001 | gsc_compliance.py | 54 |
| C | GS001 | gsc_compliance.py | 55 |
| C | GS001 | base.py | 20 |
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
| C | GS001 | gs029_secrets.py | 41 |
| C | GS001 | gs030_sca.py | 10 |
| C | GS001 | gs031_iac.py | 6 |
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
| C | GS001 | gsc_epss.py | 135 |
| C | GS001 | gsc_epss.py | 146 |
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
| C | GS001 | gsc_nuclei_export.py | 157 |
| C | GS001 | gsc_poc_generator.py | 43 |
| C | GS001 | gsc_poc_generator.py | 44 |
| C | GS001 | gsc_poc_generator.py | 45 |
| C | GS001 | gsc_poc_generator.py | 46 |
| C | GS001 | gsc_poc_generator.py | 47 |
| C | GS001 | gsc_poc_generator.py | 48 |
| C | GS001 | gsc_poc_generator.py | 49 |
| C | GS001 | gsc_proofoffix.py | 445 |
| C | GS001 | gsc_proofoffix.py | 446 |
| C | GS001 | gsc_proofoffix.py | 447 |
| C | GS001 | gsc_proofoffix.py | 448 |
| C | GS001 | gsc_proofoffix.py | 449 |
| C | GS001 | gsc_proofoffix.py | 450 |
| C | GS001 | gsc_proofoffix.py | 451 |
| C | GS001 | gsc_proofoffix.py | 452 |
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
| C | GS001 | gsc_selfhealing.py | 28 |
| C | GS001 | gsc_selfhealing.py | 28 |
| C | GS001 | gsc_selfhealing.py | 28 |
| C | GS001 | gsc_selfhealing.py | 28 |
| C | GS001 | gsc_selfhealing.py | 28 |
| C | GS001 | gsc_selfhealing.py | 28 |
| C | GS001 | 00-namespace-config.yaml | 16 |
| C | GS001 | 00-namespace-config.yaml | 14 |
| C | GS001 | 00-namespace-config.yaml | 25 |
| C | GS001 | gsc_setup_calibration.py | 15 |
| C | GS001 | gsc_setup_calibration.py | 10 |
| C | GS001 | gsc_setup_calibration.py | 8 |
| C | GS001 | gsc_setup_calibration.py | 9 |
| C | GS001 | gsc_setup_calibration.py | 10 |
| C | GS001 | gsc_setup_calibration.py | 11 |
| C | GS001 | gsc_setup_calibration.py | 12 |
| C | GS001 | gsc_setup_calibration.py | 13 |
| C | GS001 | gsc_setup_calibration.py | 14 |
| C | GS001 | gsc_setup_calibration.py | 15 |
| C | GS001 | gsc_setup_calibration.py | 16 |
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
| L | GS003 | gsc.py | 186 |
| L | GS003 | gsc.py | 188 |
| L | GS003 | gsc.py | 653 |
| L | GS003 | gsc.py | 768 |
| L | GS003 | gsc.py | 770 |
| L | GS003 | gsc.py | 773 |
| L | GS003 | gsc.py | 781 |
| L | GS003 | gsc.py | 784 |
| L | GS003 | gsc.py | 787 |
| L | GS003 | gsc.py | 789 |
| L | GS003 | gsc.py | 823 |
| L | GS003 | gsc.py | 851 |
| L | GS003 | gsc.py | 935 |
| L | GS003 | gsc.py | 977 |
| L | GS003 | gsc.py | 979 |
| L | GS003 | gsc.py | 980 |
| L | GS003 | gsc.py | 981 |
| L | GS003 | gsc.py | 982 |
| L | GS003 | gsc.py | 983 |
| L | GS003 | gsc.py | 986 |
| L | GS003 | gsc.py | 988 |
| L | GS003 | gsc.py | 1058 |
| L | GS003 | gsc.py | 1059 |
| L | GS003 | gsc.py | 1063 |
| L | GS003 | gsc.py | 1178 |
| L | GS003 | gsc.py | 1249 |
| L | GS003 | gsc.py | 1272 |
| L | GS003 | gsc.py | 1332 |
| L | GS003 | gsc.py | 1343 |
| L | GS003 | gsc.py | 1344 |
| L | GS003 | gsc.py | 1352 |
| L | GS003 | gsc.py | 1360 |
| L | GS003 | gsc.py | 1362 |
| L | GS003 | gsc.py | 1376 |
| L | GS003 | gsc.py | 1388 |
| L | GS003 | gsc.py | 1389 |
| L | GS003 | gsc.py | 1391 |
| L | GS003 | gsc.py | 1404 |
| L | GS003 | gsc.py | 1406 |
| L | GS003 | gsc.py | 1436 |
| L | GS003 | gsc.py | 1437 |
| L | GS003 | gsc.py | 1444 |
| L | GS003 | gsc.py | 1451 |
| L | GS003 | gsc.py | 1461 |
| L | GS003 | gsc.py | 1468 |
| L | GS003 | gsc.py | 1489 |
| L | GS003 | gsc.py | 1499 |
| L | GS003 | gsc.py | 1502 |
| L | GS003 | gsc.py | 1520 |
| L | GS003 | gsc.py | 1526 |
| L | GS003 | gsc.py | 1537 |
| L | GS003 | gsc.py | 1548 |
| L | GS003 | gsc.py | 1552 |
| L | GS003 | gsc.py | 1553 |
| L | GS003 | gsc.py | 1554 |
| L | GS003 | gsc.py | 1555 |
| L | GS003 | gsc.py | 1557 |
| L | GS003 | gsc.py | 1564 |
| L | GS003 | gsc.py | 1571 |
| L | GS003 | gsc.py | 1581 |
| L | GS003 | gsc.py | 1590 |
| L | GS003 | gsc.py | 1592 |
| L | GS003 | gsc.py | 1593 |
| L | GS003 | gsc.py | 1633 |
| L | GS003 | gsc.py | 1661 |
| L | GS003 | gsc.py | 1663 |
| L | GS003 | gsc.py | 1666 |
| L | GS003 | gsc.py | 1694 |
| L | GS003 | gsc.py | 1697 |
| L | GS003 | gsc.py | 1699 |
| L | GS003 | gsc.py | 1700 |
| L | GS003 | gsc.py | 1710 |
| L | GS003 | gsc.py | 1715 |
| L | GS003 | gsc.py | 1718 |
| L | GS003 | gsc.py | 1732 |
| L | GS003 | gsc.py | 1737 |
| L | GS003 | gsc.py | 1758 |
| L | GS003 | gsc.py | 1759 |
| L | GS003 | gsc.py | 1770 |
| L | GS003 | gsc.py | 1782 |
| L | GS003 | gsc.py | 1784 |
| L | GS003 | gsc.py | 1785 |
| L | GS003 | gsc.py | 1786 |
| L | GS003 | gsc.py | 1790 |
| L | GS003 | gsc.py | 2217 |
| L | GS003 | gsc.py | 2281 |
| L | GS003 | gsc.py | 2282 |
| L | GS003 | gsc.py | 2324 |
| L | GS003 | gsc.py | 2329 |
| L | GS003 | gsc.py | 2331 |
| L | GS003 | gsc.py | 2337 |
| L | GS003 | gsc.py | 2340 |
| L | GS003 | gsc_api.py | 30 |
| L | GS003 | gsc_api.py | 415 |
| L | GS003 | gsc_api.py | 417 |
| L | GS003 | gsc_api.py | 418 |
| L | GS003 | gsc_archaeology.py | 284 |
| L | GS003 | gsc_archaeology.py | 288 |
| L | GS003 | gsc_archaeology.py | 292 |
| L | GS003 | gsc_archaeology.py | 295 |
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
| L | GS003 | gsc_crossrepo_secrets.py | 162 |
| L | GS003 | gsc_crossrepo_secrets.py | 164 |
| L | GS003 | gsc_crossrepo_secrets.py | 168 |
| L | GS003 | gsc_dast_scanner.py | 10 |
| L | GS003 | gsc_dast_scanner.py | 110 |
| L | GS003 | gsc_dast_scanner.py | 111 |
| L | GS003 | gsc_dast_scanner.py | 113 |
| L | GS003 | gsc_db.py | 450 |
| L | GS003 | multi_lang.py | 188 |
| L | GS003 | multi_lang.py | 194 |
| L | GS003 | multi_lang.py | 196 |
| L | GS003 | multi_lang.py | 198 |
| L | GS003 | multi_lang.py | 200 |
| L | GS003 | gsc_epss.py | 188 |
| L | GS003 | gsc_epss.py | 191 |
| L | GS003 | gsc_epss.py | 201 |
| L | GS003 | gsc_epss.py | 206 |
| L | GS003 | gsc_external.py | 950 |
| L | GS003 | gsc_external.py | 980 |
| L | GS003 | gsc_external.py | 988 |
| L | GS003 | gsc_external.py | 1016 |
| L | GS003 | gsc_external.py | 1018 |
| L | GS003 | gsc_external.py | 1019 |
| L | GS003 | gsc_external.py | 1022 |
| L | GS003 | gsc_external.py | 1037 |
| L | GS003 | gsc_external.py | 1043 |
| L | GS003 | gsc_external.py | 1074 |
| L | GS003 | gsc_external.py | 1103 |
| L | GS003 | gsc_external.py | 1109 |
| L | GS003 | gsc_external.py | 1119 |
| L | GS003 | gsc_external.py | 1148 |
| L | GS003 | gsc_external.py | 1150 |
| L | GS003 | gsc_external.py | 1187 |
| L | GS003 | gsc_external.py | 1193 |
| L | GS003 | gsc_external.py | 1196 |
| L | GS003 | gsc_external.py | 1201 |
| L | GS003 | gsc_external.py | 1203 |
| L | GS003 | gsc_external.py | 1212 |
| L | GS003 | gsc_external.py | 1389 |
| L | GS003 | gsc_external.py | 1393 |
| L | GS003 | gsc_external.py | 1399 |
| L | GS003 | gsc_external.py | 1400 |
| L | GS003 | gsc_external.py | 1403 |
| L | GS003 | gsc_external.py | 1405 |
| L | GS003 | gsc_external.py | 1407 |
| L | GS003 | gsc_external.py | 1412 |
| L | GS003 | gsc_external.py | 1432 |
| L | GS003 | gsc_external.py | 1434 |
| L | GS003 | gsc_external.py | 1454 |
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
| L | GS003 | gsc_nlpolicy.py | 63 |
| L | GS003 | gsc_nlpolicy.py | 137 |
| L | GS003 | gsc_nlpolicy.py | 142 |
| L | GS003 | gsc_nlpolicy.py | 161 |
| L | GS003 | gsc_nlpolicy.py | 163 |
| L | GS003 | gsc_nlpolicy.py | 196 |
| L | GS003 | gsc_nlpolicy.py | 198 |
| L | GS003 | gsc_nlpolicy.py | 200 |
| L | GS003 | gsc_nlpolicy.py | 203 |
| L | GS003 | gsc_nlpolicy.py | 264 |
| L | GS003 | gsc_nlpolicy.py | 266 |
| L | GS003 | gsc_nlpolicy.py | 268 |
| L | GS003 | gsc_nlpolicy.py | 270 |
| L | GS003 | gsc_nlpolicy.py | 278 |
| L | GS003 | gsc_nlpolicy.py | 282 |
| L | GS003 | gsc_nlpolicy.py | 290 |
| L | GS003 | gsc_nlpolicy.py | 305 |
| L | GS003 | gsc_nuclei_export.py | 26 |
| L | GS003 | gsc_nuclei_export.py | 193 |
| L | GS003 | gsc_nuclei_export.py | 202 |
| L | GS003 | gsc_nuclei_export.py | 203 |
| L | GS003 | gsc_nuclei_export.py | 205 |
| L | GS003 | gsc_nuclei_import.py | 11 |
| L | GS003 | gsc_nuclei_import.py | 24 |
| L | GS003 | gsc_poc_generator.py | 80 |
| L | GS003 | gsc_poc_generator.py | 88 |
| L | GS003 | gsc_proofoffix.py | 166 |
| L | GS003 | gsc_proofoffix.py | 454 |
| L | GS003 | gsc_proofoffix.py | 502 |
| L | GS003 | gsc_proofoffix.py | 503 |
| L | GS003 | gsc_sca.py | 334 |
| L | GS003 | gsc_sca.py | 336 |
| L | GS003 | gsc_sca.py | 343 |
| L | GS003 | gsc_sca.py | 345 |
| L | GS003 | gsc_sca.py | 347 |
| L | GS003 | gsc_sca.py | 350 |
| L | GS003 | gsc_sca.py | 353 |
| L | GS003 | gsc_sca.py | 356 |
| L | GS003 | gsc_selfhealing.py | 75 |
| L | GS003 | gsc_selfhealing.py | 77 |
| L | GS003 | gsc_selfhealing.py | 96 |
| L | GS003 | gsc_selfhealing.py | 99 |
| L | GS003 | gsc_selfhealing.py | 126 |
| L | GS003 | gsc_selfhealing.py | 128 |
| L | GS003 | gsc_selfhealing.py | 133 |
| L | GS003 | gsc_selfhealing.py | 169 |
| L | GS003 | gsc_selfhealing.py | 187 |
| L | GS003 | gsc_selfhealing.py | 204 |
| L | GS003 | gsc_selfhealing.py | 205 |
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
| L | GS003 | gsc_audit_compliance.py | 11 |
| L | GS003 | gsc_audit_compliance.py | 12 |
| L | GS003 | gsc_audit_compliance.py | 15 |
| L | GS003 | gsc_audit_compliance.py | 19 |
| L | GS003 | gsc_audit_compliance.py | 21 |
| L | GS003 | gsc_audit_compliance.py | 25 |
| L | GS003 | gsc_audit_detectors.py | 27 |
| L | GS003 | gsc_audit_detectors.py | 40 |
| L | GS003 | gsc_audit_detectors.py | 44 |
| L | GS003 | gsc_audit_detectors.py | 45 |
| L | GS003 | gsc_audit_detectors.py | 49 |
| L | GS003 | gsc_audit_detectors.py | 54 |
| L | GS003 | gsc_audit_groundtruth.py | 42 |
| L | GS003 | gsc_audit_groundtruth.py | 43 |
| L | GS003 | gsc_audit_groundtruth.py | 44 |
| L | GS003 | gsc_audit_groundtruth.py | 52 |
| L | GS003 | gsc_audit_groundtruth.py | 54 |
| L | GS003 | gsc_audit_groundtruth.py | 57 |
| L | GS003 | gsc_audit_groundtruth.py | 64 |
| L | GS003 | gsc_audit_groundtruth.py | 68 |
| L | GS003 | gsc_audit_groundtruth.py | 70 |
| L | GS003 | gsc_audit_groundtruth.py | 73 |
| L | GS003 | gsc_audit_groundtruth.py | 81 |
| L | GS003 | gsc_audit_groundtruth.py | 83 |
| L | GS003 | gsc_audit_groundtruth.py | 84 |
| L | GS003 | gsc_audit_groundtruth.py | 86 |
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
| L | GS003 | gsc_reconcile.py | 42 |
| L | GS003 | gsc_reconcile.py | 44 |
| L | GS003 | gsc_reconcile.py | 45 |
| L | GS003 | gsc_reconcile.py | 46 |
| L | GS003 | gsc_reconcile.py | 53 |
| L | GS003 | gsc_reconcile.py | 56 |
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
| L | GS003 | gsc_setup_calibration.py | 30 |
| L | GS003 | gsc_setup_calibration.py | 35 |
| L | GS003 | gsc_setup_calibration.py | 36 |
| L | GS003 | gsc_stabilize.py | 43 |
| L | GS003 | gsc_stabilize.py | 46 |
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
| L | GS008 | gsc_sbom.py | 23 |
| L | GS008 | gsc_selfhealing.py | 26 |
| L | GS008 | gsc_pr_commands.py | 10 |
| i | GS020 |  | 137 |
| i | GS020 |  | 9 |
| i | GS020 |  | 63 |
| i | GS020 |  | 126 |
| i | GS020 |  | 45 |
| i | GS020 |  | 46 |
| i | GS020 |  | 10 |
| i | GS020 |  | 34 |
| i | GS020 |  | 34 |
| i | GS020 |  | 36 |
| i | GS020 |  | 45 |
| i | GS020 |  | 74 |
| i | GS020 |  | 74 |
| i | GS020 |  | 74 |
| i | GS020 |  | 31 |
| i | GS020 |  | 135 |
| i | GS020 |  | 184 |
| i | GS020 |  | 192 |
| i | GS020 |  | 267 |
| i | GS020 |  | 141 |
| H | GS000-LEGACY | gsc_external.py | 174 |
| H | GS000-LEGACY | gsc_external.py | 1310 |
| H | GS000-LEGACY | bughunter.json | 45 |
| H | GS000-LEGACY | terraform.json | 3 |
| H | GS000-LEGACY | docker.json | 6 |
| H | GS000-LEGACY | Dockerfile | 18 |
| H | GS000-LEGACY | docker-compose.yml | 35 |
| H | GS000-LEGACY | sso.yaml | 14 |
| H | GS000-LEGACY | gsc_iac.py | 99 |
| H | GS000-LEGACY | gsc.py | 2058 |
| H | GS000-LEGACY | gsc_proofoffix.py | 38 |
| H | GS000-LEGACY | gsc_proofoffix.py | 39 |
| H | GS000-LEGACY | gsc_proofoffix.py | 40 |
| H | GS000-LEGACY | gsc_proofoffix.py | 41 |
| H | GS000-LEGACY | gsc_api.py | 413 |
| H | GS000-LEGACY | gs010_ssh_hardening.py | 85 |
| C | GS029 | gsc_setup_calibration.py | 10 |
| C | GS029 | gsc_setup_calibration.py | 15 |
| C | GS029 | main.tf | 5 |
| M | GS000-LEGACY | gsc_sca.py | 121 |
| M | GS000-LEGACY | gsc_sca.py | 122 |
| H | GS000-LEGACY | user_auth.py | 60 |
| H | GS000-LEGACY | sso.py | 36 |
| H | GS000-LEGACY | gsc_issue.py | 74 |
| H | GS008 | gsc_setup_calibration.py | 11 |
| H | GS008 | framework_aware.py | 21 |
| H | GS008 | framework_aware.py | 167 |
| H | GS008 | gsc.py | 747 |
| H | GS008 | gsc.py | 756 |
| H | GS008 | gsc.py | 1306 |
| H | GS008 | gs004_dangerous_subprocess.py | 72 |
| H | GS008 | gs004_dangerous_subprocess.py | 73 |
| H | GS008 | gs004_dangerous_subprocess.py | 78 |
| H | GS008 | gs004_dangerous_subprocess.py | 79 |
| H | GS008 | gs020_xss_injection.py | 38 |
| H | GS008 | gsc_vuln_spider.py | 31 |
| C | GS007 | gsc_setup_calibration.py | 12 |
| H | GS000-LEGACY | gsc_pdf.py | 15 |
| H | GS000-LEGACY | gs004_dangerous_subprocess.py | 48 |
| C | GS031 | Dockerfile | 1 |
| C | GS029 | main.tf | 5 |
| H | GS000-LEGACY | main.tf | 3 |
| M | GS000-LEGACY | systemd.json | 18 |
| M | GS000-LEGACY | systemd.json | 19 |
| H | GS000-LEGACY | systemd.json | 23 |
| M | GS000-LEGACY | systemd.json | 63 |
| M | GS000-LEGACY | systemd.json | 68 |
| C | GS000-LEGACY | systemd.json | 78 |
| H | GS025 | .mcp.json | 0 |
| H | GS004 | gs004_dangerous_subprocess.py | 54 |
| H | GS004 | gs004_dangerous_subprocess.py | 60 |
| H | GS004 | gsc_pdf.py | 15 |
| H | GS004 | gsc_setup_calibration.py | 11 |
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
| C | GS005 | tenancy.py | 13 |
| C | GS005 | tenancy.py | 14 |
| C | GS005 | tenancy.py | 15 |
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
| C | GS005 | gsc_setup_calibration.py | 8 |
| H | GS007 | api.py | 65 |
| I | GS007 | federated_server.py | 16 |
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
| I | GS007 | gsc_crossrepo_secrets.py | 68 |
| I | GS007 | gsc_db.py | 50 |
| I | GS007 | gsc_db.py | 90 |
| I | GS007 | gsc_db.py | 103 |
| I | GS007 | gsc_db.py | 150 |
| I | GS007 | gsc_db.py | 196 |
| I | GS007 | gsc_db.py | 216 |
| I | GS007 | gsc_db.py | 230 |
| I | GS007 | gsc_db.py | 271 |
| I | GS007 | gsc_db.py | 291 |
| I | GS007 | gsc_db.py | 305 |
| I | GS007 | gsc_db.py | 318 |
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
| C | GS017 | config.py | 3 |
| H | GS019 | sso.py | 37 |
| M | GS019 | gs021_csrf_ssrf.py | 37 |
| s | GS021 |  | 81 |
| s | GS021 |  | 174 |
| s | GS021 |  | 174 |
| s | GS021 |  | 1310 |
| s | GS021 |  | 1310 |
| s | GS021 |  | 228 |
| s | GS021 |  | 74 |
| s | GS021 |  | 99 |
| s | GS021 |  | 1058 |
| s | GS021 |  | 2058 |
| s | GS021 |  | 2058 |
| s | GS021 |  | 38 |
| s | GS021 |  | 39 |
| s | GS021 |  | 40 |
| s | GS021 |  | 41 |
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
| s | GS021 |  | 3 |
| s | GS021 |  | 10 |
| s | GS021 |  | 43 |
| s | GS021 |  | 45 |
| s | GS021 |  | 46 |
| s | GS021 |  | 47 |
| r | GS022 |  | 19 |
| r | GS022 |  | 26 |
| r | GS022 |  | 46 |
| r | GS022 |  | 73 |
| r | GS022 |  | 44 |
| r | GS022 |  | 142 |
| r | GS022 |  | 668 |
| r | GS022 |  | 23 |
| r | GS022 |  | 24 |
| r | GS022 |  | 53 |
| r | GS022 |  | 18 |
| r | GS022 |  | 29 |
| r | GS022 |  | 34 |
| r | GS022 |  | 45 |
| r | GS022 |  | 6 |
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
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
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
| C | GS024 | gsc_setup_calibration.py | 8 |
| M | ? | gsc_external.py | 732 |
| M | ? | gsc_external.py | 737 |
| M | ? | gsc_external.py | 762 |
| M | ? | gsc_external.py | 764 |
| M | ? | gsc_external.py | 775 |
| M | ? | gsc_external.py | 794 |
| M | ? | gsc_external.py | 796 |
| M | ? | gsc_external.py | 916 |
| M | ? | gsc_external.py | 920 |
| M | ? | gsc_external.py | 969 |
| M | ? | gsc_external.py | 975 |
| M | ? | gsc_external.py | 982 |
| M | ? | gsc_external.py | 1025 |
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
| M | ? | gsc_dast_scanner.py | 77 |
| M | ? | gsc_evidence_pack.py | 25 |
| M | ? | gsc_evidence_pack.py | 32 |
| M | ? | gsc_pr_scanner.py | 46 |
| M | ? | gsc_pr_scanner.py | 117 |
| M | ? | gsc_audit_groundtruth.py | 29 |
| M | ? | gsc_audit_detectors.py | 32 |
| M | ? | gsc_stabilize.py | 13 |
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
| M | ? | gsc.py | 444 |
| M | ? | gsc.py | 493 |
| M | ? | gsc.py | 606 |
| M | ? | gsc.py | 1239 |
| M | ? | gsc.py | 1241 |
| M | ? | gsc.py | 1243 |
| M | ? | gsc.py | 1996 |
| M | ? | gsc.py | 2004 |
| M | ? | gsc.py | 2021 |
| M | ? | gsc.py | 2144 |
| M | ? | gsc.py | 2156 |
| M | ? | gsc.py | 2166 |
| M | ? | gsc.py | 2174 |
| M | ? | gsc.py | 2179 |
| M | ? | gsc.py | 2182 |
| M | ? | gsc.py | 2185 |
| M | ? | gsc.py | 2198 |
| M | ? | gsc.py | 2200 |
| M | ? | gsc.py | 2225 |
| M | ? | gsc.py | 2231 |
| M | ? | gsc.py | 2248 |
| M | ? | gsc.py | 2251 |
| M | ? | gsc.py | 2260 |
| M | ? | gsc.py | 2268 |
| M | ? | gsc.py | 2272 |
| M | ? | gsc.py | 2276 |
| M | ? | gsc.py | 2301 |
| M | ? | gsc.py | 2304 |
| M | ? | gsc.py | 2314 |
| M | ? | gsc_archaeology.py | 75 |
| M | ? | gsc_archaeology.py | 97 |
| M | ? | runner.py | 88 |
| M | ? | gsc_forecast.py | 35 |
| M | ? | gsc_forecast.py | 48 |
| M | ? | gsc_forecast.py | 69 |
| M | ? | gsc_forecast.py | 223 |
| M | ? | gsc_proofoffix.py | 129 |
| M | ? | gsc_selfhealing.py | 167 |
| M | ? | gsc_selfhealing.py | 172 |
| M | ? | gsc_selfhealing.py | 173 |
| M | ? | gsc_selfhealing.py | 174 |
| M | ? | gsc_selfhealing.py | 178 |
| M | ? | gsc_selfhealing.py | 180 |
| M | ? | gsc_dast_validator.py | 58 |
| M | ? | gs009_supply_chain.py | 79 |
| M | ? | gs004_dangerous_subprocess.py | 39 |
| M | ? | gs004_dangerous_subprocess.py | 44 |
| M | ? | gs004_dangerous_subprocess.py | 49 |
| M | ? | gs004_dangerous_subprocess.py | 61 |
| M | ? | go.json | 9 |
| H | ? | rust.json | 7 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T14:48:19.247068*