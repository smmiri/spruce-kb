# Risk policy proposal

Rules beat improvisation. This page is a **starter template** for defined-risk credit spreads: common retail guidance mixed with curriculum defaults you should adapt.

!!! danger "Not financial advice"
    Only you can decide what you can afford to lose. These numbers are not advice and not optimal by law of nature.

## Principles in plain language

1. Measure risk as **max loss**, not as the stock’s share price.  
2. Ban **naked / undefined** short options for live use until you explicitly unlock them. Naked short calls can lose without a structural ceiling. `[verified]`  
3. Prefer skipping a bad entry over “fixing” a disaster mid-flight.  
4. Start smaller than your ego wants. That is process advice, not a substitute for the table below.

## Starter controls

| Control | Starter default | What independent guidance often says | How to treat it |
|---------|-----------------|--------------------------------------|-----------------|
| Max loss per trade | You must set a hard cap (cash and/or % of equity) | Teaching material often cites ~**1–2% of equity** per trade `[verified]` as common guidance | Make it personal and write it down |
| Portfolio heat | Sum of open max losses ≤ **20%** of equity | Conservative writeups often sit nearer **10–15%**; 20% is looser `[operator preference]` | Adapt deliberately |
| One underlying | Max loss to one name ≤ **10%** equity | Many guides use tighter single-name caps `[operator preference]` | Adapt deliberately |
| One sector | ≤ **25%** of heat in one sector | Common discussion band ~15–25% `[operator preference]` | Warn or hard-block |
| Undefined / naked risk | Banned | Aligns with OCC-style uncovered writing warnings | Hard ban |
| Earnings window | No new short premium inside **N** days (starter **N = 5**) | Gap + IV behavior `[verified]`; exact N is preference | Hard block unless audited override |
| Weeklies | Prefer monthlies; weeklies smaller | Gamma rises near expiry | Soft preference |
| Too many positions | Soft cap (for example 8–12) | Cognitive load for part-time operators | Soft cap |
| Kill switch | Stop new risk-taking; alerts only | Process design | Manual |

### Heat, as a formula

\[
\text{heat} = \frac{\text{sum of open defined max losses}}{\text{account equity}}
\]

When you size a **new** trade, include its max loss in the sum *as if* it already filled.

## A gentler starting point

If 20% heat feels aggressive, try this trial band first:

- About **1–2%** equity max loss per trade  
- About **10–15%** total heat  
- About **5–8%** in one underlying  
- About **15–20%** of heat in one sector  

Then loosen or tighten on purpose — not by accident after a hot streak.

## Write your own numbers

Capture them somewhere private you will actually obey:

| Decision | Your number |
|----------|-------------|
| Max loss per trade | |
| Max portfolio heat | |
| Max loss per underlying | |
| Max heat per sector | |
| Earnings blackout (trading days) | |
| Soft max open positions | |

## What to do next

If you are in Canada, read [IBKR notes](../05-canadian-accounts/ibkr-canada-notes.md), [TFSA constraints](../05-canadian-accounts/tfsa-options-constraints.md), and [cash vs margin](../05-canadian-accounts/cash-vs-margin.md) before you assume a strategy is allowed where you fund it.

## Sources

- Retail position-sizing discussions (1–2% per trade; heat bands) — see [Sources](../00-meta/sources.md)  
- OCC *Characteristics and Risks of Standardized Options*  
- Event-vol explainers (for example tastylive on IV crush)  

---

*Not financial advice. Verify broker and CRA rules yourself.*
