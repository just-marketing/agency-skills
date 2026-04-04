---
name: juma-campaign-plan
description: "Use when planning a multi-channel marketing campaign, when a client has a product launch or promotion, or when translating a brief into an executable campaign. Produces a comprehensive campaign plan with creative briefs, budget allocation, timeline, and measurement framework."
---

# Campaign Plan

## Overview

Transforms a client brief or business objective into a detailed, executable multi-channel campaign plan. Covers everything from audience targeting and channel selection to creative briefs, budget allocation, timeline, and measurement — giving the client a complete blueprint and the agency team clear marching orders.

## When to Use

- Client has a product launch, promotion, or seasonal campaign
- A `juma-client-brief` has been completed and needs to be operationalized
- Quarterly planning requires campaign-level detail
- Client wants to understand how budget will be spent across channels
- New campaign needs coordination across multiple teams/channels

## Prerequisites

- **juma-client-context** — brand, audience, goals, budget
- **juma-client-brief** (recommended) — structured campaign objectives
- **juma-channel-audit** (recommended) — informs channel selection
- **juma-competitor-intel** (recommended) — competitive positioning for messaging

## Process

### Step 1: Define Campaign Objective

Clarify the single primary objective using the marketing funnel:

1. **Awareness**: Brand recognition, reach, impressions
2. **Consideration**: Engagement, traffic, content consumption
3. **Conversion**: Leads, signups, purchases, demos

Define SMART goal: "Generate [X] qualified leads at $[Y] CPL within [Z] weeks"

### Step 2: Audience Definition

From client context, define campaign-specific audience:

1. **Primary audience**: Demographics, psychographics, behaviors, pain points
2. **Secondary audience**: If applicable
3. **Audience size estimates**: Per platform (use platform tools)
4. **Exclusions**: Who NOT to target (existing customers, competitors, etc.)
5. **Persona alignment**: Map to client context personas

### Step 3: Channel Selection

Select channels with clear rationale:

For each channel considered, document:
- **Why this channel**: Audience presence, objective alignment, competitive landscape
- **Role in the campaign**: Awareness driver, engagement builder, conversion closer
- **Expected contribution**: % of total results
- **Budget share**: % of total budget with justification

Typical channel mix by objective:
- **Awareness**: Paid social (Meta, TikTok), programmatic display, YouTube, influencer
- **Consideration**: Content marketing, SEO, email nurture, paid social retargeting
- **Conversion**: Paid search, email, retargeting, landing pages

### Step 4: Messaging Framework

Develop core campaign messaging:

1. **Campaign theme/big idea**: Unifying creative concept
2. **Key message**: One sentence that captures the campaign value proposition
3. **Supporting messages**: 3-5 proof points or benefit statements
4. **Tone**: How the message should feel (aligned with brand voice)
5. **Call-to-action**: Primary CTA per funnel stage

### Step 5: Creative Briefs by Channel

For each selected channel, create a mini-brief covering objective, audience, message, format, CTA, landing page, assets needed, and specs.

See [creative-brief-template.md](creative-brief-template.md) for the complete per-channel brief template, channel-specific considerations (Paid Social, Paid Search, Email, Content, Organic Social), and the brief checklist.

### Step 6: Budget Allocation

Allocate budget across channels and phases. Include a budget pacing schedule with daily/weekly/monthly spend targets.

See [budget-pacing-template.md](budget-pacing-template.md) for the complete budget allocation tables, phase-based pacing schedule, budget reallocation rules, and spend tracking template.

### Step 7: Campaign Timeline

Build timeline with dependencies:

1. **Planning phase**: Strategy, creative development, approvals
2. **Production phase**: Asset creation, landing page build, tracking setup
3. **Launch phase**: Staggered or simultaneous channel launches
4. **Optimization phase**: Performance review cadence, adjustment triggers
5. **Wrap-up phase**: Reporting, case study, learnings documentation

Include key milestones: creative approval, asset delivery, campaign go-live, mid-campaign review, final report.

### Step 8: Measurement Plan

Define how success will be measured:

1. **Primary KPI**: The one metric that defines success
2. **Secondary KPIs**: Supporting metrics per channel
3. **Attribution model**: Last-click, multi-touch, or custom
4. **Reporting cadence**: Daily/weekly/monthly during campaign
5. **Benchmarks**: What "good" looks like for each metric
6. **Tracking setup**: UTMs, pixels, conversion events needed

### Step 9: Contingency Triggers

Define what-if scenarios:

1. **Underperformance trigger**: If [metric] is below [threshold] by [date], then [action]
2. **Overperformance trigger**: If [metric] exceeds [threshold], then [scale action]
3. **External factors**: Competitor response, market shift, PR crisis protocols
4. **Budget reallocation rules**: When and how to shift budget between channels

### Step 10: A/B Testing Opportunities

Identify testable elements within the campaign:

1. **Creative tests**: Headlines, images, video vs static
2. **Audience tests**: Segment A vs B targeting
3. **Channel tests**: Platform A vs B for same objective
4. **Landing page tests**: Layout, CTA, form variations
5. **Timing tests**: Day-of-week, time-of-day optimization

## Output Format

```markdown
# Campaign Plan: [Campaign Name]
**Client**: [Client Name] | **Prepared by**: [Agency Name] | **Date**: [Date]

## Campaign Overview
- **Objective**: [SMART goal]
- **Duration**: [Start date] – [End date]
- **Total budget**: $[X] (media: $[Y] / agency: $[Z])
- **Primary KPI**: [Metric and target]

## Target Audience
### Primary Audience
- Demographics: [Details]
- Psychographics: [Details]
- Pain points: [Details]
- Platform behaviors: [Details]

### Audience Sizing
| Platform | Estimated Reach | Audience Size |
|----------|----------------|---------------|
| [Platform] | [N] | [N] |

## Messaging Framework
- **Big idea**: [Campaign concept]
- **Key message**: [One sentence]
- **Supporting messages**: [3-5 bullets]
- **CTA**: [Primary call-to-action]

## Channel Strategy

| Channel | Role | Budget | KPI Target | Content Type |
|---------|------|--------|------------|--------------|
| [Channel] | [Role] | $[X] ([%]) | [Metric: Target] | [Format] |

### Per-Channel Creative Briefs
See [creative-brief-template.md](creative-brief-template.md) for the per-channel brief format. Repeat for each channel.

## Budget Allocation

See [budget-pacing-template.md](budget-pacing-template.md) for the complete budget allocation, phase-based pacing, and tracking tables.

## Campaign Timeline

| Week | Phase | Activities | Deliverables | Owner |
|------|-------|-----------|--------------|-------|
| W1 | Planning | [Activities] | [Deliverables] | [Team] |
| W2 | Production | [Activities] | [Deliverables] | [Team] |
| W3 | Launch | [Activities] | [Deliverables] | [Team] |

## Measurement Plan
- **Primary KPI**: [Metric] — Target: [Value]
- **Secondary KPIs**: [List with targets]
- **Attribution**: [Model]
- **Reporting**: [Cadence]

## Contingency Plan

| Trigger | Condition | Action |
|---------|-----------|--------|
| Underperformance | [Metric] < [Threshold] by [Date] | [Action] |
| Overperformance | [Metric] > [Threshold] | [Scale action] |

## A/B Testing Plan
| Test | Hypothesis | Metric | Duration |
|------|-----------|--------|----------|
| [Test name] | If [change], then [result] | [Metric] | [Duration] |

## Approvals & Next Steps
- [ ] Client approval on strategy: [Date]
- [ ] Creative assets delivered: [Date]
- [ ] Tracking setup confirmed: [Date]
- [ ] Campaign go-live: [Date]
```

## Common Mistakes

- **No single clear objective** — Campaigns that try to drive awareness AND conversions simultaneously usually do neither well. Pick one primary objective
- **Equal budget distribution** — Don't split budget evenly across channels. Allocate based on expected performance and audience presence
- **Missing contingency plan** — Every campaign needs clear triggers for adjustment. "We'll optimize as we go" isn't a plan
- **Creative brief without specs** — Channel-specific specs prevent production delays. Include dimensions, character limits, and file formats
- **No testing plan** — Every campaign is a learning opportunity. Build in A/B tests from the start
- **Timeline without dependencies** — Show what blocks what. Creative approval must happen before production begins

## Related Skills

- **juma-client-brief** — Provides the structured objectives this plan operationalizes
- **juma-content-calendar** — Content pieces created for this campaign feed into the editorial calendar
- **juma-paid-media-plan** — Detailed paid channel execution within this campaign
- **juma-ab-test-plan** — Detailed test design for campaign experiments
- **juma-analytics-setup** — Tracking configuration needed for campaign measurement
- **juma-reporting** — Campaign performance feeds into client reporting
