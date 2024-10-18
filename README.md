I have a few quesitons that I should be able to answer by making queries to my dataset:

Total amount of orders in each month of 2023.
Total amount of orders in 2023.
Total orders by each customer in 2023.
Top 3 customers by total order amount.
Best customer’s monthly orders.

Let's drop into small steps this project:

1. Establishing connection and creating database and tables

Tables:
customer_dim
date_dim
employee_dim
orders_fac
product_dim
ship_info
shipper_dim
supplier_dim

2. I have data in csv files. I need to clean this data. 
customer_dim:
date_dim: I needed to modify date column into
employee_dim
orders_fac
product_dim
ship_info
shipper_dim
supplier_dim

I need to use columns of this data in order to create a star schema in SQL

2. I need to insert into the start shema data from column that i chosed in the previous step
I need to do it using python script
For this I need
--> wirte Python script
--> clean data (keep in mind, that prices are in euros and in classicmodels in dollars 
+ we are interested only in month / year level information it will be better to have 
date_dim which has only month and year attributes)
--> transfer data ( Data value unification, De-Duplication (if any), Vertical slicing)

3. I need to write queries for funding answers to these questions:
- Total amount of orders in each month of 2023.
- Total amount of orders in 2023.
- Total orders by each customer in 2023.
- Top 3 customers by total order amount.
- Best customer’s monthly orders.

4. Development of plots
- The total amount of orders done in each month in 2023
- Top 3 customers and their amount of orders




























northwind-neo4j
===============

## Initial Load

Table => Graph mapping

1. `categories.csv`
  - product categories
  - => (:Category)
2. `customers.csv`
  - people who are customers
  - => (:Person:Customer)
3. `employees.csv`
  - people who are employees
  - => (:Person:Employee)
4. `order-details.csv`
  - extra detail about an order
  - => (:OrderDetail)
5. `orders.csv`
  - product orders
  - => (:Order)
6. `products.csv`
  - products sold by Northwind
  - => (:Product)
7. `territories.csv`
  - Sales territories
  - => (:Territory)
8. `employee-territories.csv`
  - join table of employees to their territories
  - => (:Employee)-[:SELLS_IN]->(:Territory)

## Data Clean-up
