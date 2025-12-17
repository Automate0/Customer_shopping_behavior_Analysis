# Customer Shopping Behavior Analysis

This project demonstrates a **complete, industry-standard end-to-end data analytics workflow**, closely reflecting the real responsibilities of a professional **Data Analyst**. It covers the full data lifecycle — from **data processing and cloud storage** to **SQL-driven analysis** and **business-ready visualization**.

---

## 🎯 Who This Project Is For

* 📊 **Aspiring Data Analysts** building strong portfolio projects for interviews & LinkedIn
* 📚 **Learners** practicing Python, SQL, Power BI, and Cloud Databases
* 💼 **Professionals** preparing for Data Analytics, Data Science, or Product Analytics roles

---

## 🧩 Project Objective

The goal of this project is to:

* Understand customer purchasing behavior
* Clean and transform raw data
* Store curated data in a cloud database
* Answer real-world business questions using SQL
* Deliver insights through interactive dashboards
* Communicate findings in a clear, stakeholder-friendly format

---

## 🛠️ Tech Stack

* **Python** (Pandas, NumPy, SQLAlchemy)
* **Google Colab**
* **AWS Aurora PostgreSQL**
* **SQL & pgAdmin 4**
* **Power BI Desktop**
* **GitHub**

---

## 🚀 Project Architecture – 4 Core Phases

This project is structured into **four clear phases**, mirroring a real-world analytics pipeline.

---

## 1️⃣ Data Processing (Google Colab – Python)

### Purpose

Clean, explore, and transform raw customer data in a cloud-based environment.

### Steps

* Load the dataset using:

  ```python
  pandas.read_csv()
  ```

* Inspect schema and data quality using:

  * `.head()`
  * `.info()`
  * `.describe()`

* Perform Exploratory Data Analysis (EDA):

  * Customer demographics
  * Purchase amount distributions
  * Category-level trends
  * Discount vs non-discount spending

* Clean and transform data:

  * Handle missing values
  * Convert data types
  * Standardize categorical values
  * Remove duplicates

### 📌 Outcome

A **clean, analysis-ready dataset** prepared for cloud storage.

---

## 2️⃣ Data Storage (AWS Aurora PostgreSQL)

### Purpose

Persist curated data in a **scalable, production-grade cloud database**.

### Steps

* Create an **AWS Aurora PostgreSQL** cluster
* Configure **Security Groups** (allow inbound traffic on port `5432`)
* Create a database (e.g. `customer_behavior`)
* Load cleaned data directly from Google Colab using **SQLAlchemy**:

```python
df.to_sql(
    'customer_behavior',
    engine,
    if_exists='replace',
    index=False
)
```

### 📌 Outcome

Reliable, centralized storage of curated analytical data in the cloud.

---

## 3️⃣ Data Analysis (SQL & pgAdmin 4)

### Purpose

Apply business logic and generate insights using SQL.

### Tools

* AWS Aurora PostgreSQL
* pgAdmin 4

### Example Business Questions Answered

* Who are the top-spending customers?
* What is the average purchase value by gender?
* Do discounts increase customer spending?
* Which product categories perform best?
* How much revenue comes from repeat customers?

### 📌 Outcome

**Actionable business insights** derived directly from cloud-hosted data.

---

## 4️⃣ Data Visualization (Power BI Desktop)

### Purpose

Deliver insights through **interactive, business-ready dashboards**.

### Connection Setup

* Power BI Desktop connected to AWS Aurora PostgreSQL
* PostgreSQL **ODBC Driver (psqlODBC)** required

### Dashboard Highlights

* Total revenue & average order value
* Customer segmentation
* Category-wise sales performance
* Discount impact analysis
* Interactive filters for deeper exploration

### 📌 Outcome

Clear, visual **data storytelling** for decision-makers.

---

## 📊 Key Insights Generated

* Discounted purchases show higher average spending
* A small customer segment drives a large share of revenue
* Product category preferences vary by demographic
* Repeat customers contribute significantly to total sales

---

## 🧠 Skills Demonstrated

* Cloud-based data processing (Google Colab)
* Data cleaning & EDA (Python, Pandas)
* Cloud database management (AWS Aurora PostgreSQL)
* SQL analytics & business logic
* pgAdmin database administration
* Power BI dashboarding
* End-to-end data pipeline design

---

## ⚠️ Common Errors & Solutions

### ❌ Invalid SSL / Certificate Error (Power BI ↔ PostgreSQL)

**Issue:**
Power BI fails to connect due to certificate validation.

**Solution:**

* Download the PostgreSQL root certificate
* Place it in the correct directory:

**Windows:**

```text
C:\Users\<username>\AppData\Roaming\postgresql\root.crt
```

* Restart Power BI

---

### ❌ ODBC Driver Not Found

**Issue:**
Power BI cannot detect the PostgreSQL database.

**Solution:**

* Install the PostgreSQL ODBC (**psqlODBC**) driver
* Ensure the driver version matches your PostgreSQL setup
* Restart Power BI

---

### ❌ Connection Timeout

**Issue:**
Power BI or pgAdmin cannot reach AWS Aurora.

**Solution:**

* Check AWS Security Group inbound rules
* Ensure port `5432` is open
* Verify public accessibility or VPN configuration

---

### ❌ Authentication Failed

**Issue:**
Incorrect username or password.

**Solution:**

* Double-check credentials
* Ensure the database user has sufficient privileges
* Confirm the correct database name is used

---

## 🔗 Useful Links

* Pandas Documentation:
  [https://pandas.pydata.org/docs/](https://pandas.pydata.org/docs/)

* AWS Aurora PostgreSQL:
  [https://docs.aws.amazon.com/aurora/](https://docs.aws.amazon.com/aurora/)

* pgAdmin 4:
  [https://www.pgadmin.org/docs/](https://www.pgadmin.org/docs/)

* Power BI:
  [https://learn.microsoft.com/power-bi/](https://learn.microsoft.com/power-bi/)

* PostgreSQL ODBC Driver (psqlODBC):
  [https://www.postgresql.org/ftp/odbc/versions/](https://www.postgresql.org/ftp/odbc/versions/)

---

## 🤝 Connect & Feedback

If you found this project useful:

* ⭐ Star the repository
* 🍴 Fork it
* 💬 Share feedback or suggestions

Happy Analyzing! 📈
