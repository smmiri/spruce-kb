# Greeks enough to operate

Greeks describe how an option’s price tends to move. You need only a few for day-to-day decisions.

!!! danger "Not financial advice"
    Greeks are model-based estimates — guides, not guarantees.

## Delta

**Delta** estimates how much the option price moves if the stock moves \$1, and is often used as a rough “chance of finishing in the money” heuristic. `[verified]` as a widely taught approximation.

- Long calls have positive delta; long puts have negative delta.  
- Short options flip the sign of your exposure.  
- Traders often describe strikes as “20-delta” or “30-delta.” Many education sources discuss short-premium strikes roughly in the **0.15–0.30** absolute band. `[verified]` as a common heuristic range — your exact band is `[operator preference]`.

Delta helps you **choose strikes**. It does not replace a risk category (sizing, spreads, coverage).

## Theta

**Theta** is time decay. Long options usually pay for time; short options may benefit from time if the stock cooperates. Near expiration, prices near the money can move sharply — one reason people match expiration to how often they can review ([weekly vs monthly](expirations-weekly-monthly.md)).

## Implied volatility

**IV** is the movement the market is pricing. Higher IV often means richer premiums and larger expected swings. Into **earnings**, IV often rises and can fall after the print — while the stock can still **gap** through your strikes. `[verified]` as common event behavior.

## What to skip for now

Deep gamma scalping, vol-surface modeling, and rho.

## Habit

Before any trade — long, short, or multi-leg — be able to say:

1. What is my delta / directional exposure in plain language?  
2. What is my max loss in dollars?  
3. Does an event (earnings) sit inside my window?

## What to do next

[Weekly vs monthly](expirations-weekly-monthly.md) → [Ways to manage risk](../04-portfolio-and-risk/risk-management-categories.md).

## Sources

- [tastylive — Delta as a probability gauge](https://www.tastylive.com/news-insights/options-delta-predictive-probability-gauge-directional-measure)  
- [tastylive — IV crush](https://www.tastylive.com/concepts-strategies/iv-crush)  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
