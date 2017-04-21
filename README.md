# HW_Bamazon

In this activity, I created an Amazon-like storefront with MySQL. The app takes in orders from customers and depletes stock from the store's inventory.

## Requirements

1. Create a MySQL Database called `Bamazon`.

2. Create a Table inside of that database called `products`.

3. The products table should have each of the following columns:

   * item_id (unique id for each product)

   * product_name (Name of product)

   * department_name

   * price (cost to customer)

   * stock_quantity (how much of the product is available in stores)

4. Populate this database with around 10 different products.

5. Create a Node application called `bamazonCustomer.js`. Running this application will first display all of the items available for sale. Include the ids, names, and prices of products for sale.

6. The app should then prompt users with two messages.

   * The first should ask them the ID of the product they would like to buy.
   * The second message should ask how many units of the product they would like to buy.

7. Once the customer has placed the order, your application should check if your store has enough of the product to meet the customer's request.

   * If not, the app should log a phrase like `Insufficient quantity!`, and then prevent the order from going through.

8. However, if your store _does_ have enough of the product, you should fulfill the customer's order.
   * This means updating the SQL database to reflect the remaining quantity.
   * Once the update goes through, show the customer the total cost of their purchase.


## Concepts Implemented

- Working with MySQL database and Node packages
- Updating tables in MySQL based on user input


## Code Explanation

- If user choses to enter Bamazon they are prompted to select a product and quantity they wish to buy.
- If the product the user selected has sufficient inventory then the sale is completed and the user is given a total amount.
- If the product the user selected has insufficient inventory then the sale is cancelled and the user is prompted to revise their order or leave the store.
