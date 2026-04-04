---
name: juma-client-context
description: "Use when onboarding a new client, starting any engagement, or when another skill requires client context. Produces a structured client profile covering brand identity, audiences, competitors, marketing stack, goals, voice, budget, and performance baselines."
---

# Client Context Profile

## Overview

The Client Context Profile is the foundational skill for the entire Juma.ai agency skills suite. It creates a comprehensive, structured profile of an agency client that every other skill depends on for accurate, tailored outputs. Without a properly built client context, downstream skills like campaign planning, content calendars, and proposals will produce generic work that misses the mark.

This skill transforms scattered client knowledge -- across intake calls, websites, social profiles, analytics, and tribal agency knowledge -- into a single, referenceable document that any team member or skill can consume immediately.

## When to Use

- A new client is being onboarded to the agency
- Starting a new engagement or project with an existing client
- Another juma- skill lists `juma-client-context` as a prerequisite and no profile exists yet
- An existing client profile is outdated (quarterly refresh recommended)
- The agency is preparing a pitch or proposal and needs to formalize prospect research
- A new team member is taking over an account and needs to get up to speed

## Prerequisites

None. This is the foundation skill that all other skills depend on. It has no upstream dependencies.

## Process

### Step 1: Gather Information from the User

Ask the following structured questions in conversational order. Do not dump all questions at once -- group them into logical blocks and confirm understanding before moving on.

**Block A -- Brand Identity**

1. What is the client's official brand name and any sub-brands or product lines?
2. How does the client describe what they do in one sentence? (elevator pitch)
3. What is their stated mission or purpose?
4. What are their core brand values (typically 3-5)?
5. What is their unique selling proposition -- what makes them genuinely different from competitors?
6. What is their current brand positioning? (e.g., premium, value, disruptor, legacy leader)

**Block B -- Target Audiences**

For each audience segment (aim for 2-4 segments):

1. Who are they targeting? (segment name and description)
2. What are the key demographics? (age range, location, income, job title/role, industry)
3. What are the psychographics? (motivations, aspirations, lifestyle, media consumption)
4. What pain points or challenges does this audience face that the client solves?
5. Where does this audience spend time online and offline? (specific platforms and channels)
6. What does the buyer journey look like for this segment? (awareness to purchase timeline)

**Block C -- Competitive Landscape**

1. Who are their top 3-5 direct competitors?
2. Who are 1-2 indirect or aspirational competitors?
3. For each competitor: what is their positioning, and what are they known for?
4. Where does the client believe they win against each competitor?
5. Where does the client believe they lose?
6. Are there any competitor campaigns or tactics the client admires or wants to counter?

**Block D -- Marketing Stack & Operations**

1. What marketing tools and platforms are currently in use? (CRM, email, analytics, ad platforms, CMS, social tools, SEO tools, project management)
2. What integrations exist between tools? (e.g., CRM syncs to email platform)
3. Which Juma.ai projects are connected to this client?
4. Who manages marketing internally at the client? (team size, roles, decision-makers)
5. What does the content creation process look like? (in-house, agency, freelancers, hybrid)
6. What approval workflows exist? (who signs off, how many rounds, typical turnaround)

**Block E -- Goals & KPIs**

1. What are the top 3 business goals for the next 12 months?
2. What marketing KPIs does the client currently track?
3. For each KPI: what is the current baseline and what is the target?
4. How does the client attribute revenue to marketing? (first touch, last touch, multi-touch, gut feel)
5. What does "success" look like for this agency engagement specifically?
6. Are there any hard deadlines or seasonal peaks that drive urgency?

**Block F -- Brand Voice & Tone**

1. What 3-5 adjectives describe how the brand should sound? (e.g., authoritative, approachable, bold)
2. What adjectives should the brand never sound like? (e.g., corporate, salesy, casual)
3. Are there specific words or phrases the brand always uses?
4. Are there words or phrases that are off-limits?
5. Can you share 2-3 examples of content the client considers "on-brand"?
6. Does the tone shift across channels? (e.g., more casual on social, more formal in whitepapers)

**Block G -- Budget & Constraints**

1. What is the monthly and/or annual marketing budget?
2. How is the budget currently allocated across channels? (rough percentages are fine)
3. Are there channels or tactics the client will not invest in?
4. What is the agency retainer or project fee structure?
5. What is the approval process for budget changes or overspend?
6. Are there legal, compliance, or regulatory constraints? (e.g., healthcare, finance, alcohol)

**Block H -- Current Performance Baseline**

1. What is the current monthly website traffic? (total sessions, unique visitors)
2. What are the primary traffic sources and their proportions?
3. What is the current lead volume and lead-to-customer conversion rate?
4. What is the customer acquisition cost (CAC) by channel if known?
5. What is the current revenue attribution from marketing?
6. What engagement metrics matter most? (email open rates, social engagement rates, etc.)

### Step 2: Research the Client's Online Presence

Using available tools, verify and supplement the information gathered:

1. Review the client's website for messaging, positioning, and content quality
2. Check social media profiles for posting frequency, engagement, and tone
3. Look at competitor websites and social profiles for comparison
4. Verify any stated metrics against available public data
5. Note discrepancies between what the client says and what the data shows

### Step 3: Compile and Structure the Profile

Organize all gathered information into the output format below. Fill every section. Where information is unavailable, mark it explicitly as `[TO BE CONFIRMED]` rather than leaving it blank or guessing.

### Step 4: Validate with the User

Present the completed profile and ask:

1. Is any information incorrect or outdated?
2. Are there gaps I marked as `[TO BE CONFIRMED]` that you can fill now?
3. Is there anything missing that would be important for the team to know?
4. Who should be the ongoing point of contact for updates to this profile?

Make all corrections before finalizing.

## Output Format

```markdown
# Client Context Profile: [Client Name]

**Last Updated:** [Date]
**Agency Team:** [Account lead, strategist, and other key team members]
**Juma.ai Project:** [Link or project ID]

---

## 1. Brand Identity

| Field | Detail |
|-------|--------|
| **Brand Name** | [Official name and any sub-brands] |
| **Elevator Pitch** | [One-sentence description of what they do] |
| **Mission** | [Stated mission or purpose] |
| **Core Values** | [Value 1], [Value 2], [Value 3], [Value 4] |
| **USP** | [What genuinely differentiates them] |
| **Positioning** | [Market position: premium / value / disruptor / etc.] |

---

## 2. Target Audiences

### Segment 1: [Segment Name]

- **Demographics:** [Age, location, income, job title, industry]
- **Psychographics:** [Motivations, aspirations, lifestyle]
- **Pain Points:** [Top 3 challenges this segment faces]
- **Preferred Channels:** [Where they spend attention]
- **Buyer Journey:** [Awareness-to-purchase timeline and key touchpoints]

### Segment 2: [Segment Name]

- **Demographics:** [Age, location, income, job title, industry]
- **Psychographics:** [Motivations, aspirations, lifestyle]
- **Pain Points:** [Top 3 challenges this segment faces]
- **Preferred Channels:** [Where they spend attention]
- **Buyer Journey:** [Awareness-to-purchase timeline and key touchpoints]

### Segment 3: [Segment Name]

- **Demographics:** [Age, location, income, job title, industry]
- **Psychographics:** [Motivations, aspirations, lifestyle]
- **Pain Points:** [Top 3 challenges this segment faces]
- **Preferred Channels:** [Where they spend attention]
- **Buyer Journey:** [Awareness-to-purchase timeline and key touchpoints]

*(Add Segment 4 if applicable)*

---

## 3. Competitive Landscape

### [Competitor 1 Name]

- **Positioning:** [How they position themselves]
- **Strengths:** [What they do well]
- **Weaknesses:** [Where they fall short]
- **Key Differentiator vs. Client:** [Why a customer might choose them over our client]

### [Competitor 2 Name]

- **Positioning:** [How they position themselves]
- **Strengths:** [What they do well]
- **Weaknesses:** [Where they fall short]
- **Key Differentiator vs. Client:** [Why a customer might choose them over our client]

### [Competitor 3 Name]

- **Positioning:** [How they position themselves]
- **Strengths:** [What they do well]
- **Weaknesses:** [Where they fall short]
- **Key Differentiator vs. Client:** [Why a customer might choose them over our client]

*(Add Competitors 4-5 if applicable)*

**Competitive Summary:** [2-3 sentences on where the client stands in the competitive landscape and the biggest opportunity gap]

---

## 4. Marketing Stack

| Category | Tool/Platform | Status | Notes |
|----------|---------------|--------|-------|
| **CRM** | [Tool name] | [Active / Underused / Planned] | [Integration notes] |
| **Email Marketing** | [Tool name] | [Active / Underused / Planned] | [List size, send frequency] |
| **Analytics** | [Tool name] | [Active / Underused / Planned] | [Tracking status] |
| **Ad Platforms** | [Tool name(s)] | [Active / Underused / Planned] | [Monthly spend range] |
| **CMS** | [Tool name] | [Active / Underused / Planned] | [Site details] |
| **Social Management** | [Tool name] | [Active / Underused / Planned] | [Platforms managed] |
| **SEO Tools** | [Tool name] | [Active / Underused / Planned] | [Key metrics tracked] |
| **Project Management** | [Tool name] | [Active / Underused / Planned] | [Workflow details] |

**Juma.ai Integration:** [How client work maps to Juma.ai projects, automations, or workflows]

**Internal Team:**
- [Role]: [Name] -- [Responsibilities and decision-making authority]
- [Role]: [Name] -- [Responsibilities and decision-making authority]

**Content Workflow:** [Description of how content moves from ideation to publication, including who creates, reviews, and approves]

---

## 5. Goals & KPIs

### Business Goals (Next 12 Months)

1. [Business Goal 1] -- [Why this matters]
2. [Business Goal 2] -- [Why this matters]
3. [Business Goal 3] -- [Why this matters]

### Marketing KPIs

| KPI | Current Baseline | Target | Timeline | Attribution Method |
|-----|-----------------|--------|----------|--------------------|
| [KPI 1, e.g., MQLs/month] | [Current value] | [Target value] | [By when] | [How measured] |
| [KPI 2, e.g., Organic traffic] | [Current value] | [Target value] | [By when] | [How measured] |
| [KPI 3, e.g., CAC] | [Current value] | [Target value] | [By when] | [How measured] |
| [KPI 4, e.g., ROAS] | [Current value] | [Target value] | [By when] | [How measured] |

**Agency Engagement Success Criteria:** [What specifically makes this agency engagement a success in the client's eyes]

**Key Deadlines / Seasonality:** [Any hard dates, product launches, industry events, or seasonal peaks that drive urgency]

---

## 6. Brand Voice & Tone

**Voice Attributes:** [Adjective 1], [Adjective 2], [Adjective 3], [Adjective 4], [Adjective 5]

**Never Sound Like:** [Anti-adjective 1], [Anti-adjective 2], [Anti-adjective 3]

**Always Use:**
- [Phrase or term 1]
- [Phrase or term 2]
- [Phrase or term 3]

**Never Use:**
- [Off-limits word or phrase 1]
- [Off-limits word or phrase 2]
- [Off-limits word or phrase 3]

**Sample On-Brand Phrases:**
- "[Example phrase that captures the voice]"
- "[Example phrase that captures the voice]"

**Channel-Specific Tone Adjustments:**
| Channel | Tone Shift | Example |
|---------|-----------|---------|
| Social Media | [e.g., More casual, emoji-friendly] | [Sample post snippet] |
| Email | [e.g., Conversational but professional] | [Sample subject line] |
| Website / Blog | [e.g., Authoritative, educational] | [Sample headline] |
| Sales Collateral | [e.g., Confident, data-driven] | [Sample line] |

---

## 7. Budget & Constraints

| Parameter | Detail |
|-----------|--------|
| **Monthly Marketing Budget** | [Amount or range] |
| **Annual Marketing Budget** | [Amount or range] |
| **Agency Retainer/Fee** | [Structure and amount] |
| **Budget Allocation** | [Channel breakdown with percentages] |

**Off-Limits Channels/Tactics:** [Anything the client will not invest in and why]

**Budget Approval Process:** [Who approves spend, thresholds for additional approval, turnaround time]

**Legal / Compliance Constraints:** [Industry regulations, required disclaimers, review processes, restricted claims]

---

## 8. Current Performance Baseline

### Website
- **Monthly Sessions:** [Number]
- **Unique Visitors:** [Number]
- **Top Traffic Sources:** [Source 1] ([%]), [Source 2] ([%]), [Source 3] ([%])
- **Bounce Rate:** [Percentage]
- **Avg. Session Duration:** [Time]

### Lead Generation
- **Monthly Leads:** [Number]
- **Lead-to-Customer Conversion Rate:** [Percentage]
- **Cost Per Lead (by channel):** [Channel 1]: [Amount], [Channel 2]: [Amount]

### Revenue Attribution
- **Marketing-Attributed Revenue:** [Amount or percentage of total]
- **Customer Acquisition Cost:** [Amount, by channel if available]
- **Customer Lifetime Value:** [Amount if known]

### Engagement Metrics
- **Email Open Rate:** [Percentage] | **Click Rate:** [Percentage]
- **Social Engagement Rate:** [Percentage by platform]
- **Content Performance:** [Key metric and benchmark]

**Baseline Date:** [When these numbers were captured]
**Data Confidence:** [High / Medium / Low -- note any metrics that are estimated or unreliable]

---

## Notes & Open Items

- [Any unresolved questions, pending information, or follow-up items]
- [Items marked TO BE CONFIRMED above]
```

## Common Mistakes

- **Skipping sections or accepting "I don't know"** -- Push for at least a rough answer. Mark gaps as `[TO BE CONFIRMED]` and schedule a follow-up, but never leave a section empty without flagging it.
- **Taking everything the client says at face value** -- Clients overestimate their differentiation, undercount competitors, and misremember metrics. Always verify claims against observable data in Step 2.
- **Building the profile once and never updating it** -- Client contexts drift. Schedule quarterly reviews, and update the profile whenever a major change occurs (rebrand, new product, leadership change, budget shift).
- **Making the profile too generic** -- Avoid filler language like "high-quality products" or "excellent customer service." Every entry should be specific enough that a stranger could distinguish this client from their competitors.
- **Ignoring the marketing stack details** -- Tools and integrations dictate what is actually executable. A paid media plan is useless if the client has no ad accounts set up. Map the stack thoroughly.
- **Conflating business goals with marketing KPIs** -- "Grow revenue by 30%" is a business goal. "Increase MQLs from 200 to 400/month" is a marketing KPI. Keep them distinct and show the mapping between them.
- **Writing brand voice guidelines that are too vague** -- "Professional but friendly" describes every brand. Include specific do/don't examples and sample phrases that make the voice tangible and testable.
- **Forgetting to tie the profile to Juma.ai projects** -- This profile is not just a document; it connects to active work in Juma.ai. Always link to the relevant project so the team can navigate from context to execution.

## Related Skills

- **juma-client-brief** -- Uses the client context to translate raw client requests into structured briefs
- **juma-onboarding-checklist** -- References the client context during new client onboarding
- **juma-campaign-plan** -- Pulls audience segments, goals, and budget from the context
- **juma-proposal** -- Uses brand identity, goals, and competitive landscape to build proposals
- **juma-content-calendar** -- Relies on audience segments, voice guidelines, and channel preferences
- **juma-competitor-intel** -- Expands on the competitive landscape section with deeper analysis
- **juma-channel-audit** -- Audits performance against the baseline metrics captured here
- **juma-seo-audit** -- Uses performance baseline and goals to scope SEO analysis
- **juma-paid-media-plan** -- Pulls budget, audience segments, and KPI targets
- **juma-reporting** -- Measures against the KPIs and baselines defined in the context
- **juma-sow** -- Scopes work based on goals, budget, and marketing stack
- **juma-client-qbr** -- Reviews progress against the goals and KPIs defined here

All `juma-` skills depend on this profile. If a client context does not exist, build one before running any other skill.
