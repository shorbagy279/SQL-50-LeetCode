

# SQL-50-LeetCode
Solutions for [SQL 50 study plan](https://leetcode.com/studyplan/top-sql-50/) on LeetCode


[1757. Recyclable and Low Fat Products](https://leetcode.com/problems/recyclable-and-low-fat-products/)
```sql
  select product_id 
  from Products 
  where low_fats='Y' and recyclable='Y'; 
  ```
  [584. Find Customer Referee](https://leetcode.com/problems/find-customer-referee/)
  ```sql
  select name
  from Customer
  where (referee_id is  null  or referee_id !=  2 );
  ```
  [584. Find Customer Referee](https://leetcode.com/problems/find-customer-referee/)
  ```sql
  select name, population,area
  from World
where population >=  25000000  or  area>=  3000000
  ```
  [1148. Article Views I](https://leetcode.com/problems/article-views-i/)
  ```sql
  select  distinct author_id as id
  from Views
where author_id = viewer_id
order by author_id asc
```

[1683. Invalid Tweets](https://leetcode.com/problems/invalid-tweets/)
```sql
select tweet_id
from Tweets
where  length(content)>15
```
[1378. Replace Employee ID With The Unique Identifier](https://leetcode.com/problems/replace-employee-id-with-the-unique-identifier/)
```sql
select u.unique_id ,e.name
from Employees e
left  join EmployeeUNI u
on e.id = u.id
```
[1068. Product Sales Analysis I](https://leetcode.com/problems/product-sales-analysis-i/)
```sql
select P.product_name,S.year,S.price
from Sales as S
join Product as P
on S.product_id=P.product_id
```

[1581. Customer Who Visited but Did Not Make Any Transactions](https://leetcode.com/problems/customer-who-visited-but-did-not-make-any-transactions/)

```sql
select customer_id, count(V.visit_id) as count_no_trans
from Visits as V
left  join Transactions T
on V.visit_id = T.visit_id
where transaction_id is  null
group  by customer_id
```
[197. Rising Temperature](https://leetcode.com/problems/rising-temperature/)
```sql
select w1.id as Id from Weather as w1
join Weather as w2
where     #DATEDIFF(year, '2017/08/25', '2011/08/25')
 DATEDIFF( w1.recordDate, w2.recordDate) =1 and w1.temperature > w2.temperature ;
```

