
# Zesty Drinks Analysis Project

*End-to-End Business Intelligence Solution using Snowflake + Power BI*

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

Tasks completed:

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
     
3. **Product Performance Dashboard**
   * Total Discount, Inventory Value, Average Revenue per customer
     
4. **Inventory Dashboard**
   * Total Inventory, Total Reorder Level, Average Reorder Level
     
5. **Shipping & Delivery Dashboard**
   * Total Shipping Cost, Total Shipments, Average Carrier Rating

### **6. Deployment (Power BI Service)**

* Published the report to a Power BI Workspace to simulate real-world publishing and version control.
* Created a Power BI App experience to package related reports and make them easy to navigate as a user-facing product.
* Configured scheduled refresh using sample data sources to replicate automated pipeline behavior.
* Implemented Row-Level Security (RLS) by designing roles and testing access using the “View As” feature.

---

# Key Features of the Solution

* End-to-end BI pipeline (Snowflake → Power Query → Power BI → Service)
* Clean, intuitive dashboards covering all business domains
* Fully documented DAX library
* Scalable data model designed for enterprise use
* Business insights surfaced for decision-making

---

# Author

**Jeseena Parveen K**
Aspiring Data Analyst | Power BI | SQL | Python
LinkedIn / Portfolio links

---
