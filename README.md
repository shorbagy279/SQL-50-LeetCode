
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
