## Overview
PostgreSQl is a RDBMS that performs simple and advanced queries, data definition and data manipulation through SQL.

We'll work with complex data types, regexp, views, indexing, and store procedures. Also about transaction control, administration, securioty, replication, and performance tuning.

Methods for backup, restore and recovery.

Upgrading and migration from legacy systems.

## PostgreSQL
PostgreSQL, or Postgres, is a free and open-source object-oriented relational database management system (RDBMS) emphasizing extensibility and technical standards compliance. It was initially named POSTGRES, referencing its origins as a successor to the Ingres Database developed at the University of California, Berkeley.

PostgreSQL is ACID-compliant and supports foreign keys, joins, views, triggers, and stored procedures (in multiple languages). It includes most SQL data types, including INTEGER, NUMERIC, BOOLEAN, CHAR, VARCHAR, DATE, INTERVAL, and more.

PostgreSQL has a strong reputation for its proven architecture, reliability, data integrity, extensibility, and performance. PostgreSQL supports functions and stored procedures in multiple languages, including SQL, Perl, Python, Tcl, and Java.

## Benefits of using a database, such as:

Fast and Efficient: Databases are efficient at storing data. We can store and access data quickly. PostgreSQL is known for its speedy performance.

Versatile: Databases support various data types, such as text, pictures, videos, etc. We use databases for various applications, such as storing, managing inventory, or tracking financial transactions. We can use PostgreSQL as a back-end database for our web applications.

Scalable: Databases can be scaled to support vast amounts of data. We can even use PostgreSQL for big data analytics. It’s fast and reliable, making it a good choice for high-traffic websites.

Concurrent: Databases can be used by multiple users concurrently. PostgreSQL supports concurrent transactions, meaning multiple users can access and modify the data simultaneously without affecting the data’s integrity.

Secure: Databases provide security features to protect data from unauthorized access. We can use databases to store sensitive data. PostgreSQL supports security features such as role-based access control and data encryption.

Reliable: Databases are more reliable (than file-based storage systems), and we can keep backups to prevent data loss. PostgreSQL is known for its reliability. It can handle heavy loads and can recover from crashes.

## What are the disadvantages of using a database? 
There are some disadvantages of using a database, including:

Cost: Databases can be expensive to set up and maintain.

Complex: Databases can be complex to use, particularly for non-technical users.

Training: We must learn how to use a database before utilizing it.

Support: Users must have access to support in case of problems.

Inflexible: It can be challenging to change the existing data structure of a database.

## Types of databases
- Relational databases

- Non-relational databases

### Relational databases
A relational database is a type of database that stores data in tables. We usually connect tables by relationships; this allows the data to be easily accessed and used. For example, a “Customer” table might contain customer information such as their names, addresses, and phone numbers. But the “Customer” table might also include a relationship to the “Product” table, which would store information about each product a customer has purchased. A relational database allows the data to be easily accessed and used. Relational databases are also called SQL databases.

### ACID property of a database
ACID is a set of four properties that guarantee the consistency and integrity of data in a database. The ACID properties are:
1. Atomicity: all the queries in a group must be executed or none of them will be executed.
2. Consistency: the db needs to be consistent after all the queries in a group have been executed.
3. Isolation: the execution of one group of queries will not affect the execution of another.
4. Durability: the results of all the queries in a group will be permanent, even if system fails.

ACID properties are essentials because they guarantee that data in a database is consistent and reliable. Without the ACID properties, data could become corrupted or lost.

## Non-relational database
Non-relational databases don’t store data in tables. Instead, they store data in a format that’s easy to use and understand. For example, we can represent a customer with a JSON document containing information about the customer, such as the customer’s name, address, and phone number. We can use this database for web applications that need to store data in a format that’s easy to use and understand. Non-relational databases are known as NoSQL databases.

Relational databases are better for storing data that we can organize in a well-defined way. They’re also better for running complex queries on large amounts of data. Non-relational databases are a good option for storing data that are not well-defined or for storing data in a format that’s easy to use and understand.

Both relational and non-relational databases have their advantages and disadvantages. It’s vital to choose the right type of database for your needs.

### Need for non-relational databases
Non-relational databases, or NoSQL databases, store and manage large-scale data. They are especially useful for managing unstructured data, such as text or images. They can also be used to store data accessed frequently, such as user activity logs.

Non-relational databases are designed to handle large-scale data more efficiently than traditional relational databases. Companies with large datasets, such as social media networks and online retailers, often use them.

Popular non-relational databases
The most popular non-relational databases include MongoDB, Cassandra, and HBase. These databases are used by companies such as Facebook, Twitter, and LinkedIn. They offer features not available in traditional relational databases, such as the ability to handle large-scale data and the flexibility to add and remove data.

The list below mentions the different NoSQL database systems we can encounter:

Object/document database

Column store database (Hypertable)

Key-value pair store database

Graph database

Bigtable implementation (HBase)

Spatial database

Databases with the MapReduce programming model

Multi-model database system

## Introduction to PostgreSQL
PostgreSQL is a powerful, open-source object-relational database system. It was first released in 1986, and since then, it has remained one of the most advanced database management systems. A strong developer community has actively maintained it for over 30 years. It’s known for its reliability, feature robustness, and performance. It’s available under the terms of the PostgreSQL License, a liberal open-source license.

PostgreSQL, being an object-relational database, can store data in objects. This allows data to be related to each other through relationships between objects rather than just through common fields. It supports both SQL for relational data and JSON for non-relational data. PostgreSQL is ACID compliant, meaning it supports transactions and maintains data integrity.

### PostgreSQL is a powerful database system well-suited for OLTP and OLAP applications. It’s easy to use and has many features that make it a good choice for various applications.

Online transaction processing
Online transaction processing (OLTP) is a type of database processing that deals with transactions, such as data entry and retrieval. We typically use OLTP databases for online applications that require real-time data access, such as e-commerce websites and ATM systems.

Press
+
to interact



Challenges of an OLTP system
OLTP systems can be highly complex, making them difficult to design and implement due to the following challenges:

They must handle a large number of transactions quickly and efficiently.

They must be highly available, meaning they can’t go down for even a short period.

They must be secure to prevent data loss or corruption.

Online analytical processing 
Online analytical processing (OLAP) is a type of database processing that deals with analytical data, such as data mining and business intelligence. We typically use OLAP databases for decision support applications requiring complex queries, such as financial and market analysis.

Press
+
to interact



Challenges of an OLAP system
OLAP systems are also very complex, making them difficult to design and implement due to the following challenges:

OLAP systems must handle large amounts of data quickly and efficiently.

They must be able to support complex queries.

They must be highly available, meaning they can’t go down for even a short period.

Advantages of PostgreSQL
PostgreSQL has many advantages over other database systems. Some of these advantages include the following:

It’s open source so anyone can contribute to its development.

It has many features, making it a good choice for many applications.

It’s very popular, so there’s a large community of users and developers to help us if we have questions or problems.

It’s very scalable, so it can handle large amounts of data.

Disadvantages of PostgreSQL
Like any software, PostgreSQL has some disadvantages. Some of these include:

It can be complex to set up, administer, and configure.

It can be challenging to learn, as its learning curve can be steep.

### Key features
PostgreSQL is a popular ORDBMS emphasizing extensibility and standards compliance. It has many features to help developers build applications, help administrators protect data integrity and performance, and help us manage our data no matter how big or small the dataset. PostgreSQL has many features that make it one of the most advanced databases. Some of the features of PostgreSQL include:

It supports several data types, enabling applications to store different data in the same database (e.g., text, images, numbers, etc.).

It can also query that data in various ways.

It can natively store, index, and query JSON documents.

It supports advanced data types such as arrays, JSON, XML, and HStore.

widget
PostgreSQL supports geospatial data, meaning that applications can easily store and query data about location (e.g., mapping applications).

Press
+
to interact



HStore is a data type that allows us to store key-value pairs in a PostgreSQL database. It can help store data that doesn’t fit into the traditional relational schema, such as product information or user preferences.

widget
PostgreSQL provides support for complex queries, transactions, and stored procedures. These features are essential for applications that need to be able to query the data in complex ways. It supports advanced SQL features such as typical table expressions (WITH), windowing functions, and recursive queries. It even helps run DDL commands inside a transaction block.

PostgreSQL supports nested transactions. It means we can start a transaction inside another transaction. Nested transactions can be helpful if we want to ensure that transactions make all of the changes, even if the database rolls back the outer transaction.

PostgreSQL supports concurrency without reading locks. This means we can execute multiple transactions simultaneously without waiting for each other to finish.

Performance, robustness, and stability 
PostgreSQL is an excellent choice for applications that need to be able to handle a lot of data and queries. It also makes it suitable for building applications that must be reliable and run long without interruption. In addition to the standard B-tree indexes, PostgreSQL also offers GIN and GiST indexes, which we can use for more complex data types such as arrays and HStore.

We can use the cascading replication feature of PostgreSQL for sharding solutions. We can change one database to be transparently replicated to multiple databases using cascading replication.

Materialized views allow for pre-computing joins and aggregations, improving query performance.

Multiple users and user roles 
Depending on their role, PostgreSQL allows different user access levels to the data. It also provides robust security features like role-based access control, data encryption, and secure connections.

Press
+
to interact



Storage types and extensibility
PostgreSQL supports multiple storage types:

Tablespaces: These are a means of organizing data within the database. We can use tablespaces to store data in different physical locations which can be helpful if we want to keep data on other disks or servers.

Clusters: These are groups of tables that are stored together. We can use clusters to improve performance by storing frequently accessed data.

Partitions: These divide data into smaller pieces. We can use partitions to improve performance by only accessing the needed data. It can be helpful if we want to store data on different disks or servers.

PostgreSQL has an extensible architecture. It allows for creating custom data types, functions, and operators. Foreign data wrappers allow PostgreSQL to query other data sources like regular tables.

Trigger and asynchronous commit
PostgreSQL supports trigger-based event notifications. We can set up triggers to notify us when certain events occur.

PostgreSQL also supports asynchronous commits. This means we can commit a transaction without waiting for all the other transactions to finish.

Conclusion
There are many reasons to learn PostgreSQL. Here are some of the key ones:

It’s a popular database system used by many big companies, such as Netflix, Uber, Instagram, and many others.

It’s open-source, so we can use it for free. We can also contribute to its development if we want.

It has a strong developer community that’s constantly improving the system.

It has many features that make it a good choice for a wide variety of applications.

### Key takeaways
Object-relational databases make it easier to extend the functionality of the software system.

In general, object-oriented databases make it easier to extend the functionality of a system. Object-oriented databases are designed to store objects, which are pieces of data that have attributes and methods. This makes it easy to add, remove, or change attributes and methods without affecting the rest of the data in the database.

## Overview - psql commands
### Adding constraints
Constraints are rules that restrict the data stored in a table. For example, a UNIQUE constraint ensures that all the values in a certain column are unique, while a NOT NULL constraint ensures that a certain column cannot have a null value. To add a constraint to a column, use the ALTER TABLE command with the ADD CONSTRAINT clause.

The syntax for this is given below:
```sql
ALTER TABLE 
  <table_name> 
ADD 
   CONSTRAINT <constraint_name> <constraint_type>(<column_name>);  
```
examples:

```sql
ALTER TABLE
  Customer
ADD
  CONSTRAINT customer_pk PRIMARY KEY (id); -- Adding PRIMARY KEY

ALTER TABLE
  Customer
ADD
  CONSTRAINT unique_email UNIQUE (email); -- Adding UNIQUE constraint

ALTER TABLE
  Customer
ALTER COLUMN
  id
SET
  NOT NULL; -- Adding NOT NULL constraint

ALTER TABLE 
  Customer 
ALTER COLUMN 
  dob 
SET 
  DEFAULT '2000-01-01'; -- Adding DEFAULT contstraint

ALTER TABLE
  Customer
ADD
  CONSTRAINT check_customer_id CHECK (id > 0); -- Adding CHECK constraint

ALTER TABLE
  Users
ADD
  CONSTRAINT user_customer_fk FOREIGN KEY (id) REFERENCES Customer (id); 
--- Adding FOREIGN KEY constraint

\d Customer 

SELECT '\n' AS " "; -- Adding new line

\d Users
```