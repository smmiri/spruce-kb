# Glossary (operator-facing)

Short definitions for reading playbooks and risk policy.

!!! danger "Not financial advice"
    Educational definitions only.

## Core structure terms

| Term | Meaning in Spruce |
|------|-------------------|
| **Call** | Option giving the right to buy the underlying at the strike before/at expiry (style depends on contract). |
| **Put** | Option giving the right to sell the underlying at the strike. |
| **Premium** | Price of the option (or net credit/debit of a multi-leg structure), paid by buyer / received by seller. |
| **Strike** | Price level in the option contract. |
| **Expiration / expiry** | Date the option ceases to exist (American vs European exercise rules vary). |
| **ITM (in the money)** | Call: underlying above strike. Put: underlying below strike. |
| **OTM (out of the money)** | Call: underlying below strike. Put: underlying above strike. |
| **ATM (at the money)** | Underlying near the strike. |

## Spreads and risk shape

| Term | Meaning in Spruce |
|------|-------------------|
| **Credit spread** | Multi-leg options structure that collects net premium (credit) when opened; typically short one option and long another for protection. |
| **PCS (put credit spread)** | Short put + long put further OTM (lower strike). Bullish-to-neutral bias; defined max loss. Also called a bull put spread. |
| **CCS (call credit spread)** | Short call + long call further OTM (higher strike). Bearish-to-neutral / “won’t rip higher” bias; defined max loss. Also called a bear call spread. |
| **Defined risk** | Maximum loss known at entry from structure (e.g. width of strikes minus credit, before fees). |
| **Undefined risk** | Loss theoretically unbounded or extremely large relative to premium (e.g. naked short call). **Banned for live Spruce ops** until policy unlock. |
| **Max loss** | Worst-case loss on a defined-risk trade (structure + fees); Spruce sizes and heat off this, not notional. |
| **Max profit** | On a credit spread, typically the net credit received (if expires worthless / managed as planned). |
| **Breakeven** | Underlying price at expiry where P&amp;L ≈ 0 (ignoring fees), given the structure. |

## Greeks and probability language

| Term | Meaning in Spruce |
|------|-------------------|
| **Delta** | Rough sensitivity of option price to a $1 move in the underlying; also a rough OTM/ITM probability heuristic. Primary strike-selection Greek for this system. |
| **Theta** | Time decay; short premium generally benefits if other factors hold. |
| **IV (implied volatility)** | Market’s priced-in volatility; affects premium rich/cheap feel. |
| **Buying power (BP)** | Capital the broker reserves for the position; not the same as max loss. |

## Portfolio and process

| Term | Meaning in Spruce |
|------|-------------------|
| **Heat** | Sum of open defined max losses relative to equity (see risk policy). |
| **Roll** | Close a position (or legs) and open a related one at a later expiry and/or different strikes. |
| **CSP (cash-secured put)** | Short put collateralized by cash sufficient for assignment; often a wheel building block. |
| **Wheel** | Cycle of CSP → possible assignment → covered call → rinse. Later curriculum. |
| **Covered call (CC)** | Short call against long shares. |
| **HITL** | Human-in-the-loop: system may suggest; human approves before execute. |
| **Dry-run** | Prepare / simulate without sending live orders. |

## Naming aliases

| Spruce term | Common textbook name |
|-------------|----------------------|
| PCS | Bull put spread / put credit vertical |
| CCS | Bear call spread / call credit vertical |

Payoff definitions for those structures are `[verified]` — see [payoffs](payoff-diagrams-credit-spreads.md) and [Sources](../00-meta/sources.md).
