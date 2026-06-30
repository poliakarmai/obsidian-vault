---
title: "GSC Audit: /home/openclaw/gsc"
date: 2026-06-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc

**Дата:** 29.06.2026 14:17  
**Путь:** `/home/openclaw/gsc`  
**Всего находок:** 310  
**CRITICAL:** 7 | **HIGH:** 23 | **MEDIUM:** 47 | **LOW:** 232

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 156 |
| Синхронный код в async | 26 |
| GS008 | 17 |
| eval() or exec() usage | 9 |
| GS012 | 9 |
| Bare except: | 7 |
| GS005 | 6 |
| Хардкод IP адреса | 5 |
| GS004 | 3 |
| os.system() without sanitization | 2 |
| Systemd: EnvironmentFile without quotes → word splitting | 2 |
| Systemd: Type=forking without PIDFile | 2 |
| Generic code smell #24 | 1 |
| Generic code smell #27 | 1 |
| Generic code smell #30 | 1 |
| Generic code smell #33 | 1 |
| Generic code smell #36 | 1 |
| Generic code smell #39 | 1 |
| Generic code smell #42 | 1 |
| Generic code smell #45 | 1 |
| Generic code smell #48 | 1 |
| Generic code smell #51 | 1 |
| Generic code smell #54 | 1 |
| Generic code smell #57 | 1 |
| Generic code smell #60 | 1 |
| Generic code smell #63 | 1 |
| Generic code smell #66 | 1 |
| Generic code smell #69 | 1 |
| Generic code smell #72 | 1 |
| Generic code smell #75 | 1 |
| Generic code smell #78 | 1 |
| Generic code smell #81 | 1 |
| Generic code smell #84 | 1 |
| Generic code smell #87 | 1 |
| Generic code smell #90 | 1 |
| Generic code smell #93 | 1 |
| Generic code smell #96 | 1 |
| Generic code smell #99 | 1 |
| Generic code smell #102 | 1 |
| Generic code smell #105 | 1 |
| Generic code smell #108 | 1 |
| Generic code smell #111 | 1 |
| Generic code smell #114 | 1 |
| Generic code smell #117 | 1 |
| Generic code smell #120 | 1 |
| Generic code smell #123 | 1 |
| Generic code smell #126 | 1 |
| Generic code smell #129 | 1 |
| Generic code smell #132 | 1 |
| Generic code smell #135 | 1 |
| Generic code smell #138 | 1 |
| Generic code smell #141 | 1 |
| Generic code smell #144 | 1 |
| Generic code smell #147 | 1 |
| Generic code smell #150 | 1 |
| Generic code smell #153 | 1 |
| Generic code smell #156 | 1 |
| Generic code smell #159 | 1 |
| Generic code smell #162 | 1 |
| Generic code smell #165 | 1 |
| Generic code smell #168 | 1 |
| Generic code smell #171 | 1 |
| Generic code smell #174 | 1 |
| Generic code smell #177 | 1 |
| Generic code smell #180 | 1 |
| Generic code smell #183 | 1 |
| Generic code smell #186 | 1 |
| Generic code smell #189 | 1 |
| Generic code smell #192 | 1 |
| Generic code smell #195 | 1 |
| Generic code smell #198 | 1 |
| Python: SSRF via requests without URL validation | 1 |
| User-controlled URL in request | 1 |
| Systemd: User=root or absent → runs as root | 1 |
| Systemd: AmbientCapabilities with ALL caps | 1 |
| GS009 | 1 |
| Go: sync.Mutex copy | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | systemd.json | 78 | Match:     "detail": "AmbientCapabilities=CAP_ALL grants all |
| CRITICAL | GS005 | gsc.py | 1375 | Line 1375: conn.execute( |
| CRITICAL | GS005 | gsc.py | 1380 | Line 1380: conn.execute( |
| CRITICAL | GS005 | gsc_metrics.py | 39 | Line 39: rows = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 52 | Line 52: rows = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 66 | Line 66: rows = conn.execute(f""" |
| CRITICAL | GS005 | e4_llm.py | 129 | Line 129: row = conn.execute( |
| HIGH | ? | gsc_issue.py | 74 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | gs010_ssh_hardening.py | 81 | Match:                         references=["SSH Hardening &  |
| HIGH | ? | docker.json | 6 | Match:   {"echelon": 2, "category": "MEDIUM", "title": "Dock |
| HIGH | ? | sso.yaml | 14 | Match:     http_address = "0.0.0.0:4180" |
| HIGH | ? | terraform.json | 3 | Match:   {"echelon": 2, "category": "HIGH", "title": "Terraf |
| HIGH | ? | bughunter.json | 45 | Match:     "fix": "Validate URL against allowlist. Block int |
| HIGH | ? | gsc_issue.py | 74 | Match:     r = requests.post(f"{jira_url}/rest/api/2/issue", |
| HIGH | ? | gs004_dangerous_subprocess.py | 68 | Match:         "eval() with dynamic input — code injection", |
| HIGH | ? | gs004_dangerous_subprocess.py | 69 | Match:         "Never use eval() on user input. Use ast.lite |
| HIGH | ? | gs004_dangerous_subprocess.py | 74 | Match:         "exec() on variable — code injection risk", |
| HIGH | ? | gs004_dangerous_subprocess.py | 75 | Match:         "Avoid exec(); use explicit function calls or |
| HIGH | ? | gsc.py | 646 | Match:             "Req 6": ["SQL injection", "eval()", "pic |
| HIGH | ? | gsc.py | 655 | Match:             "CC6.8": ["eval()", "pickle.load"], |
| HIGH | ? | gsc.py | 1205 | Match:         (2, "HIGH", "eval() or exec() usage", "regex" |
| HIGH | ? | framework_aware.py | 21 | Match:     "eval() usage": { |
| HIGH | ? | framework_aware.py | 167 | Match:         {"title": "eval() usage", "category": "HIGH", |
| HIGH | ? | gs004_dangerous_subprocess.py | 44 | Match:         "os.system() with .format() — command injecti |
| HIGH | ? | gsc_pdf.py | 15 | Match:     os.system(f"python3 {os.path.dirname(__file__)}/g |
| HIGH | ? | systemd.json | 23 | Match:     "title": "Systemd: User=root or absent → runs as  |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 50 | Line 50: "os.popen() — deprecated, uses shell", |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 56 | Line 56: "commands.getoutput() — deprecated shell wrapper", |
| HIGH | GS004 | gsc_pdf.py | 15 | Line 15: os.system(f"python3 {os.path.dirname(__file__)}/gsc |
| HIGH | ? | rust.json | 7 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | gsc.py | 54 |
| M | ? | gsc.py | 1204 |
| M | ? | framework_aware.py | 31 |
| M | ? | framework_aware.py | 165 |
| M | ? | gsc_doctor.py | 16 |
| M | ? | gsc_doctor.py | 33 |
| M | ? | pre-commit | 22 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| L | ? | gs001_hardcoded_secret.py | 64 |
| H | ? | gsc_issue.py | 74 |
| L | GS003 | gsc.py | 75 |
| L | GS003 | gsc.py | 80 |
| L | GS003 | gsc.py | 81 |
| L | GS003 | gsc.py | 82 |
| L | GS003 | gsc.py | 89 |
| L | GS003 | gsc.py | 119 |
| L | GS003 | gsc.py | 122 |
| L | GS003 | gsc.py | 143 |
| L | GS003 | gsc.py | 145 |
| L | GS003 | gsc.py | 552 |
| L | GS003 | gsc.py | 667 |
| L | GS003 | gsc.py | 669 |
| L | GS003 | gsc.py | 672 |
| L | GS003 | gsc.py | 680 |
| L | GS003 | gsc.py | 683 |
| L | GS003 | gsc.py | 686 |
| L | GS003 | gsc.py | 688 |
| L | GS003 | gsc.py | 722 |
| L | GS003 | gsc.py | 750 |
| L | GS003 | gsc.py | 834 |
| L | GS003 | gsc.py | 876 |
| L | GS003 | gsc.py | 878 |
| L | GS003 | gsc.py | 879 |
| L | GS003 | gsc.py | 880 |
| L | GS003 | gsc.py | 881 |
| L | GS003 | gsc.py | 882 |
| L | GS003 | gsc.py | 885 |
| L | GS003 | gsc.py | 887 |
| L | GS003 | gsc.py | 957 |
| L | GS003 | gsc.py | 958 |
| L | GS003 | gsc.py | 962 |
| L | GS003 | gsc.py | 1077 |
| L | GS003 | gsc.py | 1148 |
| L | GS003 | gsc.py | 1171 |
| L | GS003 | gsc.py | 1231 |
| L | GS003 | gsc.py | 1242 |
| L | GS003 | gsc.py | 1243 |
| L | GS003 | gsc.py | 1251 |
| L | GS003 | gsc.py | 1259 |
| L | GS003 | gsc.py | 1261 |
| L | GS003 | gsc.py | 1275 |
| L | GS003 | gsc.py | 1287 |
| L | GS003 | gsc.py | 1288 |
| L | GS003 | gsc.py | 1290 |
| L | GS003 | gsc.py | 1303 |
| L | GS003 | gsc.py | 1305 |
| L | GS003 | gsc.py | 1335 |
| L | GS003 | gsc.py | 1336 |
| L | GS003 | gsc.py | 1343 |
| L | GS003 | gsc.py | 1350 |
| L | GS003 | gsc.py | 1360 |
| L | GS003 | gsc.py | 1367 |
| L | GS003 | gsc.py | 1388 |
| L | GS003 | gsc.py | 1398 |
| L | GS003 | gsc.py | 1401 |
| L | GS003 | gsc.py | 1419 |
| L | GS003 | gsc.py | 1425 |
| L | GS003 | gsc.py | 1436 |
| L | GS003 | gsc.py | 1447 |
| L | GS003 | gsc.py | 1451 |
| L | GS003 | gsc.py | 1452 |
| L | GS003 | gsc.py | 1453 |
| L | GS003 | gsc.py | 1454 |
| L | GS003 | gsc.py | 1456 |
| L | GS003 | gsc.py | 1463 |
| L | GS003 | gsc.py | 1470 |
| L | GS003 | gsc.py | 1480 |
| L | GS003 | gsc.py | 1489 |
| L | GS003 | gsc.py | 1491 |
| L | GS003 | gsc.py | 1492 |
| L | GS003 | gsc.py | 1532 |
| L | GS003 | gsc.py | 1560 |
| L | GS003 | gsc.py | 1562 |
| L | GS003 | gsc.py | 1565 |
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
| L | GS003 | gsc_baseline.py | 12 |
| L | GS003 | gsc_baseline.py | 48 |
| L | GS003 | gsc_baseline.py | 56 |
| L | GS003 | gsc_baseline.py | 63 |
| L | GS003 | gsc_baseline.py | 81 |
| L | GS003 | gsc_baseline.py | 85 |
| L | GS003 | gsc_baseline.py | 96 |
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
| L | GS003 | gsc_metrics.py | 9 |
| L | GS003 | gsc_metrics.py | 23 |
| L | GS003 | gsc_metrics.py | 25 |
| L | GS003 | gsc_metrics.py | 26 |
| L | GS003 | gsc_metrics.py | 27 |
| L | GS003 | gsc_metrics.py | 28 |
| L | GS003 | gsc_metrics.py | 29 |
| L | GS003 | gsc_metrics.py | 30 |
| L | GS003 | gsc_metrics.py | 31 |
| L | GS003 | gsc_metrics.py | 32 |
| L | GS003 | gsc_metrics.py | 33 |
| L | GS003 | gsc_metrics.py | 35 |
| L | GS003 | gsc_metrics.py | 38 |
| L | GS003 | gsc_pdf.py | 10 |
| L | GS003 | gsc_pdf.py | 19 |
| L | GS003 | gsc_pr_comment.py | 68 |
| L | GS003 | gsc_pr_comment.py | 99 |
| L | GS003 | gsc_pr_comment.py | 101 |
| L | GS003 | gsc_reachability.py | 91 |
| L | GS003 | gsc_reachability.py | 96 |
| L | GS003 | gsc_reachability.py | 106 |
| L | GS003 | gsc_reachability.py | 108 |
| L | GS003 | gsc_reachability.py | 110 |
| L | GS003 | gsc_report.py | 10 |
| L | GS003 | gsc_report.py | 73 |
| L | GS008 | gsc.py | 40 |
| L | GS008 | gsc.py | 53 |
| L | GS008 | gs001_hardcoded_secret.py | 17 |
| L | GS008 | gs002_world_readable.py | 15 |
| L | GS008 | gs003_debug_prints.py | 14 |
| L | GS008 | gs004_dangerous_subprocess.py | 18 |
| L | GS008 | gs005_sql_injection.py | 19 |
| L | GS008 | gs007_idor.py | 18 |
| L | GS008 | gs008_dead_code.py | 20 |
| L | GS008 | gs009_supply_chain.py | 22 |
| L | GS008 | gs010_ssh_hardening.py | 21 |
| L | GS008 | gs011_jwt_vulnerabilities.py | 19 |
| L | GS008 | gs012_mass_assignment.py | 19 |
| L | GS008 | gs013_graphql_security.py | 20 |
| L | GS008 | gs014_credential_exposure.py | 24 |
| L | GS008 | registry.py | 136 |
| L | GS008 | registry.py | 137 |
| H | ? | gs010_ssh_hardening.py | 81 |
| H | ? | docker.json | 6 |
| H | ? | sso.yaml | 14 |
| H | ? | terraform.json | 3 |
| H | ? | bughunter.json | 45 |
| H | ? | gsc_issue.py | 74 |
| H | ? | gs004_dangerous_subprocess.py | 68 |
| H | ? | gs004_dangerous_subprocess.py | 69 |
| H | ? | gs004_dangerous_subprocess.py | 74 |
| H | ? | gs004_dangerous_subprocess.py | 75 |
| H | ? | gsc.py | 646 |
| H | ? | gsc.py | 655 |
| H | ? | gsc.py | 1205 |
| H | ? | framework_aware.py | 21 |
| H | ? | framework_aware.py | 167 |
| H | ? | gs004_dangerous_subprocess.py | 44 |
| H | ? | gsc_pdf.py | 15 |
| M | ? | systemd.json | 18 |
| M | ? | systemd.json | 19 |
| H | ? | systemd.json | 23 |
| M | ? | systemd.json | 63 |
| M | ? | systemd.json | 68 |
| C | ? | systemd.json | 78 |
| H | GS004 | gs004_dangerous_subprocess.py | 50 |
| H | GS004 | gs004_dangerous_subprocess.py | 56 |
| H | GS004 | gsc_pdf.py | 15 |
| C | GS005 | gsc.py | 1375 |
| C | GS005 | gsc.py | 1380 |
| C | GS005 | gsc_metrics.py | 39 |
| C | GS005 | gsc_metrics.py | 52 |
| C | GS005 | gsc_metrics.py | 66 |
| C | GS005 | e4_llm.py | 129 |
| s | GS009 |  | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gs012_mass_assignment.py | 0 |
| M | GS012 | gsc_issue.py | 0 |
| M | ? | gs004_dangerous_subprocess.py | 35 |
| M | ? | gs004_dangerous_subprocess.py | 40 |
| M | ? | gs004_dangerous_subprocess.py | 45 |
| M | ? | gs004_dangerous_subprocess.py | 57 |
| M | ? | gs009_supply_chain.py | 75 |
| M | ? | gsc.py | 88 |
| M | ? | gsc.py | 345 |
| M | ? | gsc.py | 388 |
| M | ? | gsc.py | 505 |
| M | ? | gsc.py | 1138 |
| M | ? | gsc.py | 1140 |
| M | ? | gsc.py | 1142 |
| M | ? | gsc.py | 1667 |
| M | ? | gsc.py | 1670 |
| M | ? | gsc.py | 1673 |
| M | ? | gsc.py | 1686 |
| M | ? | gsc.py | 1688 |
| M | ? | e4_llm.py | 307 |
| M | ? | gsc_doctor.py | 21 |
| M | ? | gsc_doctor.py | 31 |
| M | ? | python_async.json | 42 |
| M | ? | python_async.json | 53 |
| M | ? | python_async.json | 74 |
| M | ? | python_async.json | 75 |
| M | ? | bughunter.json | 32 |
| M | ? | bughunter.json | 33 |
| M | ? | go.json | 9 |
| H | ? | rust.json | 7 |

---
*Сгенерировано GSC v0.6 · 2026-06-29T14:17:21.511307*