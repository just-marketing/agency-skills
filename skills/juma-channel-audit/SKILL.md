---
name: juma-channel-audit
description: "Use when onboarding a new client, conducting a quarterly review, or evaluating marketing channel performance. Produces a channel-by-channel assessment with opportunity scores, effort/impact ratios, and a prioritized channel mix recommendation."
---

# Channel Audit

## Overview

Performs a comprehensive channel-by-channel marketing assessment that evaluates every active and potential marketing channel against industry benchmarks and historical performance. This is a foundational audit that agencies run during onboarding and revisit quarterly -- it drives budget allocation decisions, identifies underperforming channels, and surfaces untapped opportunities that can expand the engagement scope.

## When to Use

- New client onboarding to establish a performance baseline across all channels
- Quarterly or semi-annual strategy reviews to reassess channel priorities
- Client asks "where should we be spending our budget?"
- Before building a campaign plan or paid media plan
- When a client's overall performance has plateaued and you need to find new growth levers
- After a major market shift, algorithm change, or competitor move that may affect channel effectiveness

## Prerequisites

- **juma-client-context** (required) -- brand info, target audiences, goals, budget, and competitive landscape
- **juma-competitor-intel** (recommended) -- competitive channel presence informs benchmarking
- Access to client analytics platforms (GA4, ad platforms, email platform, social accounts)
- Historical performance data (minimum 3 months, ideally 12 months)

## Process

1. **Inventory active channels**
   - List every channel the client currently uses with monthly spend and resource allocation
   - Note channels the client has tried and abandoned, with reasons if known
   - Identify channels the client has never used but competitors leverage
   - Channels to evaluate: organic search, paid search, paid social, organic social, email marketing, content marketing, referral/partnerships, direct/brand

2. **Pull performance data for each active channel**
   - Traffic volume and trend (last 3, 6, 12 months)
   - Conversion rate and revenue/lead contribution
   - Cost per acquisition (CPA) or cost per lead (CPL)
   - Return on ad spend (ROAS) or ROI where applicable
   - Engagement metrics relevant to the channel (CTR, open rate, engagement rate, etc.)
   - Customer quality indicators (LTV of customers from each channel, retention rates)

3. **Benchmark against industry standards**
   - Compare each channel's metrics to published industry benchmarks for the client's vertical
   - Flag channels performing significantly above or below benchmarks (>20% variance)
   - Note where the client's historical trend is improving or declining
   - Account for seasonality and market conditions when interpreting benchmarks

4. **Score opportunities (1-10) for each channel**
   - Evaluate current performance headroom (gap between current and benchmark)
   - Assess audience presence (is the target audience reachable on this channel?)
   - Consider competitive intensity (how crowded is the channel in this vertical?)
   - Factor in the client's existing assets and capabilities
   - Weight scoring toward the client's stated business objectives

5. **Calculate effort/impact ratio for each channel**
   - Estimate implementation effort: budget required, team skills needed, time to launch, ongoing maintenance
   - Estimate potential impact: traffic potential, conversion potential, revenue potential, brand value
   - Categorize each channel into the effort/impact matrix quadrants (Quick Wins, Strategic Bets, Fill-Ins, Deprioritize)
   - See [effort-impact-matrix.md](effort-impact-matrix.md) for the complete matrix visualization, quadrant definitions, and estimation factors

6. **Build prioritized channel mix recommendation**
   - Recommend primary channels (top 2-3 receiving majority of budget/effort)
   - Recommend secondary channels (supporting roles, testing budget)
   - Recommend channels to pause or sunset with rationale
   - Propose a phased implementation timeline (30/60/90 days)
   - Tie channel recommendations back to the client's business objectives and budget constraints

## Output Format

```markdown
# Marketing Channel Audit: [Client Name]
**Prepared by:** [Agency Name]
**Date:** [Date]
**Period Analyzed:** [Date Range]

## Executive Summary

[2-3 paragraphs summarizing the overall channel health, key findings, and top-line recommendations. Lead with the most important insight.]

## Channel Assessment

Use the per-channel scorecard structure for each of the 8 channels. See [channel-scorecard-template.md](channel-scorecard-template.md) for the complete scorecard structure and opportunity scoring guide.

Channels to assess: Organic Search, Paid Search, Paid Social, Organic Social, Email Marketing, Content Marketing, Referral & Partnerships, Direct/Brand.

## Effort/Impact Matrix

See [effort-impact-matrix.md](effort-impact-matrix.md) for the complete matrix visualization and quadrant definitions.

## Recommended Channel Mix

| Channel | Role | Monthly Budget | % of Total | Priority |
|---------|------|---------------|------------|----------|
| [Channel] | Primary | $[X] | [X%] | P1 |
| [Channel] | Primary | $[X] | [X%] | P1 |
| [Channel] | Secondary | $[X] | [X%] | P2 |
| [Channel] | Testing | $[X] | [X%] | P3 |
| **Total** | | **$[X]** | **100%** | |

## Implementation Roadmap

### Days 1-30: Quick Wins
- [ ] [Action item with owner and expected impact]

### Days 31-60: Strategic Investments
- [ ] [Action item with owner and expected impact]

### Days 61-90: Optimization & Expansion
- [ ] [Action item with owner and expected impact]

## Appendix: Data Sources & Methodology
- [List all platforms and date ranges used]
- [Note any data gaps or limitations]
```

## Common Mistakes

- **Evaluating channels in isolation** -- channels interact (e.g., paid search captures demand that content marketing creates). Always consider the full funnel and channel interplay.
- **Ignoring the client's team capacity** -- recommending five new channels when the client has a two-person marketing team guarantees poor execution. Match recommendations to realistic resource constraints.
- **Benchmarking against wrong verticals** -- B2B SaaS benchmarks are meaningless for a local restaurant chain. Use industry-specific and business-model-specific benchmarks.
- **Recency bias in data** -- one bad month does not make a channel a failure. Look at 6-12 month trends and account for seasonality before making channel-level judgments.
- **Skipping inactive channels** -- the audit should evaluate channels the client is NOT using, not just active ones. Untapped channels are often the biggest opportunities.
- **Recommending channel changes without budget math** -- every recommendation must include estimated cost so the client can make informed trade-off decisions.

## Related Skills

- **juma-client-context** -- provides the brand, audience, and budget inputs this audit requires
- **juma-competitor-intel** -- competitive channel presence data feeds into benchmarking and gap analysis
- **juma-campaign-plan** -- use audit findings to inform channel selection for specific campaigns
- **juma-paid-media-plan** -- detailed planning for paid channels identified as priorities
- **juma-upsell-finder** -- underutilized channels often represent upsell opportunities
- **juma-client-qbr** -- channel audit findings feed into quarterly business review strategy sections
