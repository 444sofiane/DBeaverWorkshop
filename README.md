# Workshop: Importing Data into SampleData Database using DBeaver

This workshop guides you through creating a database named "SampleData" and importing provided data using DBeaver, a universal database tool.

### Part 1: Setting Up the Database and Importing Data

1. **Create Database:**

   Open DBeaver and establish a connection to your preferred database server (e.g., MySQL, PostgreSQL).

   - Right-click on the server in the Databases navigator.
   - Select "Create Database" and name it "SampleData".

2. **Create Table and Import Data:**

   - Right-click on the "SampleData" database.
   - Select "SQL Editor" to open a new SQL script.

3. **Create Table Schema:**

   Use the following SQL command to create a table to store the provided data:

   ```sql
   CREATE TABLE Sales (
       OrderDate DATE,
       Region VARCHAR(20),
       Rep VARCHAR(20),
       Item VARCHAR(20),
       Units INT,
       Unit Cost DECIMAL(10, 2),
       Total DECIMAL(10, 2)
   );

4. **Import Data From Excel**
    Save the provided data in a CSV file format. In DBeaver:

    Right-click on the "Sales" table within the "SampleData" database.
    Choose "Table Data > Import Data from File."
    Select the CSV file containing the data and follow the wizard to map the columns and import the data into the "Sales" table.


### Part 2: Querying the Data

After importing the data, you can run SQL queries in DBeaver to analyze and manipulate it.
Here are a few sample SQL queries you can execute in DBeaver using the SQL Editor :

1. **Retrieve all Data from Sales**
    See the select query in SQL

2. **Filter to show only OrderDate Column** 

3. **Calculate total Units sold and total revenue**
    See the Sum query in SQL