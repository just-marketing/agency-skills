---
name: juma-sow
description: "Use when converting an accepted proposal into a binding statement of work, or when scoping any new project engagement. Produces a detailed SOW with deliverables, acceptance criteria, timeline, revision policy, out-of-scope definitions, change order process, and milestone-based payment schedule."
---

# Statement of Work

## Overview

The Statement of Work is the operational contract between agency and client that translates a winning proposal into an executable engagement. It eliminates ambiguity by defining exactly what will be delivered, when, by whom, how success is measured, and what happens when things change. A well-built SOW is the single most effective tool for preventing scope creep, protecting agency margins, and ensuring client satisfaction -- because misaligned expectations, not bad work, are the leading cause of client churn.

This skill produces a SOW that is specific enough to be legally defensible, clear enough that both parties can self-audit progress, and structured to protect the agency from unbounded revisions and undocumented requests.

## When to Use

- A proposal has been accepted and the engagement needs to be formalized before work begins
- Scoping a new project within an existing retainer relationship
- Resetting scope after a period of scope creep has eroded profitability
- Expanding or modifying an existing engagement based on a change order
- A client requests work that does not fit neatly into the current agreement
- Transitioning from a pilot or trial engagement to a full contract

## Prerequisites

- **juma-client-context**: Must be populated with client company details, goals, KPIs, marketing stack, team structure, and approval workflows
- **juma-proposal** (recommended): The accepted proposal provides the strategic framework, agreed scope, and selected pricing tier that the SOW formalizes
- Confirmed pricing tier and budget from the proposal or client negotiation
- Internal team allocation and availability confirmed
- Client stakeholder map with decision-making authority for approvals and sign-offs
- Knowledge of the client's legal or procurement requirements for contract format

## Process

1. **Reference the accepted proposal**: Pull the agreed-upon scope, pricing tier, deliverables, timeline, and strategic approach from the accepted proposal. Identify anything that was discussed verbally during the sales process but not captured in the proposal -- these items must be explicitly included or excluded in the SOW.

2. **Break deliverables into work items**: Decompose each proposal deliverable into specific, measurable work items. For each work item, define exactly what the agency will produce, in what format, and to what specification. Avoid bundling multiple outputs into a single deliverable -- granularity prevents disputes.

3. **Define acceptance criteria**: For every deliverable, write explicit acceptance criteria that answer: "How will both parties know this deliverable is complete and satisfactory?" Acceptance criteria must be objective and testable, not subjective. "Client is happy with the design" is not acceptance criteria. "Design delivered in Figma, responsive across 3 breakpoints, incorporating brand guidelines from client context" is.

4. **Build the timeline**: Map all deliverables to a timeline with start dates, internal milestones, client review periods, and final delivery dates. Identify dependencies between deliverables and between agency work and client inputs. Build in buffer for client review delays -- specify that agency timelines shift day-for-day when client feedback is late.

5. **Document boundaries**: Write the out-of-scope section explicitly. List specific items that a reasonable person might assume are included but are not. Define the revision policy with exact numbers of rounds and turnaround times. Write the change order process so that any work beyond the SOW has a clear, documented path to approval and billing.

6. **Review with client**: Walk through the SOW with the client stakeholder, paying special attention to acceptance criteria, out-of-scope items, and the revision policy. Document any negotiated changes. Obtain sign-off from an authorized decision-maker before work begins.

## Output Format

```
# Statement of Work

**Client:** [Client Name]
**Agency:** [Agency Name]
**SOW Reference:** [SOW-YYYY-XXX]
**Date:** [Date]
**Version:** [1.0]
**Prepared by:** [Name, Title]
**Client Approver:** [Name, Title]

---

## 1. Project Overview

### Background
[2-3 sentences on the context for this engagement. Reference the proposal and the client's core objectives.]

### Objectives
1. [Specific, measurable objective tied to a business outcome]
2. [Specific, measurable objective tied to a business outcome]
3. [Specific, measurable objective tied to a business outcome]

### Success Criteria
[How will both parties evaluate whether this engagement has been successful at its conclusion? Define 2-3 measurable outcomes.]

---

## 2. Scope of Work

See [deliverable-spec-template.md](deliverable-spec-template.md) for the per-deliverable specification template with acceptance criteria guidelines. Repeat for each deliverable -- every deliverable in the proposal must appear here.

---

## 3. Timeline & Milestones

| Milestone | Deliverables Included | Target Date | Dependencies | Status |
|---|---|---|---|---|
| Project Kickoff | Kickoff meeting, access provisioning | [Date] | SOW signed | Pending |
| [Milestone 1 Name] | [Deliverables X, Y] | [Date] | [Dependencies] | Pending |
| [Milestone 2 Name] | [Deliverables X, Y] | [Date] | [Dependencies] | Pending |
| [Milestone 3 Name] | [Deliverables X, Y] | [Date] | [Dependencies] | Pending |
| Project Close / Transition | Final deliverables, handoff | [Date] | All prior milestones | Pending |

**Timeline Assumptions:**
- Client feedback will be provided within [X] business days of each deliverable submission
- Agency timelines shift day-for-day for any client feedback provided beyond the agreed review period
- Milestones are sequential unless otherwise noted; delays in earlier milestones will impact subsequent dates

---

## 4. Roles & Responsibilities

### Agency Team

| Role | Name | Responsibilities |
|---|---|---|
| Account Director | [Name] | Primary client contact, strategic oversight, escalation point |
| Project Manager | [Name] | Day-to-day execution management, timeline tracking, status reporting |
| [Specialist Role] | [Name] | [Specific responsibilities for this engagement] |
| [Specialist Role] | [Name] | [Specific responsibilities for this engagement] |

### Client Team

| Role | Name | Responsibilities |
|---|---|---|
| Primary Contact | [Name] | Day-to-day communication, feedback coordination, internal routing |
| Approver | [Name] | Final sign-off on deliverables and milestones |
| Subject Matter Expert | [Name] | Providing industry/product knowledge, reviewing technical accuracy |
| [Additional Role] | [Name] | [Specific responsibilities] |

### Client Obligations
The client is responsible for providing the following in a timely manner:
- [Specific asset, access, or information needed, with deadline]
- [Specific asset, access, or information needed, with deadline]
- [Specific asset, access, or information needed, with deadline]

Failure to provide required inputs by the specified dates may result in timeline adjustments per the timeline assumptions above.

---

## 5. Communication Plan

| Meeting/Touchpoint | Frequency | Attendees | Format | Purpose |
|---|---|---|---|---|
| Kickoff Meeting | Once | Full team (agency + client) | Video call | Align on scope, timeline, introductions |
| Status Update | [Weekly/Biweekly] | PM + Client Primary Contact | [Call/Email/Slack] | Progress review, blocker resolution |
| Strategy Review | [Monthly/Biweekly] | Account Director + Client Approver | Video call | Strategic alignment, performance check |
| Deliverable Review | Per milestone | Relevant specialists + Client reviewers | [Format] | Present work, gather feedback |

**Reporting:** [Describe what reports will be delivered, in what format, and on what cadence]

**Tools:**
- Project management: [Tool name -- where tasks and timelines are tracked]
- Communication: [Tool name -- primary async communication channel]
- File sharing: [Tool name -- where deliverables and assets are stored]

**Escalation Path:** [Describe how issues are escalated if not resolved at the working level. Include names and response time expectations.]

---

## 6. Revision Policy

See [revision-policy-template.md](revision-policy-template.md) for the complete revision policy structure by deliverable type, including revision definitions.

---

## 7. Out of Scope

The following items are explicitly excluded from this engagement. If any of these items become necessary, they will be addressed through the change order process defined in Section 8.

- [Specific exclusion that a reasonable person might assume is included]
- [Specific exclusion that a reasonable person might assume is included]
- [Specific exclusion that a reasonable person might assume is included]
- [Specific exclusion that a reasonable person might assume is included]
- [Specific exclusion that a reasonable person might assume is included]

**General Exclusions:**
- Third-party software licenses, media spend, or vendor costs unless explicitly listed in the deliverables
- Work requested by client team members outside the designated approval chain
- Deliverables or revisions requested outside the agreed-upon scope without an approved change order
- Support or maintenance after the engagement period ends unless covered by a separate agreement

---

## 8. Change Order Process

See [change-order-template.md](change-order-template.md) for the complete change order process and document template.

---

## 9. Payment Schedule

| Payment | Amount | Trigger | Due Date |
|---|---|---|---|
| Deposit | $[X] ([X]% of total) | SOW execution | Upon signing |
| Milestone 1 Payment | $[X] ([X]% of total) | [Milestone 1] completion and acceptance | Net [X] from invoice |
| Milestone 2 Payment | $[X] ([X]% of total) | [Milestone 2] completion and acceptance | Net [X] from invoice |
| Final Payment | $[X] ([X]% of total) | All deliverables accepted | Net [X] from invoice |
| **Total** | **$[X]** | | |

**Payment Terms:**
- Invoices are issued upon milestone completion and are due Net [X] days
- Late payments are subject to a [X]% monthly finance charge
- Work may be paused if any invoice remains unpaid beyond [X] days past due
- Change orders are invoiced separately upon completion of the additional work

---

## 10. Termination & Transition

### Termination by Client
- Client may terminate this SOW with [X] days written notice
- Client is responsible for payment of all work completed through the termination date, plus any non-cancellable commitments made on the client's behalf
- A termination fee of [X]% of the remaining contract value applies if terminated before [milestone/date]

### Termination by Agency
- Agency may terminate with [X] days written notice if client obligations are not met after documented escalation
- Agency may terminate immediately if payment is more than [X] days overdue

### Transition
Upon termination or completion of this engagement:
- Agency will deliver all completed work and work-in-progress within [X] business days
- Agency will provide a transition document covering active campaigns, account access, and pending items
- Client retains ownership of all final, accepted deliverables
- Agency retains ownership of proprietary methodologies, frameworks, and tools used in execution
- Access to agency tools and platforms will be revoked [X] days after the engagement ends

---

## Signatures

**Client:**

Name: ___________________________
Title: ___________________________
Date: ___________________________
Signature: ___________________________

**Agency:**

Name: ___________________________
Title: ___________________________
Date: ___________________________
Signature: ___________________________
```

## Common Mistakes

- **Vague acceptance criteria**: "Client approves the deliverable" is not acceptance criteria. Every deliverable must have objective, testable criteria that remove subjectivity from the approval process. If you cannot write a checklist that a third party could evaluate, the criteria are not specific enough.
- **No revision limits**: Unlimited revisions is a margin killer. Define exact numbers of revision rounds per deliverable type, specify that consolidated feedback counts as one round, and price additional rounds explicitly. This protects the agency and forces the client to provide organized, thoughtful feedback.
- **Missing out-of-scope section**: If you do not explicitly state what is excluded, the client will reasonably assume it is included. The out-of-scope section should list every item that exists in the gray zone -- things a reasonable person might expect but that are not part of this engagement.
- **Bundling deliverables**: "Digital marketing package" is not a deliverable. Break everything into individual, trackable work items. Bundling hides scope, makes progress impossible to measure, and creates disputes about what was promised.
- **No client obligations with deadlines**: The SOW must specify what the client needs to provide and when. Without this, the agency absorbs all timeline risk from delayed client feedback, missing assets, and slow approvals.
- **Change order process that nobody will follow**: If the change order process is too bureaucratic, the team will skip it and absorb out-of-scope work informally. Keep it simple: identify, document, approve, execute. But never skip it.
- **Payment schedule disconnected from milestones**: Tying payments to calendar dates instead of deliverable milestones creates misaligned incentives. The client pays for completed work, and the agency is motivated to hit milestones. Never do more than 50% of the work before receiving at least 50% of the payment.
- **Forgetting the transition clause**: Every engagement ends eventually. Without a transition clause, the offboarding becomes chaotic, assets get lost, and the relationship ends badly -- destroying any chance of future re-engagement or referrals.

## Related Skills

- **juma-client-context**: Provides the client intelligence, goals, team structure, and approval workflows that shape the SOW
- **juma-proposal**: The accepted proposal is the primary input for the SOW -- scope, pricing tier, and strategic approach flow directly from it
- **juma-reporting**: The reporting cadence and KPIs defined in the SOW dictate the structure of ongoing performance reports
- **juma-client-qbr**: Quarterly business reviews assess progress against the milestones and success criteria defined here
- **juma-onboarding-checklist**: The SOW's client obligations and access requirements feed into the onboarding process
- **juma-retainer-review**: For ongoing retainer engagements, periodic retainer reviews assess whether the SOW scope still matches the client's needs
- **juma-upsell-finder**: Out-of-scope items and change orders often surface upsell opportunities for expanded engagements
