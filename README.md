# Database design
*Short notes on database design topics.*

## Definitions
**Problem space** - specific set of objects and interactions that limits the design of the database system.

**Data model** - conceptualy describes the problem space (entities, their attrubutes, relationships, constraints).

**Schema** - data model described in terms of DBMS.

**DBMS** - DataBase Management System.

**Database** - physical objects (files) where the actual data is stored.

**Relation** - conseptual representation of data in the form of table with rows and columns.

**Tuple** - relation's row (single data record).

**Relation cardinality** - number of tuples in the relation.

**Attribute** - relation's column.

**Relation degree** - number of attributes in the relation.

## The Relational Model
*defines data structure, data integrity and data manipulation rules*

Main characteristics of relational DBMS:
* all data is conceptually represented as a relation
* at any given position in the relation there is one and only one value
* all operations are performed on an entire relation and result in an entire relation
