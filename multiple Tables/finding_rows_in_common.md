#  Finding Rows in Common Between Two Tables

## Problem

You want to find common rows between two tables, but there are multiple columns on which you can join. For example, consider the following view V created from the
EMP table for teaching purposes:

    create view V
    as
    select ename,job,sal
    from emp
    where job = 'CLERK'
    select * from V

ENAME | JOB | SAL
----- | ----| ----
SMITH|CLERK|800
ADAMS|CLERK|1100
JAMES|CLERK|950

Only clerks are returned from view V. However, the view does not show all possible
EMP columns. You want to return the EMPNO, ENAME, JOB, SAL, and DEPTNO of
all employees in EMP that match the rows from view V. You want the result set to be
the following:

EMPNO | ENAME | JOB | SAL | DEPTNO
----- |-------| --- | --- | -----
 7369|SMITH|CLERK|800|20
|7876|ADAMS|CLERK|1100|20
|7900|JAMES|CLERK|950|30

## Solution 

    select e.empno, e.empname, e.job,e.sal,e.deptno
    from emp e, V
    where e.empname = V.empname
    and e.job = V.job
    and e.sal = V.sal;

![common_rows](./images/common_rows.png)