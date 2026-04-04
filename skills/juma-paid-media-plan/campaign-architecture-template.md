# Campaign Architecture Template

Structure campaigns using platform best practices with consistent naming conventions and hierarchy.

## Campaign Hierarchy

```
Account
└── Campaign (objective + budget level)
    └── Ad Set / Ad Group (audience + placement level)
        └── Ad (creative + copy level)
```

## Naming Convention

**Standard format:** `[Client]_[Objective]_[Audience]_[Date]`

### Examples

| Level | Naming Pattern | Example |
|-------|---------------|---------|
| Campaign | `[Client]_[Objective]_[Audience]_[YYYY-MM]` | `Acme_LeadGen_Retargeting_2025-03` |
| Ad Set/Group | `[Audience-Segment]_[Placement]_[Geo]` | `WebVisitors-30d_Feed_US` |
| Ad | `[Format]_[Message]_[Variant]` | `Carousel_Testimonial_V2` |

## Architecture Planning Checklist

For each platform, define:

- **Number of campaigns**: Organized by objective, audience, or funnel stage
- **Ad sets/groups per campaign**: By audience segment, placement, or geography
- **Ads per ad set**: 3-5 variations for testing
- **Ad rotation setting**: Optimize for conversions vs. even distribution

## Architecture by Funnel Stage

### Awareness Campaigns
```
Campaign: [Client]_Awareness_[Audience]_[Date]
├── Ad Set: Broad-Interest_AllPlacements
│   ├── Ad: Video_BrandStory_V1
│   ├── Ad: Video_BrandStory_V2
│   └── Ad: Static_BrandAwareness_V1
└── Ad Set: Lookalike-Customers_AllPlacements
    ├── Ad: Video_BrandStory_V1
    └── Ad: Video_BrandStory_V2
```

### Consideration Campaigns
```
Campaign: [Client]_Consideration_[Audience]_[Date]
├── Ad Set: Interest-Based_Feed
│   ├── Ad: Carousel_ProductFeatures_V1
│   ├── Ad: SingleImage_CaseStudy_V1
│   └── Ad: Video_ProductDemo_V1
└── Ad Set: Engagement-Retargeting_Feed
    ├── Ad: Carousel_Testimonials_V1
    └── Ad: SingleImage_Offer_V1
```

### Conversion Campaigns
```
Campaign: [Client]_Conversion_[Audience]_[Date]
├── Ad Set: WebVisitors-30d_AllPlacements
│   ├── Ad: SingleImage_DirectCTA_V1
│   ├── Ad: SingleImage_DirectCTA_V2
│   └── Ad: Carousel_ProductBenefits_V1
└── Ad Set: CartAbandoners-7d_AllPlacements
    ├── Ad: DPA_DynamicProduct_V1
    └── Ad: SingleImage_Urgency_V1
```

## Naming Convention Rules

1. Use underscores (`_`) to separate fields
2. Use hyphens (`-`) within field values (e.g., `Cart-Abandoners`)
3. Keep names concise but descriptive
4. Use consistent date format: `YYYY-MM`
5. Version creative variants with `V1`, `V2`, etc.
6. Never use spaces in campaign names
7. Document the convention in a shared reference so all team members follow it
