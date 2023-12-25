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
## NSERT, UPDATE and DELETE  
The SQL INSERT, UPDATE, and DELETE commands enable SQL users to manipulate and modify data:<br>
* The INSERT statement introduces new rows into an existing table.<br>
    Syntax:
      ```
         INSERT INTO table_name<br>
         (column1,column2,column3...)<br>
         VALUES(value1,value2,value3...);<br>
      ```
* The DELETE statement removes a row or combination of rows from a table.<br>
    Syntax:
      ``` DELETE FROM table_name<br>
          WHERE [condition];
      ```
* The UPDATE statement enables users to update a row or group of rows in a table.<br>
    Syntax:
      ``` UPDATE table_name<br>
          SET[[column1]=[VALUES]]<br>
          WHERE [condition];<br>
      ```
