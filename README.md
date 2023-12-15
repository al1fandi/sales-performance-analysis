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
![Correlation-Heatmap](https://github.com/al1fandi/sales-performance-analysis/blob/main/Correlation%20Heatmap.jpg?raw=true)
Based on these results, there are some columns that have a strong positive correlation:
	- discount_value and sales (0.78): Indicates a strong positive correlation. When discount_value increases, sales also tends to increase.
	- discount_value and revenue (0.75): Indicates a strong positive correlation. When discount_value increases, revenue also tends to increase.

- Question 1. Which product categories and product sub-categories are most ordered?
![Product-Categories-Most-Ordered](https://github.com/al1fandi/sales-performance-analysis/blob/main/Product%20Categories%20Most%20Ordered.png?raw=true)
'Office Supplies' is the product category with the highest order of 2911 times or about 60% of the total product categories ordered.
  
![Product-Sub-Categories-Most-Ordered](https://github.com/al1fandi/sales-performance-analysis/blob/main/Product%20Sub-Categories%20Most%20Ordered.png?raw=true)
'Paper' is the product sub-category with the highest order of 736 times or about 15% of the total product sub-categories ordered.

- Question 2. Which product categories and product sub-categories are most income? 
![Product-Categories-Most-Income](https://github.com/al1fandi/sales-performance-analysis/blob/main/Product%20Categories%20Most%20Income.png?raw=true)
'Office Supplies' is the product category with the highest revenue of over 2.4 billion, or approximately 38% of the total product category revenue. Apart from being highly sold, the 'Office Supplies' product category also generates high revenue.

![Product-Sub-Categories-Most-Income](https://github.com/al1fandi/sales-performance-analysis/blob/main/Product%20Sub-Categories%20Most%20Income.png?raw=true)
'Telephones and Communication' is the product sub-category with the highest revenue of 978 million, or about 15% of the total revenue of all product sub-categories. However, the 'Telephones and Communication' product sub-category is not the highest-order item. This can happen because the price of the 'Telephones and Communication' is quite large when compared to the 'Paper'.
 
- Question 3. How is the quarterly performace of dqlab sales?
![Quarterly-Revenue-Trend](https://github.com/al1fandi/sales-performance-analysis/blob/main/Quarterly%20Revenue%20Trend.png?raw=true)
Revenue tends to peak in the 2nd (April–June) or 3rd (July–September) quarter. The highest revenue occurred in the 2nd quarter of 2012, with 480 million, or approximately 28% of total revenue during 2012. The lowest revenue occurred in the first quarter of 2010.

- Question 4. How is the monthly performance of dqlab sales?
![Monthly-Revenue-Trend](https://github.com/al1fandi/sales-performance-analysis/blob/main/Monthly%20Revenue%20Trend.png?raw=true)
Sales in September 2010 generated the highest revenue of 210 million, an increase of about 65% from the previous month (August 2010). Revenues also peaked thereafter in April and September 2012, generating 199 million and 195 million, respectively.

- Question 5. How is the daily performance of dqlab sales?
![Daily-Revenue-Trend](https://github.com/al1fandi/sales-performance-analysis/blob/main/Daily%20Revenue%20Trend.png?raw=true)

Sales on Saturday generated the highest revenue of 993 million. In addition, revenue was also high on Monday, reaching 969 million. Revenue peaked on Monday at the beginning of the weekday (15.08%) and on Saturday at the beginning of the weekend (15.45%).

- Question 6. Which product sub-categories are frequently returned and cancelled by customers?
![Product-Sub-Categories-Most-Returned-and-Cancelled](https://github.com/al1fandi/sales-performance-analysis/blob/main/Product%20Sub-Categories%20Most%20Returned%20and%20Cancelled.png?raw=true)
'Paper' is the product sub-category with the highest number of canceled and returned orders, with 68 times, or about 13.73% of the total unsuccessful orders. Returned or canceled orders can be caused by several factors, such as shipping duration, shipping quality, and item quality.

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
