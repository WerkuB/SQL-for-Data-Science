# SQL-for-Data-Science
SQL (Structured Query Language) is a programming language designed for managing data in a relational database. It's been around since the 1970s and is the most common method of accessing data in databases today. SQL has a variety of functions that allow its users to read, manipulate, and change data. Though SQL is commonly used in Data Science.<br>
SQL is great for performing the types of aggregations that we might normally do in an Excel pivot table—sums, counts, minimums and maximums, etc.—but over much larger datasets and on multiple tables at the same time.
## Basics of SELECT Statements
* The basics of SQL SELECT Statements<br>
* The keyword FROM Specifies from which table to get the data. The clause can include optional JOIN subclauses to specify the rules for 
  joining tables.<br>
* WHERE(Optional Clause): Specifies which rows to retrieve.<br>
## Count, Distinct and Limit
These keywords are used to perform various operations on data sets, such as counting, filtering, and limiting the number of rows returned by a query. 
* COUNT is a built-in database function that
retrieves the number of rows that match the query criteria.<br>
    Syntax:
      ``` SELECT COUNT(*) FROM table_name; ```
* DISTINCT is used to remove duplicate values from a result set.<br>
    Syntax:
      ``` SELECT DISTINCT columnname FROM table_name; ```
* LIMIT is used for restricting the number of rows retrieved from the database.<br>
    Syntax:
      ``` SELECT * FROM table_name LIMIT number; ```
## INSERT, UPDATE and DELETE  
The SQL INSERT, UPDATE, and DELETE commands enable SQL users to manipulate and modify data:<br>
* The INSERT statement introduces new rows into an existing table.<br>
    Syntax:
      ```
         INSERT INTO table_name
         (column1,column2,column3...)
         VALUES(value1,value2,value3...);
      ```
* The DELETE statement removes a row or combination of rows from a table.<br>
    Syntax:
      ``` DELETE FROM table_name
          WHERE [condition];
      ```
* The UPDATE statement enables users to update a row or group of rows in a table.<br>
    Syntax:
      ``` UPDATE table_name
          SET[[column1]=[VALUES]]
          WHERE [condition];
      ```
## CREATE, ALTER, TRUNCATE and DROP
Data Definition Language(DDL) is a subset of SQL and a part of DBMS(Database Management System). DDL consist of Commands to commands like CREATE, ALTER, TRUNCATE and DROP. These commands are used to create or modify the tables in SQL.<br>
* CREATE: This command is used to create a new table in the database. The user has to give information like table name, column names, and their datatypes.<br>
   Syntax:<br>
     ``` CREATE TABLE table_name```<br>
     ``` (```<br>
     ```   column_1 datatype,```<br>
     ```   column_2 datatype,```<br>
     ```   column_3 datatype,```<br>
     ```   .... ```<br>
     ``` );```<br>
* ALTER: This command is used to add, delete or change columns in the existing table. The user needs to know the existing table name and can do add, delete or modify tasks easily.<br>
   Syntax:<br>
     - Add new column to an existing table.<br>
     ``` ALTER TABLE table_name ADD column_name datatype;e```<br>
* TRUNCATE: This command is used to remove all rows from the table, but the structure of the table still exists.<br>
     Syntax: <br>
     ``` TRUNCATE TABLE table_name;```<br>
* DROP: This command is used to remove an existing table along with its structure from the Database.<br>
     Syntax: <br>
     ``` DROP TABLE table_name;```<br>
