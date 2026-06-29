# 🛍️ Customer  Behavior Analysis

> End-to-end Data Analytics project analyzing customer purchasing patterns, revenue trends, customer segments, and subscription behavior using Python, SQL, Power BI, and Gamma AI.

![Python](https://img.shields.io/badge/Python-EDA%20%26%20Cleaning-blue)
![PostgreSQL](https://img.shields.io/badge/SQL-PostgreSQL%20%7C%20MySQL%20%7C%20SQL%20Server-green)
![PowerBI](https://img.shields.io/badge/Visualization-Power%20BI-yellow)
![Gamma](https://img.shields.io/badge/Presentation-Gamma%20AI-purple)

---

![Customer Behavior Dashboard](https://github.com/pajjuri-saiteja/customer_behavior_analysis/blob/421f3db2995bc4688194b024ada5c110baac4f57/cus%20das%20pic.png)


# 📌 Project Overview

This project explores customer shopping behavior to uncover insights related to purchasing patterns, demographics, product preferences, subscriptions, discounts, and revenue generation.

The complete analytics workflow includes:

- Data loading and preprocessing in Python
- Exploratory Data Analysis (EDA)
- Data cleaning and feature engineering
- Database implementation using SQL
- Business analysis through SQL queries
- Interactive dashboard development in Power BI
- Business report preparation
- Presentation creation using Gamma AI
- Professional documentation and version control using GitHub

The objective is to transform raw customer data into actionable business insights that support data-driven decision-making.


![Project Overview](https://github.com/pajjuri-saiteja/customer_behavior_analysis/blob/421f3db2995bc4688194b024ada5c110baac4f57/ChatGPT%20Image%20Jun%2030%2C%202026%2C%2003_06_03%20AM.png)

---

# 🎯 Business Problem

A retail company wants to understand customer behavior to improve:

- Customer engagement
- Revenue growth
- Marketing effectiveness
- Product positioning
- Customer retention
- Subscription adoption

The analysis focuses on identifying trends across demographics, categories, discounts, ratings, shipping methods, and purchasing habits.

---

# 📂 Dataset Information

| Attribute | Details |
|-----------|-----------|
| Dataset | Customer Shopping Behavior Dataset |
| Total Records | 3,900 |
| Features | 18 |
| Missing Values | 37 (Review Rating) |
| Average Purchase | ₹59.76 |
| Average Review Rating | 3.75 |

### Key Columns

- Customer ID
- Gender
- Age
- Category
- Item Purchased
- Purchase Amount
- Review Rating
- Subscription Status
- Shipping Type
- Payment Method
- Discount Applied
- Promo Code Used
- Frequency of Purchases
- Season
- Location

---

# 🛠️ Tools & Technologies

| Category | Tools |
|-----------|---------|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Database | PostgreSQL / MySQL / SQL Server |
| Query Language | SQL |
| Dashboarding | Power BI |
| Reporting | Microsoft Word / PDF |
| Presentation | Gamma AI |
| Version Control | Git & GitHub |

---

# 🔄 Project Workflow

```text
Business Problem
        ↓
Python Data Loading
        ↓
EDA & Data Cleaning
        ↓
Feature Engineering
        ↓
Load Data to SQL Database
        ↓
Business Analysis Using SQL
        ↓
Power BI Dashboard Development
        ↓
Project Report Creation
        ↓
Presentation Using Gamma AI
        ↓
GitHub Repository Deployment
```

---

# 🐍 Step 1: Data Preparation & EDA (Python)

### Tasks Performed

- Imported CSV dataset
- Performed Exploratory Data Analysis (EDA)
- Checked missing values
- Handled null records using median imputation
- Standardized column names using snake_case
- Removed redundant columns
- Created derived features:
  - Age Groups
  - Purchase Frequency Metrics
- Exported cleaned data to SQL database

### Key Python Libraries

```python
pandas
numpy
matplotlib
seaborn
sqlalchemy
psycopg2
```

---

# 🗄️ Step 2: SQL Analysis

The cleaned dataset was loaded into:

- PostgreSQL
- MySQL
- SQL Server

Business questions were answered using SQL queries.

### Example Analysis Areas

- Revenue by category
- Revenue by gender
- Subscription vs non-subscription customers
- Customer segmentation
- Top-selling products
- Discount effectiveness
- Shipping performance
- Customer loyalty analysis

### Sample SQL Query

```sql
SELECT
    category,
    SUM(purchase_amount) AS revenue
FROM customer_behavior
GROUP BY category
ORDER BY revenue DESC;
```

---

# 📊 Step 3: Power BI Dashboard

The Power BI dashboard provides interactive insights into customer behavior.

### Dashboard Features

✅ Subscription filters

✅ Gender filters

✅ Category filters

✅ Shipping type filters

✅ Revenue analysis

✅ Customer segmentation

✅ Age group analysis

✅ Sales trends

### Key Metrics

| Metric | Value |
|----------|---------|
| Customers | 3.9K |
| Average Purchase | ₹59.76 |
| Average Rating | 3.75 |
| Subscribers | 27% |
| Non-Subscribers | 73% |

### Dashboard Insights

- Clothing generated the highest revenue.
- Young adults contributed the most sales.
- Male customers generated significantly higher revenue.
- Express shipping showed stronger average purchases.
- Loyal customers represented the largest customer segment.

---

# 📈 Key Findings & Results

## Revenue Analysis

- Male customers generated nearly 2× more revenue than female customers.
- Clothing was the top-performing category.
- Young adults were the highest-spending demographic.

## Subscription Insights

- 73% of customers were non-subscribers.
- Subscriber spending was similar to non-subscribers.
- Opportunity exists to increase subscription adoption.

## Customer Segmentation

| Segment | Customers | Percentage |
|----------|------------|-------------|
| Loyal | 3,116 | 80% |
| Returning | 701 | 18% |
| New | 83 | 2% |

## Product Insights

Top-rated products:

- Gloves
- Sandals
- Boots
- Hats
- Skirts

Most discounted products:

- Hats
- Sneakers
- Coats
- Sweaters
- Pants

---

# 💡 Business Recommendations

### 1. Increase Subscription Adoption

Provide:

- Exclusive discounts
- Early-access sales
- Loyalty benefits

### 2. Strengthen Loyalty Programs

Reward repeat customers through:

- Membership tiers
- Cashback programs
- Personalized offers

### 3. Optimize Discount Strategies

Balance:

- Revenue growth
- Profit margins
- Customer retention

### 4. Target High-Value Customer Segments

Focus marketing campaigns on:

- Young adults
- Loyal customers
- Express shipping users

### 5. Improve Product Positioning

Promote:

- Best-selling products
- Highest-rated categories
- Seasonal purchasing trends

---

# 📄 Project Deliverables

```text
├── dataset/
│   └── customer_shopping_behavior.csv
│
├── python/
│   ├── eda.ipynb
│   └── data_cleaning.py
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── customer_behavior_dashboard.pbix
│
├── reports/
│   └── business_report.pdf
│
├── presentation/
│   └── gamma_presentation.pptx
│
└── README.md
```

---

# 🚀 How to Run This Project

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/customer-shopping-behavior-analysis.git
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run Python Analysis

```bash
python data_cleaning.py
```

### 6. Load Data into Database

```sql
CREATE DATABASE customer_behavior;
```

Import the cleaned dataset into:

- PostgreSQL
- MySQL
- SQL Server

### 7. Execute SQL Queries

Run:

```bash
analysis_queries.sql
```

### 8. Open Power BI Dashboard

```text
Customer Behavior Dashboard.pbix
```

### 9. Review Report & Presentation

- Business Report (PDF)
- Gamma AI Presentation (PPT)

---

# 📌 Future Improvements

- Customer lifetime value prediction
- Market basket analysis
- Recommendation systems
- Customer churn prediction
- Machine learning segmentation
- Automated Power BI refresh pipelines

---

# 👨‍💻 Author

**Saiteja Pajjuri**

B.Tech — Artificial Intelligence & Data Science

Passionate about Data Analytics, Business Intelligence, SQL, Python, and Power BI.

GitHub: https://github.com/pajjuri-saiteja

LinkedIn: https://www.linkedin.com/in/saiteja-pajjuri-544b78245?utm_source=share_via&utm_content=profile&utm_medium=member_ios

---

⭐ If you found this project useful, consider giving the repository a star!
