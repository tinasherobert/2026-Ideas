# ROSCA Service — Base Example

**Idea #1 · ROSCA service** — Rotating Savings and Credit Association.

This document describes the base behaviour of the ROSCA service with a concrete example: 5 members, 10 months, fixed monthly contribution. Collateral is built in the first 5 months; months 6–9 are rotating payouts; month 10 is last member payout plus collateral shared equally.

---

## 1. Example setup

| Setting | Value |
|---------|--------|
| **Group size** | 5 members |
| **Savings period** | 10 months |
| **Monthly contribution** | 100 R per member |
| **Collateral** | Total of first 5 months’ contributions (no payouts in months 1–5) |
| **Payout rule** | Months 6–9: one member receives that month’s pool in rotation. Month 10: last member receives month 10 pool; **all members** receive their share from the collateral pool. |

**Pool per month** = 5 × 100 R = **500 R**  
**Group collateral** (after month 5) = 5 × 500 R = **2 500 R**

---

## 2. Group members (example)

| # | Member | Rotating payout (month) |
|---|--------|-------------------------|
| 1 | Thabo Molefe | 6 |
| 2 | Zanele Dlamini | 7 |
| 3 | Priya Naidoo | 8 |
| 4 | Marcus Okonkwo | 9 |
| 5 | Li Wei Chen | 10 (last) |

---

## 3. Contributions and payouts (10 months)

- **Months 1–5:** No payouts. Each member contributes **100 R** per month. All contributions form **group collateral**.
- **Months 6–9:** Each month the pool (**500 R**) is paid to one member in rotation (Thabo → Zanele → Priya → Marcus). Collateral (2 500 R) remains held.
- **Month 10:** **Li Wei** receives the month 10 pool (**500 R**). The **full collateral (2 500 R)** is then distributed to **all 5 members** (500 R each).

| Month | Thabo | Zanele | Priya | Marcus | Li Wei | **Pool** | **Cumulative collateral** | **Payout** |
|-------|-------|--------|-------|--------|--------|----------|----------------------------|------------|
| 1 | 100 | 100 | 100 | 100 | 100 | 500 | 500 | — |
| 2 | 100 | 100 | 100 | 100 | 100 | 500 | 1 000 | — |
| 3 | 100 | 100 | 100 | 100 | 100 | 500 | 1 500 | — |
| 4 | 100 | 100 | 100 | 100 | 100 | 500 | 2 000 | — |
| 5 | 100 | 100 | 100 | 100 | 100 | 500 | **2 500** | — |
| 6 | 100 | 100 | 100 | 100 | 100 | 500 | 2 500 (held) | **Thabo** 500 |
| 7 | 100 | 100 | 100 | 100 | 100 | 500 | 2 500 (held) | **Zanele** 500 |
| 8 | 100 | 100 | 100 | 100 | 100 | 500 | 2 500 (held) | **Priya** 500 |
| 9 | 100 | 100 | 100 | 100 | 100 | 500 | 2 500 (held) | **Marcus** 500 |
| 10 | 100 | 100 | 100 | 100 | 100 | 500 | 0 (distributed) | **Li Wei** 500 + **All 5** 500 each |

---

## 4. Month 10 in detail (last member + collateral)

| Payment | Amount | Recipient(s) |
|---------|--------|--------------|
| Last member payout (month 10 pool) | 500 R | Li Wei Chen |
| Collateral share | 500 R | Thabo Molefe |
| Collateral share | 500 R | Zanele Dlamini |
| Collateral share | 500 R | Priya Naidoo |
| Collateral share | 500 R | Marcus Okonkwo |
| Collateral share | 500 R | Li Wei Chen |
| **Total paid out in month 10** | **3 000 R** | 500 + (5 × 500) |

---

## 5. Summary by member

| Member | Total contributed | Rotating payout | Collateral share (month 10) | Total received | Net |
|--------|-------------------|-----------------|-----------------------------|----------------|-----|
| Thabo Molefe | 1 000 R | 500 R (month 6) | 500 R | 1 000 R | 0 |
| Zanele Dlamini | 1 000 R | 500 R (month 7) | 500 R | 1 000 R | 0 |
| Priya Naidoo | 1 000 R | 500 R (month 8) | 500 R | 1 000 R | 0 |
| Marcus Okonkwo | 1 000 R | 500 R (month 9) | 500 R | 1 000 R | 0 |
| Li Wei Chen | 1 000 R | 500 R (month 10) | 500 R | 1 000 R | 0 |
| **Total** | **5 000 R** | **2 500 R** | **2 500 R** | **5 000 R** | — |

Each member contributes **1 000 R** over 10 months and receives **1 000 R** in total: one rotating payout of **500 R** plus **500 R** from the collateral pool in month 10.

---

## 6. Collateral in this example

- **Months 1–5:** All contributions form **group collateral**. No payouts. End of month 5: collateral = **2 500 R**.
- **Months 6–9:** Collateral remains **2 500 R**. Only that month’s pool (500 R) is paid to the member in rotation. Collateral can back group rules (e.g. loans, defaults).
- **Month 10:** **Li Wei** receives the month 10 pool (500 R). The **full collateral (2 500 R)** is distributed to **all members** (500 R each). Cycle ends at zero balance.

*(Loan rules, e.g. 50% of collateral, can apply during the cycle; exact terms are set by the group.)*

---

## 7. Extended scenarios

Other documents use the same base setup (5 members, 10 months, 100 R/month) for:

| Scenario | Document | Description |
|----------|-----------|-------------|
| **1. Member default** | [ROSCA_SERVICE_DEFAULT.md](ROSCA_SERVICE_DEFAULT.md) | One member misses a payment; catch-up + penalty; penalty added to collateral and shared in month 10. |
| **2. Member removed** | [ROSCA_SERVICE_MEMBER_REMOVAL.md](ROSCA_SERVICE_MEMBER_REMOVAL.md) | Member removed; refund (contribution − penalty); cycle continues with fewer members; strategy adjusts months or payment. |
| **3. Loans** | [ROSCA_SERVICE_LOANS.md](ROSCA_SERVICE_LOANS.md) | Loans after collateral; interest and repayment penalties added to collateral, shared in month 10. |

---

## Related

- [Docs index](README.md)
- [ROSCA service — Member default](ROSCA_SERVICE_DEFAULT.md)
- [ROSCA service — Member removal](ROSCA_SERVICE_MEMBER_REMOVAL.md)
- [ROSCA service — Loans](ROSCA_SERVICE_LOANS.md)
- [Idea #2: AI support chat & call bots](BUSINESS_AI_SUPPORT_CHAT_AND_CALL_BOTS.md)
- [Idea #3:  Lay-By (SNBL)](LAYBY_SAVE_NOW_BUY_LATER.md)
