﻿# _*1.Comparison Assignment*_ 

**_Flat File Systems vs. Relational Databases_**

| Feature              | Flat File Systems                                | Relational Databases                             |
|----------------------|---------------------------------------------------|--------------------------------------------------|
| **Structure**         | Data is stored in plain text or CSV files, with each file typically representing a single table. | Data is stored in structured tables with defined schemas (rows and columns). Tables can be linked. |
| **Data Redundancy**   | High – same data often needs to be duplicated across multiple files. | Low – data is normalized and redundancy is minimized through relationships. |
| **Relationships**     | No direct support – data linking must be manually handled, which can be error-prone. | Supports relationships through foreign keys and joins between tables. |
| **Example Usage**     | Simple contact lists, CSV exports, log files, flat configuration files. | Enterprise applications, inventory systems, customer relationship management (CRM) systems. |
| **Drawbacks**         | - Not scalable<br>- Difficult to manage relationships<br>- Higher risk of inconsistency<br>- Poor performance with large data | - More complex to set up and maintain<br>- Requires a database management system (DBMS)<br>- Overhead for small/simple tasks |


# *__2. DBMS Advantages Mind Map__*

![Tux, the Linux mascot](./images/DBMS_Advantages_Mind_Map.png)


# *__3. Roles in a Database System__*

*__1. System Analyst__*

**Role:**

A System Analyst acts as a bridge between business needs and technical solutions. They gather requirements from stakeholders, analyze workflows, and design system specifications.

Key Responsibilities:

* Gather and analyze business requirements

* Propose system solutions

* Create functional specifications

* Coordinate with developers and stakeholders
* 

*__2. Database Designer__*

**Role:**

A Database Designer is responsible for structuring the database. They design how data will be stored, related, and accessed efficiently.

Key Responsibilities:

* Design data models and ER diagrams

* Define tables, relationships, keys (primary/foreign)

* Ensure normalization to reduce redundancy

* Work closely with developers and DBAs

*__3. Database Developer__*

**Role:**

A Database Developer builds and maintains the database structures and writes the logic that allows applications to interact with the database.

Key Responsibilities:

* Create and optimize SQL queries, stored procedures, and functions

* Build triggers and indexes

* Support application development by providing efficient data access

* Ensure database performance and integrity


*__4. DBA (Database Administrator)__*

**Role:**

The DBA manages and maintains the database environment to ensure it is secure, reliable, and performing optimally.

Key Responsibilities:

* Install, configure, and upgrade database software

* Monitor performance and optimize resources

* Manage backups, recovery, and security

* Handle user permissions and data integrity


*__5. Application Developer__*

**Role:**

An Application Developer designs and builds applications that interact with the database and deliver services to end users.

Key Responsibilities:

* Develop front-end and back-end application logic

* Use APIs or SQL to interact with databases

* Implement business logic in software

* Ensure data is properly displayed and used in apps


*__6. BI (Business Intelligence) Developer__*

**Role:**

A BI Developer transforms raw data into meaningful insights using data analysis, visualization tools, and reporting systems.

Key Responsibilities:

* Create dashboards and reports using BI tools (e.g., Power BI, Tableau)

* Write queries and extract data from databases or data warehouses

* Analyze data trends and patterns for decision-making

* Support business teams with actionable intelligence
 
 -------------------------------------------------------------
 # *_Additional Research Topics to Include in the Report_*

<ins>  __*(1) Types of Databases*__ </ins>

   🔹 Relational vs Non-Relational Databases:

|          |Relational  Databases | Non-Relational Databases|
|----------|----------------------|-------------------------|        
|Structure|Use tables with rows and columns|Document, key-value, column-family, or graph-based|
|Features|Data is related through keys (primary/foreign)|More flexible schema; doesn’t require fixed tables|
|Examples|MySQL, PostgreSQL, Oracle|MongoDB (document), Cassandra (column-family), Redis (key-value)|
|Best For| Structured data with clear relationships.|Unstructured or semi-structured data, scalability|
|Use Case| An online banking system where customer info, transactions, and account details must be related and queried reliably |A social media platform storing user-generated content like posts, images, likes, and comments using MongoDB for fast access and flexible formats|

-----------------------------------------------------

🔹 Centralized vs Distributed vs Cloud Databases:

|           |Centralized Database | Distributed Databases | Cloud Databases|
|-----------|---------------------|-------------|----------------|
|           |All data stored in one location/server | Data is spread across multiple locations/nodes|Hosted on cloud platforms (AWS, Azure, Google Cloud)|
|           |Easier to manage but may be a single point of failure|Offers better reliability and availability|Offers scalability, high availability, and low maintenance|
|           |Example: Small company ERP system on one server| Examples: Google Spanner, Apache Cassandra| Examples: Amazon RDS, Firebase, Google Cloud Spanner|
|           | Use Case:A university's internal system managing student records on a single on-premise server |Use Case:A global e-commerce platform using a distributed system like Cassandra to keep inventory data synced across continents|Use Case:A mobile app backend (e.g., a ride-sharing app) using Firebase for real-time user data and location tracking|

----------------------------------------------------------
<ins>  __*(2) Cloud Storage and Databases*__ </ins>

🔹 What is Cloud Storage?

**Definition:**  Cloud storage is a service that allows data to be stored on remote servers accessed via the internet.

**Examples:**  Google Drive, Amazon S3, Dropbox.

🔹 How Does Cloud Storage Relate to Databases?

     * Cloud storage is used to hold files, backups, media, and unstructured data.

     * Cloud databases, on the other hand, are database services hosted in the cloud that store structured or semi-structured data and allow querying, analytics, and transactions.

* Often, both work together:

      * Cloud storage = saves raw data (e.g., logs, backups).

      * Cloud database = manages structured data (e.g., customer records, product info).

🔹 Advantages & Disadvantages of Cloud-Based Databases:

|     | Advantages of Cloud-Based Databases | Disadvantagesof Cloud-Based Databases|
|-----|--------------------------------|---------------------------------------|
| 1   | **Scalability:**   * Easy to scale up or down based on traffic.  *Example: Auto-scaling with Amazon RDS. |**Dependence on Internet:** You need stable internet access to use the service|
| 2    |**Availability & Reliability:** Redundant servers across data centers mean higher uptime | **Data Security & Privacy:** *Sensitive data stored off-site may raise concerns.*Requires strong encryption and compliance|
| 3    |**Lower Maintenance:** No need to manage hardware, backups, or software updates—handled by the provider | **Limited Control:** Less access to the underlying infrastructure compared to on-premises databases|
| 4    |**Accessibility:** Can be accessed from anywhere with an internet connection | **Cost Over Time:** Long-term usage costs may rise, especially with high traffic or storage needs|
| 5    | **Cost Efficiency:** Pay-as-you-go pricing; no upfront infrastructure investment|                                      |

 **_Example Services:_** 

* Azure SQL Database: Cloud version of Microsoft SQL Server.

* Amazon RDS (Relational Database Service): Supports MySQL, PostgreSQL, Oracle, etc.

* Google Cloud Spanner: Globally distributed, horizontally scalable relational DB.
-----------------------------------------------------------------------------------
   
   <ins>  __*(3) Database Engines and Languages*__ </ins>

   🔹 What is a Database Engine?

A Database Engine is the core software component that:

* Stores, retrieves, modifies, and manages data in a database.

* Handles the execution of SQL queries, transactions, indexing, and data integrity.

* Acts as the "brain" of the database system—it processes all commands and manages access to the underlying data files.

🔹 Key Functions of a Database Engine:

1. **Query Processing:**  Parses and executes SQL statements.

2. **Transaction Management:**  Ensures data consistency through ACID (Atomicity, Consistency, Isolation, Durability) properties.

3. **Indexing:** Improves the speed of data retrieval.

4. **Storage Management:** Manages how data is physically stored on disk.

5. **Concurrency Control:** Manages access when multiple users interact with the database at the same time.

🔹 Examples of Database Engines:

* **InnoDB** – Default engine for MySQL (supports transactions).

* **MyISAM** – Older MySQL engine (faster reads, no transaction support).

* **SQL Server Engine** – Used by Microsoft SQL Server.

* **PostgreSQL Engine** – Built-in advanced engine for PostgreSQL.

*  **WiredTiger** – Default engine for MongoDB.

🔹 Examples: SQL Server, MySQL, Oracle, PostgreSQL

1.**SQL Server**

* Developer: Microsoft

* Type: Relational Database(RDBMS)

* Engine: SQL Server Database Engine

* Platform: Windows and Linux

* Best For: Enterprise applications, especially in Microsoft ecosystems.

* Use Case Example:
A hospital management system using Microsoft SQL Server to manage patient records, appointments, and billing securely and reliably.

 2. **MySQL**

  * Developer: Oracle Corporation

* Type: Open - source RDBMS

* Engines: InnoDB(default), MyISAM(legacy)

* Platform: Cross - platform

* Best For: Web applications, LAMP stack(Linux, Apache, MySQL, PHP / Python)

*  Use Case Example:
            A blogging platform like WordPress uses MySQL to store posts, comments, and user data.

 3. **Oracle Database**

* Developer: Oracle Corporation

* Type: High - performance RDBMS

* Engine: Oracle DB Engine(proprietary)

* Platform: Cross - platform, mainly used in large - scale systems

* Best For: Large enterprises, financial institutions, mission - critical applications.

* Use Case Example:
            A banking system using Oracle Database to manage millions of daily transactions, ensuring data integrity and performance.

4. **PostgreSQL**

* Developer: Open - source community

* Type: Object - Relational Database(advanced RDBMS)

* Engine: PostgreSQL Engine

* Platform: Cross - platform

* Best For: Applications requiring complex queries, data types, and performance tuning.

* Use Case Example:
            A geographic information system(GIS) using PostgreSQL with PostGIS to manage spatial and location data.


🔹 What languages do they use? 

Each database engine uses a variation or extension of SQL (Structured Query Language). Here are some common examples:

|Database Engine |	Language Used|
|----------------|---------------|
|SQL Server   |	T-SQL (Transact-SQL)|
|Oracle	       |  PL/SQL (Procedural SQL)|
|MySQL      |	ANSI SQL + MySQL-specific syntax |
|PostgreSQL   |	ANSI SQL + PL/pgSQL |


ANSI SQL is the standard version of SQL that most engines support.

Engines extend ANSI SQL with their own features for more functionality.



🔹 Is there a relationship between the engine and the language? 

 Yes. Each engine uses a specific dialect or variation of SQL that is tailored to its features.
 While the base SQL commands (like SELECT, INSERT, UPDATE, DELETE) are similar across engines, the procedural features, error handling, and built-in functions often vary.




 🔹 Can One Language Work Across Different Engines?

Partially. Basic SQL (ANSI SQL) works across most database engines, so simple queries can often be reused.
However, more advanced scripts or stored procedures written in T-SQL or PL/SQL are usually not compatible with other engines without modification.

* For example:

A stored procedure written in T-SQL for SQL Server won’t run on Oracle without being rewritten in PL/SQL.

----------------------------------------------------------
<ins>  __*(4) Can We Transfer a Database Between Engines?*__ </ins>

🔹  is it possible to migrate a database from SQL Server to MySQL, or Oracle to PostgreSQL?

Yes, it is possible to migrate a database from SQL Server to MySQL, or from Oracle to PostgreSQL, but it requires a well-planned process due to differences between the database engines.

* Examples of Possible Migrations:

SQL Server → MySQL: You can use tools like MySQL Workbench Migration Wizard or SQL Server Migration Assistant (SSMA).

Oracle → PostgreSQL: Tools like Ora2Pg and AWS Schema Conversion Tool can help.

🔹  What are the challenges of engine-to-engine migration?

Migrating a database from one engine to another (like SQL Server to MySQL, or Oracle to PostgreSQL)
comes with several technical and practical challenges. Here are the main ones:


1. Data Type Mismatches: Different databases have varying data types.
2. Stored Procedures and Functions: SQL Server's T-SQL and Oracle's PL/SQL have unique syntax and features.
3. Triggers and Constraints: Triggers and constraints may behave differently across engines.
4. Performance Optimization: Indexing strategies and query optimization techniques vary between engines.
5. Application Compatibility: Applications often contain hard-coded SQL queries tailored to a specific database engine. 

🔹 What should we consider before transferring (data types, triggers, stored procedures, etc.)?

Before transferring a database between engines (like SQL Server to MySQL or Oracle to PostgreSQL), 
there are several critical aspects to consider to ensure a smooth and reliable migration:

1.  Data Types Compatibility
Different engines use different data types, and they don't always match one-to-one
 
 2.  Table Structures and Constraints
  
* Review primary keys, foreign keys, unique constraints, and default values. 
* Some databases handle constraints and defaults differently.

* Make sure to preserve data integrity rules in the new engine.

3. Stored Procedures and Functions
Each engine uses its own procedural language (e.g., T-SQL, PL/SQL, PL/pgSQL).

These can't be copied directly—you must translate and rewrite them.

Also review:

* Variable declarations

* Control flow (IF, LOOP, CASE)

* Error handling

4. Views
Check for engine-specific SQL in views (e.g., functions, joins, or syntax).

Modify as needed to match the SQL dialect of the target engine.

5. Application Compatibility
Update application code to reflect changes in:

* Connection strings

* SQL syntax

* Error handling

* Retest all application features that rely on the database.

6. Testing and Validation
Do comprehensive data validation, unit testing, and integration testing.

Confirm:

* No data was lost or changed

* Business logic works correctly

* Performance is acceptable

----------------------------------------------------------------------------
<ins>  __*(5) Logical vs. Physical Schema*__ </ins>

 🔹 What is the Logical Schema?

A Logical Schema represents the abstract design of the database. It focuses on:

* Entities (e.g., Student, Course)

* Attributes (e.g., student_name, date_of_birth)

* Relationships (e.g., a student enrolls in courses)

* Rules (like data types, constraints)

It does not include details about how data is stored physically—just the structure and relationships.

 🔹 What is the Physical Schema?

A Physical Schema is the implementation of the logical schema in a specific database system. It includes:

* Actual table names

* Column definitions with specific data types (e.g., VARCHAR(100))

* Indexes

* Storage details (e.g., partitions, tablespaces)

* Performance tuning features

It’s how the database is actually built on disk.


🔹 Difference Between Logical and Physical Schema

|Feature	|  Logical Schema	|Physical Schema|
|-----------|-----------------|-----------------|
|Level of Abstraction	| High-level (conceptual)	|Low-level (implementation)|
|Focus |	What data is stored and relationships|	How data is stored|
|Independence	|Independent of DBMS	|DBMS-specific|
|Includes|	Entities, attributes, relationships|	Tables, columns, indexes, data types|
Example| 	Entity: Student, Attribute: Name |	Table: student, Column: name VARCHAR(100)|