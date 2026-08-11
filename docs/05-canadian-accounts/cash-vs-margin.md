# Cash vs margin

How collateral and buying power interact with defined-risk spreads — still not advice.

!!! danger "Not financial advice"
    Margin magnifies losses and can trigger forced liquidation. Confirm terms with your broker.

## Cash account (concept)

- You generally fund positions with settled cash.  
- Cash-secured puts require setting aside cash for assignment (where allowed).  
- Spreads may still be restricted depending on broker approval — **ask**.

## Margin account (concept)

- Broker extends buying power subject to margin rules.  
- Defined-risk spreads often use less BP than naked shorts — still not “free.”  
- Max loss of the structure ≠ margin requirement (they can differ).

## Canadian broker cross-check

| Observation | Implication | Tag |
|-------------|-------------|-----|
| IBC: **no margin** in TFSA | Cannot rely on margin-style multi-leg in TFSA | `[verified]` (IBC page) |
| Questrade: **spreads = Level 3**, require margin; registered capped at Level 2 | CCS/PCS live process → **margin / non-registered** first | `[verified]` (Questrade page) |
| Naked shorts need higher approval / more BP | Aligns with curriculum ban for live ops | `[verified]` as industry pattern |

## Curriculum operating preference (draft)

| Preference | Rationale | Status |
|------------|-----------|--------|
| Live CCS/PCS process on **non-registered margin** first | Matches how Canadian brokers typically gate multi-leg | Proposed default |
| TFSA = narrow allowlist profile | IBC/Questrade docs support narrow TFSA options set | Proposed |
| Never circumvent broker risk controls via API | Compliance / fail-closed | Assumed |

## Link to risk policy

Portfolio **heat** is an equity-relative self-limit. Broker BP is a separate ceiling. Both must pass.

## Sources

- [IBC TFSA permissions](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php)  
- [Questrade options levels](https://www.questrade.com/learning/using-questrade/options-levels)  
- [Sources index](../00-meta/sources.md)  

## Related

- [Risk policy proposal](../04-portfolio-and-risk/risk-policy.md)  
- [IBKR Canada notes](ibkr-canada-notes.md)  
- [TFSA constraints](tfsa-options-constraints.md)  

---

*Footer: Not financial advice. Verify broker rules yourself.*
