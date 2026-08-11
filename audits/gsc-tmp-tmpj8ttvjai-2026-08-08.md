---
title: "GSC Audit: /tmp/tmpj8ttvjai"
date: 2026-08-08
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/tmpj8ttvjai

**Дата:** 08.08.2026 11:52  
**Путь:** `/tmp/tmpj8ttvjai`  
**Всего находок:** 147  
**CRITICAL:** 3 | **HIGH:** 85 | **MEDIUM:** 0 | **LOW:** 0

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 82 |
| GS021 | 43 |
| GS022 | 15 |
| GS001 | 3 |
| GS025 | 3 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | http_httpsig.c | 60 | Found: "ed25519" |
| CRITICAL | GS001 | libssh2.c | 3361 | Found: "OS400QC3" |
| CRITICAL | GS001 | config2setopts.c | 590 | Found: "ed25519" |
| HIGH | GS000-LEGACY | proxy.c | 53 | Match: UNITTEST bool cidr4_match(const char *ipv4,    /* 1.2 |
| HIGH | GS000-LEGACY | proxy.c | 54 | Match:                           const char *network, /* 1.2 |
| HIGH | GS000-LEGACY | proxy.c | 56 | Match: UNITTEST bool cidr4_match(const char *ipv4,    /* 1.2 |
| HIGH | GS000-LEGACY | proxy.c | 57 | Match:                           const char *network, /* 1.2 |
| HIGH | GS000-LEGACY | ftp.c | 1271 | Match:        * EPRT |1|132.235.1.2|6275| |
| HIGH | GS000-LEGACY | ftp.c | 2799 | Match:       150 ASCII data connection for /bin/ls (137.167. |
| HIGH | GS000-LEGACY | ftp.c | 2802 | Match:       150 Opening ASCII mode data connection for [fil |
| HIGH | GS000-LEGACY | urlapi.c | 508 | Match:  * '16843009', '0x7f', '0x7f.1' '0177.1.1.1' etc. |
| HIGH | GS000-LEGACY | urlapi.c | 612 | Match:   case 3: /* a.b.c.d -- 8.8.8.8 bits */ |
| HIGH | GS000-LEGACY | urlapi.c | 921 | Match:      * "127.0.0.1" hostnames as local, otherwise as a |
| HIGH | GS000-LEGACY | urlapi.c | 929 | Match:          "127.0.0.1" to be valid */ |
| HIGH | GS000-LEGACY | urlapi.c | 931 | Match:          checkprefix("127.0.0.1/", ptr)) { |
| HIGH | GS000-LEGACY | urlapi.c | 935 | Match:         /* Invalid file://hostname/, expected localho |
| HIGH | GS000-LEGACY | cf-socket.c | 1167 | Match:            !strcmp(ctx->ip.remote_ip, "127.0.0.1")) | |
| HIGH | GS000-LEGACY | spnego_gssapi.c | 166 | Match:     /* OID 1.3.6.1.4.1.311.2.2.10 (NTLMSSP) */ |
| HIGH | GS000-LEGACY | spnego_gssapi.c | 248 | Match:     /* OID 1.3.6.1.4.1.311.2.2.10 (NTLMSSP) */ |
| HIGH | GS000-LEGACY | curl_addrinfo.c | 428 | Match:     /* This is a dotted IP address 123.123.123.123-st |
| HIGH | GS000-LEGACY | http.c | 3354 | Match:      * [RFC 2616, section 8.1.2.1] |
| HIGH | GS000-LEGACY | mime.c | 210 | Match:   /* WHATWG HTML living standard 4.10.21.8 2 specifie |
| HIGH | GS000-LEGACY | content_encoding.c | 141 | Match:     /* Only occurs for gzip with zlib < 1.2.0.4 or ra |
| HIGH | GS000-LEGACY | content_encoding.c | 750 | Match:  * See RFC 7231 section 3.1.2.2. */ |
| HIGH | GS000-LEGACY | inet_ntop.c | 58 | Match:   char tmp[sizeof("255.255.255.255")]; |
| HIGH | GS000-LEGACY | inet_ntop.c | 95 | Match:   char tmp[sizeof("ffff:ffff:ffff:ffff:ffff:ffff:255. |
| HIGH | GS000-LEGACY | hostip.c | 246 | Match: /* return a static IPv4 127.0.0.1 for the given name  |
| HIGH | GS000-LEGACY | hostip.c | 261 | Match:   if(curlx_inet_pton(AF_INET, "127.0.0.1", (char *)&i |
| HIGH | GS000-LEGACY | curl_gssapi.c | 325 | Match: /* NTLMSSP OID: 1.3.6.1.4.1.311.2.2.10 */ |
| HIGH | GS000-LEGACY | x509asn1.c | 66 | Match:   { "1.2.840.10045.3.0.1",      "c2pnb163v1" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 68 | Match:   { "1.2.840.10045.4.3.1",      "ecdsa-with-SHA224" } |
| HIGH | GS000-LEGACY | x509asn1.c | 69 | Match:   { "1.2.840.10045.4.3.2",      "ecdsa-with-SHA256" } |
| HIGH | GS000-LEGACY | x509asn1.c | 70 | Match:   { "1.2.840.10045.4.3.3",      "ecdsa-with-SHA384" } |
| HIGH | GS000-LEGACY | x509asn1.c | 71 | Match:   { "1.2.840.10045.4.3.4",      "ecdsa-with-SHA512" } |
| HIGH | GS000-LEGACY | x509asn1.c | 73 | Match:   { "1.2.840.113549.1.1.1",     "rsaEncryption" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 74 | Match:   { "1.2.840.113549.1.1.2",     "md2WithRSAEncryption |
| HIGH | GS000-LEGACY | x509asn1.c | 75 | Match:   { "1.2.840.113549.1.1.4",     "md5WithRSAEncryption |
| HIGH | GS000-LEGACY | x509asn1.c | 76 | Match:   { "1.2.840.113549.1.1.5",     "sha1WithRSAEncryptio |
| HIGH | GS000-LEGACY | x509asn1.c | 77 | Match:   { "1.2.840.113549.1.1.10",    "RSASSA-PSS" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 78 | Match:   { "1.2.840.113549.1.1.14",    "sha224WithRSAEncrypt |
| HIGH | GS000-LEGACY | x509asn1.c | 79 | Match:   { "1.2.840.113549.1.1.11",    "sha256WithRSAEncrypt |
| HIGH | GS000-LEGACY | x509asn1.c | 80 | Match:   { "1.2.840.113549.1.1.12",    "sha384WithRSAEncrypt |
| HIGH | GS000-LEGACY | x509asn1.c | 81 | Match:   { "1.2.840.113549.1.1.13",    "sha512WithRSAEncrypt |
| HIGH | GS000-LEGACY | x509asn1.c | 84 | Match:   { "1.3.14.3.2.26",            "sha1" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 85 | Match:   { "2.5.4.3",                  "CN" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 86 | Match:   { "2.5.4.4",                  "SN" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 87 | Match:   { "2.5.4.5",                  "serialNumber" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 88 | Match:   { "2.5.4.6",                  "C" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 89 | Match:   { "2.5.4.7",                  "L" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 90 | Match:   { "2.5.4.8",                  "ST" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 91 | Match:   { "2.5.4.9",                  "streetAddress" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 92 | Match:   { "2.5.4.10",                 "O" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 93 | Match:   { "2.5.4.11",                 "OU" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 94 | Match:   { "2.5.4.12",                 "title" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 95 | Match:   { "2.5.4.13",                 "description" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 96 | Match:   { "2.5.4.17",                 "postalCode" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 97 | Match:   { "2.5.4.41",                 "name" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 98 | Match:   { "2.5.4.42",                 "givenName" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 99 | Match:   { "2.5.4.43",                 "initials" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 100 | Match:   { "2.5.4.44",                 "generationQualifier" |
| HIGH | GS000-LEGACY | x509asn1.c | 101 | Match:   { "2.5.4.45",                 "X500UniqueIdentifier |
| HIGH | GS000-LEGACY | x509asn1.c | 102 | Match:   { "2.5.4.46",                 "dnQualifier" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 103 | Match:   { "2.5.4.65",                 "pseudonym" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 104 | Match:   { "1.2.840.113549.1.9.1",     "emailAddress" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 105 | Match:   { "2.5.4.72",                 "role" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 106 | Match:   { "2.5.29.17",                "subjectAltName" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 107 | Match:   { "2.5.29.18",                "issuerAltName" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 108 | Match:   { "2.5.29.19",                "basicConstraints" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 109 | Match:   { "2.16.840.1.101.3.4.2.4",   "sha224" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 110 | Match:   { "2.16.840.1.101.3.4.2.1",   "sha256" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 111 | Match:   { "2.16.840.1.101.3.4.2.2",   "sha384" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 112 | Match:   { "2.16.840.1.101.3.4.2.3",   "sha512" }, |
| HIGH | GS000-LEGACY | x509asn1.c | 113 | Match:   { "1.2.840.113549.1.9.2",     "unstructuredName" }, |
| HIGH | GS000-LEGACY | openssl.c | 2909 | Match:               if(!strcmp("1.3.6.1.5.5.7.3.1" /* OID s |
| HIGH | GS000-LEGACY | cookie.c | 89 | Match:    * RFC6265 4.1.2.3. The Domain Attribute says: |
| HIGH | GS000-LEGACY | cookie.c | 1296 | Match:     !strcmp(host, "127.0.0.1") || |
| HIGH | GS000-LEGACY | curl_sha512_256.c | 451 | Match:   /* Initial hash values, see FIPS PUB 180-4 section  |
| HIGH | GS000-LEGACY | acinclude.m4 | 306 | Match:         LDAP *ldp = ldap_init("0.0.0.0", LDAP_PORT); |
| HIGH | GS000-LEGACY | acinclude.m4 | 356 | Match:         LDAP *ldp = ldapssl_init("0.0.0.0", LDAPS_POR |
| HIGH | GS000-LEGACY | acinclude.m4 | 434 | Match:           LDAP *ldp = ldap_init("0.0.0.0", LDAP_PORT) |
| HIGH | GS000-LEGACY | acinclude.m4 | 544 | Match:           LDAP *ldp = ldap_init("0.0.0.0", LDAP_PORT) |
| HIGH | GS000-LEGACY | curl-functions.m4 | 1253 | Match:         error = getaddrinfo("127.0.0.1", 0, &hints, & |
| HIGH | GS000-LEGACY | tool_cfgable.h | 74 | Match:   char *dns_servers;   /* dot notation: 1.1.1.1;2.2.2 |
| HIGH | GS000-LEGACY | tool_getparam.c | 2872 | Match:     /* use <eth0> or <192.168.10.10> style addresses. |
| HIGH | GS000-LEGACY | build_curl-config_script.com | 46 | Match: $ x_curlversion = "0.0.0.0" |
| HIGH | GS025 | appveyor.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | renovate.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .clang-tidy.yml | 0 | Permissions 664 — should be 600 |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS001 | http_httpsig.c | 60 |
| C | GS001 | libssh2.c | 3361 |
| C | GS001 | config2setopts.c | 590 |
| H | GS000-LEGACY | proxy.c | 53 |
| H | GS000-LEGACY | proxy.c | 54 |
| H | GS000-LEGACY | proxy.c | 56 |
| H | GS000-LEGACY | proxy.c | 57 |
| H | GS000-LEGACY | ftp.c | 1271 |
| H | GS000-LEGACY | ftp.c | 2799 |
| H | GS000-LEGACY | ftp.c | 2802 |
| H | GS000-LEGACY | urlapi.c | 508 |
| H | GS000-LEGACY | urlapi.c | 612 |
| H | GS000-LEGACY | urlapi.c | 921 |
| H | GS000-LEGACY | urlapi.c | 929 |
| H | GS000-LEGACY | urlapi.c | 931 |
| H | GS000-LEGACY | urlapi.c | 935 |
| H | GS000-LEGACY | cf-socket.c | 1167 |
| H | GS000-LEGACY | spnego_gssapi.c | 166 |
| H | GS000-LEGACY | spnego_gssapi.c | 248 |
| H | GS000-LEGACY | curl_addrinfo.c | 428 |
| H | GS000-LEGACY | http.c | 3354 |
| H | GS000-LEGACY | mime.c | 210 |
| H | GS000-LEGACY | content_encoding.c | 141 |
| H | GS000-LEGACY | content_encoding.c | 750 |
| H | GS000-LEGACY | inet_ntop.c | 58 |
| H | GS000-LEGACY | inet_ntop.c | 95 |
| H | GS000-LEGACY | hostip.c | 246 |
| H | GS000-LEGACY | hostip.c | 261 |
| H | GS000-LEGACY | curl_gssapi.c | 325 |
| H | GS000-LEGACY | x509asn1.c | 66 |
| H | GS000-LEGACY | x509asn1.c | 68 |
| H | GS000-LEGACY | x509asn1.c | 69 |
| H | GS000-LEGACY | x509asn1.c | 70 |
| H | GS000-LEGACY | x509asn1.c | 71 |
| H | GS000-LEGACY | x509asn1.c | 73 |
| H | GS000-LEGACY | x509asn1.c | 74 |
| H | GS000-LEGACY | x509asn1.c | 75 |
| H | GS000-LEGACY | x509asn1.c | 76 |
| H | GS000-LEGACY | x509asn1.c | 77 |
| H | GS000-LEGACY | x509asn1.c | 78 |
| H | GS000-LEGACY | x509asn1.c | 79 |
| H | GS000-LEGACY | x509asn1.c | 80 |
| H | GS000-LEGACY | x509asn1.c | 81 |
| H | GS000-LEGACY | x509asn1.c | 84 |
| H | GS000-LEGACY | x509asn1.c | 85 |
| H | GS000-LEGACY | x509asn1.c | 86 |
| H | GS000-LEGACY | x509asn1.c | 87 |
| H | GS000-LEGACY | x509asn1.c | 88 |
| H | GS000-LEGACY | x509asn1.c | 89 |
| H | GS000-LEGACY | x509asn1.c | 90 |
| H | GS000-LEGACY | x509asn1.c | 91 |
| H | GS000-LEGACY | x509asn1.c | 92 |
| H | GS000-LEGACY | x509asn1.c | 93 |
| H | GS000-LEGACY | x509asn1.c | 94 |
| H | GS000-LEGACY | x509asn1.c | 95 |
| H | GS000-LEGACY | x509asn1.c | 96 |
| H | GS000-LEGACY | x509asn1.c | 97 |
| H | GS000-LEGACY | x509asn1.c | 98 |
| H | GS000-LEGACY | x509asn1.c | 99 |
| H | GS000-LEGACY | x509asn1.c | 100 |
| H | GS000-LEGACY | x509asn1.c | 101 |
| H | GS000-LEGACY | x509asn1.c | 102 |
| H | GS000-LEGACY | x509asn1.c | 103 |
| H | GS000-LEGACY | x509asn1.c | 104 |
| H | GS000-LEGACY | x509asn1.c | 105 |
| H | GS000-LEGACY | x509asn1.c | 106 |
| H | GS000-LEGACY | x509asn1.c | 107 |
| H | GS000-LEGACY | x509asn1.c | 108 |
| H | GS000-LEGACY | x509asn1.c | 109 |
| H | GS000-LEGACY | x509asn1.c | 110 |
| H | GS000-LEGACY | x509asn1.c | 111 |
| H | GS000-LEGACY | x509asn1.c | 112 |
| H | GS000-LEGACY | x509asn1.c | 113 |
| H | GS000-LEGACY | openssl.c | 2909 |
| H | GS000-LEGACY | cookie.c | 89 |
| H | GS000-LEGACY | cookie.c | 1296 |
| H | GS000-LEGACY | curl_sha512_256.c | 451 |
| H | GS000-LEGACY | acinclude.m4 | 306 |
| H | GS000-LEGACY | acinclude.m4 | 356 |
| H | GS000-LEGACY | acinclude.m4 | 434 |
| H | GS000-LEGACY | acinclude.m4 | 544 |
| H | GS000-LEGACY | curl-functions.m4 | 1253 |
| H | GS000-LEGACY | tool_cfgable.h | 74 |
| H | GS000-LEGACY | tool_getparam.c | 2872 |
| H | GS000-LEGACY | build_curl-config_script.com | 46 |
| H | GS025 | appveyor.yml | 0 |
| H | GS025 | renovate.json | 0 |
| H | GS025 | .clang-tidy.yml | 0 |
| s | GS009 |  | 0 |
| s | GS021 |  | 42 |
| s | GS021 |  | 35 |
| s | GS021 |  | 375 |
| s | GS021 |  | 804 |
| s | GS021 |  | 194 |
| s | GS021 |  | 270 |
| s | GS021 |  | 77 |
| s | GS021 |  | 78 |
| s | GS021 |  | 207 |
| s | GS021 |  | 142 |
| s | GS021 |  | 155 |
| s | GS021 |  | 324 |
| s | GS021 |  | 337 |
| s | GS021 |  | 354 |
| s | GS021 |  | 389 |
| s | GS021 |  | 503 |
| s | GS021 |  | 226 |
| s | GS021 |  | 239 |
| s | GS021 |  | 190 |
| s | GS021 |  | 190 |
| s | GS021 |  | 200 |
| s | GS021 |  | 206 |
| s | GS021 |  | 40 |
| s | GS021 |  | 43 |
| s | GS021 |  | 258 |
| s | GS021 |  | 313 |
| s | GS021 |  | 170 |
| s | GS021 |  | 189 |
| s | GS021 |  | 332 |
| s | GS021 |  | 345 |
| s | GS021 |  | 138 |
| s | GS021 |  | 161 |
| s | GS021 |  | 162 |
| s | GS021 |  | 166 |
| s | GS021 |  | 170 |
| s | GS021 |  | 170 |
| s | GS021 |  | 142 |
| s | GS021 |  | 655 |
| s | GS021 |  | 1169 |
| s | GS021 |  | 693 |
| s | GS021 |  | 704 |
| s | GS021 |  | 220 |
| s | GS021 |  | 427 |
| r | GS022 |  | 109 |
| r | GS022 |  | 704 |
| r | GS022 |  | 712 |
| r | GS022 |  | 471 |
| r | GS022 |  | 475 |
| r | GS022 |  | 479 |
| r | GS022 |  | 483 |
| r | GS022 |  | 503 |
| r | GS022 |  | 611 |
| r | GS022 |  | 620 |
| r | GS022 |  | 627 |
| r | GS022 |  | 635 |
| r | GS022 |  | 866 |
| r | GS022 |  | 39 |
| r | GS022 |  | 1149 |

---
*Сгенерировано GSC v0.6 · 2026-08-08T11:52:31.632519*