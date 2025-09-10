# task6_DA
# Sales Data Analysis with SQLite and Python

This project demonstrates how to use **SQLite (built into Python)** with **Pandas** and **Matplotlib** to analyze and visualize sales data.  
No external database setup is required — SQLite is included in Python’s standard library.

---

## 🚀 Features
- Creates a **SQLite database (`sales_data.db`)** with a `sales` table
- Inserts sample sales records (product, quantity, price)
- Runs SQL queries to calculate:
  - Total quantity sold
  - Total revenue per product
- Loads results into **Pandas DataFrame**
- Displays summary results in the console
- Visualizes **Revenue by Product** using a simple bar chart

---

## 🛠 Requirements
- Python 3.x (with built-in `sqlite3`)
- Libraries:
  - `pandas`
  - `matplotlib`

Install dependencies (if not already installed):
```bash
pip install pandas matplotlib

Project Files
create_db.py → Creates sales_data.db and inserts sample data
analyze_sales.py → Runs SQL queries, prints results, and plots a bar chart
sales_data.db → SQLite database file (auto-created after running create_db.py)


How to Run
1. Create the database
python create_db.py
This will generate sales_data.db with sample sales records.
2. Analyze and visualize sales
python analyze_sales.py
This will:
Print a sales summary table:
product  total_qty  revenue
Pen            30      150
Book           30      450
Bag            10      700
Show a bar chart of Revenue by Product
Save the chart as sales_chart.png

📊 Example Output
Console Output:
Sales Summary:

  product  total_qty  revenue
0     Pen         30      150
1    Book         30      450
2     Bag         10      700
Bar Chart:
A bar chart displaying revenue for Pen, Book, and Bag.
