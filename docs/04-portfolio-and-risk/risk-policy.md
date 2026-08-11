# Risk policy proposal

Starter controls for a defined-risk credit-spread process. Numbers mix **common retail guidance** (tagged) with **curriculum proposals** you should adapt — not locked law and **not financial advice**.

!!! danger "Not financial advice"
    You must set and accept your own limits. This page does not tell you what you can afford to lose.

## Principles

1. Size and heat off **defined max loss**, not notional. `[verified]` as standard for spreads.  
2. **Undefined risk and naked shorts banned** for live ops until explicit unlock. Naked short call loss is theoretically unlimited (`[verified]` — OCC / broker disclosures).  
3. Prefer prevention (quality setups, event filters) over heroic mid-disaster management.  
4. Emotional sizing (“start small and experiment”) is **process advice**, not a substitute for the table below.

## Starter control table

| Control | Starter default | Notes from cross-check | Suggested enforcement |
|---------|-----------------|------------------------|------------------------|
| Max loss per trade | **User-set hard cap** (currency and/or % equity) | Retail guidance commonly cites ~**1–2% of equity** per trade as a starting band `[verified]` as common guidance | Hard block |
| Portfolio heat | Sum of open defined max losses ≤ **20%** of equity | Common conservative writeups often cite ~**10–15%** aggregate max-loss; **20% is toward aggressive** → `[operator preference]` | Hard block new entries |
| Single underlying concentration | Max loss to one underlying ≤ **10%** equity | Independent sizing notes often use tighter single-name caps (~3–8%); **10% is loose** → `[operator preference]` | Hard block |
| Single sector concentration | ≤ **25%** of heat in one sector | Common bands ~15–25%; curriculum default at top of band `[operator preference]` | Warn → optional hard |
| Undefined risk | **Banned** | Aligns with OCC uncovered-writing risk warnings | Hard block |
| Naked short options | **Banned** (education only) | Same | Hard block |
| Earnings | No new short premium within **N** trading days of earnings (starter **N = 5**) | Gap risk + IV dynamics `[verified]`; sitting out is common; **exact N** is `[operator preference]` | Hard block (override = audited) |
| Weekly vs monthly | Prefer monthly; weeklies with tighter size | Gamma rises near expiry — supports preference, not a ban | Warn |
| Correlated ETF doubles | Flag SPY/QQQ/mega-cap overlap | Correlation ≠ diversification `[verified]` as concept | Warn |
| Max open positions | Soft cap (e.g. 8–12) for cognitive load | `[operator preference]` | Warn |
| Kill-switch | Global halt: no new risk-taking; alerts only | Process design | Manual |

## Heat definition (draft)

\[
\text{heat} = \frac{\sum \text{open defined max losses}}{\text{equity}}
\]

Hypothetical fills for candidates should be included when checking “after this trade.”

## Adapting the numbers

If you want numbers closer to common conservative retail bands:

- Per-trade: start from **1–2% equity** (or a fixed currency floor that is ≤ that %)  
- Heat: consider **10–15%**, single-name **≤5–8%**, sector **≤15–20%** — then consciously choose looser/tighter  

## What this page is not

- A promise these percentages are optimal  
- Permission to ignore broker margin or buying-power limits  
- Tax or TFSA advice — see Canadian pages  

## Write your own limits

- [ ] Max loss per trade: _______________  
- [ ] Heat / underlying / sector caps: _______________  
- [ ] Earnings window N days: _______________  
- [ ] Soft max open positions: _______________  

## Sources

- Retail position-sizing / portfolio-heat writeups (common 1–2% per trade; ~10–15% heat bands) — see [Sources](../00-meta/sources.md)  
- OCC *Characteristics and Risks of Standardized Options* (uncovered writing)  
- Event-vol / IV-crush explainers (e.g. tastylive)  

## Related

- [Cash vs margin](../05-canadian-accounts/cash-vs-margin.md)  

---

*Footer: Not financial advice. Verify broker and CRA rules yourself.*
