# bamazon

This app is an Amazon-like storefront using MySql and Inquirer npm packages. The app takes in orders from customers and deplete stock from the store's inventory. 

In addition, the app is used to track product sales across your store's departments and then provide a summary of the highest-grossing departments in the store.


The app includes a products table which stores all the items in inventory by product name, price and stock quantity.  


 Running this application will first display all of the items available for sale. Include the ids, names, and prices of products for sale.

The app then prompts users with two messages.

   * The first asks them the ID of the product they would like to buy.
   * The second message asks how many units of the product they would like to buy.

  
  Screen shot = `bamazonCustomer.js`

Once the customer has placed the order, the application checks if the store has enough of the product to meet the customer's request.

   * If not, the app logs a phrase like `Insufficient quantity!`, and then prevent the order from going through.

   Screen shot = `InsufficentQuantity.png`

However, if the store _does_ have enough of the product, the customer's order is fulfilled and the order quantity is deducted from the stock inventory.
   * The SQL database is updated to reflect the remaining quantity.
   * Once the update goes through, customer will see the total cost of their purchase.



