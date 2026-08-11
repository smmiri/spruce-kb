# Put credit spread (PCS) playbook — draft

Operator draft for defined-risk bullish-to-neutral premium selling (bull put spread).

!!! danger "Not financial advice"
    Educational draft only. Not a trade recommendation.

## Intent

Collect a credit when your thesis is that the underlying **stays above the short put** through expiry (or you manage successfully before max loss is realized).

Standard name: **bull put spread** / put credit vertical. `[verified]` structure & payoff — see [payoffs](../01-foundations/payoff-diagrams-credit-spreads.md).

## Structure reminder

Sell higher-strike put / buy lower-strike put. Max profit ≈ credit; max loss ≈ width − credit.

## Entry sketch

1. **Thesis** — Why will price not crash through the short strike? (support, quality, valuation snapshot). Direction matches standard bull-put use.  
2. **Liquidity** — Prefer underlyings/options with acceptable open interest and tight markets; skip junk fills. Numeric OI/volume floors remain `[pending-verify]` / `[operator preference]`.  
3. **Expiry** — Prefer monthly per [expirations](../01-foundations/expirations-weekly-monthly.md) unless a weekly is sized tighter.  
4. **Strikes** — Short put near target delta band; long put sets width and max loss.  
   - `[verified]` as common heuristic: short premium often discussed in ~**0.15–0.30** absolute delta.  
   - `[operator preference]`: exact short/long targets in your written policy.  
5. **Size** — Contracts so **max loss ≤** your per-trade cap and post-trade **heat** still within policy. Common retail guidance starts near **1–2% equity** per trade (`[verified]` as common guidance — not a prescription).  
6. **Events** — No new short premium inside the earnings blackout window in the risk proposal unless you use an audited override. Gap risk into earnings `[verified]` as a phenomenon; **N days** is preference.  
7. **Journal** — Thesis, strikes, credit, max loss, tags.

## Management pointers

- Prefer not entering bad setups over heroic mid-trade repairs.  
- If threatened: closing for a defined loss, rolling, or holding to expiry are all process choices — write your default.  
- Do not invent undefined hedges that break the defined-risk profile without policy.

## Exit / profit-taking

Decide in advance whether you hold for remaining credit decay, close at a profit target, or manage by time (e.g. before last week). Tag any numeric target `[operator preference]`.

## Anti-patterns

- Sizing off “premium looks big” instead of max loss  
- Ignoring sector/underlying concentration  
- Treating PCS as “safe” because it is defined-risk  
- Naked short put “temporary” without cash/defined structure  

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- [Sources index](../00-meta/sources.md)  

## Related

- [CCS playbook](call-credit-spread-playbook.md)  
- [Risk policy](../04-portfolio-and-risk/risk-policy.md)  

---

*Footer: Not financial advice. Verify broker rules yourself.*
