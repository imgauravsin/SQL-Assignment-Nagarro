##### The exercise requires SQL Server AdventureWorks OLTP database which can be found at Codeplex. 
Download and attach a copy of the database to your server instance. 
Take some time to appreciate the entire schema of the database, and functions and stored procedures (refer AdventureWorks 2008 OLTP Schema.pdf). 

#### Exersice : 1
```
Using the AdventureWorks database, perform the following queries.
1.	Display the number of records in the [SalesPerson] table. (Schema(s) involved: Sales)
2.	Select both the FirstName and LastName of records from the Person table where the FirstName begins with the letter ‘B’. (Schema(s) involved: Person)
3.	Select a list of FirstName and LastName for employees where Title is one of Design Engineer, Tool Designer or Marketing Assistant. 
    (Schema(s) involved: HumanResources, Person)
4.	Display the Name and Color of the Product with the maximum weight. (Schema(s) involved: Production)
5.	Display Description and MaxQty fields from the SpecialOffer table. Some of the MaxQty values are NULL, in this case display the value 0.00 instead. 
    (Schema(s) involved: Sales)
6.	Display the overall Average of the [CurrencyRate].[AverageRate] values for the exchange rate ‘USD’ to ‘GBP’ for the year 2005 
    i.e. FromCurrencyCode = ‘USD’ and ToCurrencyCode = ‘GBP’. Note: The field [CurrencyRate].[AverageRate] is defined as 'Average exchange rate for the day.' 
    (Schema(s) involved: Sales)
7.	Display the FirstName and LastName of records from the Person table where FirstName contains the letters ‘ss’. 
    Display an additional column with sequential numbers for each row returned beginning at integer 1. (Schema(s) involved: Person)
8.	Sales people receive various commission rates that belong to 1 of 4 bands. (Schema(s) involved: Sales)
      CommissionPct	    Commission Band
      0.00	              Band 0
      Up To 1%	          Band 1
      Up To 1.5%	        Band 2
      Greater 1.5%	      Band 3

    Display the [SalesPersonID] with an additional column entitled ‘Commission Band’ indicating the appropriate band as above.
9.	Display the managerial hierarchy from Ruth Ellerbrock (person type – EM) up to CEO Ken Sanchez. 
    Hint: use [uspGetEmployeeManagers] (Schema(s) involved: [Person], [HumanResources]) 
10.	Display the ProductId of the product with the largest stock level. 
    Hint: Use the Scalar-valued function [dbo]. [UfnGetStock]. (Schema(s) involved: Production)
    ```
