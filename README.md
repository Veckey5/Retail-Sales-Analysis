**RETAIL SALES ANALYSIS (DATABRICKS SQL)**

An end-to-end SQL analysis of a  online retailer's sales data. I built the schema, validated the data, and answered the questions a business team would ask about revenue, customers, and operational losses.

Tools: Databricks SQL, Unity Catalog, Delta tables 
SQL skills: joins (inner, left, anti), aggregations, CTEs, window functions (LAG, RANK, SUM() OVER), CASE segmentation, views, data validation

**BUSINESS PROBLEMS ANSWERED**

The mid-size online retailer wants to know:

1. What drives revenue: which products, categories, and regions?
2. Which customers matter most, and who has gone quiet?
3. How much money is lost to cancelled or returned orders, and to stock-outs?

**DATA STRUCTURE**

The data used here is hypothetical and contains five (5) tables, namely;
1. Categories
2. Products
3. Orders
4. Products
5. Customers
6. Order Items


**DATA VALIDATION**

Before analysis I checked row counts, orphaned foreign keys, duplicate order IDs, valid status values,
and whether the price charged matched the catalog price. All checks passed, with zero mismatches.

**KEY FINDINGS**

1.	A total of $1,779.74 revenue was made from 12 completed orders, with an average order value of $148.31	
2.	Home & Kitchen is the top product category with about 33% of revenue, and next is Electronics with about 26% of the revenue
3.	The Stand Mixer earns the most at $499.98 with only 2 units sold, while the Mystery Novel sells the most units (5) but earns $74.95
4.	Revenue is concentrated and this is evident because only the top 3 customers produce about 68% of total revenue
5.	20% of orders did not complete, putting $399.97 of revenue at risk. This is about 22% on top of what was earned
6.	Bluetooth Speaker is out of stock despite proven demand; the orders details shows that 2 units were sold in a completed order
7.	3 customers have no completed purchase and are a ready-made win-back list
8.	Only 37.5% of buying customers ordered more than once

Revenue swings sharply from month to month. With only 12 orders, a single large order moves the number, so this is directional rather than conclusive.

**RECOMMENDATIONS**

The online retailer will need to do the following:
1. Restock the Bluetooth Speaker and set a reorder alert for any product with recent sales and low stock.
2. Run a win-back campaign for the 3 customers with no completed purchase.
3. Build loyalty offers for the top 3 customers to reduce revenue concentration risk.
4. Investigate cancellations and the returned Espresso Machine order to find out whether the cause is product quality, pricing, or checkout friction.
5. Review Books purchasing as it holds about $7.5K of stock against about $100 of revenue.
