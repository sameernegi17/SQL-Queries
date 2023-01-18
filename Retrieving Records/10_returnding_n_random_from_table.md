# Returning n Random Records from a Table

# Problem

You want to return a specific number of random records from a table. You want to
modify the following statement such that successive executions will produce a different set of five rows:

    select ename, job
    from emp

## Solution

    select empname, job
    from emp order by rand() limit 5

![order_by_rand](./images/order_by_rand.png)