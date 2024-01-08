# SQL2_Uebungen
# SQL Exercise 3
Create the tables and insert data from the following files:
- [Parts insert and create tables](https://github.com/DaStanzel/Unterlagen-Datenbanken-CB/blob/main/%C3%9Cbungen/SQLUebung03/parts.sql)
- [Tennis Create Tables](https://github.com/DaStanzel/Unterlagen-Datenbanken-CB/blob/main/%C3%9Cbungen/SQLUebung03/tennis-tables.sql)
- [Tennis Insert Data](https://github.com/DaStanzel/Unterlagen-Datenbanken-CB/blob/main/%C3%9Cbungen/SQLUebung03/tennis-insert.sql)
- [EmpDept.sql](https://github.com/DaStanzel/SQLUebung02/blob/main/dept_emp.sql) (Create the tables DEPT and EMP)

*If there are issues with the Date Format in Oracle SQL Developer change them in Tools -> Preferences -> Database -> NLS -> Date Format: "DD-MM-YY"

## 1-8 Tennis queries
1. Output of PLAYERNO, NAME of players born after 1960.
2. Output of PLAYERNO, NAME and TOWN of all female players who do not reside in Stratford.
3. Output of player numbers of players who joined the club between 1970 and 1980.
4. Output of PlayerId, Name, Year of Birth of players born in a leap year.
5. Output of the penalty numbers of the penalties between 50,- and 100,-.
6. Output of PlayerId, name of players who do not live in Stratford or Douglas.
7. Output of playerId and name of players whose name contains 'is'.
8. Output of all hobby players.

## 9 - 21 EmpDept queries
9. Output of those employees who receive more commission than salary.
10. Output of all employees from department 30 whose salary is greater than or equal to 1500.
... [List continues with similar format for remaining queries]

# SQL Exercise 4

## 1-6 Tennis query
1. Output TEAMNO of the teams in which the player with the number 27 is not captain
2. Output of PLAYERNO, NAME and INITIALS of the players who have won at least one match
... [List continues with similar format for remaining queries]

## 7-12 EmpDept query
7. Search all departments, which have no employees
8. Search all employees who have the same job as JONES
... [List continues with similar format for remaining queries]

# SQL Exercise 5

## 1-11 Tennis query
1. Number of new players per year
2. Number and average amount of penalties per player
... [List continues with similar format for remaining queries]

## 12-19 EmpDept query
12. Output of all employees from department 30 sorted by their salary starting with the highest salary.
13. Output of all employees sorted by job and within the job by their salary
... [List continues with similar format for remaining queries]

# SQL Exercise 6

## 1-5 Tennis query
1. NAME, INITIALS and number of sets won for each player
2. NAME, PEN_DATE and AMOUNT sorted in descending order by AMOUNT
... [List continues with similar format for remaining queries]

## 6-9 EmpDept query
6. In which city does the employee Allen work?
7. Search for all employees who earn more than their supervisor
... [List continues with similar format for remaining queries]

# SQL Exercise 7

## 1-4 Tennis query
1. Output of players' names who played for both team 1 and team 2.
2. Output the NAME and INITIALS of the players who did not receive a penalty in 1980
... [List continues with similar format for remaining queries]

## 5-8 EmpDept query
5. Find all employees whose salary is higher than the average salary of their department
6. Identify all departments that have at least one employee
... [List continues with similar format for remaining queries]

# SQL Exercise 8

- Creating the PARTS table ([Parts insert and create tables](https://github.com/DaStanzel/Unterlagen-Datenbanken-CB/blob/main/%C3%9Cbungen/SQLUebung03/parts.sql))
- Display the whole hierarchy of those parts that make up P3 and P9
- At which hierarchy level is P12 used in P1
- How many parts to P1 cost more than $20
- Output of all direct and indirect employees belonging to JONES (without JONES itself, with corresponding indentation per hierarchy)
- Output of all direct and indirect superiors of SMITH (including SMITH itself)
- Output of the average salary for each hierarchy level

# SQL Exercise 6 using Joins

Solve exercise 6 using Joins.

# SQL Exercise 7 using Joins

Solve exercise 7 using Joins.

# Competence Check

## Tables
Create the following tables like shown in the [Class Diagram](https://github.com/DaStanzel/Unterlagen-Datenbanken-CB/blob/main/Übungen/Joins/codersbay_ue6.jpg)

### Class Diagram
Table description:
- REGIONS contains rows that represent a region (for example, North, South America, Asia).
- COUNTRIES contains rows for countries. Each row is linked to a region.
- LOCATIONS contains the addresses of specific offices, warehouses and/or production sites of a company in a specific country.
- DEPARTMENTS displays department details where employees work. Each department can have a relationship that represents the head of department in the EMPLOYEES table.
- EMPLOYEES contains details of each employee working for a department. Not all employees must be assigned to a department.
- JOBS contains the types of positions that each employee can hold.
- JOB_HISTORY contains the individual positions that the employee has held so far.
- JOB_GRADES identifies a salary range per pay grade level. The salary ranges do not overlap.

For inserting use the insert script file which is in the repository.

## Selects and Joins

1. The management would like a list of the different salaries per job. The output should contain the job_id as well as the sum of the salaries per job_id. In addition, the output should be sorted in descending order according to the sum of the salaries.
2. The personnel department wants to have information about the average salary of the employees at the current time.
3. The personnel department would like a list of all employees (first name, last name), on which the department name (department_name) is also displayed.
4. For the new stationery, the secretary's office needs a list of all departments (department_name) as well as their address consisting of the postal code, the city, the province, and the street_address.
5. The secretariat thanks for the list, but would like to have the name of the country in addition.
6. The secretariat thanks for the updated list. Embarrassed, the first and last name as "Manager" of the respective manager of the department is now requested in addition.
7. The personnel department needs a list of the employees with the following contents:
   - 7.1.) First and last name as "Name"
   - 7.2.) job_title as "job"
   - 7.3.) The salary
   - 7.4.) The department name
8. The new General Manager asks you to find out which subordinates each employee has. You could now collect the data manually, but something stirs inside you when you feel the challenge of generating the result via Oracle. Accept it!


