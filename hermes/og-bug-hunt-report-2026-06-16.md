# OG Bug Hunt Report — TheOriginals.io
## Submitted by: @Stukach_Bybit
## Date: 2026-06-16

---

## 🐛 Finding #1 [HIGH] — i18n Translation Keys Exposed as Raw Text

**Severity:** HIGH (UX/Trust)
**Affected pages:** Multiple legal pages and game UIs on www.theoriginals.io

### Description
Multiple pages on `www.theoriginals.io` display raw internationalization (i18n) keys instead of translated text. Users see technical identifiers like `privacy.title`, `global.auth.sign_in`, `game.bet.amount` instead of human-readable content.

### Steps to Reproduce
1. Go to https://www.theoriginals.io/legal/privacy
2. Observe: entire page shows raw i18n keys (privacy.title, privacy.section.*)
3. Go to https://www.theoriginals.io/legal/responsible-gaming
4. Observe: raw keys (responsible.title, responsible.section.*)
5. Go to https://www.theoriginals.io/game/limbo
6. Observe: UI labels are raw keys (game.bet.amount, game.bet.auto, global.auth.sign_in)

### Affected Pages (confirmed)
- `/legal/privacy` — 100% broken
- `/legal/responsible-gaming` — 100% broken
- `/legal/restricted-jurisdiction` — 100% broken (on theoriginals.io without www)
- `/game/limbo` — all UI labels broken
- `/game/plinko` — menu labels broken
- `/game/mines` — menu labels broken
- `/game/keno` — menu labels broken
- `/game/crash` — menu labels broken

### Expected Behavior
All pages should display properly translated text in the user's language.

### Impact
- **Trust/credibility:** Legal documents (Privacy Policy, Responsible Gaming) are unreadable — this is a compliance risk for a gambling platform
- **UX:** Game UI is unusable without proper labels
- **Conversion:** Users cannot understand buttons and game controls

### Possible Cause
The www subdomain appears to load a different i18n bundle or locale configuration than the apex domain. Example:
- `www.theoriginals.io/legal/terms` → renders correctly
- `www.theoriginals.io/legal/privacy` → broken
- `theoriginals.io/legal/terms` → broken (raw keys)
- `theoriginals.io/legal/responsible-gaming` → renders correctly

This suggests a CDN/edge-cache or SSR hydration mismatch between subdomains.

---

## 🐛 Finding #2 [HIGH] — Missing Security Headers

**Severity:** HIGH (Security)
**Affected:** All pages on both www.theoriginals.io and theoriginals.io

### Description
The server returns zero security-related HTTP headers. No CSP, no clickjacking protection, no MIME-type enforcement.

### Missing Headers
- `Content-Security-Policy` — no XSS protection
- `X-Frame-Options` — vulnerable to clickjacking
- `X-Content-Type-Options` — MIME sniffing risk
- `Strict-Transport-Security` — no HSTS enforcement
- `Referrer-Policy` — referrer leakage
- `Permissions-Policy` — no API abuse protection

### Steps to Verify
```bash
curl -sI https://www.theoriginals.io | grep -iE "content-security|x-frame|x-content|strict-transport|referrer-policy"
# Returns: (empty — no headers present)
```

### Impact
For a crypto gambling platform handling real funds (USDT, USDC, ETH, BTC, TON), missing security headers are a significant risk. Clickjacking could trick users into confirming withdrawals, and lack of CSP increases XSS risk.

---

## 🐛 Finding #3 [MEDIUM] — Dev Artifact in Production (localhost blob URL)

**Severity:** MEDIUM (Code Quality)
**Page:** https://theoriginals.io/game/hyperdrive

### Description
The Hyperdrive game page contains references to `blob:http://localhost/` URLs for game assets, which will never load for real users.

### Evidence
```
![Image 1: illuminated mask](blob:http://localhost/0e2835dc9b69d51d942a2511bf41dff2)
![Image 2: Dark mask](blob:http://localhost/b7d3e5ad80dd42c68b410b1746948098)
```

### Impact
Game assets fail to load, degrading user experience. Indicates development code leaked to production.

---

## 🐛 Finding #4 [LOW] — Typo on Homepage

**Severity:** LOW (Copy)
**Page:** https://www.theoriginals.io/

### Description
Homepage says "Fastest originals on the market with **provenably** fair 99% Return To Player games"

### Expected
"**provably** fair" — this is the standard term in crypto gambling for verifiable RNG fairness.

---

## Summary

| # | Severity | Category | Bounty Estimate |
|---|----------|----------|-----------------|
| 1 | HIGH | i18n/UX — legal pages unreadable | $100-300 |
| 2 | HIGH | Security — zero security headers | $200-500 |
| 3 | MEDIUM | Code quality — localhost dev artifact | $30-50 |
| 4 | LOW | Copy — typo | $10 |

**Total estimated:** $340-860

## Attachments
(Screenshots to be added by submitter)
- Screenshot 1: www.theoriginals.io/legal/privacy — raw i18n keys
- Screenshot 2: www.theoriginals.io/legal/responsible-gaming — raw i18n keys
- Screenshot 3: www.theoriginals.io/game/limbo — raw UI labels
- Screenshot 4: curl output showing zero security headers
- Screenshot 5: theoriginals.io/game/hyperdrive — localhost blob URLs
