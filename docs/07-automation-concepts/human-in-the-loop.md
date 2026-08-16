# Human-in-the-loop and dry-run

Spruce-ops is not an autopilot. The agent may **observe** and **suggest**. It may **send** an order only after an explicit approval, a policy check, and a kill-switch that is off.

!!! danger "Not financial advice"
    Automation does not change that you own every live order.

## Capability modes

| Mode | Meaning |
|------|---------|
| **Observe-only** | Read positions, watchlist, alerts. No “you should trade this” ticket. |
| **Suggest-only** | Candidates and management notes. You decide; the journal records skip / approve / reject / defer. |
| **Execute-with-approval** | Broker submit only after you approve, policy passes, dry-run is off, kill-switch is off. |

Default for a long time: **suggest-only**, with **dry-run on**. spruce-ops Suggest-only MVP: in-app candidates queue + journal decisions; Telegram / broker send stay later.

## Dry-run

`DRY_RUN=true` means prepare-order builds a payload and stores it. It does **not** send. Live send is a later, deliberate switch — not a convenience toggle during Week 2.

## What this implies while you still trade by hand (Wealthsimple)

There is **no official Wealthsimple trading API**. Until spruce-ops talks to **IBKR**, checklists and a journal *are* the system. Do not scrape the WS app.

## Kill-switch

A global halt: no prepare, no send, alerts only. Use it when heat is wrong, you are traveling, or you do not trust the last sync.

## Related

- [Operating checklists](../06-operating-playbooks/operating-checklists.md)  
- [Risk policy](../04-portfolio-and-risk/risk-policy.md)  

---

*Not financial advice. Verify broker rules yourself.*
