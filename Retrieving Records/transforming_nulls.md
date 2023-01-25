# Transforming Nulls into Real Values

##  Problem

You have rows that contain nulls and would like to return non-null values in place of
those nulls.

## Solution

    select coalesce(comm,0) as commission from emp


![coalese](./images/coalese.png) 
