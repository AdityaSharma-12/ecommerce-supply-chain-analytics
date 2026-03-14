# E-Commerce Supply Chain & Customer Experience Analytics 📊

## 📋 Project Overview
This project involves a comprehensive Power BI dashboard designed to analyze the supply chain performance and customer satisfaction of a Brazilian e-commerce marketplace (Olist). The goal was to identify the root causes of negative customer reviews by bridging the gap between logistics data and customer sentiment.

## 🎯 Problem Statement
The e-commerce platform was experiencing a high volume of 1-star reviews. Management suspected that regional shipping bottlenecks and extended delivery times were the primary drivers of customer dissatisfaction but lacked the analytical visibility to prove it or identify the worst-performing sellers.

## 🛠️ Tools & Technologies Used
- **Microsoft Power BI:** Data modeling, DAX calculations, and interactive data visualization.
- **Power Query:** Data extraction, cleaning, handling null values, and translating Portuguese product categories to English.
- **DAX (Data Analysis Expressions):** Created custom measures for tracking Average Delivery Lead Time, Total Revenue, and Customer Satisfaction (CSAT) scores.

## 🏗️ Data Architecture & Modeling
Built a robust **Snowflake Schema** connecting over 100,000 real-world order lifecycles. The model connects a central `Order Items` Fact Table to multiple Dimension Tables (Customers, Sellers, Products, Reviews) via 1-to-Many relationships to ensure accurate cross-filtering.

## 💡 Key Insights Discovered
1. **Delivery Delays Destroy Satisfaction:** The scatter plot analysis definitively proved that as delivery times extend past 15 days, customer reviews plummet directly to 1-star ratings.
2. **Geographical Bottlenecks:** The geospatial map highlights that while São Paulo drives the highest volume of orders, peripheral states experience disproportionately high delivery delays.
3. **Actionable Accountability:** Developed a "Worst Offenders" matrix that automatically flags high-volume sellers with the longest delivery times and lowest review scores, allowing management to intervene.

## 🖼️ Dashboard Previews

### 1. Executive Command Center
*(Provides a high-level view of revenue trends, total orders, and geographical performance)*
(01_executive_command_center.png)

### 2. Customer Experience Analysis
*(Maps the direct correlation between delivery days and review scores, highlighting worst-offending sellers)*
(02_customer_experience.png
## 📂 Files Included
- `Ecommerce_Dashboard_Template.pbit`: The complete Power BI project file (requires Power BI Desktop to open).
- `Dashboard_Export.pdf`: A static PDF export of the final dashboard pages.
- Dataset:https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce
