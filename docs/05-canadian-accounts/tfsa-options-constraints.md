# TFSA options constraints

**Verify with your broker and the CRA (and a tax advisor).** This page is a caution map updated with broker documentation — not clearance to trade any strategy inside a TFSA.

!!! danger "Not financial advice / verify required"
    Registered-account rules and broker allowlists differ and change. Illegal or broker-prohibited activity is never in scope for Spruce.

## Curriculum default profile

Treat TFSA as a **separate, narrower policy profile**:

- Do **not** assume US-style options freedom inside TFSA.  
- Prefer defined-risk **PCS/CCS** process in a **non-registered / margin** account until you have **broker-written confirmation** for each strategy in TFSA.  

Cross-check reason: at major Canadian brokers, **multi-leg spreads are often a higher options level that requires a margin account**, while registered accounts are capped at lower levels.

## Interactive Brokers Canada (primary page)

Per [IBC TFSA trading permissions](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) (`[verified]` against broker page as of review):

- **No margin** in TFSA; purchases paid in full; account debits not permitted.  
- Options called out include: **long** equity calls/puts; **covered calls**; **protective puts**.  
- Do **not** assume credit spreads are available in an IBC TFSA without explicit confirmation in Client Portal for *your* account.

## Questrade (example of industry level caps)

Per [Questrade options levels](https://www.questrade.com/learning/using-questrade/options-levels) (`[verified]` against broker page; page notes update Mar 2026):

- Registered accounts (RRSP, TFSA, FHSA) can only be approved up to **Level 2**.  
- **Spreads = Level 3** and require a **margin** account (and minimum equity).  
- Level 2 includes covered calls / cash-secured puts (with notes); not the Spruce CCS/PCS workhorse path.

Other brokers may differ — always check *your* firm’s matrix.

## Typically more constrained / often restricted

| Theme | Why it matters |
|-------|----------------|
| **Naked / uncovered** short options | Margin / short-sale style risk; blocked in TFSA at brokers surveyed |
| **Multi-leg short premium / spreads** | Often Level 3+ and margin-only (e.g. Questrade) |
| **Leverage / borrowing** inside TFSA | Not permitted (IBC: no margin in TFSA) |
| **High-frequency / “business” trading** | CRA may scrutinize whether TFSA activity is carrying on a business — **ask a tax advisor** `[pending-verify]` for your facts |

## Often discussed as more workable (still broker-dependent)

| Theme | Caveat |
|-------|--------|
| Long shares / ETFs | Still verify product eligibility |
| Long calls / long puts | Listed on IBC TFSA permissions; still not Spruce’s primary income process |
| Covered calls if shares held and broker allows | On IBC TFSA list; confirm for your account |
| Cash-secured puts | Broker-specific; Questrade documents CSP at Level 2 including some registered cases — **confirm**; not a substitute for verifying your broker |

## Operator checklist

- [ ] Listed every strategy you might use (PCS, CCS, CSP, CC, …)  
- [ ] Asked your broker which are allowed in TFSA vs margin **for your approvals**  
- [ ] Documented answers privately  
- [ ] Read [Sources](../00-meta/sources.md)  

## Sources

- [Interactive Brokers Canada — RRSP/TFSA information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php)  
- [Questrade — Options levels](https://www.questrade.com/learning/using-questrade/options-levels)  
- [IBKR Campus — Options as part of an RRSP/TFSA strategy](https://www.interactivebrokers.com/campus/traders-insight/securities/options/options-as-part-of-an-rrsp-tfsa-strategy/) (education; still verify tax)  

---

*Footer: Not financial advice. Verify with broker and CRA.*
