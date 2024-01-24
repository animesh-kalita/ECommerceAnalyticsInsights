# SQL Problem Statement: E-Commerce Analytics

## Database Schema:

Consider an e-commerce platform with the following tables:

1. **Products:**
   - Columns: `product_id` (integer, primary key), `product_name` (varchar), `price` (decimal), `category_id` (integer, foreign key referencing Categories).

2. **Categories:**
   - Columns: `category_id` (integer, primary key), `category_name` (varchar), `parent_category_id` (integer, references Categories).

3. **Orders:**
   - Columns: `order_id` (integer, primary key), `customer_id` (integer), `order_date` (date).

4. **OrderItems:**
   - Columns: `order_item_id` (integer, primary key), `order_id` (integer, foreign key referencing Orders), `product_id` (integer, foreign key referencing Products), `quantity` (integer), `total_price` (decimal).

## Tasks:

1. **Revenue Analysis:**
   - Retrieve the total revenue generated for each category in the last quarter (3 months) considering the order date.

2. **Category Hierarchy:**
   - Write a query to display the category hierarchy for a given product. The result should show the full path of the category, starting from the given product's category up to the root category.

3. **Customer Loyalty:**
   - Identify the top 5 customers who have made the most purchases (highest number of orders) in the last six months. Include the customer name and the total number of orders.

4. **Stock Analysis:**
   - List all products that have never been ordered. Consider only products that are currently in stock (have a positive quantity available).

5. **Monthly Growth:**
   - Calculate the month-over-month growth rate in revenue for each category over the last 12 months. Display the results with the category name and the corresponding growth rate.

## Guidelines:

- Ensure your SQL queries are efficient.
- Consider the appropriate indexes for performance.
- Feel free to make reasonable assumptions or constraints if needed.

**Good luck!**

