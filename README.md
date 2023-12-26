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
## String Patterns, Sorting & Grouping 
* The like predicate is used in a WHERE clause to search for a pattern in a column.<br>
* The IN operator allows us to specify a set of values in a WHERE clause.<br>
* The BETWEEN operator in SQL is used to check if a value is within a specified range of values. <br>
## Sub-queries and Nested SELECTs
A sub-query or a nested SELECT is a SELECT statement that is embedded within another SQL statement, such as SELECT, INSERT, UPDATE, or DELETE. A sub-query can return a single value, a list of values, or a table of values that can be used by the outer query. Sub-queries are useful for filtering, aggregating, or comparing data from different tables or sources.
## Built-in functions
* __Aggregate Function__: An aggregate function in SQL is a function that performs a calculation on a set of values and returns a single value. Aggregate functions are often used with the GROUP BY clause to group the rows into categories and apply the function to each group. Some common aggregate functions are: SUM, COUNT, AVG, MAX and MIN.<br>
* __String functions__: String functions in SQL are functions that perform operations on strings, such as concatenating, replacing, reversing, formatting, or extracting substrings. Different SQL dialects may have different sets of string functions, but some common ones are: CONCAT, REPLACE, SUBSTRING, LOWER and TRIM.<br>
* __Date Functions__: Date functions are functions that manipulate or return information about dates and times, such as CURDATE, NOW, DATEDIFF, etc.<br>
## Accessing multiple Tables
There are several ways to access multiple tables in the same query. Namely, using Sub-queries, Implicit JOIN, and JOIN operators, such as INNER JOIN and OUTER JOIN.<br>
* Accessing Multiple Tables with Sub-Queries:<br>
  ```SELECT name, salary FROM employees WHERE department_id IN (SELECT department_id FROM departments WHERE location = 'New York');```<br>
* Accessing Multiple Tables with Implicit Joins:<br>
  ```SELECT table1.column1, table2.column2 FROM table1, table2 WHERE table1.column1 = table2.column1;```<br>
* Accessing Multiple Tables with Join Operators:<br>
  ```SELECT table1.column1, table2.column2 FROM table1 INNER JOIN table2 ON table1.column1 = table2.column1;```<br>
## Accessing Databases using Python
Accessing databases using Python is a common task for data analysis, web development, and automation. Python has several libraries that allow you to connect and interact with various types of databases, such as ibm_db API for IBM DB2, psycopg2 for ProstgreSQL, and dblib API for SQL Server.<br>
* DB-API is Python's standard API for accessing relational databases. It allows us to write a single program that works with multiple kinds of relational databases instead of writing a separate program for each one.<br>
* The DB_API connect constructor creates a connection to the database and returns a Connection Object, which is then used by the various connection methods.<br>
* The connection methods are: The cursor() method, which returns a new cursor object using the connection. The commit() method, which is used to commit any pending transaction to the database. The rollback() method, which causes the database to roll-back to the start of any pending transaction. The close() method, which is used to close a database connection.<br>


