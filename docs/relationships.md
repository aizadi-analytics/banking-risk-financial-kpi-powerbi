# Power BI Data Model

Create these relationships in Power BI Model view.

## Relationships

1. `customers[customer_id]` → `accounts[customer_id]`
   - One-to-many
   - Single direction

2. `accounts[account_id]` → `transactions[account_id]`
   - One-to-many
   - Single direction

3. `customers[customer_id]` → `loans[customer_id]`
   - One-to-many
   - Single direction

4. `products[product_id]` → `loans[product_id]`
   - One-to-many
   - Single direction

5. `branches[branch_id]` → `accounts[branch_id]`
   - One-to-many
   - Single direction

6. `calendar[date]` → `transactions[transaction_date]`
   - One-to-many
   - Single direction

7. `transactions[transaction_id]` → `risk_flags[transaction_id]`
   - One-to-one or one-to-many depending on import
   - Single direction

## Important note about loans and calendar

You can connect `calendar[date]` to `loans[start_date]`, but keep it inactive if it creates ambiguity. This project can analyze loans mainly by product, customer risk, and status without a date relationship.
