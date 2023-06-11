## nosql vs sql

### What type of database is the best fit for the complex query intensive environment?
SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.

### What type of database is the best fit for hierarchical data storage?

For the type of data to be stored: SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.
### Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

 In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

 ## sql modeling techniques

 ### Among data tables, what is a one-to-many relationship and how do we “relate” them?

 In some cases an entry in one table can be related to more than one entry in another.  This is called a one-to-many relationship.  In our example there are many employees in on department; therefore, we show a many-to-one relationship.

we relate them by using the unique key values of each table

### Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.

When working with SQL databases it is often useful to create diagrams of the database tables and their relationships. 

### Explain the difference between a primary and foreign key.

**The Primary Keys**. are  uniquely identify each row in a table.  A table typically has one primary key,
**Foreign Key** it is a key used in another table to refer to it 

## sql vs nosql

### How do we treat keywords and parameters differently in SQL syntax?
Keywords: Keywords are reserved words in SQL that have a predefined meaning and are used to specify actions, operations, or conditions in a query. For example, keywords like **SELECT**, **FROM**, **WHERE**, **INSERT**, **UPDATE**, **DELETE**, **JOIN**, and **GROUP BY** are used to structure and define the operations and conditions in **SQL** statements. 

Parameters: Parameters are placeholders used in SQL statements to represent values that will be provided later during query execution. Parameters are typically denoted using a specific syntax, such as a question mark ("?") or a colon followed by a name (e.g., ":param"). 

### Define normalization within the context of schemas and data.

it refers to the process of organizing and structuring data in a relational database to minimize redundancy, improve data integrity, and optimize query performance.

### Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

**One-to-One Relationship** For example, think of a person and their passport. Each person can have only one passport, and each passport belongs to only one person.

**One-to-Many Relationship:**
For instance, consider a university and its students. A university can have many students, but each student belongs to only one university. 

**Many-to-Many Relationship:** A book can have multiple authors, and an author can write multiple books.

## sequelize api

Sequelize is a promise-based Node.js ORM tool for Postgres, MySQL, MariaDB, SQLite, Microsoft SQL Server, Oracle Database, Amazon Redshift and Snowflake’s Data Cloud. It features solid transaction support, relations, eager and lazy loading, read replication and more.