---
title: "GSC Audit: /tmp/gsc-bac-scan/django-helpdesk"
date: 2026-07-28
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-bac-scan/django-helpdesk

**Дата:** 28.07.2026 19:18  
**Путь:** `/tmp/gsc-bac-scan/django-helpdesk`  
**Всего находок:** 209  
**CRITICAL:** 4 | **HIGH:** 86 | **MEDIUM:** 3 | **LOW:** 110

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| Python: File upload without content-type validation | 61 |
| GS008 | 58 |
| GS012 | 38 |
| GS003 | 14 |
| Хардкод IP адреса | 13 |
| GS015 | 5 |
| CVE-2026-56264: Server-side request forgery (SSRF) | 2 |
| CVE-2026-56318: Information disclosure | 2 |
| Debug mode enabled | 2 |
| GS007 | 2 |
| GS011 | 2 |
| Python: assert in production | 1 |
| GS001 | 1 |
| chmod: World-readable configs | 1 |
| Hardcoded encryption key | 1 |
| World-readable file: package.json (664) | 1 |
| World-readable file: .pre-commit-config.yaml (664) | 1 |
| World-readable file: .readthedocs.yaml (664) | 1 |
| World-readable file: .yarnrc.yml (664) | 1 |
| GS005 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | setup.sh | 20 | Found: PASSWORD="$key1 >> docker.env
  else
    echo " |
| CRITICAL | ? | Dockerfile | 51 | Match: RUN chmod 0644 /etc/crontab |
| CRITICAL | ? | jquery.translate-debug-all.js | 670 | Match:                             "www.google.com/jsapi" +  |
| CRITICAL | GS005 | models.py | 1189 | Line 1189: out += gettext('changed from "%(old_value)s" to " |
| HIGH | ? | create_queue_permissions.py | 63 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | escalate_tickets.py | 85 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 203 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 205 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 243 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 500 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 511 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 602 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | forms.py | 609 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | api.py | 93 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | public.py | 121 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | kb.py | 91 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 416 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 421 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 507 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 509 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 571 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 572 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 790 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 801 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 810 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 819 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 829 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 966 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 968 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 975 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1323 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1352 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1460 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1800 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1855 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1916 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1918 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1963 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 1966 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 2008 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 2011 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 2192 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | staff.py | 2317 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 462 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 875 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 927 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 952 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 1051 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 1056 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 1252 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 1586 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | models.py | 1859 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | update_ticket.py | 107 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | update_ticket.py | 120 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | update_ticket.py | 331 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | update_ticket.py | 351 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | update_ticket.py | 379 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | lib.py | 178 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | serializers.py | 151 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | serializers.py | 256 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | email.py | 35 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | email.py | 108 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | email.py | 625 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | email.py | 637 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | email.py | 656 | File upload without MIME-type validation → malicious file up |
| HIGH | ? | webhooks.py | 34 |  |
| HIGH | ? | webhooks.py | 60 |  |
| HIGH | ? | settings.py | 34 | Match:     "DJANGO_HELPDESK_ALLOWED_HOSTS", "*, localhost, 0 |
| HIGH | ? | django.po | 493 | Match: msgid "Socks proxy IP address. Default: 127.0.0.1" |
| HIGH | ? | django.po | 494 | Match: msgstr "Adresse du Proxy Socks. Par défaut : 127.0.0. |
| HIGH | ? | django.po | 467 | Match: msgid "Socks proxy IP address. Default: 127.0.0.1" |
| HIGH | ? | django.po | 468 | Match: msgstr "Socks Proxy IP-Adresse. Standard: 127.0.0.1" |
| HIGH | ? | django.po | 416 | Match: msgid "Socks proxy IP address. Default: 127.0.0.1" |
| HIGH | ? | django.po | 448 | Match: msgid "Socks proxy IP address. Default: 127.0.0.1" |
| HIGH | ? | django.po | 428 | Match: msgid "Socks proxy IP address. Default: 127.0.0.1" |
| HIGH | ? | django.po | 486 | Match: msgid "Socks proxy IP address. Default: 127.0.0.1" |
| HIGH | ? | django.po | 487 | Match: msgstr "IP-адрес Socks-прокси. По-умолчанию: 127.0.0. |
| HIGH | ? | models.py | 321 | Match:         help_text=_("Socks proxy IP address. Default: |
| HIGH | ? | models.py | 434 | Match:                 self.socks_proxy_host = "127.0.0.1" |
| HIGH | ? | lib.py | 140 | Match:             "user_ip": request.META.get("REMOTE_ADDR" |
| HIGH | ? | quicktest.py | 91 | Match:             DEBUG=True, |
| HIGH | ? | settings.py | 19 | Match: DEBUG = True |
| HIGH | ? | package.json | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .readthedocs.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | ? | .yarnrc.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS007 | staff.py | 1436 | Line 1436: preset = PreSetReply.objects.get(id=request.GET.g |
| HIGH | GS007 | staff.py | 1215 | Line 1215: user_saved_queries = SavedSearch.objects.filter( |
| HIGH | GS011 | settings.py | 16 | Found JWT secret in code: '_crkn1+f...'. JWT secrets must be |
| HIGH | GS011 | quicktest.py | 110 | Found JWT secret in code: 'wowdonot...'. JWT secrets must be |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | models.py | 1264 |
| H | ? | create_queue_permissions.py | 63 |
| H | ? | escalate_tickets.py | 85 |
| H | ? | forms.py | 203 |
| H | ? | forms.py | 205 |
| H | ? | forms.py | 243 |
| H | ? | forms.py | 500 |
| H | ? | forms.py | 511 |
| H | ? | forms.py | 602 |
| H | ? | forms.py | 609 |
| H | ? | api.py | 93 |
| H | ? | public.py | 121 |
| H | ? | kb.py | 91 |
| H | ? | staff.py | 416 |
| H | ? | staff.py | 421 |
| H | ? | staff.py | 507 |
| H | ? | staff.py | 509 |
| H | ? | staff.py | 571 |
| H | ? | staff.py | 572 |
| H | ? | staff.py | 790 |
| H | ? | staff.py | 801 |
| H | ? | staff.py | 810 |
| H | ? | staff.py | 819 |
| H | ? | staff.py | 829 |
| H | ? | staff.py | 966 |
| H | ? | staff.py | 968 |
| H | ? | staff.py | 975 |
| H | ? | staff.py | 1323 |
| H | ? | staff.py | 1352 |
| H | ? | staff.py | 1460 |
| H | ? | staff.py | 1800 |
| H | ? | staff.py | 1855 |
| H | ? | staff.py | 1916 |
| H | ? | staff.py | 1918 |
| H | ? | staff.py | 1963 |
| H | ? | staff.py | 1966 |
| H | ? | staff.py | 2008 |
| H | ? | staff.py | 2011 |
| H | ? | staff.py | 2192 |
| H | ? | staff.py | 2317 |
| H | ? | models.py | 462 |
| H | ? | models.py | 875 |
| H | ? | models.py | 927 |
| H | ? | models.py | 952 |
| H | ? | models.py | 1051 |
| H | ? | models.py | 1056 |
| H | ? | models.py | 1252 |
| H | ? | models.py | 1586 |
| H | ? | models.py | 1859 |
| H | ? | update_ticket.py | 107 |
| H | ? | update_ticket.py | 120 |
| H | ? | update_ticket.py | 331 |
| H | ? | update_ticket.py | 351 |
| H | ? | update_ticket.py | 379 |
| H | ? | lib.py | 178 |
| H | ? | serializers.py | 151 |
| H | ? | serializers.py | 256 |
| H | ? | email.py | 35 |
| H | ? | email.py | 108 |
| H | ? | email.py | 625 |
| H | ? | email.py | 637 |
| H | ? | email.py | 656 |
| H | ? | webhooks.py | 34 |
| H | ? | webhooks.py | 60 |
| M | ? | quicktest.py | 110 |
| M | ? | settings.py | 16 |
| C | GS001 | setup.sh | 20 |
| L | GS003 | quicktest.py | 17 |
| L | GS003 | email.py | 65 |
| L | GS003 | email.py | 72 |
| L | GS003 | email.py | 112 |
| L | GS003 | email.py | 116 |
| L | GS003 | email.py | 117 |
| L | GS003 | email.py | 132 |
| L | GS003 | settings.py | 476 |
| L | GS003 | load_helpdesk_settings.py | 17 |
| L | GS003 | load_helpdesk_settings.py | 22 |
| L | GS003 | saved_queries.py | 27 |
| L | GS003 | saved_queries.py | 32 |
| L | GS003 | get_deps.js | 9 |
| L | GS003 | jquery.translate-debug-all.js | 652 |
| L | GS008 | settings.py | 19 |
| L | GS008 | settings.py | 21 |
| L | GS008 | settings.py | 64 |
| L | GS008 | settings.py | 76 |
| L | GS008 | settings.py | 93 |
| L | GS008 | settings.py | 102 |
| L | GS008 | settings.py | 113 |
| L | GS008 | settings.py | 114 |
| L | GS008 | settings.py | 115 |
| L | GS008 | settings.py | 118 |
| L | GS008 | settings.py | 121 |
| L | GS008 | settings.py | 122 |
| L | GS008 | settings.py | 123 |
| L | GS008 | settings.py | 125 |
| L | GS008 | settings.py | 140 |
| L | GS008 | settings.py | 154 |
| L | GS008 | settings.py | 160 |
| L | GS008 | settings.py | 193 |
| L | GS008 | settings.py | 194 |
| L | GS008 | settings.py | 209 |
| L | GS008 | settings.py | 211 |
| L | GS008 | settings.py | 213 |
| L | GS008 | settings.py | 216 |
| L | GS008 | settings.py | 224 |
| L | GS008 | settings.py | 240 |
| L | GS008 | settings.py | 30 |
| L | GS008 | settings.py | 161 |
| L | GS008 | settings.py | 167 |
| L | GS008 | settings.py | 199 |
| L | GS008 | settings.py | 211 |
| L | GS008 | settings.py | 221 |
| L | GS008 | settings.py | 224 |
| L | GS008 | settings.py | 229 |
| L | GS008 | settings.py | 234 |
| L | GS008 | settings.py | 239 |
| L | GS008 | settings.py | 261 |
| L | GS008 | settings.py | 272 |
| L | GS008 | settings.py | 273 |
| L | GS008 | settings.py | 528 |
| L | GS008 | settings.py | 531 |
| L | GS008 | settings.py | 33 |
| L | GS008 | settings.py | 37 |
| L | GS008 | settings.py | 38 |
| L | GS008 | settings.py | 39 |
| L | GS008 | settings.py | 71 |
| L | GS008 | settings.py | 84 |
| L | GS008 | settings.py | 101 |
| L | GS008 | settings.py | 110 |
| L | GS008 | settings.py | 148 |
| L | GS008 | settings.py | 167 |
| L | GS008 | settings.py | 173 |
| L | GS008 | settings.py | 221 |
| L | GS008 | settings.py | 223 |
| L | GS008 | settings.py | 225 |
| L | GS008 | settings.py | 228 |
| L | GS008 | settings.py | 238 |
| L | GS008 | settings.py | 251 |
| L | GS008 | settings.py | 253 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 16 |
| I | GS015 | urls.py | 1 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 16 |
| H | ? | settings.py | 34 |
| H | ? | django.po | 493 |
| H | ? | django.po | 494 |
| H | ? | django.po | 467 |
| H | ? | django.po | 468 |
| H | ? | django.po | 416 |
| H | ? | django.po | 448 |
| H | ? | django.po | 428 |
| H | ? | django.po | 486 |
| H | ? | django.po | 487 |
| H | ? | models.py | 321 |
| H | ? | models.py | 434 |
| H | ? | lib.py | 140 |
| C | ? | Dockerfile | 51 |
| C | ? | jquery.translate-debug-all.js | 670 |
| H | ? | quicktest.py | 91 |
| H | ? | settings.py | 19 |
| H | ? | package.json | 0 |
| H | ? | .pre-commit-config.yaml | 0 |
| H | ? | .readthedocs.yaml | 0 |
| H | ? | .yarnrc.yml | 0 |
| C | GS005 | models.py | 1189 |
| H | GS007 | staff.py | 1436 |
| H | GS007 | staff.py | 1215 |
| s | GS009 |  | 0 |
| H | GS011 | settings.py | 16 |
| H | GS011 | quicktest.py | 110 |
| L | GS012 | email.py | 108 |
| L | GS012 | email.py | 625 |
| L | GS012 | email.py | 637 |
| L | GS012 | email.py | 656 |
| L | GS012 | forms.py | 203 |
| L | GS012 | forms.py | 500 |
| L | GS012 | forms.py | 511 |
| L | GS012 | forms.py | 602 |
| L | GS012 | forms.py | 609 |
| L | GS012 | lib.py | 178 |
| L | GS012 | create_queue_permissions.py | 63 |
| L | GS012 | escalate_tickets.py | 85 |
| L | GS012 | models.py | 952 |
| L | GS012 | models.py | 1051 |
| L | GS012 | serializers.py | 151 |
| L | GS012 | update_ticket.py | 107 |
| L | GS012 | update_ticket.py | 120 |
| L | GS012 | update_ticket.py | 379 |
| L | GS012 | kb.py | 91 |
| L | GS012 | staff.py | 416 |
| L | GS012 | staff.py | 421 |
| L | GS012 | staff.py | 509 |
| L | GS012 | staff.py | 571 |
| L | GS012 | staff.py | 572 |
| L | GS012 | staff.py | 790 |
| L | GS012 | staff.py | 801 |
| L | GS012 | staff.py | 810 |
| L | GS012 | staff.py | 819 |
| L | GS012 | staff.py | 829 |
| L | GS012 | staff.py | 975 |
| L | GS012 | staff.py | 1323 |
| L | GS012 | staff.py | 1460 |
| L | GS012 | staff.py | 1800 |
| L | GS012 | staff.py | 1855 |
| L | GS012 | staff.py | 1918 |
| L | GS012 | staff.py | 1966 |
| L | GS012 | staff.py | 2011 |
| L | GS012 | staff.py | 2192 |

---
*Сгенерировано GSC v0.6 · 2026-07-28T19:18:55.431546*