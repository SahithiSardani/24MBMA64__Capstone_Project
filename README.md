# 24MBMA64__Capstone_Project
# Financial Analytics & Predictive Modeling on Bank Loan Data
### An MBA Capstone Project using PySpark and Databricks

This repository contains the complete end-to-end capstone project for the MBA General program. The project leverages a bank's customer loan dataset to solve five distinct business problems through data engineering, exploratory analysis, and predictive modeling, all within the Databricks Lakehouse Platform.

## 🚀 Project Objective
The primary goal of this project is to transform raw customer banking data into actionable business intelligence. By building a robust data pipeline and applying machine learning models, we aim to enhance strategic decision-making in key areas such as risk assessment, customer segmentation, marketing efficiency, and portfolio management.
📊 Five Case Studies Addressed
This project tackles five common challenges in financial analytics:

1.  **MBS Price Prediction (Proxy):** Predicting a customer's potential mortgage value to identify high-value prospects.
2.  **Risk Assessment:** Building a high-accuracy model to predict which customers are likely to accept a personal loan.
3.  **Customer Segmentation:** Grouping customers into distinct personas ("High-Value", "Developing", etc.) for targeted marketing.
4.  **Interest Rate Impact Simulation:** Modeling how economic changes like interest rate hikes could affect loan acceptance rates across the portfolio.
5.  **Drivers of Financial Stability:** Identifying the key customer attributes that indicate low risk and high financial stability.
## 🛠️ Technology Stack

*   **Platform:** Databricks Community Edition
*   **Core Engine:** Apache Spark (via PySpark)
*   **Libraries:**
    *   **Machine Learning:** Spark MLlib
    *   **Data Manipulation:** Spark SQL, Pandas
    *   **Visualization:** Matplotlib, Seaborn, and native Databricks visualizations

## 📁 Repository Structure
This repository contains all the final deliverables for the project:
*   `Bank_Personal_Loan_Modelling.csv`: The raw source data used for the project.
*   `Financial_Analytics_Cases.ipynb`: A step-by-step Databricks notebook detailing the analysis and visualization for each of the five case studies.
*   `Financial_Analytics_Pipeline.ipynb`: The final, production-style data pipeline that implements the Medallion (Bronze, Silver, Gold) architecture to automate the entire workflow.
*   `Financial_Analytics_Presentation.pptx`: A 6-slide summary presentation of the project's methodology, key findings, and business implications.
*   `Project_Walkthrough.mp4`: A screen recording that demonstrates the notebook execution, the final dashboard, and narrates the project's outcomes.
*   `README.md`: This project summary file.
## ⚙️ Methodology: The Medallion Data Pipeline
To ensure data quality and reliability, this project was built using the industry-standard **Medallion Architecture**.
*   **🥉 Bronze Layer:** Raw data was ingested from the source table, column names were cleaned for compatibility, and metadata (like an ingestion timestamp) was added.
*   **🥈 Silver Layer:** The data was transformed into a clean, validated, and trusted "single source of truth." Data quality rules, such as correcting impossible negative values, were applied here. All analysis and ML models were built using this clean Silver table.
*   **🥇 Gold Layer:** The final, business-ready tables were created. Each of the five case studies is powered by a specific Gold table, which contains the final predictions or aggregations needed to create the dashboard visualizations.
