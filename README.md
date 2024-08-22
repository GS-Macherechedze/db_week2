# Essential Data Retrieval & Filtering (Focus on Project Data)
This week, we'll dive deeper into your project by mastering essential techniques for retrieving and manipulating your data! We’ll explore the SELECT statement to extract specific information and leverage the power of filtering with the WHERE clause. Finally, we’ll learn to organize our results using ORDER BY.

<br/>

## Learning Objectives:
- Utilize the SELECT statement to retrieve data from your project database.
- Apply wildcards (%) and comparison operators for targeted data retrieval.
- Employ the WHERE clause with logical operators (AND, OR, NOT) to filter data effectively.
- Organize retrieved data using the ORDER BY clause.

<br/>
    
## Instructions
This assignment is designed to be completed in approximately 2 hours.

### What you'll need:
Access to a computer with internet access
A text editor (e.g., Microsoft Word)
Access to a sample project database (or instructor-provided data) that includes the table you designed in Week 1 (e.g., "Records"). See the database script in this repo titled "Week2.txt".

### Scenario:
Imagine you’ve diligently collected and stored data using the database you designed last week. Now, it’s time to analyze that data and gain insights!

<br/>

## Submission:
- Open MySQL WorkBench or any SQL management tool and import the file/database.
- Copy the code in week2.txt and run it in MySQL Workbench.
- Write SQL scripts to answer all questions below.
- Submit your document by uploading it onto this repo.

<br/>

## Part 1: Retrieving Data with SELECT (30 minutes)
Based on the table you designed in Week 1, which likely includes columns like "record_id," "amount," "date," and "category," complete the following tasks:

### Questions
**1.1 Retrieving All Records:**<br/>
Write an SQL query to retrieve all data points (columns) from the table (e.g., "Records").

**1.2 Specific Columns:**<br/>
Modify your query to select only specific columns relevant to your analysis. For example, you might choose "date," "category," and "amount" to analyze data trends by category and date.

**1.3 Filtering by Date Range:**<br/>
Write a query to retrieve records within a specific date range (e.g., January 1, 2021, to December 15, 2024). Remember to use the appropriate data type for the "date" column when specifying the date range in your query.

<br/>

## Part 2: Filtering with WHERE Clause (45 minutes)

### Questions
**2.1 Filtering by Category:**<br/>
Write a query to find all records belonging to a specific category (e.g., "Entertainment").

**2.2 Filtering with Comparison Operators:**<br/>
Find records with an amount greater than a certain value (e.g., $50).

**2.3 Combining Filters (AND):**<br/>
Refine your query to find records that meet multiple criteria. For example, you might search for records greater than $75 AND belonging to the "Food" category.

**2.4 Combining Filters (OR):**<br/>
Modify your query to find records belonging to one category or another (e.g., "Transportation" OR "Groceries").

**2.5 Filtering with NOT:**<br/>
Write a query to display records unrelated to a specific category (e.g., "Rent").

<br/>

## Part 3: Sorting Retrieved Data (45 minutes)

### Questions
**3.1 Sorting by Amount:**<br/>
Write a query to display all records sorted by amount in a specific order (e.g., descending order for highest to lowest values).

**3.2 Sorting by Date and Category:**<br/>
Modify your query to sort records based on multiple columns. For example, you might sort first by date (descending order) and then by category (ascending order) to see recent trends by category.

<br/>

## Part 4: Database Upgrade
Imagine you're tasked by the CIO to expand your database. Practice creating, modifying, and removing a table to manage your data.

### Questions
**4.1 Creating a New Table:**<br/>
We don’t have a table for income yet. Create a table named "Income" with columns for:

income_id (INT) - Primary Key (auto-increment)
amount (DECIMAL(10,2)) - NOT NULL
date (DATE) - NOT NULL
source (VARCHAR(50)) - NOT NULL

**4.2 Adding a New Column:**<br/>
After creating the "Income" table, you realize you also want to track the income category "source" (e.g., "Salary," "Freelance Work"). Use ALTER TABLE to add a new column named "category" of type VARCHAR(50).

**4.3 Removing a Column:**<br/>
Let’s say you decide tracking the income source isn’t necessary for now. Use ALTER TABLE again to remove the "source" column from the "Income" table.

**4.4 Dropping a Table:**<br/>
Imagine you no longer need the "Income" table entirely. Experiment by using DROP TABLE to permanently remove it from your database.

<br/><br/>
## Ensure to save all your queries in a document and upload it onto this repo.
