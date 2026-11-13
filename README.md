**Brazilian E-Commerce Sales Performance & Customer Analytics**

**Project Overview**

This project uses Power BI to analyse the sales performance and customer purchasing behaviour of a Brazilian e-commerce marketplace. Using the Olist Brazilian E-Commerce dataset, I developed an interactive report to explore revenue trends, product category performance, customer retention, orders fulfilled and their geographical sales distribution.

The objective of this project was to transform a large, raw, transactional dataset into actionable business insights through data cleaning, data modelling, DAX calculations and interactive visualisation. This project demonstrates my ability to apply data analytics techniques to a real-world business dataset and communicate analytical findings through a structured dashboard.

**Business Objectives**

The analysis was designed to address the following business questions:

  - How is overall revenue performing over time?
  - Which product categories generate the greatest revenue?
  - How do sales trends vary by month, quarter and year?
  - What proportion of customers make repeat purchases?
  - Which payment method was most commonly used in order transactions?
  - How does customer retention change over time?
  - Which geographical regions generate the greatest concentration of orders?


**Dataset**

Source: Olist Brazilian E-Commerce Public Dataset

[View the dataset on Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

The public dataset contains anonymised transactional information from a Brazilian e-commerce marketplace, covering orders placed between 2016 and 2018.

The dataset includes multiple related tables containing information about:

  - Customers
  - Orders
  - Order items
  - Products
  - Sellers
  - Payments
  - Customer reviews (not included)
  - Geographical locations

Tools & Technologies:

  - Microsoft Power BI - Dashboard development, data modelling and visualisation
  - Power Query - Data cleaning, transformation and preparation
  - DAX - Measures, calculated columns and analytical calculations
  - Data Modelling - Relationships between transactional and dimension tables
  - GitHub - Project documentation, version control and portfolio presentation


**Project Methodology**

1. Data Preparation & Cleaning

I imported the Olist datasets into Power BI and used Power Query to prepare the data for analysis.


<img width="2880" height="1800" alt="image" src="https://github.com/user-attachments/assets/e4d1aaef-e0ae-400a-b320-ca5cdfe772c4" />


The preparation process included:

  - Inspecting the structure and quality of the source tables.
  - Identifying and handling missing values where appropriate.
  - Reviewing duplicate records and unique identifiers.
  - Checking data types and ensuring date fields were correctly formatted.
  - Assessing the granularity of each table.
  - Preparing date fields for time-based analysis.
  - Ensuring that data transformations preserved the integrity of the underlying transactional data.

2. Data Modelling

I developed a relational data model connecting the relevant datasets to support analysis across multiple business dimensions.

The modelling process involved:
  - Establishing relationships between customers, orders, order items, products and other relevant tables.
  - Reviewing relationship cardinality and filter propagation.
  - Creating a dedicated date table to support time intelligence.
  - Developing customer cohort attributes to analyse repeat purchasing behaviour.
  - Considering the impact of table granularity on revenue calculations and aggregation.

3. DAX & Analytical Measures

I developed DAX measures to calculate key performance indicators and support interactive analysis.

The measures include:
  - Total Revenue
  - Total Orders
  - Total Customers
  - Average Order Value
  - Delivered Orders
  - Delivery Rate
  - Average Delivery Time
  - Year-over-Year Revenue Growth
  - Revenue Previous Year
  - Revenue by Product Category
  - Customer Retention Percentage
  - Cohort Size
  - Cohort Index
  - Retained Customers

These measures support the analysis of sales performance, customer purchasing behaviour and operational performance.

4. Dashboard Development

I developed an interactive Power BI report designed to provide both high-level performance monitoring and more detailed analytical exploration.

The report incorporates KPI cards, time-series analysis, product performance visualisations, geographical analysis and customer retention analysis.

The visual design emphasises clear presentation, consistent formatting, appropriate visual hierarchy and usability. A consistent colour scheme of neutral shades and navy blue text provides the dashboard with a professional feel, inspired by the companies colour palette.


**Dashboard Features**

Provides a high-level summary of marketplace performance through key metrics and interactive visuals.

Features include:
  - Revenue and order KPIs.
  - Customer and order value metrics.
  - Quarterly and monthly revenue trends.
  - Year-over-Year revenue comparison.
  - Product category revenue analysis.
  - Interactive filtering and cross-visual exploration.


**Sales & Product Performance**

Explores sales performance across time and product categories.
The report enables users to investigate revenue trends, identify leading product categories and explore differences in performance across business dimensions.

**Customer Cohort Retention Analysis**

A cohort retention heatmap was developed to investigate repeat purchasing behaviour over time. Customers are grouped according to their initial purchase month, with subsequent purchasing activity analysed by cohort month. The heatmap enables the comparison of customer retention across cohorts, with conditional formatting enabling viewers to quickly and easily understand customer retention rates. The drill down feature is also used on the matrix visual to allow for more in depth customer retention analysis for specific cells. 

**Geographical Order Analysis**

A geographical visualisation was developed to explore the distribution of customer orders across Brazilian states which supports the identification of regions with greater order concentration via conditional formatting of colours. This can highlight where to target product advertisement for example to boost sales.

**Interactive Reporting**

The report incorporates interactive features to support detailed exploration, including:
  - Drill-down through date hierarchies.
  - Drill-through to detailed cohort analysis.
  - Dynamic KPI calculations and formatting.
  - Context-sensitive filtering.

**Key Analytical Considerations**

Particular attention was given to:
  - Defining revenue consistently.
  - Avoiding duplicated revenue caused by relationships between tables.
  - Distinguishing order counts from item counts.
  - Using a date table for time intelligence.
  - Ensuring cohort retention percentages were calculated relative to the original cohort size.
  - Separating delivered-order analysis from broader order activity where appropriate.

These considerations were important to ensure data quality and hence that the dashboard presented meaningful and reliable business metrics.

The report provides a structured view of e-commerce performance and demonstrates how transactional data can be converted into business intelligence.

The analysis can support:
  - Monitoring sales performance over time.
  - Identifying high-performing product categories.
  - Understanding customer purchasing patterns.
  - Investigating repeat-purchase behaviour.
  - Exploring geographical order distribution.
  - Supporting data-driven commercial decision-making.


**Limitations**

The dataset represents a historical period of e-commerce activity between 2016 and 2018. Therefore, the findings should not be interpreted as a representation of current marketplace performance.

The analysis is based on the available fields within the public dataset. Additional business information, such as marketing expenditure and product costs would be required to investigate profitability and marketing return on investment in greater depth.

Hence, potential extensions to the project include:
  - Investigating product profitability where cost data is available.
  - Expanding the analysis through Python or SQL.
  - Developing additional measures for customer lifetime value.
  - Developing customer segmentation using purchasing behaviour.


**Challenges Encountered & Problem-Solving**

Throughout the development of this project, I encountered several technical and analytical challenges. Resolving these issues required iterative testing, investigation of the underlying data model, and refinement of DAX calculations.

1. Data Modelling and Relationship Configuration

Challenge: Establishing an accurate relational schema across multiple Olist datasets. Incorrect relationships and mismatched join columns risked introducing duplicated records and inconsistencies in revenue calculations.


<img width="1440" height="900" alt="Screenshot 2026-10-22 at 13 35 11" src="https://github.com/user-attachments/assets/9f664314-7fc9-40c1-b3ef-7103bfc96dd3" />


  I examined the individual tables to identify appropriate primary keys, and configured relationships between the orders, customers, order items, payments, products and sellers datasets. I investigated potential duplication arising from one-to-many relationships and validated the resulting aggregations by creating a calculated column and filtering to assess the unmatched records.


  <img width="1440" height="900" alt="Screenshot 2026-11-05 at 13 00 07" src="https://github.com/user-attachments/assets/a1801f14-ab8d-47fe-afcf-337c7ad7eea7" />



2. Data Quality and Missing Values

Challenge: Identifying and managing blank values, missing dates and incomplete records without distorting data findings.


<img width="993" height="655" alt="Screenshot 2026-11-03 at 11 10 12" src="https://github.com/user-attachments/assets/dafb89df-607c-441a-9999-687688cafd2b" />


  I investigated missing values within Power Query and the data model, distinguishing between records that could be excluded due to missing at random and fields where missing information required further investigation as it appeared systematic.

3. Complex DAX Measures and Calculated Columns

Challenge: Developing DAX calculations for business performance metrics, including revenue, average order value, delivery performance, year-over-year revenue growth and customer retention for use in KPI cards and trend analysis for example.

  I used functions such as `CALCULATE`, `DIVIDE`, `DISTINCTCOUNT`, `FILTER` and time-intelligence functions to develop measures. I     also investigated filter context, row context and both calculated columns and measures.

4. Customer Retention and Cohort Analysis

Challenge: Initial cohort retention calculations produced unexpectedly low percentages, while conditional formatting resulted in limited visual variation due to the distribution of values.


<img width="1170" height="773" alt="Screenshot 2026-11-12 at 10 59 08" src="https://github.com/user-attachments/assets/1728f4e5-0b8f-432a-81b2-9425020d2cd6" />


  I investigated the relationship between cohort size, retained customer counts and the retention percentage calculation. I also refined the conditional formatting configuration by adjusting the minimum, midpoint and maximum colour values to improve the visual distinction between retention levels.

5. Visualisation Configuration and Geographic Analysis

Challenge: Configuring Power BI's filled map visual to accurately represent the geographic distribution of customer orders across Brazil. Initial configurations resulted in a map displaying a global view, making regional patterns difficult to interpret.

  I investigated geographic field categorisation, map configuration settings and the use of Brazilian state-level geographic data. I also explored the available zoom and auto-zoom controls to improve the map's geographic focus.

6. Date Relationships and Time-Series Analysis

Challenge: Revenue trend visualisations initially displayed blank date categories, incorrect chronological ordering and incomplete quarterly trends.


<img width="787" height="163" alt="image" src="https://github.com/user-attachments/assets/d32c9e61-827b-47fc-bc82-d8964ab99f9b" />


  I created a dedicated calendar/date table, developed date-based calculated columns and investigated the relationship between order   purchase timestamps and date-only fields. I also refined the quarter sorting logic to ensure chronological ordering.


**Business Questions & Analytical Findings**

This analysis was guided by a series of business questions designed to evaluate marketplace sales performance, customer purchasing behaviour and product performance. Power BI measures and interactive visualisations were used to investigate each question and identify potential areas for business improvement.

1. How is overall revenue performing over time?

Analysis performed: 
Total Revenue, Revenue Previous Year and Year-over-Year Revenue Growth measures were developed using DAX. Line charts were used to analyse monthly and quarterly revenue trends.

Analytical findings:
The period of 2018, Q3 is identified as the period with the highest revenue of approximately $117,814. This was the most recent perod measured implying revenue has increased over time. Conversely, the period with the lowest noted revenue was the very first period recorded - 2016, Q4 with revenue of $3,609. However, the overall trend is not completely linear, with fluctuations made evident on the line chart of significant dips in revenue approximately every other quarter.

2. Which product categories generate the greatest revenue?

Analysis performed: 
Revenue by Product Category was calculated and visualised using bar charts. Category Revenue Share was used to compare the relative contribution of individual product categories to overall revenue through the use of tooltips.

Analytical findings:
The product category with the largest contribution to revenue was health and beauty, with a revenue of approximately $48,000 which contributed to 8.94% of ovrall revenue. The lowest contributor accounting for only 0.01% and $34.99 was home comforts.

3. What proportion of customers make repeat purchases?

Analysis performed:
A Repeat Purchase Rate measure was developed to calculate the proportion of unique customers who placed more than one order. A customer purchase frequency bar chart was used to categorise customers according to the number of orders placed. Cohort retention analysis investigated purchasing behaviour over time.

Analytical findings: 
The overall repeat purchase rate was identified as 2.82%. The proportion of customers who placed only 1 order was 94.23% compared to only 2.68% who placed 2 orders.

4. How does customer retention change over time?

Analysis performed:
A customer cohort retention heatmap was developed by grouping customers according to their initial purchase month. Retention percentages were calculated relative to the original cohort size and analysed across subsequent purchasing periods.

Analytical findings:
Cohort month January 2017 with cohort index 12 is identified as having a relatively high customer retention of 0.70%, in comparison to one of the lowest of only 0.02% on December 2017, cohort index 7. Retention on month 0 for all months is 100%, which is expected.
 **     [Identify cohorts with relatively high or low retention. Describe how retention changes between Month 0 and subsequent               months, and whether particular cohorts demonstrate stronger repeat-purchase behaviour.]

5. Which geographical regions generate the greatest concentration of orders?

Analysis performed:
Customer state data was used to develop a geographical visualisation of order distribution across Brazil. Total Orders was used to identify regions with comparatively high or low order volumes.

Analytical findings:
The state of Sao Paulo is easily identified as the state with the highest order volume. This is the only state formatted in a navy blue, with the surrounding states all in a light beige highlighting a low order volume. This implies order activity is highly concentrated, which is somewhat expected as Sao Paulo is the most populous city in Brazil.

6. How does customer purchasing behaviour vary across the marketplace?

Analysis performed:
Customer purchase frequency, order counts, average order value and revenue measures were used to investigate differences in purchasing behaviour. Interactive filtering and drill-through functionality enabled more detailed exploration of selected customer cohorts.

Analytical findings:

**      [Describe the distribution of customer order frequency, differences in purchasing behaviour between cohorts and any notable variations in average order value.]



<img width="721" height="407" alt="Screenshot 2026-11-13 at 13 49 47" src="https://github.com/user-attachments/assets/659bbbaa-74b8-4e54-a42d-38d43caf9015" />


<img width="724" height="409" alt="Screenshot 2026-11-13 at 13 49 56" src="https://github.com/user-attachments/assets/0af7866c-7328-4532-8392-88c69116a8d4" />


<img width="716" height="407" alt="Screenshot 2026-11-13 at 13 50 07" src="https://github.com/user-attachments/assets/79e2882e-97bb-45fe-a543-99b0958c6276" />


______________________________________________________________________________________________________________________________________________________________________________________________
Author Katie Prestwich

Economics BSc Graduate | Aspiring Data Analyst

This project forms part of my data analytics portfolio, demonstrating my application of Power BI, data modelling, DAX and analytical problem-solving to a real-world business dataset.
