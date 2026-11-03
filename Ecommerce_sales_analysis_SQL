create database ecommerce_sales;
use ecommerce_sales;

CREATE TABLE ecommerce_sales_data (
    Order_ID VARCHAR(50),
    Order_Date DATE,
    Season VARCHAR(20),
    Customer_ID VARCHAR(50),
    Customer_Gender VARCHAR(20),
    Customer_Segment VARCHAR(50),
    Region VARCHAR(50),
    Country VARCHAR(100),
    Category VARCHAR(100),
    Sub_Category VARCHAR(100),
    Product_Name VARCHAR(255),
    Unit_Price DECIMAL(10,2),
    Quantity INT,
    Discount DECIMAL(10,2),
    Revenue DECIMAL(12,2),
    Cost DECIMAL(12,2),
    Profit DECIMAL(12,2),
    Profit_Margin_Percent DECIMAL(10,2),
    Shipping_Cost DECIMAL(10,2),
    Shipping_Method VARCHAR(50),
    Shipping_Days INT,
    Payment_Method VARCHAR(50),
    Order_Status VARCHAR(50)
);
describe ecommerce_sales_data;

#Overall Business Performance (Key Metrics)
select
    sum(revenue) as total_revenue,
    sum(profit) as total_profit,
    count(distinct order_id) as total_orders,
    sum(quantity) as total_quantity,
    round(sum(revenue) / count(distinct order_id), 2) as average_order_value,
    round(sum(profit) / sum(revenue) * 100, 2) as profit_margin
from ecommerce_sales_data;


#Yearly Sales and Profit Analysis
select
    year(order_date) as year,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit
from ecommerce_sales_data
group by year(order_date)
order by year;


#Monthly Sales and Profit Trend
select
    year(order_date) as year,
    month(order_date) as month,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit
from ecommerce_sales_data
group by
    year(order_date),
    month(order_date)
order by
    year(order_date),
    month(order_date);


#Revenue and Profit by Category
select
    category,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit
from ecommerce_sales_data
group by category
order by total_revenue desc;


#Revenue and Profit by Region
select
    region,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit
from ecommerce_sales_data
group by region
order by total_revenue desc;


#Top 10 Products by Revenue
select
    product_name,
    sum(revenue) as total_revenue
from ecommerce_sales_data
group by product_name
order by total_revenue desc
limit 10;


#Top 10 Products by Profit
select
    product_name,
    sum(profit) as total_profit
from ecommerce_sales_data
group by product_name
order by total_profit desc
limit 10;


#Revenue and Profit by Customer Segment
select
    customer_segment,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit
from ecommerce_sales_data
group by customer_segment
order by total_revenue desc;


#Top 10 Customers by Revenue
select
    customer_id,
    sum(revenue) as total_revenue
from ecommerce_sales_data
group by customer_id
order by total_revenue desc
limit 10;


#Discount Impact on Revenue and Profit
select
    round(discount * 100, 2) as discount_percent,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit
from ecommerce_sales_data
group by discount
order by discount;


#Order Status Analysis
select
    order_status,
    count(distinct order_id) as total_orders,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit
from ecommerce_sales_data
group by order_status
order by total_orders desc;


#Shipping Method Analysis
select
    shipping_method,
    count(distinct order_id) as total_orders,
    round(avg(shipping_cost), 2) as avg_shipping_cost,
    round(avg(shipping_days), 2) as avg_shipping_days
from ecommerce_sales_data
group by shipping_method
order by total_orders desc;


#Payment Method Analysis
select
    payment_method,
    count(distinct order_id) as total_orders,
    sum(revenue) as total_revenue
from ecommerce_sales_data
group by payment_method
order by total_orders desc;


#Seasonal Sales and Profit Analysis
select
    season,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit,
    count(distinct order_id) as total_orders
from ecommerce_sales_data
group by season
order by total_revenue desc;


#Profit Margin by Category
select
    category,
    sum(revenue) as total_revenue,
    sum(profit) as total_profit,
    round(sum(profit) / sum(revenue) * 100, 2) as profit_margin
from ecommerce_sales_data
group by category
order by profit_margin desc;
