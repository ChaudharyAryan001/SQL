# Event Management Database System

## Features
- **Database Creation**: `event` database with normalized tables
- **Entities**:
  - Venues
  - Organizers
  - Events
  - Attendees
  - Tickets
  - Payments
- **Relationships**:
  - Events linked to Venues and Organizers
  - Tickets linked to Events and Attendees
  - Payments linked to Tickets
- **CRUD Operations**:
  - Insert, Update, Delete records
  - Query with filters (`WHERE`, `LIKE`, `HAVING`, `LIMIT`)
- **Advanced SQL Queries**:
  - Joins (INNER, LEFT, RIGHT, FULL OUTER via UNION)
  - Aggregations (SUM, COUNT, AVG)
  - Subqueries
  - Window Functions (RANK, Cumulative Sales, Running Totals)
  - CASE Expressions for categorization
  - String and Date functions

---

## Program Flow
1. **Database Setup**
   - Create `event` database
   - Define tables with primary keys, foreign keys, constraints
2. **Data Insertion**
   - Populate Venues, Organizers, Events, Attendees, Tickets, Payments
3. **Basic Operations**
   - Insert new events
   - Update ticket prices
   - Delete events
   - Search using `LIKE`
4. **Intermediate Queries**
   - Joins between tables
   - Aggregations with `GROUP BY` and `HAVING`
   - Filtering with `AND`, `OR`, `NOT`
   - Sorting with `ORDER BY`
5. **Advanced Queries**
   - Revenue calculations per event
   - Attendee counts per event
   - Ranking events by revenue
   - Subqueries for above-average revenue
   - Window functions for cumulative sales and running totals
6. **Utility Functions**
   - Date functions: `MONTH()`, `DATEDIFF()`, `DATE_FORMAT()`
   - String functions: `UPPER()`, `TRIM()`, `IFNULL()`
   - CASE expressions for demand and payment status categories

---

## Concepts Used
- **Database Design**
  - Normalized schema with relationships
- **SQL Operations**
  - DDL (CREATE TABLE), DML (INSERT, UPDATE, DELETE), DQL (SELECT)
- **Joins**
  - INNER, LEFT, RIGHT, FULL OUTER (via UNION)
- **Aggregate Functions**
  - SUM, COUNT, AVG, MAX
- **Subqueries**
  - Nested SELECT with conditions
- **Window Functions**
  - RANK, cumulative totals, running totals
- **Conditional Logic**
  - CASE expressions for categorization
- **Date Functions**
  - Extract month, calculate remaining days, format dates
- **String Functions**
  - Uppercase, trim spaces, replace NULL values


INNER JOIN tickets t ON e.event_id = t.event_id
INNER JOIN payments p ON t.ticket_id = p.ticket_id
GROUP BY e.event_name
ORDER BY total_revenue DESC
LIMIT 5;
