# Marketing, Customer & Sales Analytics

A data analytics project that transforms raw customer, marketing, and sales data into **actionable business insights** through data cleaning, exploratory analysis, customer segmentation, and an interactive Power BI dashboard.

The project analyzes **15,000 customers across 41 columns**, covering customer demographics, engagement, financial behavior, marketing acquisition, and lifecycle/retention data.

---

## 📌 Project Overview

Marketing decisions are often made using fragmented data, making it difficult to understand which customers, channels, and segments actually drive business value.

This project aims to create a single, evidence-based view of:

* Customer value and behavior
* Revenue and spending
* Customer churn and retention
* Marketing channel performance
* Customer segmentation
* Engagement and purchasing behavior
* Business risks and opportunities

The overall goal is to move from **descriptive reporting to evidence-based business decisions**.

---

## 🎯 Business Objectives

The project focuses on four main objectives:

1. Quantify revenue, spending, and churn across the customer base.
2. Identify acquisition channels that deliver **scale vs. customer value**.
3. Segment customers based on their behavior and value to support targeted retention strategies.
4. Build an interactive dashboard that managers can use for day-to-day decision-making.

---

## 📊 Dataset

The dataset contains:

* **15,000 customers**
* **41 columns**
* **5 countries:** Germany, India, UK, USA, Bangladesh
* **5 acquisition channels:** Organic, Google Ads, Facebook Ads, Email, Referral
* Customer demographic information
* Engagement and behavioral metrics
* Financial and revenue metrics
* Marketing and acquisition data
* Lifecycle and retention information

Key fields include customer demographics, visits, session behavior, total spending, average order value, lifetime value, acquisition channel, email engagement, marketing spend, signup date, last purchase date, tenure, and churn.

---

## 🔍 Analysis Workflow

The project follows a complete analytics workflow:

```text
Raw Data
   ↓
Data Quality & Cleaning
   ↓
Exploratory Data Analysis
   ↓
Statistical & Diagnostic Analysis
   ↓
Customer Segmentation
   ↓
Business Insights
   ↓
Power BI Visualization
   ↓
Recommendations & Decisions
```

The analysis follows an evidence-first approach: metrics and conclusions are based on the available data, while correlation is not interpreted as causation.

---

## 🧹 Data Quality

Several important data-quality issues were identified and handled through flags and reconciliation rather than blindly deleting records.

### Invalid Lifecycle Chronology

* **3,762 records**
* Approximately **25%** of the dataset
* `last_purchase_date` occurs before `signup_date`

These records were flagged using `valid_chronology`, while lifecycle metrics such as tenure and recency were excluded for affected records.

### Coupon & Discount Mismatch

* **7,624 records**
* Approximately **51%** of the dataset
* `coupon_code` and `discount_used` contain inconsistent information.

A reconciled `coupon_used` flag was created while preserving the underlying fields for auditing.

---

## 📈 Key Business Insights

### 1. Customer Value is Concentrated

The top **20% of customers generate approximately 39.8% of recorded spend**, showing that a relatively small group contributes a disproportionate share of value.

### 2. Scale ≠ Value

Organic is the strongest channel in terms of total spend and customer volume, while **Email and Referral** demonstrate higher spend per customer.

This highlights the difference between acquiring a large number of customers and acquiring high-value customers.

### 3. At-Risk Customers are a Major Retention Priority

The At Risk segment contains **7,479 customers**, including **1,215 churners**, with approximately **$3.2M in spend at stake**.

### 4. Data Quality is a Business Issue

The lifecycle-date problems and coupon inconsistencies can affect downstream customer lifecycle and promotional analysis. Therefore, improving the source data is considered a strategic priority rather than only a technical cleaning task.

---

# 📊 Power BI Dashboard

The project includes an interactive **Power BI dashboard** designed to transform analytical findings into actionable business insights.

### Dashboard Page 1 — Executive Overview

Provides a high-level view of:

* Overall business performance
* Revenue / spending
* Customer base
* Churn and retention
* Marketing performance
* Channel and country performance
* Key trends and management alerts

### Dashboard Page 2 — Customer Segmentation & Value

Focuses on:

* Customer segments
* Customer value
* RFM-based analysis
* High-value customers
* At-risk customers
* Churn concentration
* Retention opportunities

The dashboard is designed around the storyline:

```text
What is happening?
        ↓
Who is driving the results?
        ↓
Why is it happening?
        ↓
What should the business do?
```

The dashboard pages and business storyline are designed to connect analysis directly to management decisions.

---

## 🖼️ Dashboard Images

### Executive Overview

![Executive Overview Dashboard](Images/Overview.png)

### Customer Segmentation & Value

![Customer Segmentation & Value Dashboard](Images/Customer_Segmentation.png)

> **Note:** Replace the image filenames above with the exact filenames used in your repository's `Images` folder.

---

## 🛠️ Tools & Technologies

* **Python**

  * Pandas
  * NumPy
  * Matplotlib
  * Seaborn
  * Scikit-learn
* **Jupyter Notebook**
* **Power BI**
* **DAX**
* **Data Cleaning & EDA**
* **RFM Analysis**
* **K-Means Clustering**
* **Statistical Analysis**
* **Data Visualization**

---

## 📂 Project Structure

```text
Marketing-Customer-Sales-Analytics/
│
├── Data/
│   └── Sales_marketing_customer_dataset.csv
│
├── Notebook/
│   └── marketing-customer-sales-analysis.ipynb
│
├── PowerBI/
│   └── FinalProject.pbix
│
├── Images/
│   ├── Overview.png
│   └── Customer_Segmentation.png
│
├── Documentation/
│   ├── Marketing_Customer_Sales_Analytics.pdf
│   └── Using_prompts.pdf
│
└── README.md
```

---

## 👥 Team Members

* **[Malak Zidan](#)**
* **[Mariam Mostafa](#)**
* **[Mariam Haitham](#)**

---

## 🚀 Project Outcome

The final project connects the complete journey:

```text
Data
 ↓
Cleaning
 ↓
Analysis
 ↓
Visualization
 ↓
Dashboard
 ↓
Insights
 ↓
Business Decisions
```

The result is a **Marketing, Customer & Sales Intelligence solution** that helps management understand customer value, channel performance, churn risks, and opportunities for targeted action.

---

## ⭐ Key Takeaway

> **The goal is not simply to visualize the data — it is to turn customer, marketing, and sales data into evidence-based decisions.**
