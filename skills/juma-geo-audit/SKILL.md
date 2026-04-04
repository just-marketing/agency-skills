---
name: juma-geo-audit
description: "Use when assessing a client's visibility in AI-powered search engines and LLM outputs, when pitching GEO as a new service line, or when clients ask why they do not appear in ChatGPT, Claude, Gemini, or Perplexity responses about their industry."
---

# Generative Engine Optimization (GEO) Audit

## Overview

The GEO Audit evaluates a client's visibility, citation frequency, and content readiness for AI-powered search and large language model (LLM) outputs. As users increasingly turn to ChatGPT, Claude, Gemini, and Perplexity for product research, recommendations, and decision-making, brands that are not mentioned -- or are mentioned unfavorably -- in these responses face a growing visibility gap that traditional SEO cannot address alone.

This is a NEW service category that agencies can sell as a standalone offering ($2K-$12K/month depending on scope) or bundle with existing SEO and content retainers. The audit produces a GEO Visibility Score, a citation inventory, content optimization priorities, a competitive GEO matrix, and a phased implementation roadmap. It is designed to be both a client deliverable and a sales tool -- the findings naturally justify ongoing GEO optimization work.

**Why this matters for agencies:** AI search is shifting how buyers discover brands. Agencies that offer GEO audits position themselves as forward-thinking strategic partners, differentiate from competitors who only offer traditional SEO, and create a new recurring revenue stream. The audit itself often sells the retainer.

## When to Use

- A client asks "why don't we show up when people ask ChatGPT about [our category]?"
- Pitching GEO as a new service line to existing or prospective clients
- During onboarding to establish an AI search visibility baseline alongside traditional SEO
- When building a content strategy that needs to account for AI search citation
- Quarterly GEO health check to track changes in AI visibility
- After a competitor starts appearing prominently in LLM responses
- As a complement to a juma-seo-audit to cover both traditional and AI search
- When developing a proposal that includes GEO services

## Prerequisites

- **juma-client-context** (required) -- brand identity, product/service descriptions, target audiences, and competitive landscape
- **juma-seo-audit** (recommended) -- traditional SEO baseline provides comparison context
- **juma-competitor-intel** (recommended) -- competitor list for GEO comparison
- Access to multiple LLMs for testing: ChatGPT (GPT-4), Claude, Gemini, Perplexity (minimum)
- List of key product/service categories and use cases the client wants to be known for
- Client's current website content inventory (from SEO audit or CMS access)
- Understanding of the client's structured data implementation status

## Process

### Step 1: Design the Query Test Matrix

Build a structured set of test queries across multiple intent categories:

1. **Brand queries:** "What is [brand name]?", "Tell me about [brand name]", "[brand name] reviews"
2. **Category queries:** "Best [product/service category]", "Top [industry] companies", "Who are the leading [category] providers?"
3. **Comparison queries:** "[brand] vs [competitor]", "Compare [product category] options", "Which [category] is best for [use case]?"
4. **Problem/solution queries:** "How do I solve [problem the client addresses]?", "What's the best way to [task the client helps with]?"
5. **Recommendation queries:** "Recommend a [product/service] for [persona/use case]", "What should I look for in a [category]?"
6. **Location queries (if applicable):** "Best [category] in [city/region]", "[category] near [location]"

Create 20-40 queries minimum. Ensure they cover the client's full product/service range and all primary audience segments.

### Step 2: Test Brand Visibility Across LLMs

Run every query from the test matrix across each LLM platform:

1. **ChatGPT (GPT-4 / latest):** Record whether the brand is mentioned, in what context, what position (first mentioned, listed among others, not mentioned), and whether information is accurate
2. **Claude:** Same evaluation criteria
3. **Gemini:** Same evaluation criteria
4. **Perplexity:** Same evaluation criteria, plus note which sources are cited with links
5. **Bing Chat / Copilot:** Same evaluation criteria

For each response, document:
- Is the brand mentioned? (Yes/No)
- Position of mention (Primary recommendation, Listed among options, Brief mention, Not mentioned)
- Accuracy of information (Correct, Partially correct, Incorrect, Outdated)
- Sentiment of mention (Positive, Neutral, Negative, Mixed)
- Sources cited (if visible) -- which URLs are referenced?
- Competitor mentions in the same response

### Step 3: Analyze Citation Sources

For LLMs that show sources (Perplexity, Bing Chat, Gemini with citations):

1. Catalog every URL cited when the client's category is discussed
2. Identify which of the client's own pages get cited and for which queries
3. Identify third-party pages that mention the client (review sites, directories, publications)
4. Note which competitor pages get cited and why (content structure, authority, freshness)
5. Map citation patterns: What types of content get cited most? (listicles, data-driven articles, product pages, how-to guides, Wikipedia, industry publications)
6. Identify "citation sources" -- the trusted domains that LLMs pull from most in this category

### Step 4: Score Content Citability

Evaluate the client's website content for characteristics that make it likely to be cited by LLMs:

1. **Clear, structured answers:** Does the content provide direct, concise answers to common questions? Score: [1-10]
2. **Factual density:** Does the content include specific data points, statistics, and verifiable claims? Score: [1-10]
3. **Authority signals:** Does the content demonstrate E-E-A-T? Author bios, citations, expert quotes, original research? Score: [1-10]
4. **Structured data markup:** Is schema.org markup implemented to help machines parse the content? Score: [1-10]
5. **Content freshness:** Is the content regularly updated with current information? Score: [1-10]
6. **Unique value:** Does the content offer original insights, data, or perspectives not found elsewhere? Score: [1-10]
7. **Format accessibility:** Is the content organized with clear headings, lists, tables, and summaries that LLMs can easily extract? Score: [1-10]
8. **Topic coverage breadth:** Does the site comprehensively cover its category, or are there significant gaps? Score: [1-10]

Calculate an average Content Citability Score (1-10) across all factors.

### Step 5: Assess Structured Data and Technical Readiness

Review technical elements that influence AI content parsing:

1. **Schema.org markup:** Which schema types are implemented? Are they complete and error-free?
2. **llms.txt implementation:** Does the site have an llms.txt file? If so, is it properly formatted and comprehensive? If not, document the opportunity.
3. **robots.txt AI directives:** Are AI crawlers (GPTBot, ClaudeBot, Google-Extended, PerplexityBot) allowed or blocked?
4. **Sitemap completeness:** Can AI crawlers discover all important content?
5. **Content accessibility:** Is important content behind JavaScript rendering, login walls, or paywalls that prevent AI indexing?
6. **API/data feed availability:** Does the client offer any structured data feeds that AI systems could consume?
7. **Knowledge graph presence:** Does the client have a Google Knowledge Panel? Wikidata entry? Wikipedia page?

### Step 6: Build Competitive GEO Comparison

For each competitor identified in the test matrix:

1. Calculate their GEO Visibility Score using the same methodology
2. Count their brand mention frequency across all queries and LLMs
3. Identify which queries they dominate and why
4. Note their content citability strengths (what are they doing that gets them cited?)
5. Assess their structured data and technical GEO readiness
6. Identify where competitors are weak in AI search that the client could exploit

### Step 7: Develop the Optimization Roadmap

Based on all findings, build a phased implementation plan:

1. **Quick wins (Week 1-2):** Structured data fixes, llms.txt implementation, robots.txt updates
2. **Content optimization (Month 1-2):** Restructure existing high-value pages for citability, add FAQ sections, improve answer formatting
3. **Content creation (Month 2-4):** Create new content targeting citation gaps, develop authoritative resources for key category queries
4. **Authority building (Ongoing):** Earn mentions on citation source sites, build topical authority, pursue knowledge graph presence
5. **Monitoring and iteration (Ongoing):** Retest queries monthly to track visibility changes, adjust strategy based on LLM behavior changes

## Output Format

```markdown
# GEO Audit: [Client Name]

**Prepared by:** [Agency Name]
**Date:** [Date]
**Website:** [URL]
**LLMs Tested:** ChatGPT (GPT-4), Claude, Gemini, Perplexity, Bing Chat

---

## Executive Summary

[2-3 paragraphs summarizing the client's AI search visibility, how they compare to competitors, the most critical gaps, and the revenue opportunity. Frame findings in terms of the growing shift in buyer behavior toward AI-assisted research and decision-making.]

**Key Finding:** [Single most important insight, stated plainly]

**Revenue Opportunity:** [Estimate of traffic/leads at risk as AI search grows, or opportunity from improved visibility]

**Service Recommendation:** [Brief framing of the ongoing GEO optimization engagement this audit supports -- monthly retainer range, scope overview]

---

## GEO Visibility Score: [X/100]

| Component | Score | Weight | Weighted Score |
|-----------|-------|--------|----------------|
| Brand Mention Frequency | [X/100] | 30% | [X] |
| Citation Source Coverage | [X/100] | 25% | [X] |
| Content Citability | [X/100] | 25% | [X] |
| Technical GEO Readiness | [X/100] | 20% | [X] |
| **Overall GEO Score** | | **100%** | **[X/100]** |

---

## 1. Brand Visibility Across AI Platforms

### Overall Mention Rate

| LLM Platform | Queries Tested | Brand Mentioned | Mention Rate | Avg. Position |
|-------------|---------------|-----------------|-------------|---------------|
| ChatGPT | [X] | [X] | [X%] | [Primary/Listed/Brief/None] |
| Claude | [X] | [X] | [X%] | [Primary/Listed/Brief/None] |
| Gemini | [X] | [X] | [X%] | [Primary/Listed/Brief/None] |
| Perplexity | [X] | [X] | [X%] | [Primary/Listed/Brief/None] |
| Bing Chat | [X] | [X] | [X%] | [Primary/Listed/Brief/None] |
| **Total** | **[X]** | **[X]** | **[X%]** | |

### Visibility by Query Category

| Query Category | Total Queries | Brand Mentioned | Mention Rate | Top Competitor Mentioned |
|---------------|--------------|-----------------|-------------|------------------------|
| Brand queries | [X] | [X] | [X%] | [N/A or competitor name] |
| Category queries | [X] | [X] | [X%] | [Competitor name] |
| Comparison queries | [X] | [X] | [X%] | [Competitor name] |
| Problem/solution queries | [X] | [X] | [X%] | [Competitor name] |
| Recommendation queries | [X] | [X] | [X%] | [Competitor name] |

### Accuracy & Sentiment of Mentions

| Factor | Assessment | Details |
|--------|-----------|---------|
| Information Accuracy | [Correct/Mixed/Problematic] | [Specific inaccuracies found] |
| Brand Sentiment | [Positive/Neutral/Negative/Mixed] | [Examples of how brand is described] |
| Outdated Information | [Yes/No] | [What is outdated and where] |
| Missing Key Information | [List] | [Important facts LLMs do not know about the brand] |

---

## 2. Citation Source Analysis

### Client Pages Cited by LLMs

| Client URL | Cited By | For Which Queries | Content Type |
|-----------|----------|------------------|-------------|
| [URL 1] | [LLM names] | [Query categories] | [Blog/Product/About/etc.] |
| [URL 2] | [LLM names] | [Query categories] | [Content type] |
| [URL 3] | [LLM names] | [Query categories] | [Content type] |

### Third-Party Pages Citing the Client

| Source URL | Domain Authority | Mention Context | Cited By LLMs |
|-----------|-----------------|-----------------|---------------|
| [URL 1] | [DA] | [How client is mentioned] | [Which LLMs cite this] |
| [URL 2] | [DA] | [How client is mentioned] | [Which LLMs cite this] |

### Top Citation Sources in This Category

| Domain | Category Relevance | Cites Client | Cites Competitors | Priority to Target |
|--------|-------------------|-------------|-------------------|-------------------|
| [Domain 1] | [High/Medium] | [Yes/No] | [Which ones] | [High/Medium/Low] |
| [Domain 2] | [High/Medium] | [Yes/No] | [Which ones] | [High/Medium/Low] |
| [Domain 3] | [High/Medium] | [Yes/No] | [Which ones] | [High/Medium/Low] |

---

## 3. Content Citability Assessment

### Citability Score: [X/10]

| Factor | Score (1-10) | Assessment | Key Issues |
|--------|-------------|-----------|------------|
| Clear, structured answers | [X] | [Strong/Adequate/Weak] | [Specific issues] |
| Factual density | [X] | [Strong/Adequate/Weak] | [Specific issues] |
| Authority signals (E-E-A-T) | [X] | [Strong/Adequate/Weak] | [Specific issues] |
| Structured data markup | [X] | [Strong/Adequate/Weak] | [Specific issues] |
| Content freshness | [X] | [Strong/Adequate/Weak] | [Specific issues] |
| Unique value / original data | [X] | [Strong/Adequate/Weak] | [Specific issues] |
| Format accessibility | [X] | [Strong/Adequate/Weak] | [Specific issues] |
| Topic coverage breadth | [X] | [Strong/Adequate/Weak] | [Specific issues] |

### Content Optimization Priorities

| Page / Content Area | Current Citability | Issue | Recommended Action | Priority |
|--------------------|-------------------|-------|-------------------|----------|
| [Page/topic 1] | [Low/Medium/High] | [What is wrong] | [Specific fix] | [P1/P2/P3] |
| [Page/topic 2] | [Low/Medium/High] | [What is wrong] | [Specific fix] | [P1/P2/P3] |
| [Page/topic 3] | [Low/Medium/High] | [What is wrong] | [Specific fix] | [P1/P2/P3] |

---

## 4. Technical GEO Readiness

| Factor | Status | Details | Action Required |
|--------|--------|---------|-----------------|
| Schema.org Markup | [Complete/Partial/Missing] | [Types implemented] | [Specific additions needed] |
| llms.txt | [Implemented/Not Implemented] | [Quality assessment if present] | [Create/Update/None] |
| robots.txt AI Directives | [Allowing/Blocking AI bots] | [Specific directives found] | [Changes recommended] |
| GPTBot Access | [Allowed/Blocked/Not Configured] | | [Recommendation] |
| ClaudeBot Access | [Allowed/Blocked/Not Configured] | | [Recommendation] |
| Google-Extended Access | [Allowed/Blocked/Not Configured] | | [Recommendation] |
| PerplexityBot Access | [Allowed/Blocked/Not Configured] | | [Recommendation] |
| Knowledge Graph Presence | [Yes/Partial/No] | [Google Knowledge Panel, Wikidata] | [Steps to establish/improve] |
| Content Accessibility | [Good/Issues Found] | [JS rendering, paywalls, etc.] | [Fixes needed] |

---

## 5. Competitive GEO Matrix

| Metric | [Client] | [Comp 1] | [Comp 2] | [Comp 3] | [Comp 4] |
|--------|----------|----------|----------|----------|----------|
| **GEO Visibility Score** | [X/100] | [X/100] | [X/100] | [X/100] | [X/100] |
| **Brand Mention Rate** | [X%] | [X%] | [X%] | [X%] | [X%] |
| **Primary Mentions** | [X] | [X] | [X] | [X] | [X] |
| **Citation Count** | [X] | [X] | [X] | [X] | [X] |
| **Content Citability** | [X/10] | [X/10] | [X/10] | [X/10] | [X/10] |
| **llms.txt** | [Yes/No] | [Yes/No] | [Yes/No] | [Yes/No] | [Yes/No] |
| **Schema Completeness** | [%] | [%] | [%] | [%] | [%] |
| **Knowledge Graph** | [Yes/No] | [Yes/No] | [Yes/No] | [Yes/No] | [Yes/No] |

### Who Wins Each Query Category

| Query Category | Winner | Why They Win | Client Gap |
|---------------|--------|-------------|-----------|
| Category queries | [Competitor] | [Reason: content depth, authority, etc.] | [What client lacks] |
| Comparison queries | [Competitor] | [Reason] | [What client lacks] |
| Problem/solution queries | [Competitor] | [Reason] | [What client lacks] |
| Recommendation queries | [Competitor] | [Reason] | [What client lacks] |

---

## 6. Implementation Roadmap

### Phase 1: Foundation (Weeks 1-2)
**Focus:** Technical readiness and quick wins

- [ ] [Action 1: e.g., Implement llms.txt file] -- [Expected impact]
- [ ] [Action 2: e.g., Update robots.txt to allow AI crawlers] -- [Expected impact]
- [ ] [Action 3: e.g., Add/fix structured data markup] -- [Expected impact]
- [ ] [Action 4: e.g., Correct inaccurate brand information across web properties] -- [Expected impact]

### Phase 2: Content Optimization (Months 1-2)
**Focus:** Make existing content more citable

- [ ] [Action 1: e.g., Restructure top 10 pages with FAQ sections and clear answer formatting] -- [Expected impact]
- [ ] [Action 2: e.g., Add original data, statistics, and expert quotes to key pages] -- [Expected impact]
- [ ] [Action 3: e.g., Update outdated content with current information] -- [Expected impact]
- [ ] [Action 4: e.g., Improve E-E-A-T signals: author bios, credentials, methodology pages] -- [Expected impact]

### Phase 3: Content Creation (Months 2-4)
**Focus:** Fill citation gaps with new authoritative content

- [ ] [Action 1: e.g., Create definitive guide for [high-value category query]] -- [Expected impact]
- [ ] [Action 2: e.g., Publish original research/survey on [industry topic]] -- [Expected impact]
- [ ] [Action 3: e.g., Build comparison/vs. pages for key competitor matchups] -- [Expected impact]
- [ ] [Action 4: e.g., Develop FAQ hub covering top 50 questions in the category] -- [Expected impact]

### Phase 4: Authority Building (Ongoing)
**Focus:** Earn presence on citation source sites

- [ ] [Action 1: e.g., Pitch guest content to [top citation source domains]] -- [Expected impact]
- [ ] [Action 2: e.g., Pursue Wikipedia/Wikidata presence] -- [Expected impact]
- [ ] [Action 3: e.g., Submit to industry directories and review platforms] -- [Expected impact]
- [ ] [Action 4: e.g., Build relationships with publishers LLMs frequently cite] -- [Expected impact]

### Phase 5: Monitoring & Iteration (Monthly)
**Focus:** Track changes and adapt

- [ ] Retest full query matrix monthly across all LLMs
- [ ] Track GEO Visibility Score trend
- [ ] Monitor competitor GEO changes
- [ ] Adjust content and technical strategy based on LLM behavior updates
- [ ] Report results to client with month-over-month comparisons

---

## Service Recommendation

**Recommended Engagement:** GEO Optimization Retainer

| Tier | Monthly Investment | Scope | Best For |
|------|-------------------|-------|----------|
| **GEO Essentials** | $2,000-$4,000/mo | Monthly monitoring, technical optimization, content recommendations | Clients with strong existing content who need technical GEO readiness |
| **GEO Growth** | $5,000-$8,000/mo | Everything in Essentials + content optimization, citation building, quarterly competitive analysis | Clients who need content restructuring and active citation acquisition |
| **GEO Leadership** | $9,000-$12,000/mo | Everything in Growth + original research, authority building campaigns, weekly monitoring, dedicated GEO strategist | Clients in competitive categories who want to dominate AI search visibility |

---

## Appendix: Query Test Matrix & Raw Results

### Full Query List

| # | Query | Category | ChatGPT | Claude | Gemini | Perplexity | Bing Chat |
|---|-------|----------|---------|--------|--------|------------|-----------|
| 1 | [Query text] | [Category] | [Mentioned: Y/N, Position] | [Same] | [Same] | [Same] | [Same] |
| 2 | [Query text] | [Category] | [Result] | [Result] | [Result] | [Result] | [Result] |

### Methodology Notes
- Queries were tested on [dates] using [model versions]
- All tests were conducted without prior conversation context (new sessions)
- Results may vary based on LLM updates, user location, and conversation context
- GEO Visibility Score methodology: [Brief description of scoring formula]
- This audit represents a point-in-time snapshot; LLM outputs are non-deterministic and change over time
```

## Common Mistakes

- **Testing too few queries** -- A handful of queries does not capture the full picture. Test at least 20-40 queries across all intent categories. The more queries tested, the more reliable the visibility score.
- **Testing only on one LLM** -- Different LLMs have different training data, citation behaviors, and content preferences. Always test across at least 4 platforms to get a representative view.
- **Forgetting that LLM outputs are non-deterministic** -- The same query can produce different responses on different days or in different sessions. Run key queries multiple times and document the variance. Do not over-index on a single response.
- **Treating GEO as a replacement for SEO** -- GEO supplements traditional SEO; it does not replace it. Many LLMs cite websites that rank well in traditional search. A strong SEO foundation supports GEO visibility.
- **Ignoring the sales opportunity** -- This audit is designed to sell ongoing GEO services. If you deliver the findings without a clear service recommendation and pricing, you leave revenue on the table. Always include the service recommendation section.
- **Overlooking llms.txt** -- This is a low-effort, high-signal action that many sites have not implemented. Checking for it and recommending it is an easy quick win that demonstrates the agency's GEO expertise.
- **Presenting raw data without interpretation** -- Clients do not need to see every query response. Summarize patterns, highlight the most important gaps, and translate findings into strategic implications.
- **Not establishing a baseline for ongoing measurement** -- The first audit is a baseline. Without it, you cannot show improvement. Save all raw data and make the measurement methodology repeatable for monthly tracking.

## Related Skills

- **juma-client-context** -- provides brand identity, product descriptions, and competitive landscape for building the query test matrix
- **juma-seo-audit** -- traditional SEO health directly influences GEO visibility; these audits work as a pair
- **juma-competitor-intel** -- competitive analysis extends into the GEO comparison matrix
- **juma-content-calendar** -- GEO content creation priorities feed into the content roadmap
- **juma-channel-audit** -- AI search is an emerging channel that the channel audit should reference
- **juma-proposal** -- GEO audit findings build a compelling case for a new service engagement
- **juma-upsell-finder** -- GEO is a natural upsell for any client with an existing SEO or content retainer
- **juma-cro-audit** -- traffic from AI referrals (Perplexity, Bing Chat) may convert differently and warrants CRO attention
