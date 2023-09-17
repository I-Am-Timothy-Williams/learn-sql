# Sqlite-DBBrowser-DataAnalysis

![image](https://i.imgur.com/aP2Mw08.jpg)

## Data Used

**Data** - WSDA Music Database, Music, Sales, Customers, Employees, Etc

**Data Cleaning & Analysis** - Sqlite on DBBrowser

## PROBLEM

Money is missing!

1. Analyze WSDA data
2. Get a list of suspects
3. Narrow the list to prime suspects
4. Reveal who is responsible for the missing money!

## SOLUTION

Which tables could be potentially relevant to suspects for the crime?

1) Look at the Database Structure
	- I think it is probable that only employees have the potential to take money from WSDA
	- Tables that have employee ID are Customer(SupportRepId), Employee (EmployeeId)
	- Tables that link to money are Invoice and InvoiceLine

a) How many transactions took place between the years 2011 - 2012?
b) How much money did WSDA Music make during the same period?


2. More targeted questions that query the tables that I've identified
a) Get a list of customers who made purchases between 2011-2012
b) Get a list of customers, sales reps, and total transaction amounts for each customer between 2011-2012
c) How many transactions are above the average transaction amount during the same time?
d) What was the average transaction amount for each year that WSDA Music Co has been in business


3. Queries that Perform an In in-depth analysis with the aim of finding employees who may have been financially motivated to commit the crime

a) Get a list of employees who exceeded the average transaction amount from sales they generated during 2011-2012
b) Create a Commission payout column that displays each employee's commission based on 15% of the sales transaction amount
c) Which employee made the highest commission
d) List the customers that were served by the employee identified in the last question
e) Which customer made the highest purchase?
f) Look at the customer record.
