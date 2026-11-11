PA0603 Create relationships



Scenario
You’ve just been hired as the database administrator for a sci-fi book retail startup called NebulaStore. The company offers curated science fiction novels available for its users through an online platform. As the business expands, operational issues are beginning to surface. Customer information is scattered, inventory records are inconsistent, and order details are difficult to track. There is currently no structured system in place to organise and manage the essential data the company relies on to function efficiently.



Your job is to design the foundational structure of the database.

NebulaStore has the following tables and their attributes to keep track of its information:

Customer <customer_id, customer_name, customer_email, customer_phone>
Books <isbn, author, title, edition, quantity>
Orders <order_id, customer_id, isbn, address>
Task 1: NebulaStore
Provide evidence, then save before moving on.

1.1 – What is the cardinality of the relationship between Customer and Order? (1 mark)

One to many one customer can place many orders, while each order row refers to one customer through Orders.customer_id

1.2 – What is the cardinality of the relationship between Book and Order? (1 mark)

One to many one book can appear in many order rows, while each order row refers to one book through Orders.isbn

1.3 – Explain the cardinality of the relationship between Customer and Book. (2 mark)

Many to many through Orders a customer can order many books, and a book can be ordered by many customers. The Orders table links them using customer_id and isbn

A fourth table has been added.

CustomerAccount <customer_id, username, password_hash, account_create_date>

1.4 – Which table will CustomerAccount have a one-to-one relationship with? (1 mark)

Each Customer has exactly one CustomerAccount and each CustomerAccount belongs to exactly one Customer 1:1. CustomerAccount contains customer_id as its key and the scenario implies each customer has one account (one username and password per customer). The customer_id uniquely ties one account record to one customer record

