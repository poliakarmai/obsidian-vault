---
title: "GSC Audit: /home/openclaw/gsc"
date: 2026-08-11
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /home/openclaw/gsc

**Дата:** 11.08.2026 09:08  
**Путь:** `/home/openclaw/gsc`  
**Всего находок:** 2346  
**CRITICAL:** 195 | **HIGH:** 144 | **MEDIUM:** 256 | **LOW:** 571

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 351 |
| YAML-36ACF0AD | 274 |
| GS025-eval_usage | 258 |
| Синхронный код в async | 159 |
| GS003 | 146 |
| GS005 | 131 |
| GS020 | 128 |
| GS022 | 107 |
| GS007 | 95 |
| GS021 | 95 |
| YAML-B39DC08C | 82 |
| GS008 | 76 |
| GS025 | 75 |
| GS015 | 55 |
| GS012 | 36 |
| GS010 | 31 |
| GS001 | 27 |
| GS025-debug_mode | 22 |
| YAML-ECB85AD8 | 21 |
| YAML-A7E2F001 | 20 |
| GS025-hardcoded_secret | 17 |
| GS029 | 15 |
| GS004 | 15 |
| GS019 | 12 |
| GS024 | 11 |
| GS025-wildcard_bind | 8 |
| GS037-debug_true | 7 |
| GS034-token_collector | 6 |
| GS036-redos | 6 |
| GS025-insecure_random | 6 |
| GS037-hardcoded_password | 5 |
| GS011 | 5 |
| GS014 | 5 |
| YAML-SSTI001 | 5 |
| GS002 | 4 |
| GS039-sql_injection_find_by_sql | 3 |
| GS018 | 2 |
| GS032-fake_tool_call_execute | 2 |
| GS035-sql_injection_like | 2 |
| GS036-nosql_injection_where | 2 |
| GS037-sql_injection_format | 2 |
| GS016 | 2 |
| GS032-exfil_env_send | 1 |
| GS032-exfil_git_clone_malicious | 1 |
| GS034-typo_squatting | 1 |
| GS035-sql_injection_get | 1 |
| GS035-sql_injection_concat | 1 |
| GS037-sql_injection_percent | 1 |
| GS037-command_injection_shell_true | 1 |
| GS037-command_injection_os | 1 |
| GS039-sql_injection_where | 1 |
| GS031 | 1 |
| GS009 | 1 |
| GS017 | 1 |
| GS025-permissive_cors | 1 |
| Go: sync.Mutex copy | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | gsc_metrics.py | 31 | OWASP A03: Injection |
| CRITICAL | GS005 | gsc_setup_calibration.py | 8 | OWASP A03: Injection |
| CRITICAL | GS005 | gs018_payment_abuse.py | 215 | OWASP A03: Injection |
| CRITICAL | GS005 | gs020_llm_sqli.py | 126 | OWASP A03: Injection |
| CRITICAL | GS005 | gs020_llm_sqli.py | 230 | OWASP A03: Injection |
| CRITICAL | GS005 | server.py | 685 | OWASP A03: Injection |
| CRITICAL | GS005 | gsc_metrics.py | 31 | OWASP A03: Injection |
| CRITICAL | GS005 | gsc_setup_calibration.py | 8 | OWASP A03: Injection |
| CRITICAL | GS005 | gsc_tp_seed.py | 88 | OWASP A03: Injection |
| CRITICAL | GS005 | gsc_tp_seed.py | 103 | OWASP A03: Injection |
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
| CRITICAL | GS005 | app.py | 13 | OWASP A03: Injection |
| CRITICAL | GS005 | server.py | 353 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | corpus_gs005_python.py | 11 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | corpus_gs005_python.py | 16 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | corpus_gs005_python.py | 24 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | corpus_gs005_python.py | 25 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | gsc_epss.py | 97 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | gsc_metrics.py | 31 |  |
| CRITICAL | GS005 | gsc_setup_calibration.py | 8 |  |
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
| CRITICAL | GS005 | app.py | 13 |  |
| CRITICAL | GS025 | _cron_collect.py | 141 |  |
| CRITICAL | GS025 | gsc_pdf.py | 15 |  |
| CRITICAL | GS025 | gsc.py | 1345 |  |
| CRITICAL | GS025 | gsc_poc_deterministic.py | 140 |  |
| CRITICAL | GS025 | gsc_pdf.py | 15 |  |
| CRITICAL | GS025 | gsc.py | 1345 |  |
| CRITICAL | GS025 | gsc_proofoffix.py | 447 |  |
| CRITICAL | GS025 | gsc_collect_light.py | 212 |  |
| CRITICAL | GS025 | gsc_vuln_spider.py | 29 |  |
| CRITICAL | GS025 | gsc_vuln_spider.py | 187 |  |
| CRITICAL | GS000-LEGACY | _cron_collect.py | 139 |  |
| CRITICAL | GS000-LEGACY | gsc_collect_light.py | 210 |  |
| CRITICAL | GS000-LEGACY | _cron_collect.py | 140 |  |
| CRITICAL | GS000-LEGACY | gsc_collect_light.py | 211 |  |
| CRITICAL | GS000-LEGACY | gsc_vuln_spider.py | 39 |  |
| CRITICAL | GS001 | home.ts | 7 | Found: Pwd: 'Knowledge Base Password' |
| CRITICAL | GS001 | home.ts | 7 | Found: Pwd: '知识库密码' |
| CRITICAL | GS001 | gsc_calibration_real.py | 27 | Found: password="pass" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 15 | Found: TOKEN="ghp_abc123def456" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 10 | Found: password = "SuperSecret123!" |
| CRITICAL | GS001 | main.tf | 5 | Found: access_key = "AKIAIOSFODNN7EXAMPLE" |
| CRITICAL | GS001 | main.tf | 5 | Found: AKIAIOSFODNN7EXAMPLE |
| CRITICAL | GS001 | config.py | 2 | Found: AKIAIOSFODNN7EXAMPLE |
| CRITICAL | GS001 | config.py | 3 | Found: DATABASE_URL = "mysql://admin:secret@localhost/db" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 16 | Found: SECRET: "change-me-in-sealed-secret" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 14 | Found: REDIS_URL: "redis://redis:6379/0" |
| CRITICAL | GS001 | 00-namespace-config.yaml | 25 | Found: DATABASE_URL: "postgresql://gsc_app:CHANGE_ME@postgre |
| CRITICAL | GS001 | config.py | 27 | Found: SECRET = "854cc0d86e61a83bb1dd00c3b23a3cc5b832d45c" |
| CRITICAL | GS001 | config.py | 16 | Found: mysql://root:@localho |
| CRITICAL | GS001 | config.yaml.tmpl | 5 | Found: mysql://root:@localho |
| CRITICAL | GS001 | docker-compose.yml | 11 | Found: PASSWORD: 'true' |
| CRITICAL | GS001 | docker-compose.yml | 42 | Found: mysql://root:@db:3306/te |
| CRITICAL | GS001 | docker-compose.yml | 40 | Found: REDIS_URL: 'redis://redis:6379' |
| CRITICAL | GS001 | docker-compose.yml | 42 | Found: DB_URL: 'mysql://root:@db:3306/test?charset=utf8' |
| CRITICAL | GS001 | config.yaml | 14 | Found: mysql://lyanna:lyanna@lyanna-mariadb:3306/te |
| CRITICAL | GS001 | login.vue | 57 | Found: password: 'admin123' |
| CRITICAL | GS001 | login.js | 1 | Found: password:"admin123" |
| CRITICAL | GS001 | index.js | 5 | Found: 4503599627370496 |
| CRITICAL | GS001 | vendor.js | 5 | Found: 4503599627370496 |
| CRITICAL | GS001 | gsc_calibration_real.py | 27 | Found: password="pass" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 15 | Found: TOKEN="ghp_abc123def456" |
| CRITICAL | GS001 | gsc_setup_calibration.py | 10 | Found: password = "SuperSecret123!" |
| CRITICAL | GS029 | gsc_setup_calibration.py | 10 | Match:     "secrets-demo": ("py", 'password = "SuperSecret12 |
| CRITICAL | GS029 | gsc_setup_calibration.py | 15 | Match:     "hardcoded-secret": ("py", 'API_TOKEN="ghp_abc123 |
| CRITICAL | GS029 | gsc_setup_calibration.py | 10 | Match:     "secrets-demo": ("py", 'password = "SuperSecret12 |
| CRITICAL | GS029 | gsc_setup_calibration.py | 15 | Match:     "hardcoded-secret": ("py", 'API_TOKEN="ghp_abc123 |
| CRITICAL | GS029 | main.tf | 5 | Match: access_key = "AKIAIOSFODNN7EXAMPLE" |
| CRITICAL | GS007 | gsc_setup_calibration.py | 12 | Match:     "pickle-demo": ("py", 'import pickle\ndef load(x) |
| CRITICAL | GS007 | gsc_setup_calibration.py | 12 | Match:     "pickle-demo": ("py", 'import pickle\ndef load(x) |
| CRITICAL | GS007 | gsc_deep_reducer.py | 41 | Match: - **Code Injection**: eval(), exec(), new Function(), |
| CRITICAL | GS007 | app.py | 33 | Match:     return str(pickle.loads(base64.b64decode(data))) |
| CRITICAL | GS031 | Dockerfile | 1 | Match: FROM node:latest |
| CRITICAL | GS029 | main.tf | 5 | Match: access_key = "AKIAIOSFODNN7EXAMPLE" |
| CRITICAL | GS000-LEGACY | systemd.json | 78 | Match:     "detail": "AmbientCapabilities=CAP_ALL grants all |
| CRITICAL | GS005 | tenancy.py | 13 | Line 13: conn.execute(f"ALTER TABLE {t} ENABLE ROW LEVEL SEC |
| CRITICAL | GS005 | tenancy.py | 14 | Line 14: conn.execute(f"ALTER TABLE {t} FORCE ROW LEVEL SECU |
| CRITICAL | GS005 | tenancy.py | 15 | Line 15: conn.execute(f"CREATE POLICY tenant_isolation_{t} O |
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
| CRITICAL | GS007 | admin.py | 52 | Line 52: @bp.route('/admin') |
| CRITICAL | GS016 | gs016_linux_priv_esc.py | 35 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS016 | gs016_linux_priv_esc.py | 35 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS017 | config.py | 3 | Weak DB password in connection string: mysql://admin:secret@ |
| CRITICAL | GS019 | gsc_calibration_real.py | 36 | Session/JWT secret hardcoded in source. Anyone with code acc |
| CRITICAL | GS019 | config.py | 44 | Session/JWT secret hardcoded in source. Anyone with code acc |
| CRITICAL | GS019 | gsc_calibration_real.py | 36 | Session/JWT secret hardcoded in source. Anyone with code acc |
| CRITICAL | GS024 | gs020_llm_sqli.py | 230 | LLM confidence: 100%. The code uses an f-string to interpola |
| CRITICAL | GS024 | gsc_metrics.py | 31 | LLM confidence: 95%. The 'project' variable is interpolated  |
| CRITICAL | GS024 | gsc_metrics.py | 34 | LLM confidence: 95%. The 'project' variable is interpolated  |
| CRITICAL | GS024 | gsc_setup_calibration.py | 8 | LLM confidence: 100%. The code contains an f-string SQL quer |
| CRITICAL | GS024 | corpus_gs005_python.py | 8 | LLM confidence: 100%. The code uses f-strings, % formatting, |
| CRITICAL | GS024 | corpus_gs005_python.py | 9 | LLM confidence: 100%. The code contains multiple SQL injecti |
| CRITICAL | GS024 | corpus_gs005_python.py | 15 | LLM confidence: 100%. All lines use string interpolation or  |
| CRITICAL | GS024 | gs020_llm_sqli.py | 230 | LLM confidence: 100%. The code uses an f-string with user-co |
| CRITICAL | GS024 | gsc_metrics.py | 31 | LLM confidence: 95%. The 'project' variable is directly inte |
| CRITICAL | GS024 | gsc_metrics.py | 34 | LLM confidence: 95%. The 'project' variable is interpolated  |
| CRITICAL | GS024 | gsc_setup_calibration.py | 8 | LLM confidence: 100%. The code creates a demo file containin |
| HIGH | GS000-LEGACY | api.ts | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 24 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 26 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 27 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | page.tsx | 23 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | gsc_issue.py | 74 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | user_auth.py | 60 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | sso.py | 36 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | gsc_issue.py | 74 | User-controlled URL in HTTP request → SSRF. From BugHunter h |
| HIGH | GS000-LEGACY | fastapi_support.py | 38 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | gs012_mass_assignment.py | 44 | Hacking APIs Ch.11 |
| HIGH | GS000-LEGACY | gs012_mass_assignment.py | 44 | Hacking APIs Ch.11 |
| HIGH | GS000-LEGACY | workers.py | 22 | Redteam Kit |
| HIGH | GS000-LEGACY | gsc_vuln_spider.py | 47 | Redteam Kit |
| HIGH | GS025 | _cron_collect.py | 140 |  |
| HIGH | GS025 | gsc_collect_light.py | 211 |  |
| HIGH | GS025 | gsc_vuln_spider.py | 39 |  |
| HIGH | GS025 | gsc.py | 315 |  |
| HIGH | GS025 | gsc_poc_deterministic.py | 74 |  |
| HIGH | GS025 | gsc_poc_deterministic.py | 75 |  |
| HIGH | GS025 | gsc_poc_deterministic.py | 76 |  |
| HIGH | GS025 | gsc.py | 315 |  |
| HIGH | GS025 | _cron_collect.py | 47 |  |
| HIGH | GS025 | _cron_nvd.py | 45 |  |
| HIGH | GS025 | gsc_collect_light.py | 74 |  |
| HIGH | GS025 | gsc_issue.py | 74 |  |
| HIGH | GS025 | user_auth.py | 60 |  |
| HIGH | GS025 | sso.py | 36 |  |
| HIGH | GS025 | gsc_issue.py | 74 |  |
| HIGH | GS025 | gsc_deep_reducer.py | 38 |  |
| HIGH | GS025 | gsc_collect_light.py | 113 |  |
| HIGH | GS025 | gsc_collect_light.py | 126 |  |
| HIGH | GS000-LEGACY | _cron_collect.py | 141 |  |
| HIGH | GS000-LEGACY | gsc_collect_light.py | 212 |  |
| HIGH | GS000-LEGACY | no_debug_true.py | 9 | Match: description = """DEBUG=True in production Django/Flas |
| HIGH | GS000-LEGACY | no_debug_true.py | 11 | Match: patterns = [["\\bDEBUG\\s*=\\s*True\\b", "DEBUG=True  |
| HIGH | GS000-LEGACY | gsc_edu.py | 161 | Match:             "ключами, (3) DEBUG=True с SECRET_KEY в s |
| HIGH | GS000-LEGACY | no_debug_true.py | 9 | Match: description = """DEBUG=True in production Django/Flas |
| HIGH | GS000-LEGACY | no_debug_true.py | 11 | Match: patterns = [["\\bDEBUG\\s*=\\s*True\\b", "DEBUG=True  |
| HIGH | GS000-LEGACY | gsc_issue.py | 74 | Match:     r = requests.post(f"{jira_url}/rest/api/2/issue", |
| HIGH | GS000-LEGACY | user_auth.py | 60 | Match:     user = requests.get(f"{GH_API}/user", |
| HIGH | GS000-LEGACY | sso.py | 36 | Match:     resp = requests.get(f"{issuer_url.rstrip('/')}/.w |
| HIGH | GS000-LEGACY | gsc_issue.py | 74 | Match:     r = requests.post(f"{jira_url}/rest/api/2/issue", |
| HIGH | GS008 | gsc_setup_calibration.py | 11 | Match:     "eval-demo": ("py", 'def exec(u): return eval(u)\ |
| HIGH | GS008 | framework_aware.py | 21 | Match:     "eval() usage": { |
| HIGH | GS008 | framework_aware.py | 167 | Match:         {"title": "eval() usage", "category": "HIGH", |
| HIGH | GS008 | gsc.py | 784 | Match:             "Req 6": ["SQL injection", "eval()", "pic |
| HIGH | GS008 | gsc.py | 793 | Match:             "CC6.8": ["eval()", "pickle.load"], |
| HIGH | GS008 | gsc.py | 1343 | Match:         (2, "HIGH", "eval() or exec() usage", "regex" |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 72 | Match:         "eval() with dynamic input — code injection", |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 73 | Match:         "Never use eval() on user input. Use ast.lite |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 78 | Match:         "exec() on variable — code injection risk", |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 79 | Match:         "Avoid exec(); use explicit function calls or |
| HIGH | GS008 | gs020_xss_injection.py | 38 | Match:     (r'eval\s*\(\s*[\"\'`]', "DOM XSS: eval() with st |
| HIGH | GS008 | reverse_shell.py | 29 | Match:     [r"\bexec\s*\(\s*['\"]/bin/(?:sh|bash)\b", "exec( |
| HIGH | GS008 | no_eval_exec.py | 9 | Match: description = """Use of eval() or exec() with dynamic |
| HIGH | GS008 | no_eval_exec.py | 11 | Match: patterns = [["\\beval\\s*\\(", "eval() call — potenti |
| HIGH | GS008 | gsc_setup_calibration.py | 11 | Match:     "eval-demo": ("py", 'def exec(u): return eval(u)\ |
| HIGH | GS008 | framework_aware.py | 21 | Match:     "eval() usage": { |
| HIGH | GS008 | framework_aware.py | 167 | Match:         {"title": "eval() usage", "category": "HIGH", |
| HIGH | GS008 | gsc.py | 784 | Match:             "Req 6": ["SQL injection", "eval()", "pic |
| HIGH | GS008 | gsc.py | 793 | Match:             "CC6.8": ["eval()", "pickle.load"], |
| HIGH | GS008 | gsc.py | 1343 | Match:         (2, "HIGH", "eval() or exec() usage", "regex" |
| HIGH | GS008 | gsc_deep_reducer.py | 41 | Match: - **Code Injection**: eval(), exec(), new Function(), |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 72 | Match:         "eval() with dynamic input — code injection", |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 73 | Match:         "Never use eval() on user input. Use ast.lite |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 78 | Match:         "exec() on variable — code injection risk", |
| HIGH | GS008 | gs004_dangerous_subprocess.py | 79 | Match:         "Avoid exec(); use explicit function calls or |
| HIGH | GS008 | gs020_xss_injection.py | 38 | Match:     (r'eval\s*\(\s*[\"\'`]', "DOM XSS: eval() with st |
| HIGH | GS008 | reverse_shell.py | 29 | Match:     [r"\bexec\s*\(\s*['\"]/bin/(?:sh|bash)\b", "exec( |
| HIGH | GS008 | no_eval_exec.py | 9 | Match: description = """Use of eval() or exec() with dynamic |
| HIGH | GS008 | no_eval_exec.py | 11 | Match: patterns = [["\\beval\\s*\\(", "eval() call — potenti |
| HIGH | GS008 | run_demo.py | 60 | Match:         "GS008": "Заменить eval() на ast.literal_eval |
| HIGH | GS008 | app.py | 26 | Match:     return str(eval(expr)) |
| HIGH | GS008 | gsc_vuln_spider.py | 31 | Match:         ('"eval(" "request" language:python stars:<20 |
| HIGH | GS000-LEGACY | gsc_pdf.py | 15 | Match:     os.system(f"python3 {os.path.dirname(__file__)}/g |
| HIGH | GS000-LEGACY | gs004_dangerous_subprocess.py | 48 | Match:         "os.system() with .format() — command injecti |
| HIGH | GS000-LEGACY | gsc_pdf.py | 15 | Match:     os.system(f"python3 {os.path.dirname(__file__)}/g |
| HIGH | GS000-LEGACY | gs004_dangerous_subprocess.py | 48 | Match:         "os.system() with .format() — command injecti |
| HIGH | GS000-LEGACY | main.tf | 3 | Match:   acl    = "public-read" |
| HIGH | GS000-LEGACY | systemd.json | 23 | Match:     "title": "Systemd: User=root or absent → runs as  |
| HIGH | GS025 | .mcp.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | redis-master.conf | 0 | File redis-master.conf has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | redis-slave.conf | 0 | File redis-slave.conf has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | nginx.conf | 0 | File nginx.conf has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | supervisord.conf | 0 | File supervisord.conf has permissions -rw-rw-r-- — readable  |
| HIGH | GS004 | llm_server_hybrid.py | 26 | Line 26: ret = os.popen(cmd) |
| HIGH | GS004 | sg_search.py | 57 | Line 57: cmd = os.popen(txt) |
| HIGH | GS004 | daily_smoke.py | 21 | Line 21: cmd = os.popen(txt) |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 54 | Line 54: "os.popen() — deprecated, uses shell", |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 60 | Line 60: "commands.getoutput() — deprecated shell wrapper", |
| HIGH | GS004 | gsc_pdf.py | 15 | Line 15: os.system(f"python3 {os.path.dirname(__file__)}/gsc |
| HIGH | GS004 | gsc_setup_calibration.py | 11 | Line 11: "eval-demo": ("py", 'def exec(u): return eval(u)\n' |
| HIGH | GS004 | gsc_agentless.py | 50 | Line 50: def ssh_exec(host: str, script: str, user: str = "r |
| HIGH | GS004 | gsc_agentless.py | 80 | Line 80: output = ssh_exec(host, HARDENING_SCRIPT, user, key |
| HIGH | GS004 | gsc_agentless.py | 256 | Line 256: output = ssh_exec(host, THREAT_SCRIPT, user, key,  |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 54 | Line 54: "os.popen() — deprecated, uses shell", |
| HIGH | GS004 | gs004_dangerous_subprocess.py | 60 | Line 60: "commands.getoutput() — deprecated shell wrapper", |
| HIGH | GS004 | gsc_verify_fix.py | 84 | Line 84: result = subprocess.run( |
| HIGH | GS004 | gsc_pdf.py | 15 | Line 15: os.system(f"python3 {os.path.dirname(__file__)}/gsc |
| HIGH | GS004 | gsc_setup_calibration.py | 11 | Line 11: "eval-demo": ("py", 'def exec(u): return eval(u)\n' |
| HIGH | GS005 | corpus_gs005_javascript.js | 20 | Line 20: db.collection.find({ $where: `this.name == '${req.q |
| HIGH | GS005 | corpus_gs005_javascript.js | 21 | Line 21: db.collection.find({ name: { $regex: req.params.sea |
| HIGH | GS005 | corpus_gs005_python.py | 46 | Line 46: pd.read_sql(f"SELECT * FROM sales WHERE region = '{ |
| HIGH | GS005 | corpus_gs005_python.py | 49 | Line 49: table.scan(FilterExpression=f"username = '{user}'") |
| HIGH | GS007 | gs007_idor.py | 101 | Line 101: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP- |
| HIGH | GS007 | gs007_idor.py | 101 | Line 101: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP- |
| HIGH | GS007 | gs007_idor.py | 101 | Line 101: (r'\b(?:HTTP_METHOD_OVERRIDE|X-HTTP-Method|X-HTTP- |
| HIGH | GS007 | api.py | 71 | Line 71: @app.get("/api/v2/scans/{scan_id}") |
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
| HIGH | GS011 | gsc_calibration_real.py | 36 | Found JWT secret in code: '\\x02\\x...'. JWT secrets must be |
| HIGH | GS011 | gsc_calibration_real.py | 36 | Found JWT secret in code: '\\x02\\x...'. JWT secrets must be |
| HIGH | GS011 | server.py | 116 | Detected: key = "gsk_" |
| HIGH | GS012 | gs012_mass_assignment.py | 44 | Unpacking request body directly into model enables field inj |
| HIGH | GS012 | gs012_mass_assignment.py | 44 | Unpacking request body directly into model enables field inj |
| HIGH | GS014 | docker-compose.yml | 37 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | docker-compose.yml | 62 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | workers.py | 22 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | gsc_vuln_spider.py | 47 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | 00-namespace-config.yaml | 25 | Database URL contains password in plaintext. Use environment |
| HIGH | GS019 | wechat.py | 579 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | access.py | 10 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | access.py | 95 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | sso.py | 37 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | sso.py | 37 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | GS019 | auth.py | 13 | Session ID not regenerated after login. Vulnerable to sessio |
| HIGH | ? | rust.json | 7 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | gsc_metrics.py | 31 |
| C | GS005 | gsc_setup_calibration.py | 8 |
| C | GS005 | gs018_payment_abuse.py | 215 |
| C | GS005 | gs020_llm_sqli.py | 126 |
| C | GS005 | gs020_llm_sqli.py | 230 |
| C | GS005 | server.py | 685 |
| C | GS005 | gsc_metrics.py | 31 |
| C | GS005 | gsc_setup_calibration.py | 8 |
| C | GS005 | gsc_tp_seed.py | 88 |
| C | GS005 | gsc_tp_seed.py | 103 |
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
| C | GS005 | app.py | 13 |
| M | GS010 | sso.py | 22 |
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
| M | GS010 | gsc.py | 1342 |
| M | GS010 | gsc.py | 1873 |
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
| M | GS010 | gsc.py | 1342 |
| M | GS010 | gsc.py | 1873 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| L | GS000-LEGACY | gsc_external.py | 168 |
| L | GS000-LEGACY | gs001_hardcoded_secret.py | 89 |
| L | GS000-LEGACY | gs025_ai_provenance.py | 28 |
| H | GS000-LEGACY | api.ts | 19 |
| H | GS000-LEGACY | api.ts | 24 |
| H | GS000-LEGACY | api.ts | 26 |
| H | GS000-LEGACY | api.ts | 27 |
| H | GS000-LEGACY | page.tsx | 23 |
| M | GS018 | gsc_setup_calibration.py | 14 |
| M | GS018 | gsc_setup_calibration.py | 14 |
| C | GS005 | server.py | 353 |
| C | GS005 | corpus_gs005_python.py | 11 |
| C | GS005 | corpus_gs005_python.py | 16 |
| C | GS005 | corpus_gs005_python.py | 24 |
| C | GS005 | corpus_gs005_python.py | 25 |
| C | GS005 | gsc_epss.py | 97 |
| H | GS000-LEGACY | gsc_issue.py | 74 |
| H | GS000-LEGACY | user_auth.py | 60 |
| H | GS000-LEGACY | sso.py | 36 |
| H | GS000-LEGACY | gsc_issue.py | 74 |
| H | GS000-LEGACY | fastapi_support.py | 38 |
| H | GS000-LEGACY | gs012_mass_assignment.py | 44 |
| H | GS000-LEGACY | gs012_mass_assignment.py | 44 |
| H | GS000-LEGACY | workers.py | 22 |
| H | GS000-LEGACY | gsc_vuln_spider.py | 47 |
| M | GS025 | _cron_collect.py | 42 |
| M | GS025 | _cron_nvd.py | 40 |
| M | GS025 | gsc_collect_light.py | 69 |
| M | GS007 | gsc_setup_calibration.py | 12 |
| M | GS007 | gsc.py | 784 |
| M | GS007 | gsc.py | 793 |
| M | GS007 | gsc_setup_calibration.py | 12 |
| M | GS007 | gsc.py | 784 |
| M | GS007 | gsc.py | 793 |
| M | GS007 | gsc_deep_reducer.py | 41 |
| M | GS007 | app.py | 33 |
| M | GS007 | gsc_vuln_spider.py | 191 |
| C | GS005 | gsc_metrics.py | 31 |
| C | GS005 | gsc_setup_calibration.py | 8 |
| L | GS005 | gs020_llm_sqli.py | 126 |
| L | GS005 | gs020_llm_sqli.py | 230 |
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
| L | GS005 | gs020_llm_sqli.py | 126 |
| L | GS005 | gs020_llm_sqli.py | 230 |
| C | GS005 | app.py | 13 |
| H | GS025 | _cron_collect.py | 140 |
| L | GS025 | gs011_jwt_vulnerabilities.py | 41 |
| L | GS025 | gs011_jwt_vulnerabilities.py | 41 |
| H | GS025 | gsc_collect_light.py | 211 |
| H | GS025 | gsc_vuln_spider.py | 39 |
| H | GS025 | gsc.py | 315 |
| L | GS025 | gs005_sql_injection.py | 135 |
| H | GS025 | gsc_poc_deterministic.py | 74 |
| H | GS025 | gsc_poc_deterministic.py | 75 |
| H | GS025 | gsc_poc_deterministic.py | 76 |
| H | GS025 | gsc.py | 315 |
| L | GS025 | gs005_sql_injection.py | 135 |
| H | GS025 | _cron_collect.py | 47 |
| L | GS025 | gs016_linux_priv_esc.py | 27 |
| L | GS025 | gs016_linux_priv_esc.py | 40 |
| L | GS025 | gs016_linux_priv_esc.py | 41 |
| L | GS025 | gs016_linux_priv_esc.py | 95 |
| L | GS025 | gs016_linux_priv_esc.py | 129 |
| L | GS025 | gs014_credential_exposure.py | 29 |
| L | GS025 | gs014_credential_exposure.py | 91 |
| L | GS025 | gs014_credential_exposure.py | 92 |
| L | GS025 | gs014_credential_exposure.py | 93 |
| L | GS025 | gs014_credential_exposure.py | 94 |
| L | GS025 | gs014_credential_exposure.py | 98 |
| L | GS025 | gs014_credential_exposure.py | 99 |
| H | GS025 | _cron_nvd.py | 45 |
| L | GS025 | gs016_linux_priv_esc.py | 27 |
| L | GS025 | gs016_linux_priv_esc.py | 40 |
| L | GS025 | gs016_linux_priv_esc.py | 41 |
| L | GS025 | gs016_linux_priv_esc.py | 95 |
| L | GS025 | gs016_linux_priv_esc.py | 129 |
| L | GS025 | gs014_credential_exposure.py | 29 |
| L | GS025 | gs014_credential_exposure.py | 91 |
| L | GS025 | gs014_credential_exposure.py | 92 |
| L | GS025 | gs014_credential_exposure.py | 93 |
| L | GS025 | gs014_credential_exposure.py | 94 |
| L | GS025 | gs014_credential_exposure.py | 98 |
| L | GS025 | gs014_credential_exposure.py | 99 |
| H | GS025 | gsc_collect_light.py | 74 |
| H | GS025 | gsc_issue.py | 74 |
| H | GS025 | user_auth.py | 60 |
| H | GS025 | sso.py | 36 |
| H | GS025 | gsc_issue.py | 74 |
| H | GS025 | gsc_deep_reducer.py | 38 |
| H | GS025 | gsc_collect_light.py | 113 |
| H | GS025 | gsc_collect_light.py | 126 |
| M | GS025 | gsc_setup_calibration.py | 10 |
| M | GS025 | gsc_calibration_real.py | 27 |
| M | GS025 | gsc_calibration_real.py | 36 |
| M | GS025 | gsc_setup_calibration.py | 10 |
| M | GS025 | gsc_calibration_real.py | 27 |
| M | GS025 | gsc_calibration_real.py | 36 |
| M | GS025 | corpus_gs005_python.py | 39 |
| M | GS020 | _cron_collect.py | 33 |
| L | GS020 | multi_lang.py | 45 |
| L | GS020 | multi_lang.py | 46 |
| L | GS020 | gs020_xss_injection.py | 33 |
| L | GS020 | gs020_xss_injection.py | 36 |
| L | GS020 | gs020_xss_injection.py | 50 |
| L | GS020 | gs020_xss_injection.py | 203 |
| M | GS020 | _cron_nvd.py | 31 |
| M | GS020 | server.py | 655 |
| M | GS020 | server.py | 669 |
| M | GS020 | gsc_xss_poc.py | 199 |
| M | GS020 | gsc_tp_seed.py | 34 |
| M | GS020 | gsc_tp_seed.py | 38 |
| M | GS020 | gsc_deep_reducer.py | 45 |
| M | GS020 | gsc_edu.py | 62 |
| M | GS020 | gsc_edu.py | 66 |
| L | GS020 | multi_lang.py | 45 |
| L | GS020 | multi_lang.py | 46 |
| L | GS020 | gs020_xss_injection.py | 33 |
| L | GS020 | gs020_xss_injection.py | 36 |
| L | GS020 | gs020_xss_injection.py | 50 |
| L | GS020 | gs020_xss_injection.py | 203 |
| M | GS020 | gsc_collect_light.py | 60 |
| C | GS025 | _cron_collect.py | 141 |
| C | GS025 | gsc_pdf.py | 15 |
| C | GS025 | gsc.py | 1345 |
| L | GS025 | gs004_dangerous_subprocess.py | 38 |
| L | GS025 | gs004_dangerous_subprocess.py | 43 |
| L | GS025 | gs004_dangerous_subprocess.py | 48 |
| L | GS025 | gs004_dangerous_subprocess.py | 115 |
| C | GS025 | gsc_poc_deterministic.py | 140 |
| C | GS025 | gsc_pdf.py | 15 |
| C | GS025 | gsc.py | 1345 |
| C | GS025 | gsc_proofoffix.py | 447 |
| L | GS025 | gs004_dangerous_subprocess.py | 38 |
| L | GS025 | gs004_dangerous_subprocess.py | 43 |
| L | GS025 | gs004_dangerous_subprocess.py | 48 |
| L | GS025 | gs004_dangerous_subprocess.py | 115 |
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
| M | GS029 | gsc_calibration_real.py | 27 |
| M | GS029 | server.py | 116 |
| M | GS029 | gsc_setup_calibration.py | 10 |
| M | GS029 | gsc_setup_calibration.py | 15 |
| M | GS029 | gsc_calibration_real.py | 27 |
| M | GS029 | corpus_gs005_python.py | 24 |
| M | GS029 | corpus_gs005_python.py | 39 |
| C | GS001 | home.ts | 7 |
| C | GS001 | home.ts | 7 |
| C | GS001 | gsc_calibration_real.py | 27 |
| C | GS001 | gsc_setup_calibration.py | 15 |
| C | GS001 | gsc_setup_calibration.py | 10 |
| C | GS001 | main.tf | 5 |
| C | GS001 | main.tf | 5 |
| C | GS001 | config.py | 2 |
| C | GS001 | config.py | 3 |
| C | GS001 | 00-namespace-config.yaml | 16 |
| C | GS001 | 00-namespace-config.yaml | 14 |
| C | GS001 | 00-namespace-config.yaml | 25 |
| C | GS001 | config.py | 27 |
| C | GS001 | config.py | 16 |
| C | GS001 | config.yaml.tmpl | 5 |
| C | GS001 | docker-compose.yml | 11 |
| C | GS001 | docker-compose.yml | 42 |
| C | GS001 | docker-compose.yml | 40 |
| C | GS001 | docker-compose.yml | 42 |
| C | GS001 | config.yaml | 14 |
| C | GS001 | login.vue | 57 |
| C | GS001 | login.js | 1 |
| C | GS001 | index.js | 5 |
| C | GS001 | vendor.js | 5 |
| C | GS001 | gsc_calibration_real.py | 27 |
| C | GS001 | gsc_setup_calibration.py | 15 |
| C | GS001 | gsc_setup_calibration.py | 10 |
| L | GS003 | embedder.py | 4 |
| L | GS003 | faiss.py | 7 |
| L | GS003 | llm_reranker.py | 4 |
| L | GS003 | splitter.py | 8 |
| L | GS003 | retriever.py | 5 |
| L | GS003 | qalib.py | 130 |
| L | GS003 | get_puyu_model_list.py | 13 |
| L | GS003 | get_puyu_model_list.py | 14 |
| L | GS003 | get_puyu_model_list.py | 15 |
| L | GS003 | update_fs_max_len.py | 18 |
| L | GS003 | update_fs_max_len.py | 23 |
| L | GS003 | commands.py | 34 |
| L | GS003 | commands.py | 36 |
| L | GS003 | commands.py | 38 |
| L | GS003 | ci_report.py | 12 |
| L | GS003 | ci_report.py | 40 |
| L | GS003 | ci_report.py | 42 |
| L | GS003 | ci_report.py | 43 |
| L | GS003 | ci_report.py | 44 |
| L | GS003 | ci_report.py | 45 |
| L | GS003 | ci_report.py | 46 |
| L | GS003 | ci_report.py | 47 |
| L | GS003 | ci_report.py | 48 |
| L | GS003 | ci_report.py | 49 |
| L | GS003 | ci_report.py | 51 |
| L | GS003 | ci_report.py | 52 |
| L | GS003 | ci_report.py | 55 |
| L | GS003 | ci_report.py | 63 |
| L | GS003 | ci_report.py | 65 |
| L | GS003 | ci_report.py | 67 |
| L | GS003 | ci_report.py | 68 |
| L | GS003 | ci_report.py | 71 |
| L | GS003 | ci_report.py | 75 |
| L | GS003 | ci_report.py | 77 |
| L | GS003 | ci_report.py | 78 |
| L | GS003 | ci_report.py | 79 |
| L | GS003 | ci_report.py | 81 |
| L | GS003 | ci_report.py | 82 |
| L | GS003 | ci_report.py | 94 |
| L | GS003 | ci_report.py | 95 |
| L | GS003 | ci_report.py | 100 |
| L | GS003 | gsc_audit_compliance.py | 11 |
| L | GS003 | gsc_audit_compliance.py | 12 |
| L | GS003 | gsc_audit_compliance.py | 15 |
| L | GS003 | gsc_audit_compliance.py | 19 |
| L | GS003 | gsc_audit_compliance.py | 21 |
| L | GS003 | gsc_audit_compliance.py | 25 |
| L | GS003 | gsc_calibration_real.py | 71 |
| L | GS003 | gsc_calibration_real.py | 72 |
| L | GS003 | gsc_doctor.py | 7 |
| L | GS003 | gsc_doctor.py | 8 |
| L | GS003 | gsc_doctor.py | 74 |
| L | GS003 | gsc_stabilize.py | 43 |
| L | GS003 | gsc_stabilize.py | 46 |
| L | GS003 | django_cross_org.py | 33 |
| L | GS003 | run_demo.py | 28 |
| L | GS003 | run_demo.py | 34 |
| L | GS003 | run_demo.py | 38 |
| L | GS003 | run_demo.py | 39 |
| L | GS003 | run_demo.py | 48 |
| L | GS003 | run_demo.py | 50 |
| L | GS003 | run_demo.py | 64 |
| L | GS003 | run_demo.py | 66 |
| L | GS003 | run_demo.py | 76 |
| L | GS003 | run_demo.py | 78 |
| L | GS003 | run_demo.py | 79 |
| L | GS003 | run_demo.py | 80 |
| L | GS003 | run_demo.py | 84 |
| L | GS003 | run_demo.py | 98 |
| L | GS003 | decorators.py | 14 |
| L | GS003 | gsc_chain_composer.py | 88 |
| L | GS003 | gsc_chain_composer.py | 95 |
| L | GS003 | gsc_db.py | 498 |
| L | GS003 | gsc_poc_generator.py | 80 |
| L | GS003 | gsc_poc_generator.py | 88 |
| L | GS003 | config.py | 96 |
| L | GS003 | base.py | 156 |
| L | GS003 | blog.py | 127 |
| L | GS003 | ci_report.py | 12 |
| L | GS003 | ci_report.py | 40 |
| L | GS003 | ci_report.py | 42 |
| L | GS003 | ci_report.py | 43 |
| L | GS003 | ci_report.py | 44 |
| L | GS003 | ci_report.py | 45 |
| L | GS003 | ci_report.py | 46 |
| L | GS003 | ci_report.py | 47 |
| L | GS003 | ci_report.py | 48 |
| L | GS003 | ci_report.py | 49 |
| L | GS003 | ci_report.py | 51 |
| L | GS003 | ci_report.py | 52 |
| L | GS003 | ci_report.py | 55 |
| L | GS003 | ci_report.py | 63 |
| L | GS003 | ci_report.py | 65 |
| L | GS003 | ci_report.py | 67 |
| L | GS003 | ci_report.py | 68 |
| L | GS003 | ci_report.py | 71 |
| L | GS003 | ci_report.py | 75 |
| L | GS003 | ci_report.py | 77 |
| L | GS003 | ci_report.py | 78 |
| L | GS003 | ci_report.py | 79 |
| L | GS003 | ci_report.py | 81 |
| L | GS003 | ci_report.py | 82 |
| L | GS003 | ci_report.py | 94 |
| L | GS003 | ci_report.py | 95 |
| L | GS003 | ci_report.py | 100 |
| L | GS003 | gsc_audit_compliance.py | 11 |
| L | GS003 | gsc_audit_compliance.py | 12 |
| L | GS003 | gsc_audit_compliance.py | 15 |
| L | GS003 | gsc_audit_compliance.py | 19 |
| L | GS003 | gsc_audit_compliance.py | 21 |
| L | GS003 | gsc_audit_compliance.py | 25 |
| L | GS003 | gsc_calibration_real.py | 71 |
| L | GS003 | gsc_calibration_real.py | 72 |
| L | GS003 | gsc_doctor.py | 7 |
| L | GS003 | gsc_doctor.py | 8 |
| L | GS003 | gsc_doctor.py | 74 |
| L | GS003 | gsc_stabilize.py | 43 |
| L | GS003 | gsc_stabilize.py | 46 |
| L | GS003 | build-themes.js | 22 |
| L | GS003 | build-themes.js | 39 |
| L | GS003 | request.js | 22 |
| L | GS003 | request.js | 31 |
| L | GS003 | commonMixin.js | 73 |
| L | GS003 | websocketMixin.js | 30 |
| L | GS003 | websocketMixin.js | 59 |
| L | GS003 | websocketMixin.js | 61 |
| L | GS003 | websocketMixin.js | 80 |
| L | GS003 | websocketMixin.js | 84 |
| L | GS003 | request.js | 23 |
| L | GS003 | request.js | 32 |
| L | GS003 | vite.config.js | 27 |
| L | GS003 | vite.config.js | 109 |
| L | GS003 | blog.js | 151 |
| L | GS003 | blog.js | 153 |
| L | GS003 | blog.js | 176 |
| L | GS003 | blog.js | 178 |
| L | GS003 | blog.js | 39 |
| L | GS003 | blog.js | 39 |
| L | GS003 | blog.js | 39 |
| L | GS003 | blog.js | 39 |
| L | GS003 | index.js | 27 |
| L | GS003 | highlight.min.js | 2 |
| L | GS003 | highlight.min.js | 2 |
| L | GS003 | index.js | 69 |
| L | GS003 | index.js | 69 |
| L | GS003 | index.js | 69 |
| L | GS008 | gsc.py | 46 |
| L | GS008 | gsc.py | 59 |
| L | GS008 | gs020_llm_sqli.py | 28 |
| L | GS008 | gs020_llm_sqli.py | 29 |
| L | GS008 | gsc_pr_commands.py | 10 |
| L | GS008 | batch_and_override.py | 39 |
| L | GS008 | gsc.py | 46 |
| L | GS008 | gsc.py | 59 |
| L | GS008 | gsc_chain_composer.py | 23 |
| L | GS008 | gs020_llm_sqli.py | 28 |
| L | GS008 | gs020_llm_sqli.py | 29 |
| L | GS008 | gsc_github_adapter.py | 34 |
| L | GS008 | gsc_noise_engine.py | 33 |
| L | GS008 | gsc_sbom.py | 23 |
| L | GS008 | gsc_selfhealing.py | 26 |
| L | GS008 | config.py | 20 |
| L | GS008 | config.py | 22 |
| L | GS008 | config.py | 26 |
| L | GS008 | config.py | 29 |
| L | GS008 | config.py | 31 |
| L | GS008 | config.py | 32 |
| L | GS008 | config.py | 33 |
| L | GS008 | config.py | 34 |
| L | GS008 | config.py | 35 |
| L | GS008 | config.py | 36 |
| L | GS008 | config.py | 37 |
| L | GS008 | config.py | 38 |
| L | GS008 | config.py | 39 |
| L | GS008 | config.py | 43 |
| L | GS008 | config.py | 45 |
| L | GS008 | config.py | 46 |
| L | GS008 | config.py | 48 |
| L | GS008 | config.py | 49 |
| L | GS008 | config.py | 50 |
| L | GS008 | config.py | 52 |
| L | GS008 | config.py | 60 |
| L | GS008 | config.py | 61 |
| L | GS008 | config.py | 64 |
| L | GS008 | config.py | 66 |
| L | GS008 | config.py | 67 |
| L | GS008 | config.py | 69 |
| L | GS008 | config.py | 70 |
| L | GS008 | config.py | 72 |
| L | GS008 | gsc_pr_commands.py | 10 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 60 |
| I | GS015 | main.py | 61 |
| I | GS015 | main.py | 62 |
| I | GS015 | main.py | 67 |
| I | GS015 | main.py | 72 |
| I | GS015 | main.py | 60 |
| I | GS015 | main.py | 61 |
| I | GS015 | main.py | 62 |
| I | GS015 | main.py | 67 |
| I | GS015 | main.py | 72 |
| I | GS015 | main.py | 60 |
| I | GS015 | main.py | 61 |
| I | GS015 | main.py | 62 |
| I | GS015 | main.py | 67 |
| I | GS015 | main.py | 72 |
| I | GS015 | main.py | 35 |
| I | GS015 | main.py | 1 |
| I | GS015 | app.py | 136 |
| I | GS015 | app.py | 136 |
| I | GS015 | app.py | 136 |
| I | GS015 | app.py | 26 |
| I | GS015 | app.py | 101 |
| I | GS015 | app.py | 67 |
| I | GS015 | server.py | 179 |
| I | GS015 | server.py | 195 |
| I | GS015 | server.py | 276 |
| I | GS015 | server.py | 307 |
| I | GS015 | server.py | 322 |
| I | GS015 | server.py | 335 |
| I | GS015 | server.py | 345 |
| I | GS015 | server.py | 366 |
| I | GS015 | server.py | 429 |
| I | GS015 | server.py | 442 |
| I | GS015 | server.py | 179 |
| I | GS015 | server.py | 195 |
| I | GS015 | server.py | 276 |
| I | GS015 | server.py | 307 |
| I | GS015 | server.py | 322 |
| I | GS015 | server.py | 335 |
| I | GS015 | server.py | 345 |
| I | GS015 | server.py | 366 |
| I | GS015 | server.py | 429 |
| I | GS015 | server.py | 442 |
| I | GS015 | server.py | 179 |
| I | GS015 | server.py | 195 |
| I | GS015 | server.py | 276 |
| I | GS015 | server.py | 307 |
| I | GS015 | server.py | 322 |
| I | GS015 | server.py | 335 |
| I | GS015 | server.py | 345 |
| I | GS015 | server.py | 366 |
| I | GS015 | server.py | 429 |
| I | GS015 | server.py | 442 |
| I | GS015 | server.py | 48 |
| i | GS020 |  | 136 |
| i | GS020 |  | 135 |
| i | GS020 |  | 184 |
| i | GS020 |  | 192 |
| i | GS020 |  | 267 |
| i | GS020 |  | 141 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 655 |
| i | GS020 |  | 669 |
| i | GS020 |  | 45 |
| i | GS020 |  | 62 |
| i | GS020 |  | 137 |
| i | GS020 |  | 9 |
| i | GS020 |  | 45 |
| i | GS020 |  | 69 |
| i | GS020 |  | 126 |
| i | GS020 |  | 45 |
| i | GS020 |  | 46 |
| i | GS020 |  | 10 |
| i | GS020 |  | 34 |
| i | GS020 |  | 34 |
| i | GS020 |  | 203 |
| i | GS020 |  | 36 |
| i | GS020 |  | 45 |
| i | GS020 |  | 74 |
| i | GS020 |  | 74 |
| i | GS020 |  | 74 |
| i | GS020 |  | 14 |
| i | GS020 |  | 87 |
| i | GS020 |  | 9 |
| i | GS020 |  | 45 |
| i | GS020 |  | 69 |
| i | GS020 |  | 126 |
| i | GS020 |  | 45 |
| i | GS020 |  | 46 |
| i | GS020 |  | 10 |
| i | GS020 |  | 34 |
| i | GS020 |  | 34 |
| i | GS020 |  | 203 |
| i | GS020 |  | 36 |
| i | GS020 |  | 45 |
| i | GS020 |  | 74 |
| i | GS020 |  | 74 |
| i | GS020 |  | 74 |
| i | GS020 |  | 14 |
| i | GS020 |  | 87 |
| i | GS020 |  | 120 |
| i | GS020 |  | 20 |
| i | GS020 |  | 31 |
| i | GS020 |  | 4 |
| i | GS020 |  | 16 |
| i | GS020 |  | 180 |
| i | GS020 |  | 181 |
| i | GS020 |  | 181 |
| i | GS020 |  | 11 |
| i | GS020 |  | 20 |
| i | GS020 |  | 84 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 2 |
| i | GS020 |  | 4 |
| i | GS020 |  | 4 |
| i | GS020 |  | 8 |
| i | GS020 |  | 8 |
| i | GS020 |  | 8 |
| i | GS020 |  | 8 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 4 |
| i | GS020 |  | 8 |
| i | GS020 |  | 9 |
| i | GS020 |  | 4 |
| i | GS020 |  | 4 |
| i | GS020 |  | 4 |
| i | GS020 |  | 8 |
| i | GS020 |  | 8 |
| i | GS020 |  | 8 |
| i | GS020 |  | 8 |
| i | GS020 |  | 9 |
| i | GS020 |  | 9 |
| i | GS020 |  | 4 |
| i | GS020 |  | 8 |
| i | GS020 |  | 9 |
| i | GS020 |  | 4 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 1 |
| i | GS020 |  | 10 |
| i | GS020 |  | 16 |
| i | GS020 |  | 27 |
| ? | GS032-fake_tool_call_execute | app.py | 11 |
| ? | GS032-fake_tool_call_execute | gradio_ui.py | 182 |
| ? | GS032-exfil_env_send | index.js | 27 |
| ? | GS032-exfil_git_clone_malicious | extension.js | 26 |
| ? | GS034-typo_squatting | package.json | 48 |
| ? | GS034-token_collector | route.ts | 3 |
| ? | GS034-token_collector | route.ts | 3 |
| ? | GS034-token_collector | api.ts | 1 |
| ? | GS034-token_collector | next.config.js | 4 |
| ? | GS034-token_collector | index.js | 20 |
| ? | GS034-token_collector | index.js | 27 |
| ? | GS035-sql_injection_get | corpus_gs005_php.php | 6 |
| ? | GS035-sql_injection_concat | corpus_gs005_php.php | 6 |
| ? | GS035-sql_injection_like | corpus_gs005_php.php | 10 |
| ? | GS035-sql_injection_like | corpus_gs005_php.php | 11 |
| ? | GS036-nosql_injection_where | corpus_gs005_javascript.js | 20 |
| ? | GS036-nosql_injection_where | corpus_gs005_javascript.js | 21 |
| ? | GS036-redos | index.js | 27 |
| ? | GS036-redos | index.js | 27 |
| ? | GS036-redos | index.js | 8 |
| ? | GS036-redos | index.js | 64 |
| ? | GS036-redos | vendor.js | 8 |
| ? | GS036-redos | vendor.js | 64 |
| ? | GS037-sql_injection_format | corpus_gs005_python.py | 8 |
| ? | GS037-sql_injection_percent | corpus_gs005_python.py | 9 |
| ? | GS037-debug_true | app.py | 36 |
| ? | GS037-debug_true | config.py | 26 |
| ? | GS037-debug_true | run.py | 7 |
| ? | GS037-debug_true | gsc_deep_reducer.py | 53 |
| ? | GS037-sql_injection_format | gs020_llm_sqli.py | 126 |
| ? | GS037-debug_true | no_debug_true.py | 9 |
| ? | GS037-debug_true | no_debug_true.py | 11 |
| ? | GS037-debug_true | gsc_edu.py | 161 |
| ? | GS037-command_injection_shell_true | gsc_verify_fix.py | 84 |
| ? | GS037-hardcoded_password | config.py | 27 |
| ? | GS037-hardcoded_password | config.py | 44 |
| ? | GS037-hardcoded_password | gsc_calibration_real.py | 27 |
| ? | GS037-command_injection_os | gsc_pdf.py | 15 |
| ? | GS037-hardcoded_password | gsc_setup_calibration.py | 10 |
| ? | GS037-hardcoded_password | gsc_setup_calibration.py | 15 |
| ? | GS039-sql_injection_where | corpus_gs005_ruby.rb | 5 |
| ? | GS039-sql_injection_find_by_sql | corpus_gs005_ruby.rb | 6 |
| ? | GS039-sql_injection_find_by_sql | corpus_gs005_ruby.rb | 7 |
| ? | GS039-sql_injection_find_by_sql | corpus_gs005_ruby.rb | 8 |
| C | GS029 | gsc_setup_calibration.py | 10 |
| C | GS029 | gsc_setup_calibration.py | 15 |
| C | GS029 | gsc_setup_calibration.py | 10 |
| C | GS029 | gsc_setup_calibration.py | 15 |
| C | GS029 | main.tf | 5 |
| H | GS000-LEGACY | no_debug_true.py | 9 |
| H | GS000-LEGACY | no_debug_true.py | 11 |
| H | GS000-LEGACY | gsc_edu.py | 161 |
| H | GS000-LEGACY | no_debug_true.py | 9 |
| H | GS000-LEGACY | no_debug_true.py | 11 |
| M | GS000-LEGACY | gsc_calibration_real.py | 24 |
| M | GS000-LEGACY | gs034_supply_chain.py | 173 |
| M | GS000-LEGACY | gs034_supply_chain.py | 192 |
| M | GS000-LEGACY | gs034_supply_chain.py | 200 |
| M | GS000-LEGACY | gs034_supply_chain.py | 250 |
| M | GS000-LEGACY | gsc_threat_model.py | 157 |
| M | GS000-LEGACY | gsc_threat_model.py | 165 |
| M | GS000-LEGACY | gsc_threat_model.py | 167 |
| M | GS000-LEGACY | gsc_calibration_real.py | 24 |
| M | GS000-LEGACY | gsc_sca.py | 121 |
| M | GS000-LEGACY | gsc_sca.py | 122 |
| M | GS000-LEGACY | gs034_supply_chain.py | 173 |
| M | GS000-LEGACY | gs034_supply_chain.py | 192 |
| M | GS000-LEGACY | gs034_supply_chain.py | 200 |
| M | GS000-LEGACY | gs034_supply_chain.py | 250 |
| H | GS000-LEGACY | gsc_issue.py | 74 |
| H | GS000-LEGACY | user_auth.py | 60 |
| H | GS000-LEGACY | sso.py | 36 |
| H | GS000-LEGACY | gsc_issue.py | 74 |
| H | GS008 | gsc_setup_calibration.py | 11 |
| H | GS008 | framework_aware.py | 21 |
| H | GS008 | framework_aware.py | 167 |
| H | GS008 | gsc.py | 784 |
| H | GS008 | gsc.py | 793 |
| H | GS008 | gsc.py | 1343 |
| H | GS008 | gs004_dangerous_subprocess.py | 72 |
| H | GS008 | gs004_dangerous_subprocess.py | 73 |
| H | GS008 | gs004_dangerous_subprocess.py | 78 |
| H | GS008 | gs004_dangerous_subprocess.py | 79 |
| H | GS008 | gs020_xss_injection.py | 38 |
| H | GS008 | reverse_shell.py | 29 |
| H | GS008 | no_eval_exec.py | 9 |
| H | GS008 | no_eval_exec.py | 11 |
| H | GS008 | gsc_setup_calibration.py | 11 |
| H | GS008 | framework_aware.py | 21 |
| H | GS008 | framework_aware.py | 167 |
| H | GS008 | gsc.py | 784 |
| H | GS008 | gsc.py | 793 |
| H | GS008 | gsc.py | 1343 |
| H | GS008 | gsc_deep_reducer.py | 41 |
| H | GS008 | gs004_dangerous_subprocess.py | 72 |
| H | GS008 | gs004_dangerous_subprocess.py | 73 |
| H | GS008 | gs004_dangerous_subprocess.py | 78 |
| H | GS008 | gs004_dangerous_subprocess.py | 79 |
| H | GS008 | gs020_xss_injection.py | 38 |
| H | GS008 | reverse_shell.py | 29 |
| H | GS008 | no_eval_exec.py | 9 |
| H | GS008 | no_eval_exec.py | 11 |
| H | GS008 | run_demo.py | 60 |
| H | GS008 | app.py | 26 |
| H | GS008 | gsc_vuln_spider.py | 31 |
| C | GS007 | gsc_setup_calibration.py | 12 |
| C | GS007 | gsc_setup_calibration.py | 12 |
| C | GS007 | gsc_deep_reducer.py | 41 |
| C | GS007 | app.py | 33 |
| H | GS000-LEGACY | gsc_pdf.py | 15 |
| H | GS000-LEGACY | gs004_dangerous_subprocess.py | 48 |
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
| H | GS002 | redis-master.conf | 0 |
| H | GS002 | redis-slave.conf | 0 |
| H | GS002 | nginx.conf | 0 |
| H | GS002 | supervisord.conf | 0 |
| H | GS004 | llm_server_hybrid.py | 26 |
| H | GS004 | sg_search.py | 57 |
| H | GS004 | daily_smoke.py | 21 |
| H | GS004 | gs004_dangerous_subprocess.py | 54 |
| H | GS004 | gs004_dangerous_subprocess.py | 60 |
| H | GS004 | gsc_pdf.py | 15 |
| H | GS004 | gsc_setup_calibration.py | 11 |
| H | GS004 | gsc_agentless.py | 50 |
| H | GS004 | gsc_agentless.py | 80 |
| H | GS004 | gsc_agentless.py | 256 |
| H | GS004 | gs004_dangerous_subprocess.py | 54 |
| H | GS004 | gs004_dangerous_subprocess.py | 60 |
| H | GS004 | gsc_verify_fix.py | 84 |
| H | GS004 | gsc_pdf.py | 15 |
| H | GS004 | gsc_setup_calibration.py | 11 |
| C | GS005 | tenancy.py | 13 |
| C | GS005 | tenancy.py | 14 |
| C | GS005 | tenancy.py | 15 |
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
| I | GS007 | api_server.py | 94 |
| I | GS007 | gradio_ui.py | 28 |
| I | GS007 | helper.py | 271 |
| I | GS007 | gs007_idor.py | 54 |
| I | GS007 | gs007_idor.py | 54 |
| I | GS007 | gs007_idor.py | 56 |
| I | GS007 | gs007_idor.py | 56 |
| I | GS007 | gs007_idor.py | 56 |
| I | GS007 | gs007_idor.py | 185 |
| H | GS007 | gs007_idor.py | 101 |
| H | GS007 | gs007_idor.py | 101 |
| H | GS007 | gs007_idor.py | 101 |
| H | GS007 | api.py | 71 |
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
| I | GS007 | gsc_db.py | 445 |
| I | GS007 | gsc_db.py | 465 |
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
| C | GS007 | admin.py | 52 |
| I | GS007 | server.py | 59 |
| I | GS007 | server.py | 67 |
| s | GS009 |  | 0 |
| L | GS011 | str.py | 43 |
| H | GS011 | gsc_calibration_real.py | 36 |
| H | GS011 | gsc_calibration_real.py | 36 |
| L | GS011 | server.py | 150 |
| H | GS011 | server.py | 116 |
| H | GS012 | gs012_mass_assignment.py | 44 |
| M | GS012 | gsc_issue.py | 90 |
| H | GS012 | gs012_mass_assignment.py | 44 |
| L | GS012 | base.py | 158 |
| L | GS012 | blog.py | 268 |
| L | GS012 | blog.py | 479 |
| L | GS012 | react.py | 52 |
| L | GS012 | react.py | 70 |
| L | GS012 | index.js | 1 |
| L | GS012 | index.js | 1 |
| L | GS012 | index.js | 1 |
| L | GS012 | index.js | 6 |
| L | GS012 | index.js | 6 |
| L | GS012 | index.js | 6 |
| L | GS012 | index.js | 20 |
| L | GS012 | index.js | 20 |
| L | GS012 | index.js | 20 |
| L | GS012 | index.js | 27 |
| L | GS012 | topic-detail.js | 8 |
| L | GS012 | topic-detail.js | 8 |
| L | GS012 | index.js | 4 |
| L | GS012 | index.js | 4 |
| L | GS012 | index.js | 9 |
| L | GS012 | index.js | 9 |
| L | GS012 | vendor.js | 4 |
| L | GS012 | vendor.js | 4 |
| L | GS012 | vendor.js | 9 |
| L | GS012 | vendor.js | 9 |
| L | GS012 | tasks.py | 90 |
| L | GS012 | tasks.py | 118 |
| L | GS012 | admin.py | 132 |
| L | GS012 | admin.py | 229 |
| L | GS012 | admin.py | 289 |
| L | GS012 | admin.py | 375 |
| L | GS012 | admin.py | 465 |
| M | GS012 | gsc_issue.py | 90 |
| H | GS014 | docker-compose.yml | 37 |
| H | GS014 | docker-compose.yml | 62 |
| H | GS014 | workers.py | 22 |
| H | GS014 | gsc_vuln_spider.py | 47 |
| H | GS014 | 00-namespace-config.yaml | 25 |
| C | GS016 | gs016_linux_priv_esc.py | 35 |
| C | GS016 | gs016_linux_priv_esc.py | 35 |
| C | GS017 | config.py | 3 |
| H | GS019 | wechat.py | 579 |
| H | GS019 | access.py | 10 |
| H | GS019 | access.py | 95 |
| H | GS019 | sso.py | 37 |
| M | GS019 | gs021_csrf_ssrf.py | 37 |
| C | GS019 | gsc_calibration_real.py | 36 |
| H | GS019 | sso.py | 37 |
| H | GS019 | auth.py | 13 |
| M | GS019 | auth.py | 101 |
| M | GS019 | gs021_csrf_ssrf.py | 37 |
| C | GS019 | config.py | 44 |
| C | GS019 | gsc_calibration_real.py | 36 |
| s | GS021 |  | 43 |
| s | GS021 |  | 45 |
| s | GS021 |  | 46 |
| s | GS021 |  | 47 |
| s | GS021 |  | 56 |
| s | GS021 |  | 66 |
| s | GS021 |  | 28 |
| s | GS021 |  | 4 |
| s | GS021 |  | 8 |
| s | GS021 |  | 17 |
| s | GS021 |  | 65 |
| s | GS021 |  | 6 |
| s | GS021 |  | 4 |
| s | GS021 |  | 8 |
| s | GS021 |  | 17 |
| s | GS021 |  | 65 |
| s | GS021 |  | 6 |
| s | GS021 |  | 8 |
| s | GS021 |  | 4 |
| s | GS021 |  | 10 |
| s | GS021 |  | 81 |
| s | GS021 |  | 225 |
| s | GS021 |  | 226 |
| s | GS021 |  | 198 |
| s | GS021 |  | 198 |
| s | GS021 |  | 1356 |
| s | GS021 |  | 1356 |
| s | GS021 |  | 228 |
| s | GS021 |  | 39 |
| s | GS021 |  | 704 |
| s | GS021 |  | 171 |
| s | GS021 |  | 74 |
| s | GS021 |  | 105 |
| s | GS021 |  | 1095 |
| s | GS021 |  | 2199 |
| s | GS021 |  | 2199 |
| s | GS021 |  | 128 |
| s | GS021 |  | 123 |
| s | GS021 |  | 38 |
| s | GS021 |  | 39 |
| s | GS021 |  | 40 |
| s | GS021 |  | 41 |
| s | GS021 |  | 413 |
| s | GS021 |  | 119 |
| s | GS021 |  | 28 |
| s | GS021 |  | 22 |
| c | GS021 |  | 46 |
| s | GS021 |  | 16 |
| s | GS021 |  | 17 |
| s | GS021 |  | 21 |
| s | GS021 |  | 25 |
| s | GS021 |  | 143 |
| c | GS021 |  | 24 |
| c | GS021 |  | 31 |
| c | GS021 |  | 31 |
| c | GS021 |  | 39 |
| c | GS021 |  | 41 |
| s | GS021 |  | 53 |
| s | GS021 |  | 53 |
| s | GS021 |  | 10 |
| s | GS021 |  | 55 |
| s | GS021 |  | 55 |
| s | GS021 |  | 16 |
| s | GS021 |  | 99 |
| s | GS021 |  | 1095 |
| s | GS021 |  | 2199 |
| s | GS021 |  | 2199 |
| c | GS021 |  | 31 |
| c | GS021 |  | 31 |
| c | GS021 |  | 39 |
| c | GS021 |  | 41 |
| s | GS021 |  | 53 |
| s | GS021 |  | 53 |
| s | GS021 |  | 10 |
| s | GS021 |  | 55 |
| s | GS021 |  | 55 |
| s | GS021 |  | 16 |
| s | GS021 |  | 99 |
| s | GS021 |  | 99 |
| s | GS021 |  | 243 |
| s | GS021 |  | 117 |
| s | GS021 |  | 149 |
| s | GS021 |  | 39 |
| s | GS021 |  | 58 |
| c | GS021 |  | 66 |
| c | GS021 |  | 79 |
| s | GS021 |  | 193 |
| s | GS021 |  | 877 |
| s | GS021 |  | 563 |
| s | GS021 |  | 28 |
| s | GS021 |  | 29 |
| s | GS021 |  | 205 |
| s | GS021 |  | 454 |
| s | GS021 |  | 3 |
| s | GS021 |  | 106 |
| r | GS022 |  | 53 |
| r | GS022 |  | 69 |
| r | GS022 |  | 19 |
| r | GS022 |  | 15 |
| r | GS022 |  | 36 |
| r | GS022 |  | 116 |
| r | GS022 |  | 179 |
| r | GS022 |  | 189 |
| r | GS022 |  | 10 |
| r | GS022 |  | 22 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 8 |
| r | GS022 |  | 8 |
| r | GS022 |  | 8 |
| r | GS022 |  | 8 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 6 |
| r | GS022 |  | 8 |
| r | GS022 |  | 8 |
| r | GS022 |  | 8 |
| r | GS022 |  | 8 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 9 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 1 |
| r | GS022 |  | 53 |
| r | GS022 |  | 174 |
| r | GS022 |  | 6 |
| r | GS022 |  | 45 |
| r | GS022 |  | 187 |
| r | GS022 |  | 223 |
| r | GS022 |  | 26 |
| r | GS022 |  | 46 |
| r | GS022 |  | 73 |
| r | GS022 |  | 44 |
| r | GS022 |  | 142 |
| r | GS022 |  | 680 |
| r | GS022 |  | 23 |
| r | GS022 |  | 24 |
| r | GS022 |  | 53 |
| r | GS022 |  | 18 |
| r | GS022 |  | 29 |
| r | GS022 |  | 81 |
| r | GS022 |  | 34 |
| r | GS022 |  | 45 |
| r | GS022 |  | 13 |
| r | GS022 |  | 32 |
| r | GS022 |  | 54 |
| r | GS022 |  | 34 |
| r | GS022 |  | 45 |
| r | GS022 |  | 13 |
| r | GS022 |  | 46 |
| r | GS022 |  | 51 |
| r | GS022 |  | 234 |
| r | GS022 |  | 292 |
| r | GS022 |  | 296 |
| r | GS022 |  | 49 |
| r | GS022 |  | 52 |
| r | GS022 |  | 58 |
| r | GS022 |  | 758 |
| r | GS022 |  | 833 |
| r | GS022 |  | 101 |
| r | GS022 |  | 174 |
| r | GS022 |  | 246 |
| r | GS022 |  | 359 |
| r | GS022 |  | 365 |
| r | GS022 |  | 63 |
| r | GS022 |  | 52 |
| r | GS022 |  | 405 |
| r | GS022 |  | 448 |
| r | GS022 |  | 53 |
| r | GS022 |  | 56 |
| r | GS022 |  | 71 |
| r | GS022 |  | 70 |
| r | GS022 |  | 126 |
| r | GS022 |  | 146 |
| r | GS022 |  | 228 |
| r | GS022 |  | 346 |
| r | GS022 |  | 505 |
| r | GS022 |  | 198 |
| r | GS022 |  | 27 |
| r | GS022 |  | 39 |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
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
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
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
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-permissive_cors |  | ? |
| ? | GS025-debug_mode |  | ? |
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
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-wildcard_bind |  | ? |
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
| ? | GS025-insecure_random |  | ? |
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
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
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
| ? | GS025-insecure_random |  | ? |
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
| ? | GS025-insecure_random |  | ? |
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
| ? | GS025-insecure_random |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-wildcard_bind |  | ? |
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
| ? | GS025-debug_mode |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| C | GS024 | gs020_llm_sqli.py | 230 |
| C | GS024 | gsc_metrics.py | 31 |
| C | GS024 | gsc_metrics.py | 34 |
| C | GS024 | gsc_setup_calibration.py | 8 |
| C | GS024 | corpus_gs005_python.py | 8 |
| C | GS024 | corpus_gs005_python.py | 9 |
| C | GS024 | corpus_gs005_python.py | 15 |
| C | GS024 | gs020_llm_sqli.py | 230 |
| C | GS024 | gsc_metrics.py | 31 |
| C | GS024 | gsc_metrics.py | 34 |
| C | GS024 | gsc_setup_calibration.py | 8 |
| ? | YAML-36ACF0AD | embedder.py | ? |
| ? | YAML-36ACF0AD | llm_reranker.py | ? |
| ? | YAML-36ACF0AD | llm_server_hybrid.py | ? |
| ? | YAML-36ACF0AD | llm_server_hybrid.py | ? |
| ? | YAML-36ACF0AD | llm_server_hybrid.py | ? |
| ? | YAML-36ACF0AD | llm_server_hybrid.py | ? |
| ? | YAML-36ACF0AD | gsc.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gsc.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gsc.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gsc.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gsc.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gsc.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs020_xss_injection.py | ? |
| ? | YAML-36ACF0AD | gs035_php.py | ? |
| ? | YAML-36ACF0AD | gs035_php.py | ? |
| ? | YAML-36ACF0AD | gs036_nodejs.py | ? |
| ? | YAML-36ACF0AD | gs036_nodejs.py | ? |
| ? | YAML-36ACF0AD | gs037_python.py | ? |
| ? | YAML-36ACF0AD | gs037_python.py | ? |
| ? | YAML-36ACF0AD | gs039_ruby.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | reverse_shell.py | ? |
| ? | YAML-36ACF0AD | framework_aware.py | ? |
| ? | YAML-36ACF0AD | framework_aware.py | ? |
| ? | YAML-36ACF0AD | gsc_setup_calibration.py | ? |
| ? | YAML-36ACF0AD | gsc_setup_calibration.py | ? |
| ? | YAML-36ACF0AD | demo_report.json | ? |
| ? | YAML-36ACF0AD | demo_report.json | ? |
| ? | YAML-36ACF0AD | app.py | ? |
| ? | YAML-36ACF0AD | app.py | ? |
| ? | YAML-36ACF0AD | run_demo.py | ? |
| ? | YAML-36ACF0AD | sample.yml | ? |
| ? | YAML-36ACF0AD | sample.yml | ? |
| ? | YAML-36ACF0AD | sample.yml | ? |
| ? | YAML-36ACF0AD | sample.yml | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gsc.py | ? |
| ? | YAML-36ACF0AD | gsc_vuln_spider.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gsc_vuln_spider.py | ? |
| ? | YAML-36ACF0AD | gsc_deep_reducer.py | ? |
| ? | YAML-36ACF0AD | gsc_deep_reducer.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs020_xss_injection.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs025_ai_code.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs025_ai_code.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs035_php.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs036_nodejs.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs037_python.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs037_python.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs039_ruby.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs004_dangerous_subprocess.py | ? |
| ? | YAML-36ACF0AD | gs020_xss_injection.py | ? |
| ? | YAML-36ACF0AD | gs035_php.py | ? |
| ? | YAML-36ACF0AD | gs035_php.py | ? |
| ? | YAML-36ACF0AD | gs036_nodejs.py | ? |
| ? | YAML-36ACF0AD | gs036_nodejs.py | ? |
| ? | YAML-36ACF0AD | gs037_python.py | ? |
| ? | YAML-36ACF0AD | gs037_python.py | ? |
| ? | YAML-36ACF0AD | gs039_ruby.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | no_eval_exec.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | no_eval_exec.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | no_eval_exec.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | reverse_shell.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | no_eval_exec.py | ? |
| ? | YAML-36ACF0AD | reverse_shell.py | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.py | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.py | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.py | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.py | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.py | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.py | ? |
| ? | YAML-36ACF0AD | gsc_yaml_rules.py | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | blog.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | search.js | ? |
| ? | YAML-36ACF0AD | social-sharer.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | post-detail.js | ? |
| ? | YAML-36ACF0AD | topic-detail.js | ? |
| ? | YAML-36ACF0AD | topic-detail.js | ? |
| ? | YAML-36ACF0AD | topic-detail.js | ? |
| ? | YAML-36ACF0AD | topic-detail.js | ? |
| ? | YAML-36ACF0AD | topic-detail.js | ? |
| ? | YAML-36ACF0AD | highlight.min.js | ? |
| ? | YAML-36ACF0AD | highlight.min.js | ? |
| ? | YAML-36ACF0AD | highlight.min.js | ? |
| ? | YAML-36ACF0AD | highlight.min.js | ? |
| ? | YAML-36ACF0AD | highlight.min.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | index.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | vendor.js | ? |
| ? | YAML-36ACF0AD | bughunter.json | ? |
| ? | YAML-36ACF0AD | typescript.json | ? |
| ? | YAML-36ACF0AD | typescript.json | ? |
| ? | YAML-36ACF0AD | framework_aware.cpython-311.pyc | ? |
| ? | YAML-36ACF0AD | framework_aware.cpython-312.pyc | ? |
| ? | YAML-36ACF0AD | framework_aware.py | ? |
| ? | YAML-36ACF0AD | framework_aware.py | ? |
| ? | YAML-36ACF0AD | gsc_setup_calibration.py | ? |
| ? | YAML-36ACF0AD | gsc_setup_calibration.py | ? |
| ? | YAML-ECB85AD8 | gsc_edu.cpython-312.pyc | ? |
| ? | YAML-ECB85AD8 | gsc_yaml_rules.cpython-312.pyc | ? |
| ? | YAML-ECB85AD8 | gsc_yaml_rules.cpython-312.pyc | ? |
| ? | YAML-ECB85AD8 | gs037_python.py | ? |
| ? | YAML-ECB85AD8 | no_debug_true.py | ? |
| ? | YAML-ECB85AD8 | no_debug_true.py | ? |
| ? | YAML-ECB85AD8 | no_debug_true.py | ? |
| ? | YAML-ECB85AD8 | config.py | ? |
| ? | YAML-ECB85AD8 | sample.yml | ? |
| ? | YAML-ECB85AD8 | sample.yml | ? |
| ? | YAML-ECB85AD8 | gs025_ai_code.cpython-312.pyc | ? |
| ? | YAML-ECB85AD8 | gs037_python.cpython-312.pyc | ? |
| ? | YAML-ECB85AD8 | gs037_python.py | ? |
| ? | YAML-ECB85AD8 | no_debug_true.cpython-312.pyc | ? |
| ? | YAML-ECB85AD8 | no_debug_true.cpython-312.pyc | ? |
| ? | YAML-ECB85AD8 | no_debug_true.py | ? |
| ? | YAML-ECB85AD8 | no_debug_true.py | ? |
| ? | YAML-ECB85AD8 | no_debug_true.py | ? |
| ? | YAML-ECB85AD8 | gsc_edu.py | ? |
| ? | YAML-ECB85AD8 | gsc_yaml_rules.py | ? |
| ? | YAML-ECB85AD8 | gsc_yaml_rules.py | ? |
| ? | YAML-B39DC08C | rag_example_output.json | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | handlerDB.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | commands.py | ? |
| ? | YAML-B39DC08C | tasks.py | ? |
| ? | YAML-B39DC08C | tasks.py | ? |
| ? | YAML-B39DC08C | tasks.py | ? |
| ? | YAML-B39DC08C | gsc.cpython-311.pyc | ? |
| ? | YAML-B39DC08C | gsc.cpython-312.pyc | ? |
| ? | YAML-B39DC08C | gsc_edu.cpython-312.pyc | ? |
| ? | YAML-B39DC08C | gsc_yaml_rules.cpython-312.pyc | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | no_print_secrets.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | gsc_config.py | ? |
| ? | YAML-B39DC08C | gsc_config.py | ? |
| ? | YAML-B39DC08C | gsc_config.py | ? |
| ? | YAML-B39DC08C | gsc_issue.py | ? |
| ? | YAML-B39DC08C | gsc_pr_comment.py | ? |
| ? | YAML-B39DC08C | github_oidc.py | ? |
| ? | YAML-B39DC08C | github_oidc.py | ? |
| ? | YAML-B39DC08C | github_oidc.py | ? |
| ? | YAML-B39DC08C | manage.py | ? |
| ? | YAML-B39DC08C | manage.py | ? |
| ? | YAML-B39DC08C | themes.py | ? |
| ? | YAML-B39DC08C | themes.py | ? |
| ? | YAML-B39DC08C | graph.html | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc.py | ? |
| ? | YAML-B39DC08C | gsc_agentless.py | ? |
| ? | YAML-B39DC08C | gsc_archaeology.py | ? |
| ? | YAML-B39DC08C | gsc_check_run.py | ? |
| ? | YAML-B39DC08C | gsc_crossrepo_secrets.py | ? |
| ? | YAML-B39DC08C | gsc_crossrepo_secrets.py | ? |
| ? | YAML-B39DC08C | no_print_secrets.cpython-312.pyc | ? |
| ? | YAML-B39DC08C | no_print_secrets.py | ? |
| ? | YAML-B39DC08C | gsc_edu.py | ? |
| ? | YAML-B39DC08C | gsc_github_adapter.py | ? |
| ? | YAML-B39DC08C | gsc_github_adapter.py | ? |
| ? | YAML-B39DC08C | gsc_selfhealing.py | ? |
| ? | YAML-B39DC08C | gsc_selfhealing.py | ? |
| ? | YAML-B39DC08C | gsc_verify_fix.py | ? |
| ? | YAML-B39DC08C | batch_revalidate.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | db_encrypt.py | ? |
| ? | YAML-B39DC08C | gsc_config.py | ? |
| ? | YAML-B39DC08C | gsc_config.py | ? |
| ? | YAML-B39DC08C | gsc_config.py | ? |
| ? | YAML-B39DC08C | gsc_issue.py | ? |
| ? | YAML-B39DC08C | gsc_pr_comment.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.cpython-312.pyc | ? |
| ? | YAML-A7E2F001 | reverse_shell.cpython-312.pyc | ? |
| ? | YAML-A7E2F001 | reverse_shell.cpython-312.pyc | ? |
| ? | YAML-A7E2F001 | reverse_shell.cpython-312.pyc | ? |
| ? | YAML-A7E2F001 | reverse_shell.cpython-312.pyc | ? |
| ? | YAML-A7E2F001 | reverse_shell.cpython-312.pyc | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-A7E2F001 | reverse_shell.py | ? |
| ? | YAML-SSTI001 | gsc_poc_deterministic.cpython-312.pyc | ? |
| ? | YAML-SSTI001 | ssti_injection.py | ? |
| ? | YAML-SSTI001 | ssti_injection.cpython-312.pyc | ? |
| ? | YAML-SSTI001 | ssti_injection.py | ? |
| ? | YAML-SSTI001 | gsc_poc_deterministic.py | ? |
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
| M | ? | gsc.py | 94 |
| M | ? | gsc.py | 474 |
| M | ? | gsc.py | 527 |
| M | ? | gsc.py | 643 |
| M | ? | gsc.py | 1276 |
| M | ? | gsc.py | 1278 |
| M | ? | gsc.py | 1280 |
| M | ? | gsc.py | 2137 |
| M | ? | gsc.py | 2145 |
| M | ? | gsc.py | 2162 |
| M | ? | gsc.py | 2289 |
| M | ? | gsc.py | 2301 |
| M | ? | gsc.py | 2311 |
| M | ? | gsc.py | 2319 |
| M | ? | gsc.py | 2324 |
| M | ? | gsc.py | 2327 |
| M | ? | gsc.py | 2330 |
| M | ? | gsc.py | 2343 |
| M | ? | gsc.py | 2345 |
| M | ? | gsc.py | 2370 |
| M | ? | gsc.py | 2376 |
| M | ? | gsc.py | 2393 |
| M | ? | gsc.py | 2396 |
| M | ? | gsc.py | 2405 |
| M | ? | gsc.py | 2413 |
| M | ? | gsc.py | 2417 |
| M | ? | gsc.py | 2421 |
| M | ? | gsc.py | 2446 |
| M | ? | gsc.py | 2449 |
| M | ? | gsc.py | 2459 |
| M | ? | gs009_supply_chain.py | 79 |
| M | ? | gs004_dangerous_subprocess.py | 39 |
| M | ? | gs004_dangerous_subprocess.py | 44 |
| M | ? | gs004_dangerous_subprocess.py | 49 |
| M | ? | gs004_dangerous_subprocess.py | 61 |
| M | ? | gsc_agentless.py | 57 |
| M | ? | gsc_external.py | 756 |
| M | ? | gsc_external.py | 761 |
| M | ? | gsc_external.py | 786 |
| M | ? | gsc_external.py | 788 |
| M | ? | gsc_external.py | 799 |
| M | ? | gsc_external.py | 818 |
| M | ? | gsc_external.py | 820 |
| M | ? | gsc_external.py | 940 |
| M | ? | gsc_external.py | 944 |
| M | ? | gsc_external.py | 1015 |
| M | ? | gsc_external.py | 1021 |
| M | ? | gsc_external.py | 1028 |
| M | ? | gsc_external.py | 1071 |
| M | ? | gsc_verify_fix.py | 55 |
| M | ? | gsc_verify_fix.py | 84 |
| M | ? | gsc_verify_fix.py | 101 |
| M | ? | gsc_verify_fix.py | 119 |
| M | ? | bughunter.json | 32 |
| M | ? | bughunter.json | 33 |
| M | ? | python_async.json | 42 |
| M | ? | python_async.json | 53 |
| M | ? | python_async.json | 74 |
| M | ? | python_async.json | 75 |
| M | ? | gsc_check_run.py | 25 |
| M | ? | github_worker.py | 35 |
| M | ? | github_worker.py | 38 |
| M | ? | github_worker.py | 58 |
| M | ? | workers.py | 115 |
| M | ? | github_oidc.py | 200 |
| M | ? | worker.py | 46 |
| M | ? | server.py | 221 |
| M | ? | server.py | 229 |
| M | ? | gsc_poc_deterministic.py | 117 |
| M | ? | gsc_noise_engine.py | 47 |
| M | ? | gsc_xss_poc.py | 56 |
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
| M | ? | gsc_pr_feedback.py | 28 |
| M | ? | e4_llm.py | 307 |
| M | ? | gsc_github_adapter.py | 488 |
| M | ? | gsc_github_adapter.py | 489 |
| M | ? | gsc_github_adapter.py | 511 |
| M | ? | gsc_github_adapter.py | 577 |
| M | ? | gsc_revalidate.py | 78 |
| M | ? | gsc_revalidate.py | 91 |
| M | ? | gsc.py | 94 |
| M | ? | gsc.py | 474 |
| M | ? | gsc.py | 527 |
| M | ? | gsc.py | 643 |
| M | ? | gsc.py | 1276 |
| M | ? | gsc.py | 1278 |
| M | ? | gsc.py | 1280 |
| M | ? | gsc.py | 2137 |
| M | ? | gsc.py | 2145 |
| M | ? | gsc.py | 2162 |
| M | ? | gsc.py | 2312 |
| M | ? | gsc.py | 2324 |
| M | ? | gsc.py | 2334 |
| M | ? | gsc.py | 2342 |
| M | ? | gsc.py | 2347 |
| M | ? | gsc.py | 2350 |
| M | ? | gsc.py | 2353 |
| M | ? | gsc.py | 2366 |
| M | ? | gsc.py | 2368 |
| M | ? | gsc.py | 2393 |
| M | ? | gsc.py | 2399 |
| M | ? | gsc.py | 2416 |
| M | ? | gsc.py | 2419 |
| M | ? | gsc.py | 2428 |
| M | ? | gsc.py | 2436 |
| M | ? | gsc.py | 2440 |
| M | ? | gsc.py | 2444 |
| M | ? | gsc.py | 2452 |
| M | ? | gsc.py | 2459 |
| M | ? | gsc.py | 2467 |
| M | ? | gsc.py | 2492 |
| M | ? | gsc.py | 2495 |
| M | ? | gsc.py | 2505 |
| M | ? | gsc_archaeology.py | 75 |
| M | ? | gsc_archaeology.py | 97 |
| M | ? | runner.py | 88 |
| M | ? | action.yml | 68 |
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
| M | ? | run_demo.py | 19 |
| M | ? | go.json | 9 |
| H | ? | rust.json | 7 |

---
*Сгенерировано GSC v0.6 · 2026-08-11T09:08:56.121064*