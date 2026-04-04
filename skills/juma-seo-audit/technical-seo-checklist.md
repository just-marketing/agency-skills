# Technical SEO Audit Checklist

Use this checklist during Step 2 of the SEO audit process. Evaluate each element and score its health.

## 1. Crawlability

- [ ] Can search engines discover and access all important pages?
- [ ] Are there crawl errors (4xx, 5xx)?
- [ ] Are there redirect chains or loops?
- [ ] Are there orphan pages (no internal links pointing to them)?
- [ ] Is JavaScript rendering blocking crawling of important content?

## 2. Indexation

- [ ] Are the right pages indexed?
- [ ] Are the wrong pages indexed (index bloat)?
- [ ] Total crawlable pages vs. total indexed pages (Google Search Console) -- is there a significant gap?
- [ ] Are noindex tags applied correctly?
- [ ] Are canonical tags implemented and pointing to the correct URLs?

## 3. Site Speed

Run PageSpeed Insights on 5-10 key page types. Document scores for mobile and desktop.

| Page Type | Mobile Score | Desktop Score | Target |
|-----------|-------------|---------------|--------|
| Homepage | | | 90+ |
| Category/Service Page | | | 90+ |
| Product/Detail Page | | | 90+ |
| Blog Post | | | 90+ |
| Landing Page | | | 90+ |

## 4. Core Web Vitals

| Metric | Target | Mobile | Desktop | Pass/Fail |
|--------|--------|--------|---------|-----------|
| LCP (Largest Contentful Paint) | <2.5s | | | |
| INP (Interaction to Next Paint) | <200ms | | | |
| CLS (Cumulative Layout Shift) | <0.1 | | | |
| TTFB (Time to First Byte) | <800ms | | | |

## 5. Mobile-Friendliness

- [ ] Responsive design implemented correctly
- [ ] Touch targets are properly sized (minimum 44x44 pixels)
- [ ] Viewport is configured correctly
- [ ] No mobile-specific UX issues (horizontal scroll, overlapping elements)
- [ ] Mobile content parity with desktop

## 6. Structured Data

| Schema Type | Implemented? | Correct? | Opportunity |
|-------------|-------------|----------|-------------|
| Organization | Yes/No | Yes/No/N/A | |
| Breadcrumb | Yes/No | Yes/No/N/A | |
| FAQ | Yes/No | Yes/No/N/A | |
| Product | Yes/No | Yes/No/N/A | |
| Review/Rating | Yes/No | Yes/No/N/A | |
| Article | Yes/No | Yes/No/N/A | |
| Local Business | Yes/No | Yes/No/N/A | |
| How-To | Yes/No | Yes/No/N/A | |

## 7. XML Sitemaps

- [ ] XML sitemap is present and accessible
- [ ] Sitemap has been submitted to Google Search Console
- [ ] Sitemap is accurate (no 404s, no non-canonical URLs)
- [ ] Sitemap is up-to-date (includes all important pages)
- [ ] Sitemap file size is within limits (50,000 URLs / 50MB per file)

## 8. Robots.txt

- [ ] Robots.txt is present and accessible
- [ ] Not blocking any important pages or resources
- [ ] Correctly blocking pages that should not be crawled
- [ ] References XML sitemap location
- [ ] No conflicting directives

## 9. HTTPS & Security

- [ ] Full HTTPS implementation across all pages
- [ ] No mixed content issues (HTTP resources on HTTPS pages)
- [ ] HTTP-to-HTTPS redirects in place
- [ ] Security headers implemented (HSTS, CSP, X-Frame-Options)
- [ ] SSL certificate is valid and not expiring soon

## 10. URL Structure

- [ ] URLs are clean, descriptive, and human-readable
- [ ] URL parameters are handled correctly (not creating duplicate content)
- [ ] No duplicate content from URL variations (trailing slashes, www vs. non-www, case sensitivity)
- [ ] URL depth is reasonable (important pages within 3 levels)

## 11. International/Hreflang (If Applicable)

- [ ] Hreflang tags implemented correctly for all language/region variations
- [ ] Self-referencing hreflang tags present
- [ ] Return tags confirmed (bidirectional)
- [ ] x-default tag present
- [ ] No conflicting hreflang and canonical directives

## 12. Log File Analysis (If Available)

- [ ] Crawl budget is being used efficiently
- [ ] Search engine bots are accessing important pages
- [ ] No excessive crawling of low-value pages
- [ ] Crawl frequency aligns with content update frequency
