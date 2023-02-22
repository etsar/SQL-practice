# Case Study #7 - Balanced Tree Clothing Co.
<div>
<img src="https://user-images.githubusercontent.com/94500188/220495445-b9430a8f-6b66-47af-9e7f-c8283c03805b.png" width="500"/>
</div>
Balanced Tree Clothing Company prides itself on providing an optimised range of clothing and lifestyle wear for the modern adventurer! 
<br>Danny has asked you to assist the merchandising team analyze their sales performance and generate a basic financial report to share with the wider business.

## Case Study Questions
<br>**1. High Level Sales Analysis**
1. What was the total quantity sold for all products?
1. What is the total generated revenue for all products before discounts?
1. What was the total discount amount for all products?

**2. Transaction Analysis**
1. How many unique transactions were there?
1. What is the average unique products purchased in each transaction?
1. What are the 25th, 50th and 75th percentile values for the revenue per transaction?
1. What is the average discount value per transaction?
1. What is the percentage split of all transactions for members vs non-members?
1. What is the average revenue for member transactions and non-member transactions?

**3. Product Analysis**
1. What are the top 3 products by total revenue before discount?
1. What is the total quantity, revenue and discount for each segment?
1. What is the top selling product for each segment?
1. What is the total quantity, revenue and discount for each category?
1. What is the top selling product for each category?
1. What is the percentage split of revenue by product for each segment?
1. What is the percentage split of revenue by segment for each category?
1. What is the percentage split of total revenue by category?
1. What is the total transaction “penetration” for each product? 
(hint: penetration = number of transactions where at least 1 quantity of a product was purchased divided by total number of transactions)
1. What is the most common combination of at least 1 quantity of any 3 products in a 1 single transaction?

**4. Reporting Challenge**
<br>Write a single SQL script that combines all of the previous questions into a scheduled report that the Balanced Tree team 
can run at the beginning of each month to calculate the previous month’s values.

Imagine that the Chief Financial Officer (which is also Danny) has asked for all of these questions at the end of every month.

He first wants you to generate the data for January only - but then he also wants you to demonstrate that you can easily run 
the same analysis for February without many changes (if at all).

Feel free to split up your final outputs into as many tables as you need - 
but be sure to explicitly reference which table outputs relate to which question for full marks :)

**5. Bonus Challenge**
<br>Use a single SQL query to transform the `product_hierarchy` and `product_prices` datasets to the `product_details` table.

Hint: you may want to consider using a recursive CTE to solve this problem!
