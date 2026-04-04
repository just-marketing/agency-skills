# Sample Size Reference Table

Use this table to estimate the required sample size per variant for A/B tests. All figures assume 95% statistical significance (alpha = 0.05) and 80% statistical power (beta = 0.20).

## Quick Reference: Sample Size Per Variant

| Baseline Rate | MDE (Relative) | Sample Size Per Variant |
|---------------|----------------|------------------------|
| 1% | 20% | ~160,000 |
| 2% | 20% | ~78,000 |
| 5% | 20% | ~30,000 |
| 10% | 20% | ~14,000 |
| 20% | 20% | ~6,000 |
| 5% | 10% | ~120,000 |
| 10% | 10% | ~57,000 |

## How to Use This Table

1. **Identify your baseline conversion rate**: The current rate for the metric you are testing (e.g., form completion rate is 5%).
2. **Choose your Minimum Detectable Effect (MDE)**: The smallest improvement worth detecting. Typically 10-20% relative. A 20% relative MDE on a 5% baseline means you want to detect a change from 5.0% to 6.0%.
3. **Look up the required sample size per variant**: This is the number of visitors needed in EACH variant (control and treatment).
4. **Calculate test duration**: `(Sample size per variant x Number of variants) / Daily traffic to the test page`

## Test Duration Calculation

**Formula:**
```
Test duration (days) = (Sample size per variant x Number of variants) / Daily traffic
```

**Example:**
- Baseline rate: 5%
- MDE: 20% relative
- Sample size per variant: ~30,000
- Number of variants: 2 (control + 1 treatment)
- Daily traffic to test page: 2,000 visitors/day
- Test duration: (30,000 x 2) / 2,000 = **30 days**

## Important Rules

- **Minimum test duration**: Always run for at least 1 full business cycle (typically 1-2 weeks) regardless of sample size, to account for day-of-week effects.
- **Do not stop early**: Peeking at results and stopping when they "look good" inflates false positive rates. Wait for the full sample size.
- **Multivariate tests (MVT)**: Multiply the sample size requirement by the number of combinations. MVT requires significantly more traffic than simple A/B tests.
- **Multiple variants**: If testing A vs B vs C, you need the sample size per variant for each of the 3 variants, tripling total traffic needs compared to a simple 2-variant test.

## When Sample Size Is Too Large

If the required sample size makes the test impractical (test would take months):
1. **Increase the MDE**: Accept that you can only detect larger effects
2. **Test a bigger change**: Subtle changes need large samples; bold changes are detectable sooner
3. **Test on a higher-traffic page**: Move the test to a page with more visitors
4. **Reduce the number of variants**: Fewer variants = less total traffic needed
5. **Reconsider whether to test**: If the test would take 6+ months, the opportunity cost may not be worth it
