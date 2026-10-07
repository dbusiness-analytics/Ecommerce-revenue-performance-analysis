# 📊 E-Commerce Revenue & Performance Analysis

An end-to-end business analytics project analyzing customer behavior, website traffic, transaction performance, and revenue trends using **BigQuery SQL, Excel, and Power BI**.

The project focuses on extracting useful business data from large Google Analytics datasets, preparing the data for analysis, and transforming the results into actionable business insights.

---

## 📌 Business Scenario

A retail company wants to better understand its digital performance across:

- Customer behavior
- Website traffic
- Revenue trends
- Transaction performance
- Browser usage
- Geographic performance
- Traffic source performance

The company has millions of website records stored in BigQuery and requires analysts to extract, clean, analyze, and visualize the most relevant business data for decision-making.

---

## 🎯 Project Objectives

The main objectives of this project were to:

- Extract relevant business data from multiple BigQuery tables
- Combine datasets using SQL
- Remove duplicate records
- Clean and prepare the extracted data
- Analyze customer and revenue patterns using Excel
- Build interactive Power BI dashboards
- Identify high-performing markets and traffic sources
- Provide data-driven business recommendations

---

## 🛠️ Tools & Technologies

- **Google BigQuery** — Data extraction and SQL analysis
- **SQL** — Data transformation, filtering, aggregation, and preparation
- **Microsoft Excel** — Exploratory analysis and data preparation
- **Power BI** — Interactive dashboards and business intelligence
- **GitHub** — Project documentation and portfolio presentation

---

## 🗃️ Dataset

The project uses the **Google Analytics Sample Dataset** available through BigQuery.

The extracted dataset contains key fields including:

| Column | Description |
|---|---|
| Visit_Id | Unique visit identifier |
| Visit_Date | Date of the website visit |
| Country | Customer country |
| City | Customer city |
| Device_Category | Device used by the customer |
| Browser | Browser used |
| Traffic_Source | Source of website traffic |
| PageViews | Number of pages viewed |
| Transactions | Number of transactions |
| Revenue | Revenue generated |

Additional analytical fields were created during data preparation, including:

- Revenue Category
- Conversion Flag
- Clean City

---

## 🔍 SQL Analysis

SQL was used to extract and prepare the data from multiple BigQuery tables.

Key SQL concepts applied:

- `SELECT DISTINCT`
- `WHERE`
- `UNION ALL`
- `GROUP BY`
- Aggregate functions such as `SUM()`
- `CASE WHEN`
- `ORDER BY`
- `LIMIT`

The analysis combined data from the 2016 and 2017 Google Analytics session tables and filtered the records based on transaction, revenue, device, and traffic-source criteria.

The final exported dataset was limited to **5,000 records** for downstream analysis.

---

## 📈 Excel Analysis

The cleaned dataset was analyzed in Excel to identify patterns across:

- Revenue
- Transactions
- Pageviews
- Traffic sources
- Browsers
- Countries
- Cities
- Revenue categories
- Days of the week

The Excel analysis provided the foundation for the Power BI dashboard and helped identify the most important business trends.

---

## 📊 Power BI Dashboard

The Power BI dashboard provides an interactive view of e-commerce revenue and customer performance.

### Dashboard 1 — Executive & Geographic Overview

Key metrics:

- **Total Revenue:** $48.02K
- **Total Transactions:** 834
- **Total Pageviews:** 21K
- **Total Visits:** 825

Visualizations include:

- Revenue Category
- Revenue by Country
- Revenue by Day of Week
- Geographic Revenue Distribution
- Key Business Insights
- Business Recommendations

### Dashboard 2 — Traffic & Customer Performance

Visualizations include:

- Revenue by Traffic Source
- Revenue Trend
- Revenue by Browser
- Revenue by City
- Interactive filters for date, country, browser, traffic source, and revenue category

---

## 🖼️ Dashboard Preview

### Executive & Geographic Overview

![Executive & Geographic Overview Dashboard](images/executive-dashboard.png)

### Traffic & Customer Performance

![Traffic & Customer Performance Dashboard](images/traffic-customer-dashboard.png)

---

## 💡 Key Insights

### 1. Strong North American Performance

North America generated the highest revenue, making it the strongest-performing market.

### 2. Direct Traffic Led Revenue Generation

Direct traffic was the leading source of revenue, outperforming Google and YouTube.

### 3. Chrome and Safari Dominated

Chrome and Safari were the most frequently used browsers among revenue-generating visits.

### 4. Medium and High Revenue Segments Dominated

Medium and High revenue segments accounted for most of the total revenue, while the Low segment contributed the least.

### 5. Wednesday Recorded the Highest Revenue

Revenue varied throughout the week, with Wednesday recording the highest revenue.

---

## 💼 Business Recommendations

Based on the analysis, the following recommendations were developed:

- Increase investment in **Direct and Google marketing channels** to maintain and grow high-performing traffic sources.
- Optimize the website experience for **Chrome and Safari** users to improve usability and conversion performance.
- Expand marketing efforts in high-performing regions, particularly the **United States**, while exploring growth opportunities in other markets.
- Launch targeted promotions during **high-performing days** to maximize revenue and customer engagement.
- Continue monitoring customer and revenue behavior through interactive dashboards to support **data-driven decision-making** and identify emerging trends.

---

## 🔄 Analytics Workflow

```text
BigQuery
   ↓
SQL Data Extraction
   ↓
Data Cleaning & Transformation
   ↓
Excel Analysis
   ↓
Power BI Dashboard
   ↓
Business Insights
   ↓
Recommendations
