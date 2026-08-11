# Open decisions (private / local-only)

!!! warning "Not published on GitHub Pages"
    This page is excluded from `mkdocs.public.yml`. Operator decision log only.

Maps each Spruce decision (D1–D14) to KB pages to read before you decide. Mark status during your review; formal close happens in the **Week-2 workshop**. Canonical status also lives in `option-trading/SPRUCE_MASTER_PLAN.md` §10.

!!! danger "Not financial advice"
    Decisions are personal operating choices, not recommendations.

## Review pass scheduling

- [ ] **Review pass scheduled:** date/time _______________________  
- [ ] Reading order in [how to use](how-to-use-this-site.md) completed  
- [ ] Questions captured on [glossary](../01-foundations/glossary.md) and below  

## Decision table

| ID | Topic | Current assumption | Read first | When | Your notes / status |
|----|-------|--------------------|------------|------|---------------------|
| **D1** | Watchlist universe | Equity/ETF-focused; ~20–40 symbols later | Foundations; (watchlist pages Week 2) | After Week-1 review | Open — _______ |
| **D2** | Max loss per trade | Hard cap required; retail guidance often ~1–2% equity | [Risk policy](../04-portfolio-and-risk/risk-policy.md), PCS/CCS playbooks, [verification](verification-and-sources.md) | Week-2 workshop | Open — _______ |
| **D3** | Heat / concentration | 20% / 10% / 25% proposed (note: common heat bands often ~10–15%) | [Risk policy](../04-portfolio-and-risk/risk-policy.md) | Week-2 workshop | Proposed — _______ |
| **D4** | Strategy priority | CCS/PCS first; wheel later; PMCC/IC later | [Defined-risk](../03-strategies/defined-risk-credit-spreads.md), playbooks | Week-2 workshop | Assumed — _______ |
| **D5** | Account / TFSA posture | Non-registered/margin first; TFSA narrow (IBC/Questrade docs support) | [IBKR](../05-canadian-accounts/ibkr-canada-notes.md), [TFSA](../05-canadian-accounts/tfsa-options-constraints.md), [cash vs margin](../05-canadian-accounts/cash-vs-margin.md) | Week-2 workshop | Open — _______ |
| **D6** | IBKR API path | Gateway + ib_insync **or** Client Portal | Automation concepts (Week 2 stub) | Ops Weeks 3–4 | Open — defer |
| **D7** | KB generator | MkDocs Material | This site | Week 1 | **Assumed / in use** |
| **D8** | Ops UI stack | FastAPI + HTMX | Automation concepts (Week 2) | Ops start | Assumed — defer |
| **D9** | License | Apache-2.0 | [Disclaimer](disclaimer.md), repo LICENSE | Week 1 | **Assumed / in use** |
| **D10** | Auto-close on max loss | Disabled until months 6–12 | Risk + HITL (later) | Months 6–12 | Deferred |
| **D11** | Home server host | Always-on Linux preferred | — | Ops start | Open — defer |
| **D12** | Public domain | github.io first | — | After KB v1 | Deferred |
| **D13** | Hold to expiry vs close early | Preference pending verify | Playbooks; closing/managing (Week 2) | Week-2 workshop | Open — _______ |
| **D14** | Delta / width targets | Common short band ~15–30Δ; course ~30/10 wing still preference | [Greeks](../01-foundations/greeks-enough-to-operate.md), PCS/CCS playbooks | Week-2 workshop | Open — _______ |

## Workshop prep prompts

1. What CAD (or %) max loss lets you sleep while still making practice meaningful? (D2)  
2. Do 20/10/25 heat numbers feel too loose, too tight, or fine to trial? (D3)  
3. Confirm CCS/PCS-first and naked ban. (D4)  
4. Which account runs live spreads first? (D5)  
5. Default manage rule when a spread is threatened? (D13)  
6. Lock provisional delta bands or keep ranges only? (D14)  

---

*Footer: Not financial advice. Verify broker and CRA rules yourself.*
