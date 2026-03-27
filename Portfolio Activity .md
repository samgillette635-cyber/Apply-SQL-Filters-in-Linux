Apply Filters to SQL Queries

This project demonstrates how I applied SQL queries and filters in a Linux environment to support system security initiatives. My work focused on ensuring the organization's systems are secure, investigating potential security issues, and updating employee computers as needed.

Project Description
I used SQL queries and filters to retrieve specific information from two tables (log_in_attempts and employees) for security and operational purposes. The following are examples of the queries and filters I implemented.

1. Retrieve After-Hours Failed Login Attempts
Goal: Find failed login attempts after 18:00. 
  - Select -From- login_attempts– retrieve all data.  
  - WHERE login_time > '18:00' AND success = FALSE – filter for failed attempt's after 6 PM.

2. Retrieve Login Attempts on Specific Dates
**Goal:** Retrieve login attempts on `2022-05-08` or `2022-05-09`. 
  - `SELECT * FROM log_in_attempts`  
  - `WHERE login_date = '2022-05-08' OR login_date = '2022-05-09'` – show attempts on either date.

3. Retrieve Login Attempts Outside of Mexico
**Goal:** Filter for login attempts not in Mexico.  
  - `SELECT * FROM log_in_attempts`  
  - `WHERE country NOT LIKE 'MEX%'` – excludes both `MEX` and `MEXICO`.  
  - `%` acts as a wildcard for any characters.

4. Retrieve Employees in Finance or Sales
**Goal:** Return all employees in Finance or Sales departments.  
  - `SELECT * FROM employees`  
  - `WHERE department = 'Finance' OR department = 'Sales'` – OR is used to include both departments.

5. Retrieve All Employees Not in IT
**Goal:** Filter employees who are not in the IT department.  
  - `SELECT * FROM employees`  
  - `WHERE department NOT LIKE 'IT%'` – excludes IT/Information Technology.
