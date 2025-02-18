---
title: Database System
date: 2025-02-18 20:50:36 +0800
categories: [code, course]
tags: [ds]     # TAG names should always be lowercase
---

## Introduction

### DBMS

* Definition: Database(integrated and persistent)+A set of programs used to access, update and manage the data in database
* Properties: Efficiency, Scalability, Reduced, Independence, integrity, security, concurrent access并发访问 + robustness(recovery)
* History: File processing system, Network and hierarchical DBMS, Relational database system, Object-oriented DBMS, Object-relational DBMS, Application-oriented DBMS, Data Warehousing, Online Analytical Processing, Data Mining system
* vs File processing system: 
  * redundancy, inconsistency(No atomicity of updates:)
  * Difficulty in accessing data 
  * Data isolation, Integrity problems
  * Difficult to concurrent access by multiple users  
  * Security problems 

### Level of abstraction

* Levels:
  * Physical level: store
  * Logical level: relationships
  * View level: hide details
  * Logical data independence is harder to achieve than physical data independence
* Other:
  * Schema: structure of the database on different level  
  * Instance: actual content

### Data model

* Steps of Database Design
  * Requirement analysis
  * Conceptual database design
  * Logical database design
  * Schema refinement
  * Physical database design
  * Create and initialize the database & Security design
* E-R model：Entity Relationship（有ship） Model 

### Database Language

* DDL: data dictionary(contain metadata)
* DML: Insert, Delete, Update, Retrieve
* SQL=DDL+DML+DCL
* Two classes:
  * Procedure: how to get data
  * Nonprocedure: SQL

### DBA Database administrator 

### Transaction Management

* ACID properties: Atomicity, Consistency, Isolation, Durability
* Concurrency-control manager (并发控制管理器) 
* Transaction-management component ensures that the database remains in a consistent (correct) state 

### DBMS structure

* Storage manager: efficient storing, retrieving, updating data in the database.
  * Transaction manager, Authorization and integrity manger, File manager, Buffer manager
  
* Query processor: 
  * DDL interpreter, DML compiler, query processing 
  * Parsing and translation, Optimization, Evaluation
* Application Architectures
  * Three-tier architecture: E.g., web-based applications, and applications built using “middleware” (中间件)
![Desktop View](/assets/img/3-tier.png){: width="700" height="400" }
