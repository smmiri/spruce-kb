# Canadian brokers for options

Canadians who want defined-risk options face a real choice: several CIRO-regulated dealers offer options, but **API access, strategy allowlists, platforms, and fee shapes differ a lot**. This page is a comparison map — not a recommendation to open any account.

!!! danger "Not financial advice"
    Educational notes only. Fees, permissions, and APIs change. Confirm the current schedule and **your** account approvals with each broker.

## Working assumption for this curriculum

For defined-risk **credit spreads**, many Canadians begin in a **non-registered margin** account and treat TFSA/RRSP as a narrower options profile until the broker confirms each strategy in writing. That pattern shows up across major Canadian dealers. Details: [TFSA constraints](tfsa-options-constraints.md) · [Cash vs margin](cash-vs-margin.md).

## Dimensions that matter

| Dimension | Why it matters |
|-----------|----------------|
| **Strategy permissions** | Credit spreads usually need a higher options level and often **margin** |
| **Registered vs margin** | TFSA/RRSP allowlists are typically narrower than margin |
| **CAD / USD funding & FX** | U.S. underlyings dominate liquid equity options; conversion spreads add cost |
| **Commission model** | Ticket + per-contract vs per-contract-only vs $0 contract fees change cost of multi-leg trades |
| **Platform & data** | Chains, multi-leg tickets, Greeks, and streaming OPRA/options data |
| **Exports / statements** | Journaling and tax lots need reproducible fills |
| **Official trading API** | Matters if you want **supported** programmatic access — unofficial scrapers are not the same thing |

## Broker sketches

Fees below are **illustrative snapshots** from broker public pages around **August 2026**. Always re-check the live schedule. Regulatory, exchange, exercise/assignment, inactivity, market-data, and FX costs can sit outside the headline options rate.

### Interactive Brokers Canada (IBKR / IBC)

**Offerings & services.** Global markets (stocks, options, futures, FX, bonds, funds, and more), professional platforms (TWS, Client Portal, mobile), IBKR Campus education, detailed reporting (including Flex-style exports), and multi-currency accounts. Options tools are aimed at active / complex traders.

**Options fees (published shape).** U.S. options are typically **tiered per contract** (often cited in the **USD ~0.15–0.65** range depending on premium and monthly volume), with a **minimum per order** (commonly **USD 1.00** on tiered). Canadian-listed options have a separate CAD per-contract schedule (e.g. around **CAD 1.00–1.25**/contract with a minimum). Exchange, clearing, and regulatory fees may apply on top of the commission line. `[verified]` against [IBC options commissions](https://www.interactivebrokers.ca/en/pricing/commissions-options.php) — confirm live tiers.

**API access.** Strong official support: **Web API**, **TWS API**, and institutional **FIX**. Can cover account data, market data, and order placement (subject to permissions and risk checks). Local Gateway / TWS is a common retail path. `[verified]` against [IBKR Trading API](https://www.interactivebrokers.ca/en/trading/ib-api.php).

**Advantages often cited.** Deep product set and global access; mature official APIs; competitive active-trader economics at volume; rich reporting; multi-currency workflow.

**Shortcomings often cited.** Steeper learning curve; market-data subscriptions can add cost; account/permission setup is more “pro desk” than consumer app; inactive or small accounts may find the UX and fee stack less intuitive than simpler Canadian apps.

### Questrade

**Offerings & services.** Self-directed Canadian brokerage with stocks/ETFs, options (including multi-leg), margin, dual-currency accounts, Questrade Pro / mobile, optional **Questrade Plus** subscription, and published options education / level matrices.

**Options fees (published shape).** **U.S. equity options:** $0 contract fees for online trades (Plus subscribers may earn cashback, e.g. **CAD 0.05**/contract). **Canadian-listed options:** **CAD 0.99**/contract. **U.S. index options:** separate schedule (volume-tiered until late September 2026, then flat **USD 0.99**/contract per published transition). Assignment fees on U.S. equity options are advertised as $0 in recent pricing. `[verified]` against [Questrade transaction fees](https://www.questrade.com/pricing/self-directed-commissions-plans-fees/transaction) — re-check before acting.

**API access.** Official **REST API** with OAuth for account data, positions, orders history, and market quotes. **Order placement via API is limited to Questrade partner developers** — ordinary retail customers can generally **read** data but **not** execute trades through the public API. `[verified]` against [Questrade Developer Platform](https://developer.questrade.com/).

**Advantages often cited.** Familiar Canadian retail UX; competitive / $0 U.S. equity options contract fees; dual-currency; clear options-level documentation; useful read-only API for account and market data even when trade-submit is blocked.

**Shortcomings often cited.** Retail API **cannot** place orders; advanced data (e.g. OPRA streaming) may be paid or bundled; platform depth vs IBKR for global/complex products is different; fees and Plus bundling change over time.

### Wealthsimple

**Offerings & services.** Consumer investing app with equities/ETFs and, more recently, **equity options** including covered calls, secured puts, and multi-leg structures (verticals, calendars, diagonals, butterflies/condors, etc. — subject to approval). Long calls/puts, secured puts, and covered calls may be available in registered accounts; **other strategies typically require a margin account** with USD enabled. U.S. listed underlyings are the focus.

**Options fees (published shape).** Markets itself as **$0 commission and $0 contract fees** on equity options (as of mid‑2026 marketing). FX conversion, exercise/assignment, and other account fees can still apply — read the Trade fee disclosure. `[verified]` against [Wealthsimple options](https://www.wealthsimple.com/en-ca/trade/options) — re-check before acting.

**API access.** **No official public trading API.** Community reverse-engineered wrappers exist; they are unsupported and fragile.

**Advantages often cited.** Very low headline options trading cost; polished mobile/web UX; multi-leg strategies (including credit spreads) on margin once approved; simple onboarding relative to pro platforms.

**Shortcomings often cited.** No supported API path; product universe narrower than global multi-asset brokers (e.g. Canadian-listed options / index options may be limited or unavailable); FX and assignment edge-cases still matter; less of a “desk” reporting stack for people who rely on exports and APIs.

### Bank and traditional discount brokers

Grouped because the API story is similar even when fees differ: **TD Direct Investing**, **Qtrade**, **National Bank Direct Brokerage (NBDB)**, **CI Direct Trading** (formerly Virtual Brokers), **RBC Direct Investing**, **Scotia iTRADE**, **CIBC Investor’s Edge**, **BMO InvestorLine**, and peers.

**Offerings & services.** Full-service Canadian account types (TFSA, RRSP, non-registered, often margin), Canadian and U.S. equities/ETFs, options with level-based approvals, bank-integrated funding, phone desks, and proprietary web/mobile platforms. Some offer active-trader tiers or paid advanced platforms.

**Options fees (published shapes — examples only).**

| Broker (example) | Typical published options shape (online) |
|------------------|------------------------------------------|
| **TD Direct Investing** | Stock-like ticket (e.g. **~$9.99** standard / **~$7** active) **+ ~$1.25**/contract |
| **Qtrade** | **$0** ticket + **~$0.75**/contract (assignment/exercise fees separate) |
| **NBDB** | **$0** ticket + **~$1.25**/contract with a **minimum** (e.g. **~$6.25**) |
| **CI Direct Trading** | Ticket (e.g. **~$7.99**, lower if active) **+ ~$1.25**/contract; advanced platforms may be paid |

Confirm each firm’s live PDF/schedule. Phone-assisted and assignment/exercise fees are often much higher than online rates.

**API access.** Generally **no public retail trading API**. Workflow is UI + exports (CSV/PDF).

**Advantages often cited.** Banking relationship / funding ease; Canadian customer support in familiar channels; registered-account coverage; for some users, “good enough” options levels without learning TWS.

**Shortcomings often cited.** Higher all-in cost on multi-leg U.S. equity options vs $0-contract brokers; limited or no official API; platform feature depth varies; strategy approval matrices still gate credit spreads.

## Fee structure — how to read the models

| Model | Rough shape | What it does to a 2-leg credit spread |
|-------|-------------|----------------------------------------|
| **Ticket + per contract** | Fixed $ per order + $ per contract | Spreads pay the ticket once (or per leg, depending on how the broker bills multi-leg) plus contracts on every leg |
| **Per contract + order minimum** | Low $/contract but a floor per order | Cheap at many contracts; small 1–2 contract tickets can hit the minimum |
| **$0 contract (equity options)** | No commission line on eligible U.S. equity options | Headline cost shifts to FX, data, subscriptions, and assignment/exercise |
| **Hybrid / subscription** | Base plan + cashback or bundled data | Compare **all-in** monthly cost, not only the options line |

For defined-risk spreads, **count every leg**, remember **open and close**, and include **FX** if you fund in CAD and trade USD underlyings.

## API and auto-trading readiness

| Broker family | Official read (account / quotes) | Official trade submit (retail) | Practical note |
|---------------|----------------------------------|-------------------------------|----------------|
| **IBKR Canada** | Yes (Web / TWS APIs) | Yes (with approvals, risk checks) | Broadest supported retail API surface among these |
| **Questrade** | Yes (REST + OAuth) | **Partner developers only** | Useful for account/market data; not a retail order API |
| **Wealthsimple** | No official public API | No | Manual UI only |
| **Bank / traditional discounters** | Usually none public | Usually none | CSV/PDF exports + manual tickets |

**Never bypass broker risk controls via API.** Unofficial session scraping is not “having an API.”

## Side-by-side comparison (no ranking)

Use this as a **tradeoff sheet**. Different rows will matter more depending on whether you optimize for fees, API access, UX, or banking convenience. **No column wins overall.**

| | **IBKR Canada** | **Questrade** | **Wealthsimple** | **Bank / traditional discounters** |
|--|-----------------|---------------|------------------|--------------------------------------|
| **Primary strength** | Global markets + API depth | Canadian retail + competitive options pricing | Consumer UX + $0 equity options headline | Funding / relationship convenience |
| **Typical friction** | Complexity, data fees | Retail trade API locked | No official API; narrower product set | Higher tickets; little programmatic access |
| **Credit spreads** | Available with approvals / margin | Level-gated; margin for higher levels | Margin (+ USD) for multi-leg | Level-gated; firm-specific |
| **TFSA options** | Narrow published list | Narrower than margin | Long / covered / secured puts may be allowed; multi-leg usually not | Firm-specific; usually constrained |
| **U.S. equity options fees** | Tiered $/contract + min | Often $0/contract (online) | Often $0 commission + $0 contract | Often ticket + ~$0.75–$1.25/contract |
| **Official API** | Full retail trading APIs | Read yes / trade partner-only | None official | Generally none |
| **Reporting / exports** | Very strong (Flex, etc.) | Solid statements + API reads | App-centric; check export depth | Statements / CSV vary |
| **Best fit if you…** | Need supported programmatic trading or global markets | Want Canadian UX + low U.S. equity options fees, maybe read-only API | Want simple UI and lowest headline options ticket | Want bank-linked funding and are fine trading by hand |

## Questions to ask any broker

Use this when you message support or review your approval matrix. It is not a form on this site.

| Topic | Why it matters |
|-------|----------------|
| Options permissions for **multi-leg credit spreads** on **this** account type | Spreads need the right level on the account you will fund |
| TFSA / RRSP vs margin allowlist (get it in writing or screenshot) | Registered rules are usually narrower |
| CAD vs USD funding and FX conversion method / spread | Dominates cost for CAD-funded U.S. options |
| How multi-leg orders are billed (one ticket vs per leg) | Changes effective commission |
| Exercise / assignment notices and fees | Short options can be assigned; fees and timing differ |
| Market-data packages required for live options chains | Streaming OPRA/options data is often extra |
| Statements / API / CSV exports for journaling | Needed for reproducible records |
| Whether **retail** API can **place** orders (not only read) | Decides if programmatic trading is even possible |

For IBKR specifically, also re-read [IBC TFSA/RRSP information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) after permission changes.

## Pattern day trader notes

U.S. **PDT** rules are U.S.-specific. Canadian accounts still face **margin, buying-power, and broker risk controls**. Forum advice from U.S. IBKR or tastytrade-style accounts does not always map to Canadian dealers.

## Risk disclosure

Before trading options, read the OCC document *Characteristics and Risks of Standardized Options* (brokers usually require an acknowledgment). Uncovered writing risks are called out there.

## Related reading

- [TFSA options constraints](tfsa-options-constraints.md)  
- [Cash vs margin](cash-vs-margin.md)  
- [Sources](../00-meta/sources.md)  

---

*Not financial advice. Verify with your broker, CIRO disclosures, and advisors. Fees and APIs dated from public pages ~August 2026 — re-check before acting.*
