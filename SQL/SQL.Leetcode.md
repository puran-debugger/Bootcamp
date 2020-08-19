
Leetcode MySQL Solution by Puran
175 Combine two table
Table: Person

+-------------+---------+
| Column Name | Type    |
+-------------+---------+
| PersonId    | int     |
| FirstName   | varchar |
| LastName    | varchar |
+-------------+---------+
PersonId is the primary key column for this table.
Table: Address

+-------------+---------+
| Column Name | Type    |
+-------------+---------+
| AddressId   | int     |
| PersonId    | int     |
| City        | varchar |
| State       | varchar |
+-------------+---------+
AddressId is the primary key column for this table.
 

Write a SQL query for a report that provides the following information for each person in the Person table, 
regardless if there is an address for each of those people:

FirstName, LastName, City, State
```mysql
select FirstName, LastName, City, State
from Person
left join Address
on Person.PersonId = Address.PersonId
```
176 Second high salary
Write a SQL query to get the second highest salary from the Employee table.

+----+--------+
| Id | Salary |
+----+--------+
| 1  | 100    |
| 2  | 200    |
| 3  | 300    |
+----+--------+
For example, given the above Employee table, the query should return 200 as the second highest salary. If there is no second highest salary, then the query should return null.

+---------------------+
| SecondHighestSalary |
+---------------------+
| 200                 |
+---------------------+
ifnull(expression,'bla'): if null return 'bla', otherwise expression
```mysql
select ifnull(
    (select distinct Salary
     from Employee
     order by Salary desc
     limit 1 offset 1
    ), null) as SecondHighestSalary


select max(Salary) as SecondHighestSalary
from Employee
where Salary < (select max(Salary) from Employee)

```
177 Nth highest salary
Write a SQL query to get the nth highest salary from the Employee table.

+----+--------+
| Id | Salary |
+----+--------+
| 1  | 100    |
| 2  | 200    |
| 3  | 300    |
+----+--------+
For example, given the above Employee table, the nth highest salary where n = 2 is 200. If there is no nth highest salary, then the query should return null.

+------------------------+
| getNthHighestSalary(2) |
+------------------------+
| 200                    |
+------------------------+
```mysql
create function getNthHighestSalary(N int) returns int
begin 
declare M int;
set M = N-1;
return (
    select dictinct Salary 
    from Employee
    order by Salary desc
    limit 1 offset 1
);
end
```
