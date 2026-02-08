# Data Migration
Migrating data from SQL Server to PostgreSQL

# Preface

This project is about migrating data from SQL Server to PostgreSQL.

I'm using following tech stack:

- SQL
- Python
- Jupyter Notebook

# Migration Steps

## High Level

1. Audit the data in SQL Server (Before migration)
2. Extract the data from SQL Server (SSMS)
3. Transform the data
4. Load the data in PostgreSQL
5. Validate the data (After migration)
6. Generate a validation report

## Low Level 

1. Create a .env file
2. Load env variables
3. Connect to SQL Server using pyodbc
4. Connect to PostgreSQL using psycopg2
5. Audit the data
6. For each table:
   - Get row count
   - Extract all rows
   - Transform the column names to lower case
   - Convert the data types
   - Create the tables in PostgreSQL
   - Load the tables into PostgreSQL
7. Run post-data migration checks
8. Generate a validation report

