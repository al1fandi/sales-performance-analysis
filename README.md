# Sales-Performance-Analysis

## Objective:
- Understand business performance by tracking historical sales data to gain valuable insights.
- Get business insight about Which product categories and product sub-categories are most ordered.
- Get business insight about which product categories and product sub-categories are most income.
- Get business insight about how is the quarterly performace of dqlab sales.
- Get business insight about how is the monthly performance of dqlab sales.
- Get business insight about how is the daily performance of dqlab sales.
- Get business insight about which product sub-categories are frequently returned and cancelled by customers.

## Business Understanding
- Retail is selling something (either consumer goods or consumer services) to customers and, as a result, earning a profit.
- This project has some business question using the data:
	- Which product categories and product sub-categories are most ordered?
	- Which product categories and product sub-categories are most income?
	- How is the quarterly performace of dqlab sales?
	- How is the monthly performance of dqlab sales?
	- How is the daily performance of dqlab sales?
	- Which product sub-categories are frequently returned and cancelled by customers?

## Data Understanding
- A historical retail sales data from 2009 to 2012.
- Data contain 3 product category which are office supplies, technology, and furniture. Each category has several sub categories.
- The raw dataset has 5499 rows and 1 columns.
- Attribute Information:
- **order_id**: unique order number.
- **order_status**: status of the order, whether is finished or returned.
- **customer**: customer name.
- **order_date**: date of the order.
- **order_quantity**: the quantity on a particular order.
- **sales**: sales generated on a particular order, the value is in IDR(Indonesia Rupiah) currency.
- **discount**: a discount percentage.
- **discount_value**: a sales multiply by discount, the value is in IDR(Indonesia Rupiah) currency.
- **product_category**: a category of the product.
- **product_sub_category**: a subcategory from product category.
- Data source: Sales Performance Report DQLab Store https://www.kaggle.com/datasets/dhawyfarrasputra/sales-performance-report-dqlab-store

## Data Cleaning
After importing the data, I needed to clean it up to make the data analysis process easier. I made changes and created new columns, as follows:
- Split column.
- Remove error column name.
- Remove error value in row.
- Rename column.
- Change datatype.
- Made a new column for revenue.
- Made a new column for quarter, year, month, week_day, and hour.
- Remove outliers.

## Exploration
- Initial Exploration
[GAMBAR]
[INTERPRETASI]
- Question 1. Which product categories and product sub-categories are most ordered?
[GAMBAR]
[INTERPRETASI]
[GAMBAR]
[INTERPRETASI]  
- Question 2. Which product categories and product sub-categories are most income? 
[GAMBAR]
[INTERPRETASI]
[GAMBAR]
[INTERPRETASI] 
- Question 3. How is the quarterly performace of dqlab sales?
[GAMBAR]
[INTERPRETASI]
- Question 4. How is the monthly performance of dqlab sales?
[GAMBAR]
[INTERPRETASI]
- Question 5. How is the daily performance of dqlab sales?
[GAMBAR]
[INTERPRETASI]
- Question 6. Which product sub-categories are frequently returned and cancelled by customers?
[GAMBAR]
[INTERPRETASI]

## Conclusion
Based on the exploration and analysis of DQLab Store's sales performance, we can conclude several things, which are:
- The most orders are dominated by the 'Office Supplies' category (60%) and the 'Paper' sub-category (15%).
- The highest revenue was dominated by the 'Office Supplies' category (38%) and the 'Telephones and Communication' sub-category (15%).
- The highest revenue occurred in Q2-2012 (28%; ~over 2012).
- The highest revenue occurred in September 2010 (~65% increase).
- Revenue peaked on Mondays (15.08%) and Saturdays (15.45%).
- The product with the highest number of cancellations and returns was the 'Paper' sub-category (13.73%).

## Recommendation
- Increase the stock of the most ordered products to handle the high demand from customers.
- Increase product stock in Q2 (April–June) and Q3 (July–September) to handle the high demand in those time periods.
- Offer special promotions for bundled products in Q1 (January, February, and March) of each year. The target of product bundling is the sub-category that has the lowest sales value. This special offer is expected to increase the number of sales of products that are not selling well and boost revenue in Q1.
- Provide special coupons for transactions on weekends to attract customers, thus increasing orders and revenue.
- Provide free delivery service on weekdays to facilitate transactions for customers who are busy working, thereby increasing the number of orders and revenue.
