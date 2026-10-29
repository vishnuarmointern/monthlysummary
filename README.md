# Monthly Summary

Pick a month/year range and get a month-by-month summary of the Google Sheet (entry count + totals of every numeric column), with a grand total and monthly average at the bottom. CSV export, print, light/dark.

- `index.html`: the site (GitHub Pages). The Apps Script URL is set in `API_URL` near the top of the script.
- `apps-script/Code.gs`: the backend. Paste it into the Apps Script project, run `setLogin()` once, then deploy a new version (Execute as: Me, Access: Anyone).

The backend auto-detects the date column (first header containing "date") and sums the numeric columns; adjust `CONFIG` at the top of `Code.gs` to pin a tab, date column or columns to skip.
