
Total amount of orders in each month of 2023.
Total amount of orders in 2023.
Total orders by each customer in 2023.
Top 3 customers by total order amount.
Best customer’s monthly orders.


































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
