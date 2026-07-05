# Power BI Step-by-Step Guide

## Step 1 — Open Power BI Desktop

Open Power BI Desktop and create a blank report.

## Step 2 — Import CSV files

Go to:

Home → Get Data → Text/CSV

Import these files from the `data/` folder:

- customers.csv
- accounts.csv
- transactions.csv
- loans.csv
- branches.csv
- products.csv
- risk_flags.csv
- calendar.csv

## Step 3 — Check data types

In Power Query, set:

- Date columns as Date
- Amount, balance, fee, and rate columns as Decimal Number
- Count columns as Whole Number
- TRUE/FALSE columns as True/False
- ID columns as Text

## Step 4 — Create relationships

Go to Model view and create the relationships listed in `docs/relationships.md`.

## Step 5 — Create DAX measures

Create a new table called `Measures`.

Then add the DAX measures from `docs/dax_measures.md`.

## Step 6 — Build dashboard pages

Create these pages:

1. Executive Financial Overview
2. Risk and Control Monitoring
3. Customer and Product Analysis
4. Branch Performance

## Step 7 — Export screenshots

After building the dashboard, export screenshots and save them in the `screenshots/` folder.

Suggested names:

- executive_overview.png
- risk_monitoring.png
- customer_product_analysis.png
- branch_performance.png

## Step 8 — Upload to GitHub

Upload:

- data/
- docs/
- screenshots/
- README.md
- Banking_Risk_Financial_KPI_Dashboard.pbix

Do not upload private or real banking data.
