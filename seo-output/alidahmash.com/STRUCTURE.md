# Site Architecture — alidahmash.com
**Generated:** 2026-05-12
**Site type:** Personal brand / B2B service (SEO & PPC consulting)
**Platform:** Replit React SPA (client-side rendering)

---

## URL Structure

```
https://www.alidahmash.com/                          ← Homepage (brand hub)
│
├── /about                                            ← Personal brand / E-E-A-T page
├── /contact                                          ← Lead generation
│
├── /services/                                        ← Services hub
│   ├── /services/seo                                 ← SEO consulting service
│   ├── /services/ppc                                 ← PPC / Google Ads service
│   ├── /services/content-strategy                    ← Content marketing service
│   └── /services/growth-marketing                    ← Growth marketing service
│
├── /tampa-seo-ppc-consultant                         ← Location landing page (Tampa, FL)
│
├── /website-analyzer                                 ← Free tool (lead gen)
│
├── /case-studies                                     ← Social proof hub
│
└── /blog/                                            ← Content / authority hub
    ├── /blog/how-to-find-best-tampa-seo-expert-hiring-guide
    ├── /blog/google-analytics-4-complete-setup-guide-marketing
    └── [additional posts]
```

---

## Sitemap Organization

**Total URLs in sitemap:** 14 (current) — expected to grow with blog content
**Sitemap type:** Single file (well under 50,000 URL limit)
**Split required:** No

| Section | URL Count | Notes |
|---------|-----------|-------|
| Core pages | 3 | Homepage, About, Contact |
| Services | 5 | Hub + 4 service pages |
| Location pages | 1 | Tampa landing page |
| Tools | 1 | Website analyzer |
| Case studies | 1 | Hub page |
| Blog | 3 | Index + 2 confirmed posts |

---

## Canonical Strategy

**Canonical domain:** `https://www.alidahmash.com/` (www)

**Required redirects:**
- `http://alidahmash.com/*` → `https://www.alidahmash.com/*` (HTTP → HTTPS + non-www → www)
- `http://www.alidahmash.com/*` → `https://www.alidahmash.com/*`
- `https://alidahmash.com/*` → `https://www.alidahmash.com/*`
- `https://alidahmash.com/2015/03/15/loosing-facebook-fans/` → `https://www.alidahmash.com/blog/` (legacy WordPress URL)

---

## Growth Recommendations

### Safe Programmatic Expansion (future)

| Page Type | Scale | Rationale |
|-----------|-------|-----------|
| Blog posts | Unlimited | Unique expert content |
| Case study pages | Up to ~20 | Unique client data |
| Service sub-pages | Up to ~10 | Specific service niches |
| Location pages | ⚠️ MAX 3-5 | Only with 60%+ unique content per city |
| Tool result pages | ✅ OK at scale | User-generated, dynamic value |

### Location Page Warning

If expanding beyond Tampa to other cities (e.g., `/orlando-seo-consultant`, `/miami-ppc-consultant`):
- ⚠️ WARNING at 3+ location pages: require 60%+ unique content per page (local case studies, testimonials, local references)
- 🛑 HARD STOP at 5+ location pages without unique data: Google considers these thin/doorway pages
- Each location page must include: local case study, local testimonial, local business references, not just city-name swaps

---

## Sitemap Maintenance Checklist

- [ ] Update `<lastmod>` when page content changes significantly
- [ ] Add new blog post URLs immediately after publishing
- [ ] Remove 404 URLs within 48 hours of detection
- [ ] Do NOT include noindex pages in sitemap
- [ ] Do NOT include paginated URLs (e.g., `/blog?page=2`) unless using rel="canonical"
- [ ] Resubmit sitemap in GSC after major structural changes
- [ ] Monitor GSC "Coverage" report monthly for excluded/invalid URLs
