
# Zesty Drinks Analysis Project

*End-to-End Business Intelligence Solution using Snowflake + Power BI*

<p align="center">

<!-- Project Badges -->
<br>

<img src="https://img.shields.io/badge/Project-Zesty%20Drinks-4B9CD3?style=flat" />
<img src="https://img.shields.io/badge/Tech-Snowflake%20%7C%20%7C%20PowerBI-6C63FF?style=flat" />
<img src="https://img.shields.io/badge/EDA-Exploratory%20Data%20Analysis-brightgreen?style=flat" />
<img src="https://img.shields.io/badge/PowerBI-Reporting%20%26%20Dashboards-F2C811?style=flat" />
<img src="https://img.shields.io/badge/Status-Completed-success?style=flat" />


<br>

<br>

<!--  Name Badge  -->

<img src="https://img.shields.io/badge/Jeseena Parveen K-Data%20Analyst-pink?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTIiIGhlaWdodD0iMTIiIHZpZXdCb3g9IjAgMCAxMiAxMiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48Y2lyY2xlIGN4PSI2IiBjeT0iNiIgcj0iNiIgZmlsbD0iI0ZGRiIvPjwvc3ZnPg==" />

<!--  LinkedIn Badge -->

<a href="https://www.linkedin.com/in/jeseena-parveen-k/">
<img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin" />
</a>

</p>

---

## Project Overview

Zesty Drinks (fictional beverage company) wanted a unified analytics solution to answer key business questions:

* **Who their customers are and what they prefer**
* **Which products perform well or need attention**
* **Inventory health (shortages, overstock, trends)**
* **Shipping & delivery efficiency**
* **Overall business trends over time**

To help Zesty Drinks drive smarter decisions and future growth, I designed and developed a complete suite of interactive dashboards and reports across all major business functions.

---

# Project Workflow 

### **1. Data Loading (Snowflake → Power BI)**

* Connected Snowflake using Power BI's built-in connector
* Extracted tables: Channel, Customers, Date, Products, Promotions, Region, Factory, Shipment, Store, Warehouse, Inventory, Production, Sales, Shipping
* Validated row counts and schema before loading

### **2. Data Cleaning (Power Query)**

* Standardized column names
* Removed duplicates & null-heavy rows
* Fixed data types (dates, currency, numeric fields)
* Merged lookup tables where needed
* Added calendar and hierarchy fields
* Created Age Group custom column using conditional logic

### **3. Data Modeling**

Built a **star schema**:

* **Fact Tables:** Inventory, Production, Sales, Shipping
* **Dimension Tables:** Channel, Customers, Date, Products, Promotions, Region, Factory, Shipment, Store, Warehouse

<img width="1402" height="710" alt="image" src="https://github.com/user-attachments/assets/df864555-04b1-413e-9ed6-2252dbcc8eee" />

### **4. Data Analysis (DAX)**

Created measures for:

* Business Overview
* Customer Insights
* Product Insights
* Inventory Insights
* Shipping Insights

### **5. Visualization & Dashboard Design**

Dashboards built:

1. **Business Overview Dashboard**
   * Total Revenue, Total Profit, Total Units Sold, Profit Margin %, Sales Growth %
     
2. **Customer Insights Dashboard**
   * Average Revenue per customer, Total Customers, Gold Tier Customers
     
3. **Product Insights Dashboard**
   * Total Discount, Inventory Value, Average Revenue per customer
     
4. **Inventory Insights Dashboard**
   * Total Inventory, Total Reorder Level, Average Reorder Level
     
5. **Shipping Insights Dashboard**
   * Total Shipping Cost, Total Shipments, Average Carrier Rating

### Dashboard

## **Business Overview Insights**
<img width="1142" height="638" alt="image" src="https://github.com/user-attachments/assets/2c1e8cd9-3ada-4e52-93c0-c5be4a418004" />

* The business generated **$275M in revenue** and **$105M profit**, maintaining a strong **38% profit margin**.
* **Sales Growth is slightly negative (-0.35%)**, indicating flat or declining demand.
* **Asia accounts for ~86% of total units sold**, making it the primary driver of performance.
* Top revenue-generating countries include **Indonesia, Thailand, Pakistan, India, and Australia**.
* Revenue and profit trends show similar peaks in **2020** and **2022**, suggesting stable cost structure and demand-driven performance.
* North America and Australia contribute minimally, highlighting opportunities for **regional expansion and diversification**.

## **Customer Insights**
<img width="1143" height="648" alt="image" src="https://github.com/user-attachments/assets/2b1c106c-62c0-4f46-af93-8131787ca8d0" />

* Adults and Young Adults drive the majority of revenue, contributing $143M and $80M respectively.
* Customer segmentation is evenly split across Regular, Business, and Premium tiers (~33% each), indicating a balanced customer mix.
* Gender distribution is nearly even (Male 50.4%, Female 49.6%).
* 3,406 Gold-tier customers reflect strong loyalty and retention.

## **Product Insights**
<img width="1147" height="648" alt="image" src="https://github.com/user-attachments/assets/80856073-84fe-4d7d-8905-ad4292e9f109" />

* Top-performing categories include Soda, Milkshake, and Iced Tea, which also show the highest profit contribution.
* Ginger and Lime are the leading flavors, driving multi-category revenue.
* Major cost contributors are Milkshake ($26M), Iced Tea ($22M), and Energy Drink ($20M), highlighting areas for cost optimization.
* Product revenue distribution shows strong preference toward refreshing beverage categories over Coffee and Juice.

## **Inventory Insights**
<img width="1156" height="653" alt="image" src="https://github.com/user-attachments/assets/2fcdd9a0-d896-4f17-9e87-6799e9afe0ef" />

* Inventory value peaked in 2022 ($36.47M) and declined to $21.04M in 2023, indicating reduced stock levels or improved turnover.
* Soda, Milkshake, and Iced Tea have the highest inventory + reorder levels, aligning with their high demand.
* Coffee and Juice have lower stock levels, suggesting possible understocking or lower demand.
* Average reorder level sits at $274.57M, pointing to large-scale replenishment cycles.

## **Shipping Insights**
<img width="1153" height="648" alt="image" src="https://github.com/user-attachments/assets/82a0e88b-cc38-4fe1-af51-89c7e6478224" />

* Total shipping cost remains stable at $5.44M–$5.56M over five years.
* Sea transport is the most utilized shipping mode (23 shipments), followed by Road (20) and Air (19).
* Asia drives the majority of shipping costs ($23.6M), reflecting its dominance in sales and operational activity.
* With 75 total shipments and an average rating of 4.0, logistics performance appears reliable.

## Recommendations:
1. Address Flat Sales Growth
- Investigate demand stagnation in key regions and product categories.
- Introduce targeted promotions for underperforming segments (Teens, Seniors, Coffee, Juice).

2. Strengthen High-Value Segments
- Prioritize marketing and retention efforts for Adults and Young Adults, who contribute the most revenue.
- Expand premium offerings around top-performing flavors (Ginger, Lime).

3. Optimize Inventory Management
- Maintain strong stock levels for high-demand categories (Soda, Milkshake, Iced Tea).
- Reassess reorder thresholds for Coffee and Juice to avoid stockouts or overstocking.
- Continue monitoring downward inventory trends to ensure they reflect efficiency—not shortages.

4. Improve Cost Efficiency
- Conduct cost analysis for high-cost product categories (Milkshake, Iced Tea, Energy Drink).
- Explore supplier negotiations or production optimization.

5. Enhance Logistics Performance
- Focus on optimizing Asian shipping routes, as they account for the majority of costs.
- Review Sea freight efficiency since it's the most used mode—opportunities may exist for better rates or faster timelines.
- Monitor carrier ratings to ensure consistent service quality above 4.0.
   
### **6. Deployment (Power BI Service)**

* Published the report to a Power BI Workspace to simulate real-world publishing and version control.
* Created a Power BI App experience to package related reports and make them easy to navigate as a user-facing product.
* Configured scheduled refresh using sample data sources to replicate automated pipeline behavior.
* Implemented Row-Level Security (RLS) by designing roles and testing access using the “View As” feature.

# Key Features of the Solution

* End-to-end BI pipeline (Snowflake → Power Query → Power BI → Service)
* Clean, intuitive dashboards covering all business domains
* Fully documented DAX library
* Scalable data model designed for enterprise use
* Business insights surfaced for decision-making

---

