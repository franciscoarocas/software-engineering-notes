# Part 1: storing Engines

DB consinsts on:

1. Transport layer accepting requests

2. Query processor which selects most esfficient way to run queries

3. Execution engine carrying out operations

4. Storage engine (Component of DB ssytem which store, retrieve and manage data in memory and disk)

When you want to choose a database, first check your needs, because if you select wrong database, the migration to other engine can be expensive. You can create workloads to check each database bottlenecks for your needs, and then select db system which is better for your requierements. You need to ask these questions:

* Does the database support the required queries?

* Is this database able to handle the amount of data we're planning to store?

* How many read and write operations can a single node handle?

* How many nodes should the system have?

* How do we expand the cluster given the expected growth rate?

* What is the maintenance process?

**TCP-C** is one of the most knownoldle benchmarks to measure the performance of OLTP databases (OLTP = *Online Transaction Process*)

Choosing DB is a long-term decision, also tests new versións of your db (Example upgrade from 1.0 to 1.2), because can introduce new bugs, performance issues, etc.

Its doesnt exists a perfect DB engine. Each one has trade-off, you need to select the better engine for your aproach. For example, intensive read, or intensive write, etc.
