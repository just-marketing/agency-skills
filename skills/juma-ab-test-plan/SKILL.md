---
name: juma-ab-test-plan
description: "Use when planning A/B tests for landing pages, emails, ads, or website elements. Use when a client wants to test hypotheses about conversion improvements. Produces a structured test plan with hypothesis, sample size calculations, variant design, and results interpretation template."
---

# A/B Test Plan

## Overview

Creates rigorous, data-driven A/B test plans that go beyond "let's try a different button color." Each test plan includes a clear hypothesis, statistical requirements (sample size, duration), variant design, success criteria, and a results interpretation template — plus client communication templates for explaining outcomes to non-technical stakeholders.

## When to Use

- CRO audit has identified testable improvement opportunities
- Client wants to validate a design or messaging change before full rollout
- Campaign performance suggests landing page or creative optimization is needed
- Quarterly planning includes a testing roadmap
- Client asks "should we change X?" — the answer is "let's test it"

## Prerequisites

- **juma-client-context** — business goals, current conversion rates, traffic volumes
- **juma-cro-audit** (recommended) — provides prioritized test opportunities
- **juma-analytics-setup** (recommended) — ensures conversion tracking is in place

## Process

### Step 1: Identify Test Opportunity

From CRO audit findings, campaign data, or client requests:

1. **What's the problem?** — Current state and why it's suboptimal
2. **What's the evidence?** — Data supporting the need for a test (analytics, heatmaps, user feedback)
3. **What's the potential impact?** — Estimated conversion or revenue improvement
4. **Is it testable?** — Sufficient traffic, isolatable variable, measurable outcome

### Step 2: Formulate Hypothesis

Use the structured format:

> **If** we [specific change], **then** [specific metric] will [specific direction by specific amount] **because** [rationale based on evidence or behavioral principle].

Examples:
- "If we shorten the lead form from 8 fields to 4 fields, then form completion rate will increase by 15% because reducing friction lowers abandonment (Hick's Law)."
- "If we add customer testimonials above the fold on the pricing page, then demo request rate will increase by 10% because social proof reduces purchase anxiety."

Bad hypotheses to avoid:
- "If we make the button green, conversions will increase" (no rationale)
- "If we redesign the page, everything will improve" (not specific)

### Step 3: Calculate Sample Size

Determine how many visitors/users are needed per variant:

**Inputs required:**
1. **Baseline conversion rate**: Current rate for the metric being tested
2. **Minimum Detectable Effect (MDE)**: Smallest improvement worth detecting (typically 10-20% relative)
3. **Statistical significance level**: Usually 95% (α = 0.05)
4. **Statistical power**: Usually 80% (β = 0.20)
5. **Number of variants**: Control + 1 or more treatments

**Quick reference table:**

| Baseline Rate | MDE (Relative) | Sample Size Per Variant |
|---------------|----------------|------------------------|
| 1% | 20% | ~160,000 |
| 2% | 20% | ~78,000 |
| 5% | 20% | ~30,000 |
| 10% | 20% | ~14,000 |
| 20% | 20% | ~6,000 |
| 5% | 10% | ~120,000 |
| 10% | 10% | ~57,000 |

**Test duration** = (Sample size per variant × Number of variants) / Daily traffic to the test page

Minimum test duration: 1 full business cycle (typically 1-2 weeks) regardless of sample size to account for day-of-week effects.

### Step 4: Design Variants

For each test variant, document:

1. **Control (A)**: Current experience — describe exactly what it is
2. **Treatment (B)**: Changed experience — describe exactly what changes
3. **Isolation**: Only ONE variable should differ between control and treatment
4. **Visual mockup**: Screenshot or wireframe of each variant
5. **Implementation notes**: What needs to change technically (HTML, CSS, JS, backend)

For multivariate tests (MVT):
- Document all combinations
- Ensure traffic supports the larger sample size requirement
- Note that MVT requires significantly more traffic than A/B

### Step 5: Define Traffic Allocation

1. **Split ratio**: Typically 50/50 for two variants
2. **Ramp-up plan**: Start at 10/90 for 24 hours to catch errors, then scale to 50/50
3. **Targeting**: All visitors or specific segments?
4. **Exclusions**: Returning visitors who saw variant A shouldn't see variant B
5. **Cookie/session duration**: How long does variant assignment persist?

### Step 6: Define Success Metrics

| Metric Type | Description | Example |
|-------------|-------------|---------|
| **Primary metric** | The one metric that determines the winner | Form completion rate |
| **Secondary metrics** | Supporting metrics that provide context | Time on page, scroll depth |
| **Guardrail metrics** | Metrics that must NOT degrade | Revenue per visitor, bounce rate |

- A test is only a winner if the primary metric improves AND guardrail metrics hold
- Document the minimum acceptable threshold for each metric

### Step 7: Segmentation Plan

Define segments to analyze post-test:

1. **Device**: Desktop vs mobile vs tablet
2. **Traffic source**: Organic vs paid vs direct vs referral
3. **Geography**: By region if relevant
4. **User type**: New vs returning visitors
5. **Time**: Weekday vs weekend

Note: Segment analysis is exploratory — don't use it to cherry-pick a winner.

### Step 8: Test Execution Checklist

- [ ] Test tool configured (Google Optimize, VWO, Optimizely, etc.)
- [ ] QA on all devices and browsers
- [ ] Analytics goals tracking correctly for both variants
- [ ] No flicker or layout shift on page load
- [ ] Test documented in testing log/roadmap
- [ ] Stakeholders informed of test start date and expected duration
- [ ] Monitoring plan set (daily check for errors, not for "peeking" at results)

### Step 9: Results Interpretation Framework

When the test reaches required sample size:

1. **Statistical significance**: Is p-value < 0.05?
2. **Practical significance**: Is the actual improvement meaningful for the business?
3. **Confidence interval**: What's the range of likely true effect?
4. **Segment consistency**: Does the result hold across key segments?
5. **Guardrail check**: Did any guardrail metrics degrade?

**Decision framework:**
- Significant + practically meaningful + guardrails hold → **Implement winner**
- Significant but practically small → **Consider implementation cost vs benefit**
- Not significant → **Inconclusive. Consider: was MDE realistic? Was test duration sufficient?**
- Guardrails degraded → **Do not implement, even if primary metric improved**

### Step 10: Client Communication

Prepare results communication in non-technical language:

**Win template:**
> "We tested [change] against the original [page/element]. After [N] visitors over [N] weeks, the new version increased [metric] by [X%], which translates to approximately [Y] additional [conversions/revenue] per month. We recommend implementing this change permanently."

**Loss template:**
> "We tested [change] against the original [page/element]. After [N] visitors over [N] weeks, the original performed better. This is still a valuable result — we now know [what we learned] and can apply this insight to [next test]. Our next test will focus on [next hypothesis]."

**Inconclusive template:**
> "We tested [change] over [N] weeks but didn't see a statistically meaningful difference. This means [change] likely doesn't have a large impact on [metric]. We recommend [next action: extend test, try bigger change, move to next test]."

## Output Format

```markdown
# A/B Test Plan: [Test Name]
**Client**: [Client Name] | **Date**: [Date] | **Test ID**: [ID]

## Hypothesis
If we [specific change], then [metric] will [direction] by [amount] because [rationale].

## Test Parameters

| Parameter | Value |
|-----------|-------|
| Test page/element | [URL or element] |
| Primary metric | [Metric] |
| Baseline rate | [X%] |
| Minimum Detectable Effect | [X% relative] |
| Required sample size (per variant) | [N] |
| Estimated daily traffic | [N] |
| Estimated test duration | [N days/weeks] |
| Statistical significance target | 95% |
| Statistical power | 80% |

## Variants

### Control (A): Current Experience
[Description + screenshot/mockup]

### Treatment (B): Changed Experience
[Description + screenshot/mockup]

**Isolated variable**: [What exactly changes between A and B]

## Success Criteria

| Metric | Type | Target | Min. Acceptable |
|--------|------|--------|-----------------|
| [Primary metric] | Primary | +[X%] | +[Y%] |
| [Secondary metric] | Secondary | Directional improvement | — |
| [Guardrail metric] | Guardrail | No degradation | >[X%] |

## Traffic Allocation
- Split: [50/50]
- Targeting: [All visitors / Specific segments]
- Ramp-up: [10/90 for 24h, then 50/50]

## Segmentation Analysis Plan
- [ ] Device type
- [ ] Traffic source
- [ ] New vs returning
- [ ] [Other relevant segments]

## Implementation Checklist
- [ ] Test configured in [tool]
- [ ] QA complete (desktop, mobile, tablet)
- [ ] Conversion tracking verified
- [ ] Stakeholders notified
- [ ] Start date: [Date]
- [ ] Expected end date: [Date]

## Results Template
[Pre-formatted table for recording results when test concludes]

| Metric | Control | Treatment | Difference | Significance |
|--------|---------|-----------|------------|--------------|
| [Primary] | — | — | — | — |
| [Secondary] | — | — | — | — |
| [Guardrail] | — | — | — | — |
```

## Common Mistakes

- **Peeking at results** — Checking daily and stopping early when results look good inflates false positive rates. Wait for full sample size
- **Testing too many variables** — Multivariate tests need exponentially more traffic. Start with simple A/B tests
- **Unrealistic MDE** — Hoping to detect a 2% improvement with 500 visitors/day means a test lasting months. Be realistic about detectable effects
- **No guardrail metrics** — A test that increases signups but tanks revenue is not a win. Always define guardrails
- **Ignoring seasonal effects** — Don't run tests across major holidays or events. Results will be confounded
- **Declaring a winner without significance** — "Variant B has a higher number" is not the same as "Variant B is statistically significantly better"
- **Not documenting learnings** — Every test, win or lose, generates knowledge. Maintain a testing log

## Related Skills

- **juma-cro-audit** — Generates the prioritized test opportunities this skill operationalizes
- **juma-campaign-plan** — Campaign-level experiments use this test planning framework
- **juma-analytics-setup** — Conversion tracking must be configured before testing
- **juma-reporting** — Test results feed into monthly performance reports
- **juma-paid-media-plan** — Ad creative testing follows this same methodology
