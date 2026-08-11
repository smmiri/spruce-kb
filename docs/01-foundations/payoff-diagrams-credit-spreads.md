# Credit-spread payoffs

You already saw that credit spreads are **one** defined-risk tool among several. This page is the math and shape for put and call credit spreads only.

!!! danger "Not financial advice"
    Fees, early assignment, and broker margin change real outcomes. Numbers ignore fees.

## Reminder: why max loss often exceeds max profit

A credit spread collects a net credit \(C\) on width \(W\). Then:

\[
\text{Max profit} \approx C
\]

\[
\text{Max loss} \approx W - C
\]

Whenever \(C &lt; W/2\), max loss is larger than max profit. That is common: you are selling a higher-probability zone for a limited paycheck, and you **paid** for the long option that caps disaster. Compare with a debit spread on [the comparison page](../04-portfolio-and-risk/comparing-strategies-example.md), where max profit can exceed the debit.

---

## Shared symbols

| Symbol | Meaning |
|--------|---------|
| \(K_s\) | Short strike |
| \(K_l\) / \(K_h\) | Long put (lower) / long call (higher) |
| \(W\) | Width between strikes |
| \(C\) | Net credit per share |

Multiply by 100 per standard equity contract.

---

## Put credit spread (bull put)

Sell put \(K_s\), buy put \(K_l\), same expiry. \(W = K_s - K_l\).

| Outcome | Formula |
|---------|---------|
| Max profit | \(C\) if stock ≥ \(K_s\) |
| Max loss | \(W - C\) if stock ≤ \(K_l\) |
| Breakeven | \(K_s - C\) |

<figure markdown="span">
  <svg viewBox="0 0 520 260" width="100%" role="img" aria-label="Put credit spread payoff">
    <line x1="60" y1="20" x2="60" y2="220" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="60" y1="120" x2="500" y2="120" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="80,200 180,200 300,120 360,50 480,50"/>
    <text x="50" y="54" text-anchor="end" font-size="12" fill="currentColor">+C</text>
    <text x="50" y="124" text-anchor="end" font-size="12" fill="currentColor">0</text>
    <text x="50" y="204" text-anchor="end" font-size="12" fill="currentColor">-(W−C)</text>
    <text x="180" y="240" text-anchor="middle" font-size="12" fill="currentColor">Kl</text>
    <text x="300" y="240" text-anchor="middle" font-size="12" fill="currentColor">BE</text>
    <text x="360" y="240" text-anchor="middle" font-size="12" fill="currentColor">Ks</text>
    <text x="480" y="240" text-anchor="middle" font-size="12" fill="currentColor">price →</text>
  </svg>
</figure>

### Example with a healthier credit (still loss &gt; profit)

Sell \$100 / buy \$95 put spread for **\$2.00** credit (\$200).

- Max profit = **\$200**  
- Max loss = **\$300**  
- Breakeven = \$98  

Up ending (stock \$110): **+\$200**. Down ending through \$95: **−\$300**.  
You improved the credit versus a skinny \$1.50 example, but the structure still pays a limited reward for a defined larger loss — by design.

---

## Call credit spread (bear call)

Sell call \(K_s\), buy call \(K_h\). \(W = K_h - K_s\). Breakeven \(K_s + C\).

<figure markdown="span">
  <svg viewBox="0 0 520 260" width="100%" role="img" aria-label="Call credit spread payoff">
    <line x1="60" y1="20" x2="60" y2="220" stroke="currentColor" stroke-opacity="0.35"/>
    <line x1="60" y1="120" x2="500" y2="120" stroke="currentColor" stroke-opacity="0.35"/>
    <polyline fill="none" stroke="#0d9488" stroke-width="3" points="80,50 200,50 260,120 380,200 480,200"/>
    <text x="50" y="54" text-anchor="end" font-size="12" fill="currentColor">+C</text>
    <text x="50" y="124" text-anchor="end" font-size="12" fill="currentColor">0</text>
    <text x="50" y="204" text-anchor="end" font-size="12" fill="currentColor">-(W−C)</text>
    <text x="200" y="240" text-anchor="middle" font-size="12" fill="currentColor">Ks</text>
    <text x="260" y="240" text-anchor="middle" font-size="12" fill="currentColor">BE</text>
    <text x="380" y="240" text-anchor="middle" font-size="12" fill="currentColor">Kh</text>
    <text x="480" y="240" text-anchor="middle" font-size="12" fill="currentColor">price →</text>
  </svg>
</figure>

### Example

Sell \$100 / buy \$105 call spread for **\$1.80** credit.

- Max profit = **\$180**  
- Max loss = **\$320**  
- Breakeven = \$101.80  

---

## Habits

1. Size from max loss \(W - C\), not share price.  
2. Defined ≠ small.  
3. Prefer this structure over a naked short when you want a known floor.  
4. If you dislike “loss larger than gain,” you may prefer debit spreads or long options for that idea — revisit the [comparison](../04-portfolio-and-risk/comparing-strategies-example.md).

## What to do next

[Defined-risk credit spreads](../03-strategies/defined-risk-credit-spreads.md) · [PCS playbook](../03-strategies/put-credit-spread-playbook.md) · [CCS playbook](../03-strategies/call-credit-spread-playbook.md)

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
