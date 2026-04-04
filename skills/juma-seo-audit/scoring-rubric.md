# SEO Audit Scoring Rubric

This rubric defines the weighted scoring system used to calculate the overall SEO Health Score. Each pillar is scored independently on a 0-100 scale, then weighted to produce the final score.

---

## Pillar Weights

| Pillar | Weight | Rationale |
|--------|--------|-----------|
| **Technical SEO** | 30% | Foundation -- crawlability, speed, and indexation gate all other SEO performance |
| **On-Page SEO** | 25% | Direct ranking signals -- title tags, headings, internal links, content optimization |
| **Content** | 25% | Depth, coverage, and quality of content determine topical authority and keyword reach |
| **Backlinks** | 20% | Off-site authority signals -- link quality, volume, and growth trajectory |

---

## Score Calculation

### SEO Health Score Table

| Pillar | Score | Weight | Weighted Score |
|--------|-------|--------|----------------|
| Technical SEO | [X/100] | 30% | [X] |
| On-Page SEO | [X/100] | 25% | [X] |
| Content | [X/100] | 25% | [X] |
| Backlinks | [X/100] | 20% | [X] |
| **Overall** | | **100%** | **[X/100]** |

**Formula:** Overall Score = (Technical x 0.30) + (On-Page x 0.25) + (Content x 0.25) + (Backlinks x 0.20)

---

## Severity-Based Scoring

Each pillar starts at 100 and deducts points based on the severity of issues found:

| Severity Level | Point Deduction Per Issue | Description |
|---------------|--------------------------|-------------|
| **Critical** | -15 to -20 points | Site-breaking issues that prevent indexing, cause major traffic loss, or create security vulnerabilities |
| **High** | -8 to -12 points | Significant issues with measurable negative impact on rankings or traffic |
| **Medium** | -3 to -5 points | Moderate issues that contribute to suboptimal performance |
| **Low** | -1 to -2 points | Minor issues with marginal impact |

---

## Score Interpretation

| Score Range | Health Level | Interpretation |
|-------------|-------------|----------------|
| **90-100** | Excellent | SEO fundamentals are strong. Focus on advanced optimization and competitive edge. |
| **75-89** | Good | Solid foundation with specific areas to improve. Targeted fixes will yield gains. |
| **60-74** | Fair | Multiple issues affecting performance. Structured remediation plan needed. |
| **40-59** | Poor | Significant problems across pillars. Prioritize critical fixes immediately. |
| **0-39** | Critical | Major structural issues. SEO is likely suppressed. Requires urgent, comprehensive remediation. |

---

## Issue Categorization Guide

### Critical Issues (Fix Immediately)
- robots.txt blocking important pages
- Noindex tags on key pages
- Site-wide HTTPS issues
- Severe Core Web Vitals failures on key pages
- Major crawl errors (5xx on important pages)
- Manual penalties or security issues

### High Priority Issues (Fix Within 30 Days)
- Missing or duplicate title tags on high-traffic pages
- Significant page speed issues (LCP > 4s)
- Broken internal links on key conversion paths
- Thin content on pages targeting high-value keywords
- Toxic backlink profile requiring disavow

### Medium Priority Issues (Fix Within 60 Days)
- Missing meta descriptions
- Image optimization (alt text, file size)
- Incomplete structured data implementation
- Content freshness issues on aging pages
- Anchor text profile imbalance

### Low Priority Issues (Fix Within 90 Days)
- Minor URL structure improvements
- Non-critical schema additions
- Low-traffic page optimizations
- Nice-to-have internal linking improvements
