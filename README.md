# Case Study: Clique Bait

![icon](https://user-images.githubusercontent.com/130475600/235171527-8bd1a4f9-2295-4be5-9c9c-b9d7ecd8f7cb.PNG)

# Problem Statement
Clique Bait is not like your regular online seafood store - the founder and CEO Danny, was also a part of a digital data analytics team and wanted to expand his knowledge into the seafood industry!

In this case study - you are required to support Danny’s vision and analyse his dataset and come up with creative solutions to calculate funnel fallout rates for the Clique Bait online store.

# Available Data
**Users:**

Customers who visit the Clique Bait website are tagged via their cookie_id.

![Users](https://user-images.githubusercontent.com/130475600/235172507-9296fb6b-f043-43c5-a64a-89fe91af6ceb.PNG)

**Events:**

Customer visits are logged in this events table at a cookie_id level and the event_type and page_id values can be used to join onto relevant satellite tables to obtain further information about each event.

The sequence_number is used to order the events within each visit.

![Events](https://user-images.githubusercontent.com/130475600/235172920-5931f89c-350b-42fd-8b5a-a3cde0d10a74.PNG)

**Event Identifier:**

The event_identifier table shows the types of events which are captured by Clique Bait’s digital data systems.

![ei](https://user-images.githubusercontent.com/130475600/235173422-76e4eadb-a5d9-4c5b-8c1a-cfdc1371d61a.PNG)

**Campaign Identifier:**

This table shows information for the 3 campaigns that Clique Bait has ran on their website so far in 2020.

![ci](https://user-images.githubusercontent.com/130475600/235173622-cd9543d3-1982-4c97-8807-ca59813a6b0c.PNG)

**Page Hierarchy:**

This table lists all of the pages on the Clique Bait website which are tagged and have data passing through from user interaction events.

![page](https://user-images.githubusercontent.com/130475600/235173719-3455c94a-d6d9-4fd6-8268-bc0a850aabb7.PNG)

# Questions

**Digital Analysis:**

1. How many users are there?
2. How many cookies does each user have on average?
3. What is the unique number of visits by all users per month?
4. What is the number of events for each event type?
5. What is the percentage of visits which have a purchase event?
6. What is the percentage of visits which view the checkout page but do not have a purchase event?
7. What are the top 3 pages by number of views?
8. What is the number of views and cart adds for each product category?

**Product funnel analysis:**

Using a single SQL query - create a new output table which has the following details:

- How many times was each product viewed?
- How many times was each product added to cart?
- How many times was each product added to a cart but not purchased (abandoned)?
- How many times was each product purchased?
- Additionally, create another table which further aggregates the data for the above points but this time for each product category instead of individual products.

Use your 2 new output tables - answer the following questions:

1. Which product had the most views, cart adds and purchases?
2. Which product was most likely to be abandoned?
3. Which product had the highest view to purchase percentage?
4. What is the average conversion rate from view to cart add?
5. What is the average conversion rate from cart add to purchase?
6. What are the top 3 products by purchases?
