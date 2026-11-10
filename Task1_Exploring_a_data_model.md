Task 1: Exploring a data model
Provide evidence, then save before moving on.

1.1 – Describe the three layers of abstraction. (3 marks)

- External view shows each user or application only the data it needs
- Conceptual logical level describes the whole database's entities, relationships, and rules, independent of how it is physically stored
- Internal physical level describes how the data is actually stored and accessed, such as files and indexes.

1.2 – Identify one strength of a relational model. (1 mark)

A relational model supports strong data integrity  tables can define relationships and enforce constraints that prevent data duplication and mismatched records

1.3 – Explain the structure of a hierarchical model. (1 mark)

It organizes records in a tree of parent child relationships. Each child typically has one parent, while a parent can have multiple children

1.4 – Which model would be best for applications requiring complex queries and multi-table transactions. (1 mark)

The relational model is the best fit because SQL supports complex queries across related tables

1.5 – Provide an example of Databases that use a key-value model. (1 mark)

Redis is an example of a key-value database. Amazon DynamoDB also supports a key-value data model

1.6 – What is data stored as in a document model. (1 mark)

Data is stored as documents, commonly JSON where each document contains fields or attributes and values

1.7 – Identify one strength of using a key-value model. (1 mark)

It provides fast lookups when the key is known, making it useful for low latency access

1.8 – List one strength for hierarchical models. (1 mark)

 It is very efficient for one to many relationships for example parent child data because the tree structure allows fast navigation and retrieval along defined paths


