# Defined-risk credit spreads

By now you have seen options mechanics, risk categories, and a side-by-side dollar comparison. This page explains **why Spruce’s operating path prioritizes credit spreads** — not why they are the only strategy that exists.

!!! danger "Not financial advice"
    Priority for a personal operating system is not a recommendation that everyone should sell premium.

## Where credit spreads sit on the map

From [Ways to manage risk](../04-portfolio-and-risk/risk-management-categories.md):

- They are a **spread** (one option hedges another).  
- Risk is **defined** (max loss ≈ width − credit).  
- They usually offer **limited reward** and often **max loss &gt; max profit** — a probability-oriented shape, not a lottery ticket.

Other valid tools on the same map: sizing alone, covered calls, cash-secured puts, debit spreads, protective puts, portfolio heat caps.

## Why an operating system likes them

For batch review and later automation, a structure helps when:

1. Max loss is knowable at entry.  
2. Naked unlimited upside risk is avoided.  
3. Heat across the book can be summed.

Put credit spreads (PCS) and call credit spreads (CCS) meet those constraints. That is an **engineering preference** for Spruce ops — after education, not instead of education.

## Two workhorse structures

| View | Structure | Story |
|------|-----------|-------|
| Stock should stay above the short put | PCS / bull put | Collect credit; crash risk capped by long put |
| Stock should stay below the short call | CCS / bear call | Collect credit; melt-up risk capped by long call |

Payoff math: [Credit-spread payoffs](../01-foundations/payoff-diagrams-credit-spreads.md).  
Fair comparison with other approaches: [Compare strategies](../04-portfolio-and-risk/comparing-strategies-example.md).

## Process sketch

1. Thesis  
2. Expiration  
3. Strikes → max loss → risk policy  
4. Enter or skip  
5. Journal  
6. Manage with rules written calmly  

## Canadian note

Multi-leg spreads often need higher options approval and a margin account. See [TFSA constraints](../05-canadian-accounts/tfsa-options-constraints.md).

## Playbooks

- [Put credit spread playbook](put-credit-spread-playbook.md)  
- [Call credit spread playbook](call-credit-spread-playbook.md)  
- [Risk policy proposal](../04-portfolio-and-risk/risk-policy.md)  

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
