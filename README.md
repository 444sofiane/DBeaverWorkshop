# Workshop: Importing Data into Sales Database using DBeaver

This workshop guides you through creating a database named "Sales" and importing provided data using DBeaver, a universal database tool.

### Part 0: Installing DBeaver

#### Windows:

1. **Download DBeaver:**

   - Go to the [DBeaver official website](https://dbeaver.io/) and navigate to the download section.
   - Select the appropriate version for Windows and download the installer.

2. **Install DBeaver:**

   - Locate the downloaded installer file.
   - Double-click the file to start the installation process.
   - Follow the on-screen instructions to complete the installation.

#### Linux:

1. **Using Package Manager:**

   - For Debian/Ubuntu-based systems:
     ```bash
     sudo apt-get update
     sudo apt-get install dbeaver-ce
     ```

   - For Red Hat-based systems (Fedora, CentOS):
     ```bash
     sudo dnf install dbeaver-ce
     ```

   - For Arch Linux:
     ```bash
     sudo pacman -S dbeaver
     ```

   - For other Linux distributions, you can find installation instructions on the DBeaver website.

2. **Alternative Installation Method:**

   Alternatively, you can download the DBeaver package from the official website:
   - Go to the [DBeaver official website](https://dbeaver.io/) and navigate to the download section for Linux.
   - Follow the provided installation instructions for your specific distribution.

Once you have installed DBeaver, you can proceed with the workshop to create the "Sales" database and import provided data as described in the subsequent sections.


### Part 1: Setting Up the Database and Importing Data

1. **Create Database:**

   Open DBeaver and establish a connection to your preferred database server (e.g., MySQL, PostgreSQL).

   - Right-click on the server in the Databases navigator.
   - Select "Create Database" and name it "Sales".

2. **Create Table and Import Data:**

   - Right-click on the "Sales" database.
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

    Right-click on the "Sales" table within the "Sales" database.
    Choose "Table Data > Import Data from File."
    Select the CSV file containing the data and follow the wizard to map the columns and import the data into the "Sales" table.


### Part 2: Querying the Data

After importing the data, you can run SQL queries in DBeaver to analyze and manipulate it.
Here are a few sample SQL queries you can execute in DBeaver using the SQL Editor :

1. **Retrieve all Data from Sales**

    See the SELECT query in SQL

2. **Filter to show only OrderDate Column** 

3. **Calculate total Units sold and total revenue**

    See the SUM query in SQL

4. **Order the result set based on the values in the Total column in descending order and show only the 10 first**

    See the DESC, ORDER BY and LIMIT query in SQL

5. **Show the East region sales where the Unit cost is higher than 10**

    See the WHERE, AND query in sql

6. **Update so the Unit cost in the central region will always be 5.99**

    See the UPDATE query in sql

7. **Delete the pencil item in the west region**

    See the DELETE query in sql