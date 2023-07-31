# Offline Invoicing
 Desktop invoicing app built with nodejs and electronjs  
 
 **To use on Windows:**
 [Download](http://download.offlineinvoicing.com/OfflineInvoicing.msi) the MSI Installer

**To Customize/Create your own installer**

- Clone this project.
- Open terminal and navigate into the cloned folder.
- Run "npm install" to install dependencies.
- Run "npm run electron". 

To develop the Node.js server for the billing system with the specified functionalities, you can follow these steps:

1. Set up the Node.js project:
   - Create a new Node.js project using npm or yarn.
   - Install necessary dependencies, such as Express (for creating the server), body-parser (for parsing request bodies), and any other libraries you may need.

2. Define data structures:
   - Define data structures to represent products, services, users, and cart items. Each product and service should have attributes like name, price, and tax category.

3. Implement the APIs:
   - Create API endpoints to handle the specified functionalities for users.
   - Use appropriate HTTP methods (GET, POST, PUT, DELETE) and URL routes to handle different operations.
   - For example:
     - `POST /api/users` to create a new user account.
     - `GET /api/products` to fetch all products and their prices.
     - `POST /api/cart/add/:productId` to add a product to the cart.
     - `POST /api/cart/remove/:itemId` to remove an item from the cart.
     - `POST /api/cart/clear` to clear the entire cart.
     - `GET /api/cart/total` to view the total bill with taxes for the items in the cart.
     - `POST /api/cart/confirm` to confirm the order.

4. Implement tax calculation:
   - Create functions to calculate the tax based on the specified rules for products and services.
   - Apply the appropriate tax percentage or flat tax amount to each product/service individually during the total bill calculation.

5. Implement admin functionalities (optional):
   - If desired, create additional API endpoints for admin users to view all orders.

6. Write test cases:
   - Write test cases to simulate different scenarios to ensure the system works as expected.
   - Include test cases for creating an account, adding/removing items from the cart, calculating the total bill with taxes, and confirming the order.

7. Error handling and validation:
   - Implement proper error handling and validation for the API endpoints to handle various error scenarios gracefully.

8. Data storage (optional):
   - Decide how you want to store the data (products, services, users, cart) - it can be in-memory, using a database like MongoDB, or a combination of both.

9. Start the server:
   - Run the Node.js server and test the APIs using tools like Postman or curl to ensure they work correctly.

Remember to break down the implementation into smaller tasks and gradually build up the server. It's also a good practice to modularize the code and follow best practices for code organization and documentation. 



Submited by Abhaya Goel