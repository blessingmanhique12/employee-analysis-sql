# employee-analysis-sql

Example: Previous Task Submission

________________________________________
Expected Query Results
 
sql
-- Question 1: Write a query to select all employees who work in the 'Engineering' department.
-- This query filters and displays all employees who belong to the Engineering department.
Answer:
SELECT * FROM employees WHERE department = 'Engineering';

-- Question 2: Write a query to select all employees with a salary greater than $70,000.
-- This query returns all employees whose salary is more than $70,000.

Answer:
SELECT * FROM employees WHERE salary > 70000;

-- Question 3: Write a query to select all employees hired after January 1st, 2020.
-- This query shows employees hired after the specified date (excluding January 1st, 2020).
Answer:
SELECT * FROM employees WHERE hire_date > '2020-01-01';

-- Question 4: Write a query to delete all employees who work in the 'HR' department.
-- This query permanently removes all employees from the HR department from the database.
Answer:
DELETE FROM employees WHERE department = 'HR';
________________________________________




New Task: Employee Data Analysis
Instructions for Learners
Step 1: Set up the Database in Supabase
1.	Go to Supabase.com and log in to your account
2.	Open your project dashboard and click on the SQL Editor in the left sidebar
3.	Copy and paste the entire Setup Code below into the editor
4.	Run the SQL to create your employees table with sample data
Step 2: Complete the SQL Tasks
1.	Write SQL queries to solve each problem below
2.	Test your queries in the Supabase SQL Editor to make sure they work
3.	Create a folder on your computer called employee-analysis-task
4.	Inside this folder, create a file named solutions.sql
5.	Copy all your working SQL queries into this file, numbering them clearly
Step 3: Submit to GitHub
1.	Create a new repository on GitHub named employee-analysis-sql
2.	Upload your entire employee-analysis-task folder to the repository
3.	Push your code to complete the assignment
________________________________________
Setup Code (Run this in Supabase first)
sql
-- Create and populate the employees table
CREATE TABLE employees (
    employee_id INT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE,
    city VARCHAR(50),
    performance_rating INT
);

INSERT INTO employees ("employee_id", "first_name", "last_name", "department", "salary", "hire_date", "city", "performance_rating") 
VALUES 
('1', 'John', 'Smith', 'Engineering', '75000.00', '2020-03-15', 'New York', '8'),
('2', 'Sarah', 'Johnson', 'Marketing', '65000.00', '2019-07-22', 'Chicago', '9'),
('3', 'Michael', 'Brown', 'Engineering', '82000.00', '2018-11-05', 'New York', '7'),
('4', 'Emily', 'Davis', 'HR', '55000.00', '2021-01-30', 'Boston', '6'),
('5', 'David', 'Wilson', 'Sales', '70000.00', '2020-09-12', 'Chicago', '8'),
('6', 'Lisa', 'Anderson', 'Engineering', '90000.00', '2017-05-10', 'Boston', '9'),
('7', 'James', 'Miller', 'Marketing', '60000.00', '2022-02-28', 'New York', '7');
________________________________________
SQL Tasks
Add your solutions to the solutions.sql file:
-- Question 1: Write a query to select all employees who work in the 'HR' department.
-- This query filters and displays all employees who belong to the HR department.


-- Question 2: Write a query to select all employees with a salary greater than $80,000.
-- This query returns all employees whose salary is more than $80,000.


-- Question 3: Write a query to select all employees hired after January 1st, 2019.
-- This query shows employees hired after the specified date (excluding January 1st, 2019).


-- Question 4: Write a query to delete all employees who work in the 'Sales' department.
-- This query permanently removes all employees from the Sales department from the database.
MAKE SURE YOU SCREENSHOT ALL THE OUTPUTS WHEN YOU ARE RUNNING SQL QUERY
________________________________________
Detailed GitHub Submission Steps
1.	Create GitHub Repository:
o	Go to github.com and log in
o	Click the "+" icon in the top right and select "New repository"
o	Name it employee-analysis-sql
o	Check "Add a README file"
o	Click "Create repository"
2.	Prepare Your Files:
o	Create the folder employee-analysis-task on your computer
o	Create solutions.sql inside this folder with your answers
o	Your file structure should look like:
text
employee-analysis-task/
└── solutions.sql
3.	Upload to GitHub:
o	In your GitHub repository, click "Add file" → "Upload files"
o	Drag and drop your employee-analysis-task folder
o	Add a commit message like "Add SQL solutions"
o	Click "Commit changes"
4.	Verify Submission:
o	Check that your repository shows the folder and SQL file
o	Ensure all your queries are properly formatted in the file
Your final submission should have this structure:
text
employee-analysis-sql/          (GitHub Repository)
└── employee-analysis-task/     (Folder)
    └── solutions.sql           (File with your SQL answers)
