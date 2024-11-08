# CAPSTONE PROJECT 1
## PROJECT TITTLE: SALES DATA ANALYSIS
---
- [Project overview](#project-overview)
- [Data Characteristics](#data-characteristics)
- [Data Description](#data-description)
- [Basic Statistics in the Dataset](#basic-statistics-in-the-dataset)
- [Methodology](#methodology)
- [Dashboard Review](#dashboard-review)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [SQL Query]([#sql-query)
- [Data Analysis and Insight Generation](#data-analysis-and-insight-generation)
- [SQL Query Document](#sql-query-document)
- [Power BI Dashboard](#power-bi-dashboard)
- [Conclusion](#conclusion)
  
---
# Project overview:
---
This project involves analyzing sales data to uncover insights and trends that inform business decisions.
using [dataset/sorces], i explored various aspects of sales performance,including:
---
Data Description:
- Dataset: [dataset name]
- source: [data source]
- size: [Number of rows]*[Number of columns]
- Columns:
  - Sales ID
  - Product Name
  - Category
  - Region
  - Date
  - Sales Amount
---
  ### Data Characteristics:
---
The dataset includes the following variables:
1. OrderID : Unique identification of each order purchased by the customers.
2. CustomerID : Unique identification for each customer.
3. Product : Items purchased by the customers.
4. Region : 
5. Order Date : Date when the items(products) were purchased.
6. Quantity : The amount of items purchased in each transaction.
7. Unit Price : The cost price of each item purchased.
8. Revenue : The revenue generated when the items were sold.
9. Sales : the money gotten when the item were sold.
10. Average : The average of sale.
---
 ## BASIC STATISTICS IN THE DATASET
---
1. Total Sales: 2.1 Million
2. Average Sales: 211.8
3. Total Customer: 9921
4. Marginal Profit: 1.8 Million
5. Total Quantity: 68.5K
---
## METHODOLOGY
### Data Preparation
---
* Removing duplicates
Eliminated duplicated records to ensure Data Quality.
---
Dashboard Review:
---
- Dashboard name: sales performance dashboard
- purpose: visualize key sales metrics and trends
- Component:
- Sales by Region
- Top-selling products
- Sales trend overtime
- Category-wise sales

---
Data Source:
---
- Source:
-  [database name ]
- Type:
- [relational database, CSV file, etc.]
- Connection:
- [ODBC,API,etc.]

---
## TOOLS USED:
---
1. Microsoft Excel: Used for data cleaning, analysis and creating pivot visualization [DOWNLOAD HERE](HTTP://WWW.MICROSOFT.COM/EN-US/MICROSOFT-365/EXCEL)
2. MIcrosoft SQL server (SMSS): Used for pre-processing [DOWNLOAD HERE](HTTP://WWW.MICROSOFT.COM/EN-US/SQL-SERVER/SQL-SERVER-DOWNLOADS)
3. Microsoft Power BI desktop: Used for creating dashboards and visualization [DOWNLOAD HERE](HTTP://WWW.MICROSOFT.COM/EN-US/DOWNLOAD/DETAILS.ASPX?ID=58494)

---
Data Cleaning and preparation:
---
1. Handling missing values
2. Data normalization
3. Data tranformation
4. Data quality checks

---
SQL QUERY:
---
--
SELECT
     [Columns]
--     
FROM
    [table]
--    
WHERE
     [condition]
 --    
GROUP BY
        [columns]
--        
ORDER BY
       [columns];
 --      

---

## Data Analysis and Insight Generation
This visualization tells us what the customers patronize the most and how they shop. this reveals to us what they purchase the most and the least and at what time and period they shop most and also the regions with the highest revenue generated.
1. REGIONAL BREAKDOWN : The pie cahrt and bar chart visualization on region revealed the rate and revenue generated by each region. The region with the highest rate and revenue is South with a rate of 44.16% with 928K generated, then the East had 23.13% with 486K generated, the North had 18.42% and 387K generated, and lastly the West had 14.29% and 300K generated. The difference between the South and Other regions is a very huge which means that the other regions are underperforming when it comes to certain products, perhaps due to the stores in those regions not having what the customers are more in-need of in relations to their environment.
   RECOMMENDATION : conduct a targeted marheting campaign focusing more on the most popular products for each region and giving didcounts and promotion to the products that are not-so popular to encourage customers to purchase them. it is also recommended to move the most demanded products of a region to that region to control loss of profit in a region, for example shoes are purchased better in the south bringing more than 500K but in the west, it brings just 30K so brings the more shoes to the south where they are more in demand is good for company profit and customer satisfaction.
2. PRODUCT PERFORMANCE :  The bar and column charts visualization on sales reveal the revenue generated by each product and that certain products perform better. the product with the highest revenue is Shoe which generated 613K, followed by Shirt with 486K, Hat with 316K, Gloves with 297K, Jacket with 208K and finally Socks with 181K with the lowest revenue. this might also be as a result of customer want in relations to environment.
   RECOMMENDATION : Allocate more marketing resources to the high and better-performing products being shoes and shirts and hats and promote them on digital and social channels. the other can be introduced as complementary products to encourage upselling and analyze trend-basd demand spikes to adjust stock levels in advance to prevent profit loss.
 3. SALES TREND OVER TIME : The column and line charts Visualization represent the monthly and quarterly sales repectively. The monthly reveals that febuary has the highest revenue turnover and that september has the lowest revenue turnover. the charts also reveals seasonal spikes during seasons such as Winter and Summer and drop-down during spring and autumn, the charts shows a rise during the Winter months(December, january, February) and a fall during the Spring months(March, April, May), then another rise in the Summer months(June, July, August) and finally a fall in the Autumn months(September, October, November), in a way the monthly trend moved like a wave. The quarterly line graph shows that the highest quarter is the first quarter and the lowest is the last quarter and it also moves like a wave.
    RECOMMENDATION : Plan targeted marketing campaigns around peak sales periods to maximize engagement and offer special discounts or promotions during off-peak periods to drive sales and smooth out fluctuations. prepare contingency plans for significant trend fluctuations, and also track trending products to understand customer preferences and develop new and improved versions. 
1. Top selling product by region
2. sales trend analysis (seasonality,quarterly)
3. category wise sales performance
4. correlation between sales and marketing campaigns.
---
SQL Query Documents:
---
- Query 1: Retrieving the total sales for each product category 

SELECT
     Product,
     sum(quantity*unitprice)as total sales
FROM
    DBO.lita capstone dataset
GROUP BY
      Product;


Query 2: Number of sales transaction for each product category 
SELECT 
     Region,count(*)as number of transaction 
FROM
    (DBO).LITA CAPSTONE DATASET)
GROUP BY
       REGION

Query 3: calculate the total sales per product 

SELECT 
      product,sum(cast(quantity as int)* cast(unitprice as DECIMAL(10,2)))AS total sales 

GROUP BY
       Product 
ORDER BY
        Total sales DESC;

---
Power BI Dashboard 
---
- page 1: Sales overview 
          sales trend over time
          sales by region
  
- page 2: Product performance 
         - top selling products 
         - product wise sales
         
- Page 3: Category Analysis 
        - category wise sales
        - category wise sales trend
---           
##  CONCLUSION
---
The analysis of sales data provided valuable insights into trends, product performance and regional breakdown. key findings highlights the importance of understanding sales dynamics over time, optimizing inventory and leveraging targeted marketing strategies. By recognizing seasonal trends and identifing high-performing products and customer segment, the company can make data-driven decisions to enhance sales performance. in conclusion, this project underscores the potential for growth through infermed decision-making. By strategically responding to identified trends and patterns, the company is well-positioned to boost sales, increase profitability, and achieve sustainable growth in the coming years.


  


