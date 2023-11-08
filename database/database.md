- [SQL Commands](#sql-commands)
- [Indexing](#indexing)
- [ACID Properties](#acid-properties)
  - [Atomicity](#atomicity)
  - [Consistency](#consistency)
  - [Isolation](#isolation)
  - [Durability](#durablity)
- [Relationship between Tables](#relationship-between-tables)
- [Where Clause](#where-clause)
- [Join Clause](#join-clause)

---

## SQL Commands

These are mainly categorised into five(5) category:

- DDL (Data Definition Language)
  - CREATE
  - DROP
  - ALTER
  - TRUNCATE
- DQL (Data Query Language)
  - SELECT
- DML (Data Manipulation Language)
  - INSERT
  - UPDATE
  - DELETE
- DCL (Data Control Language)
  - GRANT
  - REVOKE
- TCL (Transaction Control Language)
  - COMMIT
  - SAVE POINT
  - ROLLBACK



## Indexing

> **Definition :** A

## ACID Properties

> ***ACID properties:*** are a set of properties that guarantee reliable processing of transactions in a database management system (DBMS). ACID properties ensure that transactions are processed reliably and consistently in a DBMS.

***Transaction:*** is a logical unit of work that access and update the content of a database. Read and write operations are used by transactions to access data.

***ACID Transaction:*** is a group of database read and write operations that only succeeds if all the operations within succeed. Transactions can impact a single record or multiple.

ACID is acronym of

- Atomicity - It ensures that a transaction is either executed completely or not at all.
- Consistency - It ensures that database remain in a consistency state before and after a transaction.
- Isolation - It ensures that multiple transactions can run concurrently without interfering with each other.
- Durability - It ensures that the result of a successfully commited transaction are permanent and cannot be lost due to system failure.

### Atomicity

 A person tries to book a ticket, selects a seat, and proceeds to the payment gateway but encounters a failure due to bank server issues, their booked seat will not be reserved for them. A complete transaction involves reserving the seat and completing the payment. If any step fails, the operation is aborted, and the user is brought back to the initial state without their seat being reserved.

### Consistency

One person is trying to book a ticket. They are able to reserve their seat but their payment hasn’t gone through due to bank issues. In this case, their transaction is rolled back. But just doing that isn’t sufficient. The number of available seats must also be updated. Otherwise, if it isn’t updated, there will be an inconsistency where the seat given up by the person is not accounted for. Hence, the total sum of seats left in the train + the sum of seats booked by users would not be equal to the total number of seats present in the train if not for consistency.

### Isolation

Two people try to book the same seat simultaneously. Transactions are serialized to maintain data consistency. The first person's transaction succeeds, and they receive a ticket. The second person's transaction fails as the seat is already booked. They receive an error message indicating no available seats.

### Durability

Suppose that there is a system failure in the railway management system resulted in the loss of all booked train details. Millions of users who had paid for their seats are now unable to board the train, causing significant financial losses and eroding trust in the company. The situation is particularly critical as these trains are needed for important reasons, causing widespread panic and inconvenience.

---

## Relationship between Tables

## Where Clause

## Join Clause
