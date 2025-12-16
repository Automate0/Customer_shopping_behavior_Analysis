This project represents a complete, industry standard, end-to-end data analytics workflow, designed to mirror the real responsibilities of professional analysts in modern business environments. The project encompasses all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.

This project is perfect for:

📊 Data Analyst aspirants who want to build a strong Portfolio Project for interviews and LinkedIn
📚 Anyone learning Python, SQL, and Power BI
💼 Professionals preparing for interviews in Data Analytics, Data Science or Product Analytics roles

📌 Project Overview

This project aims to:
Understand customer purchasing patterns
Perform data cleaning and transformation
Store and query data using SQL
Answer real-world business questions
Build an interactive Power BI dashboard
Present insights through a structured report

**Tech Stack Used:**
Python (Pandas, NumPy, SQLAlchemy)
Jupyter Notebook
MySQL / PostgreSQL / MS SQL Server
SQL
Power BI
GitHub

🚀 Step-by-Step Project Execution Guide
1️⃣ Clone the Repository

git clone https://github.com/your-username/customer-trends-data-analysis-SQL-Python-PowerBI.git -------------------------------------- Change this
cd customer-trends-data-analysis-SQL-Python-PowerBI

2️⃣ Python Environment – Google Colab
This project uses Google Colab for Python-based analysis.

Steps:
Open Google Colab
Upload or open:
Customer_Shopping_Behavior_Analysis.ipynb
Upload the dataset (customer_shopping_behavior.csv) to Colab

Libraries used:
pandas
numpy
sqlalchemy
psycopg2

📌 Goal: Perform cloud-based data analysis without local setup.

3️⃣ Data Import (Python – Pandas)
Load the dataset using pd.read_csv()
Inspect rows, schema, and statistics

Key methods:
.head()
.info()
.describe()

📌 Goal: Understand dataset structure and data quality.

4️⃣ Data Exploration (EDA)
Exploratory analysis includes:
Customer demographics analysis
Purchase amount distributio
Category-level trends
Discount vs non-discount spending

Techniques used:
GroupBy aggregations
Value counts
Descriptive statistics

📌 Goal: Identify meaningful patterns before transformation.

5️⃣ Data Cleaning & Transformation
Cleaning steps performed in Colab:
Handling missing values
Converting data types
Standardizing categorical values
Removing duplicates

📌 Goal: Prepare analysis-ready data for cloud storage.

6️⃣ Cloud Database Setup – AWS Aurora PostgreSQL
The cleaned dataset is stored in a managed cloud database.

Steps:
Create an AWS Aurora PostgreSQL cluster
Configure security groups (allow PostgreSQL port 5432)
Create a database (e.g. customer_behavior)

📌 Goal: Use a scalable, production-grade cloud database.

7️⃣ Load Cleaned Data from Colab to AWS Aurora PostgreSQL

Using SQLAlchemy, the cleaned Pandas DataFrame is written directly from Colab to Aurora PostgreSQL.

Steps:
Create PostgreSQL connection string
Create SQLAlchemy engine
Load data using .to_sql()

df.to_sql('customer_behavior', engine, if_exists='replace', index=False)

📌 Goal: Persist transformed data in a cloud database.

8️⃣ Database Management with pgAdmin 4

Steps:
Open pgAdmin 4
Register a new server using Aurora endpoint
Verify table creation and schema

📌 Goal: Validate data storage and manage the database.

9️⃣ SQL Analysis – Business Questions

Open: 👉 sql/customer_behavior_sql_queries.sql

SQL queries are executed against AWS Aurora PostgreSQL to answer business questions such as:
1. Top-spending customers
2. Average purchase amount by gender
3. Effect of discounts on spending
4. Most popular product categories
5. Customer repeat behavior

📌 Goal: Translate business requirements into SQL insights.

🔟 Connect AWS Aurora PostgreSQL to Power BI (Online)

This project uses Power BI Service (Online) — no local Power BI Desktop.

Steps:
Open Power BI Service
Use Get Data → PostgreSQL Database
Enter Aurora endpoint and credentials
Configure gateway if required

📌 Goal: Enable cloud-to-cloud data visualization.

1️⃣1️⃣ Power BI Online Dashboard Creation

Dashboard highlights:

Total revenue & average order value
Customer segmentation
Category-wise sales
Discount impact analysis
Interactive filters

📌 Goal: Deliver real-time, business-ready insights.

1️⃣2️⃣ Project Report & Presentation

Final deliverables include:

Executive summary
Data methodology
SQL insights
Dashboard screenshots
Business recommendations

📌 Goal: Communicate insights clearly to stakeholders.

📊 Key Insights Generated

Discounted purchases show higher average spend
A small customer segment drives a large portion of revenue
Product category preferences vary by demographic
Repeat customers significantly impact total sales

🧠 Skills Demonstrated

Cloud-based data analysis (Google Colab)
Data cleaning & EDA (Python, Pandas)
Cloud database management (AWS Aurora PostgreSQL)
SQL analytics
pgAdmin database administration
Power BI Online dashboarding
End-to-end data pipeline design

🔗 Useful Links

Pandas: https://pandas.pydata.org/docs/

AWS Aurora PostgreSQL: https://docs.aws.amazon.com/aurora/

pgAdmin: https://www.pgadmin.org/docs/

Power BI Service: https://learn.microsoft.com/power-bi/


🤝 Connect & Feedback
If you found this project useful:

⭐ Star the repository

🍴 Fork it

💬 Share feedback or suggestions

Happy Analyzing! 📈


