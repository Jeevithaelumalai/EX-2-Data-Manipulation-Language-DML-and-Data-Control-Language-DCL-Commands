# EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands
## AIM:
To create a mmannager database and execte DML queries using SQL.
## DML(Data Manipulation Language)
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.
## List of DML commands:
INSERT: It is used to insert data into a table.
UPDATE: It is used to update existing data within a table.
DELETE: It is used to delete records from a database table.
### OUTPUT;
## Create the table as given below:
create table manager(enumber numeric(6),ename char(15),salary numeric(5),commission numeric(4),annualsalary numeric(7),designation char(10),deptno numeric(2),reporting char(10));
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/7be97f9c-af8b-476c-a615-a7cee5c5bfb6)


## Insert the following values into the table:
insert into manager values(7369,'jeevitha',2500,500,30000,'clerk',10,'John');
insert into manager values(7839,'brin',3000,400,36000,'manager',null,'James');
insert into manager values(7934,'abrin',3500,300,42000,'manager',30,NULL);
insert into manager values(7788,'nirosha',4000,0,48000,'clerk',50,'Bond');

![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/a486fb65-598a-44bf-acdf-10fa89898a21)

## Q1) Update all the records of manager table by increasing 10% of their salary as bonus.
### QUERY:
update manager set salary=(salary*0.10)+salary;
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/aeda9662-21f5-48da-b70b-3bbe906920ac)
## Q2) Delete the records from manager table where the salary less than 2750.
### QUERY:
delete worker where salary<2750;
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/6ed2b979-beaa-4b5e-a23c-29bb18c2222e)
DELETE FROM manager where salary>2750;
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/b3c4719f-dc93-4827-aaab-28b6d757d2fb)
## Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary).
### QUERY:
SELECT ename as "Name",salary*12 as "annual salary" from manager;
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/a9ba4116-e865-4e73-bac3-fa07aa0588ef)
## Q5) List the names of Clerks from emp table.
### QUERY:
SELECT ename from manager where designation='clerk';
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/7187cf8a-986d-4dc6-9865-cdfe591f35bb)
## Q6) List the names of employee who are not Managers.
### QUERY:
SELECT ename from manager where designation!='manager';
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/18566964-20d3-4bd0-8042-58a2b4101150)
## Q7) List the names of employees not eligible for commission.
### QUERY:
SELECT ename from manager where commission=0;
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/ba58a09c-98ca-47cf-8cf4-61fbb83ebcf8)

## Q8) List employees whose name either start or end with ‘s’.
### QUERY:
select ename from manager where ename like 's%' or ename like '%s';
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/e05ec1cb-ec93-4885-8b6e-a31ebcf583b7)

# RESULT:
Thus the all the queries got the output and statifies the given question.
