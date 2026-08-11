# Options basics

Before credit spreads make sense, you need four ideas: what a call and a put are, what you pay or receive for them, what “long” and “short” mean, and why Spruce prefers **spreads** over naked short options.

!!! danger "Not financial advice"
    Educational material only. Read your broker’s options risk disclosure before trading.

## The one-sentence picture

An option is a contract. A **call** is the right to **buy** a stock at a set price (the **strike**) by a set date (**expiration**). A **put** is the right to **sell** at the strike by expiration.

You can **buy** that right (you pay a **premium**) or **sell** that right (you collect a premium — and take on an obligation).

## Long vs short, without jargon

| Role | Cash at open | Everyday analogy | Risk shape |
|------|--------------|------------------|------------|
| **Long** (you buy the option) | You pay | Buying insurance or a ticket | Loss usually capped at what you paid |
| **Short** (you sell / write the option) | You receive | Selling insurance | Risk depends on whether you hedged |

Spruce’s income path is about **collecting premium** — but only when a second option **caps** how bad things can get. That structure is a **credit spread**.

!!! tip "Why not sell a naked call?"
    An uncovered (naked) short call can lose a theoretically **unlimited** amount if the stock keeps rising. Broker and OCC disclosures call this out clearly. `[verified]` Spruce treats naked shorts as education-only, not an operating default.

## Premium, strike, expiration

- **Premium** — the market price of the option. On a spread, you care about the **net** credit (what you received minus what you paid for the long leg).  
- **Strike** — the price baked into the contract.  
- **Expiration** — when the contract ends. Many U.S. equity options are American-style, so early exercise (and assignment on shorts) is possible.

One standard equity option usually covers **100 shares**, so a \$1.00 option price is about \$100 of cash per contract (before fees).

## Intrinsic value and time value

Think of premium as two pieces:

- **Intrinsic** — value if you exercised right now (only in-the-money options have this).  
- **Time value (extrinsic)** — the rest. It tends to shrink as expiration approaches, all else equal. That decay is related to **theta**, covered next in [Greeks](greeks-enough-to-operate.md).

Credit spreads mainly harvest **time value**, as long as the stock stays away from the danger zone of your short strike.

## From single options to a spread

A **vertical credit spread** means:

1. You **sell** one option.  
2. You **buy** another option of the same type and expiration, further out of the money.  
3. The long option is your insurance. It turns an open-ended short into a **defined** max loss.

That is the whole engine behind put credit spreads (PCS) and call credit spreads (CCS). The next page walks through the math and the shape of the payoff.

## What to do next

Continue to [Credit-spread payoffs](payoff-diagrams-credit-spreads.md). If a word feels fuzzy, open the [glossary](glossary.md) in another tab.

## Sources

- OCC *Characteristics and Risks of Standardized Options*  
- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
