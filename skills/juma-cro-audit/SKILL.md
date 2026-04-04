---
name: juma-cro-audit
description: "Use when a client's website traffic is healthy but conversions are underperforming, when onboarding a new client to identify conversion bottlenecks, or when building a testing roadmap to improve lead generation, sales, or sign-up rates."
---

# Conversion Rate Optimization (CRO) Audit

## Overview

The CRO Audit systematically evaluates a website's ability to convert visitors into leads, customers, or subscribers. It walks the entire user journey from landing to conversion, identifies friction points at every stage, and produces a prioritized test roadmap with a hypothesis, estimated impact, and effort level for each recommended experiment.

Unlike a general UX review, this audit is conversion-focused -- every finding is evaluated through the lens of its impact on measurable business outcomes. The audit uses a Severity x Opportunity matrix to ensure the team works on the highest-leverage improvements first, not just the most visible ones.

This is one of the highest-ROI audits an agency can deliver. Even small conversion rate improvements compound across all traffic sources, making every dollar spent on SEO, paid media, and content marketing more effective.

## When to Use

- A client's traffic is growing but conversions are flat or declining
- New client onboarding to identify quick conversion wins
- Before launching a paid media campaign (no point driving traffic to a leaky funnel)
- Quarterly conversion review to keep the test pipeline full
- After a site redesign or major page changes to ensure conversion was not sacrificed for aesthetics
- When a client asks "why aren't we getting more leads/sales from our website?"
- As a complement to a juma-seo-audit or juma-channel-audit (traffic x conversion = revenue)
- When building a proposal that includes CRO or landing page optimization services

## Prerequisites

- **juma-client-context** (required) -- business goals, target audiences, conversion KPIs, and current performance baselines
- Access to Google Analytics (GA4) with conversion tracking properly configured
- Access to the live website for manual walkthrough
- Heatmap/session recording data if available (Hotjar, Microsoft Clarity, FullStory, or equivalent)
- Knowledge of the client's primary conversion actions (form fill, purchase, demo request, sign-up, phone call, etc.)
- Current conversion rates by page type and traffic source
- Understanding of the client's sales funnel downstream of website conversion (for lead-gen businesses)

## Process

### Step 1: Review Analytics Funnel

Before touching the website, understand the data:

1. **Map the conversion funnel in GA4:** Identify every step from session start to conversion completion. Document drop-off rates at each stage.
2. **Segment by traffic source:** Conversion rates vary dramatically by source. Break down performance by organic, paid, social, email, direct, and referral.
3. **Segment by device:** Compare mobile vs. desktop vs. tablet conversion rates. Flag significant gaps (mobile conversion rate less than 50% of desktop is a red flag).
4. **Identify top landing pages by volume:** Which pages receive the most traffic? What are their individual conversion rates?
5. **Identify worst-performing pages:** Which high-traffic pages have the lowest conversion rates? These are the highest-leverage optimization targets.
6. **Review exit pages:** Where are users leaving the site? Map the most common exit points in the conversion funnel.
7. **Check form analytics (if available):** Form abandonment rates, which fields cause drop-off, time to complete forms.
8. **Review site search data:** What are users searching for on-site? Failed searches often reveal navigation or content gaps.

### Step 2: Walk the User Journey

Manually complete the conversion journey as each primary audience segment would:

1. **First impression (0-5 seconds):** On each key landing page, can a new visitor immediately understand what the company does, who it is for, and what action to take? Document the above-fold experience.
2. **Value proposition clarity:** Is the value proposition specific and differentiated, or generic? Does it address the visitor's problem or just describe the product?
3. **Navigation and information architecture:** Can users find what they need in 3 clicks or fewer? Is the navigation intuitive or overwhelming?
4. **Content flow:** Does the page guide the user logically from problem awareness to solution to action? Or does the user have to work to understand the offer?
5. **Conversion path:** How many steps from landing to conversion? Count every click, scroll, and form field. Map the path for each conversion type.
6. **Mobile journey:** Repeat the walkthrough on mobile. Note any mobile-specific friction (tiny tap targets, horizontal scroll, overlays, slow-loading elements).
7. **Cross-device journey:** If the buying process spans multiple sessions, how well does the site support returning visitors?

### Step 3: Identify Friction Points

Categorize every friction point found across 6 dimensions (A-F): Value Proposition & Messaging, Trust Signals, CTA Effectiveness, Form Optimization, Page Performance & Technical Friction, and Mobile-Specific Issues.

See [friction-point-framework.md](friction-point-framework.md) for the complete A-F categorization framework with checklists and finding templates for each dimension.

### Step 4: Score by Severity and Opportunity

Rate every finding on two independent dimensions -- Severity (how bad is the problem?) and Opportunity (how much improvement is possible?) -- then plot on the prioritization matrix to determine P1-P4 priority.

See [severity-opportunity-matrix.md](severity-opportunity-matrix.md) for the complete matrix, rating guides for both dimensions, and priority level definitions.

### Step 5: Build the Test Roadmap

For every P1 and P2 finding, create a structured test recommendation and sequence the roadmap into 30/60/90-day sprints.

See [test-recommendation-template.md](test-recommendation-template.md) for the complete test recommendation format, test type decision guide, effort level definitions, sprint sequencing tables, and hypothesis writing guide.

## Output Format

```markdown
# CRO Audit: [Client Name]

**Prepared by:** [Agency Name]
**Date:** [Date]
**Website:** [URL]
**Period Analyzed:** [Date Range]
**Primary Conversion Actions:** [List: e.g., Demo request, Free trial sign-up, Purchase]

---

## Executive Summary

[2-3 paragraphs summarizing the overall conversion health of the site, the most significant friction points, and the estimated revenue impact of recommended improvements. Include current baseline conversion rate and projected improvement range.]

### Current Conversion Performance

| Metric | Value | Industry Benchmark | Assessment |
|--------|-------|--------------------|------------|
| Overall Conversion Rate | [X%] | [Benchmark%] | [Above/Below by X%] |
| Mobile Conversion Rate | [X%] | [Benchmark%] | [Above/Below by X%] |
| Desktop Conversion Rate | [X%] | [Benchmark%] | [Above/Below by X%] |
| Form Completion Rate | [X%] | [Benchmark%] | [Above/Below by X%] |
| Cart Abandonment Rate | [X%] (if e-commerce) | [Benchmark%] | [Above/Below by X%] |
| Avg. Pages to Conversion | [X] | -- | [Assessment] |

### Impact Projection

If the recommended optimizations achieve a conservative [X%] lift in conversion rate:
- **Current monthly conversions:** [X]
- **Projected monthly conversions:** [X] (+[X] additional)
- **Estimated additional monthly revenue:** $[X]
- **Estimated annual revenue impact:** $[X]

---

## Funnel Analysis

### Conversion Funnel Drop-Off

| Funnel Stage | Users | Drop-Off Rate | Key Issue |
|-------------|-------|--------------|-----------|
| Landing Page | [X] | -- | [Issue if any] |
| Engagement (scroll/click) | [X] | [X%] drop-off | [Issue] |
| CTA Click / Add to Cart | [X] | [X%] drop-off | [Issue] |
| Form Start / Checkout Start | [X] | [X%] drop-off | [Issue] |
| Form Complete / Purchase | [X] | [X%] drop-off | [Issue] |

### Performance by Traffic Source

| Source | Sessions | Conversion Rate | Revenue/Leads | Assessment |
|--------|----------|-----------------|---------------|------------|
| Organic Search | [X] | [X%] | [X] | [Finding] |
| Paid Search | [X] | [X%] | [X] | [Finding] |
| Paid Social | [X] | [X%] | [X] | [Finding] |
| Email | [X] | [X%] | [X] | [Finding] |
| Direct | [X] | [X%] | [X] | [Finding] |
| Referral | [X] | [X%] | [X] | [Finding] |

### Performance by Device

| Device | Sessions | Conv. Rate | Gap vs. Desktop | Key Issues |
|--------|----------|-----------|-----------------|------------|
| Desktop | [X] | [X%] | -- | [Notes] |
| Mobile | [X] | [X%] | [X% lower] | [Specific mobile issues] |
| Tablet | [X] | [X%] | [X% lower/higher] | [Notes] |

---

## Findings by Category

Document findings across all 6 categories (A-F). See [friction-point-framework.md](friction-point-framework.md) for the category checklists and finding table templates for each dimension.

---

## Severity x Opportunity Matrix

See [severity-opportunity-matrix.md](severity-opportunity-matrix.md) for the complete matrix layout and populate with finding IDs from the categories above.

---

## Prioritized Test Roadmap

See [test-recommendation-template.md](test-recommendation-template.md) for the complete test recommendation format. Create entries for all P1, P2, and P3 findings, organized into 30/60/90-day sprints.

---

## Page-Level Recommendations

### Homepage

| Issue | Recommendation | Priority | Effort |
|-------|---------------|----------|--------|
| [Issue] | [Specific recommendation] | [P1-P4] | [Effort level] |
| [Issue] | [Specific recommendation] | [P1-P4] | [Effort level] |

### [Key Landing Page 1]

| Issue | Recommendation | Priority | Effort |
|-------|---------------|----------|--------|
| [Issue] | [Specific recommendation] | [P1-P4] | [Effort level] |

### [Key Landing Page 2]

| Issue | Recommendation | Priority | Effort |
|-------|---------------|----------|--------|
| [Issue] | [Specific recommendation] | [P1-P4] | [Effort level] |

### [Product/Service Pages]

| Issue | Recommendation | Priority | Effort |
|-------|---------------|----------|--------|
| [Issue] | [Specific recommendation] | [P1-P4] | [Effort level] |

### [Checkout/Form Pages]

| Issue | Recommendation | Priority | Effort |
|-------|---------------|----------|--------|
| [Issue] | [Specific recommendation] | [P1-P4] | [Effort level] |

---

## Appendix: Data Sources & Methodology

- **Analytics:** [Tool, date range, conversion definitions]
- **Heatmaps/Session Recordings:** [Tool, sample size, date range]
- **Manual Walkthrough:** [Devices tested, browsers tested, date]
- **Industry Benchmarks:** [Sources used for benchmark data]
- **Scoring Methodology:** Severity and Opportunity are rated independently on a High/Medium/Low scale. Priority is determined by the intersection on the Severity x Opportunity matrix. Revenue impact projections use the client's current conversion rate, traffic volume, and average order value/deal size.
```

## Common Mistakes

- **Auditing design instead of conversion** -- This is not a UX or visual design review. Every finding must connect to a measurable conversion impact. "The hero image is low quality" is a design opinion. "The hero section has no value proposition or CTA above the fold, and 68% of mobile users leave without scrolling" is a conversion finding.
- **Recommending changes without hypotheses** -- "Change the CTA color to green" is not a recommendation. "Test a high-contrast CTA color against the current low-contrast button, hypothesizing a 5-10% increase in CTA click-through rate based on the current 2% CTR being below the 4% benchmark" is a recommendation.
- **Ignoring mobile** -- If mobile conversion rate is significantly lower than desktop (common), the mobile experience deserves its own dedicated section. Do not assume the desktop audit covers mobile issues.
- **Not segmenting by traffic source** -- A page may convert well for email traffic but poorly for paid search because the messaging does not match the ad copy. Always segment conversion data by source to find source-specific friction.
- **Too many tests at once** -- A 30-item test roadmap overwhelms the client. Prioritize ruthlessly. Present 6-10 tests in a 90-day roadmap with clear sequencing. Keep the rest in a backlog.
- **Skipping the revenue projection** -- Clients approve CRO work when they see the revenue impact. Always calculate: current conversions x projected lift = additional conversions x average order value or deal size = revenue impact. This is the single most persuasive element of the audit.
- **Testing trivial changes** -- Button color tests and minor copy tweaks rarely produce meaningful lifts. Focus on structural changes: value proposition, social proof placement, form reduction, page layout, and conversion path simplification.
- **Forgetting downstream conversion quality** -- A higher form submission rate is meaningless if the leads are lower quality. For lead-gen businesses, always consider lead quality and sales-qualified lead rates alongside volume.

## Related Skills

- **juma-client-context** -- provides conversion KPIs, audience segments, and performance baselines for the audit
- **juma-seo-audit** -- SEO drives traffic, CRO converts it; findings from both audits should cross-reference
- **juma-channel-audit** -- conversion rates by channel inform which channels deserve more or less investment
- **juma-campaign-plan** -- CRO findings ensure campaign landing pages are optimized before launch
- **juma-ab-test-plan** -- the test roadmap from this audit feeds directly into detailed A/B test plans
- **juma-reporting** -- ongoing CRO reporting tracks test results and conversion rate trends
- **juma-proposal** -- CRO audit findings with revenue projections make a compelling case in proposals
- **juma-upsell-finder** -- CRO is a natural upsell for any client investing in traffic generation
