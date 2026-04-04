# Sample Size Reference Table

Use this table to quickly estimate the required sample size per variant for A/B tests. All figures assume 95% statistical significance (alpha = 0.05) and 80% statistical power (beta = 0.20).

## Quick Reference

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

### Inputs Required

1. **Baseline conversion rate**: The current rate for the metric being tested (e.g., form completion rate is 5%)
2. **Minimum Detectable Effect (MDE)**: The smallest improvement worth detecting, expressed as a relative percentage (e.g., 20% relative improvement means detecting a change from 5% to 6%)
3. **Number of variants**: Control + 1 or more treatments

### Calculating Test Duration

```
Test duration = (Sample size per variant x Number of variants) / Daily traffic to the test page
```

**Example:** Baseline rate is 5%, you want to detect a 20% relative improvement, and you have 2 variants (control + treatment):
- Required sample: ~30,000 per variant = ~60,000 total
- If the test page gets 1,000 visitors/day: 60,000 / 1,000 = **60 days**

### Minimum Test Duration

Always run a test for at least **1 full business cycle** (typically 1-2 weeks) regardless of sample size. This accounts for day-of-week effects that could skew results.

### Key Considerations

- **Lower baseline rates require much larger samples**: A 1% conversion rate needs 5x more traffic than a 5% rate to detect the same relative change
- **Smaller MDE requires more traffic**: Detecting a 10% improvement needs ~4x more traffic than detecting a 20% improvement
- **Multivariate tests multiply the requirement**: Each additional variant increases total sample size proportionally
- **Be realistic about MDE**: Hoping to detect a 2% relative improvement with 500 visitors/day means a test lasting months -- set MDE at 10-20% relative for practical test durations
