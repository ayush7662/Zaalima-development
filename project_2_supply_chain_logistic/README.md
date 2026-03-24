📦 Supply Chain Analytics using PySpark
🚀 Overview

This project analyzes supply chain data using PySpark to extract insights on delivery performance, delays, sales, and profitability. It demonstrates scalable big data processing and SQL-based analytics.

🎯 Key Features
Big data processing using PySpark
SQL-based analytics
Delivery delay analysis
Late delivery risk evaluation
Category-wise sales and profit analysis
Demand trend analysis
🛠️ Tech Stack
Python
PySpark (Apache Spark)
Spark SQL
Pandas
📂 Dataset

File used: DataCoSupplyChainDataset.csv

Includes:

Shipping details
Customer data
Sales and profit
Delivery status
⚙️ Workflow
1. Initialize Spark Session
from pyspark.sql import SparkSession

spark = SparkSession.builder \
    .appName("SupplyChain_BigData_Analytics") \
    .getOrCreate()
2. Load Dataset
supply = spark.read.csv(
    "DataCoSupplyChainDataset.csv",
    header=True,
    inferSchema=True
)
3. Data Cleaning
Selected important columns
Renamed columns for clarity
📊 Analysis Performed
Delay Analysis

Difference between actual and scheduled shipping days

Delivery Performance

Order count by delivery status

Late Delivery Risk

Identify risk-prone deliveries

Category Sales & Profit

Analyze business performance

Demand Trend

Daily sales trends

📁 Output Files
category_sales_summary.csv
delivery_performance_summary.csv
demand_trend_summary.csv
💡 Key Insights
Delivery delays impact performance
High-performing categories identified
Risk detection improves planning
Trends help in forecasting
🔮 Future Improvements
Add machine learning models
Build dashboards (Power BI / Tableau)
Real-time analytics
Customer segmentation
👨‍💻 Author

Ayush Raj
