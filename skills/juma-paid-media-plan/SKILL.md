---
name: juma-paid-media-plan
description: "Use when planning paid advertising across Google Ads, Meta, LinkedIn, TikTok, or programmatic platforms. Use when a client needs a media buying strategy, budget allocation, or audience targeting plan. Produces a detailed paid media plan with campaign structure, budget pacing, and measurement framework."
---

# Paid Media Plan

## Overview

Creates a comprehensive paid media strategy covering platform selection, audience targeting, campaign architecture, budget allocation with pacing, creative requirements, bidding strategy, and measurement. This is the tactical execution plan that turns a campaign plan's paid media budget into structured, optimizable campaigns across platforms.

## When to Use

- Client is launching or scaling paid advertising
- Budget has been allocated to paid channels in a campaign plan
- Existing paid campaigns need restructuring or optimization
- Client asks "where should we spend our ad budget?"
- Onboarding a client with existing ad accounts that need an audit and restructure

## Prerequisites

- **juma-client-context** — business model, target audience, budget, goals
- **juma-campaign-plan** (recommended) — overall campaign strategy and budget allocation
- **juma-analytics-setup** (recommended) — conversion tracking must be in place
- **juma-competitor-intel** (recommended) — competitive ad landscape

## Process

### Step 1: Define Paid Media Objectives

Map business goals to paid media objectives:

1. **Awareness**: Reach, impressions, video views, brand lift
2. **Consideration**: Traffic, engagement, video views (intent-based)
3. **Conversion**: Leads, purchases, signups, app installs
4. **Retention**: Retargeting, cross-sell, upsell campaigns

Define target metrics: CPA, ROAS, CPL, CPC, CPM targets based on client's unit economics.

### Step 2: Platform Selection

Evaluate and select platforms with rationale:

See [platform-selection-guide.md](platform-selection-guide.md) for the complete platform comparison matrix, objective alignment table, and minimum budget guidance.

For each selected platform, document why it was chosen and its role in the media mix.

### Step 3: Audience Strategy

Build audience layers per platform:

1. **Core audiences**: Demographic + interest + behavior targeting
2. **Custom audiences**: Website visitors, email lists, CRM data, app users
3. **Lookalike/similar audiences**: Based on best customers, converters, high-value segments
4. **Retargeting audiences**: Site visitors (by page/action), cart abandoners, video viewers, engagers
5. **Exclusions**: Existing customers (if acquisition-focused), converters, competitors' employees

Document audience sizing per platform and expected overlap.

### Step 4: Campaign Architecture

Structure campaigns using platform best practices. See [campaign-architecture-template.md](campaign-architecture-template.md) for the complete campaign hierarchy, naming conventions, and architecture examples by funnel stage.

For each platform, define the number of campaigns, ad sets/groups, ads per ad set, and ad rotation strategy.

### Step 5: Budget Allocation & Pacing

Allocate budget across platforms, campaigns, and time:

1. **Platform split**: Based on audience presence and expected performance
2. **Campaign split**: By funnel stage (typically 20% awareness / 50% consideration / 30% conversion)
3. **Pacing strategy**:
   - **Daily budgets**: Steady-state spend level
   - **Weekly adjustments**: Performance-based reallocation
   - **Monthly cadence**: Ramp-up → sustain → optimization
   - **Flighting**: Heavy-up periods around key dates/events
4. **Minimum viable budget**: Per platform (below which performance data is unreliable)

### Step 6: Creative Requirements

Define creative needs per platform and format:

For each ad format:
- **Format**: Single image, carousel, video, responsive, text
- **Specs**: Dimensions, file size, character limits, aspect ratios
- **Quantity**: Number of variations needed
- **Key elements**: Headline, body copy, CTA, landing page URL
- **Creative guidelines**: On-brand elements, required disclaimers, do/don't

Include creative refresh schedule (new creative every 2-4 weeks to combat fatigue).

### Step 7: Bidding Strategy

Define bidding approach per platform. See [bidding-strategy-guide.md](bidding-strategy-guide.md) for the complete bidding strategy selection matrix, platform-specific recommendations, and campaign maturity progression.

Document bid caps, floors, and adjustment schedules.

### Step 8: Measurement & Attribution

Define how paid media performance will be tracked:

1. **Conversion tracking**: Platform pixels, server-side tracking, offline conversion imports
2. **Attribution model**: Last-click, data-driven, multi-touch (specify per platform)
3. **View-through window**: 1-day, 7-day, 28-day (align across platforms for fair comparison)
4. **Click-through window**: 7-day, 28-day
5. **Cross-platform deduplication**: How to avoid double-counting conversions
6. **Reporting metrics**: Primary (CPA, ROAS) + secondary (CTR, quality score, impression share)

### Step 9: Optimization Cadence

Define ongoing optimization schedule:

- **Daily**: Budget pacing, anomaly detection, ad disapprovals
- **Weekly**: Performance review, bid adjustments, audience refinement, budget reallocation
- **Biweekly**: Creative performance review, new creative deployment
- **Monthly**: Strategy review, test results, platform mix adjustment
- **Quarterly**: Full strategy reassessment, competitive review

### Step 10: Reporting Framework

Define client-facing reporting:

1. **Dashboard access**: Real-time or scheduled
2. **Report frequency**: Weekly summary, monthly deep-dive
3. **Key metrics**: Agreed-upon KPIs with targets
4. **Format**: Executive summary + channel detail + recommendations

## Output Format

```markdown
# Paid Media Plan: [Client Name]
**Prepared by**: [Agency Name] | **Date**: [Date]
**Budget**: $[X]/month | **Duration**: [Start] – [End]

## Objectives & Targets

| Metric | Target | Current Baseline |
|--------|--------|-----------------|
| Monthly spend | $[X] | $[X] |
| CPA / CPL | $[X] | $[X] |
| ROAS | [X]:1 | [X]:1 |
| Conversions/month | [N] | [N] |

## Platform Strategy

| Platform | Role | Monthly Budget | % of Total | Primary KPI |
|----------|------|---------------|------------|-------------|
| [Platform] | [Role] | $[X] | [Y%] | [KPI: Target] |

## Audience Strategy

### [Platform 1]
| Audience | Type | Est. Size | Campaign | Priority |
|----------|------|-----------|----------|----------|
| [Audience name] | Core/Custom/Lookalike/Retargeting | [N] | [Campaign] | [H/M/L] |

## Campaign Architecture

### [Platform 1]
```
Campaign: [Name] (Objective: [X], Budget: $[X]/day)
├── Ad Set: [Name] (Audience: [X], Placement: [X])
│   ├── Ad 1: [Description]
│   ├── Ad 2: [Description]
│   └── Ad 3: [Description]
└── Ad Set: [Name]
    └── ...
```

## Budget Pacing

| Month | [Platform 1] | [Platform 2] | [Platform 3] | Total |
|-------|-------------|-------------|-------------|-------|
| Month 1 | $[X] | $[X] | $[X] | $[X] |
| Month 2 | $[X] | $[X] | $[X] | $[X] |
| Month 3 | $[X] | $[X] | $[X] | $[X] |

## Creative Requirements

| Platform | Format | Specs | Quantity | Refresh Cadence |
|----------|--------|-------|----------|-----------------|
| [Platform] | [Format] | [Dimensions, limits] | [N variations] | Every [N] weeks |

## Bidding Strategy

| Platform | Campaign Type | Bid Strategy | Target | Cap |
|----------|--------------|-------------|--------|-----|
| [Platform] | [Type] | [Strategy] | $[X] | $[X] |

## Measurement Setup

| Item | Status | Details |
|------|--------|---------|
| [Platform] pixel | [Installed/Needed] | [Notes] |
| Conversion events | [Configured/Needed] | [List events] |
| UTM parameters | [Standardized/Needed] | [Convention] |
| Attribution model | [Model] | [Window settings] |

## Optimization Schedule

| Cadence | Activities | Owner |
|---------|-----------|-------|
| Daily | Budget pacing, ad disapprovals | [Team] |
| Weekly | Bid adjustments, audience refinement | [Team] |
| Biweekly | Creative refresh, A/B test review | [Team] |
| Monthly | Strategy review, client report | [Team] |

## Risks & Mitigations

| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| [Risk] | [H/M/L] | [H/M/L] | [Action] |
```

## Common Mistakes

- **No minimum budget thresholds** — Each platform needs enough spend to generate statistically significant data. Don't spread $5K across 5 platforms
- **Over-segmenting audiences** — Too many ad sets with tiny audiences leads to poor optimization. Consolidate where possible
- **Ignoring creative fatigue** — Same ads running for months lose effectiveness. Plan creative refresh cycles from the start
- **Mismatched attribution windows** — Different windows across platforms make comparison impossible. Standardize where you can
- **No negative keywords/exclusions** — Wasted spend on irrelevant searches or audiences. Build exclusion lists proactively
- **Set and forget** — Paid media requires active management. Define optimization cadence and stick to it
- **Vanity metrics focus** — Impressions and clicks don't pay bills. Tie everything back to conversions and revenue

## Related Skills

- **juma-campaign-plan** — High-level campaign strategy that this plan executes
- **juma-analytics-setup** — Conversion tracking and attribution setup
- **juma-ab-test-plan** — Detailed test design for ad creative and landing page tests
- **juma-reporting** — Paid media performance feeds into client reports
- **juma-channel-audit** — Identifies paid media opportunities and current performance
- **juma-content-calendar** — Organic content that supports paid campaigns
