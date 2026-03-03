# ROSCA Service — Scenario 2: Member Removed from Group

**ROSCA service** — One member is removed (deactivated, banned, failed to pay, or cannot continue).

When a member is removed we: (1) **Calculate their contribution so far** and apply a **penalty**; the **removed member is refunded contribution minus penalty**; the **penalty is retained in the pool** and added to collateral, shared in the last month among **current active members only**. (2) **Continue the cycle** with the remaining members using a **strategy** that may adjust months or monthly payment (or both).

---

## 1. Base setup before removal

| Setting | Value |
|---------|--------|
| **Group size** | 5 members (then 4 after removal) |
| **Original plan** | 10 months, 100 R per member per month |
| **Removal** | **Priya Naidoo** removed at **end of month 2** (e.g. failed to pay, banned, or left). |
| **Penalty on removal** | 50 R (group-defined); **retained in pool** (added to collateral). Removed member refunded **contribution − penalty**. |
| **Strategy chosen** | **Keep monthly contribution at 100 R** and **keep total cycle at 10 months**. Collateral build continues 3 more months (3–5) with 4 members; rotating payouts months 6–9; month 10: last member + collateral shared by 4 members. |

**Before removal:** Thabo Molefe, Zanele Dlamini, **Priya Naidoo**, Marcus Okonkwo, Li Wei Chen.  
**After removal:** Thabo, Zanele, Marcus, Li Wei (4 members).

---

## 2. Calculation at removal (end of month 2)

| Item | Amount |
|------|--------|
| Priya’s contributions so far | 2 × 100 R = **200 R** (already in pool) |
| Penalty fee (retained in pool, added to collateral) | **50 R** |
| **Refund to Priya** (contribution − penalty) | 200 − 50 = **150 R** |
| Pool after refund (1 000 − 150) | **850 R** |

Priya **receives 150 R**. The **50 R penalty** remains in the pool and becomes part of collateral, shared among the **4 active members** in month 10.

---

## 3. Contributions and collateral after removal (4 members)

From **month 3**, **pool per month** = 4 × 100 R = **400 R**.

- **Months 3–5:** No payouts. Collateral: 850 + 400 + 400 + 400 = **2 050 R**.
- **Months 6–9:** Rotating payouts **400 R** each (Thabo → Zanele → Marcus → Li Wei). Collateral stays 2 050 R.
- **Month 10:** Last member (Li Wei) receives **400 R** (month 10 pool). **2 050 R** collateral shared by **4 members** = **512.50 R** each.

| Month | Thabo | Zanele | Marcus | Li Wei | **Pool** | **Cumulative collateral** | **Payout** |
|-------|-------|--------|--------|--------|----------|----------------------------|------------|
| 1 | 100 | 100 | 100 | 100 | 500 (5 members) | 500 | — |
| 2 | 100 | 100 | 100 | 100 | 500 (5 members) | 1 000 | — |
| **Removal:** Priya refunded **150 R** (200 − 50). Penalty **50 R** retained. | | | | | | **850** | — |
| 3 | 100 | 100 | 100 | 100 | 400 | 1 250 | — |
| 4 | 100 | 100 | 100 | 100 | 400 | 1 650 | — |
| 5 | 100 | 100 | 100 | 100 | 400 | **2 050** | — |
| 6 | 100 | 100 | 100 | 100 | 400 | 2 050 (held) | **Thabo** 400 |
| 7 | 100 | 100 | 100 | 100 | 400 | 2 050 (held) | **Zanele** 400 |
| 8 | 100 | 100 | 100 | 100 | 400 | 2 050 (held) | **Marcus** 400 |
| 9 | 100 | 100 | 100 | 100 | 400 | 2 050 (held) | **Li Wei** 400 |
| 10 | 100 | 100 | 100 | 100 | 400 | 0 (distributed) | **Li Wei** 400 + **All 4** 512.50 each |

*(Priya omitted from month 3 onward.)*

---

## 4. Month 10 in detail (4 active members)

| Payment | Amount | Recipient(s) |
|---------|--------|--------------|
| Last member payout (month 10 pool) | 400 R | Li Wei Chen |
| Collateral share | 512.50 R | Thabo Molefe |
| Collateral share | 512.50 R | Zanele Dlamini |
| Collateral share | 512.50 R | Marcus Okonkwo |
| Collateral share | 512.50 R | Li Wei Chen |
| **Total collateral distributed** | **2 050 R** | 4 × 512.50 R |

---

## 5. Summary by active member (after removal)

| Member | Months contributed | Total contributed | Rotating payout | Collateral share | Total received | Net |
|--------|--------------------|-------------------|-----------------|------------------|----------------|-----|
| Thabo Molefe | 10 | 1 000 R | 400 R (month 6) | 512.50 R | 912.50 R | −87.50 R |
| Zanele Dlamini | 10 | 1 000 R | 400 R (month 7) | 512.50 R | 912.50 R | −87.50 R |
| Marcus Okonkwo | 10 | 1 000 R | 400 R (month 8) | 512.50 R | 912.50 R | −87.50 R |
| Li Wei Chen | 10 | 1 000 R | 800 R (months 9 + 10) | 512.50 R | 1 312.50 R | +312.50 R |

*(Li Wei receives both month 9 rotating payout and month 10 pool + collateral share; with 4 members there are 4 rotating slots in 6–9, so month 9 is Li Wei and month 10 is “last”—adjust if your rotation rule differs.)*

The 4 active members contribute 4 000 R in total and receive 4 × 400 (rotating) + 400 (month 10) + 2 050 (collateral) = 4 050 R. The **50 R penalty** (retained from Priya) is shared among them; most of that benefit goes to Li Wei (two payouts), so he nets +312.50 R and the other three net −87.50 R each.

**Removed member (Priya):** Contributed **200 R**, receives **150 R** (contribution − penalty). Net **−50 R**.

---

## 6. Strategy options (when a member is removed)

The group (or platform) can define a **strategy** for the rest of the cycle. Examples:

| Strategy | Description | Effect in this example |
|----------|-------------|-------------------------|
| **Keep months, keep monthly amount** | Same 10 months, same 100 R/month per member. | Pool drops to 400 R (4 members). Collateral = 2 050 R; shared by 4 in month 10. |
| **Keep months, increase monthly amount** | Still 10 months; raise monthly contribution so total collateral matches original plan. | e.g. 125 R/month × 4 × 5 months build = 2 500; plus 50 penalty = 2 550; share 637.50 each. |
| **Extend months, keep monthly amount** | Keep 100 R/month; add months so effective collateral or payouts match. | e.g. one extra build month: 2 050 + 400 = 2 450; 5 rotating months 6–10; month 11 last + collateral. |

The exact strategy (adjust months vs monthly payment) is **configurable**.

---

## 7. Rules used

1. **Trigger:** Member is removed (deactivated, banned, failed to pay, or cannot continue).
2. **At removal:** Calculate member’s **contribution so far**; apply **penalty**. **Refund** = **contribution − penalty**. **Penalty is retained** in the pool and added to collateral.
3. **Collateral share** in the last month is only among **current active members** (here, 4).
4. **Continue cycle** with remaining members; **strategy** defines whether to adjust **months** or **monthly payment** (or both).

---

## Related

- [Docs index](README.md)
- [ROSCA service — Base example](ROSCA_SERVICE.md)
- [ROSCA service — Member default](ROSCA_SERVICE_DEFAULT.md)
- [ROSCA service — Loans](ROSCA_SERVICE_LOANS.md)
- [Idea #2: AI support chat & call bots](BUSINESS_AI_SUPPORT_CHAT_AND_CALL_BOTS.md)
- [Idea #3:  Lay-By (SNBL)](LAYBY_SAVE_NOW_BUY_LATER.md)
