# DAX Measures

Create these measures in Power BI.

## Financial KPIs

```DAX
Total Transaction Volume = SUM(transactions[amount_eur])
```

```DAX
Total Fee Revenue = SUM(transactions[fee_eur])
```

```DAX
Transaction Count = COUNTROWS(transactions)
```

```DAX
Average Transaction Amount = DIVIDE([Total Transaction Volume], [Transaction Count])
```

```DAX
Average Account Balance = AVERAGE(accounts[current_balance])
```

## Customer KPIs

```DAX
Total Customers = DISTINCTCOUNT(customers[customer_id])
```

```DAX
Total Accounts = DISTINCTCOUNT(accounts[account_id])
```

```DAX
Active Accounts =
CALCULATE(
    DISTINCTCOUNT(accounts[account_id]),
    accounts[account_status] = "Active"
)
```

```DAX
High Risk Customers =
CALCULATE(
    DISTINCTCOUNT(customers[customer_id]),
    customers[risk_level] = "High"
)
```

```DAX
High Risk Customer % = DIVIDE([High Risk Customers], [Total Customers])
```

## Risk KPIs

```DAX
Flagged Transactions =
CALCULATE(
    COUNTROWS(transactions),
    transactions[is_flagged] = TRUE()
)
```

```DAX
Flagged Transaction % = DIVIDE([Flagged Transactions], [Transaction Count])
```

```DAX
Critical Risk Flags =
CALCULATE(
    COUNTROWS(risk_flags),
    risk_flags[severity] = "Critical"
)
```

```DAX
Escalated Risk Flags =
CALCULATE(
    COUNTROWS(risk_flags),
    risk_flags[review_status] = "Escalated"
)
```

## Loan KPIs

```DAX
Total Loan Value = SUM(loans[loan_amount_eur])
```

```DAX
Outstanding Loan Balance = SUM(loans[outstanding_balance_eur])
```

```DAX
Defaulted Loans =
CALCULATE(
    COUNTROWS(loans),
    loans[default_flag] = TRUE()
)
```

```DAX
Default Rate = DIVIDE([Defaulted Loans], COUNTROWS(loans))
```

```DAX
Late Payment Loans =
CALCULATE(
    COUNTROWS(loans),
    loans[late_payment_count] > 0
)
```

## Branch KPIs

```DAX
Branches = DISTINCTCOUNT(branches[branch_id])
```

```DAX
Customers per Branch = DIVIDE([Total Customers], [Branches])
```
