# Case Study #2 - Pizza Runner
<div>
<img src="https://user-images.githubusercontent.com/94500188/208318437-e0231633-0e57-4c4b-9495-8fe8152f9dd7.png" width="500"/>
</div>
Danny wants to use the data to expand his new Pizza Empire. 
There are a lot of questions, which are broken up by area of focus including: Pizza Metrics, Runner and Customer Experience, Ingredient Optimisation, Pricing and Ratings.

## Entity relationship diagram
![image](https://user-images.githubusercontent.com/94500188/208318488-64984105-8dea-4954-b3c3-fc5b87496efb.png)


## Case Study Questions
**A. Pizza Metrics**
1. How many pizzas were ordered?
2. How many unique customer orders were made?
3. How many successful orders were delivered by each runner?
4. How many of each type of pizza was delivered?
5. How many Vegetarian and Meatlovers were ordered by each customer?
6. What was the maximum number of pizzas delivered in a single order?
7. For each customer, how many delivered pizzas had at least 1 change and how many had no changes?
8. How many pizzas were delivered that had both exclusions and extras?
9. What was the total volume of pizzas ordered for each hour of the day?
10. What was the volume of orders for each day of the week?

**B. Runner and Customer Experience**
1. How many runners signed up for each 1 week period? (i.e. week starts 2020-01-01)
1. What was the average time in minutes it took for each runner to arrive at the Pizza Runner HQ to pickup the order? 
1. Is there any relationship between the number of pizzas and how long the order takes to prepare?
1. What was the average distance travelled for each customer?
1. What was the difference between the longest and shortest delivery times for all orders?
1. What was the average speed for each runner for each delivery and do you notice any trend for these values?
1. What is the successful delivery percentage for each runner?

**C. Ingredient Optimisation**
1. What are the standard ingredients for each pizza?
1. What was the most commonly added extra?
1. What was the most common exclusion?
1. Generate an order item for each record in the `customers_orders` table in the format of one of the following:
    - Meat Lovers
    - Meat Lovers - Exclude Beef
    - Meat Lovers - Extra Bacon
    - Meat Lovers - Exclude Cheese, Bacon - Extra Mushroom, Peppers
1. Generate an alphabetically ordered comma separated ingredient list for each pizza order from the `customer_orders` table and add a 2x in front of any relevant ingredients
    - For example: "Meat Lovers: 2xBacon, Beef, ... , Salami"
1. What is the total quantity of each ingredient used in all delivered pizzas sorted by most frequent first?

**D. Pricing and Ratings**
1. If a Meat Lovers pizza costs $12 and Vegetarian costs $10 and there were no charges for changes - how much money has Pizza Runner made so far if there are no delivery fees?
1. What if there was an additional $1 charge for any pizza extras?
    - Add cheese is $1 extra 
1. The Pizza Runner team now wants to add an additional ratings system that allows customers to rate their runner, how would you design an additional table for this new dataset - generate a schema for this new table and insert your own data for ratings for each successful customer order between 1 to 5.
1. Using your newly generated table - can you join all of the information together to form a table which has the following information for successful deliveries?
    - `customer_id`
    - `order_id`
    - `runner_id`
    - `rating`
    - `order_time`
    - `pickup_time`
    - Time between order and pickup
    - Delivery duration
    - Average speed
    - Total number of pizzas
1. If a Meat Lovers pizza was $12 and Vegetarian $10 fixed prices with no cost for extras and each runner is paid $0.30 per kilometre traveled - how much money does Pizza Runner have left over after these deliveries?
