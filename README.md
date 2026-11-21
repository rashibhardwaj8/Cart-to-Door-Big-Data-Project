# CART TO DOOR
### The Hidden Story Behind Every Online Order

## 1. Project Overview
Cart to Door is a Big Data Analytics and Data Engineering project that analyses Brazilian e-commerce data to understand customer orders, delivery performance, payment patterns, product categories and customer reviews.

The project uses Apache Spark and Databricks to process large datasets through a Medallion Architecture (Bronze, Silver and Gold layers), followed by business intelligence analysis using Power BI.

## 2. Problem Statement
E-commerce platforms generate large amounts of data through customer orders, payments, product transactions, deliveries and reviews.

The objective of this project is to process and analyse this data to identify business trends, understand delivery performance, evaluate customer satisfaction and generate meaningful business insights.

## 3. Dataset
**Dataset:** Brazilian E-Commerce Public Dataset by Olist.

The project uses nine CSV files:
- Customers
- Geolocation
- Order Items
- Order Payments
- Order Reviews
- Orders
- Products
- Sellers
- Product Category Name Translation

**Dataset Source:** https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## 4. Technologies Used
- Python
- Apache Spark (PySpark)
- Databricks
- Delta Lake
- Power BI
- Jupyter Notebook
- GitHub

## 5. Project Architecture – Medallion Architecture

### Bronze Layer
- Ingested the nine original CSV datasets into Databricks.
- Stored the raw datasets as Delta tables.
- Created nine Bronze tables.

### Silver Layer
- Removed duplicate records.
- Removed completely empty rows.
- Performed basic data cleaning.
- Created nine Silver tables.

### Gold Layer
Created seven analytical tables:
- Monthly Orders
- Order Status
- Payment Summary
- Category Summary
- Delivery Performance
- Review Summary
- Delivery Review Summary

## 6. Data Analysis
The project explores:
- Monthly order trends.
- Order status distribution.
- Payment method analysis.
- Product category performance.
- Delivery time and delivery status.
- Customer review ratings.
- Relationship between delivery performance and customer satisfaction.

## 7. Power BI Dashboard
The project includes two dashboard pages:

**Delivery Dashboard**
- Delivery status distribution.
- Average delivery days.
- Order count.
- State-wise delivery performance.

**Customer Reviews**
- Review sentiment distribution.
- Average ratings by delivery status.

## 8. Project Structure
- notebooks/ – Individual analysis and Databricks notebooks.
- data/processed/ – Processed analytical CSV outputs.
- dashboard/ – Power BI dashboard and exported PDF.
- documentation/ – Project architecture diagram.
- screenshots/ – Databricks execution screenshots.
- PROJECT_NOTES.md – Project notes.

## 9. Team Members and Contributions

| Team Member | Contribution |
|---|---|
| Rashi Bhardwaj | Data understanding, Spark analysis, Databricks Medallion pipeline, project integration |
| Ashish | Customer and order analysis |
| Kunal | Delivery analysis, customer review analysis and Power BI dashboard |
| Palak | Project coordination and presentation/documentation support |

*The team worked collaboratively on project integration and final submission.*

## 10. Results
- Nine original datasets loaded into Databricks.
- Nine Bronze Delta tables created.
- Nine Silver Delta tables created.
- Seven Gold analytical tables created.
- Total of 25 project tables verified.
- Power BI dashboard prepared for delivery and customer review analysis.

## 11. Limitations
- The project uses a publicly available historical dataset.
- Automated API-based ingestion was not implemented.
- The Power BI dashboard's direct live connection to Databricks Gold tables has not been independently verified.

## 12. Conclusion
Cart to Door demonstrates how large-scale e-commerce data can be organised, cleaned, transformed and analysed using Apache Spark and Databricks. The resulting analytical datasets and Power BI dashboard help translate raw transaction data into meaningful business insights.

---
**Project:** Cart to Door – The Hidden Story Behind Every Online Order  
**Domain:** Big Data Analytics and Data Engineering
