# GTM Container Template

Standard Google Tag Manager container structure and folder organization for agency client implementations.

## Container Structure

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

## Naming Conventions

### Tags: `[Platform]_[Type]_[Detail]`
| Prefix | Platform |
|--------|----------|
| `GA4` | Google Analytics 4 |
| `Meta` | Meta (Facebook/Instagram) Pixel |
| `Google_Ads` | Google Ads |
| `LinkedIn` | LinkedIn Insight Tag |
| `TikTok` | TikTok Pixel |
| `MS_Ads` | Microsoft Ads |

### Triggers: `[Type]_[Detail]`
| Type Prefix | Trigger Type |
|-------------|-------------|
| `Click` | Click-based triggers |
| `FormSubmission` | Form submission triggers |
| `PageView` | Page view triggers |
| `Scroll` | Scroll depth triggers |
| `Timer` | Time-based triggers |
| `CustomEvent` | Custom event / dataLayer triggers |

### Variables: `[Type]_[Detail]`
| Type Prefix | Variable Type |
|-------------|--------------|
| `DLV` | Data Layer Variable |
| `CSS` | CSS Selector |
| `URL` | URL-based variable |
| `Const` | Constant value |
| `JS` | Custom JavaScript |
| `Lookup` | Lookup Table |

## Folder Organization

Organize tags, triggers, and variables into folders by platform:

```
Folders
├── GA4 (all GA4 config and event tags)
├── Meta (pixel base + event tags)
├── Google Ads (conversion + remarketing tags)
├── LinkedIn (insight tag + event tags)
├── TikTok (pixel + event tags)
└── Utilities (consent mode, error handling, helpers)
```

## Best Practices

- Use folders to organize by platform
- Version control with clear descriptions on every publish
- Use the naming convention consistently -- no exceptions
- Test in Preview mode before publishing any changes
- Document every tag's purpose in the tag notes field
- Keep unused tags paused, not deleted (for audit trail)
- Limit container access to team members who need it
- Review and clean up the container quarterly
