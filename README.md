# E-Commerce Customer Behavior and Revenue Performance Analysis

## Project Overview

This project explores ecommerce performance using the Google Analytics Sample Ecommerce Dataset available in Google BigQuery. The analysis focuses on website traffic, customer activity, transaction performance, and revenue trends.

I used SQL to extract and prepare data, Excel to explore the results, and Power BI to build interactive dashboards. The aim was to understand how the website performed across different traffic sources, geographic locations, browsers, and days of the week, then translate the findings into practical business recommendations.

## Business Objectives

The project was designed to answer the following questions:

- How much revenue and transaction activity did the selected dataset record?
- Which countries and regions generated the most revenue?
- Which traffic sources contributed the most revenue?
- How did revenue vary across browsers and days of the week?
- What patterns could be identified in website activity and customer behavior?
- How can these findings support better business decisions?

## Tools and Technologies

- **Google BigQuery:** Accessing and querying the Google Analytics sample dataset.
- **SQL:** Extracting, filtering, combining, and preparing data for analysis.
- **Microsoft Excel:** Exploring the extracted data and reviewing performance patterns.
- **Power BI:** Building interactive dashboards and presenting business insights.
- **GitHub:** Documenting the project and presenting the work.

## Dataset

The project uses the Google Analytics Sample Ecommerce Dataset available through BigQuery. It contains website session information, traffic sources, device and browser details, geographic information, pageviews, transactions, and revenue.

The analysis combined selected session data from 2016 and 2017. The final SQL extraction was limited to 5,000 rows, so the results should be interpreted within the scope of the extracted dataset.

### Key Fields

| Field | Description |
|---|---|
| `Visit_Id` | Website visit identifier |
| `Visit_Date` | Date of the visit |
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

## Data Extraction and Preparation

I used SQL in BigQuery to retrieve the fields needed for the analysis and prepare the data for reporting.

The SQL work included:

- Selecting relevant columns and filtering records.
- Combining query results from multiple tables using `UNION ALL`.
- Using `SELECT DISTINCT` to return distinct rows.
- Applying conditional logic with `CASE WHEN`.
- Using aggregate functions, including `SUM()`.
- Sorting and limiting results with `ORDER BY` and `LIMIT`.
- Preparing fields for further analysis in Excel and Power BI.

The data preparation process also addressed duplicate rows, missing values, inconsistent city names, revenue data types, date formats, and transaction filtering where applicable.

## Excel Analysis

After extracting the data, I used Excel to explore revenue, transactions, pageviews, traffic sources, browsers, geographic locations, revenue categories, and day-of-week patterns.

This stage helped me review the data and identify trends worth examining in the Power BI dashboards.

## Power BI Dashboard

I developed two dashboard views to present the main performance metrics and make it easier to explore revenue patterns across different dimensions.

### Dashboard 1: Executive and Geographic Overview

This dashboard provides a summary of overall performance and geographic revenue distribution.

**Key performance indicators**

| Metric | Result |
|---|---:|
| Total Revenue | $48.02K |
| Total Transactions | 834 |
| Total Pageviews | 21K |
| Total Visits | 825 |

The dashboard also includes revenue by category, revenue by country, revenue by day of the week, and geographic revenue distribution.

![Executive and Geographic Overview Dashboard](executive-dashboard.png)

### Dashboard 2: Traffic and Customer Performance

This dashboard focuses on the relationship between traffic sources and revenue performance.

It includes:

- Revenue by traffic source.
- Revenue trends over time.
- Revenue by browser.
- Revenue by city.
- Interactive filters for date, country, browser, traffic source, and revenue category.

These views allow users to explore performance across the available dimensions rather than relying on summary figures alone.

![Traffic and Customer Performance Dashboard](traffic-customer-dashboard.png)

## Key Findings

### 1. Geographic Revenue Performance

North America recorded the highest revenue among the regions analyzed.

This highlights the importance of geographic analysis when evaluating ecommerce performance. Further comparisons of individual countries, transaction volumes, and conversion rates would help provide a more detailed picture of regional performance.

### 2. Traffic Source Performance

Direct traffic generated the most revenue in the analysis, outperforming Google and YouTube.

Revenue is one useful measure of channel performance, but sessions and conversion rates should also be considered when assessing the overall value of each traffic source.

### 3. Browser Usage

Chrome and Safari were the most frequently used browsers among the visits analyzed.

This provides useful context for website performance monitoring. Comparing conversion rates and transaction activity across browsers would help determine whether differences in user experience affect business outcomes.

### 4. Revenue Category Distribution

The Medium and High revenue categories accounted for most of the revenue, while the Low category contributed the least.

This pattern may help guide further investigation into customer or revenue segmentation, depending on how the categories were defined.

### 5. Revenue by Day of the Week

Wednesday recorded the highest revenue among the days analyzed.

Comparing transaction volume, average transaction value, and website traffic across weekdays could help establish whether this pattern is consistent and commercially meaningful.

## Business Recommendations

Based on the findings, I identified several areas the business could investigate:

1. **Review traffic channel performance.** Compare revenue, transactions, sessions, and conversion rates across Direct, Google, and YouTube before making changes to marketing investment.
2. **Investigate geographic opportunities.** Examine individual country performance to identify markets with promising revenue and conversion patterns.
3. **Monitor browser performance.** Test website usability across major browsers and investigate any differences in transaction or conversion performance.
4. **Explore weekday trends.** Review Wednesday's performance across multiple periods before considering day-specific campaigns.
5. **Review revenue segments.** Examine the characteristics and definitions of the Low, Medium, and High categories to determine how they can support business reporting.
6. **Maintain regular performance reporting.** Use the Power BI dashboards to monitor key metrics and investigate changes in revenue and website activity over time.

These recommendations are intended as areas for further investigation rather than guaranteed ways to increase revenue.

## Analytical Workflow

The project followed this process:

```text
Google BigQuery
       |
       v
SQL Data Extraction
       |
       v
Data Cleaning and Preparation
       |
       v
Excel Data Exploration
       |
       v
Power BI Dashboard Development
       |
       v
Business Findings
       |
       v
Recommendations
```

## Skills Demonstrated

- SQL querying and data extraction.
- Google BigQuery.
- Data cleaning and preparation.
- Exploratory data analysis.
- Ecommerce revenue and transaction analysis.
- Traffic source and geographic analysis.
- Power BI dashboard development.
- KPI reporting and data visualization.
- Business insight generation.

## Limitations

The analysis was based on a selected extract limited to 5,000 rows. The results therefore describe the extracted data and should not automatically be treated as representative of the entire source dataset.

The findings identify patterns in the available data but do not establish the causes of those patterns. Additional analysis would be needed to validate proposed business changes and measure their impact.

## About Me

I am an Economics undergraduate at the University of Port Harcourt with an interest in Data Analytics, Business Intelligence, and Business Analytics. I enjoy using data to investigate business questions, understand performance, and communicate findings that can support informed decisions.

**GitHub:** [dbusiness-analytics](https://github.com/dbusiness-analytics)

**LinkedIn:** [Daniel Basil](https://www.linkedin.com/in/daniel-basil-60aa43363/)

---

*This project demonstrates the use of SQL, BigQuery, Excel, and Power BI to explore ecommerce performance and communicate findings through business-focused dashboards.*
