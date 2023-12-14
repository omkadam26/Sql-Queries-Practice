# Sql-Queries-Practice-of-W3-School


Following are some sql practice queries with questions


Questions


Select
1. Insert the missing statement to get all the columns from the Customers table.
-> select * FROM Customers;
2.Write a statement that will select the City column from the Customers table.
-> select city from Customers;
3.Select all the different values from the Country column in the Customers table.
-> select distinct Country FROM Customers;

Where
4. Select all records where the City column has the value "Berlin".
->SELECT * FROM Customers where city = 'Berlin';
5.Use the NOT keyword to select all records where City is NOT "Berlin".
-> SELECT * FROM Customers where not city = 'Berlin';
6.Select all records where the CustomerID column has the value 32.
->SELECT * FROM Customers where CustomerID = 32;
7.Select all records where the City column has the value 'Berlin' and the PostalCode column has the value '12209'.
->select * FROM Customers where City = 'Berlin' and postalcode  = '12209';
8.Select all records where the City column has the value 'Berlin' or 'London'.
-> select * FROM Customers where City = 'Berlin' or city = 'London';

Order By
9.Select all records from the Customers table, sort the result alphabetically by the column City.
-> SELECT * FROM Customers order by city ;
10.Select all records from the Customers table, sort the result reversed alphabetically by the column City.
-> SELECT * FROM Customers order by city desc ;
11.Select all records from the Customers table, sort the result alphabetically, first by the column Country, then, by the column City.
-> SELECT * FROM Customers order by Country, City;


Insert
12.Insert a new record in the Customers table.
-> INSERT INTO Customers (CustomerName, Address, City, PostalCode,Country)VALUES ('Hekkan Burger','Gateveien 15','Sandnes','4306','Norway');


Null
13. Select all records from the Customers where the PostalCode column is empty.
-> SELECT * FROM Customers WHERE PostalCode IS NULL;
14.Select all records from the Customers where the PostalCode column is NOT empty.
->SELECT * FROM Customers WHERE PostalCode IS NOT NULL;

Update
15.Update the City column of all records in the Customers table.
->UPDATE Customers SET City = 'Oslo';
16.Set the value of the City columns to 'Oslo', but only the ones where the Country column has the value "Norway".
->UPDATE Customers SET City = 'Oslo' WHERE Country = 'Norway';
17.Update the City value and the Country value.
-> UPDATE Customers SET City = 'Oslo',Country = 'Norway'WHERE CustomerID = 32;


Delete
18.Delete all the records from the Customers table where the Country value is 'Norway'.
-> DELETE FROM Customers WHERE Country = 'Norway';
19.Delete all the records from the Customers table.
->DELETE FROM Customers;


SQL FUnctions
20.Use the MIN function to select the record with the smallest value of the Price column.
->SELECT MIN(Price)FROM Products;
21.Use an SQL function to select the record with the highest value of the Price column.
->SELECT MAX(Price)FROM Products;
22.Use the correct function to return the number of records that have the Price value set to 18.
->SELECT COUNT(*)FROM Products WHERE Price = 18;
23.Use an SQL function to calculate the average price of all products.
->SELECT AVG(Price)FROM Products;
24.Use an SQL function to calculate the sum of all the Price column values in the Products table.
->SELECT Sum(Price)FROM Products;
and


SQL Like
25.
