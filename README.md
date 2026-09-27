# 🛍️ Customer Shopping Behavior Analysis

> **An end-to-end retail analytics project combining Python EDA, MySQL, and Power BI to transform customer transaction data into actionable business insights.**

![Python](https://img.shields.io/badge/Python-EDA-blue?logo=python)
![SQL](https://img.shields.io/badge/SQL-MySQL-orange?logo=mysql)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

---

## 📌 Project Overview

Customer Shopping Behavior Analysis is an end-to-end data analytics project designed to understand **how customers purchase, what they purchase, how they respond to promotions, and which customer characteristics are associated with different purchasing patterns**.

The project combines three major analytical layers:

**Python → SQL → Power BI**

* 🐍 **Python** for data exploration, cleaning, statistical analysis, and visualization
* 🗄️ **MySQL** for structured business analysis and analytical querying
* 📊 **Power BI** for interactive reporting and business intelligence

The analysis works with **3,900 customer shopping records containing 18 attributes** covering demographics, products, purchase behavior, promotions, subscriptions, payment methods, shipping, ratings, and previous purchases.

---

## 🎯 Business Problem

Retail businesses generate large amounts of customer transaction data, but raw transaction records alone do not explain:

* Which products and categories drive demand?
* Which customer groups spend more?
* Do promotions influence purchasing?
* How does subscription status relate to purchasing frequency?
* Which payment methods are most frequently used?
* Which seasons generate stronger sales?
* Who are the highly engaged and loyal customers?
* Are there inconsistencies between promo-code usage and applied discounts?

This project converts these questions into **data-driven analytical queries and visual insights**.

---

## 📊 Dataset

### Dataset Size

| Attribute   | Details                        |
| ----------- | ------------------------------ |
| Records     | **3,900**                      |
| Features    | **18**                         |
| Data Type   | Customer shopping transactions |
| Main Domain | Retail / E-commerce            |

### Major Features

| Category        | Variables                             |
| --------------- | ------------------------------------- |
| 👤 Customer     | Customer ID, Age, Gender, Location    |
| 🛒 Product      | Item Purchased, Category, Size, Color |
| 💰 Purchase     | Purchase Amount                       |
| 🌦️ Seasonality | Season                                |
| ⭐ Engagement    | Review Rating                         |
| 🔄 Loyalty      | Previous Purchases                    |
| 🎁 Promotion    | Discount Applied, Promo Code Used     |
| 💳 Payment      | Payment Method                        |
| 📦 Fulfillment  | Shipping Type                         |
| 🔔 Subscription | Subscription Status                   |
| ⏱️ Frequency    | Frequency of Purchases                |

---

# 🧠 Analytical Objectives

The project addresses **12 business-oriented analytical questions**.

### 1. Product Performance

Identify the most frequently purchased products and categories.

### 2. Customer Demographics

Analyze purchasing behavior across:

* Age
* Gender
* Location

### 3. Promotional Impact

Measure sales and transaction patterns based on:

* Discount application
* Promo-code usage

### 4. Subscription Behavior

Study the relationship between subscription status and purchase frequency.

### 5. Payment Preferences

Identify the most frequently used payment methods.

### 6. Seasonal Revenue

Analyze transaction volume and revenue across different seasons.

### 7. Top Revenue-Generating Products

Identify the top products based on total purchase value.

### 8. Gender-Based Spending

Compare average purchase amounts across gender groups.

### 9. Promotion Validation

Identify customers who used promo codes but did not receive an applied discount.

### 10. Seasonal Spending

Determine which seasons have higher average purchase amounts.

### 11. Payment-Based Revenue

Compare transaction counts and total purchase value across payment methods.

### 12. Loyal Customer Identification

Identify customers with:

* More than 5 previous purchases
* Review rating above 4.5

These questions are implemented in the project's SQL analysis.

---

# 🔄 End-to-End Analytics Workflow

```text
                    RAW CUSTOMER DATA
                           │
                           ▼
                  Data Understanding
                           │
                           ▼
                 Python Data Cleaning
                           │
                           ▼
                 Exploratory Data Analysis
                           │
                           ▼
                    MySQL Database
                           │
                           ▼
                  Business SQL Analysis
                           │
                           ▼
                 Power BI Data Modeling
                           │
                           ▼
                Interactive Dashboard
                           │
                           ▼
                Business Insights
```

---

# 🐍 Phase 1 — Python EDA

The Jupyter Notebook is used for the initial analytical layer.

### Activities

* Load customer shopping dataset
* Inspect dataset structure
* Check data types
* Identify missing values
* Check duplicate records
* Generate descriptive statistics
* Analyze customer demographics
* Explore product categories
* Examine purchase distributions
* Analyze seasonal patterns
* Visualize customer behavior
* Identify potential patterns and anomalies

### Libraries

```text
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook
```

---

# 🗄️ Phase 2 — MySQL Analysis

The SQL layer converts business questions into measurable analytical queries.

The project standardizes database columns and performs analytical operations using:

* `GROUP BY`
* `ORDER BY`
* `COUNT()`
* `SUM()`
* `AVG()`
* `CASE`
* Filtering
* Conditional analysis
* Customer segmentation logic

The SQL file contains **12 analytical sections** covering product, customer, promotion, subscription, payment, seasonality, and loyalty analysis.

### Example Business Analysis

```sql
SELECT
    category,
    item_purchased,
    COUNT(*) AS total_purchases
FROM shopping_behaviour
GROUP BY category, item_purchased
ORDER BY total_purchases DESC;
```

This converts raw transaction records into a ranked view of product demand.

---

# 📊 Phase 3 — Power BI Dashboard

The Power BI dashboard provides an interactive business intelligence layer.

### Dashboard Capabilities

* KPI-based reporting
* Customer behavior analysis
* Product performance
* Demographic analysis
* Seasonal analysis
* Payment-method analysis
* Promotion analysis
* Customer loyalty insights
* Interactive filtering
* Drill-down analysis

The repository includes the Power BI `.pbix` dashboard used for visualization.

---

# 💡 Business Insight Areas

The project is designed around several decision-making areas.

### 🛒 Product Intelligence

Understand which products and categories generate the highest purchasing activity.

### 👥 Customer Intelligence

Analyze differences in customer behavior based on demographics and location.

### 🎁 Promotion Intelligence

Evaluate how discounts and promotional codes are associated with purchasing behavior.

### 🔄 Customer Loyalty

Identify customers with stronger historical purchase activity and high ratings.

### 💳 Payment Intelligence

Understand customer payment preferences and transaction distribution.

### 🌦️ Seasonal Intelligence

Identify seasonal differences in transaction activity and purchase value.

---

# 📁 Repository Structure

```text
Customer-Shopping-Behavior-Project/
│
├── Customer Shopping Behaviour.ipynb
│       └── Python EDA & Data Analysis
│
├── Customer Shopping Behaviour Analysis Project.sql
│       └── MySQL Business Analysis
│
├── shopping_behavior_updated.csv
│       └── Customer Shopping Dataset
│
├── Customer Shopping Dashboard.pbix
│       └── Power BI Dashboard
│
├── Customer Shopping Behaviour Analysis Problem Statement.pdf
│       └── Business Requirements
│
├── README.md
│
└── .ipynb_checkpoints/
```

The current repository contains these core project assets.

---

# 🛠️ Technology Stack

| Technology       | Purpose                     |
| ---------------- | --------------------------- |
| Python           | Data analysis               |
| Pandas           | Data manipulation           |
| NumPy            | Numerical operations        |
| Matplotlib       | Visualization               |
| Seaborn          | Statistical visualization   |
| MySQL            | Database & SQL analysis     |
| Power BI         | Dashboard & reporting       |
| Jupyter Notebook | Analytical environment      |
| GitHub           | Version control & portfolio |

---

# 📈 Key Analytical Outcomes

The project produces insights across:

* Product popularity
* Category performance
* Customer demographics
* Average spending
* Promotional activity
* Subscription behavior
* Payment preferences
* Seasonal purchasing
* Customer loyalty
* High-value customer identification

Rather than focusing only on visualization, the project connects **business questions → data analysis → SQL results → dashboard reporting**.

---

# 🚀 How to Run

## 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Customer-Shopping-Behavior-Project
```

## 2. Install Python Dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## 3. Open the Notebook

```bash
jupyter notebook
```

Then open:

```text
Customer Shopping Behaviour.ipynb
```

## 4. Configure MySQL

Create a database:

```sql
CREATE DATABASE Market;
USE Market;
```

Import the customer shopping dataset into the database and execute:

```text
Customer Shopping Behaviour Analysis Project.sql
```

## 5. Open Power BI

Open:

```text
Customer Shopping Dashboard.pbix
```

Refresh the dataset if required.

---

# 🔍 Skills Demonstrated

### Data Analytics

* Exploratory Data Analysis
* Data Cleaning
* Data Validation
* Descriptive Statistics
* Business Question Framing

### SQL

* Aggregation
* Filtering
* Grouping
* Conditional Logic
* Business KPI Analysis
* Customer Segmentation

### Business Intelligence

* Power BI
* Dashboard Development
* KPI Design
* Interactive Filtering
* Business Storytelling

### Business Analysis

* Customer Behavior
* Retail Analytics
* Product Analytics
* Promotion Analytics
* Customer Loyalty
* Payment Analytics

---

# 🚀 Future Improvements

Potential extensions include:

* Customer segmentation using clustering
* Customer lifetime value analysis
* Churn prediction
* Recommendation systems
* Customer propensity modeling
* Sales forecasting
* RFM analysis
* Advanced cohort analysis
* Automated dashboard refresh
* Predictive customer analytics

---

# 👤 Author

**Aryan Mishra**

B.Tech CSE | Data Analytics | Python | SQL | Power BI | Machine Learning

Email: [aryanmishra01718@gmail.com](mailto:aryanmishra01718@gmail.com)

---

## ⭐ Project Objective

The objective of this project is not simply to create charts, but to demonstrate a complete **analyst workflow**:

> **Understand the business problem → clean the data → explore the data → query the data → visualize the results → communicate actionable insights.**

---
