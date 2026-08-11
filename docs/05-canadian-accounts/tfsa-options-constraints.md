# TFSA options constraints

**Verify with your broker, the CRA, and a tax advisor.** This page is a caution map from broker documentation — not permission to trade a strategy inside a TFSA.

!!! danger "Not financial advice"
    Registered-account rules differ by firm and change over time.

## The short version

Treat the TFSA as a **narrower** options profile than a U.S.-style margin account. For Spruce’s workhorse **PCS/CCS** process, prefer a **non-registered / margin** account until your broker confirms each strategy for TFSA in writing.

Why: at major Canadian brokers, multi-leg spreads often sit at a higher options level that requires margin, while registered accounts are capped lower.

## What Interactive Brokers Canada publishes

From [IBC’s TFSA trading permissions](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) (`[verified]` against that page):

- **No margin** in TFSA; purchases paid in full; account debits not permitted.  
- Options listed include **long** equity calls and puts, **covered calls**, and **protective puts**.  
- Do **not** assume credit spreads are available in an IBC TFSA without confirming for your account.

## What Questrade publishes (industry example)

From [Questrade options levels](https://www.questrade.com/learning/using-questrade/options-levels) (`[verified]` against that page):

- Registered accounts (TFSA / RRSP / FHSA) max out at **Level 2**.  
- **Spreads are Level 3** and require a **margin** account.  
- Level 2 covers ideas like covered calls and cash-secured puts (with notes) — not the CCS/PCS path these playbooks describe.

Other brokers may differ. Always check *your* matrix.

## Usually restricted or blocked in TFSA

| Theme | Why people flag it |
|-------|--------------------|
| Naked / uncovered short options | Margin-style risk; blocked in TFSA at brokers surveyed here |
| Multi-leg short-premium spreads | Often Level 3+ / margin-only |
| Borrowing / leverage inside TFSA | Not permitted (IBC: no margin in TFSA) |
| Very frequent speculative trading | CRA may ask whether activity looks like a business — ask a tax advisor |

## Sometimes workable (still broker-dependent)

| Theme | Caveat |
|-------|--------|
| Long shares / ETFs | Confirm product eligibility |
| Long calls / long puts | On IBC’s TFSA list; not Spruce’s primary income process |
| Covered calls when you hold the shares | On IBC’s list; confirm for your account |
| Cash-secured puts | Broker-specific; do not infer IBKR from another firm’s blog |

## Before you fund a strategy in TFSA

| Step | Purpose |
|------|---------|
| List every strategy you might use (PCS, CCS, CSP, covered call, …) | You cannot confirm what you have not named |
| Ask the broker which of those are allowed in TFSA vs margin | Get it in writing or screenshot Client Portal |
| Keep that answer private with your records | Public sites should not hold your account details |
| Skim [Sources](../00-meta/sources.md) | Know which public pages were used for this summary |

## Sources

- [Interactive Brokers Canada — RRSP/TFSA information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php)  
- [Questrade — Options levels](https://www.questrade.com/learning/using-questrade/options-levels)  
- [IBKR Campus — Options as part of an RRSP/TFSA strategy](https://www.interactivebrokers.com/campus/traders-insight/securities/options/options-as-part-of-an-rrsp-tfsa-strategy/)  

---

*Not financial advice. Verify with broker and CRA.*
