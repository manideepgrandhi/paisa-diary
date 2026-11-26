# Paisa Diary

A small, mobile-friendly tracker for daily expenses and savings. It lives at [manideepgrandhi.github.io/paisa-diary](https://manideepgrandhi.github.io/paisa-diary/). There is no sign-up and no server: everything stays in this browser, on this device.

## What it does

- **Expenses** — log spending by category, with today / week / month totals and a breakdown chart.
- **Recurring** — rent, EMIs, bills, SIPs. Expense rules are auto-logged when you open the app. Investment / SIP rules are not counted as spend; they show on the Savings tab instead.
- **Savings** — holdings such as mutual funds, stocks, FD, PPF, EPF, NPS, gold, cash and more. Type in the current value, or fill units and price / NAV and the app will multiply them for you. Net worth is the sum of current holdings. “This month spent” is shown beside it, not subtracted again.

## Backup

Your data can disappear if you clear the site’s data or switch browsers. Use the ⋯ menu now and then:

- **JSON backup** — download and keep a file. Import it later (or on another device). Older backups without savings still import; they simply have no holdings.
- **Expenses CSV** and **Savings CSV** — for Excel or Sheets. Dates in the savings file are written so Excel will not turn them into date serials.

## Running it locally

The site is a single `index.html`. Open it in a browser, or serve the folder:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080/`.
