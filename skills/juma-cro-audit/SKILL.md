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

Categorize every friction point found across the following dimensions:

**A. Value Proposition and Messaging**
- Is the above-fold headline specific and benefit-oriented?
- Does the subheadline explain how the product/service delivers on the promise?
- Are there clear supporting proof points (stats, logos, awards, certifications)?
- Does the page speak to the visitor's problem before describing the solution?
- Is the language clear and jargon-free for the target audience?

**B. Trust Signals**
- Customer testimonials with names, titles, photos, and company logos?
- Case studies or results with specific metrics?
- Security badges, privacy policies, and compliance certifications?
- Client logos or "as seen in" media mentions?
- Review scores from third-party platforms (G2, Trustpilot, Google Reviews)?
- Money-back guarantees, free trials, or risk-reduction messaging?
- Team photos, about page depth, and transparency signals?

**C. Call-to-Action (CTA) Effectiveness**
- Is there a clear primary CTA on every key page?
- CTA placement: above-fold, mid-page, and bottom-of-page?
- CTA copy: specific and action-oriented, or generic ("Submit", "Click Here")?
- CTA visual contrast: does the button stand out from the surrounding design?
- CTA urgency or scarcity: is there a reason to act now?
- Secondary CTAs for visitors not ready to convert (newsletter, guide, chat)?
- CTA consistency: does the CTA match the page intent and funnel stage?

**D. Form Optimization**
- How many fields? (Every field above 3-4 reduces completion rate)
- Are fields labeled clearly with placeholder text AND labels?
- Inline validation or error handling after submission?
- Progress indicators for multi-step forms?
- Smart defaults and autofill support?
- Mobile-optimized input types (tel, email, number)?
- Are optional fields clearly marked or removed?
- Is the form visible without scrolling?

**E. Page Performance and Technical Friction**
- Page load time on mobile (target: under 3 seconds)
- Layout shifts during loading (CLS issues)
- Broken links, 404 pages, or dead ends in the conversion path
- Pop-ups or overlays that interrupt the conversion journey
- Chat widgets, notification bars, or other elements that obscure content or CTAs

**F. Mobile-Specific Issues**
- Touch targets (minimum 44x44 pixels)
- Mobile-specific CTAs (click-to-call, simplified forms)
- Content readability without zooming
- Sticky navigation or sticky CTAs on mobile
- Accordion/expandable content for long-form mobile pages
- Mobile checkout or form experience vs. desktop

### Step 4: Score by Severity and Opportunity

Rate every finding on two dimensions to build the prioritization matrix:

**Severity (How bad is the current problem?)**
- **High:** Directly causing measurable conversion loss. Significant portion of users affected. Clear evidence in analytics or heatmaps.
- **Medium:** Contributing to conversion friction but not a primary blocker. Moderate user impact.
- **Low:** Minor issue. Affects a small percentage of users or has marginal impact on conversion behavior.

**Opportunity (How much improvement is possible?)**
- **High:** Fixing this could produce a measurable lift (10%+ improvement on the affected metric). Large traffic volume amplifies the impact.
- **Medium:** Expected lift of 3-10% on the affected metric. Moderate traffic volume.
- **Low:** Expected lift of 1-3%. Low traffic volume or niche impact.

Plot every finding on the matrix:

| | **High Opportunity** | **Medium Opportunity** | **Low Opportunity** |
|---|---|---|---|
| **High Severity** | FIX FIRST (P1) | FIX SOON (P2) | SCHEDULE (P3) |
| **Medium Severity** | FIX SOON (P2) | SCHEDULE (P3) | BACKLOG (P4) |
| **Low Severity** | SCHEDULE (P3) | BACKLOG (P4) | BACKLOG (P4) |

### Step 5: Build the Test Roadmap

For every P1 and P2 finding, create a structured test recommendation:

1. **Observation:** What was found (the problem, with evidence)
2. **Hypothesis:** "If we [change], then [metric] will [improve/increase/decrease] because [reasoning based on user behavior or best practice]"
3. **Test type:** A/B test, multivariate test, or direct implementation (for obvious fixes that do not need testing)
4. **Estimated impact:** High / Medium / Low conversion lift
5. **Effort level:** Small (1-2 days), Medium (3-5 days), Large (1-2 weeks), Major (2+ weeks)
6. **Priority:** P1 / P2 / P3
7. **Page(s) affected:** Where to implement
8. **Success metric:** What to measure and minimum detectable effect

Sequence the roadmap into 30/60/90-day sprints.

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

### A. Value Proposition & Messaging

| # | Finding | Severity | Opportunity | Priority | Page(s) |
|---|---------|----------|------------|----------|---------|
| A1 | [Finding: e.g., Homepage headline is generic -- "Welcome to [Company]" does not communicate value] | [High/Med/Low] | [High/Med/Low] | [P1-P4] | [URLs] |
| A2 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |
| A3 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |

### B. Trust Signals

| # | Finding | Severity | Opportunity | Priority | Page(s) |
|---|---------|----------|------------|----------|---------|
| B1 | [Finding: e.g., No customer testimonials on service pages] | [Level] | [Level] | [Priority] | [URLs] |
| B2 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |
| B3 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |

### C. CTA Effectiveness

| # | Finding | Severity | Opportunity | Priority | Page(s) |
|---|---------|----------|------------|----------|---------|
| C1 | [Finding: e.g., Primary CTA button uses low-contrast color and generic "Submit" copy] | [Level] | [Level] | [Priority] | [URLs] |
| C2 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |
| C3 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |

### D. Form Optimization

| # | Finding | Severity | Opportunity | Priority | Page(s) |
|---|---------|----------|------------|----------|---------|
| D1 | [Finding: e.g., Contact form has 12 fields including 6 that are unnecessary for initial inquiry] | [Level] | [Level] | [Priority] | [URLs] |
| D2 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |
| D3 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |

### E. Page Performance & Technical

| # | Finding | Severity | Opportunity | Priority | Page(s) |
|---|---------|----------|------------|----------|---------|
| E1 | [Finding: e.g., Mobile landing page takes 6.2 seconds to load] | [Level] | [Level] | [Priority] | [URLs] |
| E2 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |

### F. Mobile Experience

| # | Finding | Severity | Opportunity | Priority | Page(s) |
|---|---------|----------|------------|----------|---------|
| F1 | [Finding: e.g., CTA button is not visible without scrolling on mobile, and no sticky CTA is present] | [Level] | [Level] | [Priority] | [URLs] |
| F2 | [Finding] | [Level] | [Level] | [Priority] | [URLs] |

---

## Severity x Opportunity Matrix

```
              HIGH OPPORTUNITY    MEDIUM OPPORTUNITY    LOW OPPORTUNITY

HIGH          [Finding IDs]       [Finding IDs]         [Finding IDs]
SEVERITY      FIX FIRST (P1)     FIX SOON (P2)         SCHEDULE (P3)

MEDIUM        [Finding IDs]       [Finding IDs]         [Finding IDs]
SEVERITY      FIX SOON (P2)      SCHEDULE (P3)          BACKLOG (P4)

LOW           [Finding IDs]       [Finding IDs]         [Finding IDs]
SEVERITY      SCHEDULE (P3)      BACKLOG (P4)           BACKLOG (P4)
```

---

## Prioritized Test Roadmap

### P1: Fix First (Highest Leverage)

#### Test 1: [Test Name]
- **Observation:** [What was found, with data]
- **Hypothesis:** If we [change], then [metric] will [improve] because [reasoning]
- **Test Type:** [A/B Test / Direct Implementation]
- **Page(s):** [URLs]
- **Estimated Impact:** [High/Medium/Low] -- [Projected conversion lift: X-X%]
- **Effort:** [Small / Medium / Large / Major]
- **Success Metric:** [What to measure, minimum detectable effect]
- **Timeline:** [Sprint 1: Days 1-30]

#### Test 2: [Test Name]
- **Observation:** [What was found]
- **Hypothesis:** If we [change], then [metric] will [improve] because [reasoning]
- **Test Type:** [A/B Test / Direct Implementation]
- **Page(s):** [URLs]
- **Estimated Impact:** [Level]
- **Effort:** [Level]
- **Success Metric:** [Metric and MDE]
- **Timeline:** [Sprint 1: Days 1-30]

### P2: Fix Soon

#### Test 3: [Test Name]
[Same structure as above]
- **Timeline:** [Sprint 2: Days 31-60]

#### Test 4: [Test Name]
[Same structure as above]
- **Timeline:** [Sprint 2: Days 31-60]

### P3: Schedule

#### Test 5: [Test Name]
[Same structure as above]
- **Timeline:** [Sprint 3: Days 61-90]

#### Test 6: [Test Name]
[Same structure as above]
- **Timeline:** [Sprint 3: Days 61-90]

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
