---
name: juma-retainer-review
description: "Use when conducting an internal profitability analysis for a retainer client, preparing for contract renewals, or assessing whether an account is healthy, at risk, or underpriced. INTERNAL ONLY -- not client-facing."
---

# Retainer Review (Internal)

**INTERNAL USE ONLY -- This document and its output are not shared with the client.**

Performs a comprehensive profitability and health assessment for a retainer client engagement. Analyzes hours utilization, deliverable completion, scope creep, client satisfaction signals, team allocation, and financial performance against agency benchmarks. Produces a clear recommendation for the next contract action: renew as-is, renegotiate scope, raise rates, add services, or prepare for potential churn.

## When to Use

- 60-90 days before a retainer contract renewal date
- Leadership requests a profitability review across the client portfolio
- Account team suspects scope creep but needs data to quantify it
- A team member reports feeling overworked on a specific account
- Client satisfaction appears to be declining (slower responses, missed meetings, negative tone)
- After a significant change in the client's business (new leadership, budget cuts, acquisition)
- Quarterly internal account health check cadence
- When considering whether to accept a client's request for reduced retainer

## Prerequisites

- **juma-client-context** (required) -- client profile, current SOW, contracted services, and engagement history
- Access to time tracking platform data (Harvest, Toggl, Clockify, or equivalent) for the review period
- Current statement of work (SOW) with contracted deliverables, hours, and rates
- Financial records: contracted retainer amount, actual costs (labor, tools, media pass-through)
- Agency benchmark data: target margins, target effective hourly rates, utilization targets
- Meeting records: scheduled vs attended meetings, client response times
- Deliverable tracking: project management platform data (Asana, Monday, ClickUp, etc.)

## Process

1. **Pull time tracking data**
   - Export hours logged against this client for the review period (minimum last 3 months, ideally 6-12 months)
   - Break down hours by team member, by role (strategist, specialist, designer, developer, account manager, etc.)
   - Break down hours by service area (SEO, paid media, content, social, reporting, meetings, etc.)
   - Break down hours by month to identify trends (is time spent increasing, decreasing, or stable?)
   - Calculate total hours worked vs total hours contracted for each period
   - Flag any team members logging significantly more hours than expected on this account

2. **Compare to SOW deliverables**
   - List every deliverable in the current SOW with its cadence (weekly, monthly, quarterly)
   - For each deliverable, determine: was it completed on time, late, or not at all?
   - Calculate the overall deliverable completion rate (completed on time / total due)
   - Identify any deliverables that are consistently late and the reasons why
   - Note any deliverables the client has stopped requesting or no longer values
   - Identify any recurring deliverables that take significantly more or less time than originally scoped

3. **Calculate profitability**
   - **Effective hourly rate:** Total retainer revenue / total hours worked (all team members)
   - **Gross margin:** (Retainer revenue - total labor cost) / retainer revenue
   - **Comparison to agency benchmarks:** Is the effective hourly rate above or below the agency target? Is the margin healthy?
   - **Trend analysis:** Is profitability improving or declining over time? What is driving the trend?
   - **Fully loaded cost:** Include allocated overhead (tools, platform costs, management time) if agency tracks this
   - **Revenue per team member hour:** Break down by role to identify where margin is being lost

4. **Assess client satisfaction signals**
   - **Response times:** How quickly does the client respond to emails, approve deliverables, provide feedback? Has this changed?
   - **Meeting attendance:** Does the client attend scheduled meetings consistently? Who attends (decision maker or delegate)?
   - **Feedback tone:** Review recent client communications for sentiment (enthusiastic, neutral, critical, disengaged)
   - **Referrals:** Has the client referred other businesses to the agency? (Strong positive signal)
   - **Ad hoc requests:** Is the client actively requesting work beyond the SOW? (Indicates engagement and trust, but also scope creep risk)
   - **Escalations:** Have there been any complaints, escalations to leadership, or expressed dissatisfaction?
   - **NPS or satisfaction survey data:** If the agency collects this, include the most recent score

5. **Identify scope creep**
   - Compare work actually performed (from time tracking and project management data) against the SOW deliverables list
   - Categorize out-of-scope work:
     - **Recurring scope creep:** Work done regularly that is not in the SOW (e.g., weekly report that was supposed to be monthly, managing a social channel that is not in scope)
     - **Ad hoc scope creep:** One-off requests that accumulate (e.g., "quick favor" design requests, unplanned strategy calls, additional platform management)
     - **Complexity creep:** In-scope deliverables that have grown more complex than originally scoped (e.g., monthly report that now takes 6 hours instead of the scoped 2 hours due to added sections)
   - Estimate hours spent on out-of-scope work per month
   - Calculate the dollar value of scope creep (hours x blended hourly rate)
   - Document specific examples with dates for use in renegotiation conversations

6. **Evaluate team utilization**
   - For each team member assigned to this account, calculate what percentage of their total capacity this account consumes
   - Flag team members who are overallocated (this account takes more than the planned percentage of their time)
   - Assess whether the right seniority level is doing the work (is a senior strategist doing work a coordinator could handle?)
   - Identify any single points of failure (one person holds all the client knowledge or relationships)
   - Note team satisfaction and retention risk on this account

7. **Build recommendation**
   - Synthesize all findings into one of the following primary recommendations:
     - **Renew as-is:** Account is healthy, profitable, and client is satisfied. No changes needed.
     - **Renegotiate scope:** Scope creep or changed client needs require a SOW revision. Define what should be added, removed, or repriced.
     - **Raise rates:** Account is profitable but below benchmark, or scope has expanded without rate adjustment. Calculate the rate increase needed to hit target margin.
     - **Add services:** Client would benefit from and is likely receptive to additional services. Pair with juma-upsell-finder output.
     - **Reduce scope:** The agency is over-delivering and the client does not value all deliverables. Propose a streamlined scope at the same or reduced rate.
     - **Churn risk -- retain:** Client shows churn signals. Recommend proactive retention actions (executive check-in, added value, strategic reset meeting).
     - **Churn risk -- manage exit:** Client is unlikely to renew or the account is unprofitable enough to let go. Plan a graceful transition.

8. **Prepare negotiation points**
   - For renegotiation scenarios, prepare:
     - Data-backed justification for changes (hours analysis, scope creep evidence, benchmark comparisons)
     - Proposed new terms (revised scope, updated rates, adjusted deliverables)
     - Value reinforcement talking points (results achieved, ROI delivered, problems solved)
     - Concessions to offer if needed (phased rate increase, added deliverable to sweeten the deal)
     - Walk-away terms (minimum acceptable terms for the agency)

## Output Format

```markdown
# Retainer Review: [Client Name]
# INTERNAL -- NOT FOR CLIENT DISTRIBUTION

**Review Period:** [Start Date] - [End Date]
**Prepared by:** [Name]
**Date:** [Date]
**Contract Renewal Date:** [Date]
**Current Monthly Retainer:** $[Amount]

---

## Account Health Scorecard

| Dimension | Score (1-5) | Trend | Notes |
|-----------|-------------|-------|-------|
| Profitability | [X] | [Up/Down/Stable] | [One-line summary] |
| Deliverable Completion | [X] | [Up/Down/Stable] | [One-line summary] |
| Client Satisfaction | [X] | [Up/Down/Stable] | [One-line summary] |
| Scope Discipline | [X] | [Up/Down/Stable] | [One-line summary] |
| Team Health | [X] | [Up/Down/Stable] | [One-line summary] |
| **Overall** | **[X]** | **[Trend]** | **[Summary assessment]** |

**Overall Status:** [Healthy / Needs Attention / At Risk / Critical]

---

## Hours Analysis

### Contracted vs Actual

| Month | Contracted Hours | Actual Hours | Variance | Utilization % |
|-------|-----------------|--------------|----------|---------------|
| [Month] | [X] | [X] | [+/- X] | [X%] |
| [Month] | [X] | [X] | [+/- X] | [X%] |
| [Month] | [X] | [X] | [+/- X] | [X%] |
| **Average** | **[X]** | **[X]** | **[+/- X]** | **[X%]** |

### Hours by Team Member

| Team Member | Role | Monthly Avg Hours | % of Account | Expected % | Flag |
|-------------|------|-------------------|-------------|------------|------|
| [Name] | [Role] | [X] | [X%] | [X%] | [Over/Under/OK] |
| [Name] | [Role] | [X] | [X%] | [X%] | [Over/Under/OK] |

### Hours by Service Area

| Service Area | Monthly Avg Hours | % of Total | SOW Allocation % | Variance |
|-------------|-------------------|------------|-------------------|----------|
| [Service] | [X] | [X%] | [X%] | [+/- X%] |
| [Service] | [X] | [X%] | [X%] | [+/- X%] |
| Meetings & Communication | [X] | [X%] | [X%] | [+/- X%] |

---

## Deliverable Completion

| Deliverable | Cadence | Completed On Time | Late | Missed | Completion Rate |
|-------------|---------|-------------------|------|--------|-----------------|
| [Deliverable] | [Weekly/Monthly/etc.] | [X] | [X] | [X] | [X%] |
| [Deliverable] | [Weekly/Monthly/etc.] | [X] | [X] | [X] | [X%] |
| **Overall** | | | | | **[X%]** |

**Deliverables the client no longer values or requests:**
- [Deliverable] -- [Last requested date, notes]

---

## Scope Creep Identification

**Total estimated hours on out-of-scope work per month:** [X] hours
**Dollar value of monthly scope creep:** $[Amount]

### Recurring Scope Creep
| Activity | Not in SOW | Est. Hours/Month | Duration | Total Uncompensated Hours |
|----------|-----------|-------------------|----------|--------------------------|
| [Activity] | [Correct] | [X] | [X months] | [X] |
| [Activity] | [Correct] | [X] | [X months] | [X] |

### Ad Hoc Scope Creep (Examples)
- [Date]: [Description of request, estimated hours spent]
- [Date]: [Description of request, estimated hours spent]
- [Date]: [Description of request, estimated hours spent]

### Complexity Creep
| Deliverable | Originally Scoped Hours | Current Avg Hours | Reason for Increase |
|-------------|------------------------|-------------------|---------------------|
| [Deliverable] | [X] | [X] | [Explanation] |

---

## Profitability Analysis

| Metric | This Account | Agency Benchmark | Status |
|--------|-------------|------------------|--------|
| Monthly retainer revenue | $[Amount] | -- | -- |
| Total monthly labor cost | $[Amount] | -- | -- |
| Gross margin | [X%] | [X%] | [Above/Below] |
| Effective hourly rate | $[Amount] | $[Amount] | [Above/Below] |
| Revenue per strategist hour | $[Amount] | $[Amount] | [Above/Below] |
| Revenue per specialist hour | $[Amount] | $[Amount] | [Above/Below] |

**Profitability trend (last 6 months):** [Improving / Declining / Stable]
**Primary margin driver:** [What is most affecting margin positively or negatively]

---

## Client Satisfaction Signals

| Signal | Assessment | Evidence |
|--------|-----------|----------|
| Response times | [Fast/Normal/Slow/Declining] | [Avg response time, trend] |
| Meeting attendance | [Consistent/Sporadic/Declining] | [Attendance rate, who attends] |
| Feedback tone | [Positive/Neutral/Critical/Disengaged] | [Recent examples] |
| Referrals given | [Yes/No] | [Details if yes] |
| Ad hoc requests | [Frequent/Occasional/Rare] | [Volume and nature] |
| Escalations | [None/Minor/Major] | [Details if any] |
| NPS / Survey score | [Score or N/A] | [Date of last survey] |

**Overall satisfaction assessment:** [Highly Satisfied / Satisfied / Neutral / At Risk / Dissatisfied]

---

## Risk Assessment

| Risk Factor | Level (1-5) | Evidence | Mitigation |
|-------------|-------------|----------|------------|
| Churn risk | [X] | [Signals observed] | [Recommended action] |
| Budget pressure | [X] | [Signals observed] | [Recommended action] |
| Competitor pitch | [X] | [Signals observed] | [Recommended action] |
| Key contact departure | [X] | [Signals observed] | [Recommended action] |
| Agency team burnout | [X] | [Signals observed] | [Recommended action] |

---

## Recommendation

**Primary recommendation:** [Renew As-Is / Renegotiate Scope / Raise Rates / Add Services / Reduce Scope / Retain (Churn Risk) / Manage Exit]

### Rationale
[2-3 paragraphs explaining the recommendation with supporting data from the analysis above. Reference specific numbers -- effective hourly rate, scope creep dollar value, satisfaction signals, and profitability trend.]

### Proposed Changes (if applicable)

| Current State | Proposed Change | Financial Impact |
|---------------|----------------|------------------|
| [Current term/scope/rate] | [Proposed term/scope/rate] | [+/- $Amount/month] |
| [Current term/scope/rate] | [Proposed term/scope/rate] | [+/- $Amount/month] |

### Negotiation Points
1. **Lead with value:** [Specific results achieved for the client to reinforce before discussing changes]
2. **Data justification:** [Key data points that support the proposed changes]
3. **Concession if needed:** [What the agency can offer if the client pushes back]
4. **Walk-away terms:** [Minimum acceptable outcome for the agency]

### Action Items

| Action | Owner | Deadline |
|--------|-------|----------|
| [Action item] | [Name] | [Date] |
| [Action item] | [Name] | [Date] |
| [Action item] | [Name] | [Date] |
```

## Common Mistakes

- **Not flagging scope creep until renewal time**: Scope creep should be tracked continuously, not discovered during the review. By the time it is quantified at renewal, the agency has already absorbed months of unpaid work with no leverage to recover it.
- **Using gut feel instead of data**: "This account feels unprofitable" is not actionable. Pull the actual hours, calculate the actual effective hourly rate, and compare to benchmarks. Data drives better decisions and stronger negotiation positions.
- **Treating all hours as equal**: An hour of a senior strategist's time costs the agency significantly more than an hour of a coordinator's time. Break down profitability by role, not just total hours.
- **Ignoring satisfaction signals**: An account can be profitable but at high churn risk if the client is dissatisfied. Profitability analysis without satisfaction assessment gives an incomplete picture.
- **Recommending rate increases without value reinforcement**: Never present a rate increase in isolation. Always pair it with a summary of results delivered and value created. The client needs to see the return before hearing about the cost change.
- **Sharing internal review data with the client**: This document contains margin data, team frustrations, and strategic calculations that are for internal use only. The negotiation points and proposed changes can inform client conversations, but the raw analysis stays internal.
- **Not preparing walk-away terms**: Enter every renegotiation knowing the minimum acceptable outcome. Without this, the agency risks agreeing to terms that perpetuate an unprofitable engagement.
- **Skipping the team health assessment**: Burnt-out team members produce worse work and eventually leave. If an account is consuming a disproportionate share of someone's capacity, that is a cost even if it does not show up in the financial analysis.

## Related Skills

- **juma-client-context** -- required for SOW details, client profile, and engagement history
- **juma-upsell-finder** -- use alongside the retainer review to pair expansion opportunities with renewal conversations
- **juma-case-study** -- high-performing retainer accounts are prime candidates for case studies, which also reinforce value during renewals
- **juma-client-qbr** -- retainer review data feeds into the internal prep for quarterly business reviews
- **juma-sow** -- if renegotiation results in new terms, generate an updated statement of work
- **juma-onboarding-checklist** -- if the review results in added services, the onboarding checklist covers access provisioning for new channels
