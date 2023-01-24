# Searching for Patterns

##  Problem

You want to return rows that match a particular substring or pattern. Consider the
following query and result set:
select ename, job
from emp
where deptno in (10,20)

| ENAME | JOB |
|------- | ---|
|SMITH| CLERK |
|JONES| MANAGER |
|CLARK| MANAGER|
|SCOTT| ANALYST|
|KING|PRESIDENT|
|ADAMS|CLERK |
|FORD| ANALYST|


Of the employees in departments 10 and 20, you want to return only those that have
either an “I” somewhere in their name or a job title ending with “ER”:
ENAME


| ENAME | JOB |
|------- | ---|
|SMITH| CLERK |
|JONES| MANAGER |
|CLARK| MANAGER|
|KING|PRESIDENT|



## Solution


