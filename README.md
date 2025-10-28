

---

# 🛍️ Customer Shopping Behavior Analysis

## 📘 Overview

This data analytics project investigates **customer shopping behavior** using transactional data from **3,900 purchases** across multiple product categories.
The goal is to uncover insights into **spending patterns, customer segmentation, product preferences, and subscription behaviors** to support **data-driven marketing and product strategies**.

**Key Business Question:**

> “How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?”

---

## 📂 Datasets

**Source:** POS (Point of Sales) System
**File:** `customer_shopping_behavior.csv`
**Rows:** 3,900 | **Columns:** 18

**Key Features:**

* **Customer Demographics:** age, gender, location, subscription status
* **Purchase Details:** item purchased, category, purchase amount, size, color, season
* **Behavioral Data:** discount applied, previous purchases, frequency, review rating, shipping type

**Data Quality Summary:**

* Missing Values: 37 (in review ratings)
* Data Types: Float64 (1), Int64 (4), Object (13)
* Cleaned and standardized to ensure consistency

---

## 🧰 Tools & Technologies

| Category                    | Tools Used                    |
| --------------------------- | ----------------------------- |
| Data Handling               | Python (pandas, numpy), Excel |
| Data Exploration & Cleaning | Jupyter Notebook              |
| Database Management         | SQLite                        |
| Querying & Analysis         | SQL                           |
| Data Visualization          | Tableau                       |
| Documentation & Reporting   | PowerPoint, Word / PDF        |

---

## 🔍 Project Steps

### 1. **Business Understanding**

* Defined 10 key business questions covering revenue, segmentation, product performance, and subscription behavior.
* Established analytical goals aligned with business strategy.

### 2. **Data Exploration (EDA)**

* Loaded dataset into Python using pandas.
* Conducted descriptive statistics and profiling (`df.describe()`, `df.info()`).
* Visualized key distributions and trends.

### 3. **Data Cleaning & Preparation**

* Handled missing values in `review_rating` via median imputation per category.
* Standardized column names to snake_case.
* Removed redundant columns (`promo_code_used`).
* Created new features:

  * `age_group` (Young Adult, Adult, Middle-aged, Senior)
  * `purchase_frequency_days` (mapped from frequency terms)
* Integrated cleaned dataset into SQLite for query analysis.

### 4. **SQL-Based Data Analysis**

Executed SQL queries to answer business questions such as:

* Revenue by gender
* High-spending discount users
* Top 5 rated products
* Average purchase comparison by shipping type
* Subscriber vs non-subscriber spending
* Customer segmentation by purchase history
* Top products per category
* Age-group revenue contribution

**Deliverable:** Cleaned dataset and SQL query notebook/report

### 5. **Insight Generation**

**Key Findings:**

* Female customers contribute ~68% of total revenue.
* 839 customers spent above-average even after discounts.
* Express shipping slightly preferred over standard.
* Majority of customers are *loyal* (3,116 out of 3,900).
* Top-rated products: Gloves, Sandals, Boots, Hats, Skirts.
* Subscribers spend slightly less and contribute less revenue than non-subscribers.

**Deliverable:** Insight Summary Report

### 6. **Data Visualization (Tableau Dashboard)**

Developed an **interactive Tableau dashboard** to display:

* Revenue by gender, category, and age group
* Product rating and sales trends
* Customer segmentation distribution
* Subscription impact on revenue

**Deliverable:** Tableau Dashboard (`Customer_Shopping_Behavior_Dashboard.twbx`)

### 7. **Recommendations**

**Business Recommendations:**

* **Boost Subscriptions:** Introduce exclusive member offers to increase retention.
* **Loyalty Program:** Reward repeat buyers to strengthen the “Loyal” segment.
* **Optimize Discounts:** Review discount strategy to maintain profit margins.
* **Product Marketing:** Highlight top-rated and high-selling products in campaigns.
* **Targeted Marketing:** Focus efforts on high-revenue age groups and express-shipping customers.

**Deliverable:** Final Business Report & Presentation Deck

---

## 📊 Dashboard

**Tool:** Tableau
**Key Visuals:**

* Revenue and Spend by Gender
* Customer Segmentation Tree
* Product Rating and Purchase Heatmaps
* Subscription vs Non-Subscription Analysis

**File:** `Customer_Shopping_Behavior_Dashboard.twbx`

---

## 📦 Project Deliverables

| Deliverable                                    | Description                                                 |
| ---------------------------------------------- | ----------------------------------------------------------- |
| `Customer_Shopping_Behavior_EDA.ipynb`         | Python notebook for data loading, cleaning, and exploration |
| `customer_shopping_behavior.csv`               | Raw dataset                                                 |
| `customer_analysis_queries.sql`                | SQL queries addressing business questions                   |
| `Customer_Shopping_Behavior_Dashboard.twbx`    | Interactive Tableau dashboard                               |
| `Customer_Shopping_Behavior_Report.pdf`        | Final analytical report with insights & recommendations     |
| `Customer_Shopping_Behavior_Presentation.pptx` | Business presentation summarizing key findings              |
| `customer.csv`                                 | Clean dataset for SQL analytics                             |

---

## ▶️ How to Run This Project

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/customer-shopping-behavior-analysis.git
   cd customer-shopping-behavior-analysis
   ```

2. **Install dependencies**

   ```bash
   pip install pandas numpy matplotlib sqlite3
   ```

3. **Run the Jupyter Notebook**

   ```bash
   jupyter notebook Customer_Shopping_Behavior_EDA.ipynb
   ```

4. **Load data into SQLite**
   Run the script cells that connect and upload data to the SQLite database.

5. **Execute SQL Queries**
   Use the provided `.sql` file in SQLite Studio or DB Browser for SQLite.

6. **Open Tableau Dashboard**
   Load `Customer_Shopping_Behavior_Dashboard.twbx` in Tableau Desktop to interact with visuals.

---

## ✅ Results Summary

* Female customers drive higher total revenue.
* Loyal customers dominate overall sales volume.
* Discounts drive higher transaction counts but not always higher profits.
* Express shipping users exhibit higher average purchase values.
* Subscribers show lower spending behavior than non-subscribers.

---

## 💡 Recommendations Recap

* Promote **subscription incentives** to improve conversion.
* Enhance **loyalty programs** for high-value repeat buyers.
* Revisit **discount and pricing** strategy for better profit margins.
* Strengthen **targeted marketing** for high-performing demographics and products.

---

## 📁 Documents Included

1. **Jupyter Notebook:** Data Loading, EDA, Cleaning
2. **SQL File:** All analytical queries
3. **Tableau Dashboard:** Visual insights
4. **PDF Report:** Summary of insights and findings
5. **PowerPoint Deck:** Business presentation
6. **Clean Dataset:** Ready-to-analyze data

---

