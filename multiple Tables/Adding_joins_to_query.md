# Adding Joins to a Query Without Interfering with Other Joins

## Problem

you want to return all employees, the location of the department in which they work, and the date they received a bonus. For this problem, the EMP_BONUS table contains the following data:

    select * from emp_bonus

EMPNO|RECEIVED|TYPE
-----|--------|----
7369|14-MAR-2005|1
7900|14-MAR-2005|2
7788|14-MAR-2005|3


## Result :

ENAME|LOC|RECEIVED
-----|---|-----------
ALLEN|CHICAGO
WARD|CHICAGO
MARTIN|CHICAGO
JAMES|CHICAGO|14-MAR-2005
TURNER|CHICAGO
BLAKE|CHICAGO
SMITH|DALLAS|14-MAR-2005
FORD|DALLAS
ADAMS|DALLAS
JONES|DALLAS
SCOTT|DALLAS|14-MAR-2005
CLARK| NEW|YORK
KING|NEW YORK