**Product funnel analysis:**

Using a single SQL query - create a new output table which has the following details:

1. How many times was each product viewed?
2. How many times was each product added to cart?
3. How many times was each product added to a cart but not purchased (abandoned)?
4. How many times was each product purchased?


For this part of the project, we only need to use two of the tables available. Events and Page_Hierarchy  as they both contain all the values neccesary to perform our calculations.

![b1](https://github.com/Sebsram/Case-Study-Clique-Bait/assets/130475600/edd1ab61-3686-4c74-873f-b753984121df)

| product_id | product_name   | product_category | views | cart_adds | abandoned | purchases |
| ---------- | -------------- | ---------------- | ----- | --------- | --------- | --------- |
| 1          | Salmon         | Fish             | 1559  | 938       | 227       | 711       |
| 2          | Kingfish       | Fish             | 1559  | 920       | 213       | 707       |
| 3          | Tuna           | Fish             | 1515  | 931       | 234       | 697       |
| 4          | Russian Caviar | Luxury           | 1563  | 946       | 249       | 697       |
| 5          | Black Truffle  | Luxury           | 1469  | 924       | 217       | 707       |
| 6          | Abalone        | Shellfish        | 1525  | 932       | 233       | 699       |
| 7          | Lobster        | Shellfish        | 1547  | 968       | 214       | 754       |
| 8          | Crab           | Shellfish        | 1564  | 949       | 230       | 719       |
| 9          | Oyster         | Shellfish        | 1568  | 943       | 217       | 726       |

5. Additionally, create another table which further aggregates the data for the above points but this time for each product category instead of individual products.

![b2](https://github.com/Sebsram/Case-Study-Clique-Bait/assets/130475600/80bc5d85-be4a-4200-9013-f9672d478f1b)

| product_category | views | cart_adds | abandoned | purchases |
| ---------------- | ----- | --------- | --------- | --------- |
| Luxury           | 3032  | 1870      | 466       | 1404      |
| Shellfish        | 6204  | 3792      | 894       | 2898      |
| Fish             | 4633  | 2789      | 674       | 2115      |

Use your 2 new output tables - answer the following questions:

1. Which product had the most views, cart adds and purchases? 
A: **Oysters had the most views. Lobster had the most cart adds and purchases.**
2. Which product was most likely to be abandoned?
A: **Fish is the most likely to be abandoned**
3. Which product had the highest view to purchase percentage?

![b3](https://github.com/Sebsram/Case-Study-Clique-Bait/assets/130475600/e0dd00d5-2b4c-4a82-9f3d-707f28f89878

A: **Lobsters had the highest view to purchase percentage**

