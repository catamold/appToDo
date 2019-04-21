---
title: Database
parent: Final Assignment
has_children: true
nav_order: 1
---

## Database
A series of concepts and statements were used in order to design the database attributes following ACID properties, so that a transaction has to follow 4 rules.
> **Atomicity:** All changes to data are performed as if they are a single operation. That is, all the changes are performed, or none of them are.
> 
> **Consistency:** Data is in a consistent state when a transaction starts and when it ends.
>
> **Isolation:** The intermediate state of a transaction is invisible to other transactions. As a result, transactions that run concurrently appear to be serialized.
>
> **Durability:** After a transaction successfully completes, changes to data persist and are not undone, even in the event of a system failure.

**Integrity constraints:** NOT NULL, UNIQUE, PRIMARY KEY, FOREIGN KEY

**Aggregate functions:** COUNT

**Data Definition Language (DDL) statements:** ALTER, CREATE, DROP, GRANT

**Data Manipulation Language (DML) statements:** CALL, INSERT, SELECT, DELETE, UPDATE

**Transaction Control statements:** COMMIT
