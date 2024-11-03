# CUSTOMER-DATA-ANALYSIS

# Customer Segmentation Analysis Project Documentation and Report

# Project Overview

The Customer Segmentation Analysis project aimed to analyze customer data for a subscription service to identify segments and trends. The project utilized Excel, SQL, and Power BI to uncover insights on customer behavior, subscription patterns, and revenue trends.

# Project Objectives

1. Analyze customer data to identify segments and trends.
2. Understand customer behavior and subscription patterns.
3. Identify key trends in cancellations and renewals.
4. Develop a Power BI dashboard to visualize key insights.

# Methodology

1. Data Collection: Customer data was collected from the company's database.
2. Data Analysis: Excel and SQL were used to analyze customer data.
3. Data Visualization: Power BI was used to create interactive dashboards.

 # Results

# Customer Segmentation

1. Regional Analysis: Customers are concentrated in East(25.11%), South (25.02%), west (24.97%) and North (24.9%).
2. Subscription Types: Basic(50.1%), Premium(25.02), Standard(24.97)


# Subscription Trends

1. Average Subscription Duration: 12 months.
2. Cancellation Rate: 20% of customers cancel within 6 months.
3. Revenue Trends: Monthly subscriptions generate 50% of total revenue.

```SQL

select * from [dbo].[sales data]

select Product , sum (revenue) as Total_sales from [dbo].[sales data]
GROUP BY product 

select Region, count ( orderID ) as Num_transaction from [dbo].[sales data] 
GROUP BY Region

select Product , sum (revenue) as Total_sales from [dbo].[sales data]
GROUP BY product
ORDER BY   Revenue asc 

select product , sum ( revenue ) as total_revenue 
from [dbo].[sales data]
group by product 


select (OrderDate ) as sales_month , sum(revenue) as Total_sales 
from [dbo].[sales data] 
where year ( 2034-08-11) 
group by OrderDate

select customer_id, sum(revenue) as total_purchase 
from [dbo].[sales data] 
group by customer_id 
order by  2 desc 

select Region , sum(revenue) / (select sum (revenue) 
from [dbo].[sales data]) * 100 as sales_percentage 
from [dbo].[sales data]
group by region

```
# Power BI Dashboard

The dashboard visualizes key insights on customer segmentation, subscription trends, and revenue analysis.

# Recommendations

1. Target marketing efforts towards North and West.
2. Offer incentives for annual subscriptions.
3. Improve customer retention strategies.

# Conclusion

The Customer Segmentation Analysis project provided valuable insights into customer behavior and subscription patterns. The Power BI dashboard enables interactive visualization of key metrics.


