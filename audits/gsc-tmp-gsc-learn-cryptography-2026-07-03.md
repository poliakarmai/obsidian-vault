---
title: "GSC Audit: /tmp/gsc-learn/cryptography"
date: 2026-07-03
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-learn/cryptography

**Дата:** 03.07.2026 04:03  
**Путь:** `/tmp/gsc-learn/cryptography`  
**Всего находок:** 2254  
**CRITICAL:** 3 | **HIGH:** 1792 | **MEDIUM:** 332 | **LOW:** 126

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS002 | 1146 |
| Хардкод IP адреса | 438 |
| GS014 | 305 |
| Rust: .clone() in hot path | 205 |
| GS008 | 94 |
| GS003 | 32 |
| Python: assert in production | 19 |
| Outdated dependency pattern | 8 |
| GS001 | 2 |
| Hardcoded encryption key | 1 |
| eval() or exec() usage | 1 |
| World-readable file: .readthedocs.yml (664) | 1 |
| GS004 | 1 |
| GS009 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | _oid.py | 367 | Found: PASSWORD: "challengePassword" |
| CRITICAL | GS001 | gen.sh | 33 | Found: password="password" |
| CRITICAL | ? | gen.sh | 33 | Match:     *-psw.*) password="password" ;; |
| HIGH | ? | extension_policy.rs | 252 | Match:                 extn_id: asn1::ObjectIdentifier::from |
| HIGH | ? | lib.rs | 622 | Match:             "invalid extension: 2.5.29.17: duplicate  |
| HIGH | ? | mod.rs | 748 | Match:         let ip_sub = Subject::IP(IPAddress::from_str( |
| HIGH | ? | types.rs | 685 | Match:         assert_ne!(IPAddress::from_str("192.168.1.1") |
| HIGH | ? | types.rs | 697 | Match:             IPAddress::from_str("192.0.2.1").unwrap() |
| HIGH | ? | types.rs | 708 | Match:         let ipv4 = IPAddress::from_str("255.255.255.0 |
| HIGH | ? | types.rs | 710 | Match:         let ipv4_nonmask = IPAddress::from_str("192.0 |
| HIGH | ? | types.rs | 721 | Match:         let ipv4 = IPAddress::from_str("192.0.2.252") |
| HIGH | ? | types.rs | 724 | Match:         assert_eq!(ipv4.mask(0), IPAddress::from_str( |
| HIGH | ? | types.rs | 727 | Match:         assert_eq!(ipv4.mask(24), IPAddress::from_str |
| HIGH | ? | types.rs | 794 | Match:         assert!(ipv4.matches(&IPAddress::from_str("19 |
| HIGH | ? | types.rs | 795 | Match:         assert!(!ipv4.matches(&IPAddress::from_str("1 |
| HIGH | ? | types.rs | 796 | Match:         assert!(ipv4_32.matches(&IPAddress::from_str( |
| HIGH | ? | types.rs | 797 | Match:         assert!(!ipv4_32.matches(&IPAddress::from_str |
| HIGH | ? | types.rs | 798 | Match:         assert!(!ipv4_32.matches(&IPAddress::from_str |
| HIGH | ? | types.rs | 849 | Match:             ("1.2.3.4.5@example.com", ("1.2.3.4.5", " |
| HIGH | ? | ec.py | 19 | Match:     SECP192R1 = ObjectIdentifier("1.2.840.10045.3.1.1 |
| HIGH | ? | ec.py | 20 | Match:     SECP224R1 = ObjectIdentifier("1.3.132.0.33") |
| HIGH | ? | ec.py | 21 | Match:     SECP256K1 = ObjectIdentifier("1.3.132.0.10") |
| HIGH | ? | ec.py | 22 | Match:     SECP256R1 = ObjectIdentifier("1.2.840.10045.3.1.7 |
| HIGH | ? | ec.py | 23 | Match:     SECP384R1 = ObjectIdentifier("1.3.132.0.34") |
| HIGH | ? | ec.py | 24 | Match:     SECP521R1 = ObjectIdentifier("1.3.132.0.35") |
| HIGH | ? | ec.py | 25 | Match:     BRAINPOOLP256R1 = ObjectIdentifier("1.3.36.3.3.2. |
| HIGH | ? | ec.py | 26 | Match:     BRAINPOOLP384R1 = ObjectIdentifier("1.3.36.3.3.2. |
| HIGH | ? | ec.py | 27 | Match:     BRAINPOOLP512R1 = ObjectIdentifier("1.3.36.3.3.2. |
| HIGH | ? | _oid.py | 14 | Match:     SUBJECT_DIRECTORY_ATTRIBUTES = ObjectIdentifier(" |
| HIGH | ? | _oid.py | 15 | Match:     SUBJECT_KEY_IDENTIFIER = ObjectIdentifier("2.5.29 |
| HIGH | ? | _oid.py | 16 | Match:     KEY_USAGE = ObjectIdentifier("2.5.29.15") |
| HIGH | ? | _oid.py | 17 | Match:     PRIVATE_KEY_USAGE_PERIOD = ObjectIdentifier("2.5. |
| HIGH | ? | _oid.py | 18 | Match:     SUBJECT_ALTERNATIVE_NAME = ObjectIdentifier("2.5. |
| HIGH | ? | _oid.py | 19 | Match:     ISSUER_ALTERNATIVE_NAME = ObjectIdentifier("2.5.2 |
| HIGH | ? | _oid.py | 20 | Match:     BASIC_CONSTRAINTS = ObjectIdentifier("2.5.29.19") |
| HIGH | ? | _oid.py | 21 | Match:     NAME_CONSTRAINTS = ObjectIdentifier("2.5.29.30") |
| HIGH | ? | _oid.py | 22 | Match:     CRL_DISTRIBUTION_POINTS = ObjectIdentifier("2.5.2 |
| HIGH | ? | _oid.py | 23 | Match:     CERTIFICATE_POLICIES = ObjectIdentifier("2.5.29.3 |
| HIGH | ? | _oid.py | 24 | Match:     POLICY_MAPPINGS = ObjectIdentifier("2.5.29.33") |
| HIGH | ? | _oid.py | 25 | Match:     AUTHORITY_KEY_IDENTIFIER = ObjectIdentifier("2.5. |
| HIGH | ? | _oid.py | 26 | Match:     POLICY_CONSTRAINTS = ObjectIdentifier("2.5.29.36" |
| HIGH | ? | _oid.py | 27 | Match:     EXTENDED_KEY_USAGE = ObjectIdentifier("2.5.29.37" |
| HIGH | ? | _oid.py | 28 | Match:     FRESHEST_CRL = ObjectIdentifier("2.5.29.46") |
| HIGH | ? | _oid.py | 29 | Match:     INHIBIT_ANY_POLICY = ObjectIdentifier("2.5.29.54" |
| HIGH | ? | _oid.py | 30 | Match:     ISSUING_DISTRIBUTION_POINT = ObjectIdentifier("2. |
| HIGH | ? | _oid.py | 31 | Match:     AUTHORITY_INFORMATION_ACCESS = ObjectIdentifier(" |
| HIGH | ? | _oid.py | 32 | Match:     SUBJECT_INFORMATION_ACCESS = ObjectIdentifier("1. |
| HIGH | ? | _oid.py | 33 | Match:     OCSP_NO_CHECK = ObjectIdentifier("1.3.6.1.5.5.7.4 |
| HIGH | ? | _oid.py | 34 | Match:     TLS_FEATURE = ObjectIdentifier("1.3.6.1.5.5.7.1.2 |
| HIGH | ? | _oid.py | 35 | Match:     CRL_NUMBER = ObjectIdentifier("2.5.29.20") |
| HIGH | ? | _oid.py | 36 | Match:     DELTA_CRL_INDICATOR = ObjectIdentifier("2.5.29.27 |
| HIGH | ? | _oid.py | 38 | Match:         "1.3.6.1.4.1.11129.2.4.2" |
| HIGH | ? | _oid.py | 40 | Match:     PRECERT_POISON = ObjectIdentifier("1.3.6.1.4.1.11 |
| HIGH | ? | _oid.py | 41 | Match:     SIGNED_CERTIFICATE_TIMESTAMPS = ObjectIdentifier( |
| HIGH | ? | _oid.py | 42 | Match:     MS_CERTIFICATE_TEMPLATE = ObjectIdentifier("1.3.6 |
| HIGH | ? | _oid.py | 43 | Match:     ADMISSIONS = ObjectIdentifier("1.3.36.8.3.3") |
| HIGH | ? | _oid.py | 47 | Match:     NONCE = ObjectIdentifier("1.3.6.1.5.5.7.48.1.2") |
| HIGH | ? | _oid.py | 48 | Match:     ACCEPTABLE_RESPONSES = ObjectIdentifier("1.3.6.1. |
| HIGH | ? | _oid.py | 52 | Match:     CERTIFICATE_ISSUER = ObjectIdentifier("2.5.29.29" |
| HIGH | ? | _oid.py | 53 | Match:     CRL_REASON = ObjectIdentifier("2.5.29.21") |
| HIGH | ? | _oid.py | 54 | Match:     INVALIDITY_DATE = ObjectIdentifier("2.5.29.24") |
| HIGH | ? | _oid.py | 58 | Match:     COMMON_NAME = ObjectIdentifier("2.5.4.3") |
| HIGH | ? | _oid.py | 59 | Match:     COUNTRY_NAME = ObjectIdentifier("2.5.4.6") |
| HIGH | ? | _oid.py | 60 | Match:     LOCALITY_NAME = ObjectIdentifier("2.5.4.7") |
| HIGH | ? | _oid.py | 61 | Match:     STATE_OR_PROVINCE_NAME = ObjectIdentifier("2.5.4. |
| HIGH | ? | _oid.py | 62 | Match:     STREET_ADDRESS = ObjectIdentifier("2.5.4.9") |
| HIGH | ? | _oid.py | 63 | Match:     ORGANIZATION_IDENTIFIER = ObjectIdentifier("2.5.4 |
| HIGH | ? | _oid.py | 64 | Match:     ORGANIZATION_NAME = ObjectIdentifier("2.5.4.10") |
| HIGH | ? | _oid.py | 65 | Match:     ORGANIZATIONAL_UNIT_NAME = ObjectIdentifier("2.5. |
| HIGH | ? | _oid.py | 66 | Match:     SERIAL_NUMBER = ObjectIdentifier("2.5.4.5") |
| HIGH | ? | _oid.py | 67 | Match:     SURNAME = ObjectIdentifier("2.5.4.4") |
| HIGH | ? | _oid.py | 68 | Match:     GIVEN_NAME = ObjectIdentifier("2.5.4.42") |
| HIGH | ? | _oid.py | 69 | Match:     TITLE = ObjectIdentifier("2.5.4.12") |
| HIGH | ? | _oid.py | 70 | Match:     INITIALS = ObjectIdentifier("2.5.4.43") |
| HIGH | ? | _oid.py | 71 | Match:     GENERATION_QUALIFIER = ObjectIdentifier("2.5.4.44 |
| HIGH | ? | _oid.py | 72 | Match:     X500_UNIQUE_IDENTIFIER = ObjectIdentifier("2.5.4. |
| HIGH | ? | _oid.py | 73 | Match:     DN_QUALIFIER = ObjectIdentifier("2.5.4.46") |
| HIGH | ? | _oid.py | 74 | Match:     PSEUDONYM = ObjectIdentifier("2.5.4.65") |
| HIGH | ? | _oid.py | 75 | Match:     USER_ID = ObjectIdentifier("0.9.2342.19200300.100 |
| HIGH | ? | _oid.py | 76 | Match:     DOMAIN_COMPONENT = ObjectIdentifier("0.9.2342.192 |
| HIGH | ? | _oid.py | 77 | Match:     EMAIL_ADDRESS = ObjectIdentifier("1.2.840.113549. |
| HIGH | ? | _oid.py | 78 | Match:     JURISDICTION_COUNTRY_NAME = ObjectIdentifier("1.3 |
| HIGH | ? | _oid.py | 79 | Match:     JURISDICTION_LOCALITY_NAME = ObjectIdentifier("1. |
| HIGH | ? | _oid.py | 81 | Match:         "1.3.6.1.4.1.311.60.2.1.2" |
| HIGH | ? | _oid.py | 83 | Match:     BUSINESS_CATEGORY = ObjectIdentifier("2.5.4.15") |
| HIGH | ? | _oid.py | 84 | Match:     POSTAL_ADDRESS = ObjectIdentifier("2.5.4.16") |
| HIGH | ? | _oid.py | 85 | Match:     POSTAL_CODE = ObjectIdentifier("2.5.4.17") |
| HIGH | ? | _oid.py | 86 | Match:     INN = ObjectIdentifier("1.2.643.3.131.1.1") |
| HIGH | ? | _oid.py | 89 | Match:     UNSTRUCTURED_NAME = ObjectIdentifier("1.2.840.113 |
| HIGH | ? | _oid.py | 93 | Match:     RSA_WITH_MD5 = ObjectIdentifier("1.2.840.113549.1 |
| HIGH | ? | _oid.py | 94 | Match:     RSA_WITH_SHA1 = ObjectIdentifier("1.2.840.113549. |
| HIGH | ? | _oid.py | 96 | Match:     _RSA_WITH_SHA1 = ObjectIdentifier("1.3.14.3.2.29" |
| HIGH | ? | _oid.py | 97 | Match:     RSA_WITH_SHA224 = ObjectIdentifier("1.2.840.11354 |
| HIGH | ? | _oid.py | 98 | Match:     RSA_WITH_SHA256 = ObjectIdentifier("1.2.840.11354 |
| HIGH | ? | _oid.py | 99 | Match:     RSA_WITH_SHA384 = ObjectIdentifier("1.2.840.11354 |
| HIGH | ? | _oid.py | 100 | Match:     RSA_WITH_SHA512 = ObjectIdentifier("1.2.840.11354 |
| HIGH | ? | _oid.py | 101 | Match:     RSA_WITH_SHA3_224 = ObjectIdentifier("2.16.840.1. |
| HIGH | ? | _oid.py | 102 | Match:     RSA_WITH_SHA3_256 = ObjectIdentifier("2.16.840.1. |
| HIGH | ? | _oid.py | 103 | Match:     RSA_WITH_SHA3_384 = ObjectIdentifier("2.16.840.1. |
| HIGH | ? | _oid.py | 104 | Match:     RSA_WITH_SHA3_512 = ObjectIdentifier("2.16.840.1. |
| HIGH | ? | _oid.py | 105 | Match:     RSASSA_PSS = ObjectIdentifier("1.2.840.113549.1.1 |
| HIGH | ? | _oid.py | 107 | Match:     ECDSA_WITH_SHA224 = ObjectIdentifier("1.2.840.100 |
| HIGH | ? | _oid.py | 108 | Match:     ECDSA_WITH_SHA256 = ObjectIdentifier("1.2.840.100 |
| HIGH | ? | _oid.py | 109 | Match:     ECDSA_WITH_SHA384 = ObjectIdentifier("1.2.840.100 |
| HIGH | ? | _oid.py | 110 | Match:     ECDSA_WITH_SHA512 = ObjectIdentifier("1.2.840.100 |
| HIGH | ? | _oid.py | 111 | Match:     ECDSA_WITH_SHA3_224 = ObjectIdentifier("2.16.840. |
| HIGH | ? | _oid.py | 112 | Match:     ECDSA_WITH_SHA3_256 = ObjectIdentifier("2.16.840. |
| HIGH | ? | _oid.py | 113 | Match:     ECDSA_WITH_SHA3_384 = ObjectIdentifier("2.16.840. |
| HIGH | ? | _oid.py | 114 | Match:     ECDSA_WITH_SHA3_512 = ObjectIdentifier("2.16.840. |
| HIGH | ? | _oid.py | 116 | Match:     DSA_WITH_SHA224 = ObjectIdentifier("2.16.840.1.10 |
| HIGH | ? | _oid.py | 117 | Match:     DSA_WITH_SHA256 = ObjectIdentifier("2.16.840.1.10 |
| HIGH | ? | _oid.py | 118 | Match:     DSA_WITH_SHA384 = ObjectIdentifier("2.16.840.1.10 |
| HIGH | ? | _oid.py | 119 | Match:     DSA_WITH_SHA512 = ObjectIdentifier("2.16.840.1.10 |
| HIGH | ? | _oid.py | 120 | Match:     ED25519 = ObjectIdentifier("1.3.101.112") |
| HIGH | ? | _oid.py | 121 | Match:     ED448 = ObjectIdentifier("1.3.101.113") |
| HIGH | ? | _oid.py | 122 | Match:     ML_DSA_44 = ObjectIdentifier("2.16.840.1.101.3.4. |
| HIGH | ? | _oid.py | 123 | Match:     ML_DSA_65 = ObjectIdentifier("2.16.840.1.101.3.4. |
| HIGH | ? | _oid.py | 124 | Match:     ML_DSA_87 = ObjectIdentifier("2.16.840.1.101.3.4. |
| HIGH | ? | _oid.py | 125 | Match:     GOSTR3411_94_WITH_3410_2001 = ObjectIdentifier("1 |
| HIGH | ? | _oid.py | 126 | Match:     GOSTR3410_2012_WITH_3411_2012_256 = ObjectIdentif |
| HIGH | ? | _oid.py | 127 | Match:     GOSTR3410_2012_WITH_3411_2012_512 = ObjectIdentif |
| HIGH | ? | _oid.py | 166 | Match:     SHA1 = ObjectIdentifier("1.3.14.3.2.26") |
| HIGH | ? | _oid.py | 167 | Match:     SHA224 = ObjectIdentifier("2.16.840.1.101.3.4.2.4 |
| HIGH | ? | _oid.py | 168 | Match:     SHA256 = ObjectIdentifier("2.16.840.1.101.3.4.2.1 |
| HIGH | ? | _oid.py | 169 | Match:     SHA384 = ObjectIdentifier("2.16.840.1.101.3.4.2.2 |
| HIGH | ? | _oid.py | 170 | Match:     SHA512 = ObjectIdentifier("2.16.840.1.101.3.4.2.3 |
| HIGH | ? | _oid.py | 171 | Match:     SHA3_224 = ObjectIdentifier("1.3.6.1.4.1.37476.3. |
| HIGH | ? | _oid.py | 172 | Match:     SHA3_256 = ObjectIdentifier("1.3.6.1.4.1.37476.3. |
| HIGH | ? | _oid.py | 173 | Match:     SHA3_384 = ObjectIdentifier("1.3.6.1.4.1.37476.3. |
| HIGH | ? | _oid.py | 174 | Match:     SHA3_512 = ObjectIdentifier("1.3.6.1.4.1.37476.3. |
| HIGH | ? | _oid.py | 175 | Match:     SHA3_224_NIST = ObjectIdentifier("2.16.840.1.101. |
| HIGH | ? | _oid.py | 176 | Match:     SHA3_256_NIST = ObjectIdentifier("2.16.840.1.101. |
| HIGH | ? | _oid.py | 177 | Match:     SHA3_384_NIST = ObjectIdentifier("2.16.840.1.101. |
| HIGH | ? | _oid.py | 178 | Match:     SHA3_512_NIST = ObjectIdentifier("2.16.840.1.101. |
| HIGH | ? | _oid.py | 184 | Match:     RSAES_PKCS1_v1_5 = ObjectIdentifier("1.2.840.1135 |
| HIGH | ? | _oid.py | 185 | Match:     RSASSA_PSS = ObjectIdentifier("1.2.840.113549.1.1 |
| HIGH | ? | _oid.py | 186 | Match:     X25519 = ObjectIdentifier("1.3.101.110") |
| HIGH | ? | _oid.py | 187 | Match:     X448 = ObjectIdentifier("1.3.101.111") |
| HIGH | ? | _oid.py | 188 | Match:     ED25519 = ObjectIdentifier("1.3.101.112") |
| HIGH | ? | _oid.py | 189 | Match:     ED448 = ObjectIdentifier("1.3.101.113") |
| HIGH | ? | _oid.py | 190 | Match:     ML_DSA_44 = ObjectIdentifier("2.16.840.1.101.3.4. |
| HIGH | ? | _oid.py | 191 | Match:     ML_DSA_65 = ObjectIdentifier("2.16.840.1.101.3.4. |
| HIGH | ? | _oid.py | 192 | Match:     ML_DSA_87 = ObjectIdentifier("2.16.840.1.101.3.4. |
| HIGH | ? | _oid.py | 196 | Match:     SERVER_AUTH = ObjectIdentifier("1.3.6.1.5.5.7.3.1 |
| HIGH | ? | _oid.py | 197 | Match:     CLIENT_AUTH = ObjectIdentifier("1.3.6.1.5.5.7.3.2 |
| HIGH | ? | _oid.py | 198 | Match:     CODE_SIGNING = ObjectIdentifier("1.3.6.1.5.5.7.3. |
| HIGH | ? | _oid.py | 199 | Match:     EMAIL_PROTECTION = ObjectIdentifier("1.3.6.1.5.5. |
| HIGH | ? | _oid.py | 200 | Match:     TIME_STAMPING = ObjectIdentifier("1.3.6.1.5.5.7.3 |
| HIGH | ? | _oid.py | 201 | Match:     OCSP_SIGNING = ObjectIdentifier("1.3.6.1.5.5.7.3. |
| HIGH | ? | _oid.py | 202 | Match:     ANY_EXTENDED_KEY_USAGE = ObjectIdentifier("2.5.29 |
| HIGH | ? | _oid.py | 203 | Match:     SMARTCARD_LOGON = ObjectIdentifier("1.3.6.1.4.1.3 |
| HIGH | ? | _oid.py | 204 | Match:     KERBEROS_PKINIT_KDC = ObjectIdentifier("1.3.6.1.5 |
| HIGH | ? | _oid.py | 205 | Match:     IPSEC_IKE = ObjectIdentifier("1.3.6.1.5.5.7.3.17" |
| HIGH | ? | _oid.py | 206 | Match:     BUNDLE_SECURITY = ObjectIdentifier("1.3.6.1.5.5.7 |
| HIGH | ? | _oid.py | 207 | Match:     CERTIFICATE_TRANSPARENCY = ObjectIdentifier("1.3. |
| HIGH | ? | _oid.py | 211 | Match:     PERMANENT_IDENTIFIER = ObjectIdentifier("1.3.6.1. |
| HIGH | ? | _oid.py | 212 | Match:     HW_MODULE_NAME = ObjectIdentifier("1.3.6.1.5.5.7. |
| HIGH | ? | _oid.py | 213 | Match:     DNS_SRV = ObjectIdentifier("1.3.6.1.5.5.7.8.7") |
| HIGH | ? | _oid.py | 214 | Match:     NAI_REALM = ObjectIdentifier("1.3.6.1.5.5.7.8.8") |
| HIGH | ? | _oid.py | 215 | Match:     SMTP_UTF8_MAILBOX = ObjectIdentifier("1.3.6.1.5.5 |
| HIGH | ? | _oid.py | 216 | Match:     ACP_NODE_NAME = ObjectIdentifier("1.3.6.1.5.5.7.8 |
| HIGH | ? | _oid.py | 217 | Match:     BUNDLE_EID = ObjectIdentifier("1.3.6.1.5.5.7.8.11 |
| HIGH | ? | _oid.py | 221 | Match:     CA_ISSUERS = ObjectIdentifier("1.3.6.1.5.5.7.48.2 |
| HIGH | ? | _oid.py | 222 | Match:     OCSP = ObjectIdentifier("1.3.6.1.5.5.7.48.1") |
| HIGH | ? | _oid.py | 226 | Match:     CA_REPOSITORY = ObjectIdentifier("1.3.6.1.5.5.7.4 |
| HIGH | ? | _oid.py | 230 | Match:     CPS_QUALIFIER = ObjectIdentifier("1.3.6.1.5.5.7.2 |
| HIGH | ? | _oid.py | 231 | Match:     CPS_USER_NOTICE = ObjectIdentifier("1.3.6.1.5.5.7 |
| HIGH | ? | _oid.py | 232 | Match:     ANY_POLICY = ObjectIdentifier("2.5.29.32.0") |
| HIGH | ? | _oid.py | 236 | Match:     CHALLENGE_PASSWORD = ObjectIdentifier("1.2.840.11 |
| HIGH | ? | _oid.py | 237 | Match:     UNSTRUCTURED_NAME = ObjectIdentifier("1.2.840.113 |
| HIGH | ? | unsupported_extension.pem | 30 | Match:             1.2.3.4:  |
| HIGH | ? | unsupported_extension_critical.pem | 30 | Match:             1.2.3.4: critical |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 129 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 151 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 261 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 283 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 311 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 366 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 454 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 476 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 592 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 603 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 801 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 812 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 107 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 140 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 239 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 272 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 344 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 355 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 443 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 487 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 570 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 614 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 746 | Match: Result = F (3 - IUT's Static public key fails PKV 5.6 |
| HIGH | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 801 | Match: Result = F (1 - CAVS's Static public key fails PKV 5. |
| HIGH | ? | pkits.schema | 1 | Match: objectclass ( 1.2.840.113533.7.67.14 |
| HIGH | ? | pkits.schema | 4 | Match: objectclass ( 1.3.6.1.4.1.18227.2.1.2 NAME 'opencaEma |
| HIGH | ? | pkits.schema | 12 | Match: objectclass ( 1.2.840.113533.7.67.15 |
| HIGH | ? | pkits.schema | 19 | Match: objectclass ( 1.2.840.113549.1.9.24.2 |
| HIGH | ? | pkits.ldif | 377 | Match: dn: title=M.D.,generationQualifier=III,sn=CA,2.5.4.65 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 82 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 118 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 172 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 244 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 352 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 424 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 442 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 478 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 678 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 750 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 786 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 804 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 894 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 912 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1002 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1020 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1166 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1274 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1346 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1400 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1454 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1562 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1580 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1652 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1690 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1708 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1726 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1942 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2014 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2068 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2140 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2194 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2232 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2268 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2304 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2376 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2520 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2556 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2664 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2682 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2792 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2846 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2864 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3008 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3134 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3152 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3224 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3242 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3442 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3460 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3514 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3532 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3586 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3622 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3694 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3802 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3912 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3984 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4020 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4074 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4200 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4254 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4326 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4380 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4490 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4508 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4544 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4616 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4688 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4742 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4760 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4922 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4996 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5014 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5032 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5068 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5230 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5338 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5410 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5428 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 64 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 82 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 118 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 226 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 334 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 352 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 388 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 496 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 696 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 714 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 822 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 840 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 894 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 912 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 930 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 948 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1202 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1220 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1238 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1328 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1418 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1508 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1526 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1562 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1690 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1852 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1906 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1942 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1960 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1978 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1996 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2068 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2232 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2322 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2448 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2484 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2502 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2520 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2610 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2682 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2810 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2900 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2954 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3026 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3044 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3080 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3098 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3206 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3424 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3442 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3550 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3568 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3604 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3676 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3748 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3766 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3966 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3984 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4002 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4056 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4146 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4164 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4254 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4272 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4418 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4436 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4508 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4598 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4706 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4778 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4796 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4886 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4942 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5032 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5122 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5194 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5230 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5248 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5374 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5392 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 55 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 81 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 146 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 159 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 237 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 250 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 276 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 393 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 447 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 460 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 486 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 590 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 655 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 668 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 746 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 759 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 839 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 930 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 956 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 982 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1073 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1086 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1138 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1164 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1244 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1283 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1309 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1400 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1452 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1478 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1491 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1556 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1623 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1636 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1649 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1675 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1831 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1896 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1922 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1987 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 81 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 107 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 159 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 224 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 276 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 341 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 367 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 406 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 473 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 486 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 512 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 538 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 694 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 707 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 720 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 746 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 826 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 839 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 904 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 956 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1021 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1151 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1164 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1190 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1283 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1322 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1361 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1400 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1491 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1543 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1556 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1582 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1636 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1649 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1675 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1753 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1922 | Match: Result = F (6 - IUT's Static public key Y fails PKV 5 |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1935 | Match: Result = F (1 - CAVS's Static public key X fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1948 | Match: Result = F (2 - CAVS's Static public key Y fails PKV  |
| HIGH | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1961 | Match: Result = F (5 - IUT's Static public key X fails PKV 5 |
| HIGH | ? | utils.py | 17 | Match:     exec(f.read(), about) |
| HIGH | ? | .readthedocs.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | dh_key_256.pem | 0 | File dh_key_256.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | dhkey.pem | 0 | File dhkey.pem has permissions -rw-rw-r-- — readable by any  |
| HIGH | GS002 | dhkey_rfc5114_2.pem | 0 | File dhkey_rfc5114_2.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | dhp.pem | 0 | File dhp.pem has permissions -rw-rw-r-- — readable by any us |
| HIGH | GS002 | dhp_privatevaluelength.pem | 0 | File dhp_privatevaluelength.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | dhp_rfc5114_2.pem | 0 | File dhp_rfc5114_2.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | dhpub.pem | 0 | File dhpub.pem has permissions -rw-rw-r-- — readable by any  |
| HIGH | GS002 | dhpub_cryptography_old.pem | 0 | File dhpub_cryptography_old.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | dhpub_rfc5114_2.pem | 0 | File dhpub_rfc5114_2.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | nilpotent.pem | 0 | File nilpotent.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | ec-missing-curve.pem | 0 | File ec-missing-curve.pem has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | explicit_parameters_private_key.pem | 0 | File explicit_parameters_private_key.pem has permissions -rw |
| HIGH | GS002 | explicit_parameters_wap_wsg_idm_ecid_wtls11_private_key.pem | 0 | File explicit_parameters_wap_wsg_idm_ecid_wtls11_private_key |
| HIGH | GS002 | high-bit-set.pem | 0 | File high-bit-set.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | secp128r1_private_key.pem | 0 | File secp128r1_private_key.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | secp256k1-explicit-no-seed.pem | 0 | File secp256k1-explicit-no-seed.pem has permissions -rw-rw-r |
| HIGH | GS002 | secp256k1-pub-explicit-no-seed.pem | 0 | File secp256k1-pub-explicit-no-seed.pem has permissions -rw- |
| HIGH | GS002 | secp256r1-explicit-no-seed.pem | 0 | File secp256r1-explicit-no-seed.pem has permissions -rw-rw-r |
| HIGH | GS002 | secp256r1-explicit-seed.pem | 0 | File secp256r1-explicit-seed.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | secp256r1-pub-explicit-no-seed.pem | 0 | File secp256r1-pub-explicit-no-seed.pem has permissions -rw- |
| HIGH | GS002 | secp256r1-pub-explicit-seed.pem | 0 | File secp256r1-pub-explicit-seed.pem has permissions -rw-rw- |
| HIGH | GS002 | secp384r1-explicit-no-seed.pem | 0 | File secp384r1-explicit-no-seed.pem has permissions -rw-rw-r |
| HIGH | GS002 | secp384r1-explicit-seed.pem | 0 | File secp384r1-explicit-seed.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | secp384r1-pub-explicit-no-seed.pem | 0 | File secp384r1-pub-explicit-no-seed.pem has permissions -rw- |
| HIGH | GS002 | secp384r1-pub-explicit-seed.pem | 0 | File secp384r1-pub-explicit-seed.pem has permissions -rw-rw- |
| HIGH | GS002 | secp521r1-explicit-no-seed.pem | 0 | File secp521r1-explicit-no-seed.pem has permissions -rw-rw-r |
| HIGH | GS002 | secp521r1-explicit-seed.pem | 0 | File secp521r1-explicit-seed.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | secp521r1-pub-explicit-no-seed.pem | 0 | File secp521r1-pub-explicit-no-seed.pem has permissions -rw- |
| HIGH | GS002 | secp521r1-pub-explicit-seed.pem | 0 | File secp521r1-pub-explicit-seed.pem has permissions -rw-rw- |
| HIGH | GS002 | sect163k1-spki.pem | 0 | File sect163k1-spki.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | sect163r2-spki.pem | 0 | File sect163r2-spki.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | sect233k1-spki.pem | 0 | File sect233k1-spki.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | sect233r1-spki.pem | 0 | File sect233r1-spki.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | ed25519-pkcs8-enc.pem | 0 | File ed25519-pkcs8-enc.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | ed25519-pkcs8.pem | 0 | File ed25519-pkcs8.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | ed25519-pub.pem | 0 | File ed25519-pub.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | ed448-pkcs8-enc.pem | 0 | File ed448-pkcs8-enc.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | ed448-pkcs8.pem | 0 | File ed448-pkcs8.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | ed448-pub.pem | 0 | File ed448-pub.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | mlkem768.pem | 0 | File mlkem768.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | dsa-nopsw.key | 0 | File dsa-nopsw.key has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | dsa-psw.key | 0 | File dsa-psw.key has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | ecdsa-nopsw.key | 0 | File ecdsa-nopsw.key has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | ecdsa-psw.key | 0 | File ecdsa-psw.key has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | ed25519-aesgcm-psw.key | 0 | File ed25519-aesgcm-psw.key has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | ed25519-nopsw.key | 0 | File ed25519-nopsw.key has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | ed25519-psw.key | 0 | File ed25519-psw.key has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | rsa-nopsw.key | 0 | File rsa-nopsw.key has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | rsa-psw.key | 0 | File rsa-psw.key has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | sk-ecdsa-nopsw.key | 0 | File sk-ecdsa-nopsw.key has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | sk-ecdsa-psw.key | 0 | File sk-ecdsa-psw.key has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | sk-ed25519-nopsw.key | 0 | File sk-ed25519-nopsw.key has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | sk-ed25519-psw.key | 0 | File sk-ed25519-psw.key has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | dsa_4096.pem | 0 | File dsa_4096.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | dsa_private_key.pem | 0 | File dsa_private_key.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | dsa_public_key.pem | 0 | File dsa_public_key.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | dsaparam.pem | 0 | File dsaparam.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | ec_private_key.pem | 0 | File ec_private_key.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | ec_private_key_encrypted.pem | 0 | File ec_private_key_encrypted.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | ec_public_key.pem | 0 | File ec_public_key.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | ec_public_key_rsa_delimiter.pem | 0 | File ec_public_key_rsa_delimiter.pem has permissions -rw-rw- |
| HIGH | GS002 | rsa-bad-1025-q-is-2.pem | 0 | File rsa-bad-1025-q-is-2.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | rsa_private_key.pem | 0 | File rsa_private_key.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | rsa_public_key.pem | 0 | File rsa_public_key.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | rsa_wrong_delimiter_public_key.pem | 0 | File rsa_wrong_delimiter_public_key.pem has permissions -rw- |
| HIGH | GS002 | bad-encryption-oid.pem | 0 | File bad-encryption-oid.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | bad-oid-dsa-key.pem | 0 | File bad-oid-dsa-key.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | ec-consistent-curve.pem | 0 | File ec-consistent-curve.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | ec-inconsistent-curve.pem | 0 | File ec-inconsistent-curve.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | ec-inconsistent-curve2.pem | 0 | File ec-inconsistent-curve2.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | ec-invalid-private-scalar.pem | 0 | File ec-invalid-private-scalar.pem has permissions -rw-rw-r- |
| HIGH | GS002 | ec-invalid-version.pem | 0 | File ec-invalid-version.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | ec_oid_not_in_reg_private_2.pkcs8.pem | 0 | File ec_oid_not_in_reg_private_2.pkcs8.pem has permissions - |
| HIGH | GS002 | ec_private_key.pem | 0 | File ec_private_key.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | ec_private_key_encrypted.pem | 0 | File ec_private_key_encrypted.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | ecc_private_with_rfc5915_ext.pem | 0 | File ecc_private_with_rfc5915_ext.pem has permissions -rw-rw |
| HIGH | GS002 | ed25519-scrypt.pem | 0 | File ed25519-scrypt.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | enc-ec-sha1-128-rc4.pem | 0 | File enc-ec-sha1-128-rc4.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | enc-rsa-3des.pem | 0 | File enc-rsa-3des.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | enc-rsa-pkcs8-pbkdf2-0iter.pem | 0 | File enc-rsa-pkcs8-pbkdf2-0iter.pem has permissions -rw-rw-r |
| HIGH | GS002 | enc-rsa-pkcs8.pem | 0 | File enc-rsa-pkcs8.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | enc-unknown-algorithm.pem | 0 | File enc-unknown-algorithm.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | enc-unknown-kdf.pem | 0 | File enc-unknown-kdf.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | enc-unknown-pbkdf2-prf.pem | 0 | File enc-unknown-pbkdf2-prf.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | enc2-rsa-pkcs8.pem | 0 | File enc2-rsa-pkcs8.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | nodompar_private.pkcs8.pem | 0 | File nodompar_private.pkcs8.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | pkcs12_s2k_pem-X_9607.pem | 0 | File pkcs12_s2k_pem-X_9607.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9671.pem | 0 | File pkcs12_s2k_pem-X_9671.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9925.pem | 0 | File pkcs12_s2k_pem-X_9925.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9926.pem | 0 | File pkcs12_s2k_pem-X_9926.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9927.pem | 0 | File pkcs12_s2k_pem-X_9927.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9928.pem | 0 | File pkcs12_s2k_pem-X_9928.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9929.pem | 0 | File pkcs12_s2k_pem-X_9929.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9930.pem | 0 | File pkcs12_s2k_pem-X_9930.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9931.pem | 0 | File pkcs12_s2k_pem-X_9931.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | pkcs12_s2k_pem-X_9932.pem | 0 | File pkcs12_s2k_pem-X_9932.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | private.pem | 0 | File private.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | rsa-40bitrc2.pem | 0 | File rsa-40bitrc2.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | rsa-aes-192-cbc.pem | 0 | File rsa-aes-192-cbc.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | rsa-pbe-3des-long-salt.pem | 0 | File rsa-pbe-3des-long-salt.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | rsa-pbewithmd5anddescbc.pem | 0 | File rsa-pbewithmd5anddescbc.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | rsa-rc2-cbc-effective-key-length.pem | 0 | File rsa-rc2-cbc-effective-key-length.pem has permissions -r |
| HIGH | GS002 | rsa-rc2-cbc.pem | 0 | File rsa-rc2-cbc.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha224.pem | 0 | File rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha224.pem has permiss |
| HIGH | GS002 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha384.pem | 0 | File rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha384.pem has permiss |
| HIGH | GS002 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha512.pem | 0 | File rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha512.pem has permiss |
| HIGH | GS002 | rsa_pss_2048.pem | 0 | File rsa_pss_2048.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | rsa_pss_2048_hash.pem | 0 | File rsa_pss_2048_hash.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | rsa_pss_2048_hash_mask.pem | 0 | File rsa_pss_2048_hash_mask.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | rsa_pss_2048_hash_mask_diff.pem | 0 | File rsa_pss_2048_hash_mask_diff.pem has permissions -rw-rw- |
| HIGH | GS002 | rsa_pss_2048_hash_mask_salt.pem | 0 | File rsa_pss_2048_hash_mask_salt.pem has permissions -rw-rw- |
| HIGH | GS002 | unenc-dsa-pkcs8.pem | 0 | File unenc-dsa-pkcs8.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | unenc-dsa-pkcs8.pub.pem | 0 | File unenc-dsa-pkcs8.pub.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | unenc-rsa-pkcs8.pem | 0 | File unenc-rsa-pkcs8.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | unenc-rsa-pkcs8.pub.pem | 0 | File unenc-rsa-pkcs8.pub.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | withdompar_private.pkcs8.pem | 0 | File withdompar_private.pkcs8.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | wrong-pem-delimiter-rsa.pem | 0 | File wrong-pem-delimiter-rsa.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | dsa-wrong-version.pem | 0 | File dsa-wrong-version.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | dsa.1024.pem | 0 | File dsa.1024.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | dsa.2048.pem | 0 | File dsa.2048.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | dsa.3072.pem | 0 | File dsa.3072.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | key1-malformed-dek-info.pem | 0 | File key1-malformed-dek-info.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | key1-malformed-iv.pem | 0 | File key1-malformed-iv.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | key1-no-dek-info.pem | 0 | File key1-no-dek-info.pem has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | key1-short-iv.pem | 0 | File key1-short-iv.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | key1.pem | 0 | File key1.pem has permissions -rw-rw-r-- — readable by any u |
| HIGH | GS002 | key2.pem | 0 | File key2.pem has permissions -rw-rw-r-- — readable by any u |
| HIGH | GS002 | rsa-wrong-version.pem | 0 | File rsa-wrong-version.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | testrsa-encrypted.pem | 0 | File testrsa-encrypted.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | testrsa.pem | 0 | File testrsa.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | x25519-pkcs8-enc.pem | 0 | File x25519-pkcs8-enc.pem has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | x25519-pkcs8.pem | 0 | File x25519-pkcs8.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | x25519-pub.pem | 0 | File x25519-pub.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | x448-pkcs8-enc.pem | 0 | File x448-pkcs8-enc.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | x448-pkcs8.pem | 0 | File x448-pkcs8.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | x448-pub.pem | 0 | File x448-pub.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | dsa.pub.pem | 0 | File dsa.pub.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | rsa.pub.pem | 0 | File rsa.pub.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | ca.pem | 0 | File ca.pem has permissions -rw-rw-r-- — readable by any use |
| HIGH | GS002 | ca_key.pem | 0 | File ca_key.pem has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | cert-aes256cbc-no-key.p12 | 0 | File cert-aes256cbc-no-key.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | cert-key-aes256cbc.p12 | 0 | File cert-key-aes256cbc.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | cert-none-key-none.p12 | 0 | File cert-none-key-none.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | cert-rc2-key-3des.p12 | 0 | File cert-rc2-key-3des.p12 has permissions -rw-rw-r-- — read |
| HIGH | GS002 | java-truststore.p12 | 0 | File java-truststore.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | name-1-no-pwd.p12 | 0 | File name-1-no-pwd.p12 has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | name-1-pwd.p12 | 0 | File name-1-pwd.p12 has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | name-2-3-no-pwd.p12 | 0 | File name-2-3-no-pwd.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | name-2-3-pwd.p12 | 0 | File name-2-3-pwd.p12 has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | name-2-no-pwd.p12 | 0 | File name-2-no-pwd.p12 has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | name-2-pwd.p12 | 0 | File name-2-pwd.p12 has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | name-3-no-pwd.p12 | 0 | File name-3-no-pwd.p12 has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | name-3-pwd.p12 | 0 | File name-3-pwd.p12 has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | name-all-no-pwd.p12 | 0 | File name-all-no-pwd.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | name-all-pwd.p12 | 0 | File name-all-pwd.p12 has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | name-unicode-no-pwd.p12 | 0 | File name-unicode-no-pwd.p12 has permissions -rw-rw-r-- — re |
| HIGH | GS002 | name-unicode-pwd.p12 | 0 | File name-unicode-pwd.p12 has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | no-cert-key-aes256cbc.p12 | 0 | File no-cert-key-aes256cbc.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | no-cert-name-2-no-pwd.p12 | 0 | File no-cert-name-2-no-pwd.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | no-cert-name-2-pwd.p12 | 0 | File no-cert-name-2-pwd.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | no-cert-name-3-no-pwd.p12 | 0 | File no-cert-name-3-no-pwd.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | no-cert-name-3-pwd.p12 | 0 | File no-cert-name-3-pwd.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | no-cert-name-all-no-pwd.p12 | 0 | File no-cert-name-all-no-pwd.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | no-cert-name-all-pwd.p12 | 0 | File no-cert-name-all-pwd.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | no-cert-name-unicode-no-pwd.p12 | 0 | File no-cert-name-unicode-no-pwd.p12 has permissions -rw-rw- |
| HIGH | GS002 | no-cert-name-unicode-pwd.p12 | 0 | File no-cert-name-unicode-pwd.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | no-cert-no-name-no-pwd.p12 | 0 | File no-cert-no-name-no-pwd.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | no-cert-no-name-pwd.p12 | 0 | File no-cert-no-name-pwd.p12 has permissions -rw-rw-r-- — re |
| HIGH | GS002 | no-name-no-pwd.p12 | 0 | File no-name-no-pwd.p12 has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | no-name-pwd.p12 | 0 | File no-name-pwd.p12 has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | no-password.p12 | 0 | File no-password.p12 has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | ascii-san.pem | 0 | File ascii-san.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | enveloped-rsa-oaep.pem | 0 | File enveloped-rsa-oaep.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | enveloped-triple-des.pem | 0 | File enveloped-triple-des.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | enveloped.pem | 0 | File enveloped.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | isrg.pem | 0 | File isrg.pem has permissions -rw-rw-r-- — readable by any u |
| HIGH | GS002 | non-ascii-san.pem | 0 | File non-ascii-san.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | AllCertificatesNoPoliciesTest2EE.crt | 0 | File AllCertificatesNoPoliciesTest2EE.crt has permissions -r |
| HIGH | GS002 | AllCertificatesSamePoliciesTest10EE.crt | 0 | File AllCertificatesSamePoliciesTest10EE.crt has permissions |
| HIGH | GS002 | AllCertificatesSamePoliciesTest13EE.crt | 0 | File AllCertificatesSamePoliciesTest13EE.crt has permissions |
| HIGH | GS002 | AllCertificatesanyPolicyTest11EE.crt | 0 | File AllCertificatesanyPolicyTest11EE.crt has permissions -r |
| HIGH | GS002 | AnyPolicyTest14EE.crt | 0 | File AnyPolicyTest14EE.crt has permissions -rw-rw-r-- — read |
| HIGH | GS002 | BadCRLIssuerNameCACert.crt | 0 | File BadCRLIssuerNameCACert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | BadCRLSignatureCACert.crt | 0 | File BadCRLSignatureCACert.crt has permissions -rw-rw-r-- —  |
| HIGH | GS002 | BadSignedCACert.crt | 0 | File BadSignedCACert.crt has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | BadnotAfterDateCACert.crt | 0 | File BadnotAfterDateCACert.crt has permissions -rw-rw-r-- —  |
| HIGH | GS002 | BadnotBeforeDateCACert.crt | 0 | File BadnotBeforeDateCACert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | BasicSelfIssuedCRLSigningKeyCACert.crt | 0 | File BasicSelfIssuedCRLSigningKeyCACert.crt has permissions  |
| HIGH | GS002 | BasicSelfIssuedCRLSigningKeyCRLCert.crt | 0 | File BasicSelfIssuedCRLSigningKeyCRLCert.crt has permissions |
| HIGH | GS002 | BasicSelfIssuedNewKeyCACert.crt | 0 | File BasicSelfIssuedNewKeyCACert.crt has permissions -rw-rw- |
| HIGH | GS002 | BasicSelfIssuedNewKeyOldWithNewCACert.crt | 0 | File BasicSelfIssuedNewKeyOldWithNewCACert.crt has permissio |
| HIGH | GS002 | BasicSelfIssuedOldKeyCACert.crt | 0 | File BasicSelfIssuedOldKeyCACert.crt has permissions -rw-rw- |
| HIGH | GS002 | BasicSelfIssuedOldKeyNewWithOldCACert.crt | 0 | File BasicSelfIssuedOldKeyNewWithOldCACert.crt has permissio |
| HIGH | GS002 | CPSPointerQualifierTest20EE.crt | 0 | File CPSPointerQualifierTest20EE.crt has permissions -rw-rw- |
| HIGH | GS002 | DSACACert.crt | 0 | File DSACACert.crt has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | DSAParametersInheritedCACert.crt | 0 | File DSAParametersInheritedCACert.crt has permissions -rw-rw |
| HIGH | GS002 | DifferentPoliciesTest12EE.crt | 0 | File DifferentPoliciesTest12EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | DifferentPoliciesTest3EE.crt | 0 | File DifferentPoliciesTest3EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest4EE.crt | 0 | File DifferentPoliciesTest4EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest5EE.crt | 0 | File DifferentPoliciesTest5EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest7EE.crt | 0 | File DifferentPoliciesTest7EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest8EE.crt | 0 | File DifferentPoliciesTest8EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest9EE.crt | 0 | File DifferentPoliciesTest9EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | GeneralizedTimeCRLnextUpdateCACert.crt | 0 | File GeneralizedTimeCRLnextUpdateCACert.crt has permissions  |
| HIGH | GS002 | GoodCACert.crt | 0 | File GoodCACert.crt has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | GoodsubCACert.crt | 0 | File GoodsubCACert.crt has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | GoodsubCAPanyPolicyMapping1to2CACert.crt | 0 | File GoodsubCAPanyPolicyMapping1to2CACert.crt has permission |
| HIGH | GS002 | InvalidBadCRLIssuerNameTest5EE.crt | 0 | File InvalidBadCRLIssuerNameTest5EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidBadCRLSignatureTest4EE.crt | 0 | File InvalidBadCRLSignatureTest4EE.crt has permissions -rw-r |
| HIGH | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest7EE.crt | 0 | File InvalidBasicSelfIssuedCRLSigningKeyTest7EE.crt has perm |
| HIGH | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest8EE.crt | 0 | File InvalidBasicSelfIssuedCRLSigningKeyTest8EE.crt has perm |
| HIGH | GS002 | InvalidBasicSelfIssuedNewWithOldTest5EE.crt | 0 | File InvalidBasicSelfIssuedNewWithOldTest5EE.crt has permiss |
| HIGH | GS002 | InvalidBasicSelfIssuedOldWithNewTest2EE.crt | 0 | File InvalidBasicSelfIssuedOldWithNewTest2EE.crt has permiss |
| HIGH | GS002 | InvalidCASignatureTest2EE.crt | 0 | File InvalidCASignatureTest2EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | InvalidCAnotAfterDateTest5EE.crt | 0 | File InvalidCAnotAfterDateTest5EE.crt has permissions -rw-rw |
| HIGH | GS002 | InvalidCAnotBeforeDateTest1EE.crt | 0 | File InvalidCAnotBeforeDateTest1EE.crt has permissions -rw-r |
| HIGH | GS002 | InvalidDNSnameConstraintsTest31EE.crt | 0 | File InvalidDNSnameConstraintsTest31EE.crt has permissions - |
| HIGH | GS002 | InvalidDNSnameConstraintsTest33EE.crt | 0 | File InvalidDNSnameConstraintsTest33EE.crt has permissions - |
| HIGH | GS002 | InvalidDNSnameConstraintsTest38EE.crt | 0 | File InvalidDNSnameConstraintsTest38EE.crt has permissions - |
| HIGH | GS002 | InvalidDNandRFC822nameConstraintsTest28EE.crt | 0 | File InvalidDNandRFC822nameConstraintsTest28EE.crt has permi |
| HIGH | GS002 | InvalidDNandRFC822nameConstraintsTest29EE.crt | 0 | File InvalidDNandRFC822nameConstraintsTest29EE.crt has permi |
| HIGH | GS002 | InvalidDNnameConstraintsTest10EE.crt | 0 | File InvalidDNnameConstraintsTest10EE.crt has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest12EE.crt | 0 | File InvalidDNnameConstraintsTest12EE.crt has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest13EE.crt | 0 | File InvalidDNnameConstraintsTest13EE.crt has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest15EE.crt | 0 | File InvalidDNnameConstraintsTest15EE.crt has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest16EE.crt | 0 | File InvalidDNnameConstraintsTest16EE.crt has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest17EE.crt | 0 | File InvalidDNnameConstraintsTest17EE.crt has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest20EE.crt | 0 | File InvalidDNnameConstraintsTest20EE.crt has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest2EE.crt | 0 | File InvalidDNnameConstraintsTest2EE.crt has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest3EE.crt | 0 | File InvalidDNnameConstraintsTest3EE.crt has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest7EE.crt | 0 | File InvalidDNnameConstraintsTest7EE.crt has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest8EE.crt | 0 | File InvalidDNnameConstraintsTest8EE.crt has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest9EE.crt | 0 | File InvalidDNnameConstraintsTest9EE.crt has permissions -rw |
| HIGH | GS002 | InvalidDSASignatureTest6EE.crt | 0 | File InvalidDSASignatureTest6EE.crt has permissions -rw-rw-r |
| HIGH | GS002 | InvalidEESignatureTest3EE.crt | 0 | File InvalidEESignatureTest3EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | InvalidEEnotAfterDateTest6EE.crt | 0 | File InvalidEEnotAfterDateTest6EE.crt has permissions -rw-rw |
| HIGH | GS002 | InvalidEEnotBeforeDateTest2EE.crt | 0 | File InvalidEEnotBeforeDateTest2EE.crt has permissions -rw-r |
| HIGH | GS002 | InvalidIDPwithindirectCRLTest23EE.crt | 0 | File InvalidIDPwithindirectCRLTest23EE.crt has permissions - |
| HIGH | GS002 | InvalidIDPwithindirectCRLTest26EE.crt | 0 | File InvalidIDPwithindirectCRLTest26EE.crt has permissions - |
| HIGH | GS002 | InvalidLongSerialNumberTest18EE.crt | 0 | File InvalidLongSerialNumberTest18EE.crt has permissions -rw |
| HIGH | GS002 | InvalidMappingFromanyPolicyTest7EE.crt | 0 | File InvalidMappingFromanyPolicyTest7EE.crt has permissions  |
| HIGH | GS002 | InvalidMappingToanyPolicyTest8EE.crt | 0 | File InvalidMappingToanyPolicyTest8EE.crt has permissions -r |
| HIGH | GS002 | InvalidMissingCRLTest1EE.crt | 0 | File InvalidMissingCRLTest1EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidMissingbasicConstraintsTest1EE.crt | 0 | File InvalidMissingbasicConstraintsTest1EE.crt has permissio |
| HIGH | GS002 | InvalidNameChainingOrderTest2EE.crt | 0 | File InvalidNameChainingOrderTest2EE.crt has permissions -rw |
| HIGH | GS002 | InvalidNameChainingTest1EE.crt | 0 | File InvalidNameChainingTest1EE.crt has permissions -rw-rw-r |
| HIGH | GS002 | InvalidNegativeSerialNumberTest15EE.crt | 0 | File InvalidNegativeSerialNumberTest15EE.crt has permissions |
| HIGH | GS002 | InvalidOldCRLnextUpdateTest11EE.crt | 0 | File InvalidOldCRLnextUpdateTest11EE.crt has permissions -rw |
| HIGH | GS002 | InvalidPolicyMappingTest10EE.crt | 0 | File InvalidPolicyMappingTest10EE.crt has permissions -rw-rw |
| HIGH | GS002 | InvalidPolicyMappingTest2EE.crt | 0 | File InvalidPolicyMappingTest2EE.crt has permissions -rw-rw- |
| HIGH | GS002 | InvalidPolicyMappingTest4EE.crt | 0 | File InvalidPolicyMappingTest4EE.crt has permissions -rw-rw- |
| HIGH | GS002 | InvalidRFC822nameConstraintsTest22EE.crt | 0 | File InvalidRFC822nameConstraintsTest22EE.crt has permission |
| HIGH | GS002 | InvalidRFC822nameConstraintsTest24EE.crt | 0 | File InvalidRFC822nameConstraintsTest24EE.crt has permission |
| HIGH | GS002 | InvalidRFC822nameConstraintsTest26EE.crt | 0 | File InvalidRFC822nameConstraintsTest26EE.crt has permission |
| HIGH | GS002 | InvalidRevokedCATest2EE.crt | 0 | File InvalidRevokedCATest2EE.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | InvalidRevokedEETest3EE.crt | 0 | File InvalidRevokedEETest3EE.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest10EE.crt | 0 | File InvalidSelfIssuedinhibitAnyPolicyTest10EE.crt has permi |
| HIGH | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest8EE.crt | 0 | File InvalidSelfIssuedinhibitAnyPolicyTest8EE.crt has permis |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest10EE.crt | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest10EE.crt has p |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest11EE.crt | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest11EE.crt has p |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest8EE.crt | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest8EE.crt has pe |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest9EE.crt | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest9EE.crt has pe |
| HIGH | GS002 | InvalidSelfIssuedpathLenConstraintTest16EE.crt | 0 | File InvalidSelfIssuedpathLenConstraintTest16EE.crt has perm |
| HIGH | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest7EE.crt | 0 | File InvalidSelfIssuedrequireExplicitPolicyTest7EE.crt has p |
| HIGH | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest8EE.crt | 0 | File InvalidSelfIssuedrequireExplicitPolicyTest8EE.crt has p |
| HIGH | GS002 | InvalidSeparateCertificateandCRLKeysTest20EE.crt | 0 | File InvalidSeparateCertificateandCRLKeysTest20EE.crt has pe |
| HIGH | GS002 | InvalidSeparateCertificateandCRLKeysTest21EE.crt | 0 | File InvalidSeparateCertificateandCRLKeysTest21EE.crt has pe |
| HIGH | GS002 | InvalidURInameConstraintsTest35EE.crt | 0 | File InvalidURInameConstraintsTest35EE.crt has permissions - |
| HIGH | GS002 | InvalidURInameConstraintsTest37EE.crt | 0 | File InvalidURInameConstraintsTest37EE.crt has permissions - |
| HIGH | GS002 | InvalidUnknownCRLEntryExtensionTest8EE.crt | 0 | File InvalidUnknownCRLEntryExtensionTest8EE.crt has permissi |
| HIGH | GS002 | InvalidUnknownCRLExtensionTest10EE.crt | 0 | File InvalidUnknownCRLExtensionTest10EE.crt has permissions  |
| HIGH | GS002 | InvalidUnknownCRLExtensionTest9EE.crt | 0 | File InvalidUnknownCRLExtensionTest9EE.crt has permissions - |
| HIGH | GS002 | InvalidUnknownCriticalCertificateExtensionTest2EE.crt | 0 | File InvalidUnknownCriticalCertificateExtensionTest2EE.crt h |
| HIGH | GS002 | InvalidWrongCRLTest6EE.crt | 0 | File InvalidWrongCRLTest6EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvalidcAFalseTest2EE.crt | 0 | File InvalidcAFalseTest2EE.crt has permissions -rw-rw-r-- —  |
| HIGH | GS002 | InvalidcAFalseTest3EE.crt | 0 | File InvalidcAFalseTest3EE.crt has permissions -rw-rw-r-- —  |
| HIGH | GS002 | InvalidcRLIssuerTest27EE.crt | 0 | File InvalidcRLIssuerTest27EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest31EE.crt | 0 | File InvalidcRLIssuerTest31EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest32EE.crt | 0 | File InvalidcRLIssuerTest32EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest34EE.crt | 0 | File InvalidcRLIssuerTest34EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest35EE.crt | 0 | File InvalidcRLIssuerTest35EE.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | InvaliddeltaCRLIndicatorNoBaseTest1EE.crt | 0 | File InvaliddeltaCRLIndicatorNoBaseTest1EE.crt has permissio |
| HIGH | GS002 | InvaliddeltaCRLTest10EE.crt | 0 | File InvaliddeltaCRLTest10EE.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | InvaliddeltaCRLTest3EE.crt | 0 | File InvaliddeltaCRLTest3EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddeltaCRLTest4EE.crt | 0 | File InvaliddeltaCRLTest4EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddeltaCRLTest6EE.crt | 0 | File InvaliddeltaCRLTest6EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddeltaCRLTest9EE.crt | 0 | File InvaliddeltaCRLTest9EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddistributionPointTest2EE.crt | 0 | File InvaliddistributionPointTest2EE.crt has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest3EE.crt | 0 | File InvaliddistributionPointTest3EE.crt has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest6EE.crt | 0 | File InvaliddistributionPointTest6EE.crt has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest8EE.crt | 0 | File InvaliddistributionPointTest8EE.crt has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest9EE.crt | 0 | File InvaliddistributionPointTest9EE.crt has permissions -rw |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest1EE.crt | 0 | File InvalidinhibitAnyPolicyTest1EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest4EE.crt | 0 | File InvalidinhibitAnyPolicyTest4EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest5EE.crt | 0 | File InvalidinhibitAnyPolicyTest5EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest6EE.crt | 0 | File InvalidinhibitAnyPolicyTest6EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest1EE.crt | 0 | File InvalidinhibitPolicyMappingTest1EE.crt has permissions  |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest3EE.crt | 0 | File InvalidinhibitPolicyMappingTest3EE.crt has permissions  |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest5EE.crt | 0 | File InvalidinhibitPolicyMappingTest5EE.crt has permissions  |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest6EE.crt | 0 | File InvalidinhibitPolicyMappingTest6EE.crt has permissions  |
| HIGH | GS002 | InvalidkeyUsageCriticalcRLSignFalseTest4EE.crt | 0 | File InvalidkeyUsageCriticalcRLSignFalseTest4EE.crt has perm |
| HIGH | GS002 | InvalidkeyUsageCriticalkeyCertSignFalseTest1EE.crt | 0 | File InvalidkeyUsageCriticalkeyCertSignFalseTest1EE.crt has  |
| HIGH | GS002 | InvalidkeyUsageNotCriticalcRLSignFalseTest5EE.crt | 0 | File InvalidkeyUsageNotCriticalcRLSignFalseTest5EE.crt has p |
| HIGH | GS002 | InvalidkeyUsageNotCriticalkeyCertSignFalseTest2EE.crt | 0 | File InvalidkeyUsageNotCriticalkeyCertSignFalseTest2EE.crt h |
| HIGH | GS002 | InvalidonlyContainsAttributeCertsTest14EE.crt | 0 | File InvalidonlyContainsAttributeCertsTest14EE.crt has permi |
| HIGH | GS002 | InvalidonlyContainsCACertsTest12EE.crt | 0 | File InvalidonlyContainsCACertsTest12EE.crt has permissions  |
| HIGH | GS002 | InvalidonlyContainsUserCertsTest11EE.crt | 0 | File InvalidonlyContainsUserCertsTest11EE.crt has permission |
| HIGH | GS002 | InvalidonlySomeReasonsTest15EE.crt | 0 | File InvalidonlySomeReasonsTest15EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest16EE.crt | 0 | File InvalidonlySomeReasonsTest16EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest17EE.crt | 0 | File InvalidonlySomeReasonsTest17EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest20EE.crt | 0 | File InvalidonlySomeReasonsTest20EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest21EE.crt | 0 | File InvalidonlySomeReasonsTest21EE.crt has permissions -rw- |
| HIGH | GS002 | InvalidpathLenConstraintTest10EE.crt | 0 | File InvalidpathLenConstraintTest10EE.crt has permissions -r |
| HIGH | GS002 | InvalidpathLenConstraintTest11EE.crt | 0 | File InvalidpathLenConstraintTest11EE.crt has permissions -r |
| HIGH | GS002 | InvalidpathLenConstraintTest12EE.crt | 0 | File InvalidpathLenConstraintTest12EE.crt has permissions -r |
| HIGH | GS002 | InvalidpathLenConstraintTest5EE.crt | 0 | File InvalidpathLenConstraintTest5EE.crt has permissions -rw |
| HIGH | GS002 | InvalidpathLenConstraintTest6EE.crt | 0 | File InvalidpathLenConstraintTest6EE.crt has permissions -rw |
| HIGH | GS002 | InvalidpathLenConstraintTest9EE.crt | 0 | File InvalidpathLenConstraintTest9EE.crt has permissions -rw |
| HIGH | GS002 | Invalidpre2000CRLnextUpdateTest12EE.crt | 0 | File Invalidpre2000CRLnextUpdateTest12EE.crt has permissions |
| HIGH | GS002 | Invalidpre2000UTCEEnotAfterDateTest7EE.crt | 0 | File Invalidpre2000UTCEEnotAfterDateTest7EE.crt has permissi |
| HIGH | GS002 | InvalidrequireExplicitPolicyTest3EE.crt | 0 | File InvalidrequireExplicitPolicyTest3EE.crt has permissions |
| HIGH | GS002 | InvalidrequireExplicitPolicyTest5EE.crt | 0 | File InvalidrequireExplicitPolicyTest5EE.crt has permissions |
| HIGH | GS002 | LongSerialNumberCACert.crt | 0 | File LongSerialNumberCACert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | Mapping1to2CACert.crt | 0 | File Mapping1to2CACert.crt has permissions -rw-rw-r-- — read |
| HIGH | GS002 | MappingFromanyPolicyCACert.crt | 0 | File MappingFromanyPolicyCACert.crt has permissions -rw-rw-r |
| HIGH | GS002 | MappingToanyPolicyCACert.crt | 0 | File MappingToanyPolicyCACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | MissingbasicConstraintsCACert.crt | 0 | File MissingbasicConstraintsCACert.crt has permissions -rw-r |
| HIGH | GS002 | NameOrderingCACert.crt | 0 | File NameOrderingCACert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | NegativeSerialNumberCACert.crt | 0 | File NegativeSerialNumberCACert.crt has permissions -rw-rw-r |
| HIGH | GS002 | NoCRLCACert.crt | 0 | File NoCRLCACert.crt has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | NoPoliciesCACert.crt | 0 | File NoPoliciesCACert.crt has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | NoissuingDistributionPointCACert.crt | 0 | File NoissuingDistributionPointCACert.crt has permissions -r |
| HIGH | GS002 | OldCRLnextUpdateCACert.crt | 0 | File OldCRLnextUpdateCACert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | OverlappingPoliciesTest6EE.crt | 0 | File OverlappingPoliciesTest6EE.crt has permissions -rw-rw-r |
| HIGH | GS002 | P12Mapping1to3CACert.crt | 0 | File P12Mapping1to3CACert.crt has permissions -rw-rw-r-- — r |
| HIGH | GS002 | P12Mapping1to3subCACert.crt | 0 | File P12Mapping1to3subCACert.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | P12Mapping1to3subsubCACert.crt | 0 | File P12Mapping1to3subsubCACert.crt has permissions -rw-rw-r |
| HIGH | GS002 | P1Mapping1to234CACert.crt | 0 | File P1Mapping1to234CACert.crt has permissions -rw-rw-r-- —  |
| HIGH | GS002 | P1Mapping1to234subCACert.crt | 0 | File P1Mapping1to234subCACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | P1anyPolicyMapping1to2CACert.crt | 0 | File P1anyPolicyMapping1to2CACert.crt has permissions -rw-rw |
| HIGH | GS002 | PanyPolicyMapping1to2CACert.crt | 0 | File PanyPolicyMapping1to2CACert.crt has permissions -rw-rw- |
| HIGH | GS002 | PoliciesP1234CACert.crt | 0 | File PoliciesP1234CACert.crt has permissions -rw-rw-r-- — re |
| HIGH | GS002 | PoliciesP1234subCAP123Cert.crt | 0 | File PoliciesP1234subCAP123Cert.crt has permissions -rw-rw-r |
| HIGH | GS002 | PoliciesP1234subsubCAP123P12Cert.crt | 0 | File PoliciesP1234subsubCAP123P12Cert.crt has permissions -r |
| HIGH | GS002 | PoliciesP123CACert.crt | 0 | File PoliciesP123CACert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | PoliciesP123subCAP12Cert.crt | 0 | File PoliciesP123subCAP12Cert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | PoliciesP123subsubCAP12P1Cert.crt | 0 | File PoliciesP123subsubCAP12P1Cert.crt has permissions -rw-r |
| HIGH | GS002 | PoliciesP123subsubCAP12P2Cert.crt | 0 | File PoliciesP123subsubCAP12P2Cert.crt has permissions -rw-r |
| HIGH | GS002 | PoliciesP123subsubsubCAP12P2P1Cert.crt | 0 | File PoliciesP123subsubsubCAP12P2P1Cert.crt has permissions  |
| HIGH | GS002 | PoliciesP12CACert.crt | 0 | File PoliciesP12CACert.crt has permissions -rw-rw-r-- — read |
| HIGH | GS002 | PoliciesP12subCAP1Cert.crt | 0 | File PoliciesP12subCAP1Cert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | PoliciesP12subsubCAP1P2Cert.crt | 0 | File PoliciesP12subsubCAP1P2Cert.crt has permissions -rw-rw- |
| HIGH | GS002 | PoliciesP2subCA2Cert.crt | 0 | File PoliciesP2subCA2Cert.crt has permissions -rw-rw-r-- — r |
| HIGH | GS002 | PoliciesP2subCACert.crt | 0 | File PoliciesP2subCACert.crt has permissions -rw-rw-r-- — re |
| HIGH | GS002 | PoliciesP3CACert.crt | 0 | File PoliciesP3CACert.crt has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | RFC3280MandatoryAttributeTypesCACert.crt | 0 | File RFC3280MandatoryAttributeTypesCACert.crt has permission |
| HIGH | GS002 | RFC3280OptionalAttributeTypesCACert.crt | 0 | File RFC3280OptionalAttributeTypesCACert.crt has permissions |
| HIGH | GS002 | RevokedsubCACert.crt | 0 | File RevokedsubCACert.crt has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | RolloverfromPrintableStringtoUTF8StringCACert.crt | 0 | File RolloverfromPrintableStringtoUTF8StringCACert.crt has p |
| HIGH | GS002 | SeparateCertificateandCRLKeysCA2CRLSigningCert.crt | 0 | File SeparateCertificateandCRLKeysCA2CRLSigningCert.crt has  |
| HIGH | GS002 | SeparateCertificateandCRLKeysCA2CertificateSigningCACert.crt | 0 | File SeparateCertificateandCRLKeysCA2CertificateSigningCACer |
| HIGH | GS002 | SeparateCertificateandCRLKeysCRLSigningCert.crt | 0 | File SeparateCertificateandCRLKeysCRLSigningCert.crt has per |
| HIGH | GS002 | SeparateCertificateandCRLKeysCertificateSigningCACert.crt | 0 | File SeparateCertificateandCRLKeysCertificateSigningCACert.c |
| HIGH | GS002 | TrustAnchorRootCertificate.crt | 0 | File TrustAnchorRootCertificate.crt has permissions -rw-rw-r |
| HIGH | GS002 | TwoCRLsCACert.crt | 0 | File TwoCRLsCACert.crt has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | UIDCACert.crt | 0 | File UIDCACert.crt has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | UTF8StringCaseInsensitiveMatchCACert.crt | 0 | File UTF8StringCaseInsensitiveMatchCACert.crt has permission |
| HIGH | GS002 | UTF8StringEncodedNamesCACert.crt | 0 | File UTF8StringEncodedNamesCACert.crt has permissions -rw-rw |
| HIGH | GS002 | UnknownCRLEntryExtensionCACert.crt | 0 | File UnknownCRLEntryExtensionCACert.crt has permissions -rw- |
| HIGH | GS002 | UnknownCRLExtensionCACert.crt | 0 | File UnknownCRLExtensionCACert.crt has permissions -rw-rw-r- |
| HIGH | GS002 | UserNoticeQualifierTest15EE.crt | 0 | File UserNoticeQualifierTest15EE.crt has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest16EE.crt | 0 | File UserNoticeQualifierTest16EE.crt has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest17EE.crt | 0 | File UserNoticeQualifierTest17EE.crt has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest18EE.crt | 0 | File UserNoticeQualifierTest18EE.crt has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest19EE.crt | 0 | File UserNoticeQualifierTest19EE.crt has permissions -rw-rw- |
| HIGH | GS002 | ValidBasicSelfIssuedCRLSigningKeyTest6EE.crt | 0 | File ValidBasicSelfIssuedCRLSigningKeyTest6EE.crt has permis |
| HIGH | GS002 | ValidBasicSelfIssuedNewWithOldTest3EE.crt | 0 | File ValidBasicSelfIssuedNewWithOldTest3EE.crt has permissio |
| HIGH | GS002 | ValidBasicSelfIssuedNewWithOldTest4EE.crt | 0 | File ValidBasicSelfIssuedNewWithOldTest4EE.crt has permissio |
| HIGH | GS002 | ValidBasicSelfIssuedOldWithNewTest1EE.crt | 0 | File ValidBasicSelfIssuedOldWithNewTest1EE.crt has permissio |
| HIGH | GS002 | ValidCertificatePathTest1EE.crt | 0 | File ValidCertificatePathTest1EE.crt has permissions -rw-rw- |
| HIGH | GS002 | ValidDNSnameConstraintsTest30EE.crt | 0 | File ValidDNSnameConstraintsTest30EE.crt has permissions -rw |
| HIGH | GS002 | ValidDNSnameConstraintsTest32EE.crt | 0 | File ValidDNSnameConstraintsTest32EE.crt has permissions -rw |
| HIGH | GS002 | ValidDNandRFC822nameConstraintsTest27EE.crt | 0 | File ValidDNandRFC822nameConstraintsTest27EE.crt has permiss |
| HIGH | GS002 | ValidDNnameConstraintsTest11EE.crt | 0 | File ValidDNnameConstraintsTest11EE.crt has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest14EE.crt | 0 | File ValidDNnameConstraintsTest14EE.crt has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest18EE.crt | 0 | File ValidDNnameConstraintsTest18EE.crt has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest19EE.crt | 0 | File ValidDNnameConstraintsTest19EE.crt has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest1EE.crt | 0 | File ValidDNnameConstraintsTest1EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidDNnameConstraintsTest4EE.crt | 0 | File ValidDNnameConstraintsTest4EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidDNnameConstraintsTest5EE.crt | 0 | File ValidDNnameConstraintsTest5EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidDNnameConstraintsTest6EE.crt | 0 | File ValidDNnameConstraintsTest6EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidDSAParameterInheritanceTest5EE.crt | 0 | File ValidDSAParameterInheritanceTest5EE.crt has permissions |
| HIGH | GS002 | ValidDSASignaturesTest4EE.crt | 0 | File ValidDSASignaturesTest4EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | ValidGeneralizedTimeCRLnextUpdateTest13EE.crt | 0 | File ValidGeneralizedTimeCRLnextUpdateTest13EE.crt has permi |
| HIGH | GS002 | ValidGeneralizedTimenotAfterDateTest8EE.crt | 0 | File ValidGeneralizedTimenotAfterDateTest8EE.crt has permiss |
| HIGH | GS002 | ValidGeneralizedTimenotBeforeDateTest4EE.crt | 0 | File ValidGeneralizedTimenotBeforeDateTest4EE.crt has permis |
| HIGH | GS002 | ValidIDPwithindirectCRLTest22EE.crt | 0 | File ValidIDPwithindirectCRLTest22EE.crt has permissions -rw |
| HIGH | GS002 | ValidIDPwithindirectCRLTest24EE.crt | 0 | File ValidIDPwithindirectCRLTest24EE.crt has permissions -rw |
| HIGH | GS002 | ValidIDPwithindirectCRLTest25EE.crt | 0 | File ValidIDPwithindirectCRLTest25EE.crt has permissions -rw |
| HIGH | GS002 | ValidLongSerialNumberTest16EE.crt | 0 | File ValidLongSerialNumberTest16EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidLongSerialNumberTest17EE.crt | 0 | File ValidLongSerialNumberTest17EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidNameChainingCapitalizationTest5EE.crt | 0 | File ValidNameChainingCapitalizationTest5EE.crt has permissi |
| HIGH | GS002 | ValidNameChainingWhitespaceTest3EE.crt | 0 | File ValidNameChainingWhitespaceTest3EE.crt has permissions  |
| HIGH | GS002 | ValidNameChainingWhitespaceTest4EE.crt | 0 | File ValidNameChainingWhitespaceTest4EE.crt has permissions  |
| HIGH | GS002 | ValidNameUIDsTest6EE.crt | 0 | File ValidNameUIDsTest6EE.crt has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValidNegativeSerialNumberTest14EE.crt | 0 | File ValidNegativeSerialNumberTest14EE.crt has permissions - |
| HIGH | GS002 | ValidNoissuingDistributionPointTest10EE.crt | 0 | File ValidNoissuingDistributionPointTest10EE.crt has permiss |
| HIGH | GS002 | ValidPolicyMappingTest11EE.crt | 0 | File ValidPolicyMappingTest11EE.crt has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest12EE.crt | 0 | File ValidPolicyMappingTest12EE.crt has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest13EE.crt | 0 | File ValidPolicyMappingTest13EE.crt has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest14EE.crt | 0 | File ValidPolicyMappingTest14EE.crt has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest1EE.crt | 0 | File ValidPolicyMappingTest1EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest3EE.crt | 0 | File ValidPolicyMappingTest3EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest5EE.crt | 0 | File ValidPolicyMappingTest5EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest6EE.crt | 0 | File ValidPolicyMappingTest6EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest9EE.crt | 0 | File ValidPolicyMappingTest9EE.crt has permissions -rw-rw-r- |
| HIGH | GS002 | ValidRFC3280MandatoryAttributeTypesTest7EE.crt | 0 | File ValidRFC3280MandatoryAttributeTypesTest7EE.crt has perm |
| HIGH | GS002 | ValidRFC3280OptionalAttributeTypesTest8EE.crt | 0 | File ValidRFC3280OptionalAttributeTypesTest8EE.crt has permi |
| HIGH | GS002 | ValidRFC822nameConstraintsTest21EE.crt | 0 | File ValidRFC822nameConstraintsTest21EE.crt has permissions  |
| HIGH | GS002 | ValidRFC822nameConstraintsTest23EE.crt | 0 | File ValidRFC822nameConstraintsTest23EE.crt has permissions  |
| HIGH | GS002 | ValidRFC822nameConstraintsTest25EE.crt | 0 | File ValidRFC822nameConstraintsTest25EE.crt has permissions  |
| HIGH | GS002 | ValidRolloverfromPrintableStringtoUTF8StringTest10EE.crt | 0 | File ValidRolloverfromPrintableStringtoUTF8StringTest10EE.cr |
| HIGH | GS002 | ValidSelfIssuedinhibitAnyPolicyTest7EE.crt | 0 | File ValidSelfIssuedinhibitAnyPolicyTest7EE.crt has permissi |
| HIGH | GS002 | ValidSelfIssuedinhibitAnyPolicyTest9EE.crt | 0 | File ValidSelfIssuedinhibitAnyPolicyTest9EE.crt has permissi |
| HIGH | GS002 | ValidSelfIssuedinhibitPolicyMappingTest7EE.crt | 0 | File ValidSelfIssuedinhibitPolicyMappingTest7EE.crt has perm |
| HIGH | GS002 | ValidSelfIssuedpathLenConstraintTest15EE.crt | 0 | File ValidSelfIssuedpathLenConstraintTest15EE.crt has permis |
| HIGH | GS002 | ValidSelfIssuedpathLenConstraintTest17EE.crt | 0 | File ValidSelfIssuedpathLenConstraintTest17EE.crt has permis |
| HIGH | GS002 | ValidSelfIssuedrequireExplicitPolicyTest6EE.crt | 0 | File ValidSelfIssuedrequireExplicitPolicyTest6EE.crt has per |
| HIGH | GS002 | ValidSeparateCertificateandCRLKeysTest19EE.crt | 0 | File ValidSeparateCertificateandCRLKeysTest19EE.crt has perm |
| HIGH | GS002 | ValidTwoCRLsTest7EE.crt | 0 | File ValidTwoCRLsTest7EE.crt has permissions -rw-rw-r-- — re |
| HIGH | GS002 | ValidURInameConstraintsTest34EE.crt | 0 | File ValidURInameConstraintsTest34EE.crt has permissions -rw |
| HIGH | GS002 | ValidURInameConstraintsTest36EE.crt | 0 | File ValidURInameConstraintsTest36EE.crt has permissions -rw |
| HIGH | GS002 | ValidUTF8StringCaseInsensitiveMatchTest11EE.crt | 0 | File ValidUTF8StringCaseInsensitiveMatchTest11EE.crt has per |
| HIGH | GS002 | ValidUTF8StringEncodedNamesTest9EE.crt | 0 | File ValidUTF8StringEncodedNamesTest9EE.crt has permissions  |
| HIGH | GS002 | ValidUnknownNotCriticalCertificateExtensionTest1EE.crt | 0 | File ValidUnknownNotCriticalCertificateExtensionTest1EE.crt  |
| HIGH | GS002 | ValidbasicConstraintsNotCriticalTest4EE.crt | 0 | File ValidbasicConstraintsNotCriticalTest4EE.crt has permiss |
| HIGH | GS002 | ValidcRLIssuerTest28EE.crt | 0 | File ValidcRLIssuerTest28EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValidcRLIssuerTest29EE.crt | 0 | File ValidcRLIssuerTest29EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValidcRLIssuerTest30EE.crt | 0 | File ValidcRLIssuerTest30EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValidcRLIssuerTest33EE.crt | 0 | File ValidcRLIssuerTest33EE.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValiddeltaCRLTest2EE.crt | 0 | File ValiddeltaCRLTest2EE.crt has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddeltaCRLTest5EE.crt | 0 | File ValiddeltaCRLTest5EE.crt has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddeltaCRLTest7EE.crt | 0 | File ValiddeltaCRLTest7EE.crt has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddeltaCRLTest8EE.crt | 0 | File ValiddeltaCRLTest8EE.crt has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddistributionPointTest1EE.crt | 0 | File ValiddistributionPointTest1EE.crt has permissions -rw-r |
| HIGH | GS002 | ValiddistributionPointTest4EE.crt | 0 | File ValiddistributionPointTest4EE.crt has permissions -rw-r |
| HIGH | GS002 | ValiddistributionPointTest5EE.crt | 0 | File ValiddistributionPointTest5EE.crt has permissions -rw-r |
| HIGH | GS002 | ValiddistributionPointTest7EE.crt | 0 | File ValiddistributionPointTest7EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidinhibitAnyPolicyTest2EE.crt | 0 | File ValidinhibitAnyPolicyTest2EE.crt has permissions -rw-rw |
| HIGH | GS002 | ValidinhibitPolicyMappingTest2EE.crt | 0 | File ValidinhibitPolicyMappingTest2EE.crt has permissions -r |
| HIGH | GS002 | ValidinhibitPolicyMappingTest4EE.crt | 0 | File ValidinhibitPolicyMappingTest4EE.crt has permissions -r |
| HIGH | GS002 | ValidkeyUsageNotCriticalTest3EE.crt | 0 | File ValidkeyUsageNotCriticalTest3EE.crt has permissions -rw |
| HIGH | GS002 | ValidonlyContainsCACertsTest13EE.crt | 0 | File ValidonlyContainsCACertsTest13EE.crt has permissions -r |
| HIGH | GS002 | ValidonlySomeReasonsTest18EE.crt | 0 | File ValidonlySomeReasonsTest18EE.crt has permissions -rw-rw |
| HIGH | GS002 | ValidonlySomeReasonsTest19EE.crt | 0 | File ValidonlySomeReasonsTest19EE.crt has permissions -rw-rw |
| HIGH | GS002 | ValidpathLenConstraintTest13EE.crt | 0 | File ValidpathLenConstraintTest13EE.crt has permissions -rw- |
| HIGH | GS002 | ValidpathLenConstraintTest14EE.crt | 0 | File ValidpathLenConstraintTest14EE.crt has permissions -rw- |
| HIGH | GS002 | ValidpathLenConstraintTest7EE.crt | 0 | File ValidpathLenConstraintTest7EE.crt has permissions -rw-r |
| HIGH | GS002 | ValidpathLenConstraintTest8EE.crt | 0 | File ValidpathLenConstraintTest8EE.crt has permissions -rw-r |
| HIGH | GS002 | Validpre2000UTCnotBeforeDateTest3EE.crt | 0 | File Validpre2000UTCnotBeforeDateTest3EE.crt has permissions |
| HIGH | GS002 | ValidrequireExplicitPolicyTest1EE.crt | 0 | File ValidrequireExplicitPolicyTest1EE.crt has permissions - |
| HIGH | GS002 | ValidrequireExplicitPolicyTest2EE.crt | 0 | File ValidrequireExplicitPolicyTest2EE.crt has permissions - |
| HIGH | GS002 | ValidrequireExplicitPolicyTest4EE.crt | 0 | File ValidrequireExplicitPolicyTest4EE.crt has permissions - |
| HIGH | GS002 | WrongCRLCACert.crt | 0 | File WrongCRLCACert.crt has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | anyPolicyCACert.crt | 0 | File anyPolicyCACert.crt has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | basicConstraintsCriticalcAFalseCACert.crt | 0 | File basicConstraintsCriticalcAFalseCACert.crt has permissio |
| HIGH | GS002 | basicConstraintsNotCriticalCACert.crt | 0 | File basicConstraintsNotCriticalCACert.crt has permissions - |
| HIGH | GS002 | basicConstraintsNotCriticalcAFalseCACert.crt | 0 | File basicConstraintsNotCriticalcAFalseCACert.crt has permis |
| HIGH | GS002 | deltaCRLCA1Cert.crt | 0 | File deltaCRLCA1Cert.crt has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | deltaCRLCA2Cert.crt | 0 | File deltaCRLCA2Cert.crt has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | deltaCRLCA3Cert.crt | 0 | File deltaCRLCA3Cert.crt has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | deltaCRLIndicatorNoBaseCACert.crt | 0 | File deltaCRLIndicatorNoBaseCACert.crt has permissions -rw-r |
| HIGH | GS002 | distributionPoint1CACert.crt | 0 | File distributionPoint1CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | distributionPoint2CACert.crt | 0 | File distributionPoint2CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | indirectCRLCA1Cert.crt | 0 | File indirectCRLCA1Cert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA2Cert.crt | 0 | File indirectCRLCA2Cert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA3Cert.crt | 0 | File indirectCRLCA3Cert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA3cRLIssuerCert.crt | 0 | File indirectCRLCA3cRLIssuerCert.crt has permissions -rw-rw- |
| HIGH | GS002 | indirectCRLCA4Cert.crt | 0 | File indirectCRLCA4Cert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA4cRLIssuerCert.crt | 0 | File indirectCRLCA4cRLIssuerCert.crt has permissions -rw-rw- |
| HIGH | GS002 | indirectCRLCA5Cert.crt | 0 | File indirectCRLCA5Cert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA6Cert.crt | 0 | File indirectCRLCA6Cert.crt has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | inhibitAnyPolicy0CACert.crt | 0 | File inhibitAnyPolicy0CACert.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitAnyPolicy1CACert.crt | 0 | File inhibitAnyPolicy1CACert.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitAnyPolicy1SelfIssuedCACert.crt | 0 | File inhibitAnyPolicy1SelfIssuedCACert.crt has permissions - |
| HIGH | GS002 | inhibitAnyPolicy1SelfIssuedsubCA2Cert.crt | 0 | File inhibitAnyPolicy1SelfIssuedsubCA2Cert.crt has permissio |
| HIGH | GS002 | inhibitAnyPolicy1subCA1Cert.crt | 0 | File inhibitAnyPolicy1subCA1Cert.crt has permissions -rw-rw- |
| HIGH | GS002 | inhibitAnyPolicy1subCA2Cert.crt | 0 | File inhibitAnyPolicy1subCA2Cert.crt has permissions -rw-rw- |
| HIGH | GS002 | inhibitAnyPolicy1subCAIAP5Cert.crt | 0 | File inhibitAnyPolicy1subCAIAP5Cert.crt has permissions -rw- |
| HIGH | GS002 | inhibitAnyPolicy1subsubCA2Cert.crt | 0 | File inhibitAnyPolicy1subsubCA2Cert.crt has permissions -rw- |
| HIGH | GS002 | inhibitAnyPolicy5CACert.crt | 0 | File inhibitAnyPolicy5CACert.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitAnyPolicy5subCACert.crt | 0 | File inhibitAnyPolicy5subCACert.crt has permissions -rw-rw-r |
| HIGH | GS002 | inhibitAnyPolicy5subsubCACert.crt | 0 | File inhibitAnyPolicy5subsubCACert.crt has permissions -rw-r |
| HIGH | GS002 | inhibitAnyPolicyTest3EE.crt | 0 | File inhibitAnyPolicyTest3EE.crt has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitPolicyMapping0CACert.crt | 0 | File inhibitPolicyMapping0CACert.crt has permissions -rw-rw- |
| HIGH | GS002 | inhibitPolicyMapping0subCACert.crt | 0 | File inhibitPolicyMapping0subCACert.crt has permissions -rw- |
| HIGH | GS002 | inhibitPolicyMapping1P12CACert.crt | 0 | File inhibitPolicyMapping1P12CACert.crt has permissions -rw- |
| HIGH | GS002 | inhibitPolicyMapping1P12subCACert.crt | 0 | File inhibitPolicyMapping1P12subCACert.crt has permissions - |
| HIGH | GS002 | inhibitPolicyMapping1P12subCAIPM5Cert.crt | 0 | File inhibitPolicyMapping1P12subCAIPM5Cert.crt has permissio |
| HIGH | GS002 | inhibitPolicyMapping1P12subsubCACert.crt | 0 | File inhibitPolicyMapping1P12subsubCACert.crt has permission |
| HIGH | GS002 | inhibitPolicyMapping1P12subsubCAIPM5Cert.crt | 0 | File inhibitPolicyMapping1P12subsubCAIPM5Cert.crt has permis |
| HIGH | GS002 | inhibitPolicyMapping1P1CACert.crt | 0 | File inhibitPolicyMapping1P1CACert.crt has permissions -rw-r |
| HIGH | GS002 | inhibitPolicyMapping1P1SelfIssuedCACert.crt | 0 | File inhibitPolicyMapping1P1SelfIssuedCACert.crt has permiss |
| HIGH | GS002 | inhibitPolicyMapping1P1SelfIssuedsubCACert.crt | 0 | File inhibitPolicyMapping1P1SelfIssuedsubCACert.crt has perm |
| HIGH | GS002 | inhibitPolicyMapping1P1subCACert.crt | 0 | File inhibitPolicyMapping1P1subCACert.crt has permissions -r |
| HIGH | GS002 | inhibitPolicyMapping1P1subsubCACert.crt | 0 | File inhibitPolicyMapping1P1subsubCACert.crt has permissions |
| HIGH | GS002 | inhibitPolicyMapping5CACert.crt | 0 | File inhibitPolicyMapping5CACert.crt has permissions -rw-rw- |
| HIGH | GS002 | inhibitPolicyMapping5subCACert.crt | 0 | File inhibitPolicyMapping5subCACert.crt has permissions -rw- |
| HIGH | GS002 | inhibitPolicyMapping5subsubCACert.crt | 0 | File inhibitPolicyMapping5subsubCACert.crt has permissions - |
| HIGH | GS002 | inhibitPolicyMapping5subsubsubCACert.crt | 0 | File inhibitPolicyMapping5subsubsubCACert.crt has permission |
| HIGH | GS002 | keyUsageCriticalcRLSignFalseCACert.crt | 0 | File keyUsageCriticalcRLSignFalseCACert.crt has permissions  |
| HIGH | GS002 | keyUsageCriticalkeyCertSignFalseCACert.crt | 0 | File keyUsageCriticalkeyCertSignFalseCACert.crt has permissi |
| HIGH | GS002 | keyUsageNotCriticalCACert.crt | 0 | File keyUsageNotCriticalCACert.crt has permissions -rw-rw-r- |
| HIGH | GS002 | keyUsageNotCriticalcRLSignFalseCACert.crt | 0 | File keyUsageNotCriticalcRLSignFalseCACert.crt has permissio |
| HIGH | GS002 | keyUsageNotCriticalkeyCertSignFalseCACert.crt | 0 | File keyUsageNotCriticalkeyCertSignFalseCACert.crt has permi |
| HIGH | GS002 | nameConstraintsDN1CACert.crt | 0 | File nameConstraintsDN1CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN1SelfIssuedCACert.crt | 0 | File nameConstraintsDN1SelfIssuedCACert.crt has permissions  |
| HIGH | GS002 | nameConstraintsDN1subCA1Cert.crt | 0 | File nameConstraintsDN1subCA1Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN1subCA2Cert.crt | 0 | File nameConstraintsDN1subCA2Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN1subCA3Cert.crt | 0 | File nameConstraintsDN1subCA3Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN2CACert.crt | 0 | File nameConstraintsDN2CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN3CACert.crt | 0 | File nameConstraintsDN3CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN3subCA1Cert.crt | 0 | File nameConstraintsDN3subCA1Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN3subCA2Cert.crt | 0 | File nameConstraintsDN3subCA2Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN4CACert.crt | 0 | File nameConstraintsDN4CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN5CACert.crt | 0 | File nameConstraintsDN5CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDNS1CACert.crt | 0 | File nameConstraintsDNS1CACert.crt has permissions -rw-rw-r- |
| HIGH | GS002 | nameConstraintsDNS2CACert.crt | 0 | File nameConstraintsDNS2CACert.crt has permissions -rw-rw-r- |
| HIGH | GS002 | nameConstraintsRFC822CA1Cert.crt | 0 | File nameConstraintsRFC822CA1Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsRFC822CA2Cert.crt | 0 | File nameConstraintsRFC822CA2Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsRFC822CA3Cert.crt | 0 | File nameConstraintsRFC822CA3Cert.crt has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsURI1CACert.crt | 0 | File nameConstraintsURI1CACert.crt has permissions -rw-rw-r- |
| HIGH | GS002 | nameConstraintsURI2CACert.crt | 0 | File nameConstraintsURI2CACert.crt has permissions -rw-rw-r- |
| HIGH | GS002 | onlyContainsAttributeCertsCACert.crt | 0 | File onlyContainsAttributeCertsCACert.crt has permissions -r |
| HIGH | GS002 | onlyContainsCACertsCACert.crt | 0 | File onlyContainsCACertsCACert.crt has permissions -rw-rw-r- |
| HIGH | GS002 | onlyContainsUserCertsCACert.crt | 0 | File onlyContainsUserCertsCACert.crt has permissions -rw-rw- |
| HIGH | GS002 | onlySomeReasonsCA1Cert.crt | 0 | File onlySomeReasonsCA1Cert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | onlySomeReasonsCA2Cert.crt | 0 | File onlySomeReasonsCA2Cert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | onlySomeReasonsCA3Cert.crt | 0 | File onlySomeReasonsCA3Cert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | onlySomeReasonsCA4Cert.crt | 0 | File onlySomeReasonsCA4Cert.crt has permissions -rw-rw-r-- — |
| HIGH | GS002 | pathLenConstraint0CACert.crt | 0 | File pathLenConstraint0CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | pathLenConstraint0SelfIssuedCACert.crt | 0 | File pathLenConstraint0SelfIssuedCACert.crt has permissions  |
| HIGH | GS002 | pathLenConstraint0subCA2Cert.crt | 0 | File pathLenConstraint0subCA2Cert.crt has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint0subCACert.crt | 0 | File pathLenConstraint0subCACert.crt has permissions -rw-rw- |
| HIGH | GS002 | pathLenConstraint1CACert.crt | 0 | File pathLenConstraint1CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | pathLenConstraint1SelfIssuedCACert.crt | 0 | File pathLenConstraint1SelfIssuedCACert.crt has permissions  |
| HIGH | GS002 | pathLenConstraint1SelfIssuedsubCACert.crt | 0 | File pathLenConstraint1SelfIssuedsubCACert.crt has permissio |
| HIGH | GS002 | pathLenConstraint1subCACert.crt | 0 | File pathLenConstraint1subCACert.crt has permissions -rw-rw- |
| HIGH | GS002 | pathLenConstraint6CACert.crt | 0 | File pathLenConstraint6CACert.crt has permissions -rw-rw-r-- |
| HIGH | GS002 | pathLenConstraint6subCA0Cert.crt | 0 | File pathLenConstraint6subCA0Cert.crt has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint6subCA1Cert.crt | 0 | File pathLenConstraint6subCA1Cert.crt has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint6subCA4Cert.crt | 0 | File pathLenConstraint6subCA4Cert.crt has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint6subsubCA00Cert.crt | 0 | File pathLenConstraint6subsubCA00Cert.crt has permissions -r |
| HIGH | GS002 | pathLenConstraint6subsubCA11Cert.crt | 0 | File pathLenConstraint6subsubCA11Cert.crt has permissions -r |
| HIGH | GS002 | pathLenConstraint6subsubCA41Cert.crt | 0 | File pathLenConstraint6subsubCA41Cert.crt has permissions -r |
| HIGH | GS002 | pathLenConstraint6subsubsubCA11XCert.crt | 0 | File pathLenConstraint6subsubsubCA11XCert.crt has permission |
| HIGH | GS002 | pathLenConstraint6subsubsubCA41XCert.crt | 0 | File pathLenConstraint6subsubsubCA41XCert.crt has permission |
| HIGH | GS002 | pre2000CRLnextUpdateCACert.crt | 0 | File pre2000CRLnextUpdateCACert.crt has permissions -rw-rw-r |
| HIGH | GS002 | requireExplicitPolicy0CACert.crt | 0 | File requireExplicitPolicy0CACert.crt has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy0subCACert.crt | 0 | File requireExplicitPolicy0subCACert.crt has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy0subsubCACert.crt | 0 | File requireExplicitPolicy0subsubCACert.crt has permissions  |
| HIGH | GS002 | requireExplicitPolicy0subsubsubCACert.crt | 0 | File requireExplicitPolicy0subsubsubCACert.crt has permissio |
| HIGH | GS002 | requireExplicitPolicy10CACert.crt | 0 | File requireExplicitPolicy10CACert.crt has permissions -rw-r |
| HIGH | GS002 | requireExplicitPolicy10subCACert.crt | 0 | File requireExplicitPolicy10subCACert.crt has permissions -r |
| HIGH | GS002 | requireExplicitPolicy10subsubCACert.crt | 0 | File requireExplicitPolicy10subsubCACert.crt has permissions |
| HIGH | GS002 | requireExplicitPolicy10subsubsubCACert.crt | 0 | File requireExplicitPolicy10subsubsubCACert.crt has permissi |
| HIGH | GS002 | requireExplicitPolicy2CACert.crt | 0 | File requireExplicitPolicy2CACert.crt has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy2SelfIssuedCACert.crt | 0 | File requireExplicitPolicy2SelfIssuedCACert.crt has permissi |
| HIGH | GS002 | requireExplicitPolicy2SelfIssuedsubCACert.crt | 0 | File requireExplicitPolicy2SelfIssuedsubCACert.crt has permi |
| HIGH | GS002 | requireExplicitPolicy2subCACert.crt | 0 | File requireExplicitPolicy2subCACert.crt has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy4CACert.crt | 0 | File requireExplicitPolicy4CACert.crt has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy4subCACert.crt | 0 | File requireExplicitPolicy4subCACert.crt has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy4subsubCACert.crt | 0 | File requireExplicitPolicy4subsubCACert.crt has permissions  |
| HIGH | GS002 | requireExplicitPolicy4subsubsubCACert.crt | 0 | File requireExplicitPolicy4subsubsubCACert.crt has permissio |
| HIGH | GS002 | requireExplicitPolicy5CACert.crt | 0 | File requireExplicitPolicy5CACert.crt has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy5subCACert.crt | 0 | File requireExplicitPolicy5subCACert.crt has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy5subsubCACert.crt | 0 | File requireExplicitPolicy5subsubCACert.crt has permissions  |
| HIGH | GS002 | requireExplicitPolicy5subsubsubCACert.crt | 0 | File requireExplicitPolicy5subsubsubCACert.crt has permissio |
| HIGH | GS002 | requireExplicitPolicy7CACert.crt | 0 | File requireExplicitPolicy7CACert.crt has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy7subCARE2Cert.crt | 0 | File requireExplicitPolicy7subCARE2Cert.crt has permissions  |
| HIGH | GS002 | requireExplicitPolicy7subsubCARE2RE4Cert.crt | 0 | File requireExplicitPolicy7subsubCARE2RE4Cert.crt has permis |
| HIGH | GS002 | requireExplicitPolicy7subsubsubCARE2RE4Cert.crt | 0 | File requireExplicitPolicy7subsubsubCARE2RE4Cert.crt has per |
| HIGH | GS002 | AllCertificatesNoPoliciesTest2EE.p12 | 0 | File AllCertificatesNoPoliciesTest2EE.p12 has permissions -r |
| HIGH | GS002 | AllCertificatesSamePoliciesTest10EE.p12 | 0 | File AllCertificatesSamePoliciesTest10EE.p12 has permissions |
| HIGH | GS002 | AllCertificatesSamePoliciesTest13EE.p12 | 0 | File AllCertificatesSamePoliciesTest13EE.p12 has permissions |
| HIGH | GS002 | AllCertificatesanyPolicyTest11EE.p12 | 0 | File AllCertificatesanyPolicyTest11EE.p12 has permissions -r |
| HIGH | GS002 | AnyPolicyTest14EE.p12 | 0 | File AnyPolicyTest14EE.p12 has permissions -rw-rw-r-- — read |
| HIGH | GS002 | BadCRLIssuerNameCACert.p12 | 0 | File BadCRLIssuerNameCACert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | BadCRLSignatureCACert.p12 | 0 | File BadCRLSignatureCACert.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | BadSignedCACert.p12 | 0 | File BadSignedCACert.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | BadnotAfterDateCACert.p12 | 0 | File BadnotAfterDateCACert.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | BadnotBeforeDateCACert.p12 | 0 | File BadnotBeforeDateCACert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | BasicSelfIssuedCRLSigningKeyCACert.p12 | 0 | File BasicSelfIssuedCRLSigningKeyCACert.p12 has permissions  |
| HIGH | GS002 | BasicSelfIssuedCRLSigningKeyCRLCert.p12 | 0 | File BasicSelfIssuedCRLSigningKeyCRLCert.p12 has permissions |
| HIGH | GS002 | BasicSelfIssuedNewKeyCACert.p12 | 0 | File BasicSelfIssuedNewKeyCACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | BasicSelfIssuedNewKeyOldWithNewCACert.p12 | 0 | File BasicSelfIssuedNewKeyOldWithNewCACert.p12 has permissio |
| HIGH | GS002 | BasicSelfIssuedOldKeyCACert.p12 | 0 | File BasicSelfIssuedOldKeyCACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | BasicSelfIssuedOldKeyNewWithOldCACert.p12 | 0 | File BasicSelfIssuedOldKeyNewWithOldCACert.p12 has permissio |
| HIGH | GS002 | CPSPointerQualifierTest20EE.p12 | 0 | File CPSPointerQualifierTest20EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | DSACACert.p12 | 0 | File DSACACert.p12 has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | DSAParametersInheritedCACert.p12 | 0 | File DSAParametersInheritedCACert.p12 has permissions -rw-rw |
| HIGH | GS002 | DifferentPoliciesTest12EE.p12 | 0 | File DifferentPoliciesTest12EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | DifferentPoliciesTest3EE.p12 | 0 | File DifferentPoliciesTest3EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest4EE.p12 | 0 | File DifferentPoliciesTest4EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest5EE.p12 | 0 | File DifferentPoliciesTest5EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest7EE.p12 | 0 | File DifferentPoliciesTest7EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest8EE.p12 | 0 | File DifferentPoliciesTest8EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | DifferentPoliciesTest9EE.p12 | 0 | File DifferentPoliciesTest9EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | GeneralizedTimeCRLnextUpdateCACert.p12 | 0 | File GeneralizedTimeCRLnextUpdateCACert.p12 has permissions  |
| HIGH | GS002 | GoodCACert.p12 | 0 | File GoodCACert.p12 has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | GoodsubCACert.p12 | 0 | File GoodsubCACert.p12 has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | GoodsubCAPanyPolicyMapping1to2CACert.p12 | 0 | File GoodsubCAPanyPolicyMapping1to2CACert.p12 has permission |
| HIGH | GS002 | InvalidBadCRLIssuerNameTest5EE.p12 | 0 | File InvalidBadCRLIssuerNameTest5EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidBadCRLSignatureTest4EE.p12 | 0 | File InvalidBadCRLSignatureTest4EE.p12 has permissions -rw-r |
| HIGH | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest7EE.p12 | 0 | File InvalidBasicSelfIssuedCRLSigningKeyTest7EE.p12 has perm |
| HIGH | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest8EE.p12 | 0 | File InvalidBasicSelfIssuedCRLSigningKeyTest8EE.p12 has perm |
| HIGH | GS002 | InvalidBasicSelfIssuedNewWithOldTest5EE.p12 | 0 | File InvalidBasicSelfIssuedNewWithOldTest5EE.p12 has permiss |
| HIGH | GS002 | InvalidBasicSelfIssuedOldWithNewTest2EE.p12 | 0 | File InvalidBasicSelfIssuedOldWithNewTest2EE.p12 has permiss |
| HIGH | GS002 | InvalidCASignatureTest2EE.p12 | 0 | File InvalidCASignatureTest2EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | InvalidCAnotAfterDateTest5EE.p12 | 0 | File InvalidCAnotAfterDateTest5EE.p12 has permissions -rw-rw |
| HIGH | GS002 | InvalidCAnotBeforeDateTest1EE.p12 | 0 | File InvalidCAnotBeforeDateTest1EE.p12 has permissions -rw-r |
| HIGH | GS002 | InvalidDNSnameConstraintsTest31EE.p12 | 0 | File InvalidDNSnameConstraintsTest31EE.p12 has permissions - |
| HIGH | GS002 | InvalidDNSnameConstraintsTest33EE.p12 | 0 | File InvalidDNSnameConstraintsTest33EE.p12 has permissions - |
| HIGH | GS002 | InvalidDNSnameConstraintsTest38EE.p12 | 0 | File InvalidDNSnameConstraintsTest38EE.p12 has permissions - |
| HIGH | GS002 | InvalidDNandRFC822nameConstraintsTest28EE.p12 | 0 | File InvalidDNandRFC822nameConstraintsTest28EE.p12 has permi |
| HIGH | GS002 | InvalidDNandRFC822nameConstraintsTest29EE.p12 | 0 | File InvalidDNandRFC822nameConstraintsTest29EE.p12 has permi |
| HIGH | GS002 | InvalidDNnameConstraintsTest10EE.p12 | 0 | File InvalidDNnameConstraintsTest10EE.p12 has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest12EE.p12 | 0 | File InvalidDNnameConstraintsTest12EE.p12 has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest13EE.p12 | 0 | File InvalidDNnameConstraintsTest13EE.p12 has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest15EE.p12 | 0 | File InvalidDNnameConstraintsTest15EE.p12 has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest16EE.p12 | 0 | File InvalidDNnameConstraintsTest16EE.p12 has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest17EE.p12 | 0 | File InvalidDNnameConstraintsTest17EE.p12 has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest20EE.p12 | 0 | File InvalidDNnameConstraintsTest20EE.p12 has permissions -r |
| HIGH | GS002 | InvalidDNnameConstraintsTest2EE.p12 | 0 | File InvalidDNnameConstraintsTest2EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest3EE.p12 | 0 | File InvalidDNnameConstraintsTest3EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest7EE.p12 | 0 | File InvalidDNnameConstraintsTest7EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest8EE.p12 | 0 | File InvalidDNnameConstraintsTest8EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidDNnameConstraintsTest9EE.p12 | 0 | File InvalidDNnameConstraintsTest9EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidDSASignatureTest6EE.p12 | 0 | File InvalidDSASignatureTest6EE.p12 has permissions -rw-rw-r |
| HIGH | GS002 | InvalidEESignatureTest3EE.p12 | 0 | File InvalidEESignatureTest3EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | InvalidEEnotAfterDateTest6EE.p12 | 0 | File InvalidEEnotAfterDateTest6EE.p12 has permissions -rw-rw |
| HIGH | GS002 | InvalidEEnotBeforeDateTest2EE.p12 | 0 | File InvalidEEnotBeforeDateTest2EE.p12 has permissions -rw-r |
| HIGH | GS002 | InvalidIDPwithindirectCRLTest23EE.p12 | 0 | File InvalidIDPwithindirectCRLTest23EE.p12 has permissions - |
| HIGH | GS002 | InvalidIDPwithindirectCRLTest26EE.p12 | 0 | File InvalidIDPwithindirectCRLTest26EE.p12 has permissions - |
| HIGH | GS002 | InvalidLongSerialNumberTest18EE.p12 | 0 | File InvalidLongSerialNumberTest18EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidMappingFromanyPolicyTest7EE.p12 | 0 | File InvalidMappingFromanyPolicyTest7EE.p12 has permissions  |
| HIGH | GS002 | InvalidMappingToanyPolicyTest8EE.p12 | 0 | File InvalidMappingToanyPolicyTest8EE.p12 has permissions -r |
| HIGH | GS002 | InvalidMissingCRLTest1EE.p12 | 0 | File InvalidMissingCRLTest1EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidMissingbasicConstraintsTest1EE.p12 | 0 | File InvalidMissingbasicConstraintsTest1EE.p12 has permissio |
| HIGH | GS002 | InvalidNameChainingOrderTest2EE.p12 | 0 | File InvalidNameChainingOrderTest2EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidNameChainingTest1EE.p12 | 0 | File InvalidNameChainingTest1EE.p12 has permissions -rw-rw-r |
| HIGH | GS002 | InvalidNegativeSerialNumberTest15EE.p12 | 0 | File InvalidNegativeSerialNumberTest15EE.p12 has permissions |
| HIGH | GS002 | InvalidOldCRLnextUpdateTest11EE.p12 | 0 | File InvalidOldCRLnextUpdateTest11EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidPolicyMappingTest10EE.p12 | 0 | File InvalidPolicyMappingTest10EE.p12 has permissions -rw-rw |
| HIGH | GS002 | InvalidPolicyMappingTest2EE.p12 | 0 | File InvalidPolicyMappingTest2EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | InvalidPolicyMappingTest4EE.p12 | 0 | File InvalidPolicyMappingTest4EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | InvalidRFC822nameConstraintsTest22EE.p12 | 0 | File InvalidRFC822nameConstraintsTest22EE.p12 has permission |
| HIGH | GS002 | InvalidRFC822nameConstraintsTest24EE.p12 | 0 | File InvalidRFC822nameConstraintsTest24EE.p12 has permission |
| HIGH | GS002 | InvalidRFC822nameConstraintsTest26EE.p12 | 0 | File InvalidRFC822nameConstraintsTest26EE.p12 has permission |
| HIGH | GS002 | InvalidRevokedCATest2EE.p12 | 0 | File InvalidRevokedCATest2EE.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | InvalidRevokedEETest3EE.p12 | 0 | File InvalidRevokedEETest3EE.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest10EE.p12 | 0 | File InvalidSelfIssuedinhibitAnyPolicyTest10EE.p12 has permi |
| HIGH | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest8EE.p12 | 0 | File InvalidSelfIssuedinhibitAnyPolicyTest8EE.p12 has permis |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest10EE.p12 | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest10EE.p12 has p |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest11EE.p12 | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest11EE.p12 has p |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest8EE.p12 | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest8EE.p12 has pe |
| HIGH | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest9EE.p12 | 0 | File InvalidSelfIssuedinhibitPolicyMappingTest9EE.p12 has pe |
| HIGH | GS002 | InvalidSelfIssuedpathLenConstraintTest16EE.p12 | 0 | File InvalidSelfIssuedpathLenConstraintTest16EE.p12 has perm |
| HIGH | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest7EE.p12 | 0 | File InvalidSelfIssuedrequireExplicitPolicyTest7EE.p12 has p |
| HIGH | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest8EE.p12 | 0 | File InvalidSelfIssuedrequireExplicitPolicyTest8EE.p12 has p |
| HIGH | GS002 | InvalidSeparateCertificateandCRLKeysTest20EE.p12 | 0 | File InvalidSeparateCertificateandCRLKeysTest20EE.p12 has pe |
| HIGH | GS002 | InvalidSeparateCertificateandCRLKeysTest21EE.p12 | 0 | File InvalidSeparateCertificateandCRLKeysTest21EE.p12 has pe |
| HIGH | GS002 | InvalidURInameConstraintsTest35EE.p12 | 0 | File InvalidURInameConstraintsTest35EE.p12 has permissions - |
| HIGH | GS002 | InvalidURInameConstraintsTest37EE.p12 | 0 | File InvalidURInameConstraintsTest37EE.p12 has permissions - |
| HIGH | GS002 | InvalidUnknownCRLEntryExtensionTest8EE.p12 | 0 | File InvalidUnknownCRLEntryExtensionTest8EE.p12 has permissi |
| HIGH | GS002 | InvalidUnknownCRLExtensionTest10EE.p12 | 0 | File InvalidUnknownCRLExtensionTest10EE.p12 has permissions  |
| HIGH | GS002 | InvalidUnknownCRLExtensionTest9EE.p12 | 0 | File InvalidUnknownCRLExtensionTest9EE.p12 has permissions - |
| HIGH | GS002 | InvalidUnknownCriticalCertificateExtensionTest2EE.p12 | 0 | File InvalidUnknownCriticalCertificateExtensionTest2EE.p12 h |
| HIGH | GS002 | InvalidWrongCRLTest6EE.p12 | 0 | File InvalidWrongCRLTest6EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvalidcAFalseTest2EE.p12 | 0 | File InvalidcAFalseTest2EE.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | InvalidcAFalseTest3EE.p12 | 0 | File InvalidcAFalseTest3EE.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | InvalidcRLIssuerTest27EE.p12 | 0 | File InvalidcRLIssuerTest27EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest31EE.p12 | 0 | File InvalidcRLIssuerTest31EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest32EE.p12 | 0 | File InvalidcRLIssuerTest32EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest34EE.p12 | 0 | File InvalidcRLIssuerTest34EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | InvalidcRLIssuerTest35EE.p12 | 0 | File InvalidcRLIssuerTest35EE.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | InvaliddeltaCRLIndicatorNoBaseTest1EE.p12 | 0 | File InvaliddeltaCRLIndicatorNoBaseTest1EE.p12 has permissio |
| HIGH | GS002 | InvaliddeltaCRLTest10EE.p12 | 0 | File InvaliddeltaCRLTest10EE.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | InvaliddeltaCRLTest3EE.p12 | 0 | File InvaliddeltaCRLTest3EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddeltaCRLTest4EE.p12 | 0 | File InvaliddeltaCRLTest4EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddeltaCRLTest6EE.p12 | 0 | File InvaliddeltaCRLTest6EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddeltaCRLTest9EE.p12 | 0 | File InvaliddeltaCRLTest9EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | InvaliddistributionPointTest2EE.p12 | 0 | File InvaliddistributionPointTest2EE.p12 has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest3EE.p12 | 0 | File InvaliddistributionPointTest3EE.p12 has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest6EE.p12 | 0 | File InvaliddistributionPointTest6EE.p12 has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest8EE.p12 | 0 | File InvaliddistributionPointTest8EE.p12 has permissions -rw |
| HIGH | GS002 | InvaliddistributionPointTest9EE.p12 | 0 | File InvaliddistributionPointTest9EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest1EE.p12 | 0 | File InvalidinhibitAnyPolicyTest1EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest4EE.p12 | 0 | File InvalidinhibitAnyPolicyTest4EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest5EE.p12 | 0 | File InvalidinhibitAnyPolicyTest5EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidinhibitAnyPolicyTest6EE.p12 | 0 | File InvalidinhibitAnyPolicyTest6EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest1EE.p12 | 0 | File InvalidinhibitPolicyMappingTest1EE.p12 has permissions  |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest3EE.p12 | 0 | File InvalidinhibitPolicyMappingTest3EE.p12 has permissions  |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest5EE.p12 | 0 | File InvalidinhibitPolicyMappingTest5EE.p12 has permissions  |
| HIGH | GS002 | InvalidinhibitPolicyMappingTest6EE.p12 | 0 | File InvalidinhibitPolicyMappingTest6EE.p12 has permissions  |
| HIGH | GS002 | InvalidkeyUsageCriticalcRLSignFalseTest4EE.p12 | 0 | File InvalidkeyUsageCriticalcRLSignFalseTest4EE.p12 has perm |
| HIGH | GS002 | InvalidkeyUsageCriticalkeyCertSignFalseTest1EE.p12 | 0 | File InvalidkeyUsageCriticalkeyCertSignFalseTest1EE.p12 has  |
| HIGH | GS002 | InvalidkeyUsageNotCriticalcRLSignFalseTest5EE.p12 | 0 | File InvalidkeyUsageNotCriticalcRLSignFalseTest5EE.p12 has p |
| HIGH | GS002 | InvalidkeyUsageNotCriticalkeyCertSignFalseTest2EE.p12 | 0 | File InvalidkeyUsageNotCriticalkeyCertSignFalseTest2EE.p12 h |
| HIGH | GS002 | InvalidonlyContainsAttributeCertsTest14EE.p12 | 0 | File InvalidonlyContainsAttributeCertsTest14EE.p12 has permi |
| HIGH | GS002 | InvalidonlyContainsCACertsTest12EE.p12 | 0 | File InvalidonlyContainsCACertsTest12EE.p12 has permissions  |
| HIGH | GS002 | InvalidonlyContainsUserCertsTest11EE.p12 | 0 | File InvalidonlyContainsUserCertsTest11EE.p12 has permission |
| HIGH | GS002 | InvalidonlySomeReasonsTest15EE.p12 | 0 | File InvalidonlySomeReasonsTest15EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest16EE.p12 | 0 | File InvalidonlySomeReasonsTest16EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest17EE.p12 | 0 | File InvalidonlySomeReasonsTest17EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest20EE.p12 | 0 | File InvalidonlySomeReasonsTest20EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidonlySomeReasonsTest21EE.p12 | 0 | File InvalidonlySomeReasonsTest21EE.p12 has permissions -rw- |
| HIGH | GS002 | InvalidpathLenConstraintTest10EE.p12 | 0 | File InvalidpathLenConstraintTest10EE.p12 has permissions -r |
| HIGH | GS002 | InvalidpathLenConstraintTest11EE.p12 | 0 | File InvalidpathLenConstraintTest11EE.p12 has permissions -r |
| HIGH | GS002 | InvalidpathLenConstraintTest12EE.p12 | 0 | File InvalidpathLenConstraintTest12EE.p12 has permissions -r |
| HIGH | GS002 | InvalidpathLenConstraintTest5EE.p12 | 0 | File InvalidpathLenConstraintTest5EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidpathLenConstraintTest6EE.p12 | 0 | File InvalidpathLenConstraintTest6EE.p12 has permissions -rw |
| HIGH | GS002 | InvalidpathLenConstraintTest9EE.p12 | 0 | File InvalidpathLenConstraintTest9EE.p12 has permissions -rw |
| HIGH | GS002 | Invalidpre2000CRLnextUpdateTest12EE.p12 | 0 | File Invalidpre2000CRLnextUpdateTest12EE.p12 has permissions |
| HIGH | GS002 | Invalidpre2000UTCEEnotAfterDateTest7EE.p12 | 0 | File Invalidpre2000UTCEEnotAfterDateTest7EE.p12 has permissi |
| HIGH | GS002 | InvalidrequireExplicitPolicyTest3EE.p12 | 0 | File InvalidrequireExplicitPolicyTest3EE.p12 has permissions |
| HIGH | GS002 | InvalidrequireExplicitPolicyTest5EE.p12 | 0 | File InvalidrequireExplicitPolicyTest5EE.p12 has permissions |
| HIGH | GS002 | LongSerialNumberCACert.p12 | 0 | File LongSerialNumberCACert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | Mapping1to2CACert.p12 | 0 | File Mapping1to2CACert.p12 has permissions -rw-rw-r-- — read |
| HIGH | GS002 | MappingFromanyPolicyCACert.p12 | 0 | File MappingFromanyPolicyCACert.p12 has permissions -rw-rw-r |
| HIGH | GS002 | MappingToanyPolicyCACert.p12 | 0 | File MappingToanyPolicyCACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | MissingbasicConstraintsCACert.p12 | 0 | File MissingbasicConstraintsCACert.p12 has permissions -rw-r |
| HIGH | GS002 | NameOrderingCACert.p12 | 0 | File NameOrderingCACert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | NegativeSerialNumberCACert.p12 | 0 | File NegativeSerialNumberCACert.p12 has permissions -rw-rw-r |
| HIGH | GS002 | NoCRLCACert.p12 | 0 | File NoCRLCACert.p12 has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | NoPoliciesCACert.p12 | 0 | File NoPoliciesCACert.p12 has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | NoissuingDistributionPointCACert.p12 | 0 | File NoissuingDistributionPointCACert.p12 has permissions -r |
| HIGH | GS002 | OldCRLnextUpdateCACert.p12 | 0 | File OldCRLnextUpdateCACert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | OverlappingPoliciesTest6EE.p12 | 0 | File OverlappingPoliciesTest6EE.p12 has permissions -rw-rw-r |
| HIGH | GS002 | P12Mapping1to3CACert.p12 | 0 | File P12Mapping1to3CACert.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | P12Mapping1to3subCACert.p12 | 0 | File P12Mapping1to3subCACert.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | P12Mapping1to3subsubCACert.p12 | 0 | File P12Mapping1to3subsubCACert.p12 has permissions -rw-rw-r |
| HIGH | GS002 | P1Mapping1to234CACert.p12 | 0 | File P1Mapping1to234CACert.p12 has permissions -rw-rw-r-- —  |
| HIGH | GS002 | P1Mapping1to234subCACert.p12 | 0 | File P1Mapping1to234subCACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | P1anyPolicyMapping1to2CACert.p12 | 0 | File P1anyPolicyMapping1to2CACert.p12 has permissions -rw-rw |
| HIGH | GS002 | PanyPolicyMapping1to2CACert.p12 | 0 | File PanyPolicyMapping1to2CACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | PoliciesP1234CACert.p12 | 0 | File PoliciesP1234CACert.p12 has permissions -rw-rw-r-- — re |
| HIGH | GS002 | PoliciesP1234subCAP123Cert.p12 | 0 | File PoliciesP1234subCAP123Cert.p12 has permissions -rw-rw-r |
| HIGH | GS002 | PoliciesP1234subsubCAP123P12Cert.p12 | 0 | File PoliciesP1234subsubCAP123P12Cert.p12 has permissions -r |
| HIGH | GS002 | PoliciesP123CACert.p12 | 0 | File PoliciesP123CACert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | PoliciesP123subCAP12Cert.p12 | 0 | File PoliciesP123subCAP12Cert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | PoliciesP123subsubCAP12P1Cert.p12 | 0 | File PoliciesP123subsubCAP12P1Cert.p12 has permissions -rw-r |
| HIGH | GS002 | PoliciesP123subsubCAP12P2Cert.p12 | 0 | File PoliciesP123subsubCAP12P2Cert.p12 has permissions -rw-r |
| HIGH | GS002 | PoliciesP123subsubsubCAP12P2P1Cert.p12 | 0 | File PoliciesP123subsubsubCAP12P2P1Cert.p12 has permissions  |
| HIGH | GS002 | PoliciesP12CACert.p12 | 0 | File PoliciesP12CACert.p12 has permissions -rw-rw-r-- — read |
| HIGH | GS002 | PoliciesP12subCAP1Cert.p12 | 0 | File PoliciesP12subCAP1Cert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | PoliciesP12subsubCAP1P2Cert.p12 | 0 | File PoliciesP12subsubCAP1P2Cert.p12 has permissions -rw-rw- |
| HIGH | GS002 | PoliciesP2subCA2Cert.p12 | 0 | File PoliciesP2subCA2Cert.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | PoliciesP2subCACert.p12 | 0 | File PoliciesP2subCACert.p12 has permissions -rw-rw-r-- — re |
| HIGH | GS002 | PoliciesP3CACert.p12 | 0 | File PoliciesP3CACert.p12 has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | RFC3280MandatoryAttributeTypesCACert.p12 | 0 | File RFC3280MandatoryAttributeTypesCACert.p12 has permission |
| HIGH | GS002 | RFC3280OptionalAttributeTypesCACert.p12 | 0 | File RFC3280OptionalAttributeTypesCACert.p12 has permissions |
| HIGH | GS002 | RevokedsubCACert.p12 | 0 | File RevokedsubCACert.p12 has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | RolloverfromPrintableStringtoUTF8StringCACert.p12 | 0 | File RolloverfromPrintableStringtoUTF8StringCACert.p12 has p |
| HIGH | GS002 | SeparateCertificateandCRLKeysCA2CRLSigningCert.p12 | 0 | File SeparateCertificateandCRLKeysCA2CRLSigningCert.p12 has  |
| HIGH | GS002 | SeparateCertificateandCRLKeysCA2CertificateSigningCACert.p12 | 0 | File SeparateCertificateandCRLKeysCA2CertificateSigningCACer |
| HIGH | GS002 | SeparateCertificateandCRLKeysCRLSigningCert.p12 | 0 | File SeparateCertificateandCRLKeysCRLSigningCert.p12 has per |
| HIGH | GS002 | SeparateCertificateandCRLKeysCertificateSigningCACert.p12 | 0 | File SeparateCertificateandCRLKeysCertificateSigningCACert.p |
| HIGH | GS002 | TrustAnchorRootCertificate.p12 | 0 | File TrustAnchorRootCertificate.p12 has permissions -rw-rw-r |
| HIGH | GS002 | TwoCRLsCACert.p12 | 0 | File TwoCRLsCACert.p12 has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | UIDCACert.p12 | 0 | File UIDCACert.p12 has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | UTF8StringCaseInsensitiveMatchCACert.p12 | 0 | File UTF8StringCaseInsensitiveMatchCACert.p12 has permission |
| HIGH | GS002 | UTF8StringEncodedNamesCACert.p12 | 0 | File UTF8StringEncodedNamesCACert.p12 has permissions -rw-rw |
| HIGH | GS002 | UnknownCRLEntryExtensionCACert.p12 | 0 | File UnknownCRLEntryExtensionCACert.p12 has permissions -rw- |
| HIGH | GS002 | UnknownCRLExtensionCACert.p12 | 0 | File UnknownCRLExtensionCACert.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | UserNoticeQualifierTest15EE.p12 | 0 | File UserNoticeQualifierTest15EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest16EE.p12 | 0 | File UserNoticeQualifierTest16EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest17EE.p12 | 0 | File UserNoticeQualifierTest17EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest18EE.p12 | 0 | File UserNoticeQualifierTest18EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | UserNoticeQualifierTest19EE.p12 | 0 | File UserNoticeQualifierTest19EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | ValidBasicSelfIssuedCRLSigningKeyTest6EE.p12 | 0 | File ValidBasicSelfIssuedCRLSigningKeyTest6EE.p12 has permis |
| HIGH | GS002 | ValidBasicSelfIssuedNewWithOldTest3EE.p12 | 0 | File ValidBasicSelfIssuedNewWithOldTest3EE.p12 has permissio |
| HIGH | GS002 | ValidBasicSelfIssuedNewWithOldTest4EE.p12 | 0 | File ValidBasicSelfIssuedNewWithOldTest4EE.p12 has permissio |
| HIGH | GS002 | ValidBasicSelfIssuedOldWithNewTest1EE.p12 | 0 | File ValidBasicSelfIssuedOldWithNewTest1EE.p12 has permissio |
| HIGH | GS002 | ValidCertificatePathTest1EE.p12 | 0 | File ValidCertificatePathTest1EE.p12 has permissions -rw-rw- |
| HIGH | GS002 | ValidDNSnameConstraintsTest30EE.p12 | 0 | File ValidDNSnameConstraintsTest30EE.p12 has permissions -rw |
| HIGH | GS002 | ValidDNSnameConstraintsTest32EE.p12 | 0 | File ValidDNSnameConstraintsTest32EE.p12 has permissions -rw |
| HIGH | GS002 | ValidDNandRFC822nameConstraintsTest27EE.p12 | 0 | File ValidDNandRFC822nameConstraintsTest27EE.p12 has permiss |
| HIGH | GS002 | ValidDNnameConstraintsTest11EE.p12 | 0 | File ValidDNnameConstraintsTest11EE.p12 has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest14EE.p12 | 0 | File ValidDNnameConstraintsTest14EE.p12 has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest18EE.p12 | 0 | File ValidDNnameConstraintsTest18EE.p12 has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest19EE.p12 | 0 | File ValidDNnameConstraintsTest19EE.p12 has permissions -rw- |
| HIGH | GS002 | ValidDNnameConstraintsTest1EE.p12 | 0 | File ValidDNnameConstraintsTest1EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidDNnameConstraintsTest4EE.p12 | 0 | File ValidDNnameConstraintsTest4EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidDNnameConstraintsTest5EE.p12 | 0 | File ValidDNnameConstraintsTest5EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidDNnameConstraintsTest6EE.p12 | 0 | File ValidDNnameConstraintsTest6EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidDSAParameterInheritanceTest5EE.p12 | 0 | File ValidDSAParameterInheritanceTest5EE.p12 has permissions |
| HIGH | GS002 | ValidDSASignaturesTest4EE.p12 | 0 | File ValidDSASignaturesTest4EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | ValidGeneralizedTimeCRLnextUpdateTest13EE.p12 | 0 | File ValidGeneralizedTimeCRLnextUpdateTest13EE.p12 has permi |
| HIGH | GS002 | ValidGeneralizedTimenotAfterDateTest8EE.p12 | 0 | File ValidGeneralizedTimenotAfterDateTest8EE.p12 has permiss |
| HIGH | GS002 | ValidGeneralizedTimenotBeforeDateTest4EE.p12 | 0 | File ValidGeneralizedTimenotBeforeDateTest4EE.p12 has permis |
| HIGH | GS002 | ValidIDPwithindirectCRLTest22EE.p12 | 0 | File ValidIDPwithindirectCRLTest22EE.p12 has permissions -rw |
| HIGH | GS002 | ValidIDPwithindirectCRLTest24EE.p12 | 0 | File ValidIDPwithindirectCRLTest24EE.p12 has permissions -rw |
| HIGH | GS002 | ValidIDPwithindirectCRLTest25EE.p12 | 0 | File ValidIDPwithindirectCRLTest25EE.p12 has permissions -rw |
| HIGH | GS002 | ValidLongSerialNumberTest16EE.p12 | 0 | File ValidLongSerialNumberTest16EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidLongSerialNumberTest17EE.p12 | 0 | File ValidLongSerialNumberTest17EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidNameChainingCapitalizationTest5EE.p12 | 0 | File ValidNameChainingCapitalizationTest5EE.p12 has permissi |
| HIGH | GS002 | ValidNameChainingWhitespaceTest3EE.p12 | 0 | File ValidNameChainingWhitespaceTest3EE.p12 has permissions  |
| HIGH | GS002 | ValidNameChainingWhitespaceTest4EE.p12 | 0 | File ValidNameChainingWhitespaceTest4EE.p12 has permissions  |
| HIGH | GS002 | ValidNameUIDsTest6EE.p12 | 0 | File ValidNameUIDsTest6EE.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValidNegativeSerialNumberTest14EE.p12 | 0 | File ValidNegativeSerialNumberTest14EE.p12 has permissions - |
| HIGH | GS002 | ValidNoissuingDistributionPointTest10EE.p12 | 0 | File ValidNoissuingDistributionPointTest10EE.p12 has permiss |
| HIGH | GS002 | ValidPolicyMappingTest11EE.p12 | 0 | File ValidPolicyMappingTest11EE.p12 has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest12EE.p12 | 0 | File ValidPolicyMappingTest12EE.p12 has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest13EE.p12 | 0 | File ValidPolicyMappingTest13EE.p12 has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest14EE.p12 | 0 | File ValidPolicyMappingTest14EE.p12 has permissions -rw-rw-r |
| HIGH | GS002 | ValidPolicyMappingTest1EE.p12 | 0 | File ValidPolicyMappingTest1EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest3EE.p12 | 0 | File ValidPolicyMappingTest3EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest5EE.p12 | 0 | File ValidPolicyMappingTest5EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest6EE.p12 | 0 | File ValidPolicyMappingTest6EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | ValidPolicyMappingTest9EE.p12 | 0 | File ValidPolicyMappingTest9EE.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | ValidRFC3280MandatoryAttributeTypesTest7EE.p12 | 0 | File ValidRFC3280MandatoryAttributeTypesTest7EE.p12 has perm |
| HIGH | GS002 | ValidRFC3280OptionalAttributeTypesTest8EE.p12 | 0 | File ValidRFC3280OptionalAttributeTypesTest8EE.p12 has permi |
| HIGH | GS002 | ValidRFC822nameConstraintsTest21EE.p12 | 0 | File ValidRFC822nameConstraintsTest21EE.p12 has permissions  |
| HIGH | GS002 | ValidRFC822nameConstraintsTest23EE.p12 | 0 | File ValidRFC822nameConstraintsTest23EE.p12 has permissions  |
| HIGH | GS002 | ValidRFC822nameConstraintsTest25EE.p12 | 0 | File ValidRFC822nameConstraintsTest25EE.p12 has permissions  |
| HIGH | GS002 | ValidRolloverfromPrintableStringtoUTF8StringTest10EE.p12 | 0 | File ValidRolloverfromPrintableStringtoUTF8StringTest10EE.p1 |
| HIGH | GS002 | ValidSelfIssuedinhibitAnyPolicyTest7EE.p12 | 0 | File ValidSelfIssuedinhibitAnyPolicyTest7EE.p12 has permissi |
| HIGH | GS002 | ValidSelfIssuedinhibitAnyPolicyTest9EE.p12 | 0 | File ValidSelfIssuedinhibitAnyPolicyTest9EE.p12 has permissi |
| HIGH | GS002 | ValidSelfIssuedinhibitPolicyMappingTest7EE.p12 | 0 | File ValidSelfIssuedinhibitPolicyMappingTest7EE.p12 has perm |
| HIGH | GS002 | ValidSelfIssuedpathLenConstraintTest15EE.p12 | 0 | File ValidSelfIssuedpathLenConstraintTest15EE.p12 has permis |
| HIGH | GS002 | ValidSelfIssuedpathLenConstraintTest17EE.p12 | 0 | File ValidSelfIssuedpathLenConstraintTest17EE.p12 has permis |
| HIGH | GS002 | ValidSelfIssuedrequireExplicitPolicyTest6EE.p12 | 0 | File ValidSelfIssuedrequireExplicitPolicyTest6EE.p12 has per |
| HIGH | GS002 | ValidSeparateCertificateandCRLKeysTest19EE.p12 | 0 | File ValidSeparateCertificateandCRLKeysTest19EE.p12 has perm |
| HIGH | GS002 | ValidTwoCRLsTest7EE.p12 | 0 | File ValidTwoCRLsTest7EE.p12 has permissions -rw-rw-r-- — re |
| HIGH | GS002 | ValidURInameConstraintsTest34EE.p12 | 0 | File ValidURInameConstraintsTest34EE.p12 has permissions -rw |
| HIGH | GS002 | ValidURInameConstraintsTest36EE.p12 | 0 | File ValidURInameConstraintsTest36EE.p12 has permissions -rw |
| HIGH | GS002 | ValidUTF8StringCaseInsensitiveMatchTest11EE.p12 | 0 | File ValidUTF8StringCaseInsensitiveMatchTest11EE.p12 has per |
| HIGH | GS002 | ValidUTF8StringEncodedNamesTest9EE.p12 | 0 | File ValidUTF8StringEncodedNamesTest9EE.p12 has permissions  |
| HIGH | GS002 | ValidUnknownNotCriticalCertificateExtensionTest1EE.p12 | 0 | File ValidUnknownNotCriticalCertificateExtensionTest1EE.p12  |
| HIGH | GS002 | ValidbasicConstraintsNotCriticalTest4EE.p12 | 0 | File ValidbasicConstraintsNotCriticalTest4EE.p12 has permiss |
| HIGH | GS002 | ValidcRLIssuerTest28EE.p12 | 0 | File ValidcRLIssuerTest28EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValidcRLIssuerTest29EE.p12 | 0 | File ValidcRLIssuerTest29EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValidcRLIssuerTest30EE.p12 | 0 | File ValidcRLIssuerTest30EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValidcRLIssuerTest33EE.p12 | 0 | File ValidcRLIssuerTest33EE.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | ValiddeltaCRLTest2EE.p12 | 0 | File ValiddeltaCRLTest2EE.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddeltaCRLTest5EE.p12 | 0 | File ValiddeltaCRLTest5EE.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddeltaCRLTest7EE.p12 | 0 | File ValiddeltaCRLTest7EE.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddeltaCRLTest8EE.p12 | 0 | File ValiddeltaCRLTest8EE.p12 has permissions -rw-rw-r-- — r |
| HIGH | GS002 | ValiddistributionPointTest1EE.p12 | 0 | File ValiddistributionPointTest1EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValiddistributionPointTest4EE.p12 | 0 | File ValiddistributionPointTest4EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValiddistributionPointTest5EE.p12 | 0 | File ValiddistributionPointTest5EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValiddistributionPointTest7EE.p12 | 0 | File ValiddistributionPointTest7EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidinhibitAnyPolicyTest2EE.p12 | 0 | File ValidinhibitAnyPolicyTest2EE.p12 has permissions -rw-rw |
| HIGH | GS002 | ValidinhibitPolicyMappingTest2EE.p12 | 0 | File ValidinhibitPolicyMappingTest2EE.p12 has permissions -r |
| HIGH | GS002 | ValidinhibitPolicyMappingTest4EE.p12 | 0 | File ValidinhibitPolicyMappingTest4EE.p12 has permissions -r |
| HIGH | GS002 | ValidkeyUsageNotCriticalTest3EE.p12 | 0 | File ValidkeyUsageNotCriticalTest3EE.p12 has permissions -rw |
| HIGH | GS002 | ValidonlyContainsCACertsTest13EE.p12 | 0 | File ValidonlyContainsCACertsTest13EE.p12 has permissions -r |
| HIGH | GS002 | ValidonlySomeReasonsTest18EE.p12 | 0 | File ValidonlySomeReasonsTest18EE.p12 has permissions -rw-rw |
| HIGH | GS002 | ValidonlySomeReasonsTest19EE.p12 | 0 | File ValidonlySomeReasonsTest19EE.p12 has permissions -rw-rw |
| HIGH | GS002 | ValidpathLenConstraintTest13EE.p12 | 0 | File ValidpathLenConstraintTest13EE.p12 has permissions -rw- |
| HIGH | GS002 | ValidpathLenConstraintTest14EE.p12 | 0 | File ValidpathLenConstraintTest14EE.p12 has permissions -rw- |
| HIGH | GS002 | ValidpathLenConstraintTest7EE.p12 | 0 | File ValidpathLenConstraintTest7EE.p12 has permissions -rw-r |
| HIGH | GS002 | ValidpathLenConstraintTest8EE.p12 | 0 | File ValidpathLenConstraintTest8EE.p12 has permissions -rw-r |
| HIGH | GS002 | Validpre2000UTCnotBeforeDateTest3EE.p12 | 0 | File Validpre2000UTCnotBeforeDateTest3EE.p12 has permissions |
| HIGH | GS002 | ValidrequireExplicitPolicyTest1EE.p12 | 0 | File ValidrequireExplicitPolicyTest1EE.p12 has permissions - |
| HIGH | GS002 | ValidrequireExplicitPolicyTest2EE.p12 | 0 | File ValidrequireExplicitPolicyTest2EE.p12 has permissions - |
| HIGH | GS002 | ValidrequireExplicitPolicyTest4EE.p12 | 0 | File ValidrequireExplicitPolicyTest4EE.p12 has permissions - |
| HIGH | GS002 | WrongCRLCACert.p12 | 0 | File WrongCRLCACert.p12 has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | anyPolicyCACert.p12 | 0 | File anyPolicyCACert.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | basicConstraintsCriticalcAFalseCACert.p12 | 0 | File basicConstraintsCriticalcAFalseCACert.p12 has permissio |
| HIGH | GS002 | basicConstraintsNotCriticalCACert.p12 | 0 | File basicConstraintsNotCriticalCACert.p12 has permissions - |
| HIGH | GS002 | basicConstraintsNotCriticalcAFalseCACert.p12 | 0 | File basicConstraintsNotCriticalcAFalseCACert.p12 has permis |
| HIGH | GS002 | deltaCRLCA1Cert.p12 | 0 | File deltaCRLCA1Cert.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | deltaCRLCA2Cert.p12 | 0 | File deltaCRLCA2Cert.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | deltaCRLCA3Cert.p12 | 0 | File deltaCRLCA3Cert.p12 has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | deltaCRLIndicatorNoBaseCACert.p12 | 0 | File deltaCRLIndicatorNoBaseCACert.p12 has permissions -rw-r |
| HIGH | GS002 | distributionPoint1CACert.p12 | 0 | File distributionPoint1CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | distributionPoint2CACert.p12 | 0 | File distributionPoint2CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | indirectCRLCA1Cert.p12 | 0 | File indirectCRLCA1Cert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA2Cert.p12 | 0 | File indirectCRLCA2Cert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA3Cert.p12 | 0 | File indirectCRLCA3Cert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA3cRLIssuerCert.p12 | 0 | File indirectCRLCA3cRLIssuerCert.p12 has permissions -rw-rw- |
| HIGH | GS002 | indirectCRLCA4Cert.p12 | 0 | File indirectCRLCA4Cert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA4cRLIssuerCert.p12 | 0 | File indirectCRLCA4cRLIssuerCert.p12 has permissions -rw-rw- |
| HIGH | GS002 | indirectCRLCA5Cert.p12 | 0 | File indirectCRLCA5Cert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | indirectCRLCA6Cert.p12 | 0 | File indirectCRLCA6Cert.p12 has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | inhibitAnyPolicy0CACert.p12 | 0 | File inhibitAnyPolicy0CACert.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitAnyPolicy1CACert.p12 | 0 | File inhibitAnyPolicy1CACert.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitAnyPolicy1SelfIssuedCACert.p12 | 0 | File inhibitAnyPolicy1SelfIssuedCACert.p12 has permissions - |
| HIGH | GS002 | inhibitAnyPolicy1SelfIssuedsubCA2Cert.p12 | 0 | File inhibitAnyPolicy1SelfIssuedsubCA2Cert.p12 has permissio |
| HIGH | GS002 | inhibitAnyPolicy1subCA1Cert.p12 | 0 | File inhibitAnyPolicy1subCA1Cert.p12 has permissions -rw-rw- |
| HIGH | GS002 | inhibitAnyPolicy1subCA2Cert.p12 | 0 | File inhibitAnyPolicy1subCA2Cert.p12 has permissions -rw-rw- |
| HIGH | GS002 | inhibitAnyPolicy1subCAIAP5Cert.p12 | 0 | File inhibitAnyPolicy1subCAIAP5Cert.p12 has permissions -rw- |
| HIGH | GS002 | inhibitAnyPolicy1subsubCA2Cert.p12 | 0 | File inhibitAnyPolicy1subsubCA2Cert.p12 has permissions -rw- |
| HIGH | GS002 | inhibitAnyPolicy5CACert.p12 | 0 | File inhibitAnyPolicy5CACert.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitAnyPolicy5subCACert.p12 | 0 | File inhibitAnyPolicy5subCACert.p12 has permissions -rw-rw-r |
| HIGH | GS002 | inhibitAnyPolicy5subsubCACert.p12 | 0 | File inhibitAnyPolicy5subsubCACert.p12 has permissions -rw-r |
| HIGH | GS002 | inhibitAnyPolicyTest3EE.p12 | 0 | File inhibitAnyPolicyTest3EE.p12 has permissions -rw-rw-r--  |
| HIGH | GS002 | inhibitPolicyMapping0CACert.p12 | 0 | File inhibitPolicyMapping0CACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | inhibitPolicyMapping0subCACert.p12 | 0 | File inhibitPolicyMapping0subCACert.p12 has permissions -rw- |
| HIGH | GS002 | inhibitPolicyMapping1P12CACert.p12 | 0 | File inhibitPolicyMapping1P12CACert.p12 has permissions -rw- |
| HIGH | GS002 | inhibitPolicyMapping1P12subCACert.p12 | 0 | File inhibitPolicyMapping1P12subCACert.p12 has permissions - |
| HIGH | GS002 | inhibitPolicyMapping1P12subCAIPM5Cert.p12 | 0 | File inhibitPolicyMapping1P12subCAIPM5Cert.p12 has permissio |
| HIGH | GS002 | inhibitPolicyMapping1P12subsubCACert.p12 | 0 | File inhibitPolicyMapping1P12subsubCACert.p12 has permission |
| HIGH | GS002 | inhibitPolicyMapping1P12subsubCAIPM5Cert.p12 | 0 | File inhibitPolicyMapping1P12subsubCAIPM5Cert.p12 has permis |
| HIGH | GS002 | inhibitPolicyMapping1P1CACert.p12 | 0 | File inhibitPolicyMapping1P1CACert.p12 has permissions -rw-r |
| HIGH | GS002 | inhibitPolicyMapping1P1SelfIssuedCACert.p12 | 0 | File inhibitPolicyMapping1P1SelfIssuedCACert.p12 has permiss |
| HIGH | GS002 | inhibitPolicyMapping1P1SelfIssuedsubCACert.p12 | 0 | File inhibitPolicyMapping1P1SelfIssuedsubCACert.p12 has perm |
| HIGH | GS002 | inhibitPolicyMapping1P1subCACert.p12 | 0 | File inhibitPolicyMapping1P1subCACert.p12 has permissions -r |
| HIGH | GS002 | inhibitPolicyMapping1P1subsubCACert.p12 | 0 | File inhibitPolicyMapping1P1subsubCACert.p12 has permissions |
| HIGH | GS002 | inhibitPolicyMapping5CACert.p12 | 0 | File inhibitPolicyMapping5CACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | inhibitPolicyMapping5subCACert.p12 | 0 | File inhibitPolicyMapping5subCACert.p12 has permissions -rw- |
| HIGH | GS002 | inhibitPolicyMapping5subsubCACert.p12 | 0 | File inhibitPolicyMapping5subsubCACert.p12 has permissions - |
| HIGH | GS002 | inhibitPolicyMapping5subsubsubCACert.p12 | 0 | File inhibitPolicyMapping5subsubsubCACert.p12 has permission |
| HIGH | GS002 | keyUsageCriticalcRLSignFalseCACert.p12 | 0 | File keyUsageCriticalcRLSignFalseCACert.p12 has permissions  |
| HIGH | GS002 | keyUsageCriticalkeyCertSignFalseCACert.p12 | 0 | File keyUsageCriticalkeyCertSignFalseCACert.p12 has permissi |
| HIGH | GS002 | keyUsageNotCriticalCACert.p12 | 0 | File keyUsageNotCriticalCACert.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | keyUsageNotCriticalcRLSignFalseCACert.p12 | 0 | File keyUsageNotCriticalcRLSignFalseCACert.p12 has permissio |
| HIGH | GS002 | keyUsageNotCriticalkeyCertSignFalseCACert.p12 | 0 | File keyUsageNotCriticalkeyCertSignFalseCACert.p12 has permi |
| HIGH | GS002 | nameConstraintsDN1CACert.p12 | 0 | File nameConstraintsDN1CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN1SelfIssuedCACert.p12 | 0 | File nameConstraintsDN1SelfIssuedCACert.p12 has permissions  |
| HIGH | GS002 | nameConstraintsDN1subCA1Cert.p12 | 0 | File nameConstraintsDN1subCA1Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN1subCA2Cert.p12 | 0 | File nameConstraintsDN1subCA2Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN1subCA3Cert.p12 | 0 | File nameConstraintsDN1subCA3Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN2CACert.p12 | 0 | File nameConstraintsDN2CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN3CACert.p12 | 0 | File nameConstraintsDN3CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN3subCA1Cert.p12 | 0 | File nameConstraintsDN3subCA1Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN3subCA2Cert.p12 | 0 | File nameConstraintsDN3subCA2Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsDN4CACert.p12 | 0 | File nameConstraintsDN4CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDN5CACert.p12 | 0 | File nameConstraintsDN5CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | nameConstraintsDNS1CACert.p12 | 0 | File nameConstraintsDNS1CACert.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | nameConstraintsDNS2CACert.p12 | 0 | File nameConstraintsDNS2CACert.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | nameConstraintsRFC822CA1Cert.p12 | 0 | File nameConstraintsRFC822CA1Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsRFC822CA2Cert.p12 | 0 | File nameConstraintsRFC822CA2Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsRFC822CA3Cert.p12 | 0 | File nameConstraintsRFC822CA3Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | nameConstraintsURI1CACert.p12 | 0 | File nameConstraintsURI1CACert.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | nameConstraintsURI2CACert.p12 | 0 | File nameConstraintsURI2CACert.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | onlyContainsAttributeCertsCACert.p12 | 0 | File onlyContainsAttributeCertsCACert.p12 has permissions -r |
| HIGH | GS002 | onlyContainsCACertsCACert.p12 | 0 | File onlyContainsCACertsCACert.p12 has permissions -rw-rw-r- |
| HIGH | GS002 | onlyContainsUserCertsCACert.p12 | 0 | File onlyContainsUserCertsCACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | onlySomeReasonsCA1Cert.p12 | 0 | File onlySomeReasonsCA1Cert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | onlySomeReasonsCA2Cert.p12 | 0 | File onlySomeReasonsCA2Cert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | onlySomeReasonsCA3Cert.p12 | 0 | File onlySomeReasonsCA3Cert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | onlySomeReasonsCA4Cert.p12 | 0 | File onlySomeReasonsCA4Cert.p12 has permissions -rw-rw-r-- — |
| HIGH | GS002 | pathLenConstraint0CACert.p12 | 0 | File pathLenConstraint0CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | pathLenConstraint0SelfIssuedCACert.p12 | 0 | File pathLenConstraint0SelfIssuedCACert.p12 has permissions  |
| HIGH | GS002 | pathLenConstraint0subCA2Cert.p12 | 0 | File pathLenConstraint0subCA2Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint0subCACert.p12 | 0 | File pathLenConstraint0subCACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | pathLenConstraint1CACert.p12 | 0 | File pathLenConstraint1CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | pathLenConstraint1SelfIssuedCACert.p12 | 0 | File pathLenConstraint1SelfIssuedCACert.p12 has permissions  |
| HIGH | GS002 | pathLenConstraint1SelfIssuedsubCACert.p12 | 0 | File pathLenConstraint1SelfIssuedsubCACert.p12 has permissio |
| HIGH | GS002 | pathLenConstraint1subCACert.p12 | 0 | File pathLenConstraint1subCACert.p12 has permissions -rw-rw- |
| HIGH | GS002 | pathLenConstraint6CACert.p12 | 0 | File pathLenConstraint6CACert.p12 has permissions -rw-rw-r-- |
| HIGH | GS002 | pathLenConstraint6subCA0Cert.p12 | 0 | File pathLenConstraint6subCA0Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint6subCA1Cert.p12 | 0 | File pathLenConstraint6subCA1Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint6subCA4Cert.p12 | 0 | File pathLenConstraint6subCA4Cert.p12 has permissions -rw-rw |
| HIGH | GS002 | pathLenConstraint6subsubCA00Cert.p12 | 0 | File pathLenConstraint6subsubCA00Cert.p12 has permissions -r |
| HIGH | GS002 | pathLenConstraint6subsubCA11Cert.p12 | 0 | File pathLenConstraint6subsubCA11Cert.p12 has permissions -r |
| HIGH | GS002 | pathLenConstraint6subsubCA41Cert.p12 | 0 | File pathLenConstraint6subsubCA41Cert.p12 has permissions -r |
| HIGH | GS002 | pathLenConstraint6subsubsubCA11XCert.p12 | 0 | File pathLenConstraint6subsubsubCA11XCert.p12 has permission |
| HIGH | GS002 | pathLenConstraint6subsubsubCA41XCert.p12 | 0 | File pathLenConstraint6subsubsubCA41XCert.p12 has permission |
| HIGH | GS002 | pre2000CRLnextUpdateCACert.p12 | 0 | File pre2000CRLnextUpdateCACert.p12 has permissions -rw-rw-r |
| HIGH | GS002 | requireExplicitPolicy0CACert.p12 | 0 | File requireExplicitPolicy0CACert.p12 has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy0subCACert.p12 | 0 | File requireExplicitPolicy0subCACert.p12 has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy0subsubCACert.p12 | 0 | File requireExplicitPolicy0subsubCACert.p12 has permissions  |
| HIGH | GS002 | requireExplicitPolicy0subsubsubCACert.p12 | 0 | File requireExplicitPolicy0subsubsubCACert.p12 has permissio |
| HIGH | GS002 | requireExplicitPolicy10CACert.p12 | 0 | File requireExplicitPolicy10CACert.p12 has permissions -rw-r |
| HIGH | GS002 | requireExplicitPolicy10subCACert.p12 | 0 | File requireExplicitPolicy10subCACert.p12 has permissions -r |
| HIGH | GS002 | requireExplicitPolicy10subsubCACert.p12 | 0 | File requireExplicitPolicy10subsubCACert.p12 has permissions |
| HIGH | GS002 | requireExplicitPolicy10subsubsubCACert.p12 | 0 | File requireExplicitPolicy10subsubsubCACert.p12 has permissi |
| HIGH | GS002 | requireExplicitPolicy2CACert.p12 | 0 | File requireExplicitPolicy2CACert.p12 has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy2SelfIssuedCACert.p12 | 0 | File requireExplicitPolicy2SelfIssuedCACert.p12 has permissi |
| HIGH | GS002 | requireExplicitPolicy2SelfIssuedsubCACert.p12 | 0 | File requireExplicitPolicy2SelfIssuedsubCACert.p12 has permi |
| HIGH | GS002 | requireExplicitPolicy2subCACert.p12 | 0 | File requireExplicitPolicy2subCACert.p12 has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy4CACert.p12 | 0 | File requireExplicitPolicy4CACert.p12 has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy4subCACert.p12 | 0 | File requireExplicitPolicy4subCACert.p12 has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy4subsubCACert.p12 | 0 | File requireExplicitPolicy4subsubCACert.p12 has permissions  |
| HIGH | GS002 | requireExplicitPolicy4subsubsubCACert.p12 | 0 | File requireExplicitPolicy4subsubsubCACert.p12 has permissio |
| HIGH | GS002 | requireExplicitPolicy5CACert.p12 | 0 | File requireExplicitPolicy5CACert.p12 has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy5subCACert.p12 | 0 | File requireExplicitPolicy5subCACert.p12 has permissions -rw |
| HIGH | GS002 | requireExplicitPolicy5subsubCACert.p12 | 0 | File requireExplicitPolicy5subsubCACert.p12 has permissions  |
| HIGH | GS002 | requireExplicitPolicy5subsubsubCACert.p12 | 0 | File requireExplicitPolicy5subsubsubCACert.p12 has permissio |
| HIGH | GS002 | requireExplicitPolicy7CACert.p12 | 0 | File requireExplicitPolicy7CACert.p12 has permissions -rw-rw |
| HIGH | GS002 | requireExplicitPolicy7subCARE2Cert.p12 | 0 | File requireExplicitPolicy7subCARE2Cert.p12 has permissions  |
| HIGH | GS002 | requireExplicitPolicy7subsubCARE2RE4Cert.p12 | 0 | File requireExplicitPolicy7subsubCARE2RE4Cert.p12 has permis |
| HIGH | GS002 | requireExplicitPolicy7subsubsubCARE2RE4Cert.p12 | 0 | File requireExplicitPolicy7subsubsubCARE2RE4Cert.p12 has per |
| HIGH | GS002 | accvraiz1.pem | 0 | File accvraiz1.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | badasn1time.pem | 0 | File badasn1time.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | badssl-sct.pem | 0 | File badssl-sct.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | belgian-eid-invalid-visiblestring.pem | 0 | File belgian-eid-invalid-visiblestring.pem has permissions - |
| HIGH | GS002 | bigoid.pem | 0 | File bigoid.pem has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | cryptography-scts.pem | 0 | File cryptography-scts.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | cryptography.io.chain.pem | 0 | File cryptography.io.chain.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | cryptography.io.chain_with_garbage.pem | 0 | File cryptography.io.chain_with_garbage.pem has permissions  |
| HIGH | GS002 | cryptography.io.old_header.pem | 0 | File cryptography.io.old_header.pem has permissions -rw-rw-r |
| HIGH | GS002 | cryptography.io.pem | 0 | File cryptography.io.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | cryptography.io.precert.pem | 0 | File cryptography.io.precert.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | cryptography.io.with_garbage.pem | 0 | File cryptography.io.with_garbage.pem has permissions -rw-rw |
| HIGH | GS002 | cryptography.io.with_headers.pem | 0 | File cryptography.io.with_headers.pem has permissions -rw-rw |
| HIGH | GS002 | admissions_extension_authority_not_provided.pem | 0 | File admissions_extension_authority_not_provided.pem has per |
| HIGH | GS002 | admissions_extension_optional_data_not_provided.pem | 0 | File admissions_extension_optional_data_not_provided.pem has |
| HIGH | GS002 | aia_ca_issuers.pem | 0 | File aia_ca_issuers.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | aia_ocsp.pem | 0 | File aia_ocsp.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | aia_ocsp_ca_issuers.pem | 0 | File aia_ocsp_ca_issuers.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | all_key_usages.pem | 0 | File all_key_usages.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | all_supported_names.pem | 0 | File all_supported_names.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | authority_key_identifier.pem | 0 | File authority_key_identifier.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | authority_key_identifier_no_keyid.pem | 0 | File authority_key_identifier_no_keyid.pem has permissions - |
| HIGH | GS002 | bad_country.pem | 0 | File bad_country.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | basic_constraints_not_critical.pem | 0 | File basic_constraints_not_critical.pem has permissions -rw- |
| HIGH | GS002 | bc_path_length_zero.pem | 0 | File bc_path_length_zero.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | ca.pem | 0 | File ca.pem has permissions -rw-rw-r-- — readable by any use |
| HIGH | GS002 | ca_key.pem | 0 | File ca_key.pem has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | rsa_ca.pem | 0 | File rsa_ca.pem has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | rsa_key.pem | 0 | File rsa_key.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | rsae_ca.pem | 0 | File rsae_ca.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | cdp_all_reasons.pem | 0 | File cdp_all_reasons.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | cdp_crl_issuer.pem | 0 | File cdp_crl_issuer.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | cdp_empty_hostname.pem | 0 | File cdp_empty_hostname.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | cdp_fullname_reasons_crl_issuer.pem | 0 | File cdp_fullname_reasons_crl_issuer.pem has permissions -rw |
| HIGH | GS002 | cdp_reason_aa_compromise.pem | 0 | File cdp_reason_aa_compromise.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | cp_cps_uri.pem | 0 | File cp_cps_uri.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | cp_invalid.pem | 0 | File cp_invalid.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | cp_user_notice_no_explicit_text.pem | 0 | File cp_user_notice_no_explicit_text.pem has permissions -rw |
| HIGH | GS002 | cp_user_notice_with_explicit_text.pem | 0 | File cp_user_notice_with_explicit_text.pem has permissions - |
| HIGH | GS002 | cp_user_notice_with_notice_reference.pem | 0 | File cp_user_notice_with_notice_reference.pem has permission |
| HIGH | GS002 | crl_all_reasons.pem | 0 | File crl_all_reasons.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | crl_almost_10k.pem | 0 | File crl_almost_10k.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | crl_bad_version.pem | 0 | File crl_bad_version.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | crl_delta_crl_indicator.pem | 0 | File crl_delta_crl_indicator.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | crl_dup_entry_ext.pem | 0 | File crl_dup_entry_ext.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | crl_empty.pem | 0 | File crl_empty.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | crl_ian_aia_aki.pem | 0 | File crl_ian_aia_aki.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | crl_idp_fullname_indirect_crl.pem | 0 | File crl_idp_fullname_indirect_crl.pem has permissions -rw-r |
| HIGH | GS002 | crl_idp_fullname_only.pem | 0 | File crl_idp_fullname_only.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | crl_idp_fullname_only_aa.pem | 0 | File crl_idp_fullname_only_aa.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | crl_idp_fullname_only_user.pem | 0 | File crl_idp_fullname_only_user.pem has permissions -rw-rw-r |
| HIGH | GS002 | crl_idp_only_ca.pem | 0 | File crl_idp_only_ca.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | crl_idp_reasons_only.pem | 0 | File crl_idp_reasons_only.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | crl_idp_relative_user_all_reasons.pem | 0 | File crl_idp_relative_user_all_reasons.pem has permissions - |
| HIGH | GS002 | crl_idp_relativename_only.pem | 0 | File crl_idp_relativename_only.pem has permissions -rw-rw-r- |
| HIGH | GS002 | crl_inval_cert_issuer_entry_ext.pem | 0 | File crl_inval_cert_issuer_entry_ext.pem has permissions -rw |
| HIGH | GS002 | crl_md2_unknown_crit_entry_ext.pem | 0 | File crl_md2_unknown_crit_entry_ext.pem has permissions -rw- |
| HIGH | GS002 | crl_no_next_update.pem | 0 | File crl_no_next_update.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | crl_unsupported_reason.pem | 0 | File crl_unsupported_reason.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | dsa_null_alg_params.pem | 0 | File dsa_null_alg_params.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | dsa_selfsigned_ca.pem | 0 | File dsa_selfsigned_ca.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | ec_no_named_curve.pem | 0 | File ec_no_named_curve.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | ecdsa_null_alg.pem | 0 | File ecdsa_null_alg.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | ekucrit-testuser-cert.pem | 0 | File ekucrit-testuser-cert.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | empty-eku.pem | 0 | File empty-eku.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | extended_key_usage.pem | 0 | File extended_key_usage.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | freshestcrl.pem | 0 | File freshestcrl.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | ian_uri.pem | 0 | File ian_uri.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | inhibit_any_policy_5.pem | 0 | File inhibit_any_policy_5.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | inhibit_any_policy_negative.pem | 0 | File inhibit_any_policy_negative.pem has permissions -rw-rw- |
| HIGH | GS002 | invalid_signature_cert.pem | 0 | File invalid_signature_cert.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | invalid_signature_crl.pem | 0 | File invalid_signature_crl.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | invalid_utf8_common_name.pem | 0 | File invalid_utf8_common_name.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | invalid_version.pem | 0 | File invalid_version.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | long-form-name-attribute.pem | 0 | File long-form-name-attribute.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | malformed-ian.pem | 0 | File malformed-ian.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | malformed-san.pem | 0 | File malformed-san.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | ms-certificate-template.pem | 0 | File ms-certificate-template.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | name_attribute_unsupported_tag.pem | 0 | File name_attribute_unsupported_tag.pem has permissions -rw- |
| HIGH | GS002 | nc_excluded.pem | 0 | File nc_excluded.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | nc_invalid_ip_netmask.pem | 0 | File nc_invalid_ip_netmask.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | nc_ip_invalid_length.pem | 0 | File nc_ip_invalid_length.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | nc_permitted.pem | 0 | File nc_permitted.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | nc_permitted_2.pem | 0 | File nc_permitted_2.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | nc_permitted_excluded.pem | 0 | File nc_permitted_excluded.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | nc_permitted_excluded_2.pem | 0 | File nc_permitted_excluded_2.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | nc_single_ip_netmask.pem | 0 | File nc_single_ip_netmask.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | negative_serial.pem | 0 | File negative_serial.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | no_sans.pem | 0 | File no_sans.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | ocsp_nocheck.pem | 0 | File ocsp_nocheck.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | pc_inhibit.pem | 0 | File pc_inhibit.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | pc_inhibit_require.pem | 0 | File pc_inhibit_require.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | pc_require.pem | 0 | File pc_require.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | policy_constraints_explicit.pem | 0 | File policy_constraints_explicit.pem has permissions -rw-rw- |
| HIGH | GS002 | post2000utctime.pem | 0 | File post2000utctime.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | private_key_usage_period_both_dates.pem | 0 | File private_key_usage_period_both_dates.pem has permissions |
| HIGH | GS002 | private_key_usage_period_only_not_after.pem | 0 | File private_key_usage_period_only_not_after.pem has permiss |
| HIGH | GS002 | private_key_usage_period_only_not_before.pem | 0 | File private_key_usage_period_only_not_before.pem has permis |
| HIGH | GS002 | rsa_pss.pem | 0 | File rsa_pss.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | rsa_pss_cert.pem | 0 | File rsa_pss_cert.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | rsa_pss_sha256_no_null.pem | 0 | File rsa_pss_sha256_no_null.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | san_dirname.pem | 0 | File san_dirname.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | san_email_dns_ip_dirname_uri.pem | 0 | File san_email_dns_ip_dirname_uri.pem has permissions -rw-rw |
| HIGH | GS002 | san_empty_hostname.pem | 0 | File san_empty_hostname.pem has permissions -rw-rw-r-- — rea |
| HIGH | GS002 | san_idna2003_dnsname.pem | 0 | File san_idna2003_dnsname.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | san_idna_names.pem | 0 | File san_idna_names.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | san_ipaddr.pem | 0 | File san_ipaddr.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | san_other_name.pem | 0 | File san_other_name.pem has permissions -rw-rw-r-- — readabl |
| HIGH | GS002 | san_registered_id.pem | 0 | File san_registered_id.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | san_rfc822_idna.pem | 0 | File san_rfc822_idna.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | san_rfc822_names.pem | 0 | File san_rfc822_names.pem has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | san_uri_with_port.pem | 0 | File san_uri_with_port.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | san_wildcard_idna.pem | 0 | File san_wildcard_idna.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | sia.pem | 0 | File sia.pem has permissions -rw-rw-r-- — readable by any us |
| HIGH | GS002 | two_basic_constraints.pem | 0 | File two_basic_constraints.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | unsupported_extension.pem | 0 | File unsupported_extension.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | unsupported_extension_2.pem | 0 | File unsupported_extension_2.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | unsupported_extension_critical.pem | 0 | File unsupported_extension_critical.pem has permissions -rw- |
| HIGH | GS002 | unsupported_subject_name.pem | 0 | File unsupported_subject_name.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | unsupported_subject_public_key_info.pem | 0 | File unsupported_subject_public_key_info.pem has permissions |
| HIGH | GS002 | utf8_common_name.pem | 0 | File utf8_common_name.pem has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | valid_signature_cert.pem | 0 | File valid_signature_cert.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | valid_signature_crl.pem | 0 | File valid_signature_crl.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | department-of-state-root.pem | 0 | File department-of-state-root.pem has permissions -rw-rw-r-- |
| HIGH | GS002 | ecdsa_root.pem | 0 | File ecdsa_root.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | ed25519-rfc8410.pem | 0 | File ed25519-rfc8410.pem has permissions -rw-rw-r-- — readab |
| HIGH | GS002 | root-ed25519.pem | 0 | File root-ed25519.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | server-ed25519-cert.pem | 0 | File server-ed25519-cert.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | root-ed448.pem | 0 | File root-ed448.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | server-ed448-cert.pem | 0 | File server-ed448-cert.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | ee-pss-sha1-cert.pem | 0 | File ee-pss-sha1-cert.pem has permissions -rw-rw-r-- — reada |
| HIGH | GS002 | letsencryptx3.pem | 0 | File letsencryptx3.pem has permissions -rw-rw-r-- — readable |
| HIGH | GS002 | rapidssl_sha256_ca_g3.pem | 0 | File rapidssl_sha256_ca_g3.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | bad-version.pem | 0 | File bad-version.pem has permissions -rw-rw-r-- — readable b |
| HIGH | GS002 | basic_constraints.pem | 0 | File basic_constraints.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | challenge-unstructured.pem | 0 | File challenge-unstructured.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | challenge.pem | 0 | File challenge.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | dsa_sha1.pem | 0 | File dsa_sha1.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | ec_sha256.pem | 0 | File ec_sha256.pem has permissions -rw-rw-r-- — readable by  |
| HIGH | GS002 | ec_sha256_old_header.pem | 0 | File ec_sha256_old_header.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | freeipa-bad-critical.pem | 0 | File freeipa-bad-critical.pem has permissions -rw-rw-r-- — r |
| HIGH | GS002 | invalid_signature.pem | 0 | File invalid_signature.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | long-form-attribute.pem | 0 | File long-form-attribute.pem has permissions -rw-rw-r-- — re |
| HIGH | GS002 | rsa_md4.pem | 0 | File rsa_md4.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | rsa_sha1.pem | 0 | File rsa_sha1.pem has permissions -rw-rw-r-- — readable by a |
| HIGH | GS002 | rsa_sha256.pem | 0 | File rsa_sha256.pem has permissions -rw-rw-r-- — readable by |
| HIGH | GS002 | san_rsa_sha1.pem | 0 | File san_rsa_sha1.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | two_basic_constraints.pem | 0 | File two_basic_constraints.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | unsupported_extension.pem | 0 | File unsupported_extension.pem has permissions -rw-rw-r-- —  |
| HIGH | GS002 | unsupported_extension_critical.pem | 0 | File unsupported_extension_critical.pem has permissions -rw- |
| HIGH | GS002 | zero-element-attribute.pem | 0 | File zero-element-attribute.pem has permissions -rw-rw-r-- — |
| HIGH | GS002 | scottishpower-bitstring-dn.pem | 0 | File scottishpower-bitstring-dn.pem has permissions -rw-rw-r |
| HIGH | GS002 | tls-feature-ocsp-staple.pem | 0 | File tls-feature-ocsp-staple.pem has permissions -rw-rw-r--  |
| HIGH | GS002 | unique_identifier.pem | 0 | File unique_identifier.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | utf8-dnsname.pem | 0 | File utf8-dnsname.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | v1_cert.pem | 0 | File v1_cert.pem has permissions -rw-rw-r-- — readable by an |
| HIGH | GS002 | verisign_md2_root.pem | 0 | File verisign_md2_root.pem has permissions -rw-rw-r-- — read |
| HIGH | GS002 | wildcard_san.pem | 0 | File wildcard_san.pem has permissions -rw-rw-r-- — readable  |
| HIGH | GS002 | wosign-bc-invalid.pem | 0 | File wosign-bc-invalid.pem has permissions -rw-rw-r-- — read |
| HIGH | GS004 | utils.py | 17 | Line 17: exec(f.read(), about) |
| HIGH | ? | extensions.rs | 36 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 37 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 62 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 32 | Clone in performance-critical code — consider references |
| HIGH | ? | buf.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 139 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 155 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 410 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 427 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 559 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 593 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 764 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 778 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 801 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 802 | Clone in performance-critical code — consider references |
| HIGH | ? | crl.rs | 803 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp.rs | 101 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp.rs | 119 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 249 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 291 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 402 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 409 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 624 | Clone in performance-critical code — consider references |
| HIGH | ? | extensions.rs | 681 | Clone in performance-critical code — consider references |
| HIGH | ? | sign.rs | 151 | Clone in performance-critical code — consider references |
| HIGH | ? | sign.rs | 152 | Clone in performance-critical code — consider references |
| HIGH | ? | sign.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | sign.rs | 323 | Clone in performance-critical code — consider references |
| HIGH | ? | sign.rs | 358 | Clone in performance-critical code — consider references |
| HIGH | ? | sign.rs | 506 | Clone in performance-critical code — consider references |
| HIGH | ? | sign.rs | 542 | Clone in performance-critical code — consider references |
| HIGH | ? | extension_policy.rs | 57 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 95 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 186 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 233 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 450 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 94 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 172 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 190 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 738 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 784 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 989 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 1014 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 1015 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 1016 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 1074 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 1096 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 1097 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 1098 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_req.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 143 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 145 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 153 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 166 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 263 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 264 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 293 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 329 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 350 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 351 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 352 | Clone in performance-critical code — consider references |
| HIGH | ? | csr.rs | 363 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 105 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 259 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 549 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 805 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 827 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 828 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 834 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 835 | Clone in performance-critical code — consider references |
| HIGH | ? | ocsp_resp.rs | 857 | Clone in performance-critical code — consider references |
| HIGH | ? | sct.rs | 265 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 220 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 281 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 344 | Clone in performance-critical code — consider references |
| HIGH | ? | common.rs | 429 | Clone in performance-critical code — consider references |
| HIGH | ? | asn1.rs | 20 | Clone in performance-critical code — consider references |
| HIGH | ? | asn1.rs | 27 | Clone in performance-critical code — consider references |
| HIGH | ? | asn1.rs | 84 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 173 | Clone in performance-critical code — consider references |
| HIGH | ? | error.rs | 325 | Clone in performance-critical code — consider references |
| HIGH | ? | utils.rs | 330 | Clone in performance-critical code — consider references |
| HIGH | ? | cmac.rs | 42 | Clone in performance-critical code — consider references |
| HIGH | ? | ciphers.rs | 28 | Clone in performance-critical code — consider references |
| HIGH | ? | ciphers.rs | 587 | Clone in performance-critical code — consider references |
| HIGH | ? | ciphers.rs | 620 | Clone in performance-critical code — consider references |
| HIGH | ? | hashes.rs | 96 | Clone in performance-critical code — consider references |
| HIGH | ? | hashes.rs | 135 | Clone in performance-critical code — consider references |
| HIGH | ? | hashes.rs | 219 | Clone in performance-critical code — consider references |
| HIGH | ? | hashes.rs | 262 | Clone in performance-critical code — consider references |
| HIGH | ? | hmac.rs | 38 | Clone in performance-critical code — consider references |
| HIGH | ? | hpke.rs | 844 | Clone in performance-critical code — consider references |
| HIGH | ? | hpke.rs | 868 | Clone in performance-critical code — consider references |
| HIGH | ? | cipher_registry.rs | 98 | Clone in performance-critical code — consider references |
| HIGH | ? | cipher_registry.rs | 99 | Clone in performance-critical code — consider references |
| HIGH | ? | ec.rs | 154 | Clone in performance-critical code — consider references |
| HIGH | ? | ec.rs | 179 | Clone in performance-critical code — consider references |
| HIGH | ? | ec.rs | 552 | Clone in performance-critical code — consider references |
| HIGH | ? | ec.rs | 633 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs12.rs | 182 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs12.rs | 389 | Clone in performance-critical code — consider references |
| HIGH | ? | test_support.rs | 34 | Clone in performance-critical code — consider references |
| HIGH | ? | decode.rs | 346 | Clone in performance-critical code — consider references |
| HIGH | ? | asn1.rs | 18 | Clone in performance-critical code — consider references |
| HIGH | ? | encode.rs | 35 | Clone in performance-critical code — consider references |
| HIGH | ? | encode.rs | 253 | Clone in performance-critical code — consider references |
| HIGH | ? | encode.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | encode.rs | 388 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 359 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 64 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 142 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 252 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 255 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 391 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 507 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 519 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 521 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 569 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 570 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 571 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 584 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 586 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 591 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 598 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 599 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 600 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 665 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs7.rs | 806 | Clone in performance-critical code — consider references |
| HIGH | ? | types.rs | 31 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 23 | Clone in performance-critical code — consider references |
| HIGH | ? | spki.rs | 181 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs8.rs | 214 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs8.rs | 360 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs8.rs | 386 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs8.rs | 422 | Clone in performance-critical code — consider references |
| HIGH | ? | pkcs8.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | ec.rs | 63 | Clone in performance-critical code — consider references |
| HIGH | ? | ec.rs | 67 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 256 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 260 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 283 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 444 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 464 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 529 | Clone in performance-critical code — consider references |
| HIGH | ? | lib.rs | 581 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 43 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 44 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 45 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 46 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 47 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 48 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 49 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 50 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 51 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 52 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 221 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 226 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 303 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 425 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 432 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 433 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 434 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 441 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 442 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 443 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 498 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 505 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 520 | Clone in performance-critical code — consider references |
| HIGH | ? | extension.rs | 541 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 70 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 71 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 72 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 73 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 156 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 157 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 158 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 159 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 160 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 161 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 162 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 163 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 164 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 202 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 315 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 336 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 514 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 800 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 810 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 820 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 829 | Clone in performance-critical code — consider references |
| HIGH | ? | mod.rs | 839 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 74 | Clone in performance-critical code — consider references |
| HIGH | ? | certificate.rs | 78 | Clone in performance-critical code — consider references |
| HIGH | ? | trust_store.rs | 22 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| M | ? | name.py | 154 |
| M | ? | backend.py | 89 |
| M | ? | ssh.py | 740 |
| M | ? | ssh.py | 998 |
| M | ? | ssh.py | 1004 |
| M | ? | ssh.py | 1020 |
| M | ? | ssh.py | 1595 |
| M | ? | padding.py | 110 |
| M | ? | rsa.py | 293 |
| M | ? | base.py | 91 |
| M | ? | keywrap.py | 34 |
| M | ? | keywrap.py | 77 |
| M | ? | keywrap.py | 102 |
| M | ? | keywrap.py | 124 |
| M | ? | noxfile.py | 65 |
| M | ? | noxfile.py | 240 |
| M | ? | noxfile.py | 279 |
| M | ? | noxfile.py | 401 |
| M | ? | release.py | 56 |
| C | GS001 | _oid.py | 367 |
| C | GS001 | gen.sh | 33 |
| L | GS003 | release.py | 27 |
| L | GS003 | build.rs | 15 |
| L | GS003 | build.rs | 18 |
| L | GS003 | build.rs | 21 |
| L | GS003 | build.rs | 24 |
| L | GS003 | build.rs | 29 |
| L | GS003 | build.rs | 33 |
| L | GS003 | build.rs | 37 |
| L | GS003 | build.rs | 41 |
| L | GS003 | build.rs | 46 |
| L | GS003 | build.rs | 58 |
| L | GS003 | build.rs | 22 |
| L | GS003 | build.rs | 23 |
| L | GS003 | build.rs | 30 |
| L | GS003 | build.rs | 31 |
| L | GS003 | build.rs | 32 |
| L | GS003 | build.rs | 51 |
| L | GS003 | build.rs | 52 |
| L | GS003 | build.rs | 144 |
| L | GS003 | build.rs | 181 |
| L | GS003 | build.rs | 195 |
| L | GS003 | build.rs | 10 |
| L | GS003 | build.rs | 14 |
| L | GS003 | build.rs | 18 |
| L | GS003 | build.rs | 24 |
| L | GS003 | build.rs | 30 |
| L | GS003 | build.rs | 13 |
| L | GS003 | build.rs | 16 |
| L | GS003 | build.rs | 21 |
| L | GS003 | build.rs | 33 |
| L | GS003 | build.rs | 36 |
| L | GS003 | build.rs | 37 |
| L | GS008 | asn1.py | 7 |
| L | GS008 | asn1.py | 11 |
| L | GS008 | asn1.py | 29 |
| L | GS008 | asn1.py | 56 |
| L | GS008 | bignum.py | 7 |
| L | GS008 | bignum.py | 11 |
| L | GS008 | bignum.py | 19 |
| L | GS008 | bignum.py | 37 |
| L | GS008 | bio.py | 7 |
| L | GS008 | bio.py | 11 |
| L | GS008 | bio.py | 17 |
| L | GS008 | bio.py | 37 |
| L | GS008 | crypto.py | 7 |
| L | GS008 | crypto.py | 11 |
| L | GS008 | crypto.py | 19 |
| L | GS008 | crypto.py | 29 |
| L | GS008 | cryptography.py | 7 |
| L | GS008 | cryptography.py | 63 |
| L | GS008 | cryptography.py | 66 |
| L | GS008 | cryptography.py | 69 |
| L | GS008 | dh.py | 7 |
| L | GS008 | dh.py | 11 |
| L | GS008 | dh.py | 15 |
| L | GS008 | dh.py | 19 |
| L | GS008 | dsa.py | 7 |
| L | GS008 | dsa.py | 11 |
| L | GS008 | dsa.py | 15 |
| L | GS008 | dsa.py | 24 |
| L | GS008 | ec.py | 7 |
| L | GS008 | ec.py | 12 |
| L | GS008 | ec.py | 20 |
| L | GS008 | ec.py | 28 |
| L | GS008 | engine.py | 7 |
| L | GS008 | engine.py | 13 |
| L | GS008 | engine.py | 20 |
| L | GS008 | engine.py | 41 |
| L | GS008 | err.py | 7 |
| L | GS008 | err.py | 11 |
| L | GS008 | err.py | 26 |
| L | GS008 | err.py | 38 |
| L | GS008 | evp.py | 7 |
| L | GS008 | evp.py | 11 |
| L | GS008 | evp.py | 25 |
| L | GS008 | evp.py | 44 |
| L | GS008 | nid.py | 7 |
| L | GS008 | nid.py | 11 |
| L | GS008 | nid.py | 15 |
| L | GS008 | nid.py | 18 |
| L | GS008 | objects.py | 7 |
| L | GS008 | objects.py | 11 |
| L | GS008 | objects.py | 14 |
| L | GS008 | objects.py | 21 |
| L | GS008 | opensslv.py | 7 |
| L | GS008 | opensslv.py | 11 |
| L | GS008 | opensslv.py | 18 |
| L | GS008 | opensslv.py | 21 |
| L | GS008 | pem.py | 7 |
| L | GS008 | pem.py | 11 |
| L | GS008 | pem.py | 15 |
| L | GS008 | pem.py | 35 |
| L | GS008 | rand.py | 7 |
| L | GS008 | rand.py | 11 |
| L | GS008 | rand.py | 14 |
| L | GS008 | rand.py | 19 |
| L | GS008 | rsa.py | 7 |
| L | GS008 | rsa.py | 11 |
| L | GS008 | rsa.py | 19 |
| L | GS008 | rsa.py | 27 |
| L | GS008 | ssl.py | 7 |
| L | GS008 | ssl.py | 11 |
| L | GS008 | ssl.py | 142 |
| L | GS008 | ssl.py | 447 |
| L | GS008 | x509.py | 7 |
| L | GS008 | x509.py | 30 |
| L | GS008 | x509.py | 111 |
| L | GS008 | x509_vfy.py | 7 |
| L | GS008 | x509_vfy.py | 125 |
| L | GS008 | x509_vfy.py | 172 |
| L | GS008 | x509name.py | 7 |
| L | GS008 | x509name.py | 16 |
| L | GS008 | x509name.py | 22 |
| L | GS008 | x509name.py | 51 |
| L | GS008 | x509v3.py | 7 |
| L | GS008 | x509v3.py | 11 |
| L | GS008 | x509v3.py | 25 |
| L | GS008 | x509v3.py | 28 |
| L | GS008 | _oid.py | 240 |
| L | GS008 | _conditional.py | 168 |
| L | GS008 | scrypt.py | 14 |
| L | GS008 | extensions.py | 705 |
| L | GS008 | extensions.py | 716 |
| L | GS008 | extensions.py | 739 |
| L | GS008 | extensions.py | 1101 |
| L | GS008 | name.py | 34 |
| H | ? | extension_policy.rs | 252 |
| H | ? | lib.rs | 622 |
| H | ? | mod.rs | 748 |
| H | ? | types.rs | 685 |
| H | ? | types.rs | 697 |
| H | ? | types.rs | 708 |
| H | ? | types.rs | 710 |
| H | ? | types.rs | 721 |
| H | ? | types.rs | 724 |
| H | ? | types.rs | 727 |
| H | ? | types.rs | 794 |
| H | ? | types.rs | 795 |
| H | ? | types.rs | 796 |
| H | ? | types.rs | 797 |
| H | ? | types.rs | 798 |
| H | ? | types.rs | 849 |
| H | ? | ec.py | 19 |
| H | ? | ec.py | 20 |
| H | ? | ec.py | 21 |
| H | ? | ec.py | 22 |
| H | ? | ec.py | 23 |
| H | ? | ec.py | 24 |
| H | ? | ec.py | 25 |
| H | ? | ec.py | 26 |
| H | ? | ec.py | 27 |
| H | ? | _oid.py | 14 |
| H | ? | _oid.py | 15 |
| H | ? | _oid.py | 16 |
| H | ? | _oid.py | 17 |
| H | ? | _oid.py | 18 |
| H | ? | _oid.py | 19 |
| H | ? | _oid.py | 20 |
| H | ? | _oid.py | 21 |
| H | ? | _oid.py | 22 |
| H | ? | _oid.py | 23 |
| H | ? | _oid.py | 24 |
| H | ? | _oid.py | 25 |
| H | ? | _oid.py | 26 |
| H | ? | _oid.py | 27 |
| H | ? | _oid.py | 28 |
| H | ? | _oid.py | 29 |
| H | ? | _oid.py | 30 |
| H | ? | _oid.py | 31 |
| H | ? | _oid.py | 32 |
| H | ? | _oid.py | 33 |
| H | ? | _oid.py | 34 |
| H | ? | _oid.py | 35 |
| H | ? | _oid.py | 36 |
| H | ? | _oid.py | 38 |
| H | ? | _oid.py | 40 |
| H | ? | _oid.py | 41 |
| H | ? | _oid.py | 42 |
| H | ? | _oid.py | 43 |
| H | ? | _oid.py | 47 |
| H | ? | _oid.py | 48 |
| H | ? | _oid.py | 52 |
| H | ? | _oid.py | 53 |
| H | ? | _oid.py | 54 |
| H | ? | _oid.py | 58 |
| H | ? | _oid.py | 59 |
| H | ? | _oid.py | 60 |
| H | ? | _oid.py | 61 |
| H | ? | _oid.py | 62 |
| H | ? | _oid.py | 63 |
| H | ? | _oid.py | 64 |
| H | ? | _oid.py | 65 |
| H | ? | _oid.py | 66 |
| H | ? | _oid.py | 67 |
| H | ? | _oid.py | 68 |
| H | ? | _oid.py | 69 |
| H | ? | _oid.py | 70 |
| H | ? | _oid.py | 71 |
| H | ? | _oid.py | 72 |
| H | ? | _oid.py | 73 |
| H | ? | _oid.py | 74 |
| H | ? | _oid.py | 75 |
| H | ? | _oid.py | 76 |
| H | ? | _oid.py | 77 |
| H | ? | _oid.py | 78 |
| H | ? | _oid.py | 79 |
| H | ? | _oid.py | 81 |
| H | ? | _oid.py | 83 |
| H | ? | _oid.py | 84 |
| H | ? | _oid.py | 85 |
| H | ? | _oid.py | 86 |
| H | ? | _oid.py | 89 |
| H | ? | _oid.py | 93 |
| H | ? | _oid.py | 94 |
| H | ? | _oid.py | 96 |
| H | ? | _oid.py | 97 |
| H | ? | _oid.py | 98 |
| H | ? | _oid.py | 99 |
| H | ? | _oid.py | 100 |
| H | ? | _oid.py | 101 |
| H | ? | _oid.py | 102 |
| H | ? | _oid.py | 103 |
| H | ? | _oid.py | 104 |
| H | ? | _oid.py | 105 |
| H | ? | _oid.py | 107 |
| H | ? | _oid.py | 108 |
| H | ? | _oid.py | 109 |
| H | ? | _oid.py | 110 |
| H | ? | _oid.py | 111 |
| H | ? | _oid.py | 112 |
| H | ? | _oid.py | 113 |
| H | ? | _oid.py | 114 |
| H | ? | _oid.py | 116 |
| H | ? | _oid.py | 117 |
| H | ? | _oid.py | 118 |
| H | ? | _oid.py | 119 |
| H | ? | _oid.py | 120 |
| H | ? | _oid.py | 121 |
| H | ? | _oid.py | 122 |
| H | ? | _oid.py | 123 |
| H | ? | _oid.py | 124 |
| H | ? | _oid.py | 125 |
| H | ? | _oid.py | 126 |
| H | ? | _oid.py | 127 |
| H | ? | _oid.py | 166 |
| H | ? | _oid.py | 167 |
| H | ? | _oid.py | 168 |
| H | ? | _oid.py | 169 |
| H | ? | _oid.py | 170 |
| H | ? | _oid.py | 171 |
| H | ? | _oid.py | 172 |
| H | ? | _oid.py | 173 |
| H | ? | _oid.py | 174 |
| H | ? | _oid.py | 175 |
| H | ? | _oid.py | 176 |
| H | ? | _oid.py | 177 |
| H | ? | _oid.py | 178 |
| H | ? | _oid.py | 184 |
| H | ? | _oid.py | 185 |
| H | ? | _oid.py | 186 |
| H | ? | _oid.py | 187 |
| H | ? | _oid.py | 188 |
| H | ? | _oid.py | 189 |
| H | ? | _oid.py | 190 |
| H | ? | _oid.py | 191 |
| H | ? | _oid.py | 192 |
| H | ? | _oid.py | 196 |
| H | ? | _oid.py | 197 |
| H | ? | _oid.py | 198 |
| H | ? | _oid.py | 199 |
| H | ? | _oid.py | 200 |
| H | ? | _oid.py | 201 |
| H | ? | _oid.py | 202 |
| H | ? | _oid.py | 203 |
| H | ? | _oid.py | 204 |
| H | ? | _oid.py | 205 |
| H | ? | _oid.py | 206 |
| H | ? | _oid.py | 207 |
| H | ? | _oid.py | 211 |
| H | ? | _oid.py | 212 |
| H | ? | _oid.py | 213 |
| H | ? | _oid.py | 214 |
| H | ? | _oid.py | 215 |
| H | ? | _oid.py | 216 |
| H | ? | _oid.py | 217 |
| H | ? | _oid.py | 221 |
| H | ? | _oid.py | 222 |
| H | ? | _oid.py | 226 |
| H | ? | _oid.py | 230 |
| H | ? | _oid.py | 231 |
| H | ? | _oid.py | 232 |
| H | ? | _oid.py | 236 |
| H | ? | _oid.py | 237 |
| H | ? | unsupported_extension.pem | 30 |
| H | ? | unsupported_extension_critical.pem | 30 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 129 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 151 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 261 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 283 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 311 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 366 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 454 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 476 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 592 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 603 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 801 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_resp.fax | 812 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 107 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 140 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 239 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 272 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 344 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 355 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 443 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 487 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 570 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 614 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 746 |
| H | ? | KASValidityTest_FFCStatic_NOKC_ZZOnly_init.fax | 801 |
| H | ? | pkits.schema | 1 |
| H | ? | pkits.schema | 4 |
| H | ? | pkits.schema | 12 |
| H | ? | pkits.schema | 19 |
| H | ? | pkits.ldif | 377 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 82 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 118 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 172 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 244 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 352 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 424 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 442 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 478 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 678 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 750 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 786 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 804 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 894 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 912 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1002 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1020 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1166 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1274 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1346 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1400 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1454 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1562 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1580 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1652 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1690 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1708 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1726 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 1942 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2014 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2068 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2140 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2194 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2232 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2268 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2304 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2376 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2520 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2556 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2664 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2682 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2792 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2846 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 2864 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3008 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3134 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3152 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3224 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3242 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3442 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3460 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3514 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3532 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3586 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3622 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3694 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3802 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3912 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 3984 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4020 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4074 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4200 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4254 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4326 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4380 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4490 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4508 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4544 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4616 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4688 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4742 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4760 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4922 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 4996 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5014 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5032 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5068 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5230 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5338 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5410 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_init.fax | 5428 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 64 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 82 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 118 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 226 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 334 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 352 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 388 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 496 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 696 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 714 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 822 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 840 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 894 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 912 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 930 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 948 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1202 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1220 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1238 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1328 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1418 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1508 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1526 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1562 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1690 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1852 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1906 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1942 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1960 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1978 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 1996 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2068 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2232 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2322 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2448 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2484 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2502 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2520 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2610 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2682 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2810 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2900 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 2954 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3026 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3044 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3080 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3098 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3206 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3424 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3442 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3550 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3568 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3604 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3676 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3748 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3766 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3966 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 3984 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4002 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4056 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4146 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4164 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4254 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4272 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4418 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4436 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4508 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4598 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4706 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4778 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4796 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4886 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 4942 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5032 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5122 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5194 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5230 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5248 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5374 |
| H | ? | KASValidityTest_ECCStaticUnified_KDFConcat_NOKC_resp.fax | 5392 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 55 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 81 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 146 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 159 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 237 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 250 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 276 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 393 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 447 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 460 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 486 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 590 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 655 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 668 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 746 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 759 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 839 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 930 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 956 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 982 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1073 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1086 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1138 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1164 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1244 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1283 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1309 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1400 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1452 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1478 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1491 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1556 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1623 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1636 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1649 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1675 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1831 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1896 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1922 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_resp.fax | 1987 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 81 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 107 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 159 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 224 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 276 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 341 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 367 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 406 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 473 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 486 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 512 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 538 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 694 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 707 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 720 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 746 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 826 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 839 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 904 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 956 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1021 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1151 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1164 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1190 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1283 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1322 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1361 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1400 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1491 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1543 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1556 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1582 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1636 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1649 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1675 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1753 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1922 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1935 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1948 |
| H | ? | KASValidityTest_ECCStaticUnified_NOKC_ZZOnly_init.fax | 1961 |
| C | ? | gen.sh | 33 |
| M | ? | noxfile.py | 36 |
| M | ? | noxfile.py | 43 |
| M | ? | release.py | 39 |
| M | ? | release.py | 45 |
| M | ? | release.py | 104 |
| M | ? | release.py | 109 |
| M | ? | release.py | 121 |
| M | ? | release.py | 127 |
| H | ? | utils.py | 17 |
| H | ? | .readthedocs.yml | 0 |
| H | GS002 | dh_key_256.pem | 0 |
| H | GS002 | dhkey.pem | 0 |
| H | GS002 | dhkey_rfc5114_2.pem | 0 |
| H | GS002 | dhp.pem | 0 |
| H | GS002 | dhp_privatevaluelength.pem | 0 |
| H | GS002 | dhp_rfc5114_2.pem | 0 |
| H | GS002 | dhpub.pem | 0 |
| H | GS002 | dhpub_cryptography_old.pem | 0 |
| H | GS002 | dhpub_rfc5114_2.pem | 0 |
| H | GS002 | nilpotent.pem | 0 |
| H | GS002 | ec-missing-curve.pem | 0 |
| H | GS002 | explicit_parameters_private_key.pem | 0 |
| H | GS002 | explicit_parameters_wap_wsg_idm_ecid_wtls11_private_key.pem | 0 |
| H | GS002 | high-bit-set.pem | 0 |
| H | GS002 | secp128r1_private_key.pem | 0 |
| H | GS002 | secp256k1-explicit-no-seed.pem | 0 |
| H | GS002 | secp256k1-pub-explicit-no-seed.pem | 0 |
| H | GS002 | secp256r1-explicit-no-seed.pem | 0 |
| H | GS002 | secp256r1-explicit-seed.pem | 0 |
| H | GS002 | secp256r1-pub-explicit-no-seed.pem | 0 |
| H | GS002 | secp256r1-pub-explicit-seed.pem | 0 |
| H | GS002 | secp384r1-explicit-no-seed.pem | 0 |
| H | GS002 | secp384r1-explicit-seed.pem | 0 |
| H | GS002 | secp384r1-pub-explicit-no-seed.pem | 0 |
| H | GS002 | secp384r1-pub-explicit-seed.pem | 0 |
| H | GS002 | secp521r1-explicit-no-seed.pem | 0 |
| H | GS002 | secp521r1-explicit-seed.pem | 0 |
| H | GS002 | secp521r1-pub-explicit-no-seed.pem | 0 |
| H | GS002 | secp521r1-pub-explicit-seed.pem | 0 |
| H | GS002 | sect163k1-spki.pem | 0 |
| H | GS002 | sect163r2-spki.pem | 0 |
| H | GS002 | sect233k1-spki.pem | 0 |
| H | GS002 | sect233r1-spki.pem | 0 |
| H | GS002 | ed25519-pkcs8-enc.pem | 0 |
| H | GS002 | ed25519-pkcs8.pem | 0 |
| H | GS002 | ed25519-pub.pem | 0 |
| H | GS002 | ed448-pkcs8-enc.pem | 0 |
| H | GS002 | ed448-pkcs8.pem | 0 |
| H | GS002 | ed448-pub.pem | 0 |
| H | GS002 | mlkem768.pem | 0 |
| H | GS002 | dsa-nopsw.key | 0 |
| H | GS002 | dsa-psw.key | 0 |
| H | GS002 | ecdsa-nopsw.key | 0 |
| H | GS002 | ecdsa-psw.key | 0 |
| H | GS002 | ed25519-aesgcm-psw.key | 0 |
| H | GS002 | ed25519-nopsw.key | 0 |
| H | GS002 | ed25519-psw.key | 0 |
| H | GS002 | rsa-nopsw.key | 0 |
| H | GS002 | rsa-psw.key | 0 |
| H | GS002 | sk-ecdsa-nopsw.key | 0 |
| H | GS002 | sk-ecdsa-psw.key | 0 |
| H | GS002 | sk-ed25519-nopsw.key | 0 |
| H | GS002 | sk-ed25519-psw.key | 0 |
| H | GS002 | dsa_4096.pem | 0 |
| H | GS002 | dsa_private_key.pem | 0 |
| H | GS002 | dsa_public_key.pem | 0 |
| H | GS002 | dsaparam.pem | 0 |
| H | GS002 | ec_private_key.pem | 0 |
| H | GS002 | ec_private_key_encrypted.pem | 0 |
| H | GS002 | ec_public_key.pem | 0 |
| H | GS002 | ec_public_key_rsa_delimiter.pem | 0 |
| H | GS002 | rsa-bad-1025-q-is-2.pem | 0 |
| H | GS002 | rsa_private_key.pem | 0 |
| H | GS002 | rsa_public_key.pem | 0 |
| H | GS002 | rsa_wrong_delimiter_public_key.pem | 0 |
| H | GS002 | bad-encryption-oid.pem | 0 |
| H | GS002 | bad-oid-dsa-key.pem | 0 |
| H | GS002 | ec-consistent-curve.pem | 0 |
| H | GS002 | ec-inconsistent-curve.pem | 0 |
| H | GS002 | ec-inconsistent-curve2.pem | 0 |
| H | GS002 | ec-invalid-private-scalar.pem | 0 |
| H | GS002 | ec-invalid-version.pem | 0 |
| H | GS002 | ec_oid_not_in_reg_private_2.pkcs8.pem | 0 |
| H | GS002 | ec_private_key.pem | 0 |
| H | GS002 | ec_private_key_encrypted.pem | 0 |
| H | GS002 | ecc_private_with_rfc5915_ext.pem | 0 |
| H | GS002 | ed25519-scrypt.pem | 0 |
| H | GS002 | enc-ec-sha1-128-rc4.pem | 0 |
| H | GS002 | enc-rsa-3des.pem | 0 |
| H | GS002 | enc-rsa-pkcs8-pbkdf2-0iter.pem | 0 |
| H | GS002 | enc-rsa-pkcs8.pem | 0 |
| H | GS002 | enc-unknown-algorithm.pem | 0 |
| H | GS002 | enc-unknown-kdf.pem | 0 |
| H | GS002 | enc-unknown-pbkdf2-prf.pem | 0 |
| H | GS002 | enc2-rsa-pkcs8.pem | 0 |
| H | GS002 | nodompar_private.pkcs8.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9607.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9671.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9925.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9926.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9927.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9928.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9929.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9930.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9931.pem | 0 |
| H | GS002 | pkcs12_s2k_pem-X_9932.pem | 0 |
| H | GS002 | private.pem | 0 |
| H | GS002 | rsa-40bitrc2.pem | 0 |
| H | GS002 | rsa-aes-192-cbc.pem | 0 |
| H | GS002 | rsa-pbe-3des-long-salt.pem | 0 |
| H | GS002 | rsa-pbewithmd5anddescbc.pem | 0 |
| H | GS002 | rsa-rc2-cbc-effective-key-length.pem | 0 |
| H | GS002 | rsa-rc2-cbc.pem | 0 |
| H | GS002 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha224.pem | 0 |
| H | GS002 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha384.pem | 0 |
| H | GS002 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha512.pem | 0 |
| H | GS002 | rsa_pss_2048.pem | 0 |
| H | GS002 | rsa_pss_2048_hash.pem | 0 |
| H | GS002 | rsa_pss_2048_hash_mask.pem | 0 |
| H | GS002 | rsa_pss_2048_hash_mask_diff.pem | 0 |
| H | GS002 | rsa_pss_2048_hash_mask_salt.pem | 0 |
| H | GS002 | unenc-dsa-pkcs8.pem | 0 |
| H | GS002 | unenc-dsa-pkcs8.pub.pem | 0 |
| H | GS002 | unenc-rsa-pkcs8.pem | 0 |
| H | GS002 | unenc-rsa-pkcs8.pub.pem | 0 |
| H | GS002 | withdompar_private.pkcs8.pem | 0 |
| H | GS002 | wrong-pem-delimiter-rsa.pem | 0 |
| H | GS002 | dsa-wrong-version.pem | 0 |
| H | GS002 | dsa.1024.pem | 0 |
| H | GS002 | dsa.2048.pem | 0 |
| H | GS002 | dsa.3072.pem | 0 |
| H | GS002 | key1-malformed-dek-info.pem | 0 |
| H | GS002 | key1-malformed-iv.pem | 0 |
| H | GS002 | key1-no-dek-info.pem | 0 |
| H | GS002 | key1-short-iv.pem | 0 |
| H | GS002 | key1.pem | 0 |
| H | GS002 | key2.pem | 0 |
| H | GS002 | rsa-wrong-version.pem | 0 |
| H | GS002 | testrsa-encrypted.pem | 0 |
| H | GS002 | testrsa.pem | 0 |
| H | GS002 | x25519-pkcs8-enc.pem | 0 |
| H | GS002 | x25519-pkcs8.pem | 0 |
| H | GS002 | x25519-pub.pem | 0 |
| H | GS002 | x448-pkcs8-enc.pem | 0 |
| H | GS002 | x448-pkcs8.pem | 0 |
| H | GS002 | x448-pub.pem | 0 |
| H | GS002 | dsa.pub.pem | 0 |
| H | GS002 | rsa.pub.pem | 0 |
| H | GS002 | ca.pem | 0 |
| H | GS002 | ca_key.pem | 0 |
| H | GS002 | cert-aes256cbc-no-key.p12 | 0 |
| H | GS002 | cert-key-aes256cbc.p12 | 0 |
| H | GS002 | cert-none-key-none.p12 | 0 |
| H | GS002 | cert-rc2-key-3des.p12 | 0 |
| H | GS002 | java-truststore.p12 | 0 |
| H | GS002 | name-1-no-pwd.p12 | 0 |
| H | GS002 | name-1-pwd.p12 | 0 |
| H | GS002 | name-2-3-no-pwd.p12 | 0 |
| H | GS002 | name-2-3-pwd.p12 | 0 |
| H | GS002 | name-2-no-pwd.p12 | 0 |
| H | GS002 | name-2-pwd.p12 | 0 |
| H | GS002 | name-3-no-pwd.p12 | 0 |
| H | GS002 | name-3-pwd.p12 | 0 |
| H | GS002 | name-all-no-pwd.p12 | 0 |
| H | GS002 | name-all-pwd.p12 | 0 |
| H | GS002 | name-unicode-no-pwd.p12 | 0 |
| H | GS002 | name-unicode-pwd.p12 | 0 |
| H | GS002 | no-cert-key-aes256cbc.p12 | 0 |
| H | GS002 | no-cert-name-2-no-pwd.p12 | 0 |
| H | GS002 | no-cert-name-2-pwd.p12 | 0 |
| H | GS002 | no-cert-name-3-no-pwd.p12 | 0 |
| H | GS002 | no-cert-name-3-pwd.p12 | 0 |
| H | GS002 | no-cert-name-all-no-pwd.p12 | 0 |
| H | GS002 | no-cert-name-all-pwd.p12 | 0 |
| H | GS002 | no-cert-name-unicode-no-pwd.p12 | 0 |
| H | GS002 | no-cert-name-unicode-pwd.p12 | 0 |
| H | GS002 | no-cert-no-name-no-pwd.p12 | 0 |
| H | GS002 | no-cert-no-name-pwd.p12 | 0 |
| H | GS002 | no-name-no-pwd.p12 | 0 |
| H | GS002 | no-name-pwd.p12 | 0 |
| H | GS002 | no-password.p12 | 0 |
| H | GS002 | ascii-san.pem | 0 |
| H | GS002 | enveloped-rsa-oaep.pem | 0 |
| H | GS002 | enveloped-triple-des.pem | 0 |
| H | GS002 | enveloped.pem | 0 |
| H | GS002 | isrg.pem | 0 |
| H | GS002 | non-ascii-san.pem | 0 |
| H | GS002 | AllCertificatesNoPoliciesTest2EE.crt | 0 |
| H | GS002 | AllCertificatesSamePoliciesTest10EE.crt | 0 |
| H | GS002 | AllCertificatesSamePoliciesTest13EE.crt | 0 |
| H | GS002 | AllCertificatesanyPolicyTest11EE.crt | 0 |
| H | GS002 | AnyPolicyTest14EE.crt | 0 |
| H | GS002 | BadCRLIssuerNameCACert.crt | 0 |
| H | GS002 | BadCRLSignatureCACert.crt | 0 |
| H | GS002 | BadSignedCACert.crt | 0 |
| H | GS002 | BadnotAfterDateCACert.crt | 0 |
| H | GS002 | BadnotBeforeDateCACert.crt | 0 |
| H | GS002 | BasicSelfIssuedCRLSigningKeyCACert.crt | 0 |
| H | GS002 | BasicSelfIssuedCRLSigningKeyCRLCert.crt | 0 |
| H | GS002 | BasicSelfIssuedNewKeyCACert.crt | 0 |
| H | GS002 | BasicSelfIssuedNewKeyOldWithNewCACert.crt | 0 |
| H | GS002 | BasicSelfIssuedOldKeyCACert.crt | 0 |
| H | GS002 | BasicSelfIssuedOldKeyNewWithOldCACert.crt | 0 |
| H | GS002 | CPSPointerQualifierTest20EE.crt | 0 |
| H | GS002 | DSACACert.crt | 0 |
| H | GS002 | DSAParametersInheritedCACert.crt | 0 |
| H | GS002 | DifferentPoliciesTest12EE.crt | 0 |
| H | GS002 | DifferentPoliciesTest3EE.crt | 0 |
| H | GS002 | DifferentPoliciesTest4EE.crt | 0 |
| H | GS002 | DifferentPoliciesTest5EE.crt | 0 |
| H | GS002 | DifferentPoliciesTest7EE.crt | 0 |
| H | GS002 | DifferentPoliciesTest8EE.crt | 0 |
| H | GS002 | DifferentPoliciesTest9EE.crt | 0 |
| H | GS002 | GeneralizedTimeCRLnextUpdateCACert.crt | 0 |
| H | GS002 | GoodCACert.crt | 0 |
| H | GS002 | GoodsubCACert.crt | 0 |
| H | GS002 | GoodsubCAPanyPolicyMapping1to2CACert.crt | 0 |
| H | GS002 | InvalidBadCRLIssuerNameTest5EE.crt | 0 |
| H | GS002 | InvalidBadCRLSignatureTest4EE.crt | 0 |
| H | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest7EE.crt | 0 |
| H | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest8EE.crt | 0 |
| H | GS002 | InvalidBasicSelfIssuedNewWithOldTest5EE.crt | 0 |
| H | GS002 | InvalidBasicSelfIssuedOldWithNewTest2EE.crt | 0 |
| H | GS002 | InvalidCASignatureTest2EE.crt | 0 |
| H | GS002 | InvalidCAnotAfterDateTest5EE.crt | 0 |
| H | GS002 | InvalidCAnotBeforeDateTest1EE.crt | 0 |
| H | GS002 | InvalidDNSnameConstraintsTest31EE.crt | 0 |
| H | GS002 | InvalidDNSnameConstraintsTest33EE.crt | 0 |
| H | GS002 | InvalidDNSnameConstraintsTest38EE.crt | 0 |
| H | GS002 | InvalidDNandRFC822nameConstraintsTest28EE.crt | 0 |
| H | GS002 | InvalidDNandRFC822nameConstraintsTest29EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest10EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest12EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest13EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest15EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest16EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest17EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest20EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest2EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest3EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest7EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest8EE.crt | 0 |
| H | GS002 | InvalidDNnameConstraintsTest9EE.crt | 0 |
| H | GS002 | InvalidDSASignatureTest6EE.crt | 0 |
| H | GS002 | InvalidEESignatureTest3EE.crt | 0 |
| H | GS002 | InvalidEEnotAfterDateTest6EE.crt | 0 |
| H | GS002 | InvalidEEnotBeforeDateTest2EE.crt | 0 |
| H | GS002 | InvalidIDPwithindirectCRLTest23EE.crt | 0 |
| H | GS002 | InvalidIDPwithindirectCRLTest26EE.crt | 0 |
| H | GS002 | InvalidLongSerialNumberTest18EE.crt | 0 |
| H | GS002 | InvalidMappingFromanyPolicyTest7EE.crt | 0 |
| H | GS002 | InvalidMappingToanyPolicyTest8EE.crt | 0 |
| H | GS002 | InvalidMissingCRLTest1EE.crt | 0 |
| H | GS002 | InvalidMissingbasicConstraintsTest1EE.crt | 0 |
| H | GS002 | InvalidNameChainingOrderTest2EE.crt | 0 |
| H | GS002 | InvalidNameChainingTest1EE.crt | 0 |
| H | GS002 | InvalidNegativeSerialNumberTest15EE.crt | 0 |
| H | GS002 | InvalidOldCRLnextUpdateTest11EE.crt | 0 |
| H | GS002 | InvalidPolicyMappingTest10EE.crt | 0 |
| H | GS002 | InvalidPolicyMappingTest2EE.crt | 0 |
| H | GS002 | InvalidPolicyMappingTest4EE.crt | 0 |
| H | GS002 | InvalidRFC822nameConstraintsTest22EE.crt | 0 |
| H | GS002 | InvalidRFC822nameConstraintsTest24EE.crt | 0 |
| H | GS002 | InvalidRFC822nameConstraintsTest26EE.crt | 0 |
| H | GS002 | InvalidRevokedCATest2EE.crt | 0 |
| H | GS002 | InvalidRevokedEETest3EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest10EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest8EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest10EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest11EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest8EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest9EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedpathLenConstraintTest16EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest7EE.crt | 0 |
| H | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest8EE.crt | 0 |
| H | GS002 | InvalidSeparateCertificateandCRLKeysTest20EE.crt | 0 |
| H | GS002 | InvalidSeparateCertificateandCRLKeysTest21EE.crt | 0 |
| H | GS002 | InvalidURInameConstraintsTest35EE.crt | 0 |
| H | GS002 | InvalidURInameConstraintsTest37EE.crt | 0 |
| H | GS002 | InvalidUnknownCRLEntryExtensionTest8EE.crt | 0 |
| H | GS002 | InvalidUnknownCRLExtensionTest10EE.crt | 0 |
| H | GS002 | InvalidUnknownCRLExtensionTest9EE.crt | 0 |
| H | GS002 | InvalidUnknownCriticalCertificateExtensionTest2EE.crt | 0 |
| H | GS002 | InvalidWrongCRLTest6EE.crt | 0 |
| H | GS002 | InvalidcAFalseTest2EE.crt | 0 |
| H | GS002 | InvalidcAFalseTest3EE.crt | 0 |
| H | GS002 | InvalidcRLIssuerTest27EE.crt | 0 |
| H | GS002 | InvalidcRLIssuerTest31EE.crt | 0 |
| H | GS002 | InvalidcRLIssuerTest32EE.crt | 0 |
| H | GS002 | InvalidcRLIssuerTest34EE.crt | 0 |
| H | GS002 | InvalidcRLIssuerTest35EE.crt | 0 |
| H | GS002 | InvaliddeltaCRLIndicatorNoBaseTest1EE.crt | 0 |
| H | GS002 | InvaliddeltaCRLTest10EE.crt | 0 |
| H | GS002 | InvaliddeltaCRLTest3EE.crt | 0 |
| H | GS002 | InvaliddeltaCRLTest4EE.crt | 0 |
| H | GS002 | InvaliddeltaCRLTest6EE.crt | 0 |
| H | GS002 | InvaliddeltaCRLTest9EE.crt | 0 |
| H | GS002 | InvaliddistributionPointTest2EE.crt | 0 |
| H | GS002 | InvaliddistributionPointTest3EE.crt | 0 |
| H | GS002 | InvaliddistributionPointTest6EE.crt | 0 |
| H | GS002 | InvaliddistributionPointTest8EE.crt | 0 |
| H | GS002 | InvaliddistributionPointTest9EE.crt | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest1EE.crt | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest4EE.crt | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest5EE.crt | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest6EE.crt | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest1EE.crt | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest3EE.crt | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest5EE.crt | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest6EE.crt | 0 |
| H | GS002 | InvalidkeyUsageCriticalcRLSignFalseTest4EE.crt | 0 |
| H | GS002 | InvalidkeyUsageCriticalkeyCertSignFalseTest1EE.crt | 0 |
| H | GS002 | InvalidkeyUsageNotCriticalcRLSignFalseTest5EE.crt | 0 |
| H | GS002 | InvalidkeyUsageNotCriticalkeyCertSignFalseTest2EE.crt | 0 |
| H | GS002 | InvalidonlyContainsAttributeCertsTest14EE.crt | 0 |
| H | GS002 | InvalidonlyContainsCACertsTest12EE.crt | 0 |
| H | GS002 | InvalidonlyContainsUserCertsTest11EE.crt | 0 |
| H | GS002 | InvalidonlySomeReasonsTest15EE.crt | 0 |
| H | GS002 | InvalidonlySomeReasonsTest16EE.crt | 0 |
| H | GS002 | InvalidonlySomeReasonsTest17EE.crt | 0 |
| H | GS002 | InvalidonlySomeReasonsTest20EE.crt | 0 |
| H | GS002 | InvalidonlySomeReasonsTest21EE.crt | 0 |
| H | GS002 | InvalidpathLenConstraintTest10EE.crt | 0 |
| H | GS002 | InvalidpathLenConstraintTest11EE.crt | 0 |
| H | GS002 | InvalidpathLenConstraintTest12EE.crt | 0 |
| H | GS002 | InvalidpathLenConstraintTest5EE.crt | 0 |
| H | GS002 | InvalidpathLenConstraintTest6EE.crt | 0 |
| H | GS002 | InvalidpathLenConstraintTest9EE.crt | 0 |
| H | GS002 | Invalidpre2000CRLnextUpdateTest12EE.crt | 0 |
| H | GS002 | Invalidpre2000UTCEEnotAfterDateTest7EE.crt | 0 |
| H | GS002 | InvalidrequireExplicitPolicyTest3EE.crt | 0 |
| H | GS002 | InvalidrequireExplicitPolicyTest5EE.crt | 0 |
| H | GS002 | LongSerialNumberCACert.crt | 0 |
| H | GS002 | Mapping1to2CACert.crt | 0 |
| H | GS002 | MappingFromanyPolicyCACert.crt | 0 |
| H | GS002 | MappingToanyPolicyCACert.crt | 0 |
| H | GS002 | MissingbasicConstraintsCACert.crt | 0 |
| H | GS002 | NameOrderingCACert.crt | 0 |
| H | GS002 | NegativeSerialNumberCACert.crt | 0 |
| H | GS002 | NoCRLCACert.crt | 0 |
| H | GS002 | NoPoliciesCACert.crt | 0 |
| H | GS002 | NoissuingDistributionPointCACert.crt | 0 |
| H | GS002 | OldCRLnextUpdateCACert.crt | 0 |
| H | GS002 | OverlappingPoliciesTest6EE.crt | 0 |
| H | GS002 | P12Mapping1to3CACert.crt | 0 |
| H | GS002 | P12Mapping1to3subCACert.crt | 0 |
| H | GS002 | P12Mapping1to3subsubCACert.crt | 0 |
| H | GS002 | P1Mapping1to234CACert.crt | 0 |
| H | GS002 | P1Mapping1to234subCACert.crt | 0 |
| H | GS002 | P1anyPolicyMapping1to2CACert.crt | 0 |
| H | GS002 | PanyPolicyMapping1to2CACert.crt | 0 |
| H | GS002 | PoliciesP1234CACert.crt | 0 |
| H | GS002 | PoliciesP1234subCAP123Cert.crt | 0 |
| H | GS002 | PoliciesP1234subsubCAP123P12Cert.crt | 0 |
| H | GS002 | PoliciesP123CACert.crt | 0 |
| H | GS002 | PoliciesP123subCAP12Cert.crt | 0 |
| H | GS002 | PoliciesP123subsubCAP12P1Cert.crt | 0 |
| H | GS002 | PoliciesP123subsubCAP12P2Cert.crt | 0 |
| H | GS002 | PoliciesP123subsubsubCAP12P2P1Cert.crt | 0 |
| H | GS002 | PoliciesP12CACert.crt | 0 |
| H | GS002 | PoliciesP12subCAP1Cert.crt | 0 |
| H | GS002 | PoliciesP12subsubCAP1P2Cert.crt | 0 |
| H | GS002 | PoliciesP2subCA2Cert.crt | 0 |
| H | GS002 | PoliciesP2subCACert.crt | 0 |
| H | GS002 | PoliciesP3CACert.crt | 0 |
| H | GS002 | RFC3280MandatoryAttributeTypesCACert.crt | 0 |
| H | GS002 | RFC3280OptionalAttributeTypesCACert.crt | 0 |
| H | GS002 | RevokedsubCACert.crt | 0 |
| H | GS002 | RolloverfromPrintableStringtoUTF8StringCACert.crt | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCA2CRLSigningCert.crt | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCA2CertificateSigningCACert.crt | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCRLSigningCert.crt | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCertificateSigningCACert.crt | 0 |
| H | GS002 | TrustAnchorRootCertificate.crt | 0 |
| H | GS002 | TwoCRLsCACert.crt | 0 |
| H | GS002 | UIDCACert.crt | 0 |
| H | GS002 | UTF8StringCaseInsensitiveMatchCACert.crt | 0 |
| H | GS002 | UTF8StringEncodedNamesCACert.crt | 0 |
| H | GS002 | UnknownCRLEntryExtensionCACert.crt | 0 |
| H | GS002 | UnknownCRLExtensionCACert.crt | 0 |
| H | GS002 | UserNoticeQualifierTest15EE.crt | 0 |
| H | GS002 | UserNoticeQualifierTest16EE.crt | 0 |
| H | GS002 | UserNoticeQualifierTest17EE.crt | 0 |
| H | GS002 | UserNoticeQualifierTest18EE.crt | 0 |
| H | GS002 | UserNoticeQualifierTest19EE.crt | 0 |
| H | GS002 | ValidBasicSelfIssuedCRLSigningKeyTest6EE.crt | 0 |
| H | GS002 | ValidBasicSelfIssuedNewWithOldTest3EE.crt | 0 |
| H | GS002 | ValidBasicSelfIssuedNewWithOldTest4EE.crt | 0 |
| H | GS002 | ValidBasicSelfIssuedOldWithNewTest1EE.crt | 0 |
| H | GS002 | ValidCertificatePathTest1EE.crt | 0 |
| H | GS002 | ValidDNSnameConstraintsTest30EE.crt | 0 |
| H | GS002 | ValidDNSnameConstraintsTest32EE.crt | 0 |
| H | GS002 | ValidDNandRFC822nameConstraintsTest27EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest11EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest14EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest18EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest19EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest1EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest4EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest5EE.crt | 0 |
| H | GS002 | ValidDNnameConstraintsTest6EE.crt | 0 |
| H | GS002 | ValidDSAParameterInheritanceTest5EE.crt | 0 |
| H | GS002 | ValidDSASignaturesTest4EE.crt | 0 |
| H | GS002 | ValidGeneralizedTimeCRLnextUpdateTest13EE.crt | 0 |
| H | GS002 | ValidGeneralizedTimenotAfterDateTest8EE.crt | 0 |
| H | GS002 | ValidGeneralizedTimenotBeforeDateTest4EE.crt | 0 |
| H | GS002 | ValidIDPwithindirectCRLTest22EE.crt | 0 |
| H | GS002 | ValidIDPwithindirectCRLTest24EE.crt | 0 |
| H | GS002 | ValidIDPwithindirectCRLTest25EE.crt | 0 |
| H | GS002 | ValidLongSerialNumberTest16EE.crt | 0 |
| H | GS002 | ValidLongSerialNumberTest17EE.crt | 0 |
| H | GS002 | ValidNameChainingCapitalizationTest5EE.crt | 0 |
| H | GS002 | ValidNameChainingWhitespaceTest3EE.crt | 0 |
| H | GS002 | ValidNameChainingWhitespaceTest4EE.crt | 0 |
| H | GS002 | ValidNameUIDsTest6EE.crt | 0 |
| H | GS002 | ValidNegativeSerialNumberTest14EE.crt | 0 |
| H | GS002 | ValidNoissuingDistributionPointTest10EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest11EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest12EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest13EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest14EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest1EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest3EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest5EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest6EE.crt | 0 |
| H | GS002 | ValidPolicyMappingTest9EE.crt | 0 |
| H | GS002 | ValidRFC3280MandatoryAttributeTypesTest7EE.crt | 0 |
| H | GS002 | ValidRFC3280OptionalAttributeTypesTest8EE.crt | 0 |
| H | GS002 | ValidRFC822nameConstraintsTest21EE.crt | 0 |
| H | GS002 | ValidRFC822nameConstraintsTest23EE.crt | 0 |
| H | GS002 | ValidRFC822nameConstraintsTest25EE.crt | 0 |
| H | GS002 | ValidRolloverfromPrintableStringtoUTF8StringTest10EE.crt | 0 |
| H | GS002 | ValidSelfIssuedinhibitAnyPolicyTest7EE.crt | 0 |
| H | GS002 | ValidSelfIssuedinhibitAnyPolicyTest9EE.crt | 0 |
| H | GS002 | ValidSelfIssuedinhibitPolicyMappingTest7EE.crt | 0 |
| H | GS002 | ValidSelfIssuedpathLenConstraintTest15EE.crt | 0 |
| H | GS002 | ValidSelfIssuedpathLenConstraintTest17EE.crt | 0 |
| H | GS002 | ValidSelfIssuedrequireExplicitPolicyTest6EE.crt | 0 |
| H | GS002 | ValidSeparateCertificateandCRLKeysTest19EE.crt | 0 |
| H | GS002 | ValidTwoCRLsTest7EE.crt | 0 |
| H | GS002 | ValidURInameConstraintsTest34EE.crt | 0 |
| H | GS002 | ValidURInameConstraintsTest36EE.crt | 0 |
| H | GS002 | ValidUTF8StringCaseInsensitiveMatchTest11EE.crt | 0 |
| H | GS002 | ValidUTF8StringEncodedNamesTest9EE.crt | 0 |
| H | GS002 | ValidUnknownNotCriticalCertificateExtensionTest1EE.crt | 0 |
| H | GS002 | ValidbasicConstraintsNotCriticalTest4EE.crt | 0 |
| H | GS002 | ValidcRLIssuerTest28EE.crt | 0 |
| H | GS002 | ValidcRLIssuerTest29EE.crt | 0 |
| H | GS002 | ValidcRLIssuerTest30EE.crt | 0 |
| H | GS002 | ValidcRLIssuerTest33EE.crt | 0 |
| H | GS002 | ValiddeltaCRLTest2EE.crt | 0 |
| H | GS002 | ValiddeltaCRLTest5EE.crt | 0 |
| H | GS002 | ValiddeltaCRLTest7EE.crt | 0 |
| H | GS002 | ValiddeltaCRLTest8EE.crt | 0 |
| H | GS002 | ValiddistributionPointTest1EE.crt | 0 |
| H | GS002 | ValiddistributionPointTest4EE.crt | 0 |
| H | GS002 | ValiddistributionPointTest5EE.crt | 0 |
| H | GS002 | ValiddistributionPointTest7EE.crt | 0 |
| H | GS002 | ValidinhibitAnyPolicyTest2EE.crt | 0 |
| H | GS002 | ValidinhibitPolicyMappingTest2EE.crt | 0 |
| H | GS002 | ValidinhibitPolicyMappingTest4EE.crt | 0 |
| H | GS002 | ValidkeyUsageNotCriticalTest3EE.crt | 0 |
| H | GS002 | ValidonlyContainsCACertsTest13EE.crt | 0 |
| H | GS002 | ValidonlySomeReasonsTest18EE.crt | 0 |
| H | GS002 | ValidonlySomeReasonsTest19EE.crt | 0 |
| H | GS002 | ValidpathLenConstraintTest13EE.crt | 0 |
| H | GS002 | ValidpathLenConstraintTest14EE.crt | 0 |
| H | GS002 | ValidpathLenConstraintTest7EE.crt | 0 |
| H | GS002 | ValidpathLenConstraintTest8EE.crt | 0 |
| H | GS002 | Validpre2000UTCnotBeforeDateTest3EE.crt | 0 |
| H | GS002 | ValidrequireExplicitPolicyTest1EE.crt | 0 |
| H | GS002 | ValidrequireExplicitPolicyTest2EE.crt | 0 |
| H | GS002 | ValidrequireExplicitPolicyTest4EE.crt | 0 |
| H | GS002 | WrongCRLCACert.crt | 0 |
| H | GS002 | anyPolicyCACert.crt | 0 |
| H | GS002 | basicConstraintsCriticalcAFalseCACert.crt | 0 |
| H | GS002 | basicConstraintsNotCriticalCACert.crt | 0 |
| H | GS002 | basicConstraintsNotCriticalcAFalseCACert.crt | 0 |
| H | GS002 | deltaCRLCA1Cert.crt | 0 |
| H | GS002 | deltaCRLCA2Cert.crt | 0 |
| H | GS002 | deltaCRLCA3Cert.crt | 0 |
| H | GS002 | deltaCRLIndicatorNoBaseCACert.crt | 0 |
| H | GS002 | distributionPoint1CACert.crt | 0 |
| H | GS002 | distributionPoint2CACert.crt | 0 |
| H | GS002 | indirectCRLCA1Cert.crt | 0 |
| H | GS002 | indirectCRLCA2Cert.crt | 0 |
| H | GS002 | indirectCRLCA3Cert.crt | 0 |
| H | GS002 | indirectCRLCA3cRLIssuerCert.crt | 0 |
| H | GS002 | indirectCRLCA4Cert.crt | 0 |
| H | GS002 | indirectCRLCA4cRLIssuerCert.crt | 0 |
| H | GS002 | indirectCRLCA5Cert.crt | 0 |
| H | GS002 | indirectCRLCA6Cert.crt | 0 |
| H | GS002 | inhibitAnyPolicy0CACert.crt | 0 |
| H | GS002 | inhibitAnyPolicy1CACert.crt | 0 |
| H | GS002 | inhibitAnyPolicy1SelfIssuedCACert.crt | 0 |
| H | GS002 | inhibitAnyPolicy1SelfIssuedsubCA2Cert.crt | 0 |
| H | GS002 | inhibitAnyPolicy1subCA1Cert.crt | 0 |
| H | GS002 | inhibitAnyPolicy1subCA2Cert.crt | 0 |
| H | GS002 | inhibitAnyPolicy1subCAIAP5Cert.crt | 0 |
| H | GS002 | inhibitAnyPolicy1subsubCA2Cert.crt | 0 |
| H | GS002 | inhibitAnyPolicy5CACert.crt | 0 |
| H | GS002 | inhibitAnyPolicy5subCACert.crt | 0 |
| H | GS002 | inhibitAnyPolicy5subsubCACert.crt | 0 |
| H | GS002 | inhibitAnyPolicyTest3EE.crt | 0 |
| H | GS002 | inhibitPolicyMapping0CACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping0subCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P12CACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P12subCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P12subCAIPM5Cert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P12subsubCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P12subsubCAIPM5Cert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P1CACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P1SelfIssuedCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P1SelfIssuedsubCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P1subCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping1P1subsubCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping5CACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping5subCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping5subsubCACert.crt | 0 |
| H | GS002 | inhibitPolicyMapping5subsubsubCACert.crt | 0 |
| H | GS002 | keyUsageCriticalcRLSignFalseCACert.crt | 0 |
| H | GS002 | keyUsageCriticalkeyCertSignFalseCACert.crt | 0 |
| H | GS002 | keyUsageNotCriticalCACert.crt | 0 |
| H | GS002 | keyUsageNotCriticalcRLSignFalseCACert.crt | 0 |
| H | GS002 | keyUsageNotCriticalkeyCertSignFalseCACert.crt | 0 |
| H | GS002 | nameConstraintsDN1CACert.crt | 0 |
| H | GS002 | nameConstraintsDN1SelfIssuedCACert.crt | 0 |
| H | GS002 | nameConstraintsDN1subCA1Cert.crt | 0 |
| H | GS002 | nameConstraintsDN1subCA2Cert.crt | 0 |
| H | GS002 | nameConstraintsDN1subCA3Cert.crt | 0 |
| H | GS002 | nameConstraintsDN2CACert.crt | 0 |
| H | GS002 | nameConstraintsDN3CACert.crt | 0 |
| H | GS002 | nameConstraintsDN3subCA1Cert.crt | 0 |
| H | GS002 | nameConstraintsDN3subCA2Cert.crt | 0 |
| H | GS002 | nameConstraintsDN4CACert.crt | 0 |
| H | GS002 | nameConstraintsDN5CACert.crt | 0 |
| H | GS002 | nameConstraintsDNS1CACert.crt | 0 |
| H | GS002 | nameConstraintsDNS2CACert.crt | 0 |
| H | GS002 | nameConstraintsRFC822CA1Cert.crt | 0 |
| H | GS002 | nameConstraintsRFC822CA2Cert.crt | 0 |
| H | GS002 | nameConstraintsRFC822CA3Cert.crt | 0 |
| H | GS002 | nameConstraintsURI1CACert.crt | 0 |
| H | GS002 | nameConstraintsURI2CACert.crt | 0 |
| H | GS002 | onlyContainsAttributeCertsCACert.crt | 0 |
| H | GS002 | onlyContainsCACertsCACert.crt | 0 |
| H | GS002 | onlyContainsUserCertsCACert.crt | 0 |
| H | GS002 | onlySomeReasonsCA1Cert.crt | 0 |
| H | GS002 | onlySomeReasonsCA2Cert.crt | 0 |
| H | GS002 | onlySomeReasonsCA3Cert.crt | 0 |
| H | GS002 | onlySomeReasonsCA4Cert.crt | 0 |
| H | GS002 | pathLenConstraint0CACert.crt | 0 |
| H | GS002 | pathLenConstraint0SelfIssuedCACert.crt | 0 |
| H | GS002 | pathLenConstraint0subCA2Cert.crt | 0 |
| H | GS002 | pathLenConstraint0subCACert.crt | 0 |
| H | GS002 | pathLenConstraint1CACert.crt | 0 |
| H | GS002 | pathLenConstraint1SelfIssuedCACert.crt | 0 |
| H | GS002 | pathLenConstraint1SelfIssuedsubCACert.crt | 0 |
| H | GS002 | pathLenConstraint1subCACert.crt | 0 |
| H | GS002 | pathLenConstraint6CACert.crt | 0 |
| H | GS002 | pathLenConstraint6subCA0Cert.crt | 0 |
| H | GS002 | pathLenConstraint6subCA1Cert.crt | 0 |
| H | GS002 | pathLenConstraint6subCA4Cert.crt | 0 |
| H | GS002 | pathLenConstraint6subsubCA00Cert.crt | 0 |
| H | GS002 | pathLenConstraint6subsubCA11Cert.crt | 0 |
| H | GS002 | pathLenConstraint6subsubCA41Cert.crt | 0 |
| H | GS002 | pathLenConstraint6subsubsubCA11XCert.crt | 0 |
| H | GS002 | pathLenConstraint6subsubsubCA41XCert.crt | 0 |
| H | GS002 | pre2000CRLnextUpdateCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy0CACert.crt | 0 |
| H | GS002 | requireExplicitPolicy0subCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy0subsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy0subsubsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy10CACert.crt | 0 |
| H | GS002 | requireExplicitPolicy10subCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy10subsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy10subsubsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy2CACert.crt | 0 |
| H | GS002 | requireExplicitPolicy2SelfIssuedCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy2SelfIssuedsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy2subCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy4CACert.crt | 0 |
| H | GS002 | requireExplicitPolicy4subCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy4subsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy4subsubsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy5CACert.crt | 0 |
| H | GS002 | requireExplicitPolicy5subCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy5subsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy5subsubsubCACert.crt | 0 |
| H | GS002 | requireExplicitPolicy7CACert.crt | 0 |
| H | GS002 | requireExplicitPolicy7subCARE2Cert.crt | 0 |
| H | GS002 | requireExplicitPolicy7subsubCARE2RE4Cert.crt | 0 |
| H | GS002 | requireExplicitPolicy7subsubsubCARE2RE4Cert.crt | 0 |
| H | GS002 | AllCertificatesNoPoliciesTest2EE.p12 | 0 |
| H | GS002 | AllCertificatesSamePoliciesTest10EE.p12 | 0 |
| H | GS002 | AllCertificatesSamePoliciesTest13EE.p12 | 0 |
| H | GS002 | AllCertificatesanyPolicyTest11EE.p12 | 0 |
| H | GS002 | AnyPolicyTest14EE.p12 | 0 |
| H | GS002 | BadCRLIssuerNameCACert.p12 | 0 |
| H | GS002 | BadCRLSignatureCACert.p12 | 0 |
| H | GS002 | BadSignedCACert.p12 | 0 |
| H | GS002 | BadnotAfterDateCACert.p12 | 0 |
| H | GS002 | BadnotBeforeDateCACert.p12 | 0 |
| H | GS002 | BasicSelfIssuedCRLSigningKeyCACert.p12 | 0 |
| H | GS002 | BasicSelfIssuedCRLSigningKeyCRLCert.p12 | 0 |
| H | GS002 | BasicSelfIssuedNewKeyCACert.p12 | 0 |
| H | GS002 | BasicSelfIssuedNewKeyOldWithNewCACert.p12 | 0 |
| H | GS002 | BasicSelfIssuedOldKeyCACert.p12 | 0 |
| H | GS002 | BasicSelfIssuedOldKeyNewWithOldCACert.p12 | 0 |
| H | GS002 | CPSPointerQualifierTest20EE.p12 | 0 |
| H | GS002 | DSACACert.p12 | 0 |
| H | GS002 | DSAParametersInheritedCACert.p12 | 0 |
| H | GS002 | DifferentPoliciesTest12EE.p12 | 0 |
| H | GS002 | DifferentPoliciesTest3EE.p12 | 0 |
| H | GS002 | DifferentPoliciesTest4EE.p12 | 0 |
| H | GS002 | DifferentPoliciesTest5EE.p12 | 0 |
| H | GS002 | DifferentPoliciesTest7EE.p12 | 0 |
| H | GS002 | DifferentPoliciesTest8EE.p12 | 0 |
| H | GS002 | DifferentPoliciesTest9EE.p12 | 0 |
| H | GS002 | GeneralizedTimeCRLnextUpdateCACert.p12 | 0 |
| H | GS002 | GoodCACert.p12 | 0 |
| H | GS002 | GoodsubCACert.p12 | 0 |
| H | GS002 | GoodsubCAPanyPolicyMapping1to2CACert.p12 | 0 |
| H | GS002 | InvalidBadCRLIssuerNameTest5EE.p12 | 0 |
| H | GS002 | InvalidBadCRLSignatureTest4EE.p12 | 0 |
| H | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest7EE.p12 | 0 |
| H | GS002 | InvalidBasicSelfIssuedCRLSigningKeyTest8EE.p12 | 0 |
| H | GS002 | InvalidBasicSelfIssuedNewWithOldTest5EE.p12 | 0 |
| H | GS002 | InvalidBasicSelfIssuedOldWithNewTest2EE.p12 | 0 |
| H | GS002 | InvalidCASignatureTest2EE.p12 | 0 |
| H | GS002 | InvalidCAnotAfterDateTest5EE.p12 | 0 |
| H | GS002 | InvalidCAnotBeforeDateTest1EE.p12 | 0 |
| H | GS002 | InvalidDNSnameConstraintsTest31EE.p12 | 0 |
| H | GS002 | InvalidDNSnameConstraintsTest33EE.p12 | 0 |
| H | GS002 | InvalidDNSnameConstraintsTest38EE.p12 | 0 |
| H | GS002 | InvalidDNandRFC822nameConstraintsTest28EE.p12 | 0 |
| H | GS002 | InvalidDNandRFC822nameConstraintsTest29EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest10EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest12EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest13EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest15EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest16EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest17EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest20EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest2EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest3EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest7EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest8EE.p12 | 0 |
| H | GS002 | InvalidDNnameConstraintsTest9EE.p12 | 0 |
| H | GS002 | InvalidDSASignatureTest6EE.p12 | 0 |
| H | GS002 | InvalidEESignatureTest3EE.p12 | 0 |
| H | GS002 | InvalidEEnotAfterDateTest6EE.p12 | 0 |
| H | GS002 | InvalidEEnotBeforeDateTest2EE.p12 | 0 |
| H | GS002 | InvalidIDPwithindirectCRLTest23EE.p12 | 0 |
| H | GS002 | InvalidIDPwithindirectCRLTest26EE.p12 | 0 |
| H | GS002 | InvalidLongSerialNumberTest18EE.p12 | 0 |
| H | GS002 | InvalidMappingFromanyPolicyTest7EE.p12 | 0 |
| H | GS002 | InvalidMappingToanyPolicyTest8EE.p12 | 0 |
| H | GS002 | InvalidMissingCRLTest1EE.p12 | 0 |
| H | GS002 | InvalidMissingbasicConstraintsTest1EE.p12 | 0 |
| H | GS002 | InvalidNameChainingOrderTest2EE.p12 | 0 |
| H | GS002 | InvalidNameChainingTest1EE.p12 | 0 |
| H | GS002 | InvalidNegativeSerialNumberTest15EE.p12 | 0 |
| H | GS002 | InvalidOldCRLnextUpdateTest11EE.p12 | 0 |
| H | GS002 | InvalidPolicyMappingTest10EE.p12 | 0 |
| H | GS002 | InvalidPolicyMappingTest2EE.p12 | 0 |
| H | GS002 | InvalidPolicyMappingTest4EE.p12 | 0 |
| H | GS002 | InvalidRFC822nameConstraintsTest22EE.p12 | 0 |
| H | GS002 | InvalidRFC822nameConstraintsTest24EE.p12 | 0 |
| H | GS002 | InvalidRFC822nameConstraintsTest26EE.p12 | 0 |
| H | GS002 | InvalidRevokedCATest2EE.p12 | 0 |
| H | GS002 | InvalidRevokedEETest3EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest10EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedinhibitAnyPolicyTest8EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest10EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest11EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest8EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedinhibitPolicyMappingTest9EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedpathLenConstraintTest16EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest7EE.p12 | 0 |
| H | GS002 | InvalidSelfIssuedrequireExplicitPolicyTest8EE.p12 | 0 |
| H | GS002 | InvalidSeparateCertificateandCRLKeysTest20EE.p12 | 0 |
| H | GS002 | InvalidSeparateCertificateandCRLKeysTest21EE.p12 | 0 |
| H | GS002 | InvalidURInameConstraintsTest35EE.p12 | 0 |
| H | GS002 | InvalidURInameConstraintsTest37EE.p12 | 0 |
| H | GS002 | InvalidUnknownCRLEntryExtensionTest8EE.p12 | 0 |
| H | GS002 | InvalidUnknownCRLExtensionTest10EE.p12 | 0 |
| H | GS002 | InvalidUnknownCRLExtensionTest9EE.p12 | 0 |
| H | GS002 | InvalidUnknownCriticalCertificateExtensionTest2EE.p12 | 0 |
| H | GS002 | InvalidWrongCRLTest6EE.p12 | 0 |
| H | GS002 | InvalidcAFalseTest2EE.p12 | 0 |
| H | GS002 | InvalidcAFalseTest3EE.p12 | 0 |
| H | GS002 | InvalidcRLIssuerTest27EE.p12 | 0 |
| H | GS002 | InvalidcRLIssuerTest31EE.p12 | 0 |
| H | GS002 | InvalidcRLIssuerTest32EE.p12 | 0 |
| H | GS002 | InvalidcRLIssuerTest34EE.p12 | 0 |
| H | GS002 | InvalidcRLIssuerTest35EE.p12 | 0 |
| H | GS002 | InvaliddeltaCRLIndicatorNoBaseTest1EE.p12 | 0 |
| H | GS002 | InvaliddeltaCRLTest10EE.p12 | 0 |
| H | GS002 | InvaliddeltaCRLTest3EE.p12 | 0 |
| H | GS002 | InvaliddeltaCRLTest4EE.p12 | 0 |
| H | GS002 | InvaliddeltaCRLTest6EE.p12 | 0 |
| H | GS002 | InvaliddeltaCRLTest9EE.p12 | 0 |
| H | GS002 | InvaliddistributionPointTest2EE.p12 | 0 |
| H | GS002 | InvaliddistributionPointTest3EE.p12 | 0 |
| H | GS002 | InvaliddistributionPointTest6EE.p12 | 0 |
| H | GS002 | InvaliddistributionPointTest8EE.p12 | 0 |
| H | GS002 | InvaliddistributionPointTest9EE.p12 | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest1EE.p12 | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest4EE.p12 | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest5EE.p12 | 0 |
| H | GS002 | InvalidinhibitAnyPolicyTest6EE.p12 | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest1EE.p12 | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest3EE.p12 | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest5EE.p12 | 0 |
| H | GS002 | InvalidinhibitPolicyMappingTest6EE.p12 | 0 |
| H | GS002 | InvalidkeyUsageCriticalcRLSignFalseTest4EE.p12 | 0 |
| H | GS002 | InvalidkeyUsageCriticalkeyCertSignFalseTest1EE.p12 | 0 |
| H | GS002 | InvalidkeyUsageNotCriticalcRLSignFalseTest5EE.p12 | 0 |
| H | GS002 | InvalidkeyUsageNotCriticalkeyCertSignFalseTest2EE.p12 | 0 |
| H | GS002 | InvalidonlyContainsAttributeCertsTest14EE.p12 | 0 |
| H | GS002 | InvalidonlyContainsCACertsTest12EE.p12 | 0 |
| H | GS002 | InvalidonlyContainsUserCertsTest11EE.p12 | 0 |
| H | GS002 | InvalidonlySomeReasonsTest15EE.p12 | 0 |
| H | GS002 | InvalidonlySomeReasonsTest16EE.p12 | 0 |
| H | GS002 | InvalidonlySomeReasonsTest17EE.p12 | 0 |
| H | GS002 | InvalidonlySomeReasonsTest20EE.p12 | 0 |
| H | GS002 | InvalidonlySomeReasonsTest21EE.p12 | 0 |
| H | GS002 | InvalidpathLenConstraintTest10EE.p12 | 0 |
| H | GS002 | InvalidpathLenConstraintTest11EE.p12 | 0 |
| H | GS002 | InvalidpathLenConstraintTest12EE.p12 | 0 |
| H | GS002 | InvalidpathLenConstraintTest5EE.p12 | 0 |
| H | GS002 | InvalidpathLenConstraintTest6EE.p12 | 0 |
| H | GS002 | InvalidpathLenConstraintTest9EE.p12 | 0 |
| H | GS002 | Invalidpre2000CRLnextUpdateTest12EE.p12 | 0 |
| H | GS002 | Invalidpre2000UTCEEnotAfterDateTest7EE.p12 | 0 |
| H | GS002 | InvalidrequireExplicitPolicyTest3EE.p12 | 0 |
| H | GS002 | InvalidrequireExplicitPolicyTest5EE.p12 | 0 |
| H | GS002 | LongSerialNumberCACert.p12 | 0 |
| H | GS002 | Mapping1to2CACert.p12 | 0 |
| H | GS002 | MappingFromanyPolicyCACert.p12 | 0 |
| H | GS002 | MappingToanyPolicyCACert.p12 | 0 |
| H | GS002 | MissingbasicConstraintsCACert.p12 | 0 |
| H | GS002 | NameOrderingCACert.p12 | 0 |
| H | GS002 | NegativeSerialNumberCACert.p12 | 0 |
| H | GS002 | NoCRLCACert.p12 | 0 |
| H | GS002 | NoPoliciesCACert.p12 | 0 |
| H | GS002 | NoissuingDistributionPointCACert.p12 | 0 |
| H | GS002 | OldCRLnextUpdateCACert.p12 | 0 |
| H | GS002 | OverlappingPoliciesTest6EE.p12 | 0 |
| H | GS002 | P12Mapping1to3CACert.p12 | 0 |
| H | GS002 | P12Mapping1to3subCACert.p12 | 0 |
| H | GS002 | P12Mapping1to3subsubCACert.p12 | 0 |
| H | GS002 | P1Mapping1to234CACert.p12 | 0 |
| H | GS002 | P1Mapping1to234subCACert.p12 | 0 |
| H | GS002 | P1anyPolicyMapping1to2CACert.p12 | 0 |
| H | GS002 | PanyPolicyMapping1to2CACert.p12 | 0 |
| H | GS002 | PoliciesP1234CACert.p12 | 0 |
| H | GS002 | PoliciesP1234subCAP123Cert.p12 | 0 |
| H | GS002 | PoliciesP1234subsubCAP123P12Cert.p12 | 0 |
| H | GS002 | PoliciesP123CACert.p12 | 0 |
| H | GS002 | PoliciesP123subCAP12Cert.p12 | 0 |
| H | GS002 | PoliciesP123subsubCAP12P1Cert.p12 | 0 |
| H | GS002 | PoliciesP123subsubCAP12P2Cert.p12 | 0 |
| H | GS002 | PoliciesP123subsubsubCAP12P2P1Cert.p12 | 0 |
| H | GS002 | PoliciesP12CACert.p12 | 0 |
| H | GS002 | PoliciesP12subCAP1Cert.p12 | 0 |
| H | GS002 | PoliciesP12subsubCAP1P2Cert.p12 | 0 |
| H | GS002 | PoliciesP2subCA2Cert.p12 | 0 |
| H | GS002 | PoliciesP2subCACert.p12 | 0 |
| H | GS002 | PoliciesP3CACert.p12 | 0 |
| H | GS002 | RFC3280MandatoryAttributeTypesCACert.p12 | 0 |
| H | GS002 | RFC3280OptionalAttributeTypesCACert.p12 | 0 |
| H | GS002 | RevokedsubCACert.p12 | 0 |
| H | GS002 | RolloverfromPrintableStringtoUTF8StringCACert.p12 | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCA2CRLSigningCert.p12 | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCA2CertificateSigningCACert.p12 | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCRLSigningCert.p12 | 0 |
| H | GS002 | SeparateCertificateandCRLKeysCertificateSigningCACert.p12 | 0 |
| H | GS002 | TrustAnchorRootCertificate.p12 | 0 |
| H | GS002 | TwoCRLsCACert.p12 | 0 |
| H | GS002 | UIDCACert.p12 | 0 |
| H | GS002 | UTF8StringCaseInsensitiveMatchCACert.p12 | 0 |
| H | GS002 | UTF8StringEncodedNamesCACert.p12 | 0 |
| H | GS002 | UnknownCRLEntryExtensionCACert.p12 | 0 |
| H | GS002 | UnknownCRLExtensionCACert.p12 | 0 |
| H | GS002 | UserNoticeQualifierTest15EE.p12 | 0 |
| H | GS002 | UserNoticeQualifierTest16EE.p12 | 0 |
| H | GS002 | UserNoticeQualifierTest17EE.p12 | 0 |
| H | GS002 | UserNoticeQualifierTest18EE.p12 | 0 |
| H | GS002 | UserNoticeQualifierTest19EE.p12 | 0 |
| H | GS002 | ValidBasicSelfIssuedCRLSigningKeyTest6EE.p12 | 0 |
| H | GS002 | ValidBasicSelfIssuedNewWithOldTest3EE.p12 | 0 |
| H | GS002 | ValidBasicSelfIssuedNewWithOldTest4EE.p12 | 0 |
| H | GS002 | ValidBasicSelfIssuedOldWithNewTest1EE.p12 | 0 |
| H | GS002 | ValidCertificatePathTest1EE.p12 | 0 |
| H | GS002 | ValidDNSnameConstraintsTest30EE.p12 | 0 |
| H | GS002 | ValidDNSnameConstraintsTest32EE.p12 | 0 |
| H | GS002 | ValidDNandRFC822nameConstraintsTest27EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest11EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest14EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest18EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest19EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest1EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest4EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest5EE.p12 | 0 |
| H | GS002 | ValidDNnameConstraintsTest6EE.p12 | 0 |
| H | GS002 | ValidDSAParameterInheritanceTest5EE.p12 | 0 |
| H | GS002 | ValidDSASignaturesTest4EE.p12 | 0 |
| H | GS002 | ValidGeneralizedTimeCRLnextUpdateTest13EE.p12 | 0 |
| H | GS002 | ValidGeneralizedTimenotAfterDateTest8EE.p12 | 0 |
| H | GS002 | ValidGeneralizedTimenotBeforeDateTest4EE.p12 | 0 |
| H | GS002 | ValidIDPwithindirectCRLTest22EE.p12 | 0 |
| H | GS002 | ValidIDPwithindirectCRLTest24EE.p12 | 0 |
| H | GS002 | ValidIDPwithindirectCRLTest25EE.p12 | 0 |
| H | GS002 | ValidLongSerialNumberTest16EE.p12 | 0 |
| H | GS002 | ValidLongSerialNumberTest17EE.p12 | 0 |
| H | GS002 | ValidNameChainingCapitalizationTest5EE.p12 | 0 |
| H | GS002 | ValidNameChainingWhitespaceTest3EE.p12 | 0 |
| H | GS002 | ValidNameChainingWhitespaceTest4EE.p12 | 0 |
| H | GS002 | ValidNameUIDsTest6EE.p12 | 0 |
| H | GS002 | ValidNegativeSerialNumberTest14EE.p12 | 0 |
| H | GS002 | ValidNoissuingDistributionPointTest10EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest11EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest12EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest13EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest14EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest1EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest3EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest5EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest6EE.p12 | 0 |
| H | GS002 | ValidPolicyMappingTest9EE.p12 | 0 |
| H | GS002 | ValidRFC3280MandatoryAttributeTypesTest7EE.p12 | 0 |
| H | GS002 | ValidRFC3280OptionalAttributeTypesTest8EE.p12 | 0 |
| H | GS002 | ValidRFC822nameConstraintsTest21EE.p12 | 0 |
| H | GS002 | ValidRFC822nameConstraintsTest23EE.p12 | 0 |
| H | GS002 | ValidRFC822nameConstraintsTest25EE.p12 | 0 |
| H | GS002 | ValidRolloverfromPrintableStringtoUTF8StringTest10EE.p12 | 0 |
| H | GS002 | ValidSelfIssuedinhibitAnyPolicyTest7EE.p12 | 0 |
| H | GS002 | ValidSelfIssuedinhibitAnyPolicyTest9EE.p12 | 0 |
| H | GS002 | ValidSelfIssuedinhibitPolicyMappingTest7EE.p12 | 0 |
| H | GS002 | ValidSelfIssuedpathLenConstraintTest15EE.p12 | 0 |
| H | GS002 | ValidSelfIssuedpathLenConstraintTest17EE.p12 | 0 |
| H | GS002 | ValidSelfIssuedrequireExplicitPolicyTest6EE.p12 | 0 |
| H | GS002 | ValidSeparateCertificateandCRLKeysTest19EE.p12 | 0 |
| H | GS002 | ValidTwoCRLsTest7EE.p12 | 0 |
| H | GS002 | ValidURInameConstraintsTest34EE.p12 | 0 |
| H | GS002 | ValidURInameConstraintsTest36EE.p12 | 0 |
| H | GS002 | ValidUTF8StringCaseInsensitiveMatchTest11EE.p12 | 0 |
| H | GS002 | ValidUTF8StringEncodedNamesTest9EE.p12 | 0 |
| H | GS002 | ValidUnknownNotCriticalCertificateExtensionTest1EE.p12 | 0 |
| H | GS002 | ValidbasicConstraintsNotCriticalTest4EE.p12 | 0 |
| H | GS002 | ValidcRLIssuerTest28EE.p12 | 0 |
| H | GS002 | ValidcRLIssuerTest29EE.p12 | 0 |
| H | GS002 | ValidcRLIssuerTest30EE.p12 | 0 |
| H | GS002 | ValidcRLIssuerTest33EE.p12 | 0 |
| H | GS002 | ValiddeltaCRLTest2EE.p12 | 0 |
| H | GS002 | ValiddeltaCRLTest5EE.p12 | 0 |
| H | GS002 | ValiddeltaCRLTest7EE.p12 | 0 |
| H | GS002 | ValiddeltaCRLTest8EE.p12 | 0 |
| H | GS002 | ValiddistributionPointTest1EE.p12 | 0 |
| H | GS002 | ValiddistributionPointTest4EE.p12 | 0 |
| H | GS002 | ValiddistributionPointTest5EE.p12 | 0 |
| H | GS002 | ValiddistributionPointTest7EE.p12 | 0 |
| H | GS002 | ValidinhibitAnyPolicyTest2EE.p12 | 0 |
| H | GS002 | ValidinhibitPolicyMappingTest2EE.p12 | 0 |
| H | GS002 | ValidinhibitPolicyMappingTest4EE.p12 | 0 |
| H | GS002 | ValidkeyUsageNotCriticalTest3EE.p12 | 0 |
| H | GS002 | ValidonlyContainsCACertsTest13EE.p12 | 0 |
| H | GS002 | ValidonlySomeReasonsTest18EE.p12 | 0 |
| H | GS002 | ValidonlySomeReasonsTest19EE.p12 | 0 |
| H | GS002 | ValidpathLenConstraintTest13EE.p12 | 0 |
| H | GS002 | ValidpathLenConstraintTest14EE.p12 | 0 |
| H | GS002 | ValidpathLenConstraintTest7EE.p12 | 0 |
| H | GS002 | ValidpathLenConstraintTest8EE.p12 | 0 |
| H | GS002 | Validpre2000UTCnotBeforeDateTest3EE.p12 | 0 |
| H | GS002 | ValidrequireExplicitPolicyTest1EE.p12 | 0 |
| H | GS002 | ValidrequireExplicitPolicyTest2EE.p12 | 0 |
| H | GS002 | ValidrequireExplicitPolicyTest4EE.p12 | 0 |
| H | GS002 | WrongCRLCACert.p12 | 0 |
| H | GS002 | anyPolicyCACert.p12 | 0 |
| H | GS002 | basicConstraintsCriticalcAFalseCACert.p12 | 0 |
| H | GS002 | basicConstraintsNotCriticalCACert.p12 | 0 |
| H | GS002 | basicConstraintsNotCriticalcAFalseCACert.p12 | 0 |
| H | GS002 | deltaCRLCA1Cert.p12 | 0 |
| H | GS002 | deltaCRLCA2Cert.p12 | 0 |
| H | GS002 | deltaCRLCA3Cert.p12 | 0 |
| H | GS002 | deltaCRLIndicatorNoBaseCACert.p12 | 0 |
| H | GS002 | distributionPoint1CACert.p12 | 0 |
| H | GS002 | distributionPoint2CACert.p12 | 0 |
| H | GS002 | indirectCRLCA1Cert.p12 | 0 |
| H | GS002 | indirectCRLCA2Cert.p12 | 0 |
| H | GS002 | indirectCRLCA3Cert.p12 | 0 |
| H | GS002 | indirectCRLCA3cRLIssuerCert.p12 | 0 |
| H | GS002 | indirectCRLCA4Cert.p12 | 0 |
| H | GS002 | indirectCRLCA4cRLIssuerCert.p12 | 0 |
| H | GS002 | indirectCRLCA5Cert.p12 | 0 |
| H | GS002 | indirectCRLCA6Cert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy0CACert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy1CACert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy1SelfIssuedCACert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy1SelfIssuedsubCA2Cert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy1subCA1Cert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy1subCA2Cert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy1subCAIAP5Cert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy1subsubCA2Cert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy5CACert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy5subCACert.p12 | 0 |
| H | GS002 | inhibitAnyPolicy5subsubCACert.p12 | 0 |
| H | GS002 | inhibitAnyPolicyTest3EE.p12 | 0 |
| H | GS002 | inhibitPolicyMapping0CACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping0subCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P12CACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P12subCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P12subCAIPM5Cert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P12subsubCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P12subsubCAIPM5Cert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P1CACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P1SelfIssuedCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P1SelfIssuedsubCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P1subCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping1P1subsubCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping5CACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping5subCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping5subsubCACert.p12 | 0 |
| H | GS002 | inhibitPolicyMapping5subsubsubCACert.p12 | 0 |
| H | GS002 | keyUsageCriticalcRLSignFalseCACert.p12 | 0 |
| H | GS002 | keyUsageCriticalkeyCertSignFalseCACert.p12 | 0 |
| H | GS002 | keyUsageNotCriticalCACert.p12 | 0 |
| H | GS002 | keyUsageNotCriticalcRLSignFalseCACert.p12 | 0 |
| H | GS002 | keyUsageNotCriticalkeyCertSignFalseCACert.p12 | 0 |
| H | GS002 | nameConstraintsDN1CACert.p12 | 0 |
| H | GS002 | nameConstraintsDN1SelfIssuedCACert.p12 | 0 |
| H | GS002 | nameConstraintsDN1subCA1Cert.p12 | 0 |
| H | GS002 | nameConstraintsDN1subCA2Cert.p12 | 0 |
| H | GS002 | nameConstraintsDN1subCA3Cert.p12 | 0 |
| H | GS002 | nameConstraintsDN2CACert.p12 | 0 |
| H | GS002 | nameConstraintsDN3CACert.p12 | 0 |
| H | GS002 | nameConstraintsDN3subCA1Cert.p12 | 0 |
| H | GS002 | nameConstraintsDN3subCA2Cert.p12 | 0 |
| H | GS002 | nameConstraintsDN4CACert.p12 | 0 |
| H | GS002 | nameConstraintsDN5CACert.p12 | 0 |
| H | GS002 | nameConstraintsDNS1CACert.p12 | 0 |
| H | GS002 | nameConstraintsDNS2CACert.p12 | 0 |
| H | GS002 | nameConstraintsRFC822CA1Cert.p12 | 0 |
| H | GS002 | nameConstraintsRFC822CA2Cert.p12 | 0 |
| H | GS002 | nameConstraintsRFC822CA3Cert.p12 | 0 |
| H | GS002 | nameConstraintsURI1CACert.p12 | 0 |
| H | GS002 | nameConstraintsURI2CACert.p12 | 0 |
| H | GS002 | onlyContainsAttributeCertsCACert.p12 | 0 |
| H | GS002 | onlyContainsCACertsCACert.p12 | 0 |
| H | GS002 | onlyContainsUserCertsCACert.p12 | 0 |
| H | GS002 | onlySomeReasonsCA1Cert.p12 | 0 |
| H | GS002 | onlySomeReasonsCA2Cert.p12 | 0 |
| H | GS002 | onlySomeReasonsCA3Cert.p12 | 0 |
| H | GS002 | onlySomeReasonsCA4Cert.p12 | 0 |
| H | GS002 | pathLenConstraint0CACert.p12 | 0 |
| H | GS002 | pathLenConstraint0SelfIssuedCACert.p12 | 0 |
| H | GS002 | pathLenConstraint0subCA2Cert.p12 | 0 |
| H | GS002 | pathLenConstraint0subCACert.p12 | 0 |
| H | GS002 | pathLenConstraint1CACert.p12 | 0 |
| H | GS002 | pathLenConstraint1SelfIssuedCACert.p12 | 0 |
| H | GS002 | pathLenConstraint1SelfIssuedsubCACert.p12 | 0 |
| H | GS002 | pathLenConstraint1subCACert.p12 | 0 |
| H | GS002 | pathLenConstraint6CACert.p12 | 0 |
| H | GS002 | pathLenConstraint6subCA0Cert.p12 | 0 |
| H | GS002 | pathLenConstraint6subCA1Cert.p12 | 0 |
| H | GS002 | pathLenConstraint6subCA4Cert.p12 | 0 |
| H | GS002 | pathLenConstraint6subsubCA00Cert.p12 | 0 |
| H | GS002 | pathLenConstraint6subsubCA11Cert.p12 | 0 |
| H | GS002 | pathLenConstraint6subsubCA41Cert.p12 | 0 |
| H | GS002 | pathLenConstraint6subsubsubCA11XCert.p12 | 0 |
| H | GS002 | pathLenConstraint6subsubsubCA41XCert.p12 | 0 |
| H | GS002 | pre2000CRLnextUpdateCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy0CACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy0subCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy0subsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy0subsubsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy10CACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy10subCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy10subsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy10subsubsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy2CACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy2SelfIssuedCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy2SelfIssuedsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy2subCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy4CACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy4subCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy4subsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy4subsubsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy5CACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy5subCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy5subsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy5subsubsubCACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy7CACert.p12 | 0 |
| H | GS002 | requireExplicitPolicy7subCARE2Cert.p12 | 0 |
| H | GS002 | requireExplicitPolicy7subsubCARE2RE4Cert.p12 | 0 |
| H | GS002 | requireExplicitPolicy7subsubsubCARE2RE4Cert.p12 | 0 |
| H | GS002 | accvraiz1.pem | 0 |
| H | GS002 | badasn1time.pem | 0 |
| H | GS002 | badssl-sct.pem | 0 |
| H | GS002 | belgian-eid-invalid-visiblestring.pem | 0 |
| H | GS002 | bigoid.pem | 0 |
| H | GS002 | cryptography-scts.pem | 0 |
| H | GS002 | cryptography.io.chain.pem | 0 |
| H | GS002 | cryptography.io.chain_with_garbage.pem | 0 |
| H | GS002 | cryptography.io.old_header.pem | 0 |
| H | GS002 | cryptography.io.pem | 0 |
| H | GS002 | cryptography.io.precert.pem | 0 |
| H | GS002 | cryptography.io.with_garbage.pem | 0 |
| H | GS002 | cryptography.io.with_headers.pem | 0 |
| H | GS002 | admissions_extension_authority_not_provided.pem | 0 |
| H | GS002 | admissions_extension_optional_data_not_provided.pem | 0 |
| H | GS002 | aia_ca_issuers.pem | 0 |
| H | GS002 | aia_ocsp.pem | 0 |
| H | GS002 | aia_ocsp_ca_issuers.pem | 0 |
| H | GS002 | all_key_usages.pem | 0 |
| H | GS002 | all_supported_names.pem | 0 |
| H | GS002 | authority_key_identifier.pem | 0 |
| H | GS002 | authority_key_identifier_no_keyid.pem | 0 |
| H | GS002 | bad_country.pem | 0 |
| H | GS002 | basic_constraints_not_critical.pem | 0 |
| H | GS002 | bc_path_length_zero.pem | 0 |
| H | GS002 | ca.pem | 0 |
| H | GS002 | ca_key.pem | 0 |
| H | GS002 | rsa_ca.pem | 0 |
| H | GS002 | rsa_key.pem | 0 |
| H | GS002 | rsae_ca.pem | 0 |
| H | GS002 | cdp_all_reasons.pem | 0 |
| H | GS002 | cdp_crl_issuer.pem | 0 |
| H | GS002 | cdp_empty_hostname.pem | 0 |
| H | GS002 | cdp_fullname_reasons_crl_issuer.pem | 0 |
| H | GS002 | cdp_reason_aa_compromise.pem | 0 |
| H | GS002 | cp_cps_uri.pem | 0 |
| H | GS002 | cp_invalid.pem | 0 |
| H | GS002 | cp_user_notice_no_explicit_text.pem | 0 |
| H | GS002 | cp_user_notice_with_explicit_text.pem | 0 |
| H | GS002 | cp_user_notice_with_notice_reference.pem | 0 |
| H | GS002 | crl_all_reasons.pem | 0 |
| H | GS002 | crl_almost_10k.pem | 0 |
| H | GS002 | crl_bad_version.pem | 0 |
| H | GS002 | crl_delta_crl_indicator.pem | 0 |
| H | GS002 | crl_dup_entry_ext.pem | 0 |
| H | GS002 | crl_empty.pem | 0 |
| H | GS002 | crl_ian_aia_aki.pem | 0 |
| H | GS002 | crl_idp_fullname_indirect_crl.pem | 0 |
| H | GS002 | crl_idp_fullname_only.pem | 0 |
| H | GS002 | crl_idp_fullname_only_aa.pem | 0 |
| H | GS002 | crl_idp_fullname_only_user.pem | 0 |
| H | GS002 | crl_idp_only_ca.pem | 0 |
| H | GS002 | crl_idp_reasons_only.pem | 0 |
| H | GS002 | crl_idp_relative_user_all_reasons.pem | 0 |
| H | GS002 | crl_idp_relativename_only.pem | 0 |
| H | GS002 | crl_inval_cert_issuer_entry_ext.pem | 0 |
| H | GS002 | crl_md2_unknown_crit_entry_ext.pem | 0 |
| H | GS002 | crl_no_next_update.pem | 0 |
| H | GS002 | crl_unsupported_reason.pem | 0 |
| H | GS002 | dsa_null_alg_params.pem | 0 |
| H | GS002 | dsa_selfsigned_ca.pem | 0 |
| H | GS002 | ec_no_named_curve.pem | 0 |
| H | GS002 | ecdsa_null_alg.pem | 0 |
| H | GS002 | ekucrit-testuser-cert.pem | 0 |
| H | GS002 | empty-eku.pem | 0 |
| H | GS002 | extended_key_usage.pem | 0 |
| H | GS002 | freshestcrl.pem | 0 |
| H | GS002 | ian_uri.pem | 0 |
| H | GS002 | inhibit_any_policy_5.pem | 0 |
| H | GS002 | inhibit_any_policy_negative.pem | 0 |
| H | GS002 | invalid_signature_cert.pem | 0 |
| H | GS002 | invalid_signature_crl.pem | 0 |
| H | GS002 | invalid_utf8_common_name.pem | 0 |
| H | GS002 | invalid_version.pem | 0 |
| H | GS002 | long-form-name-attribute.pem | 0 |
| H | GS002 | malformed-ian.pem | 0 |
| H | GS002 | malformed-san.pem | 0 |
| H | GS002 | ms-certificate-template.pem | 0 |
| H | GS002 | name_attribute_unsupported_tag.pem | 0 |
| H | GS002 | nc_excluded.pem | 0 |
| H | GS002 | nc_invalid_ip_netmask.pem | 0 |
| H | GS002 | nc_ip_invalid_length.pem | 0 |
| H | GS002 | nc_permitted.pem | 0 |
| H | GS002 | nc_permitted_2.pem | 0 |
| H | GS002 | nc_permitted_excluded.pem | 0 |
| H | GS002 | nc_permitted_excluded_2.pem | 0 |
| H | GS002 | nc_single_ip_netmask.pem | 0 |
| H | GS002 | negative_serial.pem | 0 |
| H | GS002 | no_sans.pem | 0 |
| H | GS002 | ocsp_nocheck.pem | 0 |
| H | GS002 | pc_inhibit.pem | 0 |
| H | GS002 | pc_inhibit_require.pem | 0 |
| H | GS002 | pc_require.pem | 0 |
| H | GS002 | policy_constraints_explicit.pem | 0 |
| H | GS002 | post2000utctime.pem | 0 |
| H | GS002 | private_key_usage_period_both_dates.pem | 0 |
| H | GS002 | private_key_usage_period_only_not_after.pem | 0 |
| H | GS002 | private_key_usage_period_only_not_before.pem | 0 |
| H | GS002 | rsa_pss.pem | 0 |
| H | GS002 | rsa_pss_cert.pem | 0 |
| H | GS002 | rsa_pss_sha256_no_null.pem | 0 |
| H | GS002 | san_dirname.pem | 0 |
| H | GS002 | san_email_dns_ip_dirname_uri.pem | 0 |
| H | GS002 | san_empty_hostname.pem | 0 |
| H | GS002 | san_idna2003_dnsname.pem | 0 |
| H | GS002 | san_idna_names.pem | 0 |
| H | GS002 | san_ipaddr.pem | 0 |
| H | GS002 | san_other_name.pem | 0 |
| H | GS002 | san_registered_id.pem | 0 |
| H | GS002 | san_rfc822_idna.pem | 0 |
| H | GS002 | san_rfc822_names.pem | 0 |
| H | GS002 | san_uri_with_port.pem | 0 |
| H | GS002 | san_wildcard_idna.pem | 0 |
| H | GS002 | sia.pem | 0 |
| H | GS002 | two_basic_constraints.pem | 0 |
| H | GS002 | unsupported_extension.pem | 0 |
| H | GS002 | unsupported_extension_2.pem | 0 |
| H | GS002 | unsupported_extension_critical.pem | 0 |
| H | GS002 | unsupported_subject_name.pem | 0 |
| H | GS002 | unsupported_subject_public_key_info.pem | 0 |
| H | GS002 | utf8_common_name.pem | 0 |
| H | GS002 | valid_signature_cert.pem | 0 |
| H | GS002 | valid_signature_crl.pem | 0 |
| H | GS002 | department-of-state-root.pem | 0 |
| H | GS002 | ecdsa_root.pem | 0 |
| H | GS002 | ed25519-rfc8410.pem | 0 |
| H | GS002 | root-ed25519.pem | 0 |
| H | GS002 | server-ed25519-cert.pem | 0 |
| H | GS002 | root-ed448.pem | 0 |
| H | GS002 | server-ed448-cert.pem | 0 |
| H | GS002 | ee-pss-sha1-cert.pem | 0 |
| H | GS002 | letsencryptx3.pem | 0 |
| H | GS002 | rapidssl_sha256_ca_g3.pem | 0 |
| H | GS002 | bad-version.pem | 0 |
| H | GS002 | basic_constraints.pem | 0 |
| H | GS002 | challenge-unstructured.pem | 0 |
| H | GS002 | challenge.pem | 0 |
| H | GS002 | dsa_sha1.pem | 0 |
| H | GS002 | ec_sha256.pem | 0 |
| H | GS002 | ec_sha256_old_header.pem | 0 |
| H | GS002 | freeipa-bad-critical.pem | 0 |
| H | GS002 | invalid_signature.pem | 0 |
| H | GS002 | long-form-attribute.pem | 0 |
| H | GS002 | rsa_md4.pem | 0 |
| H | GS002 | rsa_sha1.pem | 0 |
| H | GS002 | rsa_sha256.pem | 0 |
| H | GS002 | san_rsa_sha1.pem | 0 |
| H | GS002 | two_basic_constraints.pem | 0 |
| H | GS002 | unsupported_extension.pem | 0 |
| H | GS002 | unsupported_extension_critical.pem | 0 |
| H | GS002 | zero-element-attribute.pem | 0 |
| H | GS002 | scottishpower-bitstring-dn.pem | 0 |
| H | GS002 | tls-feature-ocsp-staple.pem | 0 |
| H | GS002 | unique_identifier.pem | 0 |
| H | GS002 | utf8-dnsname.pem | 0 |
| H | GS002 | v1_cert.pem | 0 |
| H | GS002 | verisign_md2_root.pem | 0 |
| H | GS002 | wildcard_san.pem | 0 |
| H | GS002 | wosign-bc-invalid.pem | 0 |
| H | GS004 | utils.py | 17 |
| s | GS009 |  | 0 |
| M | GS014 | dh_key_256.pem | 1 |
| M | GS014 | dhkey.pem | 1 |
| M | GS014 | dhkey_rfc5114_2.pem | 1 |
| M | GS014 | dhp.pem | 1 |
| M | GS014 | dhp_privatevaluelength.pem | 1 |
| M | GS014 | dhp_rfc5114_2.pem | 1 |
| M | GS014 | dhpub.pem | 1 |
| M | GS014 | dhpub_cryptography_old.pem | 1 |
| M | GS014 | dhpub_rfc5114_2.pem | 1 |
| M | GS014 | nilpotent.pem | 1 |
| M | GS014 | ec-missing-curve.pem | 1 |
| M | GS014 | explicit_parameters_private_key.pem | 1 |
| M | GS014 | explicit_parameters_wap_wsg_idm_ecid_wtls11_private_key.pem | 1 |
| M | GS014 | high-bit-set.pem | 1 |
| M | GS014 | secp128r1_private_key.pem | 1 |
| M | GS014 | secp256k1-explicit-no-seed.pem | 1 |
| M | GS014 | secp256k1-pub-explicit-no-seed.pem | 1 |
| M | GS014 | secp256r1-explicit-no-seed.pem | 1 |
| M | GS014 | secp256r1-explicit-seed.pem | 1 |
| M | GS014 | secp256r1-pub-explicit-no-seed.pem | 1 |
| M | GS014 | secp256r1-pub-explicit-seed.pem | 1 |
| M | GS014 | secp384r1-explicit-no-seed.pem | 1 |
| M | GS014 | secp384r1-explicit-seed.pem | 1 |
| M | GS014 | secp384r1-pub-explicit-no-seed.pem | 1 |
| M | GS014 | secp384r1-pub-explicit-seed.pem | 1 |
| M | GS014 | secp521r1-explicit-no-seed.pem | 1 |
| M | GS014 | secp521r1-explicit-seed.pem | 1 |
| M | GS014 | secp521r1-pub-explicit-no-seed.pem | 1 |
| M | GS014 | secp521r1-pub-explicit-seed.pem | 1 |
| M | GS014 | sect163k1-spki.pem | 1 |
| M | GS014 | sect163r2-spki.pem | 1 |
| M | GS014 | sect233k1-spki.pem | 1 |
| M | GS014 | sect233r1-spki.pem | 1 |
| M | GS014 | ed25519-pkcs8-enc.pem | 1 |
| M | GS014 | ed25519-pkcs8.pem | 1 |
| M | GS014 | ed25519-pub.pem | 1 |
| M | GS014 | ed448-pkcs8-enc.pem | 1 |
| M | GS014 | ed448-pkcs8.pem | 1 |
| M | GS014 | ed448-pub.pem | 1 |
| M | GS014 | mlkem768.pem | 1 |
| M | GS014 | dsa-nopsw.key | 1 |
| M | GS014 | dsa-psw.key | 1 |
| M | GS014 | ecdsa-nopsw.key | 1 |
| M | GS014 | ecdsa-psw.key | 1 |
| M | GS014 | ed25519-aesgcm-psw.key | 1 |
| M | GS014 | ed25519-nopsw.key | 1 |
| M | GS014 | ed25519-psw.key | 1 |
| M | GS014 | rsa-nopsw.key | 1 |
| M | GS014 | rsa-psw.key | 1 |
| M | GS014 | sk-ecdsa-nopsw.key | 1 |
| M | GS014 | sk-ecdsa-psw.key | 1 |
| M | GS014 | sk-ed25519-nopsw.key | 1 |
| M | GS014 | sk-ed25519-psw.key | 1 |
| M | GS014 | dsa_4096.pem | 1 |
| M | GS014 | dsa_private_key.pem | 1 |
| M | GS014 | dsa_public_key.pem | 1 |
| M | GS014 | dsaparam.pem | 1 |
| M | GS014 | ec_private_key.pem | 1 |
| M | GS014 | ec_private_key_encrypted.pem | 1 |
| M | GS014 | ec_public_key.pem | 1 |
| M | GS014 | ec_public_key_rsa_delimiter.pem | 1 |
| M | GS014 | rsa-bad-1025-q-is-2.pem | 1 |
| M | GS014 | rsa_private_key.pem | 1 |
| M | GS014 | rsa_public_key.pem | 1 |
| M | GS014 | rsa_wrong_delimiter_public_key.pem | 1 |
| M | GS014 | bad-encryption-oid.pem | 1 |
| M | GS014 | bad-oid-dsa-key.pem | 1 |
| M | GS014 | ec-consistent-curve.pem | 1 |
| M | GS014 | ec-inconsistent-curve.pem | 1 |
| M | GS014 | ec-inconsistent-curve2.pem | 1 |
| M | GS014 | ec-invalid-private-scalar.pem | 1 |
| M | GS014 | ec-invalid-version.pem | 1 |
| M | GS014 | ec_oid_not_in_reg_private_2.pkcs8.pem | 1 |
| M | GS014 | ec_private_key.pem | 1 |
| M | GS014 | ec_private_key_encrypted.pem | 1 |
| M | GS014 | ecc_private_with_rfc5915_ext.pem | 1 |
| M | GS014 | ed25519-scrypt.pem | 1 |
| M | GS014 | enc-ec-sha1-128-rc4.pem | 1 |
| M | GS014 | enc-rsa-3des.pem | 1 |
| M | GS014 | enc-rsa-pkcs8-pbkdf2-0iter.pem | 1 |
| M | GS014 | enc-rsa-pkcs8.pem | 1 |
| M | GS014 | enc-unknown-algorithm.pem | 1 |
| M | GS014 | enc-unknown-kdf.pem | 1 |
| M | GS014 | enc-unknown-pbkdf2-prf.pem | 1 |
| M | GS014 | enc2-rsa-pkcs8.pem | 1 |
| M | GS014 | nodompar_private.pkcs8.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9607.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9671.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9925.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9926.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9927.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9928.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9929.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9930.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9931.pem | 1 |
| M | GS014 | pkcs12_s2k_pem-X_9932.pem | 1 |
| M | GS014 | private.pem | 1 |
| M | GS014 | rsa-40bitrc2.pem | 1 |
| M | GS014 | rsa-aes-192-cbc.pem | 1 |
| M | GS014 | rsa-pbe-3des-long-salt.pem | 1 |
| M | GS014 | rsa-pbewithmd5anddescbc.pem | 1 |
| M | GS014 | rsa-rc2-cbc-effective-key-length.pem | 1 |
| M | GS014 | rsa-rc2-cbc.pem | 1 |
| M | GS014 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha224.pem | 1 |
| M | GS014 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha384.pem | 1 |
| M | GS014 | rsa_pkcs8_pbes2_pbkdf2_2048_3des_sha512.pem | 1 |
| M | GS014 | rsa_pss_2048.pem | 1 |
| M | GS014 | rsa_pss_2048_hash.pem | 1 |
| M | GS014 | rsa_pss_2048_hash_mask.pem | 1 |
| M | GS014 | rsa_pss_2048_hash_mask_diff.pem | 1 |
| M | GS014 | rsa_pss_2048_hash_mask_salt.pem | 1 |
| M | GS014 | unenc-dsa-pkcs8.pem | 1 |
| M | GS014 | unenc-dsa-pkcs8.pub.pem | 1 |
| M | GS014 | unenc-rsa-pkcs8.pem | 1 |
| M | GS014 | unenc-rsa-pkcs8.pub.pem | 1 |
| M | GS014 | withdompar_private.pkcs8.pem | 1 |
| M | GS014 | wrong-pem-delimiter-rsa.pem | 1 |
| M | GS014 | dsa-wrong-version.pem | 1 |
| M | GS014 | dsa.1024.pem | 1 |
| M | GS014 | dsa.2048.pem | 1 |
| M | GS014 | dsa.3072.pem | 1 |
| M | GS014 | key1-malformed-dek-info.pem | 1 |
| M | GS014 | key1-malformed-iv.pem | 1 |
| M | GS014 | key1-no-dek-info.pem | 1 |
| M | GS014 | key1-short-iv.pem | 1 |
| M | GS014 | key1.pem | 1 |
| M | GS014 | key2.pem | 1 |
| M | GS014 | rsa-wrong-version.pem | 1 |
| M | GS014 | testrsa-encrypted.pem | 1 |
| M | GS014 | testrsa.pem | 1 |
| M | GS014 | x25519-pkcs8-enc.pem | 1 |
| M | GS014 | x25519-pkcs8.pem | 1 |
| M | GS014 | x25519-pub.pem | 1 |
| M | GS014 | x448-pkcs8-enc.pem | 1 |
| M | GS014 | x448-pkcs8.pem | 1 |
| M | GS014 | x448-pub.pem | 1 |
| M | GS014 | dsa.pub.pem | 1 |
| M | GS014 | rsa.pub.pem | 1 |
| M | GS014 | ca.pem | 1 |
| M | GS014 | ca_key.pem | 1 |
| M | GS014 | ascii-san.pem | 1 |
| M | GS014 | enveloped-rsa-oaep.pem | 1 |
| M | GS014 | enveloped-triple-des.pem | 1 |
| M | GS014 | enveloped.pem | 1 |
| M | GS014 | isrg.pem | 1 |
| M | GS014 | non-ascii-san.pem | 1 |
| M | GS014 | accvraiz1.pem | 1 |
| M | GS014 | badasn1time.pem | 1 |
| M | GS014 | badssl-sct.pem | 1 |
| M | GS014 | belgian-eid-invalid-visiblestring.pem | 1 |
| M | GS014 | bigoid.pem | 1 |
| M | GS014 | cryptography-scts.pem | 1 |
| M | GS014 | cryptography.io.chain.pem | 1 |
| M | GS014 | cryptography.io.chain_with_garbage.pem | 1 |
| M | GS014 | cryptography.io.old_header.pem | 1 |
| M | GS014 | cryptography.io.pem | 1 |
| M | GS014 | cryptography.io.precert.pem | 1 |
| M | GS014 | cryptography.io.with_garbage.pem | 1 |
| M | GS014 | cryptography.io.with_headers.pem | 1 |
| M | GS014 | admissions_extension_authority_not_provided.pem | 1 |
| M | GS014 | admissions_extension_optional_data_not_provided.pem | 1 |
| M | GS014 | aia_ca_issuers.pem | 1 |
| M | GS014 | aia_ocsp.pem | 1 |
| M | GS014 | aia_ocsp_ca_issuers.pem | 1 |
| M | GS014 | all_key_usages.pem | 1 |
| M | GS014 | all_supported_names.pem | 1 |
| M | GS014 | authority_key_identifier.pem | 1 |
| M | GS014 | authority_key_identifier_no_keyid.pem | 1 |
| M | GS014 | bad_country.pem | 1 |
| M | GS014 | basic_constraints_not_critical.pem | 1 |
| M | GS014 | bc_path_length_zero.pem | 1 |
| M | GS014 | ca.pem | 1 |
| M | GS014 | ca_key.pem | 1 |
| M | GS014 | rsa_ca.pem | 1 |
| M | GS014 | rsa_key.pem | 1 |
| M | GS014 | rsae_ca.pem | 1 |
| M | GS014 | cdp_all_reasons.pem | 1 |
| M | GS014 | cdp_crl_issuer.pem | 1 |
| M | GS014 | cdp_empty_hostname.pem | 1 |
| M | GS014 | cdp_fullname_reasons_crl_issuer.pem | 1 |
| M | GS014 | cdp_reason_aa_compromise.pem | 1 |
| M | GS014 | cp_cps_uri.pem | 1 |
| M | GS014 | cp_invalid.pem | 1 |
| M | GS014 | cp_user_notice_no_explicit_text.pem | 1 |
| M | GS014 | cp_user_notice_with_explicit_text.pem | 1 |
| M | GS014 | cp_user_notice_with_notice_reference.pem | 1 |
| M | GS014 | crl_all_reasons.pem | 1 |
| M | GS014 | crl_almost_10k.pem | 1 |
| M | GS014 | crl_bad_version.pem | 1 |
| M | GS014 | crl_delta_crl_indicator.pem | 1 |
| M | GS014 | crl_dup_entry_ext.pem | 1 |
| M | GS014 | crl_empty.pem | 1 |
| M | GS014 | crl_ian_aia_aki.pem | 1 |
| M | GS014 | crl_idp_fullname_indirect_crl.pem | 1 |
| M | GS014 | crl_idp_fullname_only.pem | 1 |
| M | GS014 | crl_idp_fullname_only_aa.pem | 1 |
| M | GS014 | crl_idp_fullname_only_user.pem | 1 |
| M | GS014 | crl_idp_only_ca.pem | 1 |
| M | GS014 | crl_idp_reasons_only.pem | 1 |
| M | GS014 | crl_idp_relative_user_all_reasons.pem | 1 |
| M | GS014 | crl_idp_relativename_only.pem | 1 |
| M | GS014 | crl_inval_cert_issuer_entry_ext.pem | 1 |
| M | GS014 | crl_md2_unknown_crit_entry_ext.pem | 1 |
| M | GS014 | crl_no_next_update.pem | 1 |
| M | GS014 | crl_unsupported_reason.pem | 1 |
| M | GS014 | dsa_null_alg_params.pem | 1 |
| M | GS014 | dsa_selfsigned_ca.pem | 1 |
| M | GS014 | ec_no_named_curve.pem | 1 |
| M | GS014 | ecdsa_null_alg.pem | 1 |
| M | GS014 | ekucrit-testuser-cert.pem | 1 |
| M | GS014 | empty-eku.pem | 1 |
| M | GS014 | extended_key_usage.pem | 1 |
| M | GS014 | freshestcrl.pem | 1 |
| M | GS014 | ian_uri.pem | 1 |
| M | GS014 | inhibit_any_policy_5.pem | 1 |
| M | GS014 | inhibit_any_policy_negative.pem | 1 |
| M | GS014 | invalid_signature_cert.pem | 1 |
| M | GS014 | invalid_signature_crl.pem | 1 |
| M | GS014 | invalid_utf8_common_name.pem | 1 |
| M | GS014 | invalid_version.pem | 1 |
| M | GS014 | long-form-name-attribute.pem | 1 |
| M | GS014 | malformed-ian.pem | 1 |
| M | GS014 | malformed-san.pem | 1 |
| M | GS014 | ms-certificate-template.pem | 1 |
| M | GS014 | name_attribute_unsupported_tag.pem | 1 |
| M | GS014 | nc_excluded.pem | 1 |
| M | GS014 | nc_invalid_ip_netmask.pem | 1 |
| M | GS014 | nc_ip_invalid_length.pem | 1 |
| M | GS014 | nc_permitted.pem | 1 |
| M | GS014 | nc_permitted_2.pem | 1 |
| M | GS014 | nc_permitted_excluded.pem | 1 |
| M | GS014 | nc_permitted_excluded_2.pem | 1 |
| M | GS014 | nc_single_ip_netmask.pem | 1 |
| M | GS014 | negative_serial.pem | 1 |
| M | GS014 | no_sans.pem | 1 |
| M | GS014 | ocsp_nocheck.pem | 1 |
| M | GS014 | pc_inhibit.pem | 1 |
| M | GS014 | pc_inhibit_require.pem | 1 |
| M | GS014 | pc_require.pem | 1 |
| M | GS014 | policy_constraints_explicit.pem | 1 |
| M | GS014 | post2000utctime.pem | 1 |
| M | GS014 | private_key_usage_period_both_dates.pem | 1 |
| M | GS014 | private_key_usage_period_only_not_after.pem | 1 |
| M | GS014 | private_key_usage_period_only_not_before.pem | 1 |
| M | GS014 | rsa_pss.pem | 1 |
| M | GS014 | rsa_pss_cert.pem | 1 |
| M | GS014 | rsa_pss_sha256_no_null.pem | 1 |
| M | GS014 | san_dirname.pem | 1 |
| M | GS014 | san_email_dns_ip_dirname_uri.pem | 1 |
| M | GS014 | san_empty_hostname.pem | 1 |
| M | GS014 | san_idna2003_dnsname.pem | 1 |
| M | GS014 | san_idna_names.pem | 1 |
| M | GS014 | san_ipaddr.pem | 1 |
| M | GS014 | san_other_name.pem | 1 |
| M | GS014 | san_registered_id.pem | 1 |
| M | GS014 | san_rfc822_idna.pem | 1 |
| M | GS014 | san_rfc822_names.pem | 1 |
| M | GS014 | san_uri_with_port.pem | 1 |
| M | GS014 | san_wildcard_idna.pem | 1 |
| M | GS014 | sia.pem | 1 |
| M | GS014 | two_basic_constraints.pem | 1 |
| M | GS014 | unsupported_extension.pem | 1 |
| M | GS014 | unsupported_extension_2.pem | 1 |
| M | GS014 | unsupported_extension_critical.pem | 1 |
| M | GS014 | unsupported_subject_name.pem | 1 |
| M | GS014 | unsupported_subject_public_key_info.pem | 1 |
| M | GS014 | utf8_common_name.pem | 1 |
| M | GS014 | valid_signature_cert.pem | 1 |
| M | GS014 | valid_signature_crl.pem | 1 |
| M | GS014 | department-of-state-root.pem | 1 |
| M | GS014 | ecdsa_root.pem | 1 |
| M | GS014 | ed25519-rfc8410.pem | 1 |
| M | GS014 | root-ed25519.pem | 1 |
| M | GS014 | server-ed25519-cert.pem | 1 |
| M | GS014 | root-ed448.pem | 1 |
| M | GS014 | server-ed448-cert.pem | 1 |
| M | GS014 | ee-pss-sha1-cert.pem | 1 |
| M | GS014 | letsencryptx3.pem | 1 |
| M | GS014 | rapidssl_sha256_ca_g3.pem | 1 |
| M | GS014 | bad-version.pem | 1 |
| M | GS014 | basic_constraints.pem | 1 |
| M | GS014 | challenge-unstructured.pem | 1 |
| M | GS014 | challenge.pem | 1 |
| M | GS014 | dsa_sha1.pem | 1 |
| M | GS014 | ec_sha256.pem | 1 |
| M | GS014 | ec_sha256_old_header.pem | 1 |
| M | GS014 | freeipa-bad-critical.pem | 1 |
| M | GS014 | invalid_signature.pem | 1 |
| M | GS014 | long-form-attribute.pem | 1 |
| M | GS014 | rsa_md4.pem | 1 |
| M | GS014 | rsa_sha1.pem | 1 |
| M | GS014 | rsa_sha256.pem | 1 |
| M | GS014 | san_rsa_sha1.pem | 1 |
| M | GS014 | two_basic_constraints.pem | 1 |
| M | GS014 | unsupported_extension.pem | 1 |
| M | GS014 | unsupported_extension_critical.pem | 1 |
| M | GS014 | zero-element-attribute.pem | 1 |
| M | GS014 | scottishpower-bitstring-dn.pem | 1 |
| M | GS014 | tls-feature-ocsp-staple.pem | 1 |
| M | GS014 | unique_identifier.pem | 1 |
| M | GS014 | utf8-dnsname.pem | 1 |
| M | GS014 | v1_cert.pem | 1 |
| M | GS014 | verisign_md2_root.pem | 1 |
| M | GS014 | wildcard_san.pem | 1 |
| M | GS014 | wosign-bc-invalid.pem | 1 |
| H | ? | extensions.rs | 36 |
| H | ? | extensions.rs | 37 |
| H | ? | extensions.rs | 42 |
| H | ? | extensions.rs | 62 |
| H | ? | csr.rs | 27 |
| H | ? | csr.rs | 31 |
| H | ? | csr.rs | 32 |
| H | ? | buf.rs | 74 |
| H | ? | crl.rs | 139 |
| H | ? | crl.rs | 155 |
| H | ? | crl.rs | 410 |
| H | ? | crl.rs | 427 |
| H | ? | crl.rs | 559 |
| H | ? | crl.rs | 593 |
| H | ? | crl.rs | 764 |
| H | ? | crl.rs | 778 |
| H | ? | crl.rs | 801 |
| H | ? | crl.rs | 802 |
| H | ? | crl.rs | 803 |
| H | ? | ocsp.rs | 101 |
| H | ? | ocsp.rs | 119 |
| H | ? | extensions.rs | 249 |
| H | ? | extensions.rs | 291 |
| H | ? | extensions.rs | 402 |
| H | ? | extensions.rs | 409 |
| H | ? | extensions.rs | 624 |
| H | ? | extensions.rs | 681 |
| H | ? | sign.rs | 151 |
| H | ? | sign.rs | 152 |
| H | ? | sign.rs | 163 |
| H | ? | sign.rs | 323 |
| H | ? | sign.rs | 358 |
| H | ? | sign.rs | 506 |
| H | ? | sign.rs | 542 |
| H | ? | extension_policy.rs | 57 |
| H | ? | mod.rs | 46 |
| H | ? | mod.rs | 95 |
| H | ? | mod.rs | 186 |
| H | ? | mod.rs | 233 |
| H | ? | mod.rs | 450 |
| H | ? | mod.rs | 541 |
| H | ? | certificate.rs | 94 |
| H | ? | certificate.rs | 159 |
| H | ? | certificate.rs | 172 |
| H | ? | certificate.rs | 190 |
| H | ? | certificate.rs | 514 |
| H | ? | certificate.rs | 529 |
| H | ? | certificate.rs | 738 |
| H | ? | certificate.rs | 784 |
| H | ? | certificate.rs | 989 |
| H | ? | certificate.rs | 1014 |
| H | ? | certificate.rs | 1015 |
| H | ? | certificate.rs | 1016 |
| H | ? | certificate.rs | 1074 |
| H | ? | certificate.rs | 1096 |
| H | ? | certificate.rs | 1097 |
| H | ? | certificate.rs | 1098 |
| H | ? | ocsp_req.rs | 64 |
| H | ? | csr.rs | 143 |
| H | ? | csr.rs | 145 |
| H | ? | csr.rs | 153 |
| H | ? | csr.rs | 166 |
| H | ? | csr.rs | 263 |
| H | ? | csr.rs | 264 |
| H | ? | csr.rs | 265 |
| H | ? | csr.rs | 293 |
| H | ? | csr.rs | 329 |
| H | ? | csr.rs | 350 |
| H | ? | csr.rs | 351 |
| H | ? | csr.rs | 352 |
| H | ? | csr.rs | 363 |
| H | ? | ocsp_resp.rs | 105 |
| H | ? | ocsp_resp.rs | 259 |
| H | ? | ocsp_resp.rs | 549 |
| H | ? | ocsp_resp.rs | 805 |
| H | ? | ocsp_resp.rs | 827 |
| H | ? | ocsp_resp.rs | 828 |
| H | ? | ocsp_resp.rs | 834 |
| H | ? | ocsp_resp.rs | 835 |
| H | ? | ocsp_resp.rs | 857 |
| H | ? | sct.rs | 265 |
| H | ? | common.rs | 220 |
| H | ? | common.rs | 281 |
| H | ? | common.rs | 344 |
| H | ? | common.rs | 429 |
| H | ? | asn1.rs | 20 |
| H | ? | asn1.rs | 27 |
| H | ? | asn1.rs | 84 |
| H | ? | error.rs | 173 |
| H | ? | error.rs | 325 |
| H | ? | utils.rs | 330 |
| H | ? | cmac.rs | 42 |
| H | ? | ciphers.rs | 28 |
| H | ? | ciphers.rs | 587 |
| H | ? | ciphers.rs | 620 |
| H | ? | hashes.rs | 96 |
| H | ? | hashes.rs | 135 |
| H | ? | hashes.rs | 219 |
| H | ? | hashes.rs | 262 |
| H | ? | hmac.rs | 38 |
| H | ? | hpke.rs | 844 |
| H | ? | hpke.rs | 868 |
| H | ? | cipher_registry.rs | 98 |
| H | ? | cipher_registry.rs | 99 |
| H | ? | ec.rs | 154 |
| H | ? | ec.rs | 179 |
| H | ? | ec.rs | 552 |
| H | ? | ec.rs | 633 |
| H | ? | pkcs12.rs | 182 |
| H | ? | pkcs12.rs | 389 |
| H | ? | test_support.rs | 34 |
| H | ? | decode.rs | 346 |
| H | ? | asn1.rs | 18 |
| H | ? | encode.rs | 35 |
| H | ? | encode.rs | 253 |
| H | ? | encode.rs | 260 |
| H | ? | encode.rs | 388 |
| H | ? | types.rs | 359 |
| H | ? | pkcs7.rs | 64 |
| H | ? | pkcs7.rs | 142 |
| H | ? | pkcs7.rs | 252 |
| H | ? | pkcs7.rs | 255 |
| H | ? | pkcs7.rs | 391 |
| H | ? | pkcs7.rs | 507 |
| H | ? | pkcs7.rs | 519 |
| H | ? | pkcs7.rs | 520 |
| H | ? | pkcs7.rs | 521 |
| H | ? | pkcs7.rs | 569 |
| H | ? | pkcs7.rs | 570 |
| H | ? | pkcs7.rs | 571 |
| H | ? | pkcs7.rs | 581 |
| H | ? | pkcs7.rs | 584 |
| H | ? | pkcs7.rs | 586 |
| H | ? | pkcs7.rs | 591 |
| H | ? | pkcs7.rs | 598 |
| H | ? | pkcs7.rs | 599 |
| H | ? | pkcs7.rs | 600 |
| H | ? | pkcs7.rs | 665 |
| H | ? | pkcs7.rs | 806 |
| H | ? | types.rs | 31 |
| H | ? | lib.rs | 23 |
| H | ? | spki.rs | 181 |
| H | ? | pkcs8.rs | 214 |
| H | ? | pkcs8.rs | 360 |
| H | ? | pkcs8.rs | 386 |
| H | ? | pkcs8.rs | 422 |
| H | ? | pkcs8.rs | 432 |
| H | ? | ec.rs | 63 |
| H | ? | ec.rs | 67 |
| H | ? | lib.rs | 256 |
| H | ? | lib.rs | 260 |
| H | ? | lib.rs | 283 |
| H | ? | lib.rs | 444 |
| H | ? | lib.rs | 464 |
| H | ? | lib.rs | 529 |
| H | ? | lib.rs | 581 |
| H | ? | extension.rs | 43 |
| H | ? | extension.rs | 44 |
| H | ? | extension.rs | 45 |
| H | ? | extension.rs | 46 |
| H | ? | extension.rs | 47 |
| H | ? | extension.rs | 48 |
| H | ? | extension.rs | 49 |
| H | ? | extension.rs | 50 |
| H | ? | extension.rs | 51 |
| H | ? | extension.rs | 52 |
| H | ? | extension.rs | 221 |
| H | ? | extension.rs | 226 |
| H | ? | extension.rs | 303 |
| H | ? | extension.rs | 425 |
| H | ? | extension.rs | 432 |
| H | ? | extension.rs | 433 |
| H | ? | extension.rs | 434 |
| H | ? | extension.rs | 441 |
| H | ? | extension.rs | 442 |
| H | ? | extension.rs | 443 |
| H | ? | extension.rs | 498 |
| H | ? | extension.rs | 505 |
| H | ? | extension.rs | 520 |
| H | ? | extension.rs | 541 |
| H | ? | mod.rs | 70 |
| H | ? | mod.rs | 71 |
| H | ? | mod.rs | 72 |
| H | ? | mod.rs | 73 |
| H | ? | mod.rs | 156 |
| H | ? | mod.rs | 157 |
| H | ? | mod.rs | 158 |
| H | ? | mod.rs | 159 |
| H | ? | mod.rs | 160 |
| H | ? | mod.rs | 161 |
| H | ? | mod.rs | 162 |
| H | ? | mod.rs | 163 |
| H | ? | mod.rs | 164 |
| H | ? | mod.rs | 202 |
| H | ? | mod.rs | 315 |
| H | ? | mod.rs | 336 |
| H | ? | mod.rs | 514 |
| H | ? | mod.rs | 800 |
| H | ? | mod.rs | 810 |
| H | ? | mod.rs | 820 |
| H | ? | mod.rs | 829 |
| H | ? | mod.rs | 839 |
| H | ? | certificate.rs | 74 |
| H | ? | certificate.rs | 78 |
| H | ? | trust_store.rs | 22 |

---
*Сгенерировано GSC v0.6 · 2026-07-03T04:03:15.586915*