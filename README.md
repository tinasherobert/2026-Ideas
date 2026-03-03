# 2026 Ideas Board

A curated list of potential projects and ideas for 2026. Each idea is documented in the [`docs/`](docs/) folder with overviews and, where applicable, worked examples and scenarios.

---

## Ideas

### 1. ROSCA service (Rotating Savings and Credit Association)

**Status:** Documented · **Docs:** [Base example & scenarios](docs/ROSCA_SERVICE.md)

Rotating savings group: fixed group size and term (e.g. 5 members, 10 months), fixed monthly contribution. Collateral is built in the first 5 months (no payouts); months 6–9 are rotating payouts; month 10 is last member payout plus collateral shared equally.

| Document | Description |
|----------|-------------|
| [ROSCA service — Base example](docs/ROSCA_SERVICE.md) | 5 members, 10 months, 100 R/month; collateral build, rotation, month 10 payout |
| [ROSCA service — Member default](docs/ROSCA_SERVICE_DEFAULT.md) | One member misses a payment; catch-up + penalty; penalty added to collateral |
| [ROSCA service — Member removal](docs/ROSCA_SERVICE_MEMBER_REMOVAL.md) | Member removed; refund minus penalty; cycle continues with fewer members |
| [ROSCA service — Loans](docs/ROSCA_SERVICE_LOANS.md) | Loans after collateral; interest/penalties added to collateral, shared in month 10 |

Full index: [docs/README.md](docs/README.md).

---

### 2. Businesses: AI support chat and call bots

**Status:** Documented · **Doc:** [Overview](docs/BUSINESS_AI_SUPPORT_CHAT_AND_CALL_BOTS.md)

AI-powered support agents for businesses: chat and voice (call) bots that answer FAQs, triage issues, and escalate to humans. One platform for both channels, with knowledge-base training, handoff, and analytics.

| Document | Description |
|----------|-------------|
| [AI support chat & call bots](docs/BUSINESS_AI_SUPPORT_CHAT_AND_CALL_BOTS.md) | Overview, scope, and possible features |

---

### 3. Lay-By (Save Now, Buy Later)

**Status:** Documented · **Doc:** [Overview](docs/LAYBY_SAVE_NOW_BUY_LATER.md)

Digital lay-by service alongside the core (e.g. ROSCA service): same wallet, no credit check, no interest. Customers reserve at merchants and pay in instalments (deposit + plan); merchants get APIs/plugins, VRP collection, and dashboards. Informed by LayUp-style investigation (omnichannel, travel/pre-orders, optional rewards and AI).

| Document | Description |
|----------|-------------|
| [Lay-By (SNBL)](docs/LAYBY_SAVE_NOW_BUY_LATER.md) | Positioning vs core, services, AI use-cases, differentiation |

---

## Contributing

Add new ideas as documents in `docs/` and list them above with a short description and link.
