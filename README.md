# SQL-50-Leetcode-Answer
Answer to the 50 question study plan on leetcode for SQL

1757. Recyclable and Low Fat Products
```sql
Select product_id FROM Products where low_fats = "Y" and recyclable = "Y";
```
584. Find Customer Referee
```sql
select name from Customer where referee_id <> 2 or referee_id is null
```
595. Big Countries
```sql
select name, population, area from World where area >= 3000000 or population >= 25000000;
```
1683. Invalid Tweets
```sql
select tweet_id from Tweets where length(content) > 15
```
1378. Replace Employee ID With The Unique Identifier
```sql
select Eu.unique_id, E.name From Employees E left join EmployeeUNI Eu on Eu.id = E.id
```
1068. Product Sales Analysis I
```sql
select product_name, year, price from Sales left join Product on Sales.product_id = Product.product_id
```
1581. Customer Who Visited but Did Not Make Any Transactions
```sql
select customer_id, count(Visits.visit_id) as count_no_trans From Visits left join Transactions on Visits.visit_id = Transactions.visit_id where transaction_id is null group by customer_id
```

