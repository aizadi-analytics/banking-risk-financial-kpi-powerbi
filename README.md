# Banking Risk and Financial KPI Dashboard

Power BI portfolio project for banking risk monitoring, financial KPI reporting, loan performance, flagged transaction analysis, and branch-level business intelligence.

## Project objective

This project simulates an internal banking reporting environment. The main business question is:

> How can a bank monitor transaction volume, fee revenue, customer risk, suspicious activity, loan exposure, default rate, and branch/product performance in one Power BI dashboard?

The dataset is synthetic and safe to publish. It does not contain real customer or banking data.

## Target roles

This project is suitable for:

- Data Analyst
- BI Analyst
- Financial Data Analyst
- Risk Reporting Analyst
- Power BI Analyst
- Business Analyst in banking or consulting

## Dataset

The project contains eight CSV files:

- `customers.csv`
- `accounts.csv`
- `transactions.csv`
- `loans.csv`
- `branches.csv`
- `products.csv`
- `risk_flags.csv`
- `calendar.csv`

## Power BI pages

### Page 1 — Executive Financial Overview

KPIs:

- Total Customers
- Total Accounts
- Total Transaction Volume
- Total Fee Revenue
- Average Account Balance
- Total Loan Value
- Outstanding Loan Balance
- Default Rate

Visuals:

- Transaction volume over time
- Fee revenue by transaction type
- Customer count by segment
- Customer count by risk level
- Branch performance table

### Page 2 — Risk and Control Monitoring

KPIs:

- Flagged Transactions
- Flagged Transaction %
- High-Risk Customers
- High-Risk Customer %
- Defaulted Loans
- Late Payment Loans
- Critical Risk Flags

Visuals:

- Flagged transactions by reason
- Flagged transactions by severity
- Risk level by customer segment
- Flagged transaction trend
- Review status breakdown

### Page 3 — Customer and Product Analysis

Visuals:

- Customers by segment
- Average balance by segment
- Loan value by product category
- Default rate by product category
- Transaction behavior by channel

### Page 4 — Branch Performance

Visuals:

- Transaction volume by branch
- Fee revenue by branch
- Flagged transactions by branch
- Customer count by branch
- Branch ranking table

## Recommended slicers

- Date
- Country
- City
- Branch
- Customer segment
- Risk level
- Product category
- Transaction channel
- Transaction type

## Key learning points

This project demonstrates:

- Power BI data modeling
- Fact and dimension table relationships
- DAX measures
- Financial KPI design
- Risk and control monitoring
- Branch and product reporting
- Dashboard storytelling
- Synthetic data documentation

## Limitations

This is a synthetic portfolio project. It is designed for dashboarding and BI practice, not for real credit risk modeling, AML detection, or regulatory reporting.
