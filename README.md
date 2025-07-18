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
