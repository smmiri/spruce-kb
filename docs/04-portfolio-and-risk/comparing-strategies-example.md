# Compare strategies with one example

Same stock. Same story. Different structures. The point is to **see** how wins and losses change — not to crown a winner.

!!! danger "Not financial advice"
    Hypothetical numbers for education. Fees, dividends, and early assignment ignored. Not a recommendation.

## The shared story

Stock **XYZ** trades at **\$100**.

You will look at two endings a few weeks later:

| Ending | Stock price | Story |
|--------|-------------|--------|
| **Up case** | \$110 | Quiet grind higher |
| **Down case** | \$88 | Sharp selloff |

We compare **one contract** where options appear (100-share multiplier). Share examples use **100 shares** so dollars line up.

Approximate option prices used in the story (illustrative, not live quotes):

| Contract | Premium (per share) |
|----------|---------------------|
| \$100 call | \$3.00 |
| \$100 put | \$2.50 |
| \$95 put (further OTM) | \$1.00 |
| \$105 call (further OTM) | \$1.20 |

---

## Approach A — Buy 100 shares

Capital tied up ≈ \$10,000.

| Ending | P&amp;L |
|--------|---------|
| Up to \$110 | **+\$1,000** |
| Down to \$88 | **−\$1,200** |

Risk is large relative to a small options premium. Reward is one-for-one with the stock.

---

## Approach B — Long \$100 call (pay \$3)

Cost ≈ \$300. Max loss = \$300. Unlimited upside in theory.

| Ending | Approximate P&amp;L |
|--------|---------------------|
| Up to \$110 | Call worth ≈ \$10 → **+\$700** |
| Down to \$88 | Call worthless → **−\$300** |

Compared with shares: less capital, capped loss, needs a move to win big.

---

## Approach C — Naked short \$100 call (collect \$3)

Max profit = \$300. Loss grows as the stock rises. `[verified]` unlimited for uncovered calls.

| Ending | Approximate P&amp;L |
|--------|---------------------|
| Up to \$110 | Short call loses ≈ \$7/share after credit → **−\$700** |
| Down to \$88 | Call expires worthless → **+\$300** |

You “win” the quiet down/flat path — and get hurt when the stock rips. Risk management category: this is **undefined** upside risk unless you add coverage.

---

## Approach D — Covered call (100 shares + short \$100 call at \$3)

You own the shares and sell the call.

| Ending | Approximate P&amp;L vs \$100 entry |
|--------|-----------------------------------|
| Up to \$110 | Shares +\$1,000, call −\$700 net of \$300 credit → **about +\$600** (upside capped) |
| Down to \$88 | Shares −\$1,200, call +\$300 → **about −\$900** |

Category: **collateral / coverage**. You improved the down case vs naked shares a little (kept the call premium) and capped the up case.

---

## Approach E — Cash-secured put (short \$100 put, hold \$10,000 cash)

Collect \$2.50 (\$250). Prepared to buy shares at \$100.

| Ending | Approximate P&amp;L |
|--------|---------------------|
| Up to \$110 | Put expires → **+\$250** |
| Down to \$88 | Effective buy near \$97.50; unrealized mark roughly **−\$1,000-ish** vs that basis (you now own risk like a shareholder) |

Category: **collateral**. Win is limited to the premium; loss looks like stock ownership if assigned.

---

## Approach F — Put credit spread (defined-risk sell)

Sell \$100 put for \$2.50, buy \$95 put for \$1.00 → **net credit \$1.50** (\$150).

\[
W = 5,\quad C = 1.50,\quad \text{max profit} = \$150,\quad \text{max loss} = \$(5 - 1.50)\times 100 = \$350
\]

| Ending | Approximate P&amp;L |
|--------|---------------------|
| Up to \$110 | Both puts OTM → keep credit → **+\$150** |
| Down to \$88 | Through the spread → near max loss → **about −\$350** |

### Why max loss is bigger than max profit here

That is normal for many **credit** spreads. You are selling a higher-probability outcome for a **limited** reward. The long put is insurance: it stops the naked-put disaster, but insurance costs premium, so the leftover credit is smaller than the width.

This is a **feature of the structure**, not a broken example. If you want a structure where the **best case can exceed the cash you risked**, look at debit spreads next.

---

## Approach G — Call debit spread (defined-risk buy)

Buy \$100 call for \$3.00, sell \$105 call for \$1.20 → **net debit \$1.80** (\$180).

\[
W = 5,\quad D = 1.80,\quad \text{max loss} = \$180,\quad \text{max profit} = \$(5 - 1.80)\times 100 = \$320
\]

| Ending | Approximate P&amp;L |
|--------|---------------------|
| Up to \$110 | Spread worth about \$5 → **about +\$320** |
| Down to \$88 | Spread worthless → **−\$180** |

Here **max profit (\$320) is larger than max loss (\$180)**. You paid for a directional ticket with a ceiling. You need the stock to move; time decay works against you more than in a credit spread that stays safe.

---

## Side-by-side snapshot

| Approach | Up to \$110 | Down to \$88 | Max loss known? | Max gain vs max loss feel |
|----------|-------------|--------------|-----------------|---------------------------|
| 100 shares | +\$1,000 | −\$1,200 | No hard cap (stock → 0) | Symmetric with stock |
| Long call | +\$700 | −\$300 | Yes (\$300) | Gain can exceed premium |
| Naked short call | −\$700 | +\$300 | No (upside) | Gain capped; loss can dwarf credit |
| Covered call | ~+\$600 | ~−\$900 | Stock risk remains | Upside capped |
| Cash-secured put | +\$250 | Stock-like loss if assigned | Large if crash | Gain capped at premium |
| Put **credit** spread | +\$150 | ~−\$350 | Yes (\$350) | Often **loss &gt; gain** by design |
| Call **debit** spread | ~+\$320 | −\$180 | Yes (\$180) | Often **gain &gt; debit** if right |

## What to take away

1. Learn options **mechanics** first (previous pages).  
2. Risk management is a **menu**: sizing, coverage, defined structures, portfolio caps, event filters.  
3. Credit spreads are one **defined-risk** item on that menu — attractive when you want a known max loss and are willing to accept limited reward.  
4. Debit spreads flip the risk/reward *shape*; they are not “better,” just different.  
5. Spruce’s later operating bias toward credit spreads is a **policy choice** for computable risk — not a claim that every trader must start there.

## What to do next

- [Credit-spread payoffs](../01-foundations/payoff-diagrams-credit-spreads.md) — deeper math now that you have context  
- [Defined-risk credit spreads](../03-strategies/defined-risk-credit-spreads.md) — why Spruce prioritizes them for ops  
- [Risk policy proposal](risk-policy.md) — portfolio-level numbers  

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- OCC uncovered-writing risk themes  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
