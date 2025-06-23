#Library Management System - Database Schema Design

#Objective:
This project is a simple database schema design for the domain- Library Management System, built using MySQL and it basically covers fundamental database concepts such as:
- DDL (Data Definition Language)
- ER Diagram design and relationships
- Primary and Foreign Keys


#Tools that I have used:
- MySQL Workbench (for schema creation and ER diagram)
- SQL (Structured Query Language)
- GitHub (for version control and submission)

#What happened in the SQL Script:
This repo contains 3 files, that is this readme file as a go through basis and then an ER Diagram of the Schema built for Library Management System. 
It incules Entities and Attributes:
1. Authors-
- `author_id` (Primary Key)  
- `name`  
- `nationality`  

2. Books-
- `book_id` (Primary Key)  
- `title`  
- `genre`  
- `publication_year`  
- `author_id` (Foreign Key → Authors)

3. Members-  
- `member_id` (Primary Key)  
- `name`  
- `email` (Unique)  
- `join_date` (Default: current date)

4. Borrow_Records-  
- `record_id` (Primary Key)  
- `member_id` (Foreign Key → Members)  
- `book_id` (Foreign Key → Books)  
- `borrow_date`  
- `return_date`

