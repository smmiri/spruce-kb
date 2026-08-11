# Call credit spread playbook

A practical walk-through of the **call credit spread** (bear call spread): useful when you do not want unlimited upside risk, but you still want to collect a credit.

!!! danger "Not financial advice"
    Educational draft only — not a recommendation to trade any symbol or size.

## When this trade matches your story

You collect a credit when your thesis is: *the stock should stay below my short call*. Often that is a name that already looks extended, expensive, or unlikely to keep ripping higher in the near term — still a thesis you must write down, not a vibe.

If you need the stock to rise, this is the wrong tool. Consider [PCS](put-credit-spread-playbook.md) or no trade.

!!! tip "Why a spread instead of a naked short call?"
    A naked short call can lose a theoretically unlimited amount if the stock keeps climbing. `[verified]` The long call in a CCS is the cap.

## Structure (quick refresh)

- Sell call at \(K_s\)  
- Buy call at higher strike \(K_h\)  
- Max profit \(\approx C\)  
- Max loss \(\approx W - C\) where \(W = K_h - K_s\)  

Charts: [Credit-spread payoffs](../01-foundations/payoff-diagrams-credit-spreads.md).

## From idea to order — seven steps

### 1. Thesis

Why will price not melt up through the short call? Journal it.

### 2. Liquidity

Same bar as PCS — skip option chains you cannot exit cleanly.

### 3. Expiration

Monthly bias; weeklies only with tighter size.

### 4. Strikes

Short call in a delta band you already chose (common teaching range ~0.15–0.30 absolute delta). `[verified]` as heuristic. Long call sets width and max loss.

### 5. Size

Use max loss and portfolio heat — not “percent of the account sitting in premium.” Policy numbers live on the [risk page](../04-portfolio-and-risk/risk-policy.md).

### 6. Events

Respect the earnings / event blackout in your policy.

### 7. Journal

Include why you chose CCS rather than PCS (or why both appear on different names).

## If the trade goes wrong

Same honest menu as PCS: close, roll, or hold under rules you wrote when calm. Strong trends can run farther than a small credit “feels like” it should allow.

## Anti-patterns

- Naked short call because “I almost sold a spread”  
- Many correlated CCS positions that are really one big tech bet  
- Ignoring that a squeeze can tag your short strike quickly

## What to do next

[Risk policy proposal](../04-portfolio-and-risk/risk-policy.md) · [Defined-risk overview](defined-risk-credit-spreads.md)

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- OCC / broker disclosures on uncovered call writing  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
