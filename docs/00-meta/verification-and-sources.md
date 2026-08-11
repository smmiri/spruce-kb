# Verification and sources (private / local-only)

!!! warning "Not published on GitHub Pages"
    This page is excluded from `mkdocs.public.yml`. Use the public [Sources](sources.md) page online. Keep this file for operator history.

Week-1 drafts were first rewritten from private `learning-material` notes. On **2026-08-10** a second pass cross-checked core claims against independent sources. Tags on pages were updated accordingly.

!!! danger "Not financial advice"
    Sources below are for education and verification of definitions/mechanics — not recommendations.

## Tag legend (after this pass)

| Tag | Meaning |
|-----|---------|
| `[verified]` | Consistent with ≥2 independent reputable sources *or* a primary broker/regulator page for that specific claim |
| `[personal preference]` | Spruce operating choice (may be informed by common ranges) |
| `[course-derived]` | From learning notes; may still be useful process framing |
| `[pending-verify]` | Still needs stronger primary-source backup |

## What checked out (mechanics)

| Claim | Result | Sources (examples) |
|-------|--------|-------------------|
| Vertical credit spread max profit = net credit; max loss ≈ width − credit; PCS/CCS breakevens | `[verified]` | [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp), [Wikipedia — Credit spread (options)](https://en.wikipedia.org/wiki/Credit_spread_(option)) |
| Bull put = PCS; bear call = CCS naming | `[verified]` | Same as above |
| Naked/uncovered call: theoretically unlimited loss | `[verified]` | OCC *Characteristics and Risks of Standardized Options*; broker risk disclosures summarizing OCC |
| Delta ≈ rough ITM-probability heuristic (not a guarantee) | `[verified]` as heuristic | [tastylive](https://www.tastylive.com/news-insights/options-delta-predictive-probability-gauge-directional-measure), SpotGamma / options education articles |
| Short-premium delta bands often discussed around ~0.15–0.30 | `[verified]` as common heuristic range | Options education sites (e.g. OptionsBench / premium-selling primers) — **not** a law; D14 still locks Spruce’s band |
| Size defined-risk trades off max loss, often ~1–2% of equity per trade in retail guidance | `[verified]` as common guidance | Multiple retail risk/position-sizing writeups (industry rule-of-thumb, not regulation) |
| Aggregate “portfolio heat” often discussed ~10–15% (conservative) up to higher for aggressive books | Informs D3 | Same class of retail risk frameworks; Spruce’s **20%** stays `[personal preference]` pending workshop |
| Earnings: IV often rises into the event and can crush after; gaps can pierce short strikes | `[verified]` as phenomena | tastylive IV crush explainers; earnings/options risk articles |
| Exact “N trading days before earnings” blackout | Remains `[personal preference]` | Common to sit out; **N = 5** is Spruce’s proposal |

## Canadian / broker (primary-ish)

| Claim | Result | Sources |
|-------|--------|---------|
| IBKR Canada TFSA: **no margin**; listed options limited to long calls/puts, covered calls, protective puts (per IBC page) | `[verified]` against broker page | [IBC RRSP/TFSA information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) |
| Questrade: registered accounts (TFSA/RRSP/FHSA) max **Level 2**; spreads = Level 3 require **margin** | `[verified]` against broker page | [Questrade options levels](https://www.questrade.com/learning/using-questrade/options-levels) (updated Mar 2026) |
| CRA “business” risk if TFSA trading is frequent/systematic | Caveat retained; verify with advisor | Broker education pages + common CRA discussion — still **verify with tax advisor** |
| Spreads (PCS/CCS) as default live process → prefer non-registered/margin | Strengthened Spruce default | Follows Level 3 / multi-leg restrictions at major Canadian brokers |

## Still preference / open (do not over-claim)

- Exact CAD max loss (D2)  
- Heat 20% / underlying 10% / sector 25% (D3) — **20% heat is toward the aggressive end** vs common 10–15% heat guidance  
- Hold-to-expiry vs early close (D13)  
- Exact short/long delta targets (D14)  
- Minimum credit as % of width  
- Numeric OI/volume floors  

## How to re-verify later

1. Prefer primary docs (OCC, broker permission pages, CRA guidance) over blogs.  
2. For any new numeric “system rule,” require ≥2 independents **or** explicit `[personal preference]`.  
3. Re-check broker TFSA/options matrices before ops encodes allowlists — they change.

---

*Footer: Not financial advice. Verify broker and CRA rules yourself.*
