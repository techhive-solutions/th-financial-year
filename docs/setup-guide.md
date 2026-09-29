# Setup guide

## Install

Install **Financial Year Switcher** from Apps. It works on Community and Enterprise, on Odoo.sh or your own
server. Installing hides nothing.

## Run the setup wizard

The wizard opens once after install. You can run it again at any time from **Settings > General Settings >
Financial Year > Run setup**.

1. **Calendar.** Choose the month your Financial Year starts in. With Accounting installed, it is read from the
   company's fiscal year end. Then choose the year the first Financial Year starts in: it defaults to the year
   of your earliest record.
2. **What to scope.** Only models installed in your database are listed, with the date field that decides which
   year a record is in, the earliest record and the record count. Journal entries are scoped together with their
   journal items, and transfers with their stock moves.
3. **Check and apply.** Each Financial Year is listed with its record count by model. Switch on **Open to all
   users** for the past years everyone should still see. If records are dated before the first year, a warning
   tells you how many: go back and choose an earlier first year to keep them visible.

After **Apply**, the page reloads and the switcher appears in the top bar, next to the company switcher.
