# Options basics

This page is only about how options work. We will not optimize risk yet. First understand the contracts; later pages compare ways to control loss.

!!! danger "Not financial advice"
    Educational material only. Read your broker’s options risk disclosure before trading.

## What an option is

An option is a contract about a stock (or ETF) at a **strike** price by an **expiration** date.

- A **call** gives the holder the right to **buy** 100 shares (typical equity contract) at the strike.  
- A **put** gives the holder the right to **sell** 100 shares at the strike.

Someone must be on the other side. If you **buy** the option, you pay a **premium**. If you **sell** (write) the option, you receive the premium and take on an obligation if the buyer exercises.

## Four building blocks

Every options position is one of these, or a combination of them:

| Position | You… | You want… | Rough loss shape |
|----------|------|-----------|------------------|
| Long call | Pay premium | Stock up strongly | Limited to premium paid |
| Long put | Pay premium | Stock down strongly | Limited to premium paid |
| Short call | Collect premium | Stock flat or down | Can be very large if stock rips higher |
| Short put | Collect premium | Stock flat or up | Large if stock crashes (toward zero in theory) |

Later pages show how traders **pair** legs to change those loss shapes. That is risk design — not required to understand the table above.

## Premium, strike, expiration

- **Premium** — the market price of the option. Quoted per share; one contract usually multiplies by 100. A \$2.50 premium is about \$250 per contract before fees.  
- **Strike** — the contract’s reference price.  
- **Expiration** — when the contract ends. Many U.S. equity options can be exercised early (American style), so short options can be **assigned** before expiry.

## In, at, and out of the money

| Term | Call | Put |
|------|------|-----|
| **ITM** (in the money) | Stock above strike | Stock below strike |
| **ATM** (at the money) | Stock near strike | Stock near strike |
| **OTM** (out of the money) | Stock below strike | Stock above strike |

OTM options are cheaper because they need a bigger move to become valuable at expiration.

## Intrinsic value and time value

Premium has two pieces in plain language:

- **Intrinsic** — value if exercised right now (only ITM options have this).  
- **Time value** — the rest. It tends to shrink as expiration approaches if nothing else changes. That decay is related to **theta** (see [Greeks](greeks-enough-to-operate.md)).

Buyers hope the stock moves enough to overcome time decay. Sellers often hope time decay helps them — which is why selling without a plan for large adverse moves is dangerous.

## Long vs short mindset

Buying an option is paying for a defined ticket: your loss is usually capped at what you paid.

Selling an option is collecting a premium for taking on an obligation. The premium is your **maximum gain** on that single short option if it expires worthless. The loss can be much larger than the premium unless you add protection (shares, cash, or another option).

That asymmetry — small credit, larger possible loss on naked shorts — is why the next pages spend time on **payoffs** and then on **risk categories**.

## What to do next

1. [Single-option payoffs](single-option-payoffs.md) — pictures and formulas for the four building blocks  
2. [Greeks enough to operate](greeks-enough-to-operate.md)  
3. [Weekly vs monthly](expirations-weekly-monthly.md)  
4. Then [Ways to manage risk](../04-portfolio-and-risk/risk-management-categories.md) — before any playbook  

## Sources

- OCC *Characteristics and Risks of Standardized Options*  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
