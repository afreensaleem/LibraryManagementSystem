# Library Management System

This repository contains the SQL file for a Library Management System database (`libraryDB.sql`).  
It includes the database structure, tables, relationships, and sample data to demonstrate basic library management functionality.

## Tables Included

1. **author** – Stores author information  
   - Columns: `id` (Primary Key), `name`

2. **categories** – Stores book categories  
   - Columns: `id` (Primary Key), `category_name`

3. **book** – Stores book details  
   - Columns: `id` (Primary Key), `title`, `author_id` (Foreign Key), `category_id` (Foreign Key)

4. **members** – Stores library member information  
   - Columns: `id` (Primary Key), `name`, `email`, `membership_date`

5. **borrow** – Tracks borrowed books  
   - Columns: `id` (Primary Key), `member_id` (Foreign Key), `book_id` (Foreign Key), `borrow_date`, `return_date`

## Features

- Primary and foreign key relationships to ensure data integrity.  
- Sample data included in each table for testing purposes.  
- Can be imported into MySQL or any SQL-compatible database.

## How to Use

1. Download the `libraryDB.sql` file.  
2. Open your terminal and run:

```bash
mysql -u root -p < libraryDB.sql
