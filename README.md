-- 1] Library Domain
create database library;
use  library;

-- 2] Entities AND Relationships

-- Entities:
-- Book

-- Attributes: id, author_name, book_name, price

-- Customer

-- Attributes: id, customer_id, book_issue_date, book_return_date

 -- Relationship:
-- There is an implicit relationship between customers and books — a customer issues a book.

-- To formally represent this relationship:

-- You need a foreign key in customers that refers to a book's id.






-- 3] Table Created :

create table  books(
id int,
author_name varchar(20),
book_name varchar(20),
price int 
);

create table customers(
id int,
customer_id int,
book_issue_date date,
book_return_date date
);

-- 4] primary key and Foreign key 

-- Primary key is a unique values in each tables . It cannot be null 
-- foreign key is a key that are reference to other column . It is used to join two tables 

