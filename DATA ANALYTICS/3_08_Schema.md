# Schema

#### 1. Star Schema
The star schema is the simplest and most commonly used data warehouse schema. It consists of a central fact table surrounded by dimension tables.

Components: Fact table ,Dimension table.

Advantages:

Simple and easy to understand.
Efficient for querying large datasets.
Use Case: Best suited for straightforward, query-intensive environments where speed is crucial.

#### 2. Snowflake Schema
The snowflake schema is a more complex version of the star schema where dimension tables are normalized into multiple related tables.

Components: Fact tables, normalized dimension tables.

Advantages:

Reduces data redundancy.
Can improve query performance by reducing the size of dimension tables.
Use Case: Ideal for data warehouses where space efficiency and data integrity are prioritized.

#### 3. Galaxy Schema (Fact Constellation):
The galaxy schema, also known as a fact constellation, consists of multiple fact tables that share dimension tables. It's a more complex model used to represent multiple business processes.

Components: Multiple fact tables, shared dimension tables.

Advantages:

Supports complex queries across multiple business processes.
Allows for more flexibility in data analysis. .
Use Case: Best for large, enterprise-level data warehouses with diverse business processes

