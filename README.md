# TASK-7 Basic Sales Summary using SQLite and Python

This project demonstrates how to use SQL within Python to analyze a small sales dataset using **SQLite**, **pandas**, and **matplotlib**. It covers basic SQL querying, data summarization, and visualization.

# Objective

- Connect to a SQLite database (`sales_data.db`)
- Run SQL queries to get:
  - Total quantity sold per product
  - Total revenue (quantity × price) per product
- Display the results using `print()` and a bar chart

# Tools & Libraries Used

- Python 3.x
- SQLite3
- pandas
- matplotlib
- Jupyter Notebook / .py file

# SQL Query Used

sql
SELECT 
    product, 
    SUM(quantity) AS total_qty, 
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
