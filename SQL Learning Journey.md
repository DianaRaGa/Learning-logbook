# **Intro To SQL**
**SQL = Structured Query Language**

**SQL**: Programming language designed to manipulate data stored in relational databases.

**Relational database**: Database that organizes information into one or more tables.

**Table**: Collection of data organized into rows and columns.

## **Statement** 
String of characters that the database recognizes as valid commands:

**CREATE TABLE** → Creates a new table

**INSERT INTO** → Adds a new row to a table

**SELECT** → Queries data from a table

**ALTER TABLE** → Changes an existing table

**UPDATE** → Edits a row in a table

**DELETE FROM** → Deletes rows from a table

## **Column Constrains**

Rules applied to the values of individual columns:

**PRIMARY KEY** → To uniquely identify the row

**UNIQUE** → So that it has a different value for every row

**NOT NULL** → Columns must have a value

**DEFAULT** → Assigns a default value for the column when no value is specified

## **Statements in use**

```sql 
CREATE TABLE table_name (
  column1 datatype,
  column2 datatype,
  column3 datatype
);
```