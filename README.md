# data-pipeline-sales
🔄 Sales Data Pipeline (ETL Project)
📌 Overview

* This project implements an end-to-end ETL pipeline to process retail sales data and store it in a SQL database for analysis.

🧰 Tools & Technologies

* Python (Pandas)

* SQL (SQLite)

* SQLAlchemy

⚙️ Pipeline Process
1. Extract

* Loaded raw CSV dataset into Python

2. Transform

* Cleaned missing values and corrected data types

* Converted date columns into datetime format

* Created derived features such as Year and Profit Margin

3. Load

* Stored processed data into a SQLite database using SQLAlchemy

4. Query

* Executed SQL queries to analyze regional sales performance

🔍 Example Query

SELECT Region, SUM(Sales) as total_sales

FROM sales

GROUP BY Region

ORDER BY total_sales DESC;

📊 Key Insight

*Identified top-performing regions contributing the highest share of total revenue

🚀 Future Improvements

* Automate pipeline scheduling (e.g., Airflow)

* Connect to cloud database (PostgreSQL, AWS RDS)

* Handle streaming data sources
