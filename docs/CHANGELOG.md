# Changelog

## 18.0.1.1.0 (2026-10-05)

Fixes from testing on Odoo 18.0 Community and Enterprise, and two small features.

- Enterprise's Trial Balance and General Ledger keep the Undistributed Profits/Losses row when one Financial
  Year is selected, so they balance again.
- Sales, Purchase and Invoice Analysis are scoped together with sales orders, purchase orders and journal
  entries. Databases that already scope those switch them on when upgrading.
- The Purchase dashboard's Avg Order Value, Lead Time to Purchase, Purchased Last 7 Days and RFQs Sent follow the
  selected years.
- An API request for Financial Years the user can't open gets an Access Error naming them, instead of the
  current year's records.
- The Date Field of a Financial Year Scope mapping is picked from the model's date fields, in Settings and in
  the setup wizard.
- The module won't install next to `ys_financial_year`, and its web client names no longer clash with it. The
  switcher's cookie is renamed, so after upgrading each user's selection goes back to the current year once,
  and links that carried the old `fys` key open on the current year.

## 18.0.1.0.0 (2026-09-29)

First release of Financial Year Switcher for Odoo 18.0.

- A Financial Year switcher in the top bar and the mobile menu: select one year or several.
- Financial Year Scope: records dated outside the selected years are hidden by record rules, for any model with
  a date field, with journal items and stock moves scoped together with their entries and transfers.
- The Access all Financial Years group, and Financial Years open to all users. Everyone else can select only the
  current year.
- A setup wizard after install: the fiscal calendar, the models to scope and a preview with record counts. Nothing
  is hidden until it is applied.
- Opening balances in Enterprise's Partner Ledger, General Ledger, Trial Balance and Aged Receivable and Payable
  keep full history.
- AI assistants connected over MCP see every year their user may access.
- Access Errors name the Financial Year to switch to.
- The new year is created when it starts, and uninstalling removes every rule the module added.
