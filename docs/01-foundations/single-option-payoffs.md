# Single-option payoffs

Four pictures. One idea each. No spreads yet — just what happens to P&amp;L if you hold to expiration (fees ignored).

!!! danger "Not financial advice"
    Educational material only. Early assignment and fees change real outcomes.

## Shared setup for the examples

Imagine stock **XYZ** is near \$100. One contract = 100 shares. Premiums below are per share; multiply by 100 for dollars per contract.

---

## 1. Long call — you paid for upside

You buy the \$100 call for \$3.00 (\$300 per contract).

\[
\text{Max loss} = \text{premium paid} = \$3
\]

\[
\text{Breakeven} = \text{strike} + \text{premium} = \$103
\]

\[
\text{Max profit} = \text{unlimited in theory as the stock rises}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Long call payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="140" x2="490" y2="140" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,170 220,170 280,140 470,40"/>
    <text x="40" y="174" text-anchor="end" font-size="11" fill="currentColor">−prem</text>
    <text x="40" y="144" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="220" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="280" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Long call at expiration</text>
  </svg>
</figure>

**Win example:** stock finishes \$110 → call worth \$10 → profit ≈ \$7/share (\$700).  
**Loss example:** stock finishes \$95 → call expires worthless → lose the \$300 premium.

---

## 2. Long put — you paid for downside

You buy the \$100 put for \$2.50 (\$250).

\[
\text{Max loss} = \text{premium paid}
\]

\[
\text{Breakeven} = \text{strike} - \text{premium} = \$97.50
\]

\[
\text{Max profit} \approx \text{strike} - \text{premium (if stock goes to zero)}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Long put payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="140" x2="490" y2="140" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,40 200,140 260,170 470,170"/>
    <text x="40" y="174" text-anchor="end" font-size="11" fill="currentColor">−prem</text>
    <text x="40" y="144" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="200" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="260" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Long put at expiration</text>
  </svg>
</figure>

**Win example:** stock finishes \$85 → put worth \$15 → profit ≈ \$12.50/share.  
**Loss example:** stock finishes \$105 → put worthless → lose \$250.

---

## 3. Short call — you collected premium (naked)

You sell the \$100 call for \$3.00 and do **not** own the shares.

\[
\text{Max profit} = \text{premium received} = \$3
\]

\[
\text{Breakeven} = \$103
\]

\[
\text{Max loss} = \text{theoretically unlimited if the stock rises}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Short call naked payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="100" x2="490" y2="100" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,70 220,70 280,100 470,200"/>
    <text x="40" y="74" text-anchor="end" font-size="11" fill="currentColor">+prem</text>
    <text x="40" y="104" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="220" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="280" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Naked short call at expiration</text>
  </svg>
</figure>

**Win example:** stock finishes \$90 → call expires worthless → keep \$300.  
**Loss example:** stock finishes \$130 → short call loses about \$27/share before counting the \$3 credit → about \$2,400 per contract. The stock can go higher still. `[verified]` unlimited upside risk for uncovered calls.

---

## 4. Short put — you collected premium (naked / not cash-secured yet)

You sell the \$100 put for \$2.50.

\[
\text{Max profit} = \text{premium received}
\]

\[
\text{Breakeven} = \$97.50
\]

\[
\text{Max loss} \approx \text{strike} - \text{premium (if stock → 0)}
\]

<figure markdown="span">
  <svg viewBox="0 0 520 240" width="100%" role="img" aria-label="Short put payoff">
    <line x1="50" y1="20" x2="50" y2="200" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="50" y1="100" x2="490" y2="100" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="70,200 200,100 260,70 470,70"/>
    <text x="40" y="74" text-anchor="end" font-size="11" fill="currentColor">+prem</text>
    <text x="40" y="104" text-anchor="end" font-size="11" fill="currentColor">0</text>
    <text x="200" y="220" text-anchor="middle" font-size="11" fill="currentColor">BE</text>
    <text x="260" y="220" text-anchor="middle" font-size="11" fill="currentColor">K</text>
    <text x="460" y="220" text-anchor="middle" font-size="11" fill="currentColor">price →</text>
    <text x="270" y="16" text-anchor="middle" font-size="13" fill="currentColor">Short put at expiration</text>
  </svg>
</figure>

**Win example:** stock finishes \$110 → put worthless → keep \$250.  
**Loss example:** stock finishes \$70 → loss ≈ \$27.50/share (\$2,750) after the credit.

---

## What these four teach

1. Buyers have **limited** loss (the premium) and need a move.  
2. Naked sellers have **limited** gain (the premium) and can face **much larger** losses.  
3. That is not a bug in the formula — it is the deal you accept when you sell insurance without a hedge.

The next big topic is not “pick a credit spread.” It is: **what categories of risk management exist**, and how their win/loss profiles compare on the same stock story.

Continue to [Greeks](greeks-enough-to-operate.md), then [Ways to manage risk](../04-portfolio-and-risk/risk-management-categories.md).

## Sources

- OCC *Characteristics and Risks of Standardized Options*  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
