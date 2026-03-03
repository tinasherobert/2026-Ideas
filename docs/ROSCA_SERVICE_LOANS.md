# ROSCA Service — Scenario 3: Loans Against Collateral

**ROSCA service** — Loans allowed after collateral is built.

In this scenario, a member may take a **loan only after** the collateral (first 5 months’ contributions) is in place. The loan is **against that collateral**. Any **profit** from the loan (interest or repayment penalties) is **added to total collateral** and shared equally in the last month.

---

## 1. Base setup

| Setting | Value |
|---------|--------|
| **Group size** | 5 members |
| **Savings period** | 10 months |
| **Monthly contribution** | 100 R per member |
| **Collateral** | First 5 months’ contributions = **2 500 R**. No payouts in months 1–5. |
| **Loan rule** | Loan allowed only **after** collateral is fully built (after month 5). Loan amount limited by group (e.g. up to 50% of member’s collateral share). |
| **Interest / penalties** | All **profit** (interest, late repayment penalties) is added to collateral and shared in month 10. |

**Members:** Thabo Molefe, Zanele Dlamini, Priya Naidoo, Marcus Okonkwo, Li Wei Chen.  
**Collateral share per member** (end of month 5) = 2 500 ÷ 5 = **500 R** each.  
**Example loan limit** (50% of share) = **250 R** per member.

---

## 2. Loans in this scenario (after month 5)

| Member | Loan amount | Interest rate | Interest (profit) | Repayment (principal) |
|--------|-------------|---------------|--------------------|------------------------|
| Zanele Dlamini | 200 R | 10% | 20 R | 200 R (repaid on time) |
| Marcus Okonkwo | 100 R | 10% | 10 R | 100 R (repaid on time) |
| **Total profit to collateral** | | | **30 R** | |

- Loans taken in **month 6** (after collateral is in place).
- Interest due on repayment (e.g. over 2 months). **20 R** and **10 R** are **added to group collateral**.
- **End-of-cycle collateral** = 2 500 + 30 = **2 530 R**.
- **Month 10:** Each member receives **2 530 ÷ 5 = 506 R** from the collateral pool.

---

## 3. Contributions, collateral, and loan profit

| Month | Pool | **Cumulative collateral** | **Loan / profit** | **Payout** |
|-------|------|----------------------------|-------------------|------------|
| 1–5 | 500/mo | 500 → 1 000 → 1 500 → 2 000 → **2 500** | — | — |
| 6 | 500 | 2 500 (held) | Zanele borrows 200 R; Marcus borrows 100 R. | **Thabo** 500 |
| 7–9 | 500 | 2 500 → **2 530** (held) | Repayments with interest. **Total profit to collateral: 30 R** (20 + 10). | **Zanele** 500 (mo 7), **Priya** 500 (mo 8), **Marcus** 500 (mo 9) |
| 10 | 500 | 0 (distributed) | — | **Li Wei** 500 + **All 5** **506 R** each |

*(Interest and any repayment penalties are added to collateral when received; here total profit is **30 R**, so collateral at month 10 = 2 530 R.)*

---

## 4. Month 10: Collateral distribution (with loan profit)

| Payment | Amount | Recipient(s) |
|---------|--------|--------------|
| Last member payout (month 10 pool) | 500 R | Li Wei Chen |
| Collateral share | **506 R** | Thabo Molefe |
| Collateral share | **506 R** | Zanele Dlamini |
| Collateral share | **506 R** | Priya Naidoo |
| Collateral share | **506 R** | Marcus Okonkwo |
| Collateral share | **506 R** | Li Wei Chen |
| **Total collateral distributed** | **2 530 R** | 5 × 506 R |

The **30 R** loan profit increases each member’s collateral share by **6 R** (30 ÷ 5).

---

## 5. Summary by member (with loans)

| Member | Total contributed | Rotating payout | Collateral share | Total received | Net |
|--------|-------------------|-----------------|------------------|----------------|-----|
| Thabo Molefe | 1 000 R | 500 R (month 6) | 506 R | 1 006 R | +6 R |
| Zanele Dlamini | 1 000 R | 500 R (month 7) | 506 R | 1 006 R | +6 R |
| Priya Naidoo | 1 000 R | 500 R (month 8) | 506 R | 1 006 R | +6 R |
| Marcus Okonkwo | 1 000 R | 500 R (month 9) | 506 R | 1 006 R | +6 R |
| Li Wei Chen | 1 000 R | 500 R (month 10) | 506 R | 1 006 R | +6 R |

*(Zanele and Marcus paid interest; that interest goes to group collateral, so all 5 members benefit equally.)*

---

## 6. Loan rules used

1. **Eligibility:** A member may get a loan **only after** group collateral (first 5 months’ contributions) is fully built.
2. **Limit:** Loan is **against** the member’s collateral share; group sets the cap (e.g. 50% of share → max 250 R per member here).
3. **Profit to collateral:** All **profit** from the loan (interest and any repayment penalties) is **added to total collateral**.
4. **Sharing:** The increased collateral is **shared equally** among all members in the **last month** (month 10).

---

## 7. Optional: Late repayment penalty

If a member repays **late**, the group can charge a **penalty**. That penalty is also **added to collateral** and shared in month 10. Example: Marcus repays 10 R interest + 15 R late penalty → **25 R** to collateral instead of 10 R. Total collateral would be 2 500 + 20 + 25 = 2 545 R; each member gets 509 R in month 10.

---

## Related

- [Docs index](README.md)
- [ROSCA service — Base example](ROSCA_SERVICE.md)
- [ROSCA service — Member default](ROSCA_SERVICE_DEFAULT.md)
- [ROSCA service — Member removal](ROSCA_SERVICE_MEMBER_REMOVAL.md)
- [Idea #2: AI support chat & call bots](BUSINESS_AI_SUPPORT_CHAT_AND_CALL_BOTS.md)
- [Idea #3:  Lay-By (SNBL)](LAYBY_SAVE_NOW_BUY_LATER.md)
