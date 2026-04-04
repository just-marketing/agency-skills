---
name: juma-onboarding-checklist
description: "Use when a new client has signed their SOW and the agency needs to provision access, set up project infrastructure, run the kickoff meeting, and execute the first-30-days plan. Produces a comprehensive checklist with owners, deadlines, and status tracking."
---

# New Client Onboarding Checklist

Manages the end-to-end onboarding workflow for a new agency client, from signed SOW through the first 30 days of active work. Covers access provisioning, Juma project setup, kickoff meeting execution, initial audit scheduling, communication cadence, reporting configuration, stakeholder mapping, and first-30-days milestones. Designed to ensure nothing falls through the cracks during the critical first month of an engagement.

## When to Use

- A new client has signed a statement of work and the engagement is ready to begin
- An existing client has added a significant new service that requires onboarding to new platforms or channels
- A client engagement is being transferred between account teams and a re-onboarding is needed
- The agency is standardizing its onboarding process and needs a template to follow
- A past onboarding had issues and the team wants to run a more structured process for the next client

## Prerequisites

- **juma-client-context** (required) -- must be populated with client company details, key contacts, industry, goals, and contracted services before onboarding begins
- Signed statement of work (SOW) with clearly defined services, deliverables, and timeline
- Assigned account team (account manager, strategist, specialists) with confirmed availability
- Client's primary contact information and communication preferences
- Agency onboarding email templates and welcome packet (if standard materials exist)

## Process

1. **Signed SOW triggers the checklist**
   - Confirm the SOW is fully executed (both parties signed)
   - Create the onboarding project in the project management platform (Asana, Monday, ClickUp, etc.)
   - Assign the account team and notify all team members of the new engagement
   - Send the client a welcome email with introduction to the team, what to expect in the first week, and a list of access credentials and assets the agency will need
   - Schedule the kickoff meeting within the first 5 business days

2. **Provision access to all platforms**
   - Work through the access checklist systematically (see Output Format for the full list)
   - Request access via the client's preferred method (direct credentials, admin invitations, or agency manager accounts)
   - Verify each platform login works and the agency has the appropriate permission level
   - Document all access credentials in the agency's secure credential manager (never in email, chat, or documents)
   - Flag any access that is delayed or blocked and escalate to the client contact
   - Target: all critical access provisioned within 5 business days of SOW signing

3. **Set up the Juma project**
   - Create a new Project in Juma for this client
   - Upload brand context: brand guidelines, tone of voice documents, logos, color palettes, typography specs
   - Upload audience documentation: personas, customer segments, ICPs
   - Upload competitive context: known competitors, positioning documents
   - Configure AI assistants with client-specific instructions and guardrails
   - Load historical performance data if available (previous reports, benchmarks, baselines)
   - Connect relevant data integrations (analytics, ad platforms, CRM)

4. **Prepare and run the kickoff meeting**
   - Send the kickoff agenda to all attendees at least 2 business days in advance
   - Kickoff agenda covers:
     - Introductions: agency team members and their roles, client team members and their roles
     - Goals alignment: review the SOW objectives, confirm priority order, discuss how success will be measured
     - Communication preferences: preferred channels (email, Slack, Teams), response time expectations, escalation path
     - Quick wins identification: discuss 2-3 things the agency can deliver or improve in the first two weeks to build momentum and confidence
     - Timeline review: walk through the first-30-days plan, confirm key milestone dates
     - Open questions: address any client concerns, clarify ambiguities in the SOW
   - Document all decisions, action items, and open questions from the kickoff
   - Distribute the kickoff summary to all attendees within 24 hours

5. **Schedule the initial audits**
   - Based on the contracted services and client priorities, schedule audits in the appropriate order:
     - **Week 1-2 (Foundation):** Analytics audit (is tracking accurate?), brand/messaging review
     - **Week 2-3 (Channel-specific):** Channel audit, SEO audit, paid media audit, social audit -- whichever are relevant to the engagement
     - **Week 3-4 (Strategic):** Competitive analysis, content audit, conversion rate review
   - Assign each audit to the appropriate team member with a clear deadline
   - Confirm the client has provided all access needed for each audit before it begins

6. **Establish communication cadence and reporting**
   - Set up the recurring meeting schedule:
     - Weekly or biweekly status meetings (confirm day, time, duration, attendees, platform)
     - Monthly or quarterly strategy reviews (if applicable)
   - Create the shared communication channel (Slack Connect, Teams channel, or equivalent)
   - Define the reporting configuration:
     - KPIs to track (tied to SOW objectives)
     - Report format (dashboard, slide deck, written report)
     - Reporting frequency (weekly, biweekly, monthly)
     - Report delivery method (email, live meeting walkthrough, shared dashboard link)
   - Set up automated reporting where possible (Looker Studio, AgencyAnalytics, etc.)
   - Document the escalation path: who to contact for what, and how urgent issues are handled

7. **Execute the first-30-days plan**
   - Track progress against the milestone plan (see Output Format for the weekly breakdown)
   - Hold a brief internal team sync at the end of each week to review onboarding progress
   - Address any blocked items immediately -- the first 30 days set the tone for the entire engagement
   - At the end of Week 4, conduct an internal onboarding retrospective: what went well, what was delayed, what should change for the next client

8. **Document everything**
   - Ensure all onboarding decisions, access details, meeting notes, and audit findings are stored in the project management platform and Juma
   - Update juma-client-context with any new information gathered during onboarding
   - Create the client's stakeholder map and store it where the full account team can access it
   - Confirm the onboarding checklist is complete and archive it for reference

## Output Format

```markdown
# Client Onboarding Checklist: [Client Name]
**SOW Signed:** [Date]
**Kickoff Date:** [Date]
**Account Manager:** [Name]
**Account Team:** [Names and roles]

---

## Stakeholder Map

### Client Side
| Name | Title | Role in Engagement | Decision Authority | Contact |
|------|-------|-------------------|-------------------|---------|
| [Name] | [Title] | Day-to-day contact | [Approvals, feedback, etc.] | [Email, phone] |
| [Name] | [Title] | Executive sponsor | [Budget, strategic decisions] | [Email, phone] |
| [Name] | [Title] | Subject matter expert | [Technical, product, brand input] | [Email, phone] |

### Agency Side
| Name | Role | Responsibilities | Allocation % |
|------|------|-----------------|-------------|
| [Name] | Account Manager | Client communication, project oversight | [X%] |
| [Name] | Strategist | Strategy development, audits, planning | [X%] |
| [Name] | Specialist | Channel execution, optimization | [X%] |

---

## Access Provisioning Checklist

### Analytics
- [ ] Google Analytics 4 -- [Status: Requested/Granted/Verified] -- [Date]
- [ ] Adobe Analytics -- [Status] -- [Date]
- [ ] Google Search Console -- [Status] -- [Date]
- [ ] Google Tag Manager -- [Status] -- [Date]
- [ ] Other analytics: [Platform] -- [Status] -- [Date]

### Ad Platforms
- [ ] Google Ads -- [Status] -- [Date]
- [ ] Meta Ads Manager (Facebook/Instagram) -- [Status] -- [Date]
- [ ] LinkedIn Campaign Manager -- [Status] -- [Date]
- [ ] TikTok Ads Manager -- [Status] -- [Date]
- [ ] Microsoft Ads (Bing) -- [Status] -- [Date]
- [ ] Other ad platform: [Platform] -- [Status] -- [Date]

### CMS & Website
- [ ] CMS access (WordPress, Shopify, Webflow, etc.) -- [Status] -- [Date]
- [ ] Hosting / CDN access (if needed) -- [Status] -- [Date]
- [ ] Landing page platform (Unbounce, Instapage, etc.) -- [Status] -- [Date]

### Social Media Accounts
- [ ] Facebook Page admin -- [Status] -- [Date]
- [ ] Instagram account -- [Status] -- [Date]
- [ ] LinkedIn Company Page admin -- [Status] -- [Date]
- [ ] Twitter/X account -- [Status] -- [Date]
- [ ] TikTok account -- [Status] -- [Date]
- [ ] YouTube channel manager -- [Status] -- [Date]
- [ ] Other social: [Platform] -- [Status] -- [Date]

### Email & CRM
- [ ] Email marketing platform (Mailchimp, Klaviyo, HubSpot, etc.) -- [Status] -- [Date]
- [ ] CRM access (Salesforce, HubSpot, Pipedrive, etc.) -- [Status] -- [Date]
- [ ] Marketing automation platform -- [Status] -- [Date]

### Brand & Creative Assets
- [ ] Brand guidelines document -- [Status] -- [Date]
- [ ] Logo files (vector + raster) -- [Status] -- [Date]
- [ ] Font files or font family names -- [Status] -- [Date]
- [ ] Color palette (hex codes) -- [Status] -- [Date]
- [ ] Photography / image library access -- [Status] -- [Date]
- [ ] Design asset library (Figma, Canva, shared drive) -- [Status] -- [Date]
- [ ] Previous campaign creative -- [Status] -- [Date]

### Other
- [ ] Project management platform invitation -- [Status] -- [Date]
- [ ] Shared drive / document repository access -- [Status] -- [Date]
- [ ] Call tracking platform (CallRail, etc.) -- [Status] -- [Date]
- [ ] Review platform (Yelp, Google Business Profile, etc.) -- [Status] -- [Date]

**Access blockers:**
- [Platform] -- [Issue] -- [Escalation action] -- [Owner]

---

## Juma Project Setup

- [ ] Juma Project created -- [Date]
- [ ] Brand guidelines uploaded -- [Date]
- [ ] Audience personas / ICPs uploaded -- [Date]
- [ ] Competitive context uploaded -- [Date]
- [ ] AI assistants configured with client-specific instructions -- [Date]
- [ ] Historical performance data loaded -- [Date]
- [ ] Data integrations connected -- [Date]
- [ ] Team members added to Juma project -- [Date]

---

## Kickoff Meeting

**Date/Time:** [Date, Time, Duration]
**Location/Platform:** [Zoom, Google Meet, In-person, etc.]
**Attendees:** [Names]

### Agenda
1. Introductions (10 min)
2. Goals alignment and success metrics (15 min)
3. Communication preferences and cadence (10 min)
4. Quick wins discussion (10 min)
5. First-30-days timeline review (10 min)
6. Open questions and next steps (5 min)

### Kickoff Decisions & Action Items
| Decision/Action | Owner | Deadline | Status |
|----------------|-------|----------|--------|
| [Item] | [Name] | [Date] | [Open/Done] |
| [Item] | [Name] | [Date] | [Open/Done] |

---

## Communication Cadence

| Meeting/Touchpoint | Frequency | Day/Time | Attendees | Platform |
|-------------------|-----------|----------|-----------|----------|
| Status meeting | [Weekly/Biweekly] | [Day, Time] | [Names] | [Platform] |
| Strategy review | [Monthly/Quarterly] | [Day, Time] | [Names] | [Platform] |
| Async updates | [As needed] | -- | [Names] | [Slack/Teams/Email] |

### Escalation Path
- **Routine questions:** [Contact] via [Channel]
- **Urgent issues:** [Contact] via [Channel], response expected within [X hours]
- **Executive escalation:** [Contact] via [Channel]

### Reporting Configuration
| Element | Setting |
|---------|---------|
| Primary KPIs | [List of KPIs tied to SOW objectives] |
| Report format | [Dashboard / Slide deck / Written report] |
| Reporting frequency | [Weekly / Biweekly / Monthly] |
| Delivery method | [Email / Meeting / Shared link] |
| Reporting platform | [Looker Studio / AgencyAnalytics / Manual / etc.] |

---

## Initial Audit Schedule

| Audit | Assigned To | Start Date | Due Date | Status | Access Required |
|-------|-------------|-----------|----------|--------|-----------------|
| Analytics audit | [Name] | [Date] | [Date] | [Not Started/In Progress/Complete] | [GA4, GTM] |
| Channel audit | [Name] | [Date] | [Date] | [Status] | [All platforms] |
| SEO audit | [Name] | [Date] | [Date] | [Status] | [GSC, CMS, GA4] |
| Paid media audit | [Name] | [Date] | [Date] | [Status] | [Ad platforms] |
| Social audit | [Name] | [Date] | [Date] | [Status] | [Social accounts] |
| Content audit | [Name] | [Date] | [Date] | [Status] | [CMS, GA4] |
| Competitive analysis | [Name] | [Date] | [Date] | [Status] | [None] |

---

## First-30-Days Milestones

### Week 1: Access + Kickoff
- [ ] Welcome email sent to client -- [Owner] -- [Date]
- [ ] All access requests submitted -- [Owner] -- [Date]
- [ ] Juma project created and brand context uploaded -- [Owner] -- [Date]
- [ ] Kickoff meeting completed -- [Owner] -- [Date]
- [ ] Kickoff summary distributed -- [Owner] -- [Date]
- [ ] Communication channels established (Slack/Teams, meeting cadence) -- [Owner] -- [Date]
- [ ] Quick wins identified and execution started -- [Owner] -- [Date]

### Week 2: Initial Audits
- [ ] All critical access verified and working -- [Owner] -- [Date]
- [ ] Analytics audit completed -- [Owner] -- [Date]
- [ ] Channel-specific audits started -- [Owner] -- [Date]
- [ ] First status meeting held -- [Owner] -- [Date]
- [ ] Quick wins delivered or in progress -- [Owner] -- [Date]
- [ ] Reporting template drafted -- [Owner] -- [Date]

### Week 3: Strategy Development
- [ ] All audits completed -- [Owner] -- [Date]
- [ ] Audit findings presented to client -- [Owner] -- [Date]
- [ ] Initial strategy and recommendations developed -- [Owner] -- [Date]
- [ ] Reporting template finalized and first report delivered -- [Owner] -- [Date]
- [ ] Any access blockers resolved -- [Owner] -- [Date]

### Week 4: First Deliverables + Review
- [ ] First round of strategic deliverables completed -- [Owner] -- [Date]
- [ ] Client review and feedback on initial deliverables -- [Owner] -- [Date]
- [ ] 30-day internal retrospective completed -- [Owner] -- [Date]
- [ ] juma-client-context updated with all onboarding learnings -- [Owner] -- [Date]
- [ ] Onboarding checklist marked complete and archived -- [Owner] -- [Date]

---

## Onboarding Health Check

**Completed at end of Week 4:**

| Question | Answer | Notes |
|----------|--------|-------|
| Is all access provisioned and verified? | [Yes/No] | [Details on any gaps] |
| Were all audits completed on time? | [Yes/No] | [Details on any delays] |
| Is the client satisfied with the first 30 days? | [Yes/No/Unclear] | [Evidence] |
| Is the communication cadence working? | [Yes/No] | [Adjustments needed] |
| Are reports configured and delivering on schedule? | [Yes/No] | [Details] |
| Is the Juma project fully set up? | [Yes/No] | [Missing items] |
| Did we deliver on quick wins? | [Yes/No] | [What was delivered] |
| What should we do differently next time? | [Lessons learned] | |
```

## Common Mistakes

- **Starting work before access is confirmed**: The team begins channel audits or optimizations only to discover they have read-only access or the wrong account linked. Verify permissions before any work begins.
- **Skipping the kickoff or treating it as a formality**: The kickoff meeting is where expectations are set, relationships are built, and misunderstandings are caught early. A poorly run kickoff creates problems that compound for months.
- **Not identifying quick wins**: The first two weeks are when the client is evaluating whether they made the right choice. Delivering a visible, tangible improvement early builds trust and buys time for deeper strategic work.
- **Failing to document the stakeholder map**: Not knowing who approves what leads to delays, rework, and frustrated clients. Map decision authority during onboarding, not after the first approval bottleneck.
- **Letting access provisioning drag on**: If access is not escalated aggressively in Week 1, it can delay audits and deliverables for the entire first month. Set a 5-business-day target and escalate daily after that.
- **Not setting up reporting from Day 1**: If the client does not see a report until Week 4, they have spent three weeks wondering what the agency is doing. Even a simple Week 1 status update demonstrates professionalism and transparency.
- **Assuming the client knows how agencies work**: Many clients are working with an agency for the first time. Explain the process, set expectations for turnaround times, and clarify what they need to provide vs what the agency handles.
- **No internal retrospective at Day 30**: Without reviewing the onboarding process, the same mistakes repeat for every new client. The five-minute retrospective is the most valuable meeting of the onboarding.

## Related Skills

- **juma-client-context** -- must be populated as the first step of onboarding; updated throughout the process
- **juma-channel-audit** -- the primary audit run during Weeks 2-3 of onboarding
- **juma-sow** -- the signed SOW is the trigger for onboarding and defines the scope of all setup activities
- **juma-proposal** -- onboarding begins after a proposal is accepted and SOW is signed
- **juma-retainer-review** -- the onboarding baseline data (hours, deliverables, access) becomes the foundation for future retainer reviews
- **juma-content-calendar** -- content calendar setup is often one of the first strategic deliverables after onboarding audits
