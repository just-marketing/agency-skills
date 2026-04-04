# Campaign Architecture Template

Structure campaigns using platform best practices with consistent naming conventions and a clear hierarchy.

## Campaign Hierarchy

```
Account
└── Campaign (objective + budget level)
    └── Ad Set / Ad Group (audience + placement level)
        └── Ad (creative + copy level)
```

## Naming Convention

**Campaign level:** `[Client]_[Objective]_[Audience]_[Date]`

Examples:
- `Acme_Conversion_Retargeting_2025-Q2`
- `Acme_Awareness_Lookalike-TopCustomers_2025-04`
- `Acme_LeadGen_B2B-ITManagers_2025-Q2`

**Ad Set / Ad Group level:** `[Audience Segment]_[Placement]_[Geo]`

Examples:
- `Lookalike-Purchasers_Feed-Stories_US`
- `Retargeting-CartAbandoners_AllPlacements_US`

**Ad level:** `[Format]_[Creative Concept]_[Version]`

Examples:
- `Video_Testimonial-CEO_V1`
- `Carousel_ProductFeatures_V2`
- `StaticImage_PainPoint-Security_V1`

## Architecture Decisions

For each platform, define:

| Element | Decision | Notes |
|---------|----------|-------|
| **Number of campaigns** | By objective, audience, or funnel stage | [Rationale] |
| **Ad sets/groups per campaign** | By audience segment, placement, or geography | [Rationale] |
| **Ads per ad set** | 3-5 variations for testing | [Creative plan] |
| **Ad rotation** | Optimize for conversions vs even distribution | [Strategy] |

## Example Architecture

```
Acme Corp Google Ads Account
├── Campaign: Acme_Search_Brand_2025-Q2 (Budget: $50/day)
│   └── Ad Group: Brand-Terms_US
│       ├── Ad: RSA_BrandMessage_V1
│       └── Ad: RSA_BrandMessage_V2
├── Campaign: Acme_Search_NonBrand_2025-Q2 (Budget: $200/day)
│   ├── Ad Group: DataSecurity-Keywords_US
│   │   ├── Ad: RSA_SecurityPitch_V1
│   │   ├── Ad: RSA_SecurityPitch_V2
│   │   └── Ad: RSA_SecurityPitch_V3
│   └── Ad Group: ComplianceAutomation-Keywords_US
│       ├── Ad: RSA_CompliancePitch_V1
│       └── Ad: RSA_CompliancePitch_V2
└── Campaign: Acme_Display_Retargeting_2025-Q2 (Budget: $75/day)
    ├── Ad Set: SiteVisitors-30Day_AllPlacements
    │   ├── Ad: ResponsiveDisplay_Testimonial_V1
    │   └── Ad: ResponsiveDisplay_ProductDemo_V1
    └── Ad Set: CartAbandoners-7Day_AllPlacements
        ├── Ad: ResponsiveDisplay_Discount_V1
        └── Ad: ResponsiveDisplay_Urgency_V1
```
