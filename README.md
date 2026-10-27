# NovaTrust Bank Performance Analysis

*An individual practice project using a simulated banking dataset.*

## Objective
Analyze NovaTrust Bank's branch, customer, product and transaction data to understand revenue and profitability, and recommend ways to improve performance.

## Tools
PostgreSQL (data cleaning and analysis) • Power BI (dashboard)

## What I did
1. Imported four datasets (Branch, Customer, Product, Transactions) and set up the relationships between them
2. Cleaned the data: removed 15 duplicate customers and 60 duplicate transactions, and fixed inconsistent text
3. Created Revenue and Profitability fields
4. Answered five business questions using SQL
5. Built a Power BI dashboard with KPI cards, five visuals and Region and Product Category slicers

## Dashboard
[Dashboard](dashboard.png)
## Key numbers
- Revenue: ₦15.54M
- Cost: ₦1.74M
- Profit: ₦13.80M
- Transactions: 2,940

## Key findings

1. **Branch performance is very uneven.** Kano Fagge is the top branch (₦1.9M revenue), followed by Kano Bompai and Lagos Surulere. The lowest branch, Abuja Asokoro, earned about ₦50K, roughly 38 times less than the top branch. Revenue is concentrated in a few locations.
2. **Premium and Retail customers bring in the most revenue.** Premium contributes ₦5.4M and Retail ₦3.8M. The Student segment contributes only ₦0.4M.
3. **Volume comes from low-value, high-frequency products.** Mobile Money (686 transactions), POS (589) and ATM Withdrawal (475) dominate. Lending products such as SME Business Loan (35) have very few transactions.
4. **Revenue is volatile.** It rose from ₦0.9M in January to a peak of ₦2.6M in June, then dropped sharply to ₦0.1M in July. Possible causes are seasonality, a system outage, or a data issue, so July needs investigating.
5. **Transactions with fee waivers made much less profit in total** (₦1.81M vs ₦11.99M without waivers). More analysis is needed, such as average profit per transaction, to confirm whether waivers reduce profit.

## Recommendations

1. **Learn from the best branches.** Study what Kano Fagge, Kano Bompai and Lagos Surulere do differently (staffing, marketing, product mix) and apply it in the weakest Abuja and Lagos branches.
2. **Control fee waivers.** Set approval limits or a waiver budget per branch, and track waiver use against profit every month.
3. **Check margins before pushing volume.** Measure the profit on each product line, then promote underused products that earn well, such as savings, fixed deposits and loans.
4. **Decide what the Student segment is for.** Either treat it as a long-term plan to grow future customers, or offer tailored products that raise its contribution.
5. **Investigate July.** Find out what caused the drop, such as an outage, staff shortage or data entry issue, so it can be prevented or corrected.

## Limitations and next steps

- This is a simulated dataset, and the analysis covers one year of data.
- Next steps: compare average profit per transaction for waived and non-waived fees, and check the July transaction count.

## Files
- `NovaTrust Bank Assignment.docx`: full write-up of the process, dashboard explanation, findings and recommendations
- `dashboard.png`: final Power BI dashboard
- `Q1` to `Q5` screenshots: SQL query results for each business question

- ## SQL Analysis

**Q1: Which branch earns the most revenue?**

![Q1](Q1-Top%20branch%20by%20revenue%20.png)

**Q2: Which customer segment earns the most revenue?**

![Q2](Q2-customer-segment%20with%20most%20revenue.png)

**Q3: Which product has the most transactions?**

![Q3](Q3-product%20with%20highest%20transaction.png)

**Q4: How does revenue change over time?**

![Q4](Q4-monthly%20revenue%20over%20time2.png)

**Q5: How do fee waivers affect profitability?**

![Q5](Q5-%20fee-waiver%20and%20profitability.png)
