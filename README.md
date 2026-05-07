# B&J GROCERIES-DASHBOARD
![](SBS.jpg)
Interactive Excel dashboard for B&amp;J Groceries to track sales, revenue, profit, and customer behavior across products, locations, and payment methods. Built with cleaned data, SUMIFS, INDEX/MATCH, and KPIs, it delivers reusable, data-driven insights with slicers, cards, and ranking visuals.
## Project summary & key insights
- **Purpose**: Provide a single-pane-of-glass view for sales, revenue, cost, and profit across channels and customer segments.
- **Audience**: Sales managers, finance teams, operations lead, and executives who need quick insights and drill-down capability.
- **Outcome**: The dashboard highlights top-performing products, top customers, most profitable locations, payment-method distribution, and demographic revenue splits — enabling targeted marketing, pricing, and inventory decisions.

 
**Example top-line insight (from the dashboard): The 60-74 age group and Chicago location are among the highest contributors to revenue, while Shortbread is a top profitable brand.**
## Quick demo / preview
Here is the snapshot of the dashboard
![](Dashboard1.png)
Click here to interact with the dashboard: [here](B$J_Biscuit_Dashboard1.xlsm)
## Key performance indicators (KPIs) and Cards
Each KPI is implemented as a live cell (card) that reads from the clean data/Pivot/measure.
- Quantity Sold
- Total COGS-Meaning Total Cost of Goods Sold
- Total Profit
- %Profit Margin
- Profitable Brand
- Profitable Location
- Profitable Customer
- Top Salesperson
- Profitable Age Group
## Slicers includes
- Location
- Age Group
## Data — raw & clean
**Raw Data**                               
original transaction data.
![](Raw_data.png) 
[Downloadhere](Raw_Data.xlsx)

**Cleaned Data**
cleaned and enriched dataset for the dashboard.
![](Cleaned_data.png)
[Downloadhere](Cleaned_data.xlsm)

## How I Produced the Cleaned Data
- **Imported raw CSV**: Brought sales_transactions_raw.csv into Excel using Power Query for a repeatable process.
- **Defined column types**: Set correct data types (Date, Text, Whole Number, Decimal) to prevent calculation errors.
- **Removed duplicates**: Checked for duplicate TransactionID (or Date + TransactionID) and eliminated exact repeats.
- **Standardized text**: Trimmed spaces and unified capitalization for ProductName, Category, City, and PaymentMethod.
- **Handled missing values**: Defaulted missing Quantity to 1 or flagged rows; imputed or flagged missing UnitPrice/UnitCost.
- **Created derived fields**: Calculated Revenue, COGS, Profit, and ProfitMargin for each row.
- **Built lookup tables**: Added master tables for Products, Cities, and Customers to support consistency and enrich analysis.
- **Generated buckets**: Grouped Age into ranges (e.g., 15–29, 30–44) and created price tiers for better slicing.
- **Validated totals**: Reconciled aggregate totals (Revenue, Quantity) with the source system to confirm accuracy.
- **Exported clean file** 

## Formulas, Functions & Techniques Used
The dashboard combines classic Excel formulas, modern functions, and Power Query transformations to ensure both flexibility and repeatability.
### Key Functions Applied:
- Aggregate & Conditional: SUMIFS, COUNTIFS, AVERAGEIFS
- Lookups: VLOOKUP, INDEX, MATCH, XLOOKUP
- Logic & Error Handling: IF, IFS, IFERROR
- Ranking & Sorting: LARGE, SMALL
- Text Manipulation: TEXT, CONCATENATE, TEXTJOIN
- Rounding & Date Math: ROUND, ROUNDUP, ROUNDDOWN, YEAR, MONTH, EOMONTH, DATE
- Dynamic Arrays (Excel 365): FILTER, SORT

## Insights from the Dashboard
### Profitable Segments
- Most profitable brand: Shortbread.
- Most profitable location: Chicago.
- Most profitable customer: Robert Hernandez ($445.4k revenue).
- Most profitable salesperson: Travis Doyle.
- Most profitable age group: 60–74.
### Revenue Distribution
- 90% of revenue comes from expensive products.
- Revenue contribution by age is highest among 30–74 age brackets, each generating 14M+ in sales.
- Male customers dominate revenue share (84.4%) compared to female (9.5%) and other (6.1%).
### Payment Methods
- Revenue is evenly distributed across payment methods (Cash, Credit Card, Debit Card, Mobile Payment), each contributing ≈15M.
### Geographic Performance
- San Antonio leads revenue share (7.3M), followed closely by San Jose and Philadelphia (≈6.3M each).
- Chicago, despite being a profitable location, ranks lowest in revenue share (5.7M).

## Informed Decisions
- Product Strategy: Focus more on high-end (expensive) product categories since they drive the bulk of revenue.
- Customer Targeting: Prioritize engagement with middle-aged (30–74) customers, who form the backbone of revenue contribution.
- Salesforce Management: Replicate the strategies of top salesperson Travis Doyle to improve overall team performance.
- Geographic Allocation: Despite Chicago’s profitability, cities like San Antonio and San Jose are stronger in revenue, suggesting different pricing or cost dynamics.
## Recommendations
- Expand High-End Offerings: Increase stock, marketing, and bundling options for expensive products to maintain dominance.
- Engage Female Customers: Female revenue share is low (9.5%); create targeted promotions, discounts, and loyalty programs for this demographic.
- Leverage Top Customers: Strengthen relationships with high-value customers like Robert Hernandez through VIP programs.
- Optimize Regional Pricing: Investigate why Chicago is profitable yet contributes less revenue — adjust pricing or product mix accordingly.
- Empower Sales Reps: Use Travis Doyle’s sales approach as a best-practice benchmark across the sales team.

  ## 👨‍💻 Author
### Folagbade Olatunbosun Samuel
- 💼 LinkedIn:https://www.linkedin.com/in/olatunbosun-folagbade-559151243/
- 📧 Email:Folagbadeolatunbosun@gmail.com










































