
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
