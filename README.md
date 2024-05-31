# Just In Time Supply Chain Analytics Project

## Executive Summary

### Key Insights

#### Supply Chain Overview:
- **Revenue by Product Category**: High-performing categories include “Fishing,” “Camping & Hiking,” “Cleats,” “Water Sports,” and “Women’s Apparel.”
- **Revenue by Region and Shipment Delay**: Regions like “Central America” and “Western Europe” exhibit substantial revenue but also face notable shipment delays.
- **Shipment Mode Distribution**: The predominance of modes like “Standard Class” and “Second Class” indicates a focus on fast delivery.

#### Shipment Analysis:
- **Trends in Shipment Processing Days Over Time**: Fluctuations indicate potential periods of operational inefficiencies.
- **Delayed Shipments by Market**: Latin America had the highest number of delayed shipments, while Africa recorded the least on-time shipments.
- **Shipment Mode Performance**: “Same Day Shipment Mode” had the least average shipment processing days, highest on-time delivery rate, and lowest delayed delivery rate.

#### Sales Analysis: Supply vs Demand
- **Product Department Ranked by Supply-Demand Ratio**: The Golf department has the highest supply-demand ratio, indicating a strong balance between inventory levels and customer demand.
- **Sales Performance by Customer Market**: Latin America leads in net sales and total profit, followed by Europe and Pacific Asia.
- **Stock Status Distribution**: 60.14% of the stock is stockout, indicating potential inventory management issues.

#### Product Performance Insights:
- **Top-Performing Products**: Field & Stream Sportsman 16 Gunfire Safe and Perfect Fitness Perfect Rip Deck.
- **Underperforming Products**: Adidas Youth Germany Black/Red Away Match Soc and LIJA Women’s Eyelet Sleeveless Golf Polo.

#### Customer Insights:
- **Trends in Customer Orders, Revenue, and Profit**: Total profit peaked in 2016, with a noticeable drop in customer engagement in 2017.
- **Customer Segmentation Analysis by Country**: The USA had the highest number of customers and orders, followed by Mexico and the UK.

### Business Recommendations
- **Boost Low-Performing Categories**: Implement targeted marketing strategies and promotions.
- **Improve Shipment Efficiency**: Focus on reducing shipment delays, particularly in regions like Latin America and Africa.
- **Address Shipment Mode Issues**: Improve performance of First Class shipment mode and promote Same Day shipment mode.
- **Optimize Inventory Management**: Address high stockout rate by improving inventory forecasting and management.
- **Enhance Product Offerings**: Review and improve underperforming products through innovation or better marketing.
- **Leverage Top-Performing Products**: Ensure sufficient stock and continued promotion of high-performing products.
- **Expand Market Penetration**: Explore growth opportunities in underperforming regions and low-customer countries.
- **Optimize Shipment Processing**: Reduce average shipment processing time for products with longer processing times.

## Dashboard Screenshot

<img src="https://github.com/yanny-alt/Just-in-Time-Supply-Chain-Analysis-/blob/main/images/hMBg84yNUD.png?raw=true" alt="Dashboard Screenshot" title="Just In Time Supply Chain Analytics Dashboard">


[Power BI Link:](https://app.powerbi.com/view?r=eyJrIjoiOGVhMzE4MGQtOTNjYS00ZDljLThlNGYtY2RjNmY1ZjA4OGU2IiwidCI6IjQ5MWM2ZTNhLTA3MjItNDhmMi1iMDFhLWFhMzliODc0MGYxNiJ9)


## Background of the Project

### Introduction
Maintaining a competitive advantage in today’s fast-paced business environment relies heavily on supply chain efficiency. Effective supply chain management ensures timely deliveries, optimal inventory levels, and satisfied customers. As a newly employed data analyst at Just In Time, my main responsibility is to address key shipment and inventory management challenges. This case study emphasizes the significance of supply chain efficiency and the influence of data analytics. By identifying supply chain inefficiencies and generating informative dashboards, my goal is to educate business stakeholders and showcase the potential of data in resolving these challenges.

### Project Background

#### Company Overview
Just In Time is a major player in the logistics and supply chain industry, specializing in providing efficient shipment and inventory management solutions. The company operates globally, serving diverse markets and regions.

#### Challenges Faced
- Shipment delays
- Inconsistent inventory management
- Balancing supply and demand
- Lack of detailed understanding of customer behavior and segmentation

#### Goals of the Analysis
- **Improve Shipment Performance**: Identify and address the root causes of shipment delays. Optimize shipment processing times to enhance delivery efficiency.
- **Optimize Supply-Demand Levels**: Analyze inventory levels to reduce overstock and stockout situations. Implement strategies for better supply-demand balance.
- **Enhance Customer Insights**: Segment customers by market, region, and purchasing behavior. Analyze orders, revenue, and profitability by customer segment. Identify trends and patterns in customer behavior to inform marketing and sales strategies.

## Data Overview

### Data Description
The data for this analysis was spread across three different tables, each containing crucial information for understanding shipment and inventory management at Just In Time.

#### orders_and_shipments.csv
- **Customer ID**: Unique customer identification.
- **Customer Market**: Geographic grouping of customer countries.
- **Customer Region**: Geographic grouping of customer countries.
- **Customer Country**: Customer’s country.
- **Order ID**: Unique order identification.
- **Order Item ID**: Unique order item identification.
- **Order Year/Month/Day**: The year, month, and day of the order.
- **Order Time**: Timestamp of the order in UTC.
- **Order Quantity**: Number of items ordered.
- **Product Department**: Product grouping into categories.
- **Product Category**: Product grouping into categories.
- **Product Name**: Name of the purchased product.
- **Gross Sales**: Revenue before discounts.
- **Discount %**: Discount percentage applied to the catalogue price.
- **Profit**: Profit generated by the sales.
- **Shipment Year/Month/Day**: The year, month, and day of the shipment.
- **Shipment Mode**: How the shipment has been dispatched.
- **Shipment Days — Scheduled**: Typical number of days needed to dispatch the goods.
- **Warehouse Country**: The country of the warehouse that fulfilled the order.

#### inventory.csv
- **Warehouse Inventory**: Monthly product inventory level.
- **Inventory cost per unit**: Monthly storage cost per unit.

#### fulfillment.csv
- **Warehouse Order fulfillment (days)**: Average number of days to refill stock if inventory drops below zero.

### Data Cleaning and Transformation
- **Negative Shipment Time**: Removed records with negative shipment times.
- **Orders Taking Too Long to Ship**: Filtered out orders taking more than 14 days to ship.
- **Correction of Country Names**: Corrected special characters in country names.
- **Data Integrity Check**: Ensured no missing values or duplicated rows.
- **Column Names Standardization**: Removed trailing spaces and ensured uniformity.
- **Date Columns Conversion**: Converted date columns to DateTime data type.

### Measures Created
- **Shipments**: Average Shipment Processing Days, On Time Shipments, Delayed Shipments, On Time Delivery Rate, Delayed Delivery Rate.
- **Sales**: Total Revenue, Total Profit, Profit Margin, Number of Orders, Quantity Sold, Number of Customers, Total Discount Given.
- **Products**: Stock Status (In stock, Stockouts, Overstock).

## Business Analysis and Insights

### Supply Chain Overview
- **Revenue by Product Category**: High-performing categories generate significant revenue, indicating strong market demand.
- **Revenue by Region and Shipment Delay**: Some regions exhibit substantial revenue but also face notable shipment delays.
- **Shipment Mode Distribution**: Focus on fast delivery is crucial for maintaining high customer satisfaction levels.

### Shipment Analysis
- **Trends in Shipment Processing Days Over Time**: Indicates potential periods of operational inefficiencies.
- **Delayed Shipments by Market**: Significant regional disparities in shipment efficiency.
- **Shipment Mode Performance**: Indicates performance issues and areas for improvement.

### Sales Analysis: Supply vs Demand
- **Product Department Ranked by Supply-Demand Ratio**: Indicates balance between inventory levels and customer demand.
- **Sales Performance by Customer Market**: Highlights market performance and areas for improvement.
- **Stock Status Distribution**: Indicates potential inventory management issues.

### Product Performance Insights
- **Sales, Profit, and Discount by Product**: Identifies high-performing and underperforming products.
- **Product Analysis by Category and Department**: Provides insights into product performance and shipment times.
- **Top and Underperforming Products**: Helps identify where to focus improvement efforts.
- **Shipment Processing Time by Product**: Highlights efficiency of shipment processing for different products.

### Customer Insights
- **Trends in Customer Orders, Revenue, and Profit**: Indicates trends in customer engagement and market performance.
- **Customer Purchasing Behavior Over Time**: Shows growth trends and areas for improvement.
- **Customer Segmentation Analysis by Country**: Provides insights into customer base and market penetration.

## Recommendations
- **Boost Low-Performing Categories**: Implement targeted marketing strategies and promotions.
- **Improve Shipment Efficiency**: Optimize logistical operations and enhance shipment planning.
- **Address Shipment Mode Issues**: Improve performance of First Class shipment mode and promote Same Day shipment mode.
- **Optimize Inventory Management**: Improve inventory forecasting and management to balance supply and demand more effectively.
- **Enhance Product Offerings**: Review and improve underperforming products through innovation or better marketing.
- **Leverage Top-Performing Products**: Ensure sufficient stock and continued promotion of high-performing products.
- **Expand Market Penetration**: Explore growth opportunities in underperforming regions and low-customer countries.
- **Optimize Shipment Processing**: Reduce average shipment processing time for products with longer processing times.

## Conclusion
This project provided valuable insights into Just In Time’s supply chain, sales, and customer data. The analysis highlighted key areas for improvement and offered recommendations for optimizing operations and boosting performance. I truly enjoyed working on this project and improving my Power BI skills through data visualization and report creation.

## Dashboard

[Click Here for Full Interaction with the Dashboard](https://app.powerbi.com/view?r=eyJrIjoiOGVhMzE4MGQtOTNjYS00ZDljLThlNGYtY2RjNmY1ZjA4OGU2IiwidCI6IjQ5MWM2ZTNhLTA3MjItNDhmMi1iMDFhLWFhMzliODc0MGYxNiJ9)

## Stay Connected
- **Twitter**: [My Twitter Handle](https://x.com/yannynow)
- **LinkedIn**: [My LinkedIn Profile](https://www.linkedin.com/in/favourokechukwu/)
- **Medium**: [My Medium Profile](https://medium.com/@favour.okechukwu)
- **GitHub**: [My GitHub Profile](https://github.com/yanny-alt)

Thank you for reading and God bless!
