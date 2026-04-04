---
name: juma-reporting
description: "Use when producing a monthly or weekly client performance report that combines data analysis with strategic storytelling. Produces a structured report with executive summary, KPI dashboard, channel-by-channel performance, wins and losses analysis, budget utilization, and forward-looking recommendations."
---

# Client Performance Report

## Overview

The Client Performance Report transforms raw marketing data into a narrative that busy executives can act on. This is not a data dump -- it is a storytelling document that answers three questions every client has: "What happened?", "So what?", and "Now what?" Great reporting is the single highest-leverage retention tool an agency has. Clients do not churn from agencies that consistently demonstrate they understand the numbers, own the outcomes, and have a clear plan for what comes next.

This skill produces reports that lead with insights rather than metrics, address bad news proactively with remediation plans, and always connect tactical performance back to the client's business objectives.

## When to Use

- Monthly performance reporting to clients (standard cadence)
- Weekly pulse reports for high-spend or high-velocity engagements
- Ad-hoc performance reports requested by clients after a campaign, launch, or event
- Building the data foundation for a quarterly business review (juma-client-qbr)
- When a client asks "how are we doing?" and needs more than a verbal answer

## Prerequisites

- **juma-client-context**: Must be populated with client KPIs, targets, baselines, channel strategy, and business goals to contextualize performance data
- **juma-sow** (recommended): Defines the deliverables and success criteria that the report should measure against
- Access to performance data from all active channels (GA4, ad platforms, email platform, social analytics, CRM)
- Previous period report for period-over-period comparison consistency
- Confirmed client KPI targets and budget allocations for the reporting period
- Knowledge of any campaigns, launches, or external events that occurred during the period

## Process

1. **Pull performance data**: Collect data from every active channel for the reporting period. Pull the same metrics from the previous period and the same period last year (if available) for comparison. Ensure data sources are consistent with prior reports -- switching attribution models or date ranges mid-engagement destroys trend analysis credibility.

2. **Calculate period-over-period changes**: For every KPI and channel metric, calculate the change from the previous period (absolute and percentage). Flag any metric that moved more than 15% in either direction -- these are the stories in your data. Calculate progress toward period targets and annual goals.

3. **Identify stories in the data**: Behind every significant metric movement is a story. Correlate performance changes with known activities: campaigns launched, budget changes, algorithm updates, seasonal patterns, competitor moves, or client-side changes (new product, pricing change, PR event). Every significant number needs a "why."

4. **Write the "so what?" analysis**: For each key finding, translate the data into business impact. "Organic traffic increased 23%" is a metric. "Organic traffic increased 23% driven by the pillar content strategy launched in Month 2, contributing an estimated $[X] in pipeline value" is an insight. Connect every metric to revenue, leads, or strategic progress.

5. **Draft recommendations**: For every underperforming area, include a specific remediation plan with timeline. For every outperforming area, include a plan to double down or replicate the success. Recommendations must be actionable -- include what, who, when, and expected impact. Never present a problem without a proposed solution.

6. **Compile the report**: Assemble all sections in the output format below. Write the executive summary last -- it should distill the entire report into 3-5 key takeaways that a CEO could read in 90 seconds and understand the health of the engagement.

## Output Format

```
# [Client Name] Performance Report

**Period:** [Month/Week and Year]
**Prepared by:** [Name, Title]
**Date:** [Date]

---

## Executive Summary

[3-5 bullet points, each one sentence, covering the most important takeaways for the period. Lead with the single most impactful finding. Format: what happened + why it matters + what we are doing about it. This section must stand alone -- many executives read only this.]

- **[Key Takeaway 1]:** [What happened, why it matters, what's next]
- **[Key Takeaway 2]:** [What happened, why it matters, what's next]
- **[Key Takeaway 3]:** [What happened, why it matters, what's next]
- **[Key Takeaway 4]:** [What happened, why it matters, what's next]
- **[Key Takeaway 5]:** [What happened, why it matters, what's next]

**Overall Health:** [On Track / Watch / Off Track] toward [quarterly/annual] goals

---

## KPI Dashboard

See [kpi-dashboard-template.md](kpi-dashboard-template.md) for the complete KPI dashboard table structure.

---

## Channel Performance

See [channel-performance-template.md](channel-performance-template.md) for the per-channel performance section template with channel-specific metric sets (Organic Search, Paid Search, Paid Social, Organic Social, Email Marketing) and analysis guidelines. Add additional channels as relevant.

---

## What Worked: Wins This Period

### Win 1: [Headline - Specific and Quantified]
[2-3 sentences describing what was done, what the result was, and what it means for the business. Attribute the win to a specific action or strategy.]

### Win 2: [Headline - Specific and Quantified]
[2-3 sentences describing what was done, what the result was, and what it means for the business.]

### Win 3: [Headline - Specific and Quantified]
[2-3 sentences describing what was done, what the result was, and what it means for the business.]

---

## What Didn't Work: Challenges & Remediation

### Challenge 1: [Headline - Specific and Honest]
- **What happened:** [Factual description of the underperformance]
- **Why:** [Root cause analysis -- not excuses, but genuine understanding]
- **What we are doing about it:** [Specific remediation plan with timeline and expected impact]

### Challenge 2: [Headline - Specific and Honest]
- **What happened:** [Factual description]
- **Why:** [Root cause analysis]
- **What we are doing about it:** [Specific remediation plan]

---

## Content & Campaign Highlights

| Campaign / Content Piece | Channel | Goal | Result | Status |
|---|---|---|---|---|
| [Campaign Name] | [Channel] | [Target metric] | [Actual metric] | [Exceeded / Met / Below] |
| [Campaign Name] | [Channel] | [Target metric] | [Actual metric] | [Exceeded / Met / Below] |
| [Content Piece] | [Channel] | [Target metric] | [Actual metric] | [Exceeded / Met / Below] |

**Key Insight:** [1-2 sentences on the pattern or learning from campaign/content performance this period]

---

## Budget Utilization

| Channel / Line Item | Planned Spend | Actual Spend | Variance | Notes |
|---|---|---|---|---|
| [Channel 1] | $[Value] | $[Value] | [+/-$X / +/-X%] | [Explanation if variance > 10%] |
| [Channel 2] | $[Value] | $[Value] | [+/-$X / +/-X%] | [Explanation if variance > 10%] |
| [Channel 3] | $[Value] | $[Value] | [+/-$X / +/-X%] | [Explanation if variance > 10%] |
| Agency Fees | $[Value] | $[Value] | [+/-$X / +/-X%] | [Notes] |
| **Total** | **$[Value]** | **$[Value]** | **[+/-$X / +/-X%]** | |

**Budget Efficiency:** [1-2 sentences on overall budget utilization effectiveness and any reallocation recommendations]

---

## Next Period: Priorities & Planned Actions

### Priority 1: [Action with Expected Impact]
- **What:** [Specific description of what will be done]
- **Why:** [Business rationale tied to data from this report]
- **Expected Impact:** [Quantified projection]
- **Timeline:** [When it will start, when results are expected]

### Priority 2: [Action with Expected Impact]
- **What:** [Specific description]
- **Why:** [Business rationale]
- **Expected Impact:** [Quantified projection]
- **Timeline:** [Start and result dates]

### Priority 3: [Action with Expected Impact]
- **What:** [Specific description]
- **Why:** [Business rationale]
- **Expected Impact:** [Quantified projection]
- **Timeline:** [Start and result dates]

---

## Appendix: Raw Data

### Website Traffic Summary
| Metric | [Current Period] | [Previous Period] | [Same Period Last Year] |
|---|---|---|---|
| Total Sessions | [Value] | [Value] | [Value] |
| Unique Visitors | [Value] | [Value] | [Value] |
| Pages per Session | [Value] | [Value] | [Value] |
| Avg. Session Duration | [Value] | [Value] | [Value] |
| Bounce Rate | [X%] | [X%] | [X%] |

### Traffic by Source
| Source | Sessions | % of Total | Conversions | Conv. Rate |
|---|---|---|---|---|
| Organic Search | [Value] | [X%] | [Value] | [X%] |
| Paid Search | [Value] | [X%] | [Value] | [X%] |
| Paid Social | [Value] | [X%] | [Value] | [X%] |
| Organic Social | [Value] | [X%] | [Value] | [X%] |
| Email | [Value] | [X%] | [Value] | [X%] |
| Direct | [Value] | [X%] | [Value] | [X%] |
| Referral | [Value] | [X%] | [Value] | [X%] |
| Other | [Value] | [X%] | [Value] | [X%] |
| **Total** | **[Value]** | **100%** | **[Value]** | **[X%]** |

### Conversion Funnel
| Stage | Volume | Rate | Period Change |
|---|---|---|---|
| Visitors | [Value] | -- | [+/-X%] |
| Leads | [Value] | [X%] | [+/-X%] |
| MQLs | [Value] | [X%] | [+/-X%] |
| SQLs | [Value] | [X%] | [+/-X%] |
| Customers | [Value] | [X%] | [+/-X%] |

**Data Sources:** [List all platforms, tools, and date ranges used to compile this report]
**Methodology Notes:** [Any changes in tracking, attribution, or data collection to be aware of]
```

## Common Mistakes

- **Data dumps without insights**: A table of numbers is not a report. Every metric in the report must be accompanied by context (why it changed), significance (what it means for the business), and direction (what to do about it). If you cannot explain why a number moved, investigate before publishing.
- **Hiding bad news**: Clients lose trust when they discover underperformance that was buried or omitted. Address every significant negative trend head-on with a root cause analysis and remediation plan. Agencies that own bad news and present solutions earn more trust than agencies that only report wins.
- **No forward-looking recommendations**: A backward-looking report without recommendations for next period is only half the job. Every report must close with specific, prioritized actions that connect this period's learnings to next period's plan. This is what separates strategic partners from vendors.
- **Inconsistent metrics period to period**: Switching KPIs, changing attribution models, or using different date ranges between reports makes trend analysis impossible and erodes client confidence. Lock in your metrics framework in month one and keep it consistent.
- **Writing for analysts instead of executives**: The primary audience is the client decision-maker who has 5 minutes. Lead with the executive summary, use plain language, and save granular data for the appendix. If the executive summary does not stand alone, the report fails.
- **Missing the "so what?"**: "Email open rate was 22%" is a fact. "Email open rate increased from 18% to 22% after we segmented the list by purchase history, suggesting personalization is driving engagement" is analysis. Every metric needs a "so what?" before it belongs in the report.
- **Reporting on vanity metrics**: Impressions, followers, and page views feel good but rarely connect to business outcomes. Always tie channel metrics back to conversion and revenue impact. If a metric does not connect to a business objective, question whether it belongs in the report.
- **Not comparing to targets**: Reporting actuals without targets leaves the client unable to evaluate performance. Every KPI must show actual vs. target vs. prior period. This three-way comparison tells the full story: are we improving, and are we where we need to be?

## Related Skills

- **juma-client-context**: Provides KPI targets, baselines, business goals, and channel strategy that contextualize every data point in the report
- **juma-sow**: Defines the deliverables and success criteria that the report measures against
- **juma-client-qbr**: Quarterly business reviews aggregate monthly reports and add strategic analysis -- this report is the building block
- **juma-channel-audit**: Channel audit findings inform the benchmarks and expectations used in reporting
- **juma-campaign-plan**: Campaign plans define the goals and tactics that this report evaluates
- **juma-paid-media-plan**: Paid media plans set the budget and performance targets tracked in the paid channel sections
- **juma-upsell-finder**: Outperforming channels and successful campaigns often reveal upsell opportunities to highlight in the report
