# E-Commerce Customer Behavior and Revenue Performance Analysis

## Project Overview

This end-to-end business analytics project examines website traffic, customer behavior, transaction performance, and revenue trends using Google BigQuery, SQL, Microsoft Excel, and Power BI.

The project demonstrates a structured analytical workflow, from extracting and preparing data to exploring business performance, visualizing findings, and developing recommendations to support data-informed decision-making.

## Business Scenario

A retail business wants to better understand its digital performance across customer behavior, website traffic, transaction activity, and revenue generation.

With website analytics data stored in BigQuery, the objective is to extract relevant information, identify meaningful patterns, and present the findings in a format that supports business reporting and decision-making.

## Project Objectives

- Extract relevant data from multiple BigQuery tables.
- Combine datasets using SQL.
- Prepare and clean data for analysis.
- Explore revenue, transactions, pageviews, and traffic sources.
- Compare performance across countries, cities, browsers, and days of the week.
- Develop interactive Power BI dashboards.
- Identify key business patterns and potential growth opportunities.
- Translate analytical findings into practical recommendations.

## Tools and Technologies

- **Google BigQuery:** Data extraction and querying.
- **SQL:** Filtering, combining, aggregating, and preparing data.
- **Microsoft Excel:** Data exploration and analysis.
- **Power BI:** Interactive dashboards and business intelligence.
- **GitHub:** Project documentation and portfolio presentation.

## Dataset

The project uses the Google Analytics Sample Ecommerce Dataset available through BigQuery.

The analysis uses fields representing website sessions, dates, geographic locations, devices, browsers, traffic sources, pageviews, transactions, and revenue.

### Key Fields

| Column | Description |
|---|---|
| `Visit_Id` | Website visit identifier |
| `Visit_Date` | Date of the website visit |
| `Country` | Country associated with the visit |
| `Clean_City` | Standardized city value |
| `Device_Category` | Device category |
| `Browser` | Browser used |
| `Traffic_Source` | Source of website traffic |
| `PageViews` | Number of pages viewed |
| `Transactions` | Transaction count |
| `Revenue` | Revenue recorded |
| `Revenue Category` | Revenue classification |
| `Conversion Flag` | Indicator of conversion status |

## SQL Analysis

SQL was used to extract, filter, combine, and prepare data for further analysis.

### SQL Concepts Applied

- `SELECT DISTINCT`
- `WHERE`
- `UNION ALL`
- `GROUP BY`
- Aggregate functions, including `SUM()`
- `CASE WHEN`
- `ORDER BY`
- `LIMIT`

### Data Extraction and Filtering

The analysis combined Google Analytics session data from 2016 and 2017.

The extraction included filtering conditions related to revenue-generating sessions, transactions greater than zero, mobile users, and selected traffic sources.

`SELECT DISTINCT` was used to return distinct rows, and the final extraction was limited to 5,000 rows.

**Important:** `SELECT DISTINCT` removes duplicate result rows; it does not necessarily guarantee that each visit identifier appears only once. The extraction limit also means the results represent the selected dataset rather than necessarily the entire source dataset.

## Excel Analysis

The extracted dataset was explored in Microsoft Excel to examine patterns across:

- Revenue and transactions
- Pageviews and traffic sources
- Browsers and geographic locations
- Revenue categories
- Days of the week

The analysis helped identify patterns and prepare findings for presentation in the Power BI dashboards.

## Power BI Dashboard

The Power BI report presents an interactive view of ecommerce revenue, website activity, and traffic performance.

### Dashboard 1: Executive and Geographic Overview

**Key performance indicators**

| Metric | Result |
|---|---:|
| Total Revenue | $48.02K |
| Total Transactions | 834 |
| Total Pageviews | 21K |
| Total Visits | 825 |

**Key visualizations**

- Revenue by category
- Revenue by country
- Revenue by day of the week
- Geographic revenue distribution
- Business
