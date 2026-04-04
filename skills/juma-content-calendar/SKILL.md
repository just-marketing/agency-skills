---
name: juma-content-calendar
description: "Use when building a monthly or quarterly editorial content calendar that maps pillar topics to channels, assigns resources, and plans repurposing workflows."
---

# Content Calendar

Generate a comprehensive monthly or quarterly editorial calendar that aligns content production to business goals, maps pillar topics across channels, plans publishing cadence, and builds repurposing workflows to maximize output from every piece of content.

## When to Use

- Kicking off a new content retainer and need a structured publishing plan
- Quarterly planning for an existing client's content program
- Client wants to increase content volume without proportionally increasing budget (repurposing strategy)
- Aligning content efforts with an upcoming product launch, seasonal campaign, or industry event cycle
- SEO strategy has been defined and needs to be operationalized into a publishing schedule
- Multiple teams or freelancers need a single source of truth for content assignments and deadlines

## Prerequisites

- **juma-client-context**: Must be populated with client brand voice, target audience segments, business goals, existing content channels, and any brand guidelines or approval workflows
- SEO keyword research or keyword targets (from juma-seo-strategy or equivalent)
- Knowledge of active marketing channels and their current performance baselines
- List of available content creators, designers, and approvers with capacity estimates
- Client's industry event calendar, product roadmap, and seasonal patterns
- Access to or summary of existing content inventory and top-performing historical pieces

## Process

1. **Review client context**: Pull all relevant information from juma-client-context including business objectives, target personas, brand voice guidelines, active channels, and approval workflows. Identify the primary goal the content calendar must serve (lead generation, brand awareness, thought leadership, SEO growth, nurture, etc.).

2. **Identify pillar topics**: Define 3-5 core content pillars directly tied to business goals and audience pain points. Each pillar should represent a broad theme that can sustain multiple pieces of content across formats. Validate pillars against SEO keyword clusters to ensure search demand exists. Example: a B2B SaaS client might have pillars like "Data Security Best Practices," "Compliance Automation," and "IT Team Productivity."

3. **Map content types to channels**: For each pillar, determine which content formats are appropriate for each active channel. Match format to channel strength: long-form blog posts for organic search, short-form video for social, deep-dive whitepapers for email nurture, podcast episodes for thought leadership. Document the specific requirements for each format (word count, dimensions, duration, tone).

4. **Plan publishing cadence**: Establish a sustainable rhythm per channel based on team capacity and budget. Define frequency (e.g., 2 blog posts/week, 5 social posts/week, 1 email/week, 1 whitepaper/month, 2 podcast episodes/month). Build in buffer time for revisions and approvals. Ensure cadence is realistic given available resources.

5. **Align with SEO keywords**: Assign 1-2 target keywords to every content piece. Map primary and secondary keywords from the keyword strategy to specific calendar entries. Ensure keyword coverage across all pillars and that no critical keyword clusters are neglected. Track keyword-to-content mapping to avoid cannibalization.

6. **Identify seasonal and event hooks**: Overlay industry events, conferences, product launches, holidays, and seasonal trends onto the calendar. Plan content around these moments at least 4-6 weeks in advance to allow for production timelines. Flag time-sensitive content that cannot slip.

7. **Build repurposing workflows**: Design a systematic flow for extracting maximum value from each pillar content piece. Define the cascade: one pillar piece (e.g., a whitepaper or long-form guide) breaks down into a blog post series, social media snippets, email newsletter content, infographic, video script, and podcast talking points. Document who is responsible for each derivative piece and the timeline for each step.

8. **Assign resources and create the calendar**: Populate the calendar with specific dates, topics, channels, content types, assigned owners (writer, designer, reviewer, approver), target keywords, and status tracking. Include the full production timeline for each piece (draft due, review due, design due, publish date). Set up performance tracking metrics per content piece (target traffic, engagement, conversions).

## Output Format

```
# Content Calendar: [Client Name]

**Period:** [Month/Quarter and Year]
**Prepared by:** [Strategist Name]
**Date:** [Date]
**Version:** [Version Number]

---

## Content Strategy Summary

### Business Objectives
[2-3 sentences on what the content program is designed to achieve this period. Tie directly to client business goals.]

### Target Audience
| Segment | Description | Primary Channels | Content Preferences |
|---|---|---|---|
| [Persona 1] | [Brief description] | [Channels they use] | [Formats they prefer] |
| [Persona 2] | [Brief description] | [Channels they use] | [Formats they prefer] |

---

## Content Pillars

### Pillar 1: [Pillar Name]
**Business goal alignment:** [Which objective this serves]
**Keyword cluster:** [Primary keywords in this theme]
**Content ratio:** [% of total content dedicated to this pillar]
**Description:** [2-3 sentences on what this pillar covers and why it matters to the audience]

### Pillar 2: [Pillar Name]
**Business goal alignment:** [Which objective this serves]
**Keyword cluster:** [Primary keywords in this theme]
**Content ratio:** [% of total content dedicated to this pillar]
**Description:** [2-3 sentences]

### Pillar 3: [Pillar Name]
**Business goal alignment:** [Which objective this serves]
**Keyword cluster:** [Primary keywords in this theme]
**Content ratio:** [% of total content dedicated to this pillar]
**Description:** [2-3 sentences]

[Add Pillars 4-5 if applicable]

---

## Publishing Cadence

| Channel | Format | Frequency | Pillar Mix | Primary Metric |
|---|---|---|---|---|
| Blog | Long-form articles (1,200-2,000 words) | [X per week/month] | [Pillar distribution] | [Organic sessions, time on page] |
| Social - [Platform] | [Format: carousels, reels, text posts] | [X per week] | [Pillar distribution] | [Engagement rate, reach] |
| Email | Newsletter / Nurture sequences | [X per week/month] | [Pillar distribution] | [Open rate, CTR] |
| Video - [Platform] | [Format: short-form, long-form] | [X per month] | [Pillar distribution] | [Views, watch time] |
| Podcast | Episodes ([Duration]) | [X per month] | [Pillar distribution] | [Downloads, listens] |
| Whitepapers / Guides | Gated long-form ([Word count]) | [X per quarter] | [Pillar distribution] | [Downloads, leads generated] |

---

## Repurposing Workflows

### Pillar Content Cascade
**Source piece:** [e.g., Quarterly Whitepaper or Long-Form Guide]

| Step | Derivative Content | Channel | Owner | Timeline from Source Publish |
|---|---|---|---|---|
| 1 | [e.g., Blog post series (3 posts extracted from guide)] | Blog | [Writer] | [Week 1-2] |
| 2 | [e.g., Social snippet series (10 posts with key stats/quotes)] | Social | [Social Manager] | [Week 1-3] |
| 3 | [e.g., Email series (3 emails summarizing key sections)] | Email | [Email Specialist] | [Week 1-2] |
| 4 | [e.g., Infographic summarizing main findings] | Social / Blog | [Designer] | [Week 2] |
| 5 | [e.g., Video script (2-3 min explainer)] | YouTube / Social | [Video Producer] | [Week 2-3] |
| 6 | [e.g., Podcast episode discussion points] | Podcast | [Host / Producer] | [Week 3-4] |

---

## Seasonal and Event Hooks

| Date / Window | Event / Hook | Content Planned | Channel(s) | Status |
|---|---|---|---|---|
| [Date] | [Industry event, holiday, product launch] | [Content piece title/concept] | [Target channels] | [Planned / In Progress / Complete] |
| [Date] | [Event / Hook] | [Content piece] | [Channels] | [Status] |

---

## Editorial Calendar

### Week of [Date]

| Publish Date | Content Title | Pillar | Channel | Format | Target Keyword | Writer | Designer | Reviewer | Approver | Status | Performance Target |
|---|---|---|---|---|---|---|---|---|---|---|---|
| [Date] | [Title] | [Pillar #] | [Channel] | [Format] | [Keyword] | [Name] | [Name] | [Name] | [Name] | [Draft / Review / Approved / Scheduled / Published] | [Target metric and value] |
| [Date] | [Title] | [Pillar #] | [Channel] | [Format] | [Keyword] | [Name] | [Name] | [Name] | [Name] | [Status] | [Target] |

### Week of [Date]

| Publish Date | Content Title | Pillar | Channel | Format | Target Keyword | Writer | Designer | Reviewer | Approver | Status | Performance Target |
|---|---|---|---|---|---|---|---|---|---|---|---|
| [Date] | [Title] | [Pillar #] | [Channel] | [Format] | [Keyword] | [Name] | [Name] | [Name] | [Name] | [Status] | [Target] |

[Repeat for each week in the calendar period]

---

## SEO Keyword Map

| Target Keyword | Search Volume | Difficulty | Assigned Content | Publish Date | Pillar |
|---|---|---|---|---|---|
| [Keyword] | [Volume] | [Difficulty score] | [Content title] | [Date] | [Pillar #] |
| [Keyword] | [Volume] | [Difficulty score] | [Content title] | [Date] | [Pillar #] |

---

## Resource Requirements

| Role | Name / Team | Weekly Hours Allocated | Responsibilities |
|---|---|---|---|
| Content Strategist | [Name] | [Hours] | Editorial direction, pillar planning, keyword alignment |
| Writer(s) | [Names] | [Hours] | Drafting blog posts, whitepapers, email copy, scripts |
| Designer | [Name] | [Hours] | Social graphics, infographics, email templates, video thumbnails |
| Social Media Manager | [Name] | [Hours] | Scheduling, community engagement, social copy adaptation |
| Reviewer / Editor | [Name] | [Hours] | Quality assurance, brand voice consistency, fact-checking |
| Client Approver | [Name] | [Hours] | Final sign-off on content before publish |

---

## Distribution Plan

| Content Type | Owned Channels | Paid Amplification | Partner / Earned | Timing |
|---|---|---|---|---|
| [Blog posts] | [Website, email newsletter] | [Social boost budget: $X] | [Guest syndication, PR] | [Publish day + distribution schedule] |
| [Whitepapers] | [Landing page, email nurture] | [LinkedIn Sponsored, Google Ads] | [Industry publications] | [Launch + ongoing promotion] |
| [Videos] | [YouTube, website] | [YouTube Ads, social boost] | [Embed partners] | [Publish + social clips schedule] |

---

## Performance Tracking

| Metric | Baseline | Monthly Target | Tracking Tool | Review Cadence |
|---|---|---|---|---|
| Organic blog sessions | [Current] | [Target] | [GA4 / Search Console] | [Weekly] |
| Social engagement rate | [Current] | [Target] | [Platform analytics / Sprout] | [Weekly] |
| Email open rate | [Current] | [Target] | [ESP] | [Per send] |
| Email click-through rate | [Current] | [Target] | [ESP] | [Per send] |
| Content-attributed leads | [Current] | [Target] | [CRM / GA4] | [Monthly] |
| Keyword rankings improved | [Current count] | [Target count] | [SEMrush / Ahrefs] | [Monthly] |
```

## Common Mistakes

- **Too many pillars**: More than 5 pillars dilutes focus and confuses the audience. If everything is a priority, nothing is. Force-rank and cut to 3-5 pillars that directly serve business goals.
- **Unsustainable cadence**: Planning for 5 blog posts a week when the team can realistically produce 2 leads to missed deadlines, burnout, and declining quality. Always validate cadence against actual team capacity before committing.
- **No repurposing plan**: Creating every piece of content from scratch is the most expensive way to run a content program. Every pillar piece should spawn at least 5-8 derivative assets across channels.
- **Keyword stuffing the calendar**: Assigning keywords without considering search intent leads to content that ranks but does not convert. Match keyword intent (informational, navigational, commercial, transactional) to the content format and funnel stage.
- **Ignoring the approval bottleneck**: Client review cycles are the most common cause of missed publish dates. Build approval time into every deadline and identify backup approvers for when primary contacts are unavailable.
- **Static calendar**: A content calendar is a living document. Build in a monthly review cadence to adjust based on performance data, trending topics, and shifting business priorities. A calendar that never changes is a calendar that is not being managed.
- **No distribution plan**: Publishing content without a distribution strategy means relying entirely on organic discovery. Every piece needs a plan for how it reaches the target audience beyond just hitting "publish."
- **Missing performance targets**: Without a target metric per content piece, there is no way to evaluate what is working. Every calendar entry should have a specific, measurable goal attached.

## Related Skills

- **juma-client-context**: Foundation for audience, brand voice, and business objectives that drive the calendar
- **juma-seo-strategy**: Provides the keyword research and clustering that informs pillar topics and content assignments
- **juma-paid-media-plan**: Coordinates paid amplification budget for content distribution
- **juma-ab-test-plan**: Test content variations (headlines, formats, CTAs) to optimize performance
- **juma-analytics-setup**: Ensures tracking is in place to measure content performance against targets
- **juma-campaign-brief**: Detailed briefs for individual content pieces identified in the calendar
