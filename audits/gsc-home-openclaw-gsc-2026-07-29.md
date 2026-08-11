---
title: "GSC Audit: /home/openclaw/gsc"
date: 2026-07-29
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc

**Дата:** 29.07.2026 20:11  
**Путь:** `/home/openclaw/gsc`  
**Всего находок:** 577  
**CRITICAL:** 95 | **HIGH:** 76 | **MEDIUM:** 56 | **LOW:** 339

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 241 |
| GS005 | 54 |
| GS008 | 39 |
| Синхронный код в async | 31 |
| GS007 | 27 |
| CVE-2026-56233: Privilege escalation | 15 |
| SQL injection risk: f-string in query | 12 |
| CVE-2026-55721: SQL injection | 12 |
| CVE-2026-56413: Command injection | 10 |
| eval() or exec() usage | 10 |
| Bare except: | 7 |
| Хардкод IP адреса | 5 |
| Python: raw string concatenation in SQL | 4 |
| CVE-2026-56219: Authentication bypass | 4 |
| CVE-2026-54696: Buffer overflow | 3 |
| CVE-2026-55223: Insecure deserialization | 3 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 3 |
| CVE-2026-56356: Cross-site scripting (XSS) | 3 |
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
| Go: sync.Mutex copy | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
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
| CRITICAL | ? | corpus_gs005_python.py | 11 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | corpus_gs005_python.py | 16 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | corpus_gs005_python.py | 24 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | corpus_gs005_python.py | 25 | String concatenation with SQL — classic SQL injection vector |
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
| CRITICAL | ? | _cron_collect.py | 141 |  |
| CRITICAL | ? | gsc_pdf.py | 15 |  |
| CRITICAL | ? | gsc.py | 1228 |  |
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
| CRITICAL | GS005 | gsc_metrics.py | 39 | Line 39: rows = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 52 | Line 52: rows = conn.execute(f""" |
| CRITICAL | GS005 | gsc_metrics.py | 66 | Line 66: rows = conn.execute(f""" |
| CRITICAL | GS016 | gs016_linux_priv_esc.py | 31 | SUID binary outside standard system paths — potential privil |
| HIGH | ? | gsc_issue.py | 74 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | ? | fastapi_support.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | gs012_mass_assignment.py | 40 | Hacking APIs Ch.11 |
| HIGH | ? | gsc_vuln_spider.py | 47 | Redteam Kit |
| HIGH | ? | _cron_collect.py | 140 |  |
| HIGH | ? | gs011_jwt_vulnerabilities.py | 37 |  |
| HIGH | ? | gsc_collect_light.py | 211 |  |
| HIGH | ? | gsc_vuln_spider.py | 39 |  |
| HIGH | ? | gsc.py | 263 |  |
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
| HIGH | ? | bughunter.json | 45 | Match:     "fix": "Validate URL against allowlist. Block int |
| HIGH | ? | terraform.json | 3 | Match:   {"echelon": 2, "category": "HIGH", "title": "Terraf |
| HIGH | ? | docker.json | 6 | Match:   {"echelon": 2, "category": "MEDIUM", "title": "Dock |
| HIGH | ? | sso.yaml | 14 | Match:     http_address = "0.0.0.0:4180" |
| HIGH | ? | gs010_ssh_hardening.py | 81 | Match:                         references=["SSH Hardening &  |
| HIGH | ? | gsc_issue.py | 74 | Match:     r = requests.post(f"{jira_url}/rest/api/2/issue", |
| HIGH | ? | framework_aware.py | 21 | Match:     "eval() usage": { |
| HIGH | ? | framework_aware.py | 167 | Match:         {"title": "eval() usage", "category": "HIGH", |
| HIGH | ? | gsc.py | 667 | Match:             "Req 6": ["SQL injection", "eval()", "pic |
| HIGH | ? | gsc.py | 676 | Match:             "CC6.8": ["eval()", "pickle.load"], |
| HIGH | ? | gsc.py | 1226 | Match:         (2, "HIGH", "eval() or exec() usage", "regex" |
| HIGH | ? | gs004_dangerous_subprocess.py | 68 | Match:         "eval() with dynamic input — code injection", |
| HIGH | ? | gs004_dangerous_subprocess.py | 69 | Match:         "Never use eval() on user input. Use ast.lite |
| HIGH | ? | gs004_dangerous_subprocess.py | 74 | Match:         "exec() on variable — code injection risk", |
| HIGH | ? | gs004_dangerous_subprocess.py | 75 | Match:         "Avoid exec(); use explicit function calls or |
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
| M | ? | pre-commit | 22 |
| M | ? | gsc_doctor.py | 16 |
| M | ? | gsc_doctor.py | 33 |
| M | ? | framework_aware.py | 31 |
| M | ? | framework_aware.py | 165 |
| M | ? | gsc.py | 54 |
| M | ? | gsc.py | 1225 |
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
| M | ? | gsc.py | 667 |
| M | ? | gsc.py | 676 |
| M | ? | gsc_vuln_spider.py | 191 |
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
| H | ? | _cron_collect.py | 140 |
| H | ? | gs011_jwt_vulnerabilities.py | 37 |
| H | ? | gsc_collect_light.py | 211 |
| H | ? | gsc_vuln_spider.py | 39 |
| H | ? | gsc.py | 263 |
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
| M | ? | gsc_collect_light.py | 60 |
| C | ? | _cron_collect.py | 141 |
| C | ? | gsc_pdf.py | 15 |
| C | ? | gsc.py | 1228 |
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
| L | GS003 | gsc.py | 573 |
| L | GS003 | gsc.py | 688 |
| L | GS003 | gsc.py | 690 |
| L | GS003 | gsc.py | 693 |
| L | GS003 | gsc.py | 701 |
| L | GS003 | gsc.py | 704 |
| L | GS003 | gsc.py | 707 |
| L | GS003 | gsc.py | 709 |
| L | GS003 | gsc.py | 743 |
| L | GS003 | gsc.py | 771 |
| L | GS003 | gsc.py | 855 |
| L | GS003 | gsc.py | 897 |
| L | GS003 | gsc.py | 899 |
| L | GS003 | gsc.py | 900 |
| L | GS003 | gsc.py | 901 |
| L | GS003 | gsc.py | 902 |
| L | GS003 | gsc.py | 903 |
| L | GS003 | gsc.py | 906 |
| L | GS003 | gsc.py | 908 |
| L | GS003 | gsc.py | 978 |
| L | GS003 | gsc.py | 979 |
| L | GS003 | gsc.py | 983 |
| L | GS003 | gsc.py | 1098 |
| L | GS003 | gsc.py | 1169 |
| L | GS003 | gsc.py | 1192 |
| L | GS003 | gsc.py | 1252 |
| L | GS003 | gsc.py | 1263 |
| L | GS003 | gsc.py | 1264 |
| L | GS003 | gsc.py | 1272 |
| L | GS003 | gsc.py | 1280 |
| L | GS003 | gsc.py | 1282 |
| L | GS003 | gsc.py | 1296 |
| L | GS003 | gsc.py | 1308 |
| L | GS003 | gsc.py | 1309 |
| L | GS003 | gsc.py | 1311 |
| L | GS003 | gsc.py | 1324 |
| L | GS003 | gsc.py | 1326 |
| L | GS003 | gsc.py | 1356 |
| L | GS003 | gsc.py | 1357 |
| L | GS003 | gsc.py | 1364 |
| L | GS003 | gsc.py | 1371 |
| L | GS003 | gsc.py | 1381 |
| L | GS003 | gsc.py | 1388 |
| L | GS003 | gsc.py | 1409 |
| L | GS003 | gsc.py | 1419 |
| L | GS003 | gsc.py | 1422 |
| L | GS003 | gsc.py | 1440 |
| L | GS003 | gsc.py | 1446 |
| L | GS003 | gsc.py | 1457 |
| L | GS003 | gsc.py | 1468 |
| L | GS003 | gsc.py | 1472 |
| L | GS003 | gsc.py | 1473 |
| L | GS003 | gsc.py | 1474 |
| L | GS003 | gsc.py | 1475 |
| L | GS003 | gsc.py | 1477 |
| L | GS003 | gsc.py | 1484 |
| L | GS003 | gsc.py | 1491 |
| L | GS003 | gsc.py | 1501 |
| L | GS003 | gsc.py | 1510 |
| L | GS003 | gsc.py | 1512 |
| L | GS003 | gsc.py | 1513 |
| L | GS003 | gsc.py | 1553 |
| L | GS003 | gsc.py | 1581 |
| L | GS003 | gsc.py | 1583 |
| L | GS003 | gsc.py | 1586 |
| L | GS003 | gsc.py | 1614 |
| L | GS003 | gsc.py | 1617 |
| L | GS003 | gsc.py | 1619 |
| L | GS003 | gsc.py | 1620 |
| L | GS003 | gsc.py | 1630 |
| L | GS003 | gsc.py | 1635 |
| L | GS003 | gsc.py | 1638 |
| L | GS003 | gsc.py | 1652 |
| L | GS003 | gsc.py | 1654 |
| L | GS003 | gsc.py | 1655 |
| L | GS003 | gsc.py | 1656 |
| L | GS003 | gsc.py | 1660 |
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
| L | GS008 | batch_and_override.py | 39 |
| L | GS008 | gsc.py | 40 |
| L | GS008 | gsc.py | 53 |
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
| L | GS008 | registry.py | 152 |
| L | GS008 | registry.py | 153 |
| H | ? | bughunter.json | 45 |
| H | ? | terraform.json | 3 |
| H | ? | docker.json | 6 |
| H | ? | sso.yaml | 14 |
| H | ? | gs010_ssh_hardening.py | 81 |
| H | ? | gsc_issue.py | 74 |
| H | ? | framework_aware.py | 21 |
| H | ? | framework_aware.py | 167 |
| H | ? | gsc.py | 667 |
| H | ? | gsc.py | 676 |
| H | ? | gsc.py | 1226 |
| H | ? | gs004_dangerous_subprocess.py | 68 |
| H | ? | gs004_dangerous_subprocess.py | 69 |
| H | ? | gs004_dangerous_subprocess.py | 74 |
| H | ? | gs004_dangerous_subprocess.py | 75 |
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
| C | GS005 | gsc_metrics.py | 39 |
| C | GS005 | gsc_metrics.py | 52 |
| C | GS005 | gsc_metrics.py | 66 |
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
| I | GS007 | gs007_idor.py | 50 |
| I | GS007 | gs007_idor.py | 50 |
| I | GS007 | gs007_idor.py | 52 |
| I | GS007 | gs007_idor.py | 52 |
| I | GS007 | gs007_idor.py | 52 |
| I | GS007 | gs007_idor.py | 164 |
| H | GS007 | gs007_idor.py | 97 |
| H | GS007 | gs007_idor.py | 97 |
| H | GS007 | gs007_idor.py | 97 |
| s | GS009 |  | 0 |
| H | GS012 | gs012_mass_assignment.py | 40 |
| M | GS012 | gsc_issue.py | 90 |
| H | GS014 | gsc_vuln_spider.py | 47 |
| C | GS016 | gs016_linux_priv_esc.py | 31 |
| M | ? | bughunter.json | 32 |
| M | ? | bughunter.json | 33 |
| M | ? | python_async.json | 42 |
| M | ? | python_async.json | 53 |
| M | ? | python_async.json | 74 |
| M | ? | python_async.json | 75 |
| M | ? | gsc_github_dorks.py | 94 |
| M | ? | gsc_doctor.py | 21 |
| M | ? | gsc_doctor.py | 31 |
| M | ? | e4_llm.py | 307 |
| M | ? | gsc_revalidate.py | 74 |
| M | ? | gsc_revalidate.py | 87 |
| M | ? | gsc.py | 88 |
| M | ? | gsc.py | 366 |
| M | ? | gsc.py | 409 |
| M | ? | gsc.py | 526 |
| M | ? | gsc.py | 1159 |
| M | ? | gsc.py | 1161 |
| M | ? | gsc.py | 1163 |
| M | ? | gsc.py | 1780 |
| M | ? | gsc.py | 1783 |
| M | ? | gsc.py | 1786 |
| M | ? | gsc.py | 1799 |
| M | ? | gsc.py | 1801 |
| M | ? | gsc.py | 1808 |
| M | ? | gsc.py | 1812 |
| M | ? | gs009_supply_chain.py | 75 |
| M | ? | gs004_dangerous_subprocess.py | 35 |
| M | ? | gs004_dangerous_subprocess.py | 40 |
| M | ? | gs004_dangerous_subprocess.py | 45 |
| M | ? | gs004_dangerous_subprocess.py | 57 |
| M | ? | go.json | 9 |
| H | ? | rust.json | 7 |

---
*Сгенерировано GSC v0.6 · 2026-07-29T20:11:08.017683*