# Technical SEO Checklist

Use this checklist when evaluating the Technical SEO pillar (30% weight) of the SEO audit. Each item should be assessed and scored for the overall technical health score.

---

## 1. Crawlability & Indexation

- [ ] **Crawl all pages** -- Capture HTTP status codes, redirects, canonical tags, and meta data
- [ ] **Identify crawl errors** -- Document all 4xx and 5xx errors
- [ ] **Check redirect chains** -- Flag chains of 2+ redirects; note the longest chain
- [ ] **Find orphan pages** -- Pages with no internal links pointing to them
- [ ] **Review XML sitemaps** -- Present, submitted to GSC, accurate, no errors
- [ ] **Review robots.txt** -- Check for unintentional blocks on important pages
- [ ] **Compare crawlable vs. indexed pages** -- GSC index coverage vs. crawl count
- [ ] **Check JavaScript rendering** -- Verify JS-dependent content is accessible to crawlers

### Output Table

| Check | Status | Details |
|-------|--------|---------|
| Total pages crawled | [Number] | [Notes] |
| Pages indexed (GSC) | [Number] | [Indexed vs. crawled gap analysis] |
| Crawl errors (4xx) | [Count] | [Top errors listed] |
| Crawl errors (5xx) | [Count] | [Top errors listed] |
| Redirect chains | [Count] | [Longest chain noted] |
| Orphan pages | [Count] | [Impact assessment] |
| XML sitemap | [Present/Missing] | [Errors or issues] |
| Robots.txt | [Correct/Issues] | [Specific problems] |

---

## 2. Site Speed & Core Web Vitals

Test 5-10 key page types using PageSpeed Insights / Lighthouse.

- [ ] **PageSpeed Score** -- Mobile and desktop (target: 90+)
- [ ] **LCP (Largest Contentful Paint)** -- Target: <2.5s
- [ ] **INP (Interaction to Next Paint)** -- Target: <200ms
- [ ] **CLS (Cumulative Layout Shift)** -- Target: <0.1
- [ ] **TTFB (Time to First Byte)** -- Target: <800ms

### Output Table

| Metric | Mobile | Desktop | Target | Status |
|--------|--------|---------|--------|--------|
| PageSpeed Score | [Score] | [Score] | 90+ | [Pass/Fail] |
| LCP | [Time] | [Time] | <2.5s | [Pass/Fail] |
| INP | [Time] | [Time] | <200ms | [Pass/Fail] |
| CLS | [Score] | [Score] | <0.1 | [Pass/Fail] |
| TTFB | [Time] | [Time] | <800ms | [Pass/Fail] |

### Page-Level Breakdown

| Page Type | Mobile Score | LCP | INP | CLS |
|-----------|-------------|-----|-----|-----|
| Homepage | [Score] | [Time] | [Time] | [Score] |
| Category/Service | [Score] | [Time] | [Time] | [Score] |
| Product/Detail | [Score] | [Time] | [Time] | [Score] |
| Blog Post | [Score] | [Time] | [Time] | [Score] |
| Landing Page | [Score] | [Time] | [Time] | [Score] |

---

## 3. Mobile-Friendliness

- [ ] **Responsive design** -- Pages render correctly across viewport sizes
- [ ] **Touch targets** -- All interactive elements meet minimum size (44x44px)
- [ ] **Viewport configuration** -- Proper meta viewport tag
- [ ] **Mobile-specific UX** -- No horizontal scroll, text readable without zoom

---

## 4. Structured Data

- [ ] **Audit current schema markup** -- List all implemented types
- [ ] **Validate implementation** -- Check for errors via Google Rich Results Test
- [ ] **Identify missing opportunities** -- Compare against relevant schema types

### Output Table

| Schema Type | Implemented | Correct | Opportunity |
|-------------|------------|---------|-------------|
| Organization | [Yes/No] | [Yes/No/N/A] | [Notes] |
| Breadcrumb | [Yes/No] | [Yes/No/N/A] | [Notes] |
| FAQ | [Yes/No] | [Yes/No/N/A] | [Notes] |
| Product | [Yes/No] | [Yes/No/N/A] | [Notes] |
| Review/Rating | [Yes/No] | [Yes/No/N/A] | [Notes] |
| Article | [Yes/No] | [Yes/No/N/A] | [Notes] |
| Local Business | [Yes/No] | [Yes/No/N/A] | [Notes] |
| How-To | [Yes/No] | [Yes/No/N/A] | [Notes] |

---

## 5. HTTPS & Security

- [ ] **Full HTTPS implementation** -- All pages served over HTTPS
- [ ] **Mixed content** -- No HTTP resources loaded on HTTPS pages
- [ ] **Security headers** -- HSTS, X-Content-Type-Options, X-Frame-Options assessed

---

## 6. URL Structure

- [ ] **Clean, descriptive URLs** -- Human-readable, keyword-relevant
- [ ] **Parameter handling** -- No duplicate content from URL parameters
- [ ] **Duplicate URL variations** -- Trailing slashes, www vs. non-www, HTTP vs. HTTPS all canonicalized

---

## 7. International / Hreflang (If Applicable)

- [ ] **Hreflang tags** -- Correct implementation for language/region targeting
- [ ] **Return links** -- Bidirectional hreflang references between language versions
- [ ] **x-default** -- Default language version specified

---

## 8. Log File Analysis (If Available)

- [ ] **Crawl budget efficiency** -- Are search engines spending crawl budget on important pages?
- [ ] **Bot frequency** -- How often are key pages crawled?
- [ ] **Wasted crawl budget** -- Are bots crawling low-value pages (filters, parameters, etc.)?
