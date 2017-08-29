# Bamazon
A Node.js &amp; MySQL digital storefront. This is a command line Node app that mimics an online retailer.

##Description

This application implements a simple command line based storefront using the npm inquirer package and the MySQL database backend together with the npm mysql package. The application presents two interfaces: customer and manager.

###MySQL Database Setup

In order to run this application, you should have the MySQL database already set up on your machine. If you don't, visit the MySQL installation page to install the version you need for your operating system. Once you have MySQL isntalled, you will be able to create the Bamazon database and the products table with the SQL code found in Bamazon.sql. Run this code inside your MySQL client like Sequel Pro to populate the database, then you will be ready to proceed with running the Bamazon customer and manager interfaces.

###Customer Interface

The customer interface allows the user to view the current inventory of store items: item IDs, descriptions, department in which the item is located and price. The user is then able to purchase one of the existing items by entering the item ID and the desired quantity. If the selected quantity is currently in stock, the user's order is fulfilled, displaying the total purchase price and updating the store database. If the desired quantity is not available, the user is prompted to modify their order.

To run the customer interface please follow the steps below:

		git clone git@github.com:angrbrd/bamazon.git
		cd bamazon
		npm install
		node bamazonCustomer.js

###Manager Interace

The manager interface presents a list of four options, as below.

		? Please select an option: (Use arrow keys)
		❯ View Products for Sale 
  		View Low Inventory 
  		Add to Inventory 
 		Add New Product

The **View Products for Sale** option allows the user to view the current inventory of store items: item IDs, descriptions, department in which the item is located, price, and the quantity available in stock.

The **View Low Inventory** option shows the user the items which currently have fewer than 100 units available.

The **Add to Inventory** option allows the user to select a given item ID and add additional inventory to the target item.

The **Add New Product** option allows the user to enter details about a new product which will be entered into the database upon completion of the form.

To run the manager interface please follow the steps below:

		git clone git@github.com:angrbrd/bamazon.git
		cd bamazon
		npm install
		node bamazonManager.js

###Image Demo
Example of bamazonCustomer.js
![alt text](images/Customer_example.png)
![alt text](images/manager_option_1_and_2.png)
![alt text](images/Cmanager_option_3_and_4.png)