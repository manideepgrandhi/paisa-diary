# Changelog

## 2026-11-26 — Holding type dropdown

- The Add / Edit holding sheet now has one type dropdown, grouped as Common (Mutual Fund, Stocks, FD, PPF, EPF, Gold) and then the rest by category.
- Interest rate and maturity fields show only for deposits and similar schemes. Units and price / NAV show only for market and metal types (and if a holding already has units).
- Existing holdings and the Savings filter chips are unchanged.


## 2026-11-26 — Savings tab

- New **Savings** tab for holdings (mutual funds, stocks, ETFs, FD, RD, PPF, EPF, VPF, NPS, SSY, NSC, KVP, post office schemes, SCSS, SGB, gold, silver, bonds, corporate FD, real estate, savings account, emergency cash, crypto, ULIP, chit fund, and other).
- Optional units and price / NAV: when both are filled, current value is units × price. Otherwise you type the current value.
- Net worth is the sum of current holdings. This month’s spending is shown beside it, not subtracted.
- Recurring rules can be an **Expense** (auto-logged as spend) or an **Investment / SIP** (shown on Savings, not counted as spend). Existing rules stay expenses.
- JSON backup is now version 3 and includes holdings. Version 1 and 2 backups still import.
- New **Savings CSV** export, with Excel-safe dates.
- A month-by-month net worth chart fills in as you use the app; it does not invent past history.

## 2026-10 — Recurring payments

- Recurring rules, auto-logging with catch-up, upcoming 7 days, and backup version 2.

## 2026-10 — First release

- Daily expense tracker, categories, totals, JSON backup and expenses CSV.
