# Finding Rows That Satisfy Multiple Conditions

##  Problem

You want to return rows that satisfy multiple conditions.

## Solution

    select * from  emp  where deptno = 10 and sal > 3000;

![multiple_conditons_1](./images/multiple_conditons_1.png)

    select * from  emp  where deptno = 10 or sal > 3000;

![multiple_conditons_2](./images/multiple_conditons_2.png)