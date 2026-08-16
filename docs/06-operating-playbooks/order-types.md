# Stock order types (weekend and the open)

You can plan and **queue** stock or ETF buys when the market is closed. The risk is not “trading on Saturday.” It is sending an order that will pay **any** Monday opening price.

!!! danger "Not financial advice"
    Broker tickets differ. Confirm live labels and expiry on your app. This page uses percents and process, not account dollars.

## What happens when you submit after the close

Regular North American cash sessions are roughly **Monday–Friday, 9:30–16:00 Eastern**. `[verified]` as the usual NYSE/TSX window; holidays differ.

Orders placed **outside** that window typically go into a **queue**. The broker **submits them at the next regular open** (Monday 9:30 ET after a normal weekend, or the next session after a holiday). `[verified]` against common Canadian broker help text (including Wealthsimple: queued orders execute when the market opens).

The fill is the **opening prints**, not Friday’s last trade. Canadian-listed names open on the TSX clock; U.S.-listed names open on the U.S. clock. Same idea.

A **gap** is when the first Monday trade is away from Friday’s close (news, futures, FX). Gaps are normal. For a long-term share sleeve they are **not** a special disaster **if you refuse to pay any price**.

## Four common buy types

Names match a typical Wealthsimple **Buy** ticket. Other brokers use the same ideas.

| Type | What Monday open does | Beginner default for queued stock buys |
|------|------------------------|----------------------------------------|
| **Market buy** | Fill at the **best available** open price — no cap. If the market was closed when you sent it, that price is Monday’s open, which can be far from Friday. Brokers may **cancel** a queued market **buy** if the open would overdraw the account. `[verified]` as Wealthsimple’s stated market-order behaviour | **Do not queue** when the market is closed `[operator preference]` |
| **Limit buy** | Fill only at your **limit or cheaper**. If the open gaps **above** the limit, you get nothing (or a partial) | **Yes — default** `[operator preference]` |
| **Stop limit buy** | Waits until price **rises through** a stop, then becomes a limit. A breakout tool, not “buy my core over the weekend” | **No** for ordinary long-term entries |
| **Stop market buy** | After a stop, becomes a **market** order. Some apps disable it **outside market hours** | **No** for ordinary long-term entries |

**Curriculum default `[operator preference]`:** for stock/ETF orders sent when the market is closed, use **Limit buy**. Use the **last official close** as the buy-limit **ceiling**. If Monday opens at or below that price, you can fill. If it gaps up, you do **not** chase. Unfilled is acceptable; review after the session and queue again later if you still want the name.

Use **day / this-session expiry**, not a 90-day good-until-cancelled, until you are used to leftover working orders.

The same limit default is reasonable **during** the day for a slow accumulation sleeve. Market orders are for people who accept any print in a very liquid name **while they are watching**.

## Options

Place options only in **regular hours**, after you can see a **two-sided** chain you would actually trade. Weekend stock tickets are not an options workflow. See [operating checklists](operating-checklists.md).

## Related

- [Glossary](../01-foundations/glossary.md) — market, limit, gap, queued order  
- [HITL / dry-run](../07-automation-concepts/human-in-the-loop.md)  

---

*Not financial advice. Verify broker rules yourself.*
