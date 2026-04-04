# Test Recommendation Template

Use this structured template for every P1 and P2 finding in the CRO audit test roadmap. Each test recommendation must include all fields below to be actionable.

---

## Test Recommendation Format

### Test [#]: [Test Name]

- **Observation:** [What was found -- the problem, with supporting data from analytics, heatmaps, or manual review]
- **Hypothesis:** If we [specific change], then [specific metric] will [improve/increase/decrease] because [reasoning based on user behavior evidence or established best practice]
- **Test Type:** [A/B Test / Multivariate Test / Direct Implementation]
- **Page(s):** [Specific URLs where the test will be implemented]
- **Estimated Impact:** [High / Medium / Low] -- [Projected conversion lift: X-X%]
- **Effort:** [Small (1-2 days) / Medium (3-5 days) / Large (1-2 weeks) / Major (2+ weeks)]
- **Priority:** [P1 / P2 / P3]
- **Success Metric:** [What to measure and minimum detectable effect (MDE)]
- **Timeline:** [Sprint assignment: Days 1-30 / Days 31-60 / Days 61-90]

---

## Test Type Decision Guide

| Scenario | Recommended Test Type |
|----------|----------------------|
| Clear best-practice violation with strong evidence | **Direct Implementation** -- no need to test the obvious |
| Single variable change with measurable impact | **A/B Test** -- isolate the variable and measure lift |
| Multiple interacting variables on one page | **Multivariate Test** -- test combinations simultaneously |
| Low-traffic page (insufficient data for statistical significance) | **Direct Implementation** -- A/B test would take too long to reach significance |

---

## Effort Level Definitions

| Level | Duration | Typical Scope |
|-------|----------|--------------|
| **Small** | 1-2 days | Copy change, CTA color/text, adding a trust badge, reordering page sections |
| **Medium** | 3-5 days | Form redesign, new page section, hero rewrite with design, adding testimonials |
| **Large** | 1-2 weeks | Landing page rebuild, multi-step form redesign, new conversion path |
| **Major** | 2+ weeks | Site-wide navigation change, checkout flow overhaul, new page template |

---

## Sprint Sequencing

### Sprint 1: Days 1-30 (P1 Tests)

| Test # | Test Name | Type | Effort | Est. Impact |
|--------|-----------|------|--------|-------------|
| 1 | [Name] | [Type] | [Effort] | [Impact] |
| 2 | [Name] | [Type] | [Effort] | [Impact] |

### Sprint 2: Days 31-60 (P2 Tests)

| Test # | Test Name | Type | Effort | Est. Impact |
|--------|-----------|------|--------|-------------|
| 3 | [Name] | [Type] | [Effort] | [Impact] |
| 4 | [Name] | [Type] | [Effort] | [Impact] |

### Sprint 3: Days 61-90 (P3 Tests)

| Test # | Test Name | Type | Effort | Est. Impact |
|--------|-----------|------|--------|-------------|
| 5 | [Name] | [Type] | [Effort] | [Impact] |
| 6 | [Name] | [Type] | [Effort] | [Impact] |

---

## Hypothesis Writing Guide

A strong hypothesis follows this pattern:

> **If we** [make this specific change] **then** [this specific metric] **will** [improve in this direction] **because** [this is what we know about user behavior or best practices that supports this prediction].

**Good example:** "If we reduce the contact form from 12 fields to 4 (name, email, company, message), then form completion rate will increase by 15-25% because form analytics show 62% of users abandon after field 5, and industry benchmarks show each field above 4 reduces completion by approximately 5%."

**Weak example:** "If we change the form, conversions will go up because shorter forms are better."
