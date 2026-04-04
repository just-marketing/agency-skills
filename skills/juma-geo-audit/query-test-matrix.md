# Query Test Matrix

Use this matrix to design the structured set of test queries for the GEO audit. Build 20-40 queries minimum covering the client's full product/service range and all primary audience segments.

---

## Query Categories

### 1. Brand Queries
Test whether LLMs know the brand and present accurate information.

| # | Query Template | Customization Notes |
|---|---------------|-------------------|
| 1 | "What is [brand name]?" | Direct brand knowledge |
| 2 | "Tell me about [brand name]" | Open-ended brand awareness |
| 3 | "[brand name] reviews" | Reputation and sentiment |
| 4 | "Is [brand name] good?" | Qualitative brand perception |

### 2. Category Queries
Test whether the brand appears when users search for the product/service category.

| # | Query Template | Customization Notes |
|---|---------------|-------------------|
| 1 | "Best [product/service category]" | Category leadership |
| 2 | "Top [industry] companies" | Market position |
| 3 | "Who are the leading [category] providers?" | Industry authority |
| 4 | "What are the most popular [category] options?" | Market awareness |

### 3. Comparison Queries
Test whether the brand appears in head-to-head and category comparisons.

| # | Query Template | Customization Notes |
|---|---------------|-------------------|
| 1 | "[brand] vs [competitor]" | Direct comparison (test with each key competitor) |
| 2 | "Compare [product category] options" | Category comparison |
| 3 | "Which [category] is best for [use case]?" | Use-case-driven comparison |
| 4 | "[competitor] alternatives" | Alternative discovery |

### 4. Problem/Solution Queries
Test whether the brand appears when users describe the problem the client solves.

| # | Query Template | Customization Notes |
|---|---------------|-------------------|
| 1 | "How do I solve [problem the client addresses]?" | Problem-aware stage |
| 2 | "What's the best way to [task the client helps with]?" | Task-oriented |
| 3 | "Why is [pain point] happening and how to fix it?" | Diagnostic |
| 4 | "Tools/services to help with [challenge]" | Solution-seeking |

### 5. Recommendation Queries
Test whether the brand is recommended for specific personas or use cases.

| # | Query Template | Customization Notes |
|---|---------------|-------------------|
| 1 | "Recommend a [product/service] for [persona/use case]" | Persona-matched |
| 2 | "What should I look for in a [category]?" | Evaluation criteria |
| 3 | "Best [category] for small businesses" | Segment-specific (adapt to client's segments) |
| 4 | "What [category] do experts recommend?" | Authority-driven |

### 6. Location Queries (If Applicable)
Test local/regional visibility in AI search.

| # | Query Template | Customization Notes |
|---|---------------|-------------------|
| 1 | "Best [category] in [city/region]" | Local discovery |
| 2 | "[category] near [location]" | Proximity-based |
| 3 | "Top-rated [category] in [state/country]" | Regional reputation |

---

## Response Documentation Template

For each query tested across each LLM, document:

| Field | What to Record |
|-------|---------------|
| **Brand mentioned?** | Yes / No |
| **Position of mention** | Primary recommendation / Listed among options / Brief mention / Not mentioned |
| **Accuracy** | Correct / Partially correct / Incorrect / Outdated |
| **Sentiment** | Positive / Neutral / Negative / Mixed |
| **Sources cited** | URLs referenced (if visible) |
| **Competitor mentions** | Which competitors appear in the same response |

## LLM Platforms to Test

1. **ChatGPT (GPT-4 / latest)**
2. **Claude**
3. **Gemini**
4. **Perplexity**
5. **Bing Chat / Copilot**

Run every query on each platform. Use new sessions (no prior conversation context) for consistent results.
