---
name: juma-analytics-setup
description: "Use when setting up analytics for a new client, when standardizing tracking across clients, or when auditing an existing analytics implementation. Produces a GA4 configuration plan, conversion event taxonomy, UTM standards, attribution model recommendation, and dashboard specification."
---

# Analytics Setup

## Overview

Establishes the analytics infrastructure that every other agency skill depends on for data. Creates standardized, agency-wide tracking conventions that work across all clients while allowing client-specific customization. Covers GA4 configuration, conversion event taxonomy, UTM standards, attribution modeling, dashboard design, and tag management — ensuring clean, reliable data from day one.

## When to Use

- Onboarding a new client (before any audits or campaigns)
- Existing client has messy, unreliable, or incomplete analytics
- Launching a new campaign that needs tracking setup
- Client migrating from Universal Analytics or another platform
- Agency standardizing analytics practices across all accounts
- Data discrepancies are causing reporting issues

## Prerequisites

- **juma-client-context** — business model, conversion types, marketing channels, goals
- **juma-onboarding-checklist** (recommended) — analytics is part of the onboarding process

## Process

### Step 1: Audit Existing Setup

Before building, assess what exists:

1. **GA4 property**: Exists? Properly configured? Data flowing?
2. **GTM container**: Exists? Organized? Who has access?
3. **Conversion tracking**: What events are being tracked? Are they firing correctly?
4. **Cross-domain tracking**: Needed? Configured?
5. **Data integrity**: Filters, bot traffic exclusion, internal traffic exclusion
6. **Historical data**: How much useful historical data exists?
7. **Platform pixels**: Meta, Google Ads, LinkedIn, TikTok — installed and verified?

Document findings and gaps.

### Step 2: Design Event Taxonomy

Create a standardized naming convention for all events:

**Agency-wide convention:**
```
[category]_[action]_[label]
```

**Categories:**
- `form` — Form interactions
- `cta` — Button/CTA clicks
- `page` — Page-level events
- `video` — Video interactions
- `download` — File downloads
- `ecomm` — Ecommerce events
- `engage` — Engagement signals
- `account` — Account/auth events

**Examples:**
| Event Name | Category | Action | Description |
|-----------|----------|--------|-------------|
| `form_submit_contact` | form | submit | Contact form submitted |
| `form_submit_demo` | form | submit | Demo request form submitted |
| `form_start_contact` | form | start | Contact form interaction started |
| `cta_click_pricing` | cta | click | Pricing page CTA clicked |
| `page_view_pricing` | page | view | Pricing page viewed |
| `video_play_product` | video | play | Product video started |
| `video_complete_product` | video | complete | Product video watched to end |
| `download_click_whitepaper` | download | click | Whitepaper download clicked |
| `ecomm_add_to_cart` | ecomm | add_to_cart | Product added to cart |
| `ecomm_purchase` | ecomm | purchase | Purchase completed |

**Key conversion events** (mark as conversions in GA4):
- Primary: `form_submit_demo`, `ecomm_purchase`, `form_submit_contact`
- Secondary: `form_start_*`, `page_view_pricing`, `cta_click_*`

### Step 3: Configure GA4

**Property-level settings:**
1. Data retention: Set to maximum (14 months)
2. Google Signals: Enable for cross-device tracking
3. Data collection acknowledgment: Configure per client's privacy requirements
4. Internal traffic filters: Define by IP range
5. Unwanted referral exclusions: Payment processors, SSO providers
6. Cross-domain measurement: Configure if multi-domain

**Data streams:**
1. Web stream with enhanced measurement enabled
2. Review enhanced measurement settings (page views, scrolls, outbound clicks, site search, video engagement, file downloads)
3. Disable any enhanced measurement that conflicts with custom tracking

**Custom dimensions and metrics:**
| Dimension/Metric | Scope | Purpose |
|-----------------|-------|---------|
| `client_segment` | User | Audience segment identification |
| `content_type` | Event | Content categorization |
| `campaign_tier` | Event | Campaign hierarchy |
| `lead_score` | User | Lead quality indicator |

### Step 4: Set Up GTM Container

**Container structure:**
```
Tags (naming: [Platform]_[Type]_[Detail])
├── GA4_Config_Base
├── GA4_Event_FormSubmit
├── GA4_Event_CTAClick
├── GA4_Event_VideoPlay
├── Meta_Pixel_Base
├── Meta_Event_Lead
├── Google_Ads_Conversion_Lead
├── Google_Ads_Remarketing
├── LinkedIn_Insight_Base
└── LinkedIn_Event_Conversion

Triggers (naming: [Type]_[Detail])
├── Click_SubmitButton
├── Click_CTAButton
├── FormSubmission_Contact
├── FormSubmission_Demo
├── PageView_ThankYou
├── Scroll_50Percent
├── Timer_30Seconds
└── CustomEvent_VideoPlay

Variables (naming: [Type]_[Detail])
├── DLV_FormID
├── DLV_ButtonText
├── DLV_PageCategory
├── CSS_CTAButton
├── URL_QueryParameter_UTM
└── Const_GA4MeasurementID
```

**Best practices:**
- Use folders to organize by platform
- Version control with clear descriptions
- Use a naming convention consistently
- Test in Preview mode before publishing
- Document every tag's purpose

### Step 5: Define UTM Standards

**Agency-wide UTM convention:**

| Parameter | Convention | Examples |
|-----------|-----------|---------|
| `utm_source` | Platform name (lowercase) | `google`, `meta`, `linkedin`, `newsletter`, `partner-name` |
| `utm_medium` | Channel type | `cpc`, `cpm`, `paid-social`, `email`, `organic-social`, `referral` |
| `utm_campaign` | Campaign name | `spring-2025-launch`, `brand-awareness-q2`, `retargeting-cart` |
| `utm_content` | Creative/ad variant | `headline-a`, `video-testimonial`, `carousel-products` |
| `utm_term` | Keyword (search only) | `marketing+agency`, `seo+services` |

**Rules:**
- Always lowercase
- Use hyphens, not spaces or underscores
- Be consistent across all clients (the convention is the same; the values are client-specific)
- Document in a shared UTM builder spreadsheet
- Never use UTMs on internal links

### Step 6: Select Attribution Model

Recommend attribution model based on business model:

| Business Model | Recommended Model | Rationale |
|---------------|-------------------|-----------|
| Short sales cycle (ecomm) | Data-driven or last-click | Purchase decision is quick |
| Long sales cycle (B2B SaaS) | Data-driven or linear | Multiple touchpoints matter |
| Lead gen | Data-driven or position-based | First and last touch both important |
| Brand + performance mix | Data-driven | Let the algorithm weight touchpoints |

Document:
- Primary attribution model for reporting
- Secondary model for comparison/validation
- Lookback windows per channel
- Cross-device considerations

### Step 7: Design Dashboards

**Executive dashboard** (for client stakeholders):
- Overall KPIs: Sessions, conversions, conversion rate, revenue/leads, CPA/ROAS
- Trend lines: Month-over-month, year-over-year
- Goal progress: Actual vs target
- Top-level channel performance

**Channel dashboard** (for agency team):
- Per-channel deep dive: Traffic, engagement, conversion metrics
- Campaign-level performance
- Audience insights: Demographics, devices, geography
- Content performance: Top pages, landing pages, exit pages

**Campaign dashboard** (for active campaigns):
- Campaign-specific KPIs
- Budget pacing
- Creative performance
- A/B test status

For each dashboard, specify:
- Tool: Looker Studio, GA4 Explorations, or client's preferred BI tool
- Refresh cadence: Real-time, daily, weekly
- Access: Who can view, who can edit

### Step 8: Configure Alerts

Set up automated alerts for:

| Alert | Condition | Notification |
|-------|-----------|-------------|
| Traffic drop | >20% decrease vs previous period | Email to account team |
| Conversion spike/drop | >30% change in conversion rate | Email + Slack |
| Budget pacing | >110% or <80% of daily budget | Email to media team |
| 404 errors | >10 per hour | Email to SEO team |
| Goal completion | Monthly target reached | Email to account team |

### Step 9: Document Everything

Create a client-specific analytics documentation:

1. **Property and container IDs**: GA4, GTM, platform pixel IDs
2. **Event taxonomy**: Full list of custom events with descriptions
3. **Conversion events**: Which events are marked as conversions
4. **UTM convention**: Client-specific examples
5. **Dashboard locations**: URLs and access instructions
6. **Alert configurations**: What triggers what notification
7. **Access log**: Who has access to what, at what permission level
8. **Change log**: History of configuration changes

## Output Format

```markdown
# Analytics Setup: [Client Name]
**Prepared by**: [Agency Name] | **Date**: [Date]

## Setup Summary

| Component | Status | Details |
|-----------|--------|---------|
| GA4 Property | [Configured/Existing/New] | Property ID: [ID] |
| GTM Container | [Configured/Existing/New] | Container ID: [ID] |
| Conversion tracking | [N] events configured | [List key events] |
| Platform pixels | [List platforms] | [Status each] |
| UTM standards | Documented | [Link to UTM builder] |
| Dashboards | [N] created | [List with URLs] |
| Alerts | [N] configured | [List key alerts] |

## Event Taxonomy

| Event Name | Type | Description | Conversion? | Parameters |
|-----------|------|-------------|-------------|------------|
| [event_name] | [Custom/Enhanced] | [Description] | [Yes/No] | [key params] |

## Conversion Events

| Event | Type | Value | Counting |
|-------|------|-------|----------|
| [event] | [Primary/Secondary] | [$X or N/A] | [Once per session/Every] |

## UTM Standards

| Parameter | Convention | Client Examples |
|-----------|-----------|-----------------|
| utm_source | [Convention] | [Examples] |
| utm_medium | [Convention] | [Examples] |
| utm_campaign | [Convention] | [Examples] |

## GTM Container Structure

### Tags
| Tag Name | Platform | Type | Trigger | Status |
|----------|----------|------|---------|--------|
| [Name] | [Platform] | [Type] | [Trigger name] | [Active/Draft] |

### Key Triggers
| Trigger Name | Type | Conditions |
|-------------|------|------------|
| [Name] | [Type] | [Conditions] |

## Attribution Model
- **Primary model**: [Model name]
- **Rationale**: [Why this model]
- **Lookback window**: [N days click, N days view]

## Dashboards

| Dashboard | Audience | Tool | URL | Refresh |
|-----------|----------|------|-----|---------|
| Executive | Client stakeholders | [Tool] | [URL] | [Cadence] |
| Channel | Agency team | [Tool] | [URL] | [Cadence] |
| Campaign | Media team | [Tool] | [URL] | [Cadence] |

## Alerts

| Alert | Condition | Recipients | Channel |
|-------|-----------|------------|---------|
| [Alert name] | [Trigger condition] | [Who] | [Email/Slack] |

## Access Log

| Platform | Account/Property | User | Permission Level |
|----------|-----------------|------|-----------------|
| [Platform] | [Account] | [User/Email] | [Admin/Editor/Viewer] |

## Documentation & References
- Event taxonomy spreadsheet: [Link]
- UTM builder: [Link]
- GTM change log: [Link]
- Analytics playbook: [Link]
```

## Common Mistakes

- **No naming convention** — Without a standard, event names become inconsistent across clients and team members. Establish and enforce the convention
- **Over-tracking** — Tracking everything creates noise. Focus on events tied to business outcomes
- **Forgetting enhanced measurement conflicts** — GA4's built-in enhanced measurement can conflict with custom GTM tags, causing double-counting
- **No internal traffic filter** — Agency and client team visits skew data. Always filter internal traffic
- **Missing cross-domain setup** — If the client has multiple domains in the user journey (e.g., blog on subdomain, checkout on different domain), cross-domain tracking is essential
- **Skipping the documentation** — When the team member who set it up leaves, undocumented analytics becomes a black box. Document everything
- **Not testing before launch** — Always use GTM Preview mode and GA4 DebugView before publishing changes

## Related Skills

- **juma-onboarding-checklist** — Analytics setup is a key onboarding step
- **juma-reporting** — Clean analytics data enables accurate reporting
- **juma-ab-test-plan** — Testing requires proper conversion tracking
- **juma-campaign-plan** — Campaign measurement depends on analytics setup
- **juma-paid-media-plan** — Conversion tracking and attribution for paid media
- **juma-channel-audit** — Accurate channel data requires proper tracking
