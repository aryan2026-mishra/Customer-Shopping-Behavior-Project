# Customer Shopping Behaviour Analysis Project

A comprehensive data analysis project exploring customer shopping behavior patterns using **Python EDA**, **SQL queries**, and **Power BI dashboards**.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Business Objectives](#business-objectives)
- [Project Structure](#project-structure)
- [Tools & Technologies](#tools--technologies)
- [Installation & Setup](#installation--setup)
- [Project Workflow](#project-workflow)
- [Key Findings](#key-findings)
- [Files Description](#files-description)
- [How to Use](#how-to-use)
- [Git Commands](#git-commands)
- [Contact](#contact)

## 🎯 Project Overview

This project performs an in-depth analysis of customer shopping behavior to extract actionable business insights. The analysis pipeline includes:

1. **Exploratory Data Analysis (EDA)** - Using Python and Pandas
2. **SQL Analysis** - Advanced queries for data insights
3. **Data Visualization** - Interactive Power BI dashboard

The project answers 11 key business questions about customer demographics, purchasing patterns, seasonal trends, payment preferences, and promotional effectiveness.

## 🎖️ Business Objectives

The analysis addresses the following key business questions:

1. **Popular Products** - Identify the most popular product categories and items driving sales
2. **Demographic Influence** - Analyze how age, gender, and location affect purchasing behavior
3. **Promotional Impact** - Measure the effectiveness of discounts and promo codes on revenue
4. **Subscription Analysis** - Examine the relationship between subscription status and purchase frequency
5. **Payment Trends** - Evaluate payment method preferences and seasonal sales trends
6. **Top Categories** - Retrieve the top 5 best-selling product categories
7. **Gender Spending** - Compare average purchase amounts across gender demographics
8. **Promo Code Anomalies** - Identify customers using promo codes but not applying discounts
9. **Seasonal Patterns** - Determine which season drives the highest average purchase amounts
10. **Payment Methods** - Understand customer payment preferences
11. **Loyal Customers** - Identify high-value customers with 5+ previous purchases and ratings >4.5

## 🛠️ Tools & Technologies

### **Python Libraries (Jupyter Notebook)**
- **Pandas** - Data manipulation and aggregation
- **NumPy** - Numerical computations
- **Matplotlib** - Static visualizations
- **Seaborn** - Advanced data visualizations

### **Database & SQL**
- **MySQL** - Database management
- **SQL Queries** - Complex data analysis and filtering

### **Visualization**
- **Power BI** - Interactive dashboards and business intelligence

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.7+ (for Jupyter notebook)
- MySQL Server (for SQL queries)
- Power BI Desktop (for dashboard visualization)
- Jupyter Notebook or JupyterLab

### Step 1: Clone Repository
```bash
git clone https://github.com/yourusername/Customer_Shopping_Behaviour_Analysis.git
cd Customer_Shopping_Behaviour_Analysis
```

### Step 2: Create Virtual Environment
```bash
python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Run Jupyter Notebook
```bash
jupyter notebook notebooks/Customer_Shopping_Behaviour.ipynb
```

### Step 5: Set Up SQL Database
1. Open your MySQL client
2. Create a database named `Market`
3. Import the SQL script:
```bash
mysql -u root -p Market < sql/Customer_Shopping_Behaviour_Analysis_Project.sql
```

### Step 6: Open Power BI Dashboard
1. Open Power BI Desktop
2. Load `dashboards/Customer_Shopping_Dashboard.pbix`
3. Refresh data connections if needed

## 🔄 Project Workflow

### Phase 1: Data Exploration (Python - Jupyter)
- Load customer shopping data from CSV using Pandas
- Check data types, missing values, and duplicates
- Generate descriptive statistics
- Explore distributions and relationships
- Create exploratory visualizations

### Phase 2: Data Analysis (SQL)
- Clean and standardize column names
- Execute 12 analytical queries covering:
  - Product popularity analysis
  - Demographic insights
  - Promotional impact assessment
  - Seasonal trends
  - Payment method preferences
  - Customer loyalty metrics

### Phase 3: Dashboard Creation (Power BI)
- Create interactive visualizations
- Build KPI cards and performance metrics
- Enable data filtering and drill-down capabilities
- Design user-friendly dashboard layout

## 💡 Key Findings

The analysis reveals insights about:
- **Most Popular Categories** - Top-selling product categories
- **Seasonal Trends** - Highest revenue and purchase seasons
- **Demographic Patterns** - Customer behavior by age, gender, and location
- **Promotional Effectiveness** - Impact of discounts and promo codes on sales
- **Payment Preferences** - Most used payment methods
- **Customer Loyalty** - Segments of loyal and high-value customers
- **Average Spending** - Differences in spending habits across demographics

*See Power BI dashboard for detailed visualizations of these findings.*

## 📄 Files Description

### Jupyter Notebook
**`Customer_Shopping_Behaviour.ipynb`**
- Loads and explores the shopping behavior dataset
- Performs EDA with statistical analysis
- Creates exploratory visualizations
- Identifies data patterns and anomalies
- Data cleaning and preparation

### SQL Script
**`Customer_Shopping_Behaviour_Analysis_Project.sql`**
- 12 sophisticated SQL queries
- Data validation and cleaning operations
- Analyzes customer segments and spending patterns
- Identifies temporal and demographic trends
- Insights on payment methods and seasonal patterns

### Power BI Dashboard
**`Customer_Shopping_Dashboard.pbix`**
- Interactive dashboard with multiple visualizations
- Visual KPIs and performance metrics
- Filterable charts and drill-down capabilities
- Real-time data representation
- Customer behavior insights

### Problem Statement
**`Customer_Shopping_Behaviour_Analysis_Problem_Statement.pdf`**
- Detailed business requirements
- 11 analytical objectives
- Expected deliverables and metrics

## 🚀 How to Use

### For Data Analysis
1. Open the Jupyter notebook in your browser
2. Run cells sequentially to see the analysis
3. Modify queries and visualizations as needed
4. Add your own analysis and insights

### For SQL Queries
1. Connect to your MySQL database
2. Run queries from the SQL script
3. Modify WHERE clauses and conditions as per requirements
4. Export results for presentations

### For Dashboard Visualization
1. Open Power BI Desktop
2. Load the `.pbix` file
3. Interact with filters and charts
4. Drill down into specific data segments
5. Customize visualizations as needed

## 📊 Dataset Information

**Dataset:** `shopping_behavior_updated.csv`

**Total Attributes:** 18 customer shopping features

**Key Columns:**
- **Customer Info:** Customer ID, Age, Gender, Location
- **Product Details:** Item Purchased, Category, Size, Color
- **Purchase Behavior:** Purchase Amount (USD), Season, Frequency of Purchases
- **Engagement:** Review Rating, Subscription Status
- **Promotions:** Discount Applied, Promo Code Used
- **Transaction:** Payment Method, Shipping Type
- **Loyalty:** Previous Purchases

## 📋 Dependencies
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
jupyterlab>=3.0.0
ipython>=7.0.0
mysql-connector-python>=8.0.0
PyMySQL>=1.0.0
python-dotenv>=0.19.0
openpyxl>=3.6.0

## 🔄 Git Commands - How to Push to GitHub

### Step 1: Create a GitHub Repository
1. Go to https://github.com/aryan2026-mishra
2. Click **"New"** or **"+"** → **"New repository"**
3. Name: `Customer_Shopping_Behaviour_Analysis`
4. Click **"Create repository"** (don't initialize with README)

### Step 2: Push Your Project

**Copy and paste these commands one by one:**
```bash
git init
git add .
git commit -m "Initial commit: Customer Shopping Behaviour Analysis"
git remote add origin https://github.com/YOUR_USERNAME/Customer_Shopping_Behaviour_Analysis.git
git branch -M main
git push -u origin main
```

**Replace `YOUR_USERNAME` with your actual GitHub username!**

### Step 3: For Future Updates
```bash
git add .
git commit -m "Description of changes"
git push origin main
```

## 📝 License

This project is open source and available under the MIT License.

## 👤 Author

**Aryan Mishra**
- Email: [aryanmishra01718@gmail.com](mailto:aryanmishra01718@gmail.com)
 

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

 

For questions or issues:
- Open an issue on GitHub
- Email: aryanmishra01718@gmail.com


pandas>=1.3.0
numpy>=1.21.0
scipy>=1.7.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
jupyterlab>=3.0.0
ipython>=7.0.0
mysql-connector-python>=8.0.0
PyMySQL>=1.0.0
python-dotenv>=0.19.0
openpyxl>=3.6.0

