# DSA-SQL-PROJECT
My developmental milestone in DSA
- SQL


KMS Business Intelligence Capstone Report

Project Title

Data-Driven Business Performance Analysis for KMS: Trends in Sales, Shipping, and Customer Activity (2009–2012)

Project Summary

This project presents a comprehensive analysis of Kultra Mega Stores (KMS), a Nigerian-based company operating in the retail and wholesale markets for office supplies and furnishings. KMS serves a diverse client base:

Private individuals (Consumer)

Small-scale enterprises (Retail)

Large corporations (Wholesale)


Operating across several regions, KMS seeks to strengthen its performance—particularly within the Abuja zone—through insights grounded in data analytics.


---

Project Purpose

As a Business Intelligence Analyst, you were tasked to:

Explore sales, shipping, and customer datasets spanning 2009 to 2012

Detect trends, performance gaps, and inefficiencies

Recommend solutions to boost revenue and control operational costs



---

Technologies Employed

SQL: Employed for data extraction, transformation, and aggregation

GitHub: Utilized for portfolio presentation and project tracking



---

Key Takeaways

Technology Products: Outperformed all other categories in sales

Top Performing Region: Abuja led overall performance; Ibadan fell behind

Logistics Insight: First Class shipping was the most expensive

Customer Strategy: Incentives should target low-engagement customers

High-Value Customers: Mainly purchased high-margin tech and office items



---

Approach to Analysis

1. Database Setup: Imported the dataset into SQL Server


2. Schema Design: Created structured tables and defined appropriate data types


3. Preprocessing: Addressed missing values and cleaned raw data


4. Query Development: Designed SQL scripts for business-specific inquiries


5. Insight Derivation: Interpreted results to drive actionable conclusions


6. Communication: Documented key findings and aligned them with business goals







CASE SCENARIO I: Regional & Product Performance

1. Which category generated the highest sales?

Answer: Technology

Impact:

Indicates robust demand and pricing power

Aligns with B2B clients’ purchasing behaviors

Potential for ongoing revenue through recurring purchases


Recommendations:

Profile buyers of tech products by customer segment

Focus inventory on top-selling gadgets

Promote product bundles (e.g., laptop + accessories)



---

2. Regional Sales Ranking

Top Regions:

Abuja

Lagos

Port Harcourt


Underperformers:

Ibadan

Kano

Benin


Insights:

Strong sales regions benefit from urbanization and supply chain effectiveness

Low performers may suffer from logistics gaps or low brand awareness


Suggestions:

Expand investment in high-performing zones

Conduct localized promotions and partnership strategies in weaker markets




---

3. Ontario’s Appliance Sales

Finding: Low-to-average appliance sales

Potential Causes:

Limited customer interest

Poor promotion or product availability


Recommendations:

Minimize appliance stock in Ontario

Pair appliances with more popular product bundles

Study market gaps or competitors



---

4. Bottom 10 Customers

Insight:
These clients generate minimal revenue but offer growth potential

Recommended Actions:

Classify them by segment and purchase behavior

Use personalized incentives or loyalty offers

Assign dedicated follow-up from sales reps


---

5. Costly Shipping Method

Insight: First Class shipping significantly increases delivery costs

Implications:

Frequently selected for orders that don’t require fast delivery

Suggests need for stricter criteria or policy adjustment


Recommendations:

Apply premium shipping only for urgent or valuable orders

Set order thresholds for free/discounted shipping

Encourage cost-efficient alternatives


---

CASE SCENARIO II: Customer Performance Evaluation

6. High-Spending Corporate Clients

Insight: These customers frequently order tech and furniture

Recommendations:

Offer dedicated account management

Tailor bundled packages and loyalty rewards



---

7. Loyal Small Business Buyer

Insight: This customer’s repeat purchases indicate reliability

Suggestion:

Provide subscription or reorder options

Launch business-specific loyalty offers



---

8. Frequent Order Customer

Insight: Prioritizes regular delivery over large one-time purchases

Strategy:

Introduce long-term supply agreements

Offer volume discounts



---

9. High-Margin, Low-Risk Customer

Insight: Consistent purchases without discounts or returns

Recommendations:

Understand their purchase patterns

Reward loyalty and encourage referrals


---

10. Customer Returns Insight

Insight: Retail and consumer segments show higher return rates

Recommendations:

Improve product clarity and order verification

Offer real-time support for high-return segments


11. Shipping Priority Mismatch

Finding:

Premium shipping used for low-priority orders

Slow methods assigned to urgent orders


Implications:

Missed SLAs and added cost

Indicates manual errors or lack of automation


Recommendations:

Automate shipping decisions by urgency

Train staff and update internal guidelines

Allow customers to choose speed vs. cost






  ###### DATA ANALYSIS
  create database


  
  use database


  
  create sale table


  
  alter sale table

  


1. Which product category had the highest sales?


![IMG-20250706-WA0005](https://github.com/user-attachments/assets/5baaf6aa-35d1-4b8e-9a86-2df05b28cb37)



  2a. What are the Top 3 in terms of sales
  
  
  ![IMG-20250706-WA0006](https://github.com/user-attachments/assets/23414816-0694-488e-8290-ca89e1e3f9b9)

  
  
  2b. what are the Bottom 3 regions in terms of sales?



![IMG-20250706-WA0007](https://github.com/user-attachments/assets/0270e655-78d0-4a1f-99fd-1c7c4f808a2b)

  



3. What were the total sales of appliances in Ontario?

![IMG-20250706-WA0008](https://github.com/user-attachments/assets/03a27f15-4cf9-445d-8d1b-ec650d4cb856)


4. Advise the management of KMS on what to do to increase the revenue from the bottom 
10 customers


![IMG-20250706-WA0009](https://github.com/user-attachments/assets/38f82705-f023-4d87-9991-d117877e8629)


5.KMS incurred the most shipping cost using which shipping method?


![IMG-20250706-WA0010](https://github.com/user-attachments/assets/2bd05505-b87e-4390-aaf0-f61e4dbca40f)


6. Who are the most valuable customers, and what products or services do they typically 
purchase? 


![IMG-20250706-WA0011](https://github.com/user-attachments/assets/2337e2e3-d699-4ea2-bceb-1c4b36fa3063)


7. Which small business customer had the highest sales?

![IMG-20250706-WA0012](https://github.com/user-attachments/assets/d28853f1-080d-47fd-8f81-06806760c38a)


8. Which Corporate Customer placed the most number of orders in 2009 – 2012?


   ![IMG-20250706-WA0013](https://github.com/user-attachments/assets/eb569f6d-a1c6-4fc5-b63b-a17d1686d79e)


 9. Which consumer customer was the most profitable one?
  

  ![IMG-20250706-WA0014](https://github.com/user-attachments/assets/5b465186-da0e-43f1-b007-46c90648fcc1)



10. Which customer returned items, and what segment do they belong to?


![IMG-20250706-WA0015](https://github.com/user-attachments/assets/936989e1-b0b6-445b-8d12-d0ba52359e47)



11. If the delivery truck is the most economical but the slowest shipping method and 
Express Air is the fastest but the most expensive one, do you think the company 
appropriately spent shipping costs based on the Order Priority? Explain your answer 



![IMG-20250706-WA0016](https://github.com/user-attachments/assets/76751e31-a7d5-4e90-b23b-d3262ad41fcd)


  
  ```Step 1: Create the database
CREATE DATABASE KMS_database;

-- Use the database
USE KMS_database;

Create the sales table with all your listed columns
CREATE TABLE sales (
    row_id INT PRIMARY KEY AUTO_INCREMENT,
    order_id VARCHAR(50),
    order_date DATE,
    order_priority VARCHAR(20),
    order_quantity INT,
    sales DECIMAL(10,2),
    discount DECIMAL(5,2),
    ship_mode VARCHAR(30),
    profit DECIMAL(10,2),
    unit_price DECIMAL(10,2),
    shipping_cost DECIMAL(10,2),
    customer_name VARCHAR(100),
    province VARCHAR(100),
    region VARCHAR(50),
    customer_segment VARCHAR(50),
    product_category VARCHAR(50),
    product_sub_category VARCHAR(50),
    product_name VARCHAR(150)
);




``` USE KMS_database;

ALTER TABLE sales
ADD COLUMN product_container VARCHAR(50),
ADD COLUMN product_base_margin DECIMAL(5,2),
ADD COLUMN ship_date DATE;
``` select * from [dbo].[KMS Sql Case Study]

``` SELECT TOP 1 [Product_Category],SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Product_Category]
ORDER BY Total_Sales DESC;


```SELECT TOP 3 Region,SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY Region
ORDER BY Total_Sales DESC;



```SELECT TOP 3 Region,SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY Region
ORDER BY Total_Sales ASC;


```SELECT Region,  Product_Sub_Category, SUM(Sales) AS TotalSales
FROM [dbo].[KMS Sql Case Study]
WHERE Region = 'Ontario'
AND Product_Sub_Category = 'Appliances' 
GROUP BY Region,  Product_Sub_Category
ORDER BY TotalSales desc



```SELECT TOP 10 Customer_Name, SUM(sales) AS total_sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY Customer_Name
ORDER BY total_sales ASC;


``` SELECT TOP 1 [Ship_Mode], SUM([Shipping_Cost]) AS Total_Shipping_Cost
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Ship_Mode]
ORDER BY Total_Shipping_Cost DESC;



``` SELECT [Customer_Name],[Product_Name],
SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Customer_Name], [Product_Name]
ORDER BY Total_Sales DESC;



``` SELECT TOP 1 Customer_Name, SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
WHERE Customer_Segment = 'Small Business'
GROUP BY [Customer_Name]
ORDER BY Total_Sales DESC;


``` SELECT TOP 1 Customer_Name, COUNT(DISTINCT Order_ID) AS Number_of_Orders
FROM [dbo].[KMS Sql Case Study]
WHERE customer_Segment = 'Corporate'
AND Order_Date BETWEEN '2009-01-01' AND '2012-12-31'
GROUP BY Customer_Name
ORDER BY Number_of_Orders DESC;



``` SELECT TOP 1 [Customer_Name], SUM(Profit) AS Total_Profit
FROM [dbo].[KMS Sql Case Study]
WHERE [Customer_Segment] = 'Consumer'
GROUP BY [Customer_Name]
ORDER BY Total_Profit DESC;



``` SELECT DISTINCT [Customer_Name], [Customer_Segment]
FROM [dbo].[KMS Sql Case Study]
WHERE [Returned] = 'Yes';

SELECT TOP 10 * FROM [dbo].[KMS Sql Case Study]
WHERE [Returned] IS NOT NULL;


``` SELECT
[Order_Priority], [Ship_Mode], COUNT([Order_ID]) AS OrderCount,
ROUND(SUM(Sales - Profit), 2) AS EstimatedShippingCost,
AVG(DATEDIFF(day, [Order_Date], [Ship_Date])) AS AvgShipDays
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Order_Priority], [Ship_Mode]
ORDER BY [Order_Priority], [Ship_Mode] DESC;



