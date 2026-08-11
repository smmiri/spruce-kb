# Weekly vs monthly expirations

Proposal for a defined-risk income process, with notes on why short-dated shorts behave differently.

!!! danger "Not financial advice"
    Educational material only.

## Proposal (draft)

| Preference | Stance | Tag |
|------------|--------|-----|
| **Default for defined-risk income** | Prefer **monthly** (or longer dated) credit spreads | `[operator preference]` |
| **Weeklies** | Allowed with **tighter size** and stricter event/earnings checks | `[operator preference]` |
| **Hold to expiry vs close early** | Document both in your own manage/exit policy | Operator choice |

## Why monthly bias is defensible (not mandatory)

- Near expiry, **gamma** for ATM options rises — short-dated shorts can move P&amp;L faster. Supports tighter size on weeklies.  
- Fewer roll decisions if you review in batches; less weekend pin/gamma stress from ultra-short dated shorts.  
- Weeklies can still fit tactical views if size respects heat.

These are risk-management reasons, not proof monthlies outperform.

## Earnings and events

Regardless of weekly vs monthly: new short premium inside **N trading days** of earnings is blocked in the risk-policy proposal (starter default: 5 days) unless an audited override exists in your process.

`[verified]`: IV often elevates into earnings and can crush after; stocks can **gap** through strikes. `[operator preference]`: exact **N = 5**.

## Cognitive load

Prefer fewer expiries in flight. Soft caps on open positions live in the risk policy proposal.

## Questions to decide for yourself

- [ ] Accept monthly-default proposal?  
- [ ] If weeklies allowed, what max % of heat may sit in ≤7 DTE?  
- [ ] Default when a spread is threatened: hold, close, or roll?  

## Sources

- [tastylive — IV crush](https://www.tastylive.com/concepts-strategies/iv-crush)  
- [Sources index](../00-meta/sources.md)  

## Next

- [Risk policy proposal](../04-portfolio-and-risk/risk-policy.md)  

---

*Footer: Not financial advice. Verify broker rules yourself.*
