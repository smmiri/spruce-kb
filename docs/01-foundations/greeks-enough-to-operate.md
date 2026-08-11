# Greeks enough to operate

Only what you need to pick strikes, judge time, and avoid Greek theater.

!!! danger "Not financial advice"
    Educational material only. Greeks are model-dependent approximations.

## Delta (primary)

**Delta** answers two operator questions:

1. Roughly how much the option’s price moves if the underlying moves $1.  
2. A **rough heuristic** for the chance the option finishes ITM — **not** a guarantee. `[verified]` as a widely taught approximation (true probabilities depend on the return distribution and model).

`[verified]` as common short-premium heuristic: many education sources discuss selling roughly in the **0.15–0.30** absolute-delta band (lower delta → higher chance OTM / less premium; higher delta → more premium / tested more often).

Lock your own short/long delta (or % OTM) bands in a written policy. A common long-wing starting idea is further OTM than the short (sometimes discussed near ~0.10 absolute delta); treat the **exact** numbers as `[operator preference]` — liquidity and width matter more than a magic delta.

## Theta (secondary)

Short premium generally **benefits from time decay** if the short strike stays safe. Spreads still have a long leg whose theta partially offsets. Do not assume “theta always pays you” once the short is threatened.

Near expiry, **gamma** rises for ATM options — short-dated (weekly) shorts can move against you faster. That supports Spruce’s monthly-bias *preference*, not a ban on weeklies.

## IV (enough)

Higher **implied volatility** usually means richer premiums and wider expected moves. Selling into rich IV can look attractive; it can also mean the market prices a larger move.

Into scheduled events (especially **earnings**), IV often rises beforehand and can **crush** afterward if uncertainty resolves — but a gap through your short strike can dominate any vega benefit. `[verified]` as common event-vol behavior; strategy around earnings remains policy (see risk page).

## What you can ignore for now

- Full gamma scalping theory  
- Vega portfolios and vol surface modeling  
- Rho  

## Operator checklist

- [ ] Short strike chosen with an explicit delta (or % OTM) rationale  
- [ ] Long strike defines width and max loss you accept  
- [ ] Expiry chosen with weekly-vs-monthly policy in mind  
- [ ] No naked short “because delta looked fine”  

## Sources

- [tastylive — Delta as probability gauge](https://www.tastylive.com/news-insights/options-delta-predictive-probability-gauge-directional-measure)  
- [tastylive — IV crush](https://www.tastylive.com/concepts-strategies/iv-crush)  
- [Sources index](../00-meta/sources.md)  

## Next

- [Weekly vs monthly expirations](expirations-weekly-monthly.md)  
- [Defined-risk credit spreads](../03-strategies/defined-risk-credit-spreads.md)  

---

*Footer: Not financial advice. Verify broker rules yourself.*
