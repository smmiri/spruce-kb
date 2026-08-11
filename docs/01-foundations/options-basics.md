# Options basics

Operator-level primer so credit-spread playbooks make sense. Not a full textbook.

!!! danger "Not financial advice"
    Educational material only. Read the OCC options disclosure before trading.

## Why options show up in Spruce

Options let you express a view with **defined structures** (spreads) where max loss is knowable at entry. Spruce starts with **selling premium inside defined-risk spreads**, not naked short options.

Uncovered (naked) short calls can have theoretically **unlimited** loss (`[verified]` — OCC / broker risk disclosures). That is why Spruce bans them for live ops.

## Calls and puts (one sentence each)

- **Call:** right to **buy** the underlying at the strike (American-style equity options: typically any time before expiry, subject to contract specs).  
- **Put:** right to **sell** the underlying at the strike.  

Long options: you pay premium; loss is typically limited to premium paid. Short options: you receive premium; risk depends on whether the short is naked or hedged (spread / covered).

## Long vs short (mindset)

| Side | You | Typical goal in Spruce context |
|------|-----|--------------------------------|
| Long option | Pay debit | Directional / insurance (not the focus of these pages) |
| Short option | Collect credit | Income / probability — **only inside defined-risk** for ops |

Spruce **restricts** live premium-selling to defined-risk credit spreads until policy explicitly unlocks other structures.

## Premium, strikes, expiration

- **Premium** is the market price of the option (or net credit of a spread).  
- **Strike** is the contract’s reference price.  
- **Expiration** ends the contract; American-style equity options may be exercised early (assignment risk on shorts still matters inside spreads).

## Intrinsic vs time value (enough)

- **Intrinsic:** ITM value if exercised now.  
- **Extrinsic / time value:** remainder of premium; decays as expiry approaches (all else equal) — related to **theta**.

Credit spreads collect net extrinsic; management decisions often hinge on how much credit remains vs how threatened the short strike is.

## Multi-leg = structure

A **credit spread** (vertical) pairs a short option with a further-OTM long option so the long caps loss. That is the foundation of PCS and CCS playbooks. Payoff math is `[verified]` on the [payoffs page](payoff-diagrams-credit-spreads.md).

## Sources

- OCC *Characteristics and Risks of Standardized Options*  
- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [Sources index](../00-meta/sources.md)  

## Next

- [Payoff diagrams for credit spreads](payoff-diagrams-credit-spreads.md)  
- [Greeks enough to operate](greeks-enough-to-operate.md)  

---

*Footer: Not financial advice. Verify broker rules yourself.*
