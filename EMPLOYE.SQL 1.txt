CREATE DATABASE Company;
CREATE DATABASE Company;
USE Company;

 CREATE TABLE Employee(
Emp_Id VARCHAR(20) PRIMARY KEY,
  Name CHAR(20) NOT NULL,
  Age INT NOT NULL,
  R_Address VARCHAR(25) NOT NULL,
  Salary FLOAT NOT NULL
 );
 
INSERT INTO Employee (Emp_Id, Name, Age, R_Address, Salary)
VALUES
('E12', "Ghanwa", 17, 'Nawabshah', 50000.00),
('E02', "Aqsa", 19, 'Karach', 60000.00),
('E61', "Vingus", 18, 'Larkana', 70000.00),
('E11', "Fatima", 18, 'Karachi', 55000.00),
('E40', "Kausar", 18, 'Nawabshah', 65000.00),
('E55', "Sanam", 20, 'Nawabshah', 64000.00),
('E67', "Saba", 27, 'Lahore', 2000.00),
('E10', "Muskan", 20 , 'Larkana', 68000.00);


SELECT * FROM Employee;

SELECT * FROM Employee WHERE R_Address ='Larkana' AND R_Address='Nawabshah';

SELECT Emp_Id,Salary,R_Address FROM Employee Where Salary>=3000;

SELECT Name,Age,R_Address FROM Employee Where age<=20;

SELECT * FROM Employee Where R_Address!='Larkana';

SELECT Name,Salary,R_Address FROM Employee Where Salary>=500000 or R_Address='Lahore';