# Introduction to SQL Queries

## Create table emp
    CREATE TABLE `tutorials`.`emp` (
    `empno` INT NOT NULL,
    `empname` VARCHAR(45) NOT NULL,
    `job` VARCHAR(45) NOT NULL,
    `mgr` VARCHAR(45) NULL,
    `hiredate` DATE NOT NULL,
    `sal` INT NOT NULL,
    `comm` INT NULL,
    `deptno` INT NOT NULL,
    PRIMARY KEY (`empno`));

## ## Create table department emp
    INSERT INTO `tutorials`.`emp`
    (`empno`,
    `empname`,
    `job`,
    `mgr`,
    `hiredate`,
    `sal`,
    `comm`,
    `deptno`)
    VALUES
    (7369,"SMITH","CLERK",7902,"2005-12-17",800,null,20),
    (7499,"ALLEN","SALESMAN",7698,"2006-02-20",1600,300,30),
    (7521,"WARD","SALESMAN",7698,"2006-02-22",1250,500,30),
    (7566,"JONES","MANAGER",7839,"2006-04-02",2975,null,20),
    (7654,"MARTIN","SALESMAN",7698,"2006-09-28",1250,1400,30),
    (7698,"BLAKE","MANAGER",7839,"2006-05-01",2850,null,30),
    (7782,"CLARK","MANAGER",7839,"2006-06-09",2450,null,10),
    (7788,"SCOTT","ANALYST",7566,"2007-12-09",3000,null,20),
    (7839,"KING","PRESIDENT",null,"2006-11-17",5000,null,10),
    (7844,"TURNER","SALESMAN",7698,"2006-09-08",1500,0,30),
    (7876,"ADAMS","CLERK",7788,"2008-01-12",1100,null,20),
    (7900,"JAMES","CLERK",7698,"2006-12-03",950,null,30);

## Employee table will look like

 ![Emp_table](.\images\emp_table.png)

## Create table department
    CREATE TABLE `tutorials`.`dept` (
    `Deptno` INT NOT NULL,
    `deptname` VARCHAR(45) NOT NULL,
    `loc` VARCHAR(45) NOT NULL,
    PRIMARY KEY (`Deptno`));


## Insert data into department
    INSERT INTO `tutorials`.`dept`
    (`Deptno`,
    `deptname`,
    `loc`)
    VALUES
    (10, "ACCOUNTING", "NEW YORK"),
    (20, "RESEARCH", "DALLAS"),
    ( 30, "SALES", "CHICAGO"),
    ( 40 , "OPERATIONS" ,"BOSTON");

## Department table will look like

 ![Dept_table](.\images\dept_table.png)

