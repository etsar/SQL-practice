# Case Study #6 - Clique Bait
<div>
<img src="https://user-images.githubusercontent.com/94500188/218828883-b7e3ab0c-0cd7-4abe-ac20-87cb4b7d50e6.png" width="500"/>
</div>
In this case study - you are required to support Danny’s vision and analyse his dataset and come up with creative solutions 
to calculate funnel fallout rates for the Clique Bait online store.

## Case Study Questions
<br>**1. Enterprise Relationship Diagram**
<br>Using the following [DDL schema details](https://github.com/etsar/SQL-practice/blob/main/SQL_case_study_6%20-%20Clique%20Bait/SQL_case_study_6_DBschema.ipynb) to create an ERD for all the Clique Bait datasets.

**2. Digital Analysis**
<br>**Using the available datasets - answer the following questions using a single query for each one:**
   1. How many users are there?
   1. How many cookies does each user have on average?
   1. What is the unique number of visits by all users per month?
   1. What is the number of events for each event type?
   1. What is the percentage of visits which have a purchase event?
   1. What is the percentage of visits which view the checkout page but do not have a purchase event?
   1. What are the top 3 pages by number of views?
   1. What is the number of views and cart adds for each product category?
   1. What are the top 3 products by purchases?

**3. Product Funnel Analysis**
<br>**A: Using a single SQL query - create a new output table which has the following details:**
   1. How many times was each product viewed?
   2. How many times was each product added to cart?
   3. How many times was each product added to a cart but not purchased (abandoned)?
   4. How many times was each product purchased?

**B: Additionally, create another table which further aggregates the data for the above points but this time for each product category instead of individual products.
<br>Use your 2 new output tables - answer the following questions:**
   1. Which product had the most views, cart adds and purchases?
   2. Which product was most likely to be abandoned?
   3. Which product had the highest view to purchase percentage?
   4. What is the average conversion rate from view to cart add?
   5. What is the average conversion rate from cart add to purchase?

**4. Campaigns Analysis**
<br>**Generate a table that has 1 single row for every unique `visit_id` record and has the following columns:**
- `user_id`
- `visit_id`
- `visit_start_time`: the earliest `event_time` for each visit
- `page_views`: count of page views for each visit
- `cart_adds`: count of product cart add events for each visit
- `purchase`: 1/0 flag if a purchase event exists for each visit
- `campaign_name`: map the visit to a campaign if the `visit_start_time` falls between the `start_date` and `end_date`
- `impression`: count of ad impressions for each visit
- `click`: count of ad clicks for each visit
- (Optional column) `cart_products`: a comma separated text value with products added to the cart sorted by the order they were added to the cart (hint: use the `sequence_number`)
