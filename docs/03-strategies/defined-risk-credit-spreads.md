# Defined-risk credit spreads

Why Spruce starts here — and what is education-only until policy unlocks.

!!! danger "Not financial advice"
    Educational material only. Defined-risk still means you can lose the full defined max loss.

## Priority thesis

For operators who want **batch review**, not screen-watching:

1. **Know max loss at entry** — size and portfolio heat become computable. `[verified]` for vertical credit spreads: max loss ≈ width − credit.  
2. **Avoid undefined short premium** in live ops — naked shorts stay education-only. Uncovered short call risk is theoretically unlimited (`[verified]` — OCC).  
3. **Two workhorse structures:** put credit spreads (PCS / bull put) and call credit spreads (CCS / bear call). Naming `[verified]` via standard vertical-spread references.

Wheel / CSP / covered call / PMCC / iron condors appear later in a fuller curriculum; they are not the default operating set on these pages.

## Defined vs undefined

| Shape | Example | Spruce live ops |
|-------|---------|-----------------|
| Defined | PCS, CCS (vertical credit spreads with long protection) | Preferred |
| Undefined / extreme | Naked short call; many naked shorts | **Banned** until explicit policy unlock |

## When to reach for which

| Bias | Structure | Rough idea |
|------|-----------|------------|
| Constructive / “won’t break support” | PCS (bull put) | Collect credit; risk is a sharp selloff through the put spread |
| Cautious / “won’t melt-up through resistance” | CCS (bear call) | Collect credit; risk is a sharp rally through the call spread |

`[verified]` directionally: bull put is a bullish credit vertical; bear call is a bearish credit vertical ([Investopedia vertical spreads](https://www.investopedia.com/terms/v/verticalspread.asp)).

Always journal the thesis; technical/fundamental filters belong on a watchlist process you maintain separately.

## What “good process” looks like

1. Thesis on underlying and direction/range  
2. Expiry choice (monthly bias proposal)  
3. Strikes → compute max loss → check risk policy  
4. Written entry / manage / exit rules  
5. Journal outcomes  

## Canadian note

Multi-leg spreads are often gated behind higher options levels / **margin** accounts at Canadian brokers — another reason Spruce defaults live CCS/PCS discussion toward non-registered/margin (see [TFSA](../05-canadian-accounts/tfsa-options-constraints.md)).

## Playbooks

- [Put credit spread playbook](put-credit-spread-playbook.md)  
- [Call credit spread playbook](call-credit-spread-playbook.md)  
- [Risk policy proposal](../04-portfolio-and-risk/risk-policy.md)  
- [Sources](../00-meta/sources.md)  

---

*Footer: Not financial advice. Verify broker rules yourself.*
