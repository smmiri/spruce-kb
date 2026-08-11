# How to use this site

Spruce is a short course. Resist the urge to jump straight to credit-spread playbooks. Those pages assume you already understand options and the risk menu.

!!! danger "Not financial advice"
    Educational material only. Verify broker and CRA rules yourself.

## Reading path

**Part A — Mechanics**

1. [Disclaimer](disclaimer.md)  
2. [Glossary](../01-foundations/glossary.md)  
3. [Options basics](../01-foundations/options-basics.md)  
4. [Single-option payoffs](../01-foundations/single-option-payoffs.md)  
5. [Greeks](../01-foundations/greeks-enough-to-operate.md) → [Weekly vs monthly](../01-foundations/expirations-weekly-monthly.md)  

**Part B — Risk management**

6. [Ways to manage risk](../04-portfolio-and-risk/risk-management-categories.md)  
7. [Compare strategies with one example](../04-portfolio-and-risk/comparing-strategies-example.md)  

**Part C — Credit spreads (one tool)**

8. [Credit-spread payoffs](../01-foundations/payoff-diagrams-credit-spreads.md)  
9. Playbooks and [risk policy](../04-portfolio-and-risk/risk-policy.md)  
10. Canadian notes if relevant  

## Tags

| Tag | Meaning |
|-----|---------|
| `[verified]` | Matches independent public sources or a primary broker page |
| `[operator preference]` | Curriculum default you can change |
| `[pending-verify]` | Needs a stronger primary source |

## Local preview

```bash
pip install -r requirements.txt
mkdocs serve -f mkdocs.public.yml   # public site
mkdocs serve                        # includes private operator pages
```
