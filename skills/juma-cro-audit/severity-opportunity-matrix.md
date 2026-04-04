# Severity x Opportunity Prioritization Matrix

Use this matrix to prioritize every CRO finding based on two independent dimensions: how severe the problem is (Severity) and how much improvement is possible (Opportunity). The intersection determines the priority level.

---

## The Matrix

| | **High Opportunity** | **Medium Opportunity** | **Low Opportunity** |
|---|---|---|---|
| **High Severity** | FIX FIRST (P1) | FIX SOON (P2) | SCHEDULE (P3) |
| **Medium Severity** | FIX SOON (P2) | SCHEDULE (P3) | BACKLOG (P4) |
| **Low Severity** | SCHEDULE (P3) | BACKLOG (P4) | BACKLOG (P4) |

## Visual Layout

```
              HIGH OPPORTUNITY    MEDIUM OPPORTUNITY    LOW OPPORTUNITY

HIGH          [Finding IDs]       [Finding IDs]         [Finding IDs]
SEVERITY      FIX FIRST (P1)     FIX SOON (P2)         SCHEDULE (P3)

MEDIUM        [Finding IDs]       [Finding IDs]         [Finding IDs]
SEVERITY      FIX SOON (P2)      SCHEDULE (P3)          BACKLOG (P4)

LOW           [Finding IDs]       [Finding IDs]         [Finding IDs]
SEVERITY      SCHEDULE (P3)      BACKLOG (P4)           BACKLOG (P4)
```

---

## Severity Rating Guide

**How bad is the current problem?**

| Rating | Definition | Evidence Examples |
|--------|-----------|------------------|
| **High** | Directly causing measurable conversion loss. Significant portion of users affected. Clear evidence in analytics or heatmaps. | High bounce rate, funnel drop-off spike, heatmap dead zones over CTAs, form abandonment data |
| **Medium** | Contributing to conversion friction but not a primary blocker. Moderate user impact. | Below-average page engagement, inconsistent conversion rates, qualitative friction signals |
| **Low** | Minor issue. Affects a small percentage of users or has marginal impact on conversion behavior. | Cosmetic issues, edge-case scenarios, minor UX inconsistencies |

---

## Opportunity Rating Guide

**How much improvement is possible?**

| Rating | Definition | Sizing Criteria |
|--------|-----------|----------------|
| **High** | Fixing this could produce a measurable lift (10%+ improvement on the affected metric). Large traffic volume amplifies the impact. | High-traffic page, fundamental conversion element (CTA, form, value prop), clear best-practice gap |
| **Medium** | Expected lift of 3-10% on the affected metric. Moderate traffic volume. | Medium-traffic page, supporting conversion element, moderate best-practice gap |
| **Low** | Expected lift of 1-3%. Low traffic volume or niche impact. | Low-traffic page, peripheral element, minor optimization |

---

## Priority Level Definitions

| Priority | Action | Timeline | Scope |
|----------|--------|----------|-------|
| **P1 - Fix First** | Highest-leverage changes. Address immediately. | Sprint 1: Days 1-30 | Include in the 30-day test roadmap |
| **P2 - Fix Soon** | Significant improvements. Schedule promptly. | Sprint 2: Days 31-60 | Include in the 60-day test roadmap |
| **P3 - Schedule** | Meaningful but not urgent. Plan into the roadmap. | Sprint 3: Days 61-90 | Include in the 90-day test roadmap |
| **P4 - Backlog** | Low-priority improvements. Track for future sprints. | Beyond 90 days | Document but do not schedule yet |

---

## How to Use

1. **Rate each finding independently** on Severity and Opportunity -- do not let one dimension influence the other
2. **Plot findings on the matrix** using their finding IDs (A1, B2, C3, etc.)
3. **Determine priority** from the matrix intersection
4. **Sequence P1 items first** in the test roadmap, then P2, then P3
5. **Present the populated matrix** to the client to visually explain prioritization logic
