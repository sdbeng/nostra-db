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