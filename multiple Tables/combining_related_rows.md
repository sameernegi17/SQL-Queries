# Combining Related Rows

## Problem

You want to return rows from multiple tables by joining on a known common column or joining on columns that share common values. For example, you want to display the names of all employees in department 10 along with the location of each
employee’s department, but that data is stored in two separate tables.

ENAME| LOC
-----| ---
CLARK|NEW YORK
KING| NEW YORK


## Solution

    select  e.empname, d.loc from emp e, dept d 
    where e.deptno = d.deptno 
    and  e.deptno = 10

![join](./images/join.png)