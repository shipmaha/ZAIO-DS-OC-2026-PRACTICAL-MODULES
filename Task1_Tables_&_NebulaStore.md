Task 1: Tables & NebulaStore
Provide evidence, then save before moving on.

1.1 – What do the attributes and tuples in a table represent? (2 marks)

Attributes are the columns the properties recorded for each item. tuples are the rows individual records

1.2 – What can you do with a table? (3 marks)

You can insert records, retrieve or query records, and update or delete records. Queries can also filter and sort records to find useful information.

You’ve just been hired as the database administrator for a sci-fi book retail startup called NebulaStore. The company offers curated science fiction novels available for its users through an online platform. As the business expands, operational issues are beginning to surface. Customer information is scattered, inventory records are inconsistent, and order details are difficult to track. There is currently no structured system in place to organise and manage the essential data the company relies on to function efficiently.



Your job is to design the foundational structure of the database.

NebulaStore needs to keep track of:

Who the customers are
What books exist in inventory
What orders have been placed


2.1 – Identify three entities or tables that this database will need to model. (3 marks)

- Customers
- Books
- Orders

2.2 – For the first entity or table identify at least four attributes. (4 marks)

Customers: CustomerID (primary key), FirstName, LastName, Email (unique)

2.3 – For the second entity or table identify at least four attributes. (4 marks)

Books: BookID (primary key), ISBN (unique candidate key), Title, Price

2.4 – For the third entity or table identify at least four attributes. (4 marks)

Orders: OrderID (primary key), CustomerID (foreign key), OrderDate, TotalAmount

2.5 – Differentiate a primary key from a candidate key. (2 marks)

A candidate key is a combination of attributes, that can uniquely identify a row. A primary key is the candidate key selected as the table's main identifier. A table can have several candidate keys, but only one primary key, the primary key must be unique and not null

2.6 – Identify at least one possible attribute that could be used as a foreign key for each table. (3 marks)

A foreign key is in the table that references another table. Orders.CustomerID references Customers.CustomerID. Customers.CustomerID and Books.BookID are primary keys in their own tables and can be referenced by other tables, they do not need foreign key columns themselves
