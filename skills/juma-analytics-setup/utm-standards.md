# UTM Parameter Standards

Agency-wide UTM convention for consistent campaign tracking across all clients and platforms.

## UTM Parameter Convention

| Parameter | Convention | Examples |
|-----------|-----------|---------|
| `utm_source` | Platform name (lowercase) | `google`, `meta`, `linkedin`, `newsletter`, `partner-name` |
| `utm_medium` | Channel type | `cpc`, `cpm`, `paid-social`, `email`, `organic-social`, `referral` |
| `utm_campaign` | Campaign name | `spring-2025-launch`, `brand-awareness-q2`, `retargeting-cart` |
| `utm_content` | Creative/ad variant | `headline-a`, `video-testimonial`, `carousel-products` |
| `utm_term` | Keyword (search only) | `marketing+agency`, `seo+services` |

## Rules

1. **Always lowercase** -- never mix cases
2. **Use hyphens, not spaces or underscores** -- hyphens are URL-safe and readable
3. **Be consistent across all clients** -- the convention is the same; the values are client-specific
4. **Document in a shared UTM builder spreadsheet** -- prevents ad hoc naming that breaks reporting
5. **Never use UTMs on internal links** -- UTMs override source attribution; internal UTMs will misattribute traffic and break session data

## Common Medium Values

| Medium Value | Use For |
|-------------|---------|
| `cpc` | Paid search (Google Ads, Microsoft Ads) |
| `cpm` | Display and programmatic |
| `paid-social` | Paid social media ads (Meta, LinkedIn, TikTok) |
| `organic-social` | Organic social media posts |
| `email` | Email campaigns and newsletters |
| `referral` | Partner referrals and guest posts |
| `affiliate` | Affiliate marketing links |
| `sms` | SMS/text campaigns |

## Example UTM Strings

**Google Search Ad:**
```
?utm_source=google&utm_medium=cpc&utm_campaign=spring-2025-launch&utm_term=marketing+agency
```

**Meta Paid Social Ad:**
```
?utm_source=meta&utm_medium=paid-social&utm_campaign=retargeting-cart&utm_content=carousel-products
```

**Email Newsletter:**
```
?utm_source=newsletter&utm_medium=email&utm_campaign=weekly-digest-2025-03-15&utm_content=hero-cta
```

**LinkedIn Organic Post:**
```
?utm_source=linkedin&utm_medium=organic-social&utm_campaign=thought-leadership-q1
```
