# Operating checklists

Use these in a batch session. They encode the operator trial rules as **percent of equity**. Dollar caps live in your private log.

!!! danger "Not financial advice"
    Checklists are process aids, not trade recommendations.

## Before the session

- [ ] Kill-switch is off only if you intend to consider new risk  
- [ ] Heat *before* any new trade is under **12%** of equity  
- [ ] You know whether you are on ladder step **1** (long calls/puts), **2** (covered calls), or **3** (CCS/PCS)  
- [ ] USD account is enabled if the underlying is U.S.-listed  
- [ ] Earnings calendar checked for names you might touch  
- [ ] If the cash market is **closed**: stock/ETF ticket is **Limit** at last close, not Market ([order types](order-types.md))  

## Entry

- [ ] Thesis in one or two sentences (journal first)  
- [ ] Name is on the **starter** watchlist, not the later/high-vol bucket, unless you explicitly override  
- [ ] Stock/ETF: **limit** (or you are watching a live tape and accept a market print)  
- [ ] Options: **regular hours** only; you can see a two-sided market you would actually trade  
- [ ] Expiration: prefer a **monthly**; if weekly, size smaller  
- [ ] **Max loss** of this structure ≤ **2%** of equity  
- [ ] After a hypothetical fill: heat ≤ **12%**; this name ≤ **5%**; this sector ≤ **15%** of heat  
- [ ] Open positions still inside the **6–8** soft cap  
- [ ] Not inside the **5-trading-day** earnings blackout for new short premium (spreads / covered short calls)  
- [ ] Covered call only if you already hold **100 shares per contract** in the same account  
- [ ] No naked / undefined short options  

## Management (default)

- [ ] Default: **close or roll around 21 DTE** — do not sit expiration week as the base case `[operator preference]`  
- [ ] If the short strike is tested or the thesis is dead: close or roll with a new max-loss check  
- [ ] Rolling must still pass the 2% / 12% / 5% tests on the *new* structure  
- [ ] Long options: have a time stop (e.g. 21 DTE) or a thesis invalidation — do not “hope” through decay  

## Exit / weekly review

- [ ] Every close has a reason in the journal (profit, 21 DTE, thesis fail, heat, earnings)  
- [ ] Count open max losses vs 12% heat  
- [ ] Note rule breaks (even tiny ones)  
- [ ] No new risk if you are tired, rushed, or unclear on max loss  

## Related

- [Order types](order-types.md)  
- [Risk policy](../04-portfolio-and-risk/risk-policy.md)  
- [PCS playbook](../03-strategies/put-credit-spread-playbook.md) · [CCS playbook](../03-strategies/call-credit-spread-playbook.md)  
- [HITL / dry-run](../07-automation-concepts/human-in-the-loop.md)  

---

*Not financial advice. Verify broker rules yourself.*
