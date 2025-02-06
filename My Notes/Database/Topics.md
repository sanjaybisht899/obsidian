---

---

---


Concurrency Control

- Locking Mechanisms (Pessimistic and Optimistic Locking)
- Deadlock and its prevention
- Transaction Isolation and Lock Granularity

Database Backup and Recovery

- Backup Types (Full, Incremental, Differential)
- Point-in-Time Recovery
- Strategies for Database Recovery

---

- Types of NoSQL Databases
- Document-based (MongoDB, CouchDB)
- Key-Value Stores (Redis, DynamoDB)
- Column-family Stores (Cassandra, HBase)
- Graph Databases (Neo4j, ArangoDB)
- Use Cases and Advantages of NoSQL
- Horizontal Scalability
- Schema Flexibility
- CAP Theorem (Consistency, Availability, Partition Tolerance)
- Basic Operations in NoSQL
- CRUD operations
- Querying and Indexing in NoSQL

---


Distributed Databases and Architectures

- Sharding and Partitioning
- Horizontal and Vertical Partitioning
- Sharding Strategies (Range-based, Hash-based)
- Replication
- Master-Slave, Master-Master Replication
- Synchronous vs Asynchronous Replication
- Distributed Transactions
- Two-Phase Commit Protocol (2PC)
- Distributed Locking and Concurrency Control
---
Performance Optimization

- Query Optimization
- Execution Plans and Analyzing Performance
- Indexing for Performance Improvement
- Query Caching
- Database Tuning
- Buffer Pool and Memory Configuration
- Database Configuration Parameters
- Hardware Optimizations (Disk, CPU, RAM)
- Database Partitioning
- Horizontal and Vertical Partitioning
- Range, List, Hash, and Composite Partitioning
---
Data Security and Integrity

- Database Security
- Authentication and Authorization
- Role-based Access Control (RBAC)
- Encryption (Data-at-rest, Data-in-transit)
- Data Integrity
- Integrity Constraints (Entity Integrity, Referential Integrity)
- CHECK constraints, NOT NULL, UNIQUE, PRIMARY KEY, and FOREIGN KEY
---
Cloud Databases

- Cloud Database Concepts
- Database as a Service (DBaaS)
- AWS RDS, Google Cloud SQL, Azure SQL Database
- Advantages and Limitations of Cloud Databases
- Scaling Cloud Databases
- Vertical and Horizontal Scaling
- Autoscaling

---
Data Warehousing and ETL


- Data Warehousing Concepts
- Data Warehousing Architecture
- OLAP vs OLTP
- Star Schema, Snowflake Schema, Fact Tables, and Dimension Tables
- ETL Process
- Extract, Transform, Load Concepts
- ETL Tools (Talend, Apache Nifi, Informatica)
- Data Pipeline Architecture

---
Database Tools and Technologies

- Database Management Tools
- MySQL Workbench, pgAdmin, MongoDB Compass
- Query Optimization and Profiling Tools
- Database Migration
- Database Migration Strategies
- Tools for Database Migration (Flyway, Liquibase)

---

New Trends and Technologies

- Big Data Technologies
- Hadoop, Spark, and their integration with databases
- Data Lakes
- In-Memory Databases
- Redis, Memcached
- Use Cases for In-Memory Databases
- Blockchain Databases
- Concepts of Blockchain in DBMS
- Use of Blockchain in Database Integrity

---
Interview Specific Topics

- Real-World Database Scenarios
- Design a database for a given use case
- Optimize a slow-running query
- Solve common database design issues (like missing indexes, normalization/denormalization)
- Troubleshooting and Debugging
- Handling deadlocks and performance bottlenecks
- Diagnosing and resolving data inconsistencies

---
Interview-Specific Topics - Deep

#### 1. Real-World Database Scenarios

- Database Design for Specific Use Cases

- Designing a database for an E-commerce application (products, users, orders, payments, etc.)
- Designing a Social Media platform database (posts, comments, likes, followers)
- Designing a Banking system (accounts, transactions, users, loans, deposits)
- Designing a Library Management System (books, users, borrow history, fines)
- Designing a University Management System (students, courses, professors, grades)
- Designing a Hospital Management System (patients, doctors, appointments, medical records)

- Normalization and Denormalization
- Normalizing a database to eliminate redundancy and achieve 3NF
- When to denormalize for performance reasons, such as in reporting or OLAP systems
- Handling Many-to-Many Relationships
- Designing junction tables and ensuring referential integrity
- Managing large amounts of data in many-to-many relationships
- Database Model Conversion

- Converting an ER Diagram to a relational schema
- Mapping NoSQL data models (document-based, key-value stores) to relational schemas

# Optimize a Slow-Running Query
- Identifying Bottlenecks in Queries

- Analyzing Query Execution Plans to find slow steps (full table scans, joins without indexes, etc.)
- Checking Indexes: Are the right indexes being used? Should composite indexes be created?
- Optimizing joins: Converting subqueries to joins, avoiding N+1 queries.
- Reducing the size of the result set: Using proper filtering with WHERE, limiting GROUP BY clauses.
- Index Optimization

- Creating the right indexes for frequently used query patterns (e.g., composite indexes)
- Covering Indexes that can fulfill the query without accessing the table
- Use of Partial Indexes for selective indexing (index only the rows that meet certain conditions)

- Query Refactoring

- SELECT * → SELECT specific columns: Avoiding unnecessary data retrieval
- Use of LIMIT and OFFSET for pagination to reduce the number of rows processed
- Using EXPLAIN to debug queries and improve their execution time

- Caching Strategies

- Using materialized views for complex aggregation queries
- Implementing query caching or result caching for frequently executed queries

- Partitioning and Sharding

- Splitting a large table into smaller partitions to improve performance (range, list, or hash partitioning)
- Horizontal Sharding to distribute data across multiple databases

#### Troubleshooting and Debugging

- Handling Deadlocks

- Identifying and resolving deadlocks by analyzing the deadlock graph and transaction logs
- Implementing deadlock prevention strategies, such as:

- Ensuring consistent lock ordering
- Using lower isolation levels (e.g., Read Committed) when appropriate
- Retrying failed transactions after a deadlock
- Performance Bottlenecks

- Disk I/O bottlenecks: Checking slow disk access and optimizing queries or indexing strategies
- CPU bottlenecks: Identifying queries that use excessive CPU resources and optimizing them
- Memory bottlenecks: Checking for excessive memory usage by queries or the database engine, and optimizing memory configuration (buffer cache, query cache)
- Slow Response Times

- Diagnosing issues in database connection pooling and improving connection reuse
- Lock contention: Checking for blocking queries and resolving lock contention issues
- Query execution time analysis and identifying missing indexes
- Database Connection Issues

- Resolving issues related to connection pooling: Ensuring optimal use of database connections in applications
- Debugging timeouts and network issues between the application and the database server
- Diagnosing and Resolving Data Inconsistencies

- Data Integrity Violations: Checking for missing or inconsistent foreign key references, duplicated entries
- Fixing orphaned records (e.g., child records with no corresponding parent record)
- Data corruption: Checking and repairing corrupted tables (e.g., using REPAIR TABLE in MySQL)
- Database Migration Problems

- Handling data type mismatches during migration (e.g., string to date conversions)
- Managing data loss and ensuring data consistency during migrations
- Automating schema migrations (e.g., using tools like Flyway, Liquibase)

---
Design a database

1. *Define the Problem Space:* -

Understand problem and define scope.

Clarify functional and non-functional requirements.

State assumptions and decisions explicitly.

2. *Design the System at a High Level:* -

Design APIs to define how clients access system resources.

Consider request parameters, response types, and communication between client and server.

Create a high-level design diagram to illustrate system architecture.

1. *Deep Dive into the Design:*

Examine system components and relationships in detail.

Consider non-functional requirements' impact on design choices.

Present different design options with pros and cons.

2. *Identify Bottlenecks and Scaling Opportunities:* -

Assess system's ability to operate under various conditions and support growth.

Address single points of failure, data replication, global service support, and scalability.

Consider concepts like horizontal sharding, CDN, caching, rate limiting, and databases.

 *Review and Wrap Up:*

Summarize major decisions with justifications and trade-offs.

Ensure design satisfies all requirements.

Identify directions for further improvement.
---
others

oracle db and mysql  same or different
cursor in mysql
what is normalization and denormalization
what is acid properties 
left join
right join
innter join
outer join