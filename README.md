# Task7_Analysis_-Python-SQLite
🧾 Analyzing Sales Data with Just Python + SQLite

 In my task 7, I built a basic Sales Summary tool using:
 🔧 Tools Used
 Python (sqlite3, pandas, matplotlib)
 SQLite (fully built-in, no setup!)
 Jupyter Notebook for code + visuals

  
📊 What It Does:
✅ Connects to a local SQLite database (sales_data.db)
✅ Runs a SQL query to calculate:
  • Total quantity sold per product
  • Total revenue per product
✅  - Prints a summary DataFrame
✅ Displays the output with a clean bar chart using Matplotlib



💡 Key Learnings:
✅ How to embed SQL inside Python
✅ Load query results directly into pandas
✅ Quick data visualization with no extra tools
✅ Perfect for small apps, local tools & quick insights


📌 SQL Query Used

```sql
SELECT product, 
       SUM(quantity) AS total_qty, 
       SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product
