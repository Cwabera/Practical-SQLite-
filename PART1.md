Whats is a Primary Key 
A primary key is a unique identifier for a record in a database table. It ensures that every row is distinct and cannot be null. In our bookstore database,id serves as the primary key for all tables.

What is a Foreign Key?
A foreign key is a column that creates a link between two tables. It refers to the Primary Key of another table, establishing a relationship. For example, customer_id in the Orders table points to the id in the customer table.


Relationship Types
One-to-many (1:M): A sigle record in one table is related to multiple records in another. 

example: One customer can place many orders, but each order belongs to only one customer .


Many-to-Many(M:N): Multiplr records in one table relate to multiple records in another. 

example: One order can contain many books, and one book can appear in many different orders. This is handleded using the order_items bridge table.


Database Normalization
Normalization is the process of organizing data to redce redundancy and improve data integrity. by spiliting our data into four tables (Customer Books, Orders, Order_Items), we ensue that if a customer changes their name , we only have to update it in one place.