# Database design
*Short notes on database design topics.*

## Definitions
**Problem space** - specific set of objects and interactions that limits the design of the database system.

**Data model** - conceptually describes the problem space (entities, their attributes, relationships, constraints).

**Schema** - data model described in terms of DBMS.

**DBMS** - DataBase Management System.

**Database** - physical objects (files) where the actual data is stored.

**Relation** - conceptual representation of data in the form of table with rows and columns.

**Tuple** - relation's row (single data record).

**Relation cardinality** - number of tuples in the relation.

**Attribute** - relation's column.

**Domain** - the set of all possible values that an attribute may validly contain. Can be *type-compatible*.

**Relation degree** - number of attributes in the relation.

**Entity** - anything about which the DBMS needs to store information. Can be *concrete* or *abstract*.

**Relationship** - association between entities (*relationship participants*). Can be *one-to-one*, *one-to-many*, or *many-to-many*. Entity participation in a relationship can be *partial* or *total*.

## The Relational Model
*defines data structure, data integrity and data manipulation rules*

Main characteristics of relational DBMS:
* all data is conceptually represented as a relation
* at any given position in the relation there is one and only one value
* all operations are performed on an entire relation and result in an entire relation
