---
name: Modellierung
semester: 2026W
bereich: univie
kürzel: MOD
---

# Entity-Relationship Model
Tool: [[Bee-Up]]
Idea: A Model of a Database, before creating the Database.

## Elements
- Entities
- Relationships (with *cardinalities*)
- Attributes

![[Pasted image 20261005224440.png]]

## Mapping *cardinality* of relationships
- 1:1, 1:n, m:n, ... (how many entities are in relation to how many entities)
- m:n is problematic, circumvent this problem by adding another table. Example: Customer / Company
![[Pasted image 20261005224107.png]]

## Conversion to [[Database]]
-Entities: Table
-Relationships: Primary key <-> Foreign Key
-Attributes: Rows in a table