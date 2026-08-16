# Glossary

Plain-language definitions. Skim once, then return whenever a page uses a term you do not remember.

!!! danger "Not financial advice"
    Educational definitions only.

## Building blocks

| Term | Plain meaning |
|------|----------------|
| **Call** | Contract with the right to **buy** the stock at the strike. |
| **Put** | Contract with the right to **sell** the stock at the strike. |
| **Premium** | Price of the option (or the net credit/debit of a multi-leg trade). |
| **Strike** | The price named in the contract. |
| **Expiration** | When the contract ends. |
| **ITM** | In the money — a call when stock is above the strike; a put when stock is below. |
| **OTM** | Out of the money — the opposite of ITM. |
| **ATM** | At the money — stock near the strike. |

## Spreads and risk shape

| Term | Plain meaning |
|------|----------------|
| **Credit spread** | You open a multi-leg options trade and **receive** a net credit. Usually one short option plus one long option for protection. |
| **PCS / put credit spread** | Sell a put, buy a lower put. Also called a **bull put spread**. You want the stock to stay above the short put. |
| **CCS / call credit spread** | Sell a call, buy a higher call. Also called a **bear call spread**. You want the stock to stay below the short call. |
| **Defined risk** | You know the worst-case loss from the structure at entry (before fees). |
| **Undefined risk** | Loss can grow without a clean structural cap (classic example: naked short call). |
| **Max loss** | Worst case on a defined-risk trade. Spruce sizes positions from this number. |
| **Max profit** | On a credit spread, roughly the credit you collected. |
| **Breakeven** | Stock price at expiry where P&amp;L is about zero (ignoring fees). |

## Greeks and portfolio words

| Term | Plain meaning |
|------|----------------|
| **Delta** | Sensitivity to a \$1 stock move; also a rough “chance of finishing ITM” heuristic. |
| **Theta** | Time decay. |
| **IV** | Implied volatility — how much movement the market is pricing. |
| **Buying power** | Capital your broker sets aside for the trade — not the same as max loss. |
| **Heat** | Sum of open defined max losses, compared with account equity. |
| **Roll** | Close a position and reopen related strikes/expiry to manage risk or time. |
| **CSP** | Cash-secured put — short put backed by cash for assignment. |
| **Wheel** | A cycle of cash-secured puts and covered calls. Later topic. |
| **Covered call** | Short call against shares you already own. |
| **HITL** | Human-in-the-loop — suggestions allowed; live sending needs a person. |
| **Dry-run** | Practice / prepare without sending a live order. |
| **Watchlist** | Names you **follow**. You might own $0. |
| **Portfolio / “actually bought”** | Names you spent real money on. |
| **Envelope / sleeve** | A planning bucket of cash (e.g. $24k to own shares), not a special account type. |

Payoff formulas for single options are on [Single-option payoffs](single-option-payoffs.md). Credit-spread formulas are on [Credit-spread payoffs](payoff-diagrams-credit-spreads.md). Compare structures on [Compare strategies](../04-portfolio-and-risk/comparing-strategies-example.md). Public references: [Sources](../00-meta/sources.md).
