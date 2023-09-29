# EX 2 Data Manipulation Language (DML) Commands and built in functions in SQL
## AIM:
To create a manager database and execute DML queries using SQL.


## DML(Data Manipulation Language)
<div align="justify">
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.
</div>

## List of DML commands: 
<div align="justify">
INSERT: It is used to insert data into a table.<br>
UPDATE: It is used to update existing data within a table.<br>
DELETE: It is used to delete records from a database table.<br>
</div>

## Create the table as given below:
```sql
create table manager(enumber number(6),ename char(15),salary number(5),commission number(4),annualsalary number(7),Hiredate date,designation char(10),deptno number(2),reporting char(10));
```
## insert the following values into the table
```sql
insert into manager values(7369,'Dharsan',2500,500,30000,'30-June-81','clerk',10,'John');
insert into manager values(7839,'Subu',3000,400,36000,'1-Jul-82','manager',null,'James');
insert into manager values(7934,'Aadhi',3500,300,42000,'1-May-82','manager',30,NULL);
insert into manager values(7788,'Vikash',4000,0,48000,'12-Aug-82','clerk',50,'Bond');
```

### Q1) Update all the records of manager table by increasing 10% of their salary as bonus.

### QUERY:

![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/c8cde3d5-7d3c-4fd9-9d45-b3f4f22da4e8)

### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/01628305-9c11-49d0-bc8b-50aee128f170)

### Q2) Delete the records from manager table where the salary less than 2750.


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/c91f4e68-36dc-48f3-94ed-76903844bad7)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/34db2c9b-5117-444a-9aef-159d32a9338c)

### Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/7f83ed7d-d95d-4a75-aec4-4bf8004e7b49)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/590180fa-f98a-48d7-8d3c-b07364a2528b)

### Q5)	List the names of Clerks from emp table.


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/187e3be8-14ef-4a62-84cf-0e0dc88d6f0d)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/10f5e6ed-f57e-48e7-8c25-6f3dc4ea152e)


### Q6)	List the names of employee who are not Managers.


### QUERY:

![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/0662095e-606f-4551-9422-a1a63ee28e66)

### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/1eb9c261-840e-4ffb-8aef-f44fd62b7db9)


### Q7)	List the names of employees not eligible for commission.


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/0796637f-8a0b-4078-a536-7a31b72b23a7)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/4666635c-2bab-4cff-8e61-11a7d55f9237)


### Q8)	List employees whose name either start or end with ‘s’.


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/8a2eac3b-fc17-4100-bfab-83c3b0d19822)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/8772a9f2-d55f-4c31-9052-1c9e79206556)


### Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/da807830-6a9a-48dd-9222-7646d38279df)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/e9b17669-5354-48e8-998c-a77463c91cb4)


### Q10) List the Details of Employees who have joined before 30 Sept 81.


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/8a8a8966-07d8-4567-b1d3-12c1ecebc6e9)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/056a0dca-bb1c-4414-a0f5-5ef7775ded3d)


### Q11)	List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/9d7d9693-1a4a-4b4e-8524-db71b346f950)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/c7c0f23f-9952-475f-8675-1c0b85de8ac2)


### Q12) List the names of employees not belonging to dept no 30,40 & 10


### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/e1fc9daf-e9ab-4069-89ca-6536389a5acf)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/ce47a304-1847-4e92-a586-cdfc94ef1c3f)

### Q13) Find number of rows in the table EMP

### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/d957a206-b96d-41f4-a3dc-3d1d71108542)


### OUTPUT:

![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/0bfcc921-cac5-423b-87e6-37422ffbf04a)

### Q14) Find maximum, minimum and average salary in EMP table.

### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/bf03230b-7cf5-4b1c-bea1-8159251cd78e)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/d11809ee-3232-4c58-b88c-7cd9b725d48b)


### Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.

### QUERY:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/99468141-55a7-49db-bd2a-e6dc6db8d2f0)


### OUTPUT:
![image](https://github.com/Jeevithaelumalai/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118708245/1039c807-ae86-45a4-86d6-f72b6a52111f)
