---
title: "GSC Audit: /tmp/gsc-calibration/pygoat"
date: 2026-08-07
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-calibration/pygoat

**Дата:** 07.08.2026 11:48  
**Путь:** `/tmp/gsc-calibration/pygoat`  
**Всего находок:** 371  
**CRITICAL:** 34 | **HIGH:** 53 | **MEDIUM:** 65 | **LOW:** 114

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS003 | 57 |
| GS021 | 43 |
| GS015 | 42 |
| Bare except: | 40 |
| GS008 | 35 |
| Python: File upload without content-type validation | 22 |
| GS001 | 20 |
| GS012 | 19 |
| Хардкод IP адреса | 15 |
| CVE-2026-37270: Hardcoded credential | 9 |
| CVE-2026-56318: Information disclosure | 8 |
| GS011 | 7 |
| Hardcoded encryption key | 6 |
| GS020 | 5 |
| GS019 | 5 |
| CVE-2026-55223: Insecure deserialization | 4 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 3 |
| eval() or exec() usage | 3 |
| GS025-debug_mode | 3 |
| GS025-no_rate_limit_auth | 3 |
| GS025-eval_usage | 3 |
| GS025-hardcoded_secret | 3 |
| Python: raw string concatenation in SQL | 2 |
| Debug mode enabled | 2 |
| pickle.load() — unsafe deserialization | 2 |
| GS004 | 2 |
| GS025-wildcard_bind | 2 |
| Open redirect: user-supplied URL | 1 |
| CVE-2026-56413: Command injection | 1 |
| Outdated dependency pattern | 1 |
| World-readable file: docker-compose.yml (664) | 1 |
| GS009 | 1 |
| Синхронный код в async | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | ? | views.py | 158 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | views.py | 864 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | ? | mitre.py | 233 |  |
| CRITICAL | GS001 | views.py | 56 | Found: 4111111111111111 |
| CRITICAL | GS001 | views.py | 80 | Found: 4111111111111111 |
| CRITICAL | GS001 | views.py | 96 | Found: 4111111111111111 |
| CRITICAL | GS001 | entrypoint.sh | 11 | Found: api_key='demokey123456789' |
| CRITICAL | GS001 | entrypoint.sh | 11 | Found: 4111111111111111 |
| CRITICAL | GS001 | mitre.py | 169 | Found: 'HS256' |
| CRITICAL | GS001 | mitre.py | 182 | Found: 'HS256' |
| CRITICAL | GS001 | mitre.py | 194 | Found: 'HS256' |
| CRITICAL | GS001 | a9.js | 18 | Found: eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpZCI6MSwiZXhw |
| CRITICAL | GS001 | sql.html | 63 | Found: password='<b>anything' |
| CRITICAL | GS001 | sec_mis_lab3.html | 30 | Found: 'HS256' |
| CRITICAL | GS001 | sec_mis_lab3.html | 40 | Found: 'HS256' |
| CRITICAL | GS001 | injection.html | 72 | Found: password='<b>anything' |
| CRITICAL | GS001 | mitre_top3.html | 65 | Found: password='<b>anything' |
| CRITICAL | GS001 | views.py | 866 | Found: password="65079b006e85a7e798abecb99e47c154" |
| CRITICAL | GS001 | views.py | 868 | Found: password="jack" |
| CRITICAL | GS001 | views.py | 870 | Found: password="b4f945433ea4c369c12741f62a23ccc0" |
| CRITICAL | GS001 | views.py | 872 | Found: password="f8d1ce191319ea8f4d1d26e65e130dd5" |
| CRITICAL | GS001 | views.py | 1095 | Found: 'HS256' |
| CRITICAL | GS001 | views.py | 1107 | Found: 'HS256' |
| CRITICAL | ? | entrypoint.sh | 11 | Match: echo "from django.contrib.auth.models import User; fr |
| CRITICAL | ? | challenge.html | 21 | Match:     const csrf_token = "{{ csrf_token|safe }}"; |
| CRITICAL | ? | sec_mis_lab3.html | 42 | Match: &emsp;&emsp;response.set_cookie(key = "auth_cookie",  |
| CRITICAL | ? | sql.html | 63 | Match:                 <br><code>SELECT * FROM introduction_ |
| CRITICAL | ? | injection.html | 72 | Match:                     <br><code>SELECT * FROM introduct |
| CRITICAL | ? | mitre_top3.html | 65 | Match:                         <br><code>SELECT * FROM intro |
| CRITICAL | ? | main.py | 36 | Match:         user = pickle.loads(decoded_data) |
| CRITICAL | ? | views.py | 214 | Match:             admin = pickle.loads(token) |
| CRITICAL | GS019 | app.py | 8 | Session/JWT secret hardcoded in source. Anyone with code acc |
| CRITICAL | GS019 | settings.py | 8 | Session/JWT secret hardcoded in source. Anyone with code acc |
| CRITICAL | GS019 | settings.py | 25 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | ? | views.py | 59 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 62 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 79 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | populate_challenge.py | 16 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 29 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 50 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 592 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 596 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 708 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 867 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 869 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 871 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 873 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 992 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 1142 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 1153 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 1156 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 1202 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 15 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 18 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | mitre.py | 205 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | mitre.py | 207 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | views.py | 963 |  |
| HIGH | ? | utility.py | 9 |  |
| HIGH | ? | soln.py | 9 |  |
| HIGH | ? | app.py | 123 | Match:     app.run(host='0.0.0.0', port=5000, debug=True)  # |
| HIGH | ? | Dockerfile | 19 | Match: CMD ["python", "manage.py", "runserver", "0.0.0.0:800 |
| HIGH | ? | docker-compose.yml | 13 | Match:              python manage.py runserver 0.0.0.0:8000" |
| HIGH | ? | Dockerfile | 11 | Match: ENV FLASK_RUN_HOST=0.0.0.0 |
| HIGH | ? | main.py | 51 | Match:     app.run(host='0.0.0.0', port=8080) |
| HIGH | ? | Dockerfile | 33 | Match: CMD ["gunicorn", "--bind", "0.0.0.0:8000", "--workers |
| HIGH | ? | docker-compose.yml | 4 | Match:     command: gunicorn --bind 0.0.0.0:8000 --workers 6 |
| HIGH | ? | views.py | 667 | Match:             if ip != '127.0.0.1': |
| HIGH | ? | views.py | 950 | Match:     if ip == '127.0.0.1': |
| HIGH | ? | apis.py | 79 | Match:         url = "http://127.0.0.1:8000/2021/discussion/ |
| HIGH | ? | ssrf.html | 28 | Match:           now there is a page at <a href="/ssrf_targe |
| HIGH | ? | a10_lab2.html | 65 | Match:     &emsp;&emsp;&emsp;if ip != '127.0.0.1':<br> |
| HIGH | ? | mitre_top21.html | 40 | Match:       now there is a page at <a href="/ssrf_target">/ |
| HIGH | ? | settings.py | 32 | Match: ALLOWED_HOSTS = ['pygoat.herokuapp.com', '0.0.0.0.'] |
| HIGH | ? | settings.py | 172 | Match: CSRF_TRUSTED_ORIGINS = ["http://127.0.0.1:8000","http |
| HIGH | ? | settings.py | 11 | Match: DEBUG = True |
| HIGH | ? | settings.py | 30 | Match: DEBUG = True |
| HIGH | ? | views.py | 460 | Match:                 output = eval(val) |
| HIGH | ? | views.py | 588 | Match:             output = ImageMath.eval(function_str,img  |
| HIGH | ? | mitre.py | 218 | Match:         result = eval(expression) |
| HIGH | ? | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS004 | mitre.py | 233 | Line 233: process = subprocess.Popen(command, shell=True, st |
| HIGH | GS004 | views.py | 430 | Line 430: process = subprocess.Popen( |
| HIGH | GS011 | settings.py | 8 | Found JWT secret in code: 'django-i...'. JWT secrets must be |
| HIGH | GS011 | views.py | 211 | Detected: key='token' |
| HIGH | GS011 | views.py | 1109 | Detected: key = "auth_cookie" |
| HIGH | GS011 | settings.py | 25 | Found JWT secret in code: 'lr66%-a!...'. JWT secrets must be |
| HIGH | GS019 | app.py | 36 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | app.py | 117 |
| M | ? | views.py | 24 |
| M | ? | views.py | 42 |
| M | ? | populate_challenge.py | 17 |
| M | ? | views.py | 163 |
| M | ? | views.py | 294 |
| M | ? | views.py | 296 |
| M | ? | views.py | 308 |
| M | ? | views.py | 322 |
| M | ? | views.py | 324 |
| M | ? | views.py | 442 |
| M | ? | views.py | 461 |
| M | ? | views.py | 563 |
| M | ? | views.py | 566 |
| M | ? | views.py | 713 |
| M | ? | views.py | 725 |
| M | ? | views.py | 882 |
| M | ? | views.py | 930 |
| M | ? | views.py | 965 |
| M | ? | views.py | 1045 |
| M | ? | views.py | 1083 |
| M | ? | views.py | 1100 |
| M | ? | views.py | 1144 |
| M | ? | views.py | 1186 |
| M | ? | views.py | 1195 |
| M | ? | views.py | 1225 |
| M | ? | apis.py | 100 |
| M | ? | apis.py | 136 |
| M | ? | sec_mis_lab3.html | 33 |
| M | ? | ssrf_lab2.html | 42 |
| M | ? | ssrf_lab.html | 60 |
| M | ? | ssrf_discussion.html | 49 |
| M | ? | ssrf_discussion.html | 116 |
| M | ? | lab3.html | 51 |
| M | ? | lab3.html | 60 |
| M | ? | lab2.html | 59 |
| M | ? | index.html | 29 |
| M | ? | index.html | 38 |
| M | ? | mitre.py | 188 |
| M | ? | main.py | 11 |
| C | ? | views.py | 158 |
| C | ? | views.py | 864 |
| H | ? | views.py | 59 |
| H | ? | views.py | 62 |
| H | ? | views.py | 79 |
| H | ? | populate_challenge.py | 16 |
| H | ? | models.py | 29 |
| H | ? | views.py | 50 |
| H | ? | views.py | 592 |
| H | ? | views.py | 596 |
| H | ? | views.py | 708 |
| H | ? | views.py | 867 |
| H | ? | views.py | 869 |
| H | ? | views.py | 871 |
| H | ? | views.py | 873 |
| H | ? | views.py | 992 |
| H | ? | views.py | 1142 |
| H | ? | views.py | 1153 |
| H | ? | views.py | 1156 |
| H | ? | views.py | 1202 |
| H | ? | forms.py | 15 |
| H | ? | forms.py | 18 |
| H | ? | mitre.py | 205 |
| H | ? | mitre.py | 207 |
| M | ? | views.py | 998 |
| M | ? | main.py | 36 |
| M | ? | views.py | 214 |
| M | ? | views.py | 560 |
| M | ? | test.py | 23 |
| H | ? | views.py | 963 |
| H | ? | utility.py | 9 |
| H | ? | soln.py | 9 |
| M | ? | settings.py | 8 |
| M | ? | views.py | 158 |
| M | ? | views.py | 864 |
| M | ? | views.py | 866 |
| M | ? | views.py | 868 |
| M | ? | views.py | 870 |
| M | ? | views.py | 872 |
| M | ? | settings.py | 25 |
| C | ? | mitre.py | 233 |
| M | ? | app.py | 8 |
| M | ? | views.py | 158 |
| M | ? | views.py | 211 |
| M | ? | views.py | 864 |
| M | ? | views.py | 866 |
| M | ? | views.py | 868 |
| M | ? | views.py | 870 |
| M | ? | views.py | 872 |
| M | ? | views.py | 1109 |
| C | GS001 | views.py | 56 |
| C | GS001 | views.py | 80 |
| C | GS001 | views.py | 96 |
| C | GS001 | entrypoint.sh | 11 |
| C | GS001 | entrypoint.sh | 11 |
| C | GS001 | mitre.py | 169 |
| C | GS001 | mitre.py | 182 |
| C | GS001 | mitre.py | 194 |
| C | GS001 | a9.js | 18 |
| C | GS001 | sql.html | 63 |
| C | GS001 | sec_mis_lab3.html | 30 |
| C | GS001 | sec_mis_lab3.html | 40 |
| C | GS001 | injection.html | 72 |
| C | GS001 | mitre_top3.html | 65 |
| C | GS001 | views.py | 866 |
| C | GS001 | views.py | 868 |
| C | GS001 | views.py | 870 |
| C | GS001 | views.py | 872 |
| C | GS001 | views.py | 1095 |
| C | GS001 | views.py | 1107 |
| L | GS003 | PyGoatBot.py | 40 |
| L | GS003 | PyGoatBot.py | 47 |
| L | GS003 | PyGoatBot.py | 50 |
| L | GS003 | PyGoatBot.py | 57 |
| L | GS003 | PyGoatBot.py | 61 |
| L | GS003 | utility.py | 8 |
| L | GS003 | views.py | 77 |
| L | GS003 | apis.py | 118 |
| L | GS003 | test.py | 30 |
| L | GS003 | views.py | 159 |
| L | GS003 | views.py | 161 |
| L | GS003 | views.py | 164 |
| L | GS003 | views.py | 292 |
| L | GS003 | views.py | 306 |
| L | GS003 | views.py | 314 |
| L | GS003 | views.py | 320 |
| L | GS003 | views.py | 422 |
| L | GS003 | views.py | 441 |
| L | GS003 | views.py | 445 |
| L | GS003 | views.py | 457 |
| L | GS003 | views.py | 464 |
| L | GS003 | views.py | 601 |
| L | GS003 | views.py | 604 |
| L | GS003 | views.py | 755 |
| L | GS003 | views.py | 756 |
| L | GS003 | views.py | 795 |
| L | GS003 | views.py | 860 |
| L | GS003 | views.py | 861 |
| L | GS003 | views.py | 874 |
| L | GS003 | views.py | 880 |
| L | GS003 | views.py | 1054 |
| L | GS003 | views.py | 1065 |
| L | GS003 | views.py | 1131 |
| L | GS003 | views.py | 1146 |
| L | GS003 | views.py | 1159 |
| L | GS003 | uninstaller.py | 35 |
| L | GS003 | uninstaller.py | 54 |
| L | GS003 | uninstaller.py | 60 |
| L | GS003 | uninstaller.py | 69 |
| L | GS003 | uninstaller.py | 76 |
| L | GS003 | uninstaller.py | 86 |
| L | GS003 | uninstaller.py | 89 |
| L | GS003 | uninstaller.py | 93 |
| L | GS003 | uninstaller.py | 103 |
| L | GS003 | uninstaller.py | 114 |
| L | GS003 | uninstaller.py | 127 |
| L | GS003 | uninstaller.py | 131 |
| L | GS003 | uninstaller.py | 132 |
| L | GS003 | ssrf.js | 74 |
| L | GS003 | ssrf.js | 83 |
| L | GS003 | a6.js | 21 |
| L | GS003 | a6.js | 40 |
| L | GS003 | a6.js | 52 |
| L | GS003 | a7.js | 21 |
| L | GS003 | a7.js | 26 |
| L | GS003 | a9.js | 36 |
| L | GS003 | a9.js | 44 |
| L | GS008 | settings.py | 13 |
| L | GS008 | settings.py | 16 |
| L | GS008 | settings.py | 27 |
| L | GS008 | settings.py | 39 |
| L | GS008 | settings.py | 55 |
| L | GS008 | settings.py | 58 |
| L | GS008 | settings.py | 82 |
| L | GS008 | settings.py | 83 |
| L | GS008 | settings.py | 84 |
| L | GS008 | settings.py | 85 |
| L | GS008 | settings.py | 86 |
| L | GS008 | settings.py | 93 |
| L | GS008 | settings.py | 96 |
| L | GS008 | settings.py | 100 |
| L | GS008 | mitre.py | 19 |
| L | GS008 | settings.py | 27 |
| L | GS008 | settings.py | 30 |
| L | GS008 | settings.py | 32 |
| L | GS008 | settings.py | 37 |
| L | GS008 | settings.py | 55 |
| L | GS008 | settings.py | 68 |
| L | GS008 | settings.py | 84 |
| L | GS008 | settings.py | 90 |
| L | GS008 | settings.py | 120 |
| L | GS008 | settings.py | 122 |
| L | GS008 | settings.py | 124 |
| L | GS008 | settings.py | 126 |
| L | GS008 | settings.py | 128 |
| L | GS008 | settings.py | 136 |
| L | GS008 | settings.py | 138 |
| L | GS008 | settings.py | 140 |
| L | GS008 | settings.py | 151 |
| L | GS008 | settings.py | 156 |
| L | GS008 | settings.py | 159 |
| L | GS008 | settings.py | 172 |
| I | GS015 | urls.py | 1 |
| I | GS015 | app.py | 27 |
| I | GS015 | app.py | 31 |
| I | GS015 | app.py | 35 |
| I | GS015 | app.py | 58 |
| I | GS015 | app.py | 78 |
| I | GS015 | app.py | 97 |
| I | GS015 | app.py | 103 |
| I | GS015 | app.py | 27 |
| I | GS015 | app.py | 31 |
| I | GS015 | app.py | 35 |
| I | GS015 | app.py | 58 |
| I | GS015 | app.py | 78 |
| I | GS015 | app.py | 97 |
| I | GS015 | app.py | 103 |
| I | GS015 | app.py | 27 |
| I | GS015 | app.py | 31 |
| I | GS015 | app.py | 35 |
| I | GS015 | app.py | 58 |
| I | GS015 | app.py | 78 |
| I | GS015 | app.py | 97 |
| I | GS015 | app.py | 103 |
| I | GS015 | app.py | 7 |
| I | GS015 | main.py | 17 |
| I | GS015 | main.py | 21 |
| I | GS015 | main.py | 30 |
| I | GS015 | main.py | 17 |
| I | GS015 | main.py | 21 |
| I | GS015 | main.py | 30 |
| I | GS015 | main.py | 17 |
| I | GS015 | main.py | 21 |
| I | GS015 | main.py | 30 |
| I | GS015 | main.py | 6 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 7 |
| I | GS015 | main.py | 1 |
| I | GS015 | main.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | asgi.py | 16 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 16 |
| i | GS020 |  | 20 |
| i | GS020 |  | 32 |
| i | GS020 |  | 35 |
| i | GS020 |  | 46 |
| i | GS020 |  | 40 |
| H | ? | app.py | 123 |
| H | ? | Dockerfile | 19 |
| H | ? | docker-compose.yml | 13 |
| H | ? | Dockerfile | 11 |
| H | ? | main.py | 51 |
| H | ? | Dockerfile | 33 |
| H | ? | docker-compose.yml | 4 |
| H | ? | views.py | 667 |
| H | ? | views.py | 950 |
| H | ? | apis.py | 79 |
| H | ? | ssrf.html | 28 |
| H | ? | a10_lab2.html | 65 |
| H | ? | mitre_top21.html | 40 |
| H | ? | settings.py | 32 |
| H | ? | settings.py | 172 |
| C | ? | entrypoint.sh | 11 |
| C | ? | challenge.html | 21 |
| C | ? | sec_mis_lab3.html | 42 |
| C | ? | sql.html | 63 |
| C | ? | injection.html | 72 |
| C | ? | mitre_top3.html | 65 |
| H | ? | settings.py | 11 |
| H | ? | settings.py | 30 |
| M | ? | uninstaller.py | 52 |
| H | ? | views.py | 460 |
| H | ? | views.py | 588 |
| H | ? | mitre.py | 218 |
| C | ? | main.py | 36 |
| C | ? | views.py | 214 |
| H | ? | docker-compose.yml | 0 |
| H | GS004 | mitre.py | 233 |
| H | GS004 | views.py | 430 |
| s | GS009 |  | 0 |
| H | GS011 | settings.py | 8 |
| L | GS011 | mitre.py | 182 |
| L | GS011 | mitre.py | 194 |
| L | GS011 | views.py | 1095 |
| H | GS011 | views.py | 211 |
| H | GS011 | views.py | 1109 |
| H | GS011 | settings.py | 25 |
| L | GS012 | populate_challenge.py | 16 |
| L | GS012 | views.py | 59 |
| L | GS012 | views.py | 62 |
| L | GS012 | views.py | 79 |
| L | GS012 | forms.py | 18 |
| L | GS012 | mitre.py | 205 |
| L | GS012 | mitre.py | 207 |
| L | GS012 | views.py | 50 |
| L | GS012 | views.py | 62 |
| L | GS012 | views.py | 708 |
| L | GS012 | views.py | 867 |
| L | GS012 | views.py | 869 |
| L | GS012 | views.py | 871 |
| L | GS012 | views.py | 873 |
| L | GS012 | views.py | 992 |
| L | GS012 | views.py | 1142 |
| L | GS012 | views.py | 1153 |
| L | GS012 | views.py | 1156 |
| L | GS012 | views.py | 1202 |
| H | GS019 | app.py | 36 |
| C | GS019 | app.py | 8 |
| M | GS019 | app.py | 79 |
| C | GS019 | settings.py | 8 |
| C | GS019 | settings.py | 25 |
| s | GS021 |  | 40 |
| s | GS021 |  | 64 |
| s | GS021 |  | 3 |
| c | GS021 |  | 239 |
| c | GS021 |  | 255 |
| c | GS021 |  | 335 |
| c | GS021 |  | 341 |
| c | GS021 |  | 414 |
| c | GS021 |  | 452 |
| c | GS021 |  | 492 |
| c | GS021 |  | 550 |
| c | GS021 |  | 573 |
| c | GS021 |  | 738 |
| c | GS021 |  | 746 |
| c | GS021 |  | 782 |
| c | GS021 |  | 846 |
| c | GS021 |  | 854 |
| c | GS021 |  | 1178 |
| s | GS021 |  | 537 |
| s | GS021 |  | 540 |
| s | GS021 |  | 667 |
| s | GS021 |  | 950 |
| c | GS021 |  | 22 |
| c | GS021 |  | 59 |
| c | GS021 |  | 93 |
| c | GS021 |  | 112 |
| c | GS021 |  | 125 |
| s | GS021 |  | 79 |
| c | GS021 |  | 177 |
| c | GS021 |  | 214 |
| c | GS021 |  | 237 |
| s | GS021 |  | 32 |
| s | GS021 |  | 172 |
| s | GS021 |  | 172 |
| c | GS021 |  | 35 |
| c | GS021 |  | 58 |
| c | GS021 |  | 78 |
| s | GS021 |  | 123 |
| c | GS021 |  | 21 |
| c | GS021 |  | 30 |
| s | GS021 |  | 51 |
| c | GS021 |  | 7 |
| c | GS021 |  | 7 |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-no_rate_limit_auth |  | ? |
| ? | GS025-wildcard_bind |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| M | ? | uninstaller.py | 41 |

---
*Сгенерировано GSC v0.6 · 2026-08-07T11:48:51.088969*