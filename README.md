# DSA-SQL-PROJECT
My developmental milestone in DSA
- SQL
  ###### DATA ANALYSIS
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


1. Which product category had the highest sales?

SELECT TOP 1 [Product_Category],SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Product_Category]
ORDER BY Total_Sales DESC;

2. What are the Top 3 and Bottom 3 regions in terms of sales?


SELECT TOP 3 Region,SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY Region
ORDER BY Total_Sales DESC;


2b. Bottom 3
SELECT TOP 3 Region,SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY Region
ORDER BY Total_Sales ASC;

3. What were the total sales of appliances in Ontario?

SELECT Region,  Product_Sub_Category, SUM(Sales) AS TotalSales
FROM [dbo].[KMS Sql Case Study]
WHERE Region = 'Ontario'
AND Product_Sub_Category = 'Appliances' 
GROUP BY Region,  Product_Sub_Category
ORDER BY TotalSales desc


4. Advise the management of KMS on what to do to increase the revenue from the bottom 
10 customers

SELECT TOP 10 Customer_Name, SUM(sales) AS total_sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY Customer_Name
ORDER BY total_sales ASC;


5.KMS incurred the most shipping cost using which shipping method?

SELECT TOP 1 [Ship_Mode], SUM([Shipping_Cost]) AS Total_Shipping_Cost
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Ship_Mode]
ORDER BY Total_Shipping_Cost DESC;

6. Who are the most valuable customers, and what products or services do they typically 
purchase? 

SELECT [Customer_Name],[Product_Name],
SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Customer_Name], [Product_Name]
ORDER BY Total_Sales DESC;

7. Which small business customer had the highest sales?

SELECT TOP 1 Customer_Name, SUM(Sales) AS Total_Sales
FROM [dbo].[KMS Sql Case Study]
WHERE Customer_Segment = 'Small Business'
GROUP BY [Customer_Name]
ORDER BY Total_Sales DESC;


8. Which Corporate Customer placed the most number of orders in 2009 – 2012?

SELECT TOP 1 Customer_Name, COUNT(DISTINCT Order_ID) AS Number_of_Orders
FROM [dbo].[KMS Sql Case Study]
WHERE customer_Segment = 'Corporate'
AND Order_Date BETWEEN '2009-01-01' AND '2012-12-31'
GROUP BY Customer_Name
ORDER BY Number_of_Orders DESC;

9. Which consumer customer was the most profitable one? 

SELECT TOP 1 [Customer_Name], SUM(Profit) AS Total_Profit
FROM [dbo].[KMS Sql Case Study]
WHERE [Customer_Segment] = 'Consumer'
GROUP BY [Customer_Name]
ORDER BY Total_Profit DESC;

10. Which customer returned items, and what segment do they belong to? 

SELECT DISTINCT [Customer_Name], [Customer_Segment]
FROM [dbo].[KMS Sql Case Study]
WHERE [Returned] = 'Yes';

SELECT TOP 10 * FROM [dbo].[KMS Sql Case Study]
WHERE [Returned] IS NOT NULL;

11. If the delivery truck is the most economical but the slowest shipping method and 
Express Air is the fastest but the most expensive one, do you think the company 
appropriately spent shipping costs based on the Order Priority? Explain your answer 

SELECT
[Order_Priority], [Ship_Mode], COUNT([Order_ID]) AS OrderCount,
ROUND(SUM(Sales - Profit), 2) AS EstimatedShippingCost,
AVG(DATEDIFF(day, [Order_Date], [Ship_Date])) AS AvgShipDays
FROM [dbo].[KMS Sql Case Study]
GROUP BY [Order_Priority], [Ship_Mode]
ORDER BY [Order_Priority], [Ship_Mode] DESC;




![IMG-20250706-WA0001](https://github.com/user-attachments/assets/ff8011f3-a998-4116-a588-c8ab3d8fbb24)



