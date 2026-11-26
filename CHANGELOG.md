# Changelog

## 2026-11-26 — One amount, friendlier typing

- A holding now has a single **Amount**. Current value, gain/loss, units and price / NAV are gone. Existing holdings keep the old invested amount; current value and units from older data are ignored. Net worth is the sum of those amounts, and the gain/loss card is removed.
- Amount fields on the expense and holding forms are one big ₹ box (`type=text`, `inputmode=decimal`, no spinner, no `e`). Figures get Indian comma grouping as you type (1,00,000), and stay focused as the first field.
- Quick-add chips under the box add +100, +500, +1,000 or +5,000 to the amount.
- Pasting values like ₹1,200, 1200.50 or 1.2k (and L / lakh) is accepted. The stored value is a plain number.
- Older JSON backups that still have current or units fields still import. The savings CSV now has one Amount column.


## 2026-11-26 — Amount first, and custom Other names

- The amount field is at the top of both the Add / Edit expense form and the Add / Edit holding form, and it is focused with a numeric keyboard (`inputmode=decimal`) when the sheet opens.
- Both the expense category picker and the savings type dropdown have an **Other** option. Choosing it shows a box for a custom name (for example, Pet care). Saved names are remembered and offered as choices next time. They live in this browser and are included in the JSON backup; older backups still import.
- Custom expense categories appear in totals, the breakdown chart, and the expenses CSV. Custom savings types are grouped under Other for the chart and filters, and their name is shown on the holding and in the savings CSV.


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
