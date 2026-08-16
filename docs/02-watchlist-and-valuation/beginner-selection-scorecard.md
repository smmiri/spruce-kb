# Beginner selection scorecard

You already have a watchlist. The next system is **not** “go shop for new tickers.” It is: **score every name on that list twice**, then shortlist.

!!! danger "Not financial advice"
    Scores are operating filters, not forecasts. Delta is a **heuristic**, not a true probability. Confirm the live options chain and filings yourself.

## Two scores per name

| Score | Question | Used for |
|-------|----------|----------|
| **StockFit (0–3)** | Would I *own* this with long-term money? | Shortlist the **own-for-years** envelope (target 5–8 names) |
| **OptionsFit (0–3)** | Is this a sane name to *practice options* on? | Shortlist the **options** envelope (can differ from StockFit) |

A name can be high OptionsFit and low StockFit (example: a very liquid U.S. stock you do not want as a huge share holding). That is expected.

## Spreading the own-for-years money

Once names pass StockFit, dollars are not equal-weight by default. A simple **core–satellite** pattern `[operator preference]`:

| Piece | Share of the own-for-years envelope | Idea |
|-------|--------------------------------------|------|
| **Core** | about **40–60%** | One Canadian-listed **equity ETF** — either a global all-in-one *or* a single index (for example S&P 500 in CAD). Smaller core if satellites are companies **outside** that index |
| **Satellites** | the rest | A few companies you actually follow that are **not already inside the core** |
| **One company cap** | about **15%** of that envelope | Stops a single stock from becoming the whole portfolio |

Do not hold two ETFs that do the same job (two all-in-ones, or an all-in-one **plus** the S&P 500). If the core **is** the S&P 500, extra AAPL/GOOGL-type shares usually **increase** concentration, not balance. Satellites that spread a US-index core are typically **non-US** companies (Canada, Europe, Asia), not more S&P 500 names.

Dollar examples stay in the operator’s private log, not on this public page. A scrubbed ticker table is on [Example scored watchlist](example-scored-watchlist.md).

**Hard fail (score 0 on both)** if: crypto product, you cannot explain it, or the broker will not let you trade it.

## Which options “probability” method to start with

**Start with: defined-risk size + delta-as-POP.** `[operator preference]` aligned with common retail teaching.

| Idea | Plain meaning | When it applies |
|------|----------------|-----------------|
| **Max loss first** | Worst case of the *structure* must be ≤ **2%** of equity; heat ≤ **12%** | Every options trade, including long calls |
| **Delta ≈ rough chance the option finishes in the money** | A **0.20 delta** short put is often taught as “about 20% chance it expires in the money” — **rough**, not a promise `[verified]` as a common heuristic | Mostly when you **sell** premium (ladder step 3: credit spreads) |
| **Credit / width** | On a credit spread, credit ÷ strike-width is a crude “how much you get paid per dollar of max loss” | Same step 3 |

**Do not start with:** Kelly (needs a real edge you do not have yet), or a full **contract grader** (scores every strike). Those wait until you have a live chain feed.

**Name columns (D20 locked):** a **QVM-lite** rank (quality + value + momentum, 0–9) orders the own-for-years shortlist inside StockFit ≥ 2. An **LIV** column (liquidity + IV rank + earnings/events) orders option *names*. IV rank needs a 52-week IV history — leave it blank until the broker or ops can fill it; MVP uses the liquidity leg. Piotroski F-score is a company-only overlay (not ETFs). Greenblatt’s Magic Formula ranks a *large universe*, not a 12-name friends list.

**Ladder reminder:** you are still on **long calls/puts first**. For longs, OptionsFit is mostly **liquidity + size + earnings**, not selling 16-delta premium. The delta-as-POP rules become the main *trade* filter when you reach credit spreads. The *name* filter (this page) is useful from day one.

## StockFit (0–3)

| Points | Meaning |
|--------|---------|
| **3** | I can explain it; it is a broad ETF or a durable business I would hold without options; it will not eat the whole $24k by itself |
| **2** | I can explain it; quality is OK, but it is a concentrated/theme bet (e.g. one mega-cap tech) |
| **1** | Speculative or cyclical; only a small slice, if any |
| **0** | Crypto, story-only, or I do not understand it |

Canadian-listed ETFs still score well **if they are on the watchlist**. If they are not on the list yet, **add them then score** — do not pause scoring of names you already have.

## OptionsFit (0–3)

| Points | Meaning |
|--------|---------|
| **3** | U.S. listed; tight, busy options chain (you can enter and exit) |
| **2** | Options exist and are usable; a bit wider or jumpy |
| **1** | Chain exists but is a poor beginner market (wide quotes, thin) |
| **0** | No usable chain at your broker, or crypto |

Before a **live** options order, still check: earnings blackout (short premium), and max loss vs 2%/12%. Those are **trade** checks, not name scores.

## How this becomes automation

Same columns, same names:

1. **Done:** score the current watchlist by hand (private table).  
2. **Done (ops):** store StockFit / OptionsFit, QVM-lite, LIV liquidity, gates.  
3. **Suggest-only MVP:** propose high OptionsFit + LIV liquidity (and underfunded D19 stock names); human records skip / approve / reject / defer.  
4. **Later:** refresh scores; fill IV-rank on LIV; still HITL. No Magic Formula or contract grader until the data exists.

The dynamic watchlist is **re-scoring and suggesting**, not scraping the internet onto the list.

## Related

- [Operating checklists](../06-operating-playbooks/operating-checklists.md)  
- [Risk policy](../04-portfolio-and-risk/risk-policy.md)  
- [Greeks — delta](../01-foundations/greeks-enough-to-operate.md)  

---

*Not financial advice. Verify broker and CRA rules yourself.*
