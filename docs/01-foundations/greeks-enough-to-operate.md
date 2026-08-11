# Greeks enough to operate

You do not need a textbook on every Greek. For credit spreads, **delta** does most of the daily work; **theta** and **implied volatility** explain why time and events matter.

!!! danger "Not financial advice"
    Greeks are model-based estimates. They are guides, not guarantees.

## Delta — your strike dial

**Delta** answers two related questions:

1. Roughly how much the option’s price moves if the stock moves \$1.  
2. A **rough** sense of how likely the option is to finish in the money — useful, not a promise. `[verified]` as a widely taught heuristic.

When you **sell** premium, traders often talk in deltas such as “a 20-delta put” or “a 30-delta call.” Many education sources discuss short strikes in about the **0.15–0.30** absolute-delta band:

- Closer to **0.15** → usually further out of the money, less premium, tested less often.  
- Closer to **0.30** → more premium, tested more often.

Your exact band belongs in a written policy (`[operator preference]`). Liquidity and the **width** of the spread still matter more than any single magic number.

The long option in a spread is simply your insurance further out of the money. Pick it so the **max loss** (\(W - C\)) is a dollar amount you already accepted.

## Theta — why waiting can help (until it does not)

**Theta** describes time decay. If you are short premium and the stock cooperates, time often works in your favor. A spread also has a long leg, so the benefit is partial — not free money.

Near expiration, prices can move sharply around the short strike. That is one reason many people prefer **monthly** expirations for calm income processes, and size **weeklies** smaller. See [Weekly vs monthly](expirations-weekly-monthly.md).

## Implied volatility — the “how nervous is the market?” dial

**Implied volatility (IV)** is the volatility the options market is pricing in. Higher IV usually means richer premiums *and* a market that expects bigger swings.

Around **earnings**, IV often rises beforehand and can fall quickly afterward (“IV crush”). That sounds friendly to sellers — until a **gap** jumps through your short strike. `[verified]` as common event behavior. Spruce’s risk proposal therefore suggests sitting out new short premium near earnings unless you have an explicit override process.

## What you can skip for now

Deep gamma scalping, vol-surface modeling, and rho. Revisit later if you manage complex books.

## A short pre-entry habit

Before you click send at the broker, be able to say out loud:

1. My short strike’s delta (or % out of the money) is ____ because ____.  
2. My max loss in dollars is ____.  
3. My expiration choice is monthly / weekly because ____.  
4. I am **not** selling naked risk “because the delta looked fine.”

## What to do next

[Weekly vs monthly](expirations-weekly-monthly.md), then the [defined-risk overview](../03-strategies/defined-risk-credit-spreads.md).

## Sources

- [tastylive — Delta as a probability gauge](https://www.tastylive.com/news-insights/options-delta-predictive-probability-gauge-directional-measure)  
- [tastylive — IV crush](https://www.tastylive.com/concepts-strategies/iv-crush)  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
