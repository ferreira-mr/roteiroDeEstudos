# Livro: Database System Concepts - Silberschatz, Korth, Sudarshan

## Materiais do Livros

- [Slides](https://www.db-book.com/db7/slides-dir/index.html)
- [Solutions to Practice Exercises](https://www.db-book.com/db7/practice-exer-dir/index.html)
- [Online SQL interpreter](https://www.db-book.com/db7/university-lab-dir/sqljs.html)
- [DB Tips](https://www.db-book.com/db7/university-lab-dir/db-tips.html)
- [Lab Exercises and Sample Term Projects](https://www.db-book.com/db7/university-lab-dir/lab-exercises-projects.html)
- [Sample Table](https://www.db-book.com/db7/university-lab-dir/sample_tables-dir/index.html)

## Chapter 01 - Introduction

### Summary

- A database-management system (DBMS) consists of a collection of interrelated data and a collection of programs to access those data. The data describe one particular enterprise.
  
- The primary gola of a DBMS is to provide an environment that is bot convenient and efficient for people to use in retrieving and storing information.

- Database systems are ubiquitous today and most people interact, ether directly or indirectly,  with databases many time every day.

- Database systems are designed to store large bodies of information. The management of data evolves both the definition of structures of the storage of information and the provision of mechanisms for the manipulation of information. Tn addition, the database system must price for the safety go the information stored in the face of system crashes or attempts at unauthorized access. If data are to be shares among several users, the system must avoid possible anomalous results.

- A major purpose of a database system is to provide users with an abstract view to the data. That is,  the system gudes certain details if gig the data are stored and maintained.

- Underlying the structure of database is the data model: a collection of conceptual tools for describing data, data relationships, data semantics, and data constraints.

- The relation data model is the most widely deployed model for storing data in databases Other data models are the object-oriented mode, the object-relation model, and semi-structured data modes.

- A data-manipulation language (DML) is a language that enables users to access or manipulate data. Nonprocedural DMLs, which requires a user to specify only what data are needed without specifying exactly hoe to get those datam are widely used today.

- A data-definition language (DD): is a language for specking the database schema and other properties of the data.

- Database design mainly involves the design of the database schema . The entity relationship (E-R) data model is widely used model for database design. It provides a convenient graphical representation to view data, relationships, and constraint.
  
- A database system has several subsystems.
  - The stored manager subsystem provides the interface between the low-level data stored in the database and the application programs and queries submitted to the system.
- The query processor subsystem compels and executes DDL and DML statements.

- Transaction management ensures that the database remiss in a consistent (correct) state despite system failures. The transactions manager ensures that concurrent transaction excite proceed without conflicts.
  
- The architecture of datives system is greatly influence by the underlying computer system on which the data system runs. Database system can be centralizer, or parallel, involving multiple machines, Distributed databases span multiple geographically separated machines .

- Database applications are typically broken up into a front-end part that runs at client machines and a part that runs at the backend. In two-tier architectures, the front end directly communicates with a database running at the back end. In three-tier architectures, the back end part is itself broken up into an application server and a database server.

- There are four different types o database-system users, differentiated by the way they expect to interact with the system. Different types of user interfaces have been decided fo the different types of users.

- Data-analysis techniques attempt to automatically discover rules and pattern from data. The field of data mining combines knowledge-discovery techniques invented by artificial  intelligence researchers and statical analysts with efficient implementation techniques that enable them to be used on extremely large database.

### Review Terms

- Database-management system (DBMS)
- Database-system applications
- Online transaction proceeding
- Data analytics
- File-processing systems
- Data inconsistency
- Consistency constraints
- Data abstraction
  - Physical level
  - Logical level
  - View level
- Instance
- Schema
  - Physical schema
  - Logical schema
  - Subschema
- Physical data independence
- Data models
  - Entity-relationship model
  - Relational data model
  - Semi-Structured data model
  - Object-based data model
- Data base languages
- Data0definition language
- Data-manimupaltion languege
  - Procedura DML
  - Declarative DML
  - nonprocedural DML
- Query language
- Data-Definition language
- Domain Contrants
- Referential Integrity
- Authorization
  - Read authorization
  - Insert authorization
  - Update authorization
  - Delete authorization
- Metadata
- Application program
- Database design
  - Conceptual design
  - Normalization
  - Specification of function requirements
  - Physical-Design phase
- Database Engine
- Stored manager
  - Authorization and integrity manager
  - Transaction manager
  - File manager
  - Buffer manager
  - Data files
  - Data dictionary
  - Indices
- Query processor
  - DDL interpreter
  - DML compiles
  - Query optimization
  - Query evaluation engine
- Transaction
- Atomicity
- Consistency
- Durability
- Recovery manager
- Failure recovery
- Concurrency-control manager
- Database Architecture
  - Centralized
  - Parallel
  - Distributed
- Database Application Architecture
  - Two-tier
  - Three-tier
  - Application server
- Database administrator (DBA)

### Practice Exercises

1. This chapter has described several major advantages of a datable system. What are two disadvantages?
Two disadvantages associated with dater systems are listed below.
   - Setup of the dater system requires more knowledge,  money, skills, and time.
   - The complicit of the database may result in poor performance.

2. List five ways in which the type deception system of a language such as Java or C++differs from the data definition language used in a database.
   - Executing an action in the DDL result in the creation of an object in the database; in contrast, a programming langue type declaration is simp an abstraction used in the program.
   - Database DDLs allow consistent constraints to be specified, which programming langue type system generally do not allow. These include cramming language type systems generally do not allow. These include domain contrasts and referential integrity constraints.
   - Database DDLs support authorization, giving different access rights to different users. Programming langue type systems do not provide such protection (at best, the protest attributes in a class from being accessed by meths in another class).
   - Programming langue type systems are usually music richer than the SQL type system. Most databases support only basic types such as different types of number and string, although some databases do support some comply types such as arrays and objects.
   - A database DDL is focused on specifying types of attributes of relations; in contrast,  a programming langue allows objects and collection of objects to be create

3. List six major steps that you would take in setting up a database for a particular enterprise.
Six major step in setting up a datable for a particular enterprise are:
   1. Define the high-level requirements of the enterprise (this step generates a document known as the system requirements specification.)
   2. Define a model containing all appropriate types of data and data relation ships.
   3. Define the integrity constraints on the data.
   4. Define the physical level.
   5. For each know problem to be solved on a regular basis (e. g., tasks to be carried out by clerks or web users), define a user interface to carry out the task, and write the necessary application programs to impute the user interface.
        - Create/initialize the database.

4. Supposes you want to build a video similar to YouTube. Consider each of the point listed in Section 1.2 as disadvantages of keep data in file-professing system. Discuss the relevance of each of theses points to the stores of actual vide data, and to metadata about the video, such as tiles, the user who upload it, tags, and which users viewed it.
    - **Data redundancy and inconsistent**. This would be revenant to metadata to some extent, although no to the actual video data, which are not updated. There are vey relationships here, and none of them can lead to redundancy.
    - **Difficulty in accessing data**. If video data are only accessed though a few predefine interface, as is done in video sharing sites today, this will noved be a problem. However, if an organization needs to find video data based on specific sear condition (beyond simple keyword queries), if metadata were store in files it would be hard to find revelation data with writing application programs. Using a database would be important for the task of find data.
    - **Data isolation**. Since data are not usually updated, but instead newly created data isolation is no a major issue, Even the task of keeping track of who has viewed what vides is (conceptually) append only agin making isolation not a major issues of concurrent updates to authorization information.
    - **Integrity problems**. It seems unlikely there are significant integrity constraints in this application, except for primary keys. If the data are distributed, there may be issues in enforcing primary key constraints. Integrity problems are probably not a major issue
    - **Atomicity problems.** When a video is uploaded, metadata about the video and the video should be added atomically, otherwise there would be an inconsistency in the data. An underlying recovery mechanism would be required to ensure atomic in the event of failures.
    - **Concurrent-access anomalies.** Since data are updated, concurrent access anomalies would be unlikely to occur.
    - **Security problems.** These would  be an issue if the system supported authorization.
5. Keyword queries used in dev search are quite different  from databases queries. List key differences between the two, in therms of the way the queries are specified and in term of what is the result of a query.
    Queries used in the web are specified by providing a list of keyword with no specific syntax. The result is typically an ordered list of URLs, along with snippets of information about he content of the URLs. IN contrast, data base queries have a specific syntax allowing compels queries to be specified. And in the relation world the result of a  query is always a table.

### Exercises

1. List four application you have used that most Kiel employed a database system to tore persistent data.
2. List four applications you have used that most likely employed a database system to store persistent data.
3. Explain the concept oh physical data independence and its importance in database systems.
4. List five responsibilities of a database-management system. For each responsibility, explain the problems that would arise if the responsibility were not discharged.
5. List at lest two reason why database systems support data manipulation using a declarative query language such as SQL, instead of just providing a library of C or C++ function to carry out data manipulation.
6. Assume that two students at trying to reciter for a course in which there is only one open seat. What component of a datable system prevents both student from being give that last seat?
7. Explain the difference between two-tier and three-tier application architectures. Which is better suited for web applications? Why?
8. List two features develop in the 2000s and that help database system handle data-analytics workloads.
9. Explain why NoSQL systems emerged in the 2000s, and briefly contrast thesis features with traditional database systems.
10. Describe at least three table that might be used to stores information in a social-networking system such as Facebook.

## Chapter 02 - Introduction to The  Relational Model

### Summary

- The relational data model is based on a collection of tables. The user of the database system may query these tables, inset new types, delete tuples, and update (modify) tuples. There are several languages for expressing these operation.
- The schema of a relation refers to its logical design, while an instance of the relation refer to its content at a point in time. The schema of a database and an instance of dative are similarly defined. The schema of a relation includes its attributes, and optionally the types of the attributes and constraints on the relation such as primary and foreign-key constraints.
- A superkey of a relation is a set one or more attributes whose values are guaranteed to identify tuples in the relation uniquely. A candidate key is a minimal superbly, that is, a set of attributes that forms a super key, but none of whose subsets is a superkey. One of the candidate key of a relation is chosen as its primary key.
- A foreign-key from attribute(s) A of relation r1 is the primary-key B of relation r2 states that the value of A for each tuple in r1 must also be the value of B for some tuple in r2. The relation r1 is called the referencing relation, and r1 is called the refined relation.
- A schema diagram is a pictorial depiction of the schema of a database that shown the ration in the database, their attributes, and primary keys and foreign keys.
- The relation query languages define a set of operation that operate on tables and output tables as their results. These operations can be combined to get expressions that express seared queries.
- The relation algebra proceeds a set of operation that take one or more relation as input and return a relation as an output. Pratic query languages such SQL are based on the relational algebra, but they add a number of useful syntactic features.
- The relation algebra defines a set of algebraic operations that operate on tables, and output tables as their result. These operations can be combined to get expression that express serried queries. The algebra defines the basic operations used within relation query languages like SQL.

### Review Terms

- Table
- Relation
- Tuple
- Attribute
- Relation instance
- Domain
- Atomic domain
- Null value
- Database schema
- Database instance
- Relation schema
- Keys
  - Superkey
  - Candidate key
  - Primary key
  - Primary key constrains
- Foreign-key constraint
  - Referencing relation
  - Referenced relation
- Referencial integrity constraint
- Schema diagram
- Query language types
  - Imperative
  - Funcional
  - Declarative
- Relation algebra
- Relational-algebra expression
- Relational-algebra operations
  - Select **σ**
  - Project  **π**
  - Cartesian product **⨯**
  - Join **⨝**
  - Union **∪**
  - Set diference **-**
  - Set intersection **∩**
  - Assignment **=**
  - Rename **ρ**

```figure 2.17
employee (person_name, street, city)
works (person_name, company_name, salary)
company (company_name, city)
```

[relational algebra calculator](https://dbis-uibk.github.io/relax/calc.htm#)

### Practice Exercises

1. Consider the employee database of Figure 2.17. What are the appropriate primary keys?
The appropriate primary key shown below:

```sql
employee ( ~person_name~, street, city)
works ( ~person_name~, company_name, salary)
company ( ~company_name~, city)
```

2. Consider the foreign-key constraint from the *dept_name* attribute of *instructor* to the*department* relation. Give examples of inserts and deletes to these relation that can cause aviolation of the foreign-key constraint.

- Inserting a tuple: (1011, Ostrom, Economics, 110000)
- Deleting the tuple: (Biology, Watson, 90000)

3. Consider the *time-slot* relation. Given that a particular time slot can meet more than once ina week, explain why *day* and *start_time* are part of the primary key of this relation, while*end_time* is not.

   > The attributes *day* and *start_time* are part of the primary key since a particular call will most likely meed on several deferents days and may even meet more than on in a day. However, end_time is not part of the prime key since a particular class that start at a particular time on a particular day cannot end at more than one time.

4. In the instance of instructor shown in Figure 2.1, no two instructors have the same name. From this, can we conclude that *name* can be used as a super key? (Or primary key) of *instructor*?

    > No. For this possible instance of the instructor table the names are unique, but in general this may no always be the case (unless the universes has a rule that  two instructors cannot have the same name, which is a rather unlikely scenario.

5. What is the sets of first performing the Cartesian product of *student* and *advisor*, and then performing a selection operation on the result with the predicative *s_id = ID* (Using the symbolic notation of relation algebra, this query can be written as `σ s_id = ID (student ⨯ advisor)`

    > The result attributes include all attribute values of *student* followed by all attributes of *advisor*. The tuples in the result are as follows: For each student who has an advisor, the result has a row containing that student’s attributes, followed b as *s_id* attribute identical to the students advisor. Students who do not have an advisor will not appear in the result. Student who has more than one advisor will appertains a correspoinid number of times in the result.

6. Consider the employee database of Figure 2.17. Give an expression in the relation algebra to express each of the following queries:
    1. Find the name of each employee who lives in city “Miami”
    2. Find the name of each employee whose salary is greater than \$100000.
    3. Find the name of each employee who lives in “Miami”and whose salary is greater than \$100000.

```Figure 2.18
branch(banch_name, branch_city, assets)
customer(ID, customer_name, customer_street, custumer_city)
loan(loan_number, banch_name, amout)
borrower(ID. loan_number)
account(account_number, branch_name, balance)
deposito(ID, accounta_number)
```

7. Consider the bank data base of Figure 2.18. Give an expression in the relation algebra for each of the following queries:
    1. Find the name of each branch located in “Chicago”.
    2. Find the ID of each borrower this has a loan in branch “Downtown”

8. Consider the employee database of Figure 2.17. Give an expression in the relation algebra to express each of the following queries:
    1. Find the ID and name of each employee who does not work for “BIgBank”.
    2. Find the ID and name of each employee who earns at leat as much as every employee in the database.

9. The **division operator** of relation algebra, ÷, is defined as fallows, Let r(R) and s(S) be relations, and let S contido em R; that is, every attribute of schema S is also in schema R. Given  a tuple t, let t(S) denote te projection of tuple t on the attributes in S. Then r dividido por s is a relation on schedule R - S (that is, on the schema contacting all atributes of schema R that are not in schema S).  A tuple t is r / Sid and only both of the condition hold:~~

### Exercises

10. Describe the differences in meaning between the terms *relation* and *relation schema*.

11. Consider the *advisor* relation shown in the schema diagram in Figure 2.9 with `s_id` as the primary key of *advisor*. Suppose a student can have more than one advisor. Them would `s_id` still be a primary key of the *advisor* relation? If not what should the primary key of *adviser* be?

12. Consider the bank database of Figure 2.18. Assume the branch names and customer namer uniquely identify branches and customers, but loans and accounts can be associated with more than one customer.
    1. What are the appropriate primary keys?
    2. Given your choice of primary keys, identify appropriate foreign keys.

13. Construct a schema diagram for the bank database of Figure 2.18

14. Consider the employee database of Figure 2.17. Give an expression in the relational algebra to express each of following queries:
    1. Find the ID and name of each employee who works for “BigBank”.
    2. Find the ID, name and city of residence of each employee who works for “BigBank”
    3. Find the ID, name, street address, and city of residence of each employee who works for “BigBank” and earns more than $10000.
    4. Find the ID and name of each employee in this database who live in. The same cit as the company for which she or he works.

15. Consider the bank database of Figure 2.18. I’ve an expression in the relation algebra for each of the following queries:
    1. Find each loan number with a loan amount greater than $10000.
    2. Find ID of each deposit who has an account with a balance greater than $6000.
    3. Find the ID of each deposit who has an account with a balance greater than $6000 at the “Uptown” branch".

16. List two reason why null values might be introduce into a database.

17. Discuss the relative merits of imperative, functional, and decorative languages.

18. Write the flowing queries in relation algebra, using the university schema.
    1. Find the ID and name of each instructor in the Physics department.
    2. Find the ID and name of each instructor in a department located in the building “Watson”.
    3. Find the ID and name of each student who has taken at least one course in the “Comp. Sci.” Department.
    4. Find the ID and name of each student who has taken at least one cause section in the year 2018.
    5. Find the ID and name of each student who has not take any cause section n the year 2018.

### Review Terms

- Database-management system (DBMS),
- Data model
- Data-maniputaliton-language (DML)
- Data-definition-language (DDL)
- Storage manager
- Query processor
- Transaction management
- Data mining
- Database-system applications
- File-processing systems
- Data inconsistency
- Consistency contraints
- Data abstraction
- Instance
- Schema
  - Phisycal schema
  - Logical schema
- Physical data independence
- Data models
  - Entity-relationship model
  - Relational data model
  - Object-based data model
  - Semistructured data model
- Database languages
  - Data-definition language (DDL)
  - Data-manipulation language (DML)
  - Query language
- Metadata
- Application program
- Normalization
- Data dictionary
- Storage manager
- Query processor
- Transactions
  - Atomicity
  - Failure recovery
  - Concurrency control
- Two-and three-tier database architectures
- Data mining
- Database administrator (DBA)

## Chapter 03 - Introduction to SQL

### Summary

- SQL is the most influential commercially marketed relational query language. The SQL language has several part:
- **Data-definition language (DDL)**, which provides commands for defining relation schemas, deleting relations, and modifying relation schemas.
- **Data-manipulation language (DML)**, which includes a query language and commands to inset tuples into, deletes tuples from, and modify tuples in the database.
- The SQL data-definition language is used to creat relations with specified schemas. In addition to specifying the names and types of relation attributes, SQL also allows the specification of integrity constraints such as primary-key constraints and foreign-key constraints.
- SQL includes a variety of language contracts for queries on the database. These includes the **SELECT**, **FROM**, and **WHERE** clauses, and support fo the natural join operation.
- SQL supports basic set operation on relations including **UNION**, **INTERSECT**, and **EXEPT**, which correspond to the mathematic set-theory operation.
- SQL Hades queries on relation containing null values by adding the truth value “unknown”to the usual truth values of true and false.
- SQL supports aggregation, including the ability to divide a relation into groups, applying aggregation separately on each group. SQL also supports set operation on groups.
- SQL supports nested subqueries in the **WHERE**, and **FROM** clauses of an outer query. It also supports scalar subqueries ,wherever an expression returning a values is permitted.
- SQL provides contracts for **UPDATE**, **INSERT** and **DELET** information.

### Reviews Terms

- Data-definition language
- Data-manipulation language
- Database schema
- Database instance
- Relation schema
- Relation instance
- Primary key
- Foreign key
  - Referencing relation
  - Referenced relation
- Null value
- Query language
- SQL query structure
  - **SELECT** clause
  - **FROM** clause
  - **WHERE** clause
- Natural join operation
- **AS** clause
- **ORDER BY** clause
- Correlation name (correlation variable, tuple variable)
- Set operations
  - **UNION**
  - **INTERSEPT**
  - **EXEPT**
- Null values
  - Truth value “unknown”
- Agregate functions
  - **AVG**, **MIN**, **MAX**, **SUN**, **COUNT**
  - **GROUP BY**
  - **HAVING**
- Nested subqueries
- Set comparison
  - {<,  <=, >, >=}  {**some**, **all**}
  - **EXISTS**
  - **UNIQUE**
- **LATERAL** clause
- **WHIT** clause
- Scalar subquery
- Database modification
  - **DELETE**
  - **INSERT**
  - **UPDATE**