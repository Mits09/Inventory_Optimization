# E-Grocery Inventory Management & Optimization (ML + EDA Project)
📌 Project Overview

This project focuses on Inventory Analysis and Optimization for an E-Grocery business using Python, Pandas, Data Analysis, and Machine Learning (K-Means Clustering).

Efficient inventory management is critical in e-commerce as it directly affects:

📊 Operational efficiency

💰 Cost control

📦 Stock availability

😊 Customer satisfaction

The objective of this project is to analyze inventory data, identify trends, segment products, evaluate suppliers, and generate actionable optimization strategies.

🎯 Project Objectives

Data Cleaning & Preparation

Exploratory Data Analysis (EDA)

Inventory Segmentation using K-Means Clustering

ABC Classification Analysis

Supplier Performance Evaluation

Demand Forecasting Comparison

Inventory Optimization Recommendations

🛠️ Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn (KMeans, Silhouette Score)

📂 Dataset Features

The dataset contains inventory-related attributes such as:

SKU_ID

Category

Supplier_Name

Warehouse_ID

Quantity_On_Hand

Quantity_Reserved

Quantity_Committed

Avg_Daily_Sales

Days_of_Inventory

Unit_Cost_USD

Total_Inventory_Value_USD

Received_Date

Expiry_Date

Lead_Time_Days

Safety_Stock

Supplier_OnTime_Pct

Audit_Variance_Pct

ABC_Class

FIFO_FEFO

🔄 Data Preprocessing Steps

✔ Converted date columns to datetime format
✔ Cleaned currency columns (removed $ and commas)
✔ Standardized decimal values
✔ Checked and handled missing values
✔ Validated logical constraints
✔ Removed duplicate SKU records
✔ Encoded categorical features
✔ Created cleaned analysis-ready dataset

📊 Exploratory Data Analysis (EDA)
Key Analysis Performed:

Summary statistics of inventory & cost

Distribution of Quantity_On_Hand (Histogram)

Category vs Inventory Value (Bar Chart)

Top 5 SKUs by inventory value

Stock age calculation

Expiring soon products

Avg_Daily_Sales vs Days_of_Inventory (Scatter plot)

Key Findings:

Inventory distribution is right-skewed (overstock risk for few SKUs)

ABC-A items contribute maximum inventory value

Some SKUs show potential stockout risk

Expiring items identified for proactive clearance

🤖 Inventory Segmentation (K-Means Clustering)
Features Used:

Avg_Daily_Sales

Days_of_Inventory

Quantity_On_Hand

Total_Inventory_Value_USD

Steps:

Feature Scaling (StandardScaler)

KMeans (k=3)

Cluster Assignment

Visualization

Silhouette Score Evaluation

Silhouette Score: ~0.345
→ Indicates moderate cluster separation.

📦 ABC Analysis

Class A: High-value SKUs (strict control required)

Class B: Medium-value SKUs

Class C: Low-value SKUs

ABC-A items dominate inventory value and require tighter monitoring.

📈 Demand Forecasting Analysis

Forecasted 30-day demand = Avg_Daily_Sales × 30

Compared forecast with Quantity_On_Hand

Identified SKUs at stockout risk

🚚 Supplier Performance Analysis

Evaluated Supplier_OnTime_Pct

Identified suppliers with high audit variance

Highlighted performance variability among suppliers

🔍 Key Business Insights

ABC-A items contribute majority of inventory value.

Some SKUs show overstocking while others risk stockouts.

Certain suppliers exhibit high audit variance.

FEFO reduces expiry risk for perishable goods.

📌 Inventory Optimization Recommendations

✔ Implement automated reordering for fast-moving SKUs
✔ Apply FEFO to all perishable products
✔ Improve coordination with underperforming suppliers
✔ Adjust safety stock based on lead time
✔ Improve forecasting models
