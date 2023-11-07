- [Indexing](#indexing)
- [ACID Properties](#acid-properties)
  - [Atomicity](#atomicity)
  - [Consistency](#consistency)
  - [Isolation](#isolation)
  - [Durablity](#durablity)
- [Relationship between Tables](#relationship-between-tables)
- [Where Clause](#where-clause)
- [Join Clause](#join-clause)

---

## Indexing

## ACID Properties

> ***ACID properties:*** are a set of properties that guarantee reliable processing of transactions in a database management system (DBMS). ACID properties ensure that transactions are processed reliably and consistently in a DBMS.

***Transaction:*** is a logical unit of work that accesses and updates the content of a database. Read and write operations are used by transactions to access data.

***ACID Transaction:*** is a group of database read and write operations that only succeeds if all the operations within succeed. Transactions can impact a single record or multiple.

ACID is acronym of

- Atomicity - It ensures that a transaction is either executed completely or not at all.
- Consistency - It ensures that database remain in a consistance state before and after a transaction.
- Isolation - It ensures that multiple transactions can run concurrently without interfering with each other.
- Durability - It ensures that the result of a successfully commited transaction are premanent and cannot be lost due to system failure.

### Atomicity

### Consistency

### Isolation

### Durablity

---

## Relationship between Tables

## Where Clause

## Join Clause
