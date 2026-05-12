# University Database Management System

## Features
- Create and manage relational tables: Students, Departments, Courses, Instructors, Enrollments
- Insert sample records for testing queries
- Perform CRUD operations:
  - **Create**: Insert new records
  - **Read**: Select queries with filters, joins, and aggregations
  - **Update**: Modify student emails, course credits, instructor salaries
  - **Delete**: Remove specific enrollments
- Execute advanced SQL queries:
  - Joins (INNER, LEFT)
  - Aggregations (COUNT, AVG, MAX)
  - Subqueries
  - Window functions (running totals)
  - Conditional logic (CASE statements)
- Demonstrates practical academic database use cases

## Program Flow
1. **Database Creation**
   - Create `FINAL` database
   - Define tables with primary keys, foreign keys, and constraints
2. **Data Insertion**
   - Populate Students, Departments, Courses, Instructors, Enrollments
3. **Basic Queries**
   - Select all records from tables
   - Update and delete operations
4. **Intermediate Queries**
   - Joins between Students, Courses, Departments, Instructors
   - Aggregations with `GROUP BY` and `HAVING`
   - Subqueries for conditional filtering
5. **Advanced Queries**
   - Window functions for running totals
   - CASE statements for classification (Senior/Junior)
   - String concatenation for instructor names
   - Extracting year from dates
6. **Output**
   - Query results demonstrate database relationships and analytics

## Concepts Used
- **Database Design**
  - Primary keys, foreign keys, constraints
- **SQL Operations**
  - DDL (CREATE TABLE), DML (INSERT, UPDATE, DELETE), DQL (SELECT)
- **Joins**
  - INNER JOIN, LEFT JOIN
- **Aggregate Functions**
  - COUNT, AVG, MAX
- **Subqueries**
  - Nested SELECT statements
- **Window Functions**
  - Running totals with `OVER()`
- **Conditional Logic**
  - CASE statements for classification
- **String Functions**
  - CONCAT for full names
- **Date Functions**
  - YEAR(), DATEDIFF() for calculations
