# Admin guide

## Financial Years

**Settings > Users & Companies > Financial Years** lists them. Each has a start and end date, and they can't
overlap. The next year is created automatically when it starts. You can rename a year or change its dates here.

## Who can select which years

- Users in **Access all Financial Years** can select every year. Settings administrators and Accounting
  administrators have it. Give it to other users on their user form, under **Financial Year**.
- Everyone else can select the current year, plus any year with **Open to all users** switched on.
- Portal and public users are never affected.

The same limits apply everywhere: the web client, exports, XML-RPC and AI assistants connected over MCP. A
request without a selection, such as a scheduled action or an XML-RPC call, sees the current year.

## Which models are scoped

**Settings > Users & Companies > Financial Year Scope** lists one line per model, with its date field. Switch a
line off to stop scoping that model. Add a line to scope another model: any stored date or datetime field works.
For a record with a date range, such as a payslip, use the end date.

## What users see

- The switcher shows the selected year, or the number of years selected. **Confirm** applies a new selection;
  clicking a year's name selects only that year.
- Records dated outside the selection are hidden in lists, forms, reports and exports.
- Opening a record from another year shows which year it is in, and whether to switch or ask an administrator.
- On Odoo Enterprise, opening balances in the Partner Ledger, General Ledger, Trial Balance and Aged Receivable
  and Payable include every earlier year.

## Hiding is not locking

Financial Year Scope decides what users see. To stop posting in a closed period, use Odoo's lock dates.

## Uninstalling

Uninstalling removes every rule the module added, and all records are visible again.
