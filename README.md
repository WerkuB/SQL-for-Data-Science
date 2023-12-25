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
* LIMIT is used for restricting the number of rows retrieved from the database.
    Syntax:
      ``` SELECT * FROM table_name LIMIT number; ```
