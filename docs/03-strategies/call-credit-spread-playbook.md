# Call credit spread (CCS) playbook — draft

Operator draft for defined-risk “won’t rip higher” premium selling (bear call spread).

!!! danger "Not financial advice"
    Educational draft only. Not a trade recommendation.

## Intent

Collect a credit when your thesis is that the underlying **stays below the short call** through expiry (or you manage successfully). Typical use: stretched names where you refuse the theoretically unlimited risk of a **naked** short call (`[verified]` unlimited risk for uncovered calls).

Standard name: **bear call spread** / call credit vertical. `[verified]` — [Investopedia vertical spreads](https://www.investopedia.com/terms/v/verticalspread.asp).

Use CCS when you do not expect a large short-term rise; pair with a journaled research bias (valuation, technical location, “extended” tape).

## Structure reminder

Sell lower-strike call / buy higher-strike call. Max profit ≈ credit; max loss ≈ width − credit. See [payoffs](../01-foundations/payoff-diagrams-credit-spreads.md).

## Entry sketch

1. **Thesis** — Why will price not melt up through the short call?  
2. **Liquidity** — Same bar as PCS.  
3. **Expiry** — Monthly bias; weeklies only with tighter size.  
4. **Strikes** — Short call at target delta; long call defines width.  
   - `[verified]` common short-premium heuristic band ~0.15–0.30Δ.  
   - `[operator preference]` for exact targets in your policy.  
5. **Size** — Max loss and heat policy — not “% of portfolio in premium.”  
6. **Events** — Earnings blackout per risk proposal.  
7. **Journal** — Include why CCS instead of PCS (or both on different names).

## Management pointers

Same philosophy as PCS: avoid broken setups; when wrong, choose close / roll / hold with eyes open.

## Anti-patterns

- Naked short call because “I almost sold a spread”  
- Stacking correlated CCS (e.g. many mega-cap tech) until sector heat blows past policy  
- Ignoring that a strong trend can run farther than your credit  

## Sources

- [Investopedia — Vertical spread](https://www.investopedia.com/terms/v/verticalspread.asp)  
- OCC / broker disclosures on uncovered call writing  
- [Sources index](../00-meta/sources.md)  

## Related

- [PCS playbook](put-credit-spread-playbook.md)  
- [Defined-risk overview](defined-risk-credit-spreads.md)  
- [Risk policy](../04-portfolio-and-risk/risk-policy.md)  

---

*Footer: Not financial advice. Verify broker rules yourself.*
