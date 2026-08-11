# How to use this site

Spruce KB is a curriculum you read in order — not a signal feed.

!!! danger "Not financial advice"
    Educational material only. Verify broker and CRA rules yourself.

## Suggested reading order

1. [Disclaimer](disclaimer.md)  
2. [Glossary](../01-foundations/glossary.md)  
3. Foundations: [options basics](../01-foundations/options-basics.md) → [payoffs](../01-foundations/payoff-diagrams-credit-spreads.md) → [Greeks enough](../01-foundations/greeks-enough-to-operate.md) → [weekly vs monthly](../01-foundations/expirations-weekly-monthly.md)  
4. Strategies: [defined-risk overview](../03-strategies/defined-risk-credit-spreads.md) → [PCS playbook](../03-strategies/put-credit-spread-playbook.md) → [CCS playbook](../03-strategies/call-credit-spread-playbook.md)  
5. [Risk policy proposal](../04-portfolio-and-risk/risk-policy.md)  
6. Canadian: [IBKR notes](../05-canadian-accounts/ibkr-canada-notes.md) → [TFSA constraints](../05-canadian-accounts/tfsa-options-constraints.md) → [cash vs margin](../05-canadian-accounts/cash-vs-margin.md)  
7. Optional: [Sources](sources.md)  

## Claim tags

| Tag | Meaning |
|-----|---------|
| `[verified]` | Consistent with ≥2 independent sources or a primary broker/regulator page (see [Sources](sources.md)) |
| `[operator preference]` | A documented operating choice for this curriculum, not a market law |
| `[pending-verify]` | Still needs stronger primary-source backup |

## Local preview

```bash
pip install -r requirements.txt
# Full local site (includes private operator docs):
mkdocs serve
# Public deploy preview:
mkdocs serve -f mkdocs.public.yml
```

Open `http://127.0.0.1:8000/`.

## What this site is not

A brokerage, signal service, tax advisor, or live order system. Automation tooling (if any) is out of scope for these pages.
