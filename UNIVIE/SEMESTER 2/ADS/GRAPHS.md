---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

## FORMAL DEFINITION

A Graph $G = (V, E)$ is a pair of:
- Vertices $V = \{\text{nodes}\}$
- Edges $E = \{\{u, v\} \text{ or } (u,v) \text{ in a directed graph }\}$

Degree of a Vertex $V$: how many edges $E$ are coming out of it.

![[Pasted image 20260822215816.png]]

## TRAVERSING

A $path$ is a route from Vertex A to Vertex B.
1. An [[EULER PATH]] is a $path$ that uses every edge strictly once.

A $circuit$ is a route from Vertex A to Vertex A.
1. An [[EULER CURCUIT]] is a $circuit$ that uses every edge strictly once.
2. No circuits at all: *acyclic graph*

A [[MINIMUM SPANNING TREE]] is a sub-graph that contains every vertex and minimal edges (minimal amount and minimal weight).

## TYPES OF GRAPHS

A Graph is $connected$ if there is a path from every vertex to every vertex.
[[TREES]] are connected graphs with minimum edges for connectivity.

Graphs can be:
1. weighted / unweighted
2. directed / undirected

## GRAPH ALGORITHMS
[[GRAPH ALGORITHMS]]


[[TOPOLOGICAL ORDER]]

## REPRESENTATION

Write out all edges $E$ -> inefficient -> adjacency matrix or adjacecy list

![[Pasted image 20260822215543.png]]