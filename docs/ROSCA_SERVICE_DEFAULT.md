# ROSCA Service — Scenario 1: Member Default

**ROSCA service** — One member defaults on a payment.

This scenario uses the same base setup as the [ROSCA service base example](ROSCA_SERVICE.md) (5 members, 10 months, 100 R/month). One member misses a payment; they pay the missed amount plus a **penalty fee**. The **penalty is added to group collateral** and shared equally in month 10.

---

## 1. Base setup

| Setting | Value |
|---------|--------|
| **Group size** | 5 members |
| **Savings period** | 10 months |
| **Monthly contribution** | 100 R per member |
| **Collateral** | First 5 months’ contributions (no payouts months 1–5). Month 10: last member + collateral shared equally. |
| **Default penalty** | 25 R (e.g. 25% of one contribution; group-defined) |

**Members:** Thabo Molefe, Zanele Dlamini, Priya Naidoo, Marcus Okonkwo, Li Wei Chen.

---

## 2. What happens

- **Month 3:** **Thabo** does not pay his 100 R on time (default).
- **Month 4:** Thabo pays:
  - **100 R** (catch-up for month 3)
  - **100 R** (normal month 4)
  - **25 R** (penalty)  
  Total in month 4: **225 R**.
- The **25 R penalty** is added to **group collateral** (not to the normal monthly pool). The 100 R catch-up counts as month 3 contribution; month 3 pool remains 500 R for collateral.
- **End of month 5:** Collateral = 5 × 500 R + **25 R** = **2 525 R**.
- **Month 10:** Last member (Li Wei) receives month 10 pool (500 R). **Full collateral 2 525 R** is shared equally: **505 R** each to all 5 members.

---

## 3. Contributions and collateral (with default and penalty)

| Month | Thabo | Zanele | Priya | Marcus | Li Wei | **Pool** | **Penalty to collateral** | **Cumulative collateral** | **Payout** |
|-------|-------|--------|-------|--------|--------|----------|----------------------------|----------------------------|------------|
| 1 | 100 | 100 | 100 | 100 | 100 | 500 | — | 500 | — |
| 2 | 100 | 100 | 100 | 100 | 100 | 500 | — | 1 000 | — |
| 3 | **0** (default) | 100 | 100 | 100 | 100 | 400* | — | 1 400 | — |
| 4 | **225** (100+100+25) | 100 | 100 | 100 | 100 | 500 + 25 | **25** | 2 025 → **2 525** | — |
| 5 | 100 | 100 | 100 | 100 | 100 | 500 | — | **2 525** | — |
| 6 | 100 | 100 | 100 | 100 | 100 | 500 | — | 2 525 (held) | **Thabo** 500 |
| 7 | 100 | 100 | 100 | 100 | 100 | 500 | — | 2 525 (held) | **Zanele** 500 |
| 8 | 100 | 100 | 100 | 100 | 100 | 500 | — | 2 525 (held) | **Priya** 500 |
| 9 | 100 | 100 | 100 | 100 | 100 | 500 | — | 2 525 (held) | **Marcus** 500 |
| 10 | 100 | 100 | 100 | 100 | 100 | 500 | — | 0 (distributed) | **Li Wei** 500 + **All 5** 505 each |

\* Month 3: 400 R received on time; Thabo’s 100 R received in month 4 as catch-up. Collateral still counts month 3 as 500 once catch-up is paid (end-of-month-5 collateral = 2 500 + 25 = 2 525).

---

## 4. Month 10: Collateral distribution (with penalty)

| Payment | Amount | Recipient(s) |
|---------|--------|--------------|
| Last member payout (month 10 pool) | 500 R | Li Wei Chen |
| Collateral share | **505 R** | Thabo Molefe |
| Collateral share | **505 R** | Zanele Dlamini |
| Collateral share | **505 R** | Priya Naidoo |
| Collateral share | **505 R** | Marcus Okonkwo |
| Collateral share | **505 R** | Li Wei Chen |
| **Total collateral distributed** | **2 525 R** | 5 × 505 R |

The **25 R penalty** increases each member’s collateral share by **5 R** (25 ÷ 5).

---

## 5. Summary by member

| Member | Total contributed | Rotating payout | Collateral share | Total received | Net |
|--------|-------------------|-----------------|------------------|----------------|-----|
| Thabo Molefe | 1 025 R (incl. 25 penalty) | 500 R (month 6) | 505 R | 1 005 R | −20 R* |
| Zanele Dlamini | 1 000 R | 500 R (month 7) | 505 R | 1 005 R | +5 R |
| Priya Naidoo | 1 000 R | 500 R (month 8) | 505 R | 1 005 R | +5 R |
| Marcus Okonkwo | 1 000 R | 500 R (month 9) | 505 R | 1 005 R | +5 R |
| Li Wei Chen | 1 000 R | 500 R (month 10) | 505 R | 1 005 R | +5 R |

\* Thabo effectively bears the 25 R penalty (contributes 1 025 R, receives 1 005 R). The other four each gain 5 R from the penalty shared in collateral.

---

## 6. Rules used

1. **Default:** Missed contribution must be paid (catch-up) plus a **penalty fee** (group-defined).
2. **Penalty destination:** Penalty is **added to group collateral**, not to the defaulting member’s personal balance.
3. **Collateral share:** Increased collateral (2 525 R) is **shared equally** among **all** members in month 10 (505 R each).
4. **Notifications:** The system notifies the member of the missed payment and penalty (e.g. email and in-app).

---

## Related

- [Docs index](README.md)
- [ROSCA service — Base example](ROSCA_SERVICE.md)
- [ROSCA service — Member removal](ROSCA_SERVICE_MEMBER_REMOVAL.md)
- [ROSCA service — Loans](ROSCA_SERVICE_LOANS.md)
- [Idea #2: AI support chat & call bots](BUSINESS_AI_SUPPORT_CHAT_AND_CALL_BOTS.md)
- [Idea #3:  Lay-By (SNBL)](LAYBY_SAVE_NOW_BUY_LATER.md)
