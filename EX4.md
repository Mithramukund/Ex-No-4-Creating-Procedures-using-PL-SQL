# Ex. No: 4 Creating Procedures using PL/SQL
## DATE:25/09/23
### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```
CREATE TABLE employeee(empid NUMBER,empname VARCHAR(10),dept VARCHAR(10),salary NUMBER);
 CREATE OR REPLACE PROCEDURE insert_employeee_data AS
  2  BEGIN
  3  INSERT INTO employeee(empid,empname,dept,salary)
  4  VALUES(1,'john','HR',50000);
  5  INSERT INTO employeee(empid,empname,dept,salary)
  6  VALUES(2,'joe','IT',60000);
  7  INSERT INTO employeee(empid,empname,dept,salary)
  8  VALUES(3,'bob','Finance',55000);
  9  COMMIT;
 10  END;
 11  /
BEGIN
  2  insert_employeee_data;
  3  END;
    select * from employeee;
  4  /
```
### Output:
![image](https://github.com/bharathraj1905/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121490575/30626b33-2354-451c-869c-54ed63878888)
![image](https://github.com/bharathraj1905/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121490575/8ef1336d-c979-4626-9ca5-985b3495d055)


### Result:
this sql program is executed successfully.
