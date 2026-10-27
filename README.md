# BTO Office Days Calculator

A responsive, standalone website that calculates estimated monthly office attendance requirements.

## How it works
- Select a month and year.
- The website automatically counts Monday–Friday weekdays for that month.
- Enter the number of public holidays that fall on working days and the number of leave days.
- It deducts PH and leave days, applies a 50% attendance rate, and rounds the result up to the next whole office day.

**Formula:** `ceil((weekdays in month - PH - leaves) × 50%)`

## Important assumptions
- Weekends are Saturday and Sunday.
- Public holiday dates are not fetched automatically; you enter the count for your applicable location/company calendar.
- The 50% rate and rounding-up rule are based on the example calculation discussed, not a verified official Capgemini policy. Adjust the code if your current internal policy differs.
- This is an independent planning tool, not an official Capgemini application.

## Host on GitHub Pages
1. Create a new repository on GitHub, for example `bto-office-days-calculator`.
2. Upload `index.html` to the repository root (and optionally this README).
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then save.
6. Wait for GitHub Pages to publish the site. The published URL will be shown in the Pages section.

No backend, API key, or build step is required.
