# Restaurant-Orders
There were two tables for this dataset:

CREATE TABLE order_details (  
  order_details_id SMALLINT NOT NULL,  
  order_id SMALLINT NOT NULL,  
  order_date DATE,  
  order_time TIME,  
  item_id SMALLINT,  
  PRIMARY KEY (order_details_id));  

CREATE TABLE menu_items (  
  menu_item_id SMALLINT NOT NULL,  
  item_name VARCHAR(45),  
  category VARCHAR(45),  
  price DECIMAL(5,2),  
  PRIMARY KEY (menu_item_id));  

# The main questions are listed below which I answered using only SQL.

1. What were the least and most ordered items? What categories were they in?
2. What do the highest spend orders look like? Which items did they buy and how much did they spend?
3. Were there certain times that had more or less orders?
4. Which cuisines should we focus on developing more menu items for based on the data?

There were 137 null values which contained no relevant information so I deleted from the dataset.


# Most Ordered Items:
"Hamburger" in the "American" category with 622 orders.
"Edamame" in the "Asian" category with 620 orders.
"Korean Beef Bowl" in the "Asian" category with 588 orders.

# Least Ordered Items:
"Chicken Tacos" in the "Mexican" category with 123 orders.
"Potstickers" in the "Asian" category with 205 orders.
"Cheese Lasagna" in the "Italian" category with 207 orders.

# Highest Spend Orders:
The three highest spend orders were order_id 17 with 10 items totaling $154.15, order_id 9 with 9 items totaling $132.25, and order_id 2 with 5 items totaling $64.45.
Items Purchased in Highest Spend Orders:
For order_id 17, the customer bought 6 items from the "Italian" category, 3 items from the "Mexican" category, and 1 item from the "American" category.

# Time Analysis:
Certain dates had more or fewer orders.
The highest number of total orders was on 2023-02-01 with 186 orders.

# Weekly Orders Analysis:
The analysis of weekly orders shows the average, minimum, and maximum orders for each week.

Focus on Developing Menu Items:
Based on the highest spending customer (order_id 17), there is an opportunity to develop more menu items in the "Italian" category.

Category Revenue Analysis:
Analyzing revenue by category shows that "Italian" cuisine generated the highest revenue, followed by "Asian," "Mexican," and "American" cuisines.
This analysis provides insights into popular and less popular menu items, high spend orders, order trends over time, and opportunities for menu development in specific cuisines. The focus on revenue by category guides potential areas for further menu expansion.
