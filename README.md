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

**Lossless decomposition** - dividing relations in such a way that the resultant relations can be recombined without losing any of the information.

**Candidate key** - irreducible combination of attributes that uniquely identifies each tuple. Candidate key can be *simple* or *composite*.

**Functional dependency** - dependency between two sets, when for each value in the first set there is only one value in the second set.

**Normalization** - the process of organizing the attributes and relations to minimize data redundancy.

## The Relational Model
*defines data structure, data integrity and data manipulation rules*

Main characteristics of relational DBMS:
* all data is conceptually represented as a relation
* at any given position in the relation there is one and only one value
* all operations are performed on an entire relation and result in an entire relation

## Normalization forms
### First normal form (1NF)
Each attribute of a tuple must contain a single value.
###Second normal form (2NF)
The relation must be in first normal form and all its attributes must depend on the entire candidate key, not on the part of it. 
###Third normal form(3NF)
The relation must be in second normal form and all its non-key attributes must be mutually independent.
###Boyce/Codd normal form (BCNF)
The relation must be in second normal form. There must be no functional dependencies between candidate keys.
###Fourth normal form (4NF)
The relation must be in Boyce/Codd normal form and independent repeating groups must not be combined in a single relation.
###Fifth normal form (5NF)
A relation is in the 5NF if decomposing it would not remove any redundancies.

