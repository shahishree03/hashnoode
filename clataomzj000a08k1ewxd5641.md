---
title: "Structured Query Language"
datePublished: Wed Nov 23 2022 06:58:54 GMT+0000 (Coordinated Universal Time)
cuid: clataomzj000a08k1ewxd5641
slug: structured-query-language
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1669137278208/9sdZVLGm4.png

---

**What is SQL?**   
SQL stands for Structured Query Language , which lets you access and manipulate databases, also for stream processing in a relational data stream management system (RDSMS). It is particularly useful in handling structured data, i.e. data incorporating relations among entities and variables.
SQL became a standard of the American National Standards Institute (ANSI) in 1986, and of the International Organization for Standardization (ISO) in 1987.
Compared to more traditional read-write APIs like ISAM or VSAM, SQL has two key benefits. Firstly, it introduced the concept of accessing several records with a single command. Secondly, the requirement to define how to access a record, such as with or without an index, is also removed.

**What Can SQL do?**
1. Executes queries against a database.
2. It can retrieve data from a database.
3. Inserts records in a database.
4. Updates records in a database.
5. Deletes records from a database.
6. SQL can create new databases.
7. It can create new tables in a database.
8. Create stored procedures in a database.
9. Create views in a database.
10. SQL can set permissions on tables, procedures, and views.

**Using SQL in Your Web Site**  
To build a web site that shows data from a database, you will need:   
-> An RDBMS database program (i.e. MS Access, SQL Server, MySQL)   
-> To use a server-side scripting language, like PHP or ASP     
-> To use SQL to get the data you want   
-> To use HTML / CSS to style the page  

**SQL commands : **  

**1. SELECT ** 
Extract data from the database, The data returned is stord in a result table called the result set.

```
SELECT column1, column2, ...
FROM table_name;
```

Here, column1, column2, ... are the field names of the table you want to select data from. If you want to select all the fields available in the table, use the following syntax:

```
SELECT*FROM table_name;
```
The following SQL statement selects the "CustomerName" and "City" columns from the "Customers" table:       
Example: 
```
SELECT CustomerName, City FROM Customers;
```


**2. UPDATE**  
The update statement is used to modify and make changes to the records that are existing in a table.    
UPDATE Syntax    

```
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```
*Note* : Be careful when updating records in a table! Notice the WHERE clause in the UPDATE statement. The WHERE clause specifies which record(s) that should be updated. If you omit the WHERE clause, all records in the table will be updated!

The following SQL statement updates the first customer (CustomerID = 1) with a new contact person and a new city.

**Example**

```
UPDATE Customers
SET ContactName = 'Iliyan Momin', City= 'Mumbai'
WHERE CustomerID = 1;
```

**3. DELETE **    
The delete statement in SQL  
Existing records in a table can be deleted using the DELETE command. 

Delete Syntax
```
DELETE FROM table_name WHERE condition;
```
SQL DELETE Example:  
The following SQL statement deletes the customer "Iliyan Momin" from the "Customers" table:

**Example**
```
DELETE FROM Customers WHERE CustomerName='Iliyan Momin';
```

**4. INSERT INTO**   
The SQL INSERT INTO Statement
The INSERT INTO statement is used to insert new records in a table.

INSERT INTO Syntax
It is possible to write the INSERT INTO statement in two ways:

1. Specify both the column names and the values to be inserted:

```
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);
```

2. If you are adding values for all the columns of the table, you do not need to specify the column names in the SQL query. However, make sure the order of the values is in the same order as the columns in the table. Here, the INSERT INTO syntax would be as follows:

```
INSERT INTO table_name
VALUES (value1, value2, value3, ...);
```

INSERT INTO Example  
The following SQL statement inserts a new record in the "Customers" table:

**Example** 
```
INSERT INTO Customers (CustomerName, ContactName, Address, City, PostalCode, Country)
VALUES ('Iliyan', 'Iliyan momin', 'Jogeshwari', 'Mumbai', '400102', 'India');
```

**5. WHERE clause **

SQL WHERE Clause 
The SQL WHERE Clause : The WHERE clause is used to filter records.
It is used to extract only those records that fulfill a specified condition.

WHERE Syntax
```
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

**Note:** The WHERE clause is not only used in SELECT statements, it is also used in UPDATE, DELETE, etc.!

WHERE Clause Example
The following SQL statement selects all the customers from the country "India", in the "Customers" table:

**Example**
```
SELECT * FROM Customers
WHERE Country='India';
```
**6. NULL value **
What is a NULL Value?
A field with a NULL value is a field with no value.
If a field in a table is optional, it is possible to insert a new record or update a record without adding a value to this field. Then, the field will be saved with a NULL value.

**Note:** A NULL value is different from a zero value or a field that contains spaces. A field with a NULL value is one that has been left blank during record creation!

How to Test for NULL Values?
It is not possible to test for NULL values with comparison operators, such as =, <, or <>.

We will have to use the IS NULL and IS NOT NULL operators instead.

IS NULL Syntax: 

```
SELECT column_names
FROM table_name
WHERE column_name IS NULL;
```

IS NOT NULL Syntax:
```
SELECT column_names
FROM table_name
WHERE column_name IS NOT NULL;
```
The IS NULL operator is used to test for empty values (NULL values).
The following SQL lists all customers with a NULL value in the "Address" field:

**Example :**
```
SELECT CustomerName, ContactName, Address
FROM Customers
WHERE Address IS NULL;
```