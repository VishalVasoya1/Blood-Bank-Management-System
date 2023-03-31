# Blood-Bank-Management-System
PostgreSQL, RDBMS, DBMS, SQL, Normalization

Title: Blood Bank Management System with PostgreSQL

<h3>Problem Statement:</h3>
Blood Bank Management Systems are important for efficient and effective management of blood donation and transfusion. However, many blood banks still rely on manual methods for tracking blood donations and inventory, which can be inefficient and error-prone. This project aims to solve this problem by using PostgreSQL to create a database for tracking blood donations, inventory, and other important information related to blood bank management, including managing blood camps.

<h3>Solution:</h3> 
We used PostgreSQL to create a database for a Blood Bank Management System that tracks blood donations, inventory, and other related information, including managing blood camps. We followed the principles of RDBMS and normalized the tables to minimize data redundancy and ensure data integrity. We created the following tables:

<h3>Important tables</h3>
</t><b>Donor:</b> stores information about blood donors, including donor ID, name, age, blood group, contact information, and last donation date.<br>
* Donation: stores information about blood donations, including donation ID, donor ID, donation date, blood type, and quantity.
* Inventory: stores information about the inventory of blood products, including inventory ID, blood type, quantity, and expiration date.
* Hospital: stores information about hospitals that receive blood products from the blood bank, including hospital ID, name, location, and contact information.
* Request: stores information about requests for blood products from hospitals, including request ID, hospital ID, blood type, quantity, and request date.
* Camp: stores information about blood donation camps, including camp ID, location, date, and contact information.
* We also created relations between these tables to ensure data consistency and to make querying the data easier. For example, the Donation table has a foreign key relationship with the Donor table, the Request table has a foreign key relationship with both the Hospital and Inventory tables, and the Donation table has a foreign key relationship with the Camp table.

<h3>We wrote a variety of analysis queries that can provide useful information for managing a blood bank and blood camps, such as:</h3>

* List of all donors who have donated in the last 6 months.
* Inventory status report, showing the quantity and expiration date of each blood type.
* List of all hospitals and their requests for blood products in the last week.
* Donor report, showing the total number of donations for each donor and the last donation date.
* Hospital report, showing the total quantity of blood products received by each hospital.
* List of all blood donation camps and their details.
* Report of all donations made at a specific blood donation camp.

<h3>We also wrote several required queries for managing a blood bank and blood camps, such as:</h3>

* Add a new donor to the Donor table.
* Add a new donation to the Donation table and update the Inventory table.
* Update the inventory quantity for a specific blood type.
* Delete a donor from the Donor table and update the Donation and Inventory tables accordingly.
* Mark a request as fulfilled and update the Inventory table.
* Add a new blood donation camp to the Camp table.
* Add a new donation made at a specific blood donation camp to the Donation table and update the Inventory table.

<h3>Conclusion:</h3>
In conclusion, this project provides an efficient and effective way to manage blood donations and inventory using PostgreSQL, including managing blood camps. By normalizing the tables and following the principles of RDBMS, we ensure data integrity and make querying the data easier. The analysis queries and required queries provide useful information for managing a blood bank and blood camps and performing necessary operations.
