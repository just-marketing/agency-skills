---
name: juma-client-brief
description: "Use when a client submits a vague request, kicks off a new project, or when any downstream skill needs a structured brief. Translates raw client input into a comprehensive, SMART-goal-driven project brief with defined scope, success metrics, timeline, and deliverables."
---

# Client Brief

## Overview

The Client Brief skill transforms unstructured client requests -- "we need more leads," "our social media isn't working," "we want to rebrand" -- into rigorous, actionable project briefs that the entire agency team can execute against. This is the critical translation layer between what a client says they want and what the agency actually delivers. A poorly scoped brief is the single most common cause of scope creep, misaligned expectations, and failed engagements.

This skill takes the rich context from juma-client-context and combines it with the client's immediate request to produce a brief that eliminates ambiguity before any work begins.

## When to Use

- A client sends a vague or open-ended request ("we need to do something about our SEO")
- Kicking off a new project, campaign, or initiative within an existing engagement
- A client asks for work that falls outside the current scope of work
- Translating a verbal conversation or meeting into a documented brief
- Before running any execution-level skill (campaign plan, content calendar, paid media plan, etc.)
- When multiple stakeholders have conflicting expectations and alignment is needed
- A retainer client requests a new deliverable or service not previously defined

## Prerequisites

- **juma-client-context** (required) -- the client profile must exist before building a brief. The brief pulls audience segments, goals, brand voice, budget parameters, and performance baselines directly from the context. If no client context exists, build one first.

## Process

### Step 1: Capture the Raw Client Request

Record the client's request exactly as stated, preserving their language and framing. Do not interpret, reframe, or correct at this stage. Capture:

- The exact words the client used to describe what they want
- The channel or medium the request came through (email, call, Slack, meeting)
- Who made the request and their role (decision-maker, day-to-day contact, executive sponsor)
- Any stated or implied urgency ("we need this by Q3," "ASAP," "when you get a chance")
- Any context the client provided about why they want this now

### Step 2: Ask Clarifying Questions to Fill Gaps

Compare the raw request against the brief template below. Identify every gap and prepare targeted questions. Group questions logically and ask them in a single, organized message -- do not drip-feed questions across multiple exchanges.

**Background & Context Questions:**
1. What prompted this request right now? (trigger event, competitive pressure, internal mandate, seasonal opportunity)
2. Has the client attempted this before? What happened?
3. Are there internal stakeholders beyond the requester who have input or veto power?
4. Is this tied to a larger initiative or standalone?

**Objective Questions:**
1. What does success look like in concrete terms? (not "more leads" but "how many more, by when, from where")
2. What is the primary objective vs. secondary nice-to-haves?
3. Is this about acquiring new customers, retaining existing ones, or reactivating lapsed ones?
4. What would make this project a failure even if all deliverables are completed on time?

**Audience Questions:**
1. Which audience segments from the client context are the priority for this initiative?
2. Are there segments to explicitly exclude?
3. Is there a geographic, demographic, or behavioral focus that narrows the audience further?
4. Where is the target audience in the buyer journey for this specific initiative?

**Scope & Constraints Questions:**
1. What channels or tactics are in scope? What is explicitly out of scope?
2. Are there brand guidelines, legal requirements, or compliance rules that apply?
3. What existing assets can be leveraged (creative, content, data, landing pages)?
4. Are there technical constraints (platform limitations, integration requirements, tracking gaps)?

**Budget & Timeline Questions:**
1. What is the budget for this specific initiative (separate from the overall retainer)?
2. Is the budget fixed or flexible based on projected results?
3. What is the hard deadline, and what is driving it?
4. Are there interim milestones or checkpoints required?

**Deliverable Questions:**
1. What format does the client expect the final output in?
2. Who needs to review and approve, and how many revision rounds are included?
3. Does the client need the strategy/plan only, or execution as well?
4. What does the handoff look like -- does the agency implement, or does the client's team?

### Step 3: Map to SMART Objectives

Take the client's stated goals and convert each into SMART format:

- **Specific**: What exactly will be achieved? Name the metric, audience, and channel.
- **Measurable**: What number defines success? Include the unit of measurement.
- **Achievable**: Is this realistic given the budget, timeline, and current baseline from juma-client-context? If not, flag it and propose an alternative.
- **Relevant**: Does this objective connect to the business goals defined in juma-client-context? Show the connection explicitly.
- **Time-bound**: By what date must this be achieved? Include interim milestones.

If the client's request does not translate into at least one SMART objective, the brief is not ready. Go back to Step 2.

### Step 4: Define Measurable Success Criteria

For each SMART objective, define:

1. The primary KPI and how it will be measured (tool, methodology, frequency)
2. The current baseline from juma-client-context performance data
3. The target value and the rationale for that target (benchmark, historical trend, client expectation)
4. Leading indicators that will show progress before the final KPI moves (e.g., impressions before clicks before conversions)
5. A measurement cadence (daily, weekly, monthly) and who receives the reporting
6. The definition of failure -- what result would cause the project to be paused or pivoted

### Step 5: Identify Constraints and Dependencies

Document everything that could block or limit execution:

- **Budget constraints**: Total budget, monthly caps, approval thresholds for overspend
- **Timeline constraints**: Hard deadlines, seasonal windows, dependent launches
- **Resource constraints**: Client team availability for reviews, asset creation bottlenecks, agency team capacity
- **Technical constraints**: Platform limitations, tracking gaps, integration requirements
- **Legal/compliance constraints**: Industry regulations, required disclaimers, approval workflows
- **Dependencies on other work**: Does this brief depend on another project completing first? Does anything else depend on this brief?
- **Assumptions**: State every assumption explicitly so it can be validated before work begins

### Step 6: Structure into the Brief Template

Compile all gathered, clarified, and validated information into the output format below. Every field must be completed. Use `[TO BE CONFIRMED]` for any remaining gaps and note the follow-up plan for each.

Cross-reference the juma-client-context profile to ensure consistency. If the brief contradicts the context (e.g., targeting an audience not in the profile, or setting a budget that exceeds the stated allocation), flag the discrepancy.

### Step 7: Present for Client Approval

Share the completed brief with the client and key stakeholders. Frame the review as:

1. "Here is what we heard" -- confirm the raw request was captured accurately
2. "Here is what we recommend" -- present the SMART objectives and scope
3. "Here is what is out of scope" -- set boundaries explicitly so there is no ambiguity
4. "Here is what we need from you" -- list any client-side dependencies, approvals, or assets
5. "Please confirm or correct" -- request written approval before any execution begins

Do not proceed to execution-level skills until the brief is approved in writing by the designated decision-maker identified in juma-client-context.

## Output Format

```markdown
# Project Brief: [Project Name]

**Client:** [Client Name]
**Prepared by:** [Agency Team Member]
**Date:** [Date]
**Brief Status:** [Draft / Pending Approval / Approved]
**Approved by:** [Name and Role, once approved]

---

## 1. Background & Context

### Raw Client Request
> [Exact quote or paraphrase of what the client asked for, preserved in their language]

**Requested by:** [Name and role]
**Request channel:** [Email / Call / Meeting / Slack / etc.]
**Date of request:** [Date]

### Situation Context
[2-3 paragraphs explaining the background. Why is this request happening now? What business conditions, competitive pressures, or internal mandates are driving it? Reference relevant information from juma-client-context -- market position, recent performance trends, competitive landscape shifts.]

### Prior Attempts
[Has this been tried before? What happened? What should be done differently this time? If no prior attempts, state "No prior initiatives addressing this objective."]

---

## 2. Objectives

### Primary Objective
**Goal:** [SMART objective statement]
- **Specific:** [What exactly will be achieved]
- **Measurable:** [The metric and target number]
- **Achievable:** [Why this is realistic given current baseline and resources]
- **Relevant:** [How this connects to business goals from juma-client-context]
- **Time-bound:** [Deadline with interim milestones]

### Secondary Objectives
1. [SMART objective 2]
2. [SMART objective 3, if applicable]

### Non-Goals
- [What this project is explicitly NOT trying to achieve]
- [Scope boundaries stated as non-goals to prevent creep]

---

## 3. Target Audience

### Primary Audience
**Segment:** [Segment name from juma-client-context]
- **Who:** [Demographics and firmographics]
- **Why them:** [Why this segment is the priority for this initiative]
- **Where to reach them:** [Channels and touchpoints relevant to this project]
- **Buyer journey stage:** [Awareness / Consideration / Decision / Retention]
- **Key message resonance:** [What this audience cares about most relative to this project]

### Secondary Audience
**Segment:** [Segment name from juma-client-context]
- **Who:** [Demographics and firmographics]
- **Why them:** [Why this segment is included as secondary]
- **Where to reach them:** [Channels and touchpoints]
- **Buyer journey stage:** [Stage]

### Excluded Audiences
- [Segments explicitly out of scope for this initiative and why]

---

## 4. Success Metrics

| Metric | Baseline | Target | Timeline | Measurement Tool | Reporting Cadence |
|--------|----------|--------|----------|-----------------|-------------------|
| **Primary KPI:** [Metric name] | [Current value from juma-client-context] | [Target value] | [By when] | [GA4 / CRM / Ad Platform / etc.] | [Weekly / Monthly] |
| **Leading Indicator 1:** [Metric] | [Current value] | [Target value] | [By when] | [Tool] | [Cadence] |
| **Leading Indicator 2:** [Metric] | [Current value] | [Target value] | [By when] | [Tool] | [Cadence] |
| **Secondary KPI:** [Metric] | [Current value] | [Target value] | [By when] | [Tool] | [Cadence] |

**Definition of Success:** [One sentence describing the minimum outcome that makes this project a success]

**Definition of Failure:** [One sentence describing the outcome that would cause the project to be paused or pivoted]

---

## 5. Scope

### In Scope
- [Specific deliverable or activity 1]
- [Specific deliverable or activity 2]
- [Specific deliverable or activity 3]
- [Specific deliverable or activity 4]

### Out of Scope
- [Explicitly excluded item 1] -- [Reason for exclusion]
- [Explicitly excluded item 2] -- [Reason for exclusion]
- [Explicitly excluded item 3] -- [Reason for exclusion]

### Assumptions
- [Assumption 1 -- e.g., "Client will provide product images by [date]"]
- [Assumption 2 -- e.g., "Existing landing page will be used without redesign"]
- [Assumption 3 -- e.g., "Budget does not include media spend, only management fees"]

---

## 6. Budget

| Line Item | Amount | Notes |
|-----------|--------|-------|
| **Total Project Budget** | $[Amount] | [Fixed / Flexible / Not-to-exceed] |
| Strategy & Planning | $[Amount] | [Included in retainer / Separate project fee] |
| Creative & Production | $[Amount] | [Rounds of revision included] |
| Media Spend | $[Amount] | [Platform breakdown if known] |
| Technology & Tools | $[Amount] | [Any new tools or licenses required] |
| Contingency | $[Amount] | [Typically 10-15% for unforeseen needs] |

**Budget Approval Process:** [Who approves, threshold for additional spend, turnaround time for approval]

**Budget Constraints:** [Any hard caps, spending restrictions, or allocation rules]

---

## 7. Timeline & Milestones

| Milestone | Date | Owner | Dependencies |
|-----------|------|-------|-------------|
| Brief approved | [Date] | [Client decision-maker] | None |
| [Phase 1 deliverable] | [Date] | [Agency team member] | Brief approval |
| Client review round 1 | [Date] | [Client reviewer] | Phase 1 complete |
| [Phase 2 deliverable] | [Date] | [Agency team member] | Client feedback |
| Client review round 2 | [Date] | [Client reviewer] | Phase 2 complete |
| Final deliverable | [Date] | [Agency team member] | All approvals |
| Launch / Go-live | [Date] | [Owner] | Final approval |
| Performance review | [Date] | [Agency team member] | 30 days post-launch |

**Hard Deadline:** [Date and what is driving it -- event, season, product launch, board meeting, etc.]

**Review Turnaround:** [Expected turnaround time for client reviews -- e.g., "2 business days per review round"]

---

## 8. Deliverables

| # | Deliverable | Format | Description | Due Date |
|---|------------|--------|-------------|----------|
| 1 | [Deliverable name] | [PDF / Deck / Dashboard / Live campaign / etc.] | [What it includes and level of detail] | [Date] |
| 2 | [Deliverable name] | [Format] | [Description] | [Date] |
| 3 | [Deliverable name] | [Format] | [Description] | [Date] |

**Revision Policy:** [Number of included revision rounds, process for additional revisions, cost of additional rounds]

**Handoff Process:** [Does the agency implement or hand off to the client's team? What does the transition look like?]

---

## 9. Approval & Governance

**Decision-Maker:** [Name, role -- the person whose sign-off is required to proceed]

**Stakeholders:**
| Name | Role | Involvement |
|------|------|-------------|
| [Name] | [Role] | [Approver / Reviewer / Informed] |
| [Name] | [Role] | [Approver / Reviewer / Informed] |
| [Name] | [Role] | [Approver / Reviewer / Informed] |

**Approval Process:**
1. Agency presents brief to [decision-maker]
2. Client has [X] business days to review and provide consolidated feedback
3. Agency incorporates feedback and returns revised brief within [X] business days
4. Client provides written approval (email confirmation is sufficient)
5. No execution begins until written approval is received

**Change Request Process:** [How are scope changes handled after brief approval? Who can request changes, what is the process, and how does it affect budget and timeline?]

---

## 10. Open Items & Risks

### Open Items
| # | Item | Owner | Due Date | Status |
|---|------|-------|----------|--------|
| 1 | [Unresolved question or pending information] | [Who is responsible] | [When needed] | [Open / In Progress] |
| 2 | [Unresolved question or pending information] | [Who is responsible] | [When needed] | [Open / In Progress] |

### Risks
| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| [Risk description] | [High / Medium / Low] | [High / Medium / Low] | [How to prevent or respond] |
| [Risk description] | [High / Medium / Low] | [High / Medium / Low] | [How to prevent or respond] |
```

## Common Mistakes

- **Accepting the client's framing without challenge** -- When a client says "we need more social media posts," they usually mean "we need more leads" or "we need more brand awareness." Always dig past the stated request to the underlying business objective. The brief should address the real problem, not just the client's self-prescribed solution.
- **Skipping the SMART conversion** -- Vague objectives like "improve SEO" or "grow our audience" are not briefable. If you cannot attach a specific number, timeline, and measurement method to an objective, the brief is incomplete and will lead to misaligned expectations at the review stage.
- **Not defining out-of-scope explicitly** -- Scope creep starts the moment the brief is approved. If a boundary is not written down, the client will assume it is included. List non-goals and out-of-scope items with the same specificity as in-scope items.
- **Ignoring the client context profile** -- The brief must pull audience segments, performance baselines, budget parameters, and brand voice from juma-client-context. If the brief introduces a new audience segment, contradicts the stated budget, or targets a metric not tracked in the marketing stack, those discrepancies must be flagged and resolved.
- **Setting unrealistic targets to please the client** -- If the client wants to triple leads in 30 days on the same budget, the brief must flag this as unachievable and propose an alternative. Agreeing to unrealistic targets poisons the engagement from day one.
- **Missing the approval process** -- Every brief must name the decision-maker and define the approval workflow. Starting work on an "approved" brief that was only approved by the day-to-day contact, not the budget holder, is a recipe for rework and writeoffs.
- **Treating the brief as a formality** -- The brief is a contract between the agency and the client. It defines what will be delivered, what success looks like, and what is out of bounds. Rushing through it or treating it as a checkbox guarantees problems downstream.
- **Forgetting to include leading indicators** -- If the primary KPI is revenue, you need leading indicators (traffic, leads, conversion rate) that confirm progress before the final number moves. Without these, the first meaningful check-in happens too late to course-correct.
- **No change request process** -- Clients will request changes. If there is no documented process for handling scope changes, budget adjustments, and timeline shifts, every change becomes an uncomfortable ad hoc negotiation.

## Related Skills

- **juma-client-context** -- required input; provides the audience, goals, budget, and performance data that the brief builds upon
- **juma-campaign-plan** -- the natural next step after brief approval; translates the brief into a detailed campaign execution plan
- **juma-proposal** -- for new business, the brief may be generated alongside or shortly after the proposal is accepted
- **juma-content-calendar** -- execution-level skill that consumes the brief's audience, timeline, and channel scope
- **juma-sow** -- the brief often serves as the basis for a formal statement of work, especially for project-based engagements
- **juma-reporting** -- uses the success metrics and KPIs defined in the brief as the reporting framework
- **juma-paid-media-plan** -- pulls budget, audience, and objective data from the brief for media planning
- **juma-channel-audit** -- may be triggered by a brief that requires channel evaluation before execution planning
