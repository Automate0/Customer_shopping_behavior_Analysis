This project represents a complete, industry standard, end-to-end data analytics workflow, designed to mirror the real responsibilities of professional analysts in modern business environments. The project encompasses all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.

This project is perfect for:

📊 Data Analyst aspirants who want to build a strong Portfolio Project for interviews and LinkedIn
📚 Anyone learning Python, SQL, and Power BI
💼 Professionals preparing for interviews in Data Analytics, Data Science or Product Analytics roles

# Customer_shopping_behavior_Analysis
Analysis on customer shopping behavior 
Problem Statement: A leading retail company wants to better undertsnad its customers shpping behavior in order to improve sales, customer satisfaction and long term loyalty. The management team has noticed changes in purchasing patterns across demographics product categories and sales channels (online vs offline). They are particularly interested in uncovering which factors such as discounts, reviews, seasons or payment preferences, drive consumer (behavior) decisions and repeat purchases

Task: To analyze the companys consumer behavior dataset to answer the following business question:
"How can the company leverage consumer shopping data to identify trends, improve customer engagement and optimize marketing and product strategies."
What was done:
 1. Business Porblem / Imported data into Python)
 2. Data Modelling & EDA in Python / then, Load to PSQL database)
 3. Connect to a database in AWS for security
 4. Data Analysis in PSQL / then, connect with PowerBI
 5. Interactive Dashboard using PowerBI / Summarize findings
 6. Project Report / present findings
 7. PowerPoint / Upload project files on Github
 8. Create GitHub repository

DataSet:
Using Jupyter notebook from google collab
Open the file: Customer_Shopping_Behaviour_Analysis.ipynb
The file contains us:
Importing pandas
To get the first 5 rows
Over-all structure
Combined statistics of all numerical column
Categorical columns
Replace missing values with mean or median? we should choose median over mean as mean could be affected by outliers but median is robust to outliers, getting the median by categories and filling the values in the null values in their respective category.
Note: You should use snake casing for the column header's as it would be easier to reference while coding and we wont have to worry about the casing.
Get the column names in snake casing (i.e. all lowercase with _)
displaying the column to check
create a new column
create a column with 4 age group young-adults, Adults, Middle-aged, Senior that splits the ages into 4 equal size groups based on the data distribution and assigns the labels we defined.
check the first 10 rows of new column created
create a column for purchase_frequency_days. converting the textual frequencies into numbers
convert text into numbers for analysis
check the first 10 rows
find out how many had discount and how many had promo_code_used. all matched ( meaning we dont need 2 columns showing the same thing we can drop one)
drop the column promo_code

Connecting to AWS Aurora PostgreSQL for extra security to have a log of who uses the dataset or tampers with it
Load dataframe into PostgreSQL



 


DataSource:





How to Use This Project
Clone the repository

cd customer-trends-data-analysis-SQL-Python-PowerBI
Open Customer_Shopping_Behavior_Analysis.ipynb notebook

This file contains:

Data Import

Data exploration

Data cleaning

Connection to SQL Database

Load the data from Python notebook into MySQL/PostgreSQL/MS SQL Server

Create a database in SQL

Run Python code to load data into SQL database

Open customer_behavior_sql_queries.sql

Answer Business Questions using SQL Queries

Connect the SQL Database to Power BI

Open customer_behavior_dashboard.pbix

Create interactive dashboard in Power BI

Create Project Report and Presentation



📜 License
MIT — feel free to fork, star, and use in your portfolio.
