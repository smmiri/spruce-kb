# Put credit spread playbook

A practical walk-through of the **put credit spread** (bull put spread): when it fits, how to build it, and how to think about size and trouble.

!!! danger "Not financial advice"
    Educational draft only — not a recommendation to trade any symbol or size.

## When this trade matches your story

You collect a credit when your thesis is: *the stock should stay above my short put*. You are comfortable defining a max loss if you are wrong.

If that sentence does not match your view, do not force a PCS — look at [CCS](call-credit-spread-playbook.md) or stand aside.

## Structure (quick refresh)

- Sell put at \(K_s\)  
- Buy put at lower strike \(K_l\)  
- Max profit \(\approx C\) (the credit)  
- Max loss \(\approx W - C\) where \(W = K_s - K_l\)  

Full charts and a numeric example: [Credit-spread payoffs](../01-foundations/payoff-diagrams-credit-spreads.md).

## From idea to order — seven steps

### 1. Thesis

In one or two sentences: why will price not crash through the short put? Support, quality, valuation — whatever your process uses — belongs in the journal.

### 2. Liquidity

Prefer names and option lines with reasonable volume and open interest so you are not fighting huge bid/ask spreads. Exact numeric floors are `[operator preference]`.

### 3. Expiration

Start with the monthly bias unless you have a reason for a weekly and a smaller size. See [Weekly vs monthly](../01-foundations/expirations-weekly-monthly.md).

### 4. Strikes

Common education material discusses short premium around **0.15–0.30** absolute delta. `[verified]` as a common heuristic range. Lock *your* band in writing. The long put sets width and therefore max loss.

### 5. Size

Count contracts from **max loss**, not from share price. Many retail guides start near **1–2% of equity** per trade as a teaching band. `[verified]` as common guidance — your hard cap is personal. Also check **heat** after the fill (see [risk policy](../04-portfolio-and-risk/risk-policy.md)).

### 6. Events

If earnings (or another binary event) sit inside your blackout window, skip or wait. Gaps can ignore your carefully chosen delta.

### 7. Journal

Record thesis, strikes, credit, max loss, and tags. Future-you needs that more than a perfect chart annotation.

## If the trade goes wrong

There is no magic repair kit. Typical choices:

- Close for a defined loss  
- Roll (change expiry/strikes) with eyes open on new risk  
- Hold toward expiration if that is your written policy  

Decide the *default* on a calm day, not while the stock is cascading.

## Anti-patterns

- Sizing because “the credit looks big”  
- Stacking many PCS on the same sector until one theme sinks them all  
- Treating “defined risk” as “small risk”  
- Skipping the long put “just this once”

## What to do next

[Call credit spread playbook](call-credit-spread-playbook.md) · [Risk policy](../04-portfolio-and-risk/risk-policy.md)

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
