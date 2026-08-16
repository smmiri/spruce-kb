# Worked example — put credit spread (anonymized)

Fictional XYZ. This is **ladder step 3** — after you can journal long options and (if used) covered calls without confusion.

!!! danger "Not financial advice"
    Not a recommendation. Width is chosen so max loss stays under a 2% equity cap.

## Setup

- XYZ at **$50**  
- Sell the **45** put, buy the **40** put, same monthly expiry (~30–45 DTE)  
- Width \(W = 5\) → $500 per contract before credit  
- Credit **$0.80** ($80)  
- Max profit **$80**  
- Max loss \(500 - 80 = 420\) per contract  

If 2% of equity is your cap, **one** contract fits only if \(420 \le 0.02 \times \text{equity}\). Heat after fill must still be ≤ 12% of equity, and this name ≤ 5%.

## Thesis (example)

“I do not think XYZ closes below 45 by this expiry because … Support is at … I will not hold into expiration week (21 DTE default).”

## Short delta

Education material often discusses short premium in a **~15–30** delta band `[verified]` as a common heuristic. Pick a strike in that band only if width still respects max loss. `[operator preference]`

## Management

Default from the operator trial: **close or roll around 21 DTE**. A roll is a *new* trade: re-check 2% / 12% / 5%.

## Anti-pattern in this example

Two contracts would be **$840** max loss. That is fine only if it still ≤ 2% *and* heat/name caps. “The credit looks nice” is not a size rule.

See also the [PCS playbook](../03-strategies/put-credit-spread-playbook.md) and [credit-spread payoffs](../01-foundations/payoff-diagrams-credit-spreads.md).

---

*Not financial advice.*
