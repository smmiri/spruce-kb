# Cash vs margin

Collateral and buying power are easy to confuse with “max loss.” They are related, but they are not the same number.

!!! danger "Not financial advice"
    Margin can amplify losses and trigger forced liquidation. Confirm terms with your broker.

## Cash account, in plain language

You generally pay for positions with settled cash. A cash-secured put, where allowed, means setting aside cash for assignment. Whether spreads are allowed at all still depends on your broker’s approval matrix.

## Margin account, in plain language

The broker extends buying power under margin rules. Defined-risk spreads often use less buying power than naked shorts — that does **not** mean the trade is free or small. The structure’s **max loss** and the broker’s **margin requirement** can differ.

## What Canadian broker pages imply for Spruce

| Observation | Practical implication | Tag |
|-------------|----------------------|-----|
| IBC: **no margin** inside TFSA | Do not plan margin-style multi-leg trades in TFSA by default | `[verified]` (IBC page) |
| Questrade: spreads are **Level 3** and need margin; registered accounts stop at Level 2 | Live CCS/PCS process usually means **margin / non-registered** first | `[verified]` (Questrade page) |
| Naked shorts need higher approval | Matches the curriculum ban on naked risk for live trading | Common industry pattern |

## Curriculum preference (draft)

| Preference | Why |
|------------|-----|
| Run CCS/PCS on **non-registered margin** first | Matches how Canadian brokers typically gate multi-leg spreads |
| Keep TFSA on a narrow allowlist | Matches published TFSA option lists |
| Never bypass broker risk controls via API | Fail closed |

## Heat vs buying power

[Portfolio heat](../04-portfolio-and-risk/risk-policy.md) is your own equity-relative limit. Broker buying power is a second ceiling. Both must be satisfied.

## Related reading

- [Risk policy](../04-portfolio-and-risk/risk-policy.md)  
- [Canadian brokers](canadian-brokers.md)  
- [TFSA constraints](tfsa-options-constraints.md)  
- [Sources](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
