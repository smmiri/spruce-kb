# Defined-risk credit spreads

Spruce starts here for a reason: you can know the worst case **before** you click send, and you can add those worst cases up across the whole account.

!!! danger "Not financial advice"
    “Defined risk” still means you can lose the full defined max loss. It is not “safe.”

## The idea in one paragraph

A **credit spread** sells one option and buys another further out of the money for protection. You collect a net credit. If the stock behaves, you keep most of that credit. If it does not, your loss is capped by the width of the strikes minus the credit — see [payoffs](../01-foundations/payoff-diagrams-credit-spreads.md).

That cap is why Spruce prefers spreads over naked short calls. Uncovered short calls can lose a theoretically unlimited amount if the stock keeps rising. `[verified]`

## Two workhorse trades

| Your view | Structure | Everyday story |
|-----------|-----------|----------------|
| “I do not expect a sharp drop through my put strikes” | **Put credit spread (PCS)** / bull put | Collect credit while staying bullish-to-neutral |
| “I do not expect a sharp melt-up through my call strikes” | **Call credit spread (CCS)** / bear call | Collect credit while capping upside disaster |

Both names and payoff shapes are standard vertical-spread material. `[verified]`

Wheel strategies, cash-secured puts, and covered calls belong in a fuller curriculum later. They are not required to understand these pages.

## A calm process (before tools and automation)

1. Write a short thesis for the stock and the direction/range you need.  
2. Choose expiration (monthly bias is the starter preference).  
3. Choose strikes → compute **max loss** → check your risk policy.  
4. Enter only if size and heat still fit.  
5. Journal what you did and why.  
6. Manage with rules you wrote in advance — not improvisation under stress.

## Canadian reality check

At several Canadian brokers, multi-leg **spreads** sit behind higher options approvals and often need a **margin** account, while TFSA permissions are narrower. That is why the Canadian pages suggest confirming spreads on the account you will actually use — often non-registered/margin first. Details: [TFSA constraints](../05-canadian-accounts/tfsa-options-constraints.md).

## What to do next

Open the [PCS playbook](put-credit-spread-playbook.md), then the [CCS playbook](call-credit-spread-playbook.md). Finish with the [risk policy proposal](../04-portfolio-and-risk/risk-policy.md) so sizing has numbers.

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [Sources index](../00-meta/sources.md)  

---

*Not financial advice. Verify broker rules yourself.*
