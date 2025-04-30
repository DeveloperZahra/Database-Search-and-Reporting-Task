# _*1.Comparison Assignment*_ 

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
 

