---
name: juma-cro-audit
description: "Use when a client wants to improve website conversion rates, when landing pages underperform, or when diagnosing why traffic isn't converting. Produces a conversion audit with severity/opportunity scoring and prioritized test roadmap."
---

# CRO (Conversion Rate Optimization) Audit

## Overview

Systematically evaluates a client's website or landing pages for conversion barriers — from value proposition clarity to form friction to mobile experience. Unlike generic UX reviews, this audit produces an actionable test roadmap prioritized by potential revenue impact, giving the client a clear path to measurable improvement.

## When to Use

- Client says "we're getting traffic but not enough leads/sales"
- Landing page conversion rates are below industry benchmarks
- After a website redesign to validate conversion performance
- As part of a comprehensive channel audit or campaign plan
- Client is investing in paid media but ROI is below target
- During quarterly reviews when conversion metrics are trending down

## Prerequisites

- **juma-client-context** — business model, target audience, current conversion rates
- **juma-analytics-setup** (recommended) — ensures clean conversion data exists
- **juma-channel-audit** (recommended) — identifies which channels feed the conversion funnel

## Process

### Step 1: Define Conversion Framework

Map the client's conversion funnel:

1. **Primary conversions**: Purchase, demo request, contact form, signup
2. **Micro-conversions**: Email subscribe, content download, pricing page view, add-to-cart
3. **Baseline metrics**: Current conversion rate per stage, traffic volume, revenue per conversion
4. **Benchmarks**: Industry averages for comparison (by industry, business model, traffic source)

### Step 2: Value Proposition Audit

Evaluate above-the-fold experience on key pages:

1. **Clarity**: Can a visitor understand what you do in 5 seconds?
2. **Relevance**: Does the headline match the traffic source intent?
3. **Differentiation**: Why choose this over competitors?
4. **Proof**: Are credibility signals visible above the fold?
5. **CTA visibility**: Is the primary action obvious?

Score each key landing page 1-10 on value proposition clarity.

### Step 3: User Journey Friction Analysis

Walk through the complete conversion path for each persona:

1. **Entry points**: Top landing pages by traffic volume
2. **Click depth**: How many clicks to convert? (Benchmark: 3 or fewer)
3. **Navigation clarity**: Can users find what they need?
4. **Content sufficiency**: Is enough information provided to make a decision?
5. **Objection handling**: Are common concerns addressed on the page?
6. **Exit points**: Where are users dropping off? (Analytics funnel data)

### Step 4: Trust Signal Assessment

Inventory and evaluate trust elements:

1. **Social proof**: Customer logos, case studies, testimonials, review counts
2. **Authority signals**: Awards, certifications, media mentions, partnerships
3. **Security indicators**: SSL, payment badges, privacy policy visibility
4. **Transparency**: Pricing clarity, no hidden fees, clear refund policy
5. **Contact accessibility**: Phone number, live chat, physical address

### Step 5: CTA Effectiveness Review

For every CTA on key pages:

1. **Copy**: Action-oriented? Specific? Value-communicating? ("Get your free audit" vs "Submit")
2. **Visual prominence**: Color contrast, size, whitespace, position
3. **Placement**: Above fold, after value proposition, at natural decision points
4. **Urgency/scarcity**: Appropriate urgency without being manipulative
5. **Friction level**: What's required to complete the action?

### Step 6: Form Optimization Analysis

For every conversion form:

1. **Field count**: How many fields? (Each field reduces conversions ~7%)
2. **Field types**: Are any unnecessary? Can any be auto-filled?
3. **Labels and placeholders**: Clear, concise, no jargon
4. **Error handling**: Inline validation, helpful error messages, field highlighting
5. **Progress indicators**: For multi-step forms, is progress visible?
6. **Mobile experience**: Touch targets, keyboard types, autocomplete attributes

### Step 7: Mobile Experience Audit

Evaluate mobile-specific conversion factors:

1. **Responsive design**: Layout, readability, image scaling
2. **Touch targets**: Minimum 44x44px, adequate spacing
3. **Page speed**: Mobile-specific load times (target: <3 seconds)
4. **Mobile CTAs**: Click-to-call, simplified forms, mobile payment options
5. **Thumb zone**: Key actions within natural thumb reach
6. **Content prioritization**: Is mobile content hierarchy optimized?

### Step 8: Page-Level Analysis

Audit critical page types:

1. **Homepage**: First impression, navigation, key CTAs
2. **Product/service pages**: Information completeness, comparison tools, CTAs
3. **Pricing page**: Clarity, tier differentiation, FAQ, objection handling
4. **Landing pages**: Message match with ads, single focus, conversion path
5. **Checkout/form pages**: Simplicity, trust, progress, recovery

### Step 9: Score and Prioritize

For each finding, assign:

- **Severity** (High/Medium/Low): How much is this hurting conversions?
- **Opportunity** (High/Medium/Low): How much improvement is possible?
- **Effort** (High/Medium/Low): How hard is this to fix/test?
- **Priority score**: Severity × Opportunity / Effort

### Step 10: Build Test Roadmap

Create prioritized A/B test plan:

1. Sort findings by priority score
2. Formulate hypothesis for each test
3. Estimate sample size and duration
4. Define success metrics per test
5. Group into sprints/phases (quick wins → medium effort → major changes)

## Output Format

```markdown
# CRO Audit: [Client Name]
**Prepared by**: [Agency Name] | **Date**: [Date]

## Executive Summary
- Overall CRO Score: [X/100]
- Estimated conversion rate improvement potential: [X-Y%]
- Estimated annual revenue impact: $[X]
- Critical issues found: [N]
- Top 3 quick wins: [List]

## Current Performance Baseline

| Metric | Current | Industry Benchmark | Gap |
|--------|---------|-------------------|-----|
| Overall conversion rate | [X%] | [X%] | [+/-X%] |
| Mobile conversion rate | [X%] | [X%] | [+/-X%] |
| Cart abandonment rate | [X%] | [X%] | [+/-X%] |
| Bounce rate (key pages) | [X%] | [X%] | [+/-X%] |
| Avg. time to convert | [X] | [X] | [+/-X] |

## Conversion Funnel Analysis

| Stage | Traffic | Conversion Rate | Drop-off | Opportunity |
|-------|---------|-----------------|----------|-------------|
| Landing page → [Next step] | [N] | [X%] | [X%] | [H/M/L] |
| [Step] → [Step] | [N] | [X%] | [X%] | [H/M/L] |
| [Step] → Conversion | [N] | [X%] | [X%] | [H/M/L] |

## Findings by Category

### Value Proposition
| Page | Score | Issue | Severity | Opportunity | Recommendation |
|------|-------|-------|----------|-------------|----------------|
| [URL] | [X/10] | [Issue] | [H/M/L] | [H/M/L] | [Action] |

### User Journey & Friction
[Same table format]

### Trust Signals
[Same table format]

### CTA Effectiveness
[Same table format]

### Form Optimization
[Same table format]

### Mobile Experience
[Same table format]

## Severity × Opportunity Matrix

|            | High Opportunity | Medium Opportunity | Low Opportunity |
|------------|------------------|--------------------|-----------------|
| **High Severity** | [Issues - FIX FIRST] | [Issues] | [Issues] |
| **Medium Severity** | [Issues] | [Issues] | [Issues] |
| **Low Severity** | [Issues] | [Issues] | [Issues - MONITOR] |

## Prioritized Test Roadmap

### Sprint 1: Quick Wins (Weeks 1-2)
| Test # | Hypothesis | Page | Primary Metric | Est. Impact | Effort |
|--------|-----------|------|----------------|-------------|--------|
| 1 | If we [change], then [metric] will [improve] because [reason] | [URL] | [Metric] | [X%] | Low |

### Sprint 2: Medium Effort (Weeks 3-6)
[Same table format]

### Sprint 3: Major Changes (Weeks 7-12)
[Same table format]

## Implementation Notes
- Recommended testing tool: [Tool]
- Minimum sample size per test: [N visitors]
- Statistical significance threshold: 95%
- Estimated test velocity: [N tests/month]

## Appendix
- Screenshot annotations for key findings
- Competitive conversion UX comparison
- Mobile vs desktop performance breakdown
```

## Common Mistakes

- **No baseline data** — Always establish current conversion rates before recommending changes. Can't measure improvement without a baseline
- **Ignoring traffic quality** — Low conversion may be a traffic problem, not a CRO problem. Check traffic source quality first
- **Too many changes at once** — Test one variable at a time. Bundle changes only when they're logically connected
- **Desktop-only audit** — Over 50% of traffic is mobile for most sites. Always audit mobile separately
- **Opinions instead of hypotheses** — Every recommendation should be framed as a testable hypothesis, not "I think this button should be green"
- **Ignoring statistical significance** — Don't call a winner too early. Calculate required sample sizes upfront
- **Missing the revenue math** — Always tie CRO improvements to dollar impact. "2% conversion increase = $X additional revenue"

## Related Skills

- **juma-ab-test-plan** — Detailed test design for top recommendations from this audit
- **juma-analytics-setup** — Ensures conversion tracking is properly configured
- **juma-channel-audit** — Identifies traffic quality issues that affect conversion
- **juma-campaign-plan** — CRO findings inform landing page strategy for campaigns
- **juma-reporting** — CRO test results feed into monthly performance reports
- **juma-upsell-finder** — CRO services are a natural upsell from SEO or paid media
