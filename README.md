Brazilian E-Commerce Sales Performance & Customer Analytics

Project Overview

This project uses Power BI to analyse the sales performance and customer purchasing behaviour of a Brazilian e-commerce marketplace. Using the Olist Brazilian E-Commerce dataset, I developed an interactive report to explore revenue trends, product category performance, customer retention, orders fulfilled and their geographical sales distribution.

The objective was to transform a large, raw, transactional dataset into actionable business insights through data cleaning, data modelling, DAX calculations and interactive visualisation. This project demonstrates my ability to apply data analytics techniques to a real-world business dataset and communicate analytical findings through a structured dashboard.

Business Objectives

The analysis was designed to address the following business questions:

  How is overall revenue performing over time?

  Which product categories generate the greatest revenue?

  How do sales trends vary by month, quarter and year?

**  What proportion of customers make repeat purchases?

  Which payment method was most commonly used in order transactions? 

  How does customer retention change over time?

**  How do order fulfilment and delivery performance affect the customer experience?

  Which geographical regions generate the greatest concentration of orders?


Dataset

Source: Olist Brazilian E-Commerce Public Dataset

View the dataset on Kaggle

The dataset contains anonymised transactional information from a Brazilian e-commerce marketplace, covering orders placed between 2016 and 2018.

The dataset includes multiple related tables containing information about:

  - Customers

  - Orders

  - Order items

  - Products

  - Sellers

  - Payments

  - Customer reviews (decided to not include)

  - Geographical locations

This relational structure provides an opportunity to develop a data model capable of supporting analysis across sales, customers and products.

Tools & Technologies

  Microsoft Power BI

  Dashboard development, data modelling and visualisation

  Power Query

  Data cleaning, transformation and preparation

  DAX

  Measures, calculated columns and analytical calculations

  Data Modelling

  Relationships between transactional and dimension tables

  Initial data inspection and supporting analysis


Project Methodology

1. Data Preparation & Cleaning

I imported the Olist datasets into Power BI and used Power Query to prepare the data for analysis.

The preparation process included:

Inspecting the structure and quality of the source tables.

Identifying and handling missing values where appropriate.

Reviewing duplicate records and unique identifiers.

Checking data types and ensuring date fields were correctly formatted.

Assessing the granularity of each table.

Preparing date fields for time-based analysis.

Ensuring that data transformations preserved the integrity of the underlying transactional data.

2. Data Modelling

I developed a relational data model connecting the relevant datasets to support analysis across multiple business dimensions.

The modelling process involved:

Establishing relationships between customers, orders, order items, products and other relevant tables.

Reviewing relationship cardinality and filter propagation.

Creating a dedicated date table to support time intelligence.

Developing customer cohort attributes to analyse repeat purchasing behaviour.

Considering the impact of table granularity on revenue calculations and aggregation.

3. DAX & Analytical Measures

I developed DAX measures to calculate key performance indicators and support interactive analysis.

The measures include:

Total Revenue

Total Orders

Total Customers

Average Order Value

Delivered Orders

Delivery Rate

Average Delivery Time

Year-over-Year Revenue Growth

Revenue Previous Year

Revenue by Product Category

Customer Retention Percentage

Cohort Size

Retained Customers

These measures support the analysis of sales performance, customer purchasing behaviour and operational performance.

4. Dashboard Development

I developed an interactive Power BI report designed to provide both high-level performance monitoring and more detailed analytical exploration.

The report incorporates KPI cards, time-series analysis, product performance visualisations, geographical analysis and customer retention analysis.

The visual design emphasises clear presentation, consistent formatting, appropriate visual hierarchy and usability.

Dashboard Features

Sales Performance Overview

Provides a high-level summary of marketplace performance through key metrics and interactive visuals.

Features include:

Revenue and order KPIs.

Customer and order value metrics.

Quarterly and monthly revenue trends.

Year-over-Year revenue comparison.

Product category revenue analysis.

Interactive filtering and cross-visual exploration.

Sales & Product Performance

Explores sales performance across time and product categories.

The report enables users to investigate revenue trends, identify leading product categories and explore differences in performance across business dimensions.

Customer Cohort Retention Analysis

A cohort retention heatmap was developed to investigate repeat purchasing behaviour over time.

Customers are grouped according to their initial purchase month, with subsequent purchasing activity analysed by cohort month.

The heatmap enables the comparison of customer retention across cohorts and retention periods.

Geographical Order Analysis

A geographical visualisation was developed to explore the distribution of customer orders across Brazilian states.

This supports the identification of regions with greater order concentration.

Interactive Reporting

The report incorporates interactive features to support detailed exploration, including:

Slicers and cross-filtering.

Drill-down through date hierarchies.

Drill-through to detailed cohort analysis.

Dynamic KPI calculations.

Context-sensitive filtering.

Key Analytical Considerations

Throughout the project, I considered the importance of data quality, analytical definitions and the reliability of calculated measures.

Particular attention was given to:

Defining revenue consistently.

Avoiding duplicated revenue caused by relationships between tables with different levels of granularity.

Distinguishing order counts from item counts.

Using an appropriate date table for time intelligence.

Ensuring cohort retention percentages were calculated relative to the original cohort size.

Separating delivered-order analysis from broader order activity where appropriate.

These considerations were important in ensuring that the dashboard presented meaningful and reliable business metrics.

Business Value

The report provides a structured view of e-commerce performance and demonstrates how transactional data can be converted into business intelligence.

The analysis can support:

Monitoring sales performance over time.

Identifying high-performing product categories.

Understanding customer purchasing patterns.

Investigating repeat-purchase behaviour.

Exploring geographical order distribution.

Supporting data-driven commercial decision-making.

Repository Structure

olist-ecommerce-sales-performance-analysis/
│
├── README.md
│
├── PowerBI/
│   └── Olist_Sales_Performance_Dashboard.pbix
│
├── Screenshots/
│   ├── dashboard_overview.png
│   ├── sales_performance.png
│   ├── customer_retention_heatmap.png
│   └── cohort_drillthrough.png
│
├── Documentation/
│   ├── data_model.png
│   ├── data_dictionary.md
│   └── dax_measures.md
│
└── Data/
    └── README.md

Limitations

The dataset represents a historical period of e-commerce activity between 2016 and 2018. Therefore, the findings should not be interpreted as a representation of current marketplace performance.

The analysis is based on the available fields within the public dataset. Additional business information, such as marketing expenditure, product costs and customer acquisition costs, would be required to investigate profitability and marketing return on investment in greater depth.

Future Development

Potential extensions to the project include:

Developing customer segmentation using purchasing behaviour.

Investigating product profitability where cost data is available.

Analysing customer review scores in relation to delivery performance.

Expanding the analysis through Python or SQL.

Developing additional measures for customer lifetime value.

Improving report deployment and sharing through Power BI Service.

Author

Economics BSc Graduate | Aspiring Data Analyst

This project forms part of my data analytics portfolio, demonstrating my application of Power BI, data modelling, DAX and analytical problem-solving to a real-world business dataset.
