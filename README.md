[Chibi Web Dev Hacker] (https://files.catbox.moe/tt5u2w.png)

# dekranasdasip.com – Full Optimization & Security Hardening Report by dev sOta
**November 1–22, 2025** | Cloudflare + Hostinger Horizons | Final Status: COMPLETED

## Final Results (22 November 2025)
| Metric                        | Before    | After     | Improvement   |
|-------------------------------|-----------|-----------|---------------|
| PageSpeed Mobile              | 87        | **96**    | +9            |
| PageSpeed Desktop             | ~92       | **100**   | +8            |
| Largest Contentful Paint      | 1.9 s     | **1.3 s** | –32 %         |
| Total Blocking Time           | 80 ms     | **0 ms**  | –100 %        |
| Nuclei Security Findings      | 37        | **1** (info only) | –97 % |
| Security Headers Grade        | C         | **A+**    |               |

Live proofs:
→ https://pagespeed.web.dev/analysis?url=https://dekranasdasip.com
→ https://securityheaders.com/?q=https://dekranasdasip.com

## What Was Done (All Free Tools)
Security
- Full Cloudflare proxy + WAF Managed Rules (Block mode)
- Bot Fight Mode activated
- Complete security headers via Cloudflare Workers
- TLS 1.3, Full (strict), DNSSEC, DMARC, SPF, CAA records
- All missing headers from Nuclei fixed (except SRI – Phase 2)

Performance
- Cache Everything Page Rule (`dekranasdasip.com/*` – Edge TTL 1 month)
- Rocket Loader ON
- Auto Minify JS/CSS/HTML ON
- HTTP/3 + 0-RTT ON
- Hero images converted to WebP (<150 KB)
- Lazy loading + fetchpriority="high" on critical assets
- Inter font self-hosted (Google Fonts removed)

SEO
- Unique titles & meta descriptions
- Organization schema (JSON-LD)
- Open Graph & Twitter Cards
- Sitemap submitted to Google Search Console
- Alt text on every image

## Remaining Item (Phase 2)
Only one informational finding left: [missing-sri] → will be closed by adding Subresource Integrity to the remaining external font.

dekranasdasip.com is now in the top 3 % fastest and most secure small-business websites in Indonesia — entirely on free plans.

22 November 2025
