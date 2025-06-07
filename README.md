# Task_7
Basic Sales Summary with SQLite & Python

## Objective
Use SQL inside Python to get total quantity sold and revenue per product, then display results and a bar chart.

## Code Summary
- Connect to `sales_data.db` using `sqlite3`
- Create `sales` table and insert sample data
- Run SQL query with `GROUP BY product` to get totals
- Load results into pandas DataFrame
- Print summary and plot revenue bar chart with matplotlib

## SQL Query Used
```sql
SELECT product, SUM(quantity) AS total_quantity, SUM(quantity * price) AS revenue
FROM sales
GROUP BY product

Explanation
GROUP BY groups sales by product

Revenue calculated as sum of (quantity × price)

Visualization shows revenue per product

Combining SQL and Python allows easy data analysis and plotting

Files
Task_7_Sales_Summary.ipynb

sales_data.db

sales_chart.png
