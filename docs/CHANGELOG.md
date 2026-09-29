# Changelog

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
