<i>project by Bartosz Jaromin</i>
# ShopInventory

Shop Inventory SQL + Python project

This is repository for my personal project in which I created a mockup shop inventory and orders database and created a dashboard to analyze and showcase some important data.
Tools used for this project:
<ul>
  <li>SQL (MySQL)</li>
  <li>Python (sqlalchemy, pandas, numpy, matplotlib)</li>
  <li>Jupyter Lab</li>
  <li>QuickDBD </li>
  <li>SQL Server Management Studio</li>
  <li>Google Spreadsheets </li>
  
</ul>

# This project contains
### <b> 1. Designing and creating a database </b>
  I designed and created a relational database that would simulate one of a shop selling computer accesories. The database contains structure is showcased on the image below. I created a database in SQL Server Management Studio.

### <b> 2. Generating data </b>
  Most of the data in the database is generated using Mockaroo.com. Because of the database structure however the records in Orders table had to be generated based on OrderItems table. For the data to be coherent, I generated values for Orders table in Google Sheets, exported it in .csv file and then inserted the data into the database using SQL. The data contains information from 1 month of sales

### <b> 3. Creating the dashboard and accessing the DB </b>
  Using SQLAlchemy in Jupyter Lab I managed to connect to the created Database. I also made a simple function allowing to lookup the database tables and their content within the dashboard. 
  
### <b> 4. Analyzing Product Sales </b>
  This is the core of the whole project, focusing on retrieving data from the database using SQL queries and showcasing or visualizing it using Python. I split it into three sections:
<ol>
  <li>Product data</li>
    This section focuses on products, and showcases data about total revenue and best selling products. It contains graphs visualizing revenue generated by the top 5 products.
  <li>Orders data</li>
    This section contains statistics about orders such as amount of orders, average, median and mode of all orders and the most frequent buyers.
  <li>Restock data</li>
    This section contains information which products might need restocking based on the previous month of sales. If the amount of orders previous month was greater than products currently in stock, the product will be shown with a number to order.
</ol>
