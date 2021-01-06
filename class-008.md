# Class 08 Reading Notes - SQL

### SQL
- SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database.
- Due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.
- There are many popular SQL databases including SQLite, MySQL, Postgres, Oracle and Microsoft SQL Server.
- All of them support the common SQL language standard, which is what this site will be teaching, but each implementation can differ in the additional features and storage types it supports.
- A relational database represents a collection of related (two-dimensional) tables.
- Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.
- By learning SQL, the goal is to learn how to answer specific questions about this data, like "What types of vehicles are on the road have less than four wheels?", or "How many models of cars does Tesla produce?", to help us make better decisions down the road.
- To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries.
- A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned. 
- It has a specific syntax though, which is what we are going to learn in the following exercises.
- You can think of a table in SQL as a type of an entity (ie. Dogs), and each row in that table as a specific instance of that type (ie. A pug, a beagle, a different colored pug, etc).
- This means that the columns would then represent the common properties shared by all instances of that entity (ie. Color of fur, length of tail, etc).
- Using SQL: FIND XX FROM XX; -- i.e. FIND title FROM movies; -- this searched for only the titles of the movies from a table

### Cheat Sheet Refs (http://www.cheat-sheets.org/sites/sql.su/)
- CREATE DATABASE database_name -> Create Database
- DROP DATABASE database_name -> Delete a Database
- CREATE TABLE "table_name" ->  Create a Table in a Database
("column_1" "data_type_for_column_1",
"column_2" "data_type_for_column_2",
- ALTER TABLE table_name ADD column_name datatype -> Add columns in an existing table.
- ALTER TABLE table_name DROP column_name datatype ->  Delete columns in an existing table.
- DROP TABLE table_name -> Delete a table.
