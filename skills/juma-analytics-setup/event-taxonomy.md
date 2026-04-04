# Event Taxonomy

Standardized naming convention for all conversion and engagement events across client analytics implementations.

## Agency-Wide Naming Convention

```
[category]_[action]_[label]
```

## Event Categories

| Category | Purpose |
|----------|---------|
| `form` | Form interactions |
| `cta` | Button/CTA clicks |
| `page` | Page-level events |
| `video` | Video interactions |
| `download` | File downloads |
| `ecomm` | Ecommerce events |
| `engage` | Engagement signals |
| `account` | Account/auth events |

## Event Examples

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

## Key Conversion Events

Mark these as conversions in GA4:

**Primary conversions:**
- `form_submit_demo`
- `ecomm_purchase`
- `form_submit_contact`

**Secondary conversions:**
- `form_start_*` (form engagement signals)
- `page_view_pricing` (high-intent page views)
- `cta_click_*` (CTA engagement)

## Naming Rules

1. Always lowercase
2. Use underscores to separate category, action, and label
3. Keep labels short and descriptive
4. Use consistent action verbs: `submit`, `start`, `click`, `view`, `play`, `complete`, `add_to_cart`, `purchase`
5. Apply the same convention across all clients (values change, structure stays the same)
6. Document every custom event with a description in the client analytics documentation
