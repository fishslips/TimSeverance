### Relations

Relation is the word we use when an element from one set maps to an element in another set.

We use the notation xRy to indicate that x relates, or maps, to y. R is the set of relations from one set to another set.

If we have a cartesian product A x B where A = {1,2} and B = {A, B}, then A x B = {(1, A), (1,B), (2, A), (2,B)}

We can represent any subset of this Cartesian Product as the set R (Relation). What we're indicating here is that we have this sort of ordered mapping, where the first element in the tuple is an element from the domain, and that the second element is from the range. So we're indicating that 1 maps to A, and it also maps to B. 2 maps to A, and it also maps to B. Keep in mind, we're not necessarily ensuring that the mappings enforce a well defined function. 

Set R doesn't have to include every element of the cartesian product. It just represents some given subset.

#### Reflexive

if all elements in the domain A map to themselves. Or in other words, for all x in A, xRx.

Example: A = {1,2} ... A x A = {(1,1), (1,2), (2,1), (2,2)} 

R = {(1,1), (2,2)}
Note: This subset R doesn't include all elements from the cartesian product, but the elements it does include follow the rule of xRx. In other words, 1 maps to 1, 2 maps to 2, and is reflexive.

R = {(1,1), (1,2), (2,1)} 
Note: This subset R doesn't include all elements from the cartesian product. And since it's missing (2,2), it is not reflexive

#### Anti-Reflexive

For all elements in the domain, it is not true that xRx. 

Example: A = {1,2} ... A x A = {(1,1), (1,2), (2,1), (2,2)} 

R = {(1,2)}
Note: This subset R has mappings (1,2) xRy. Since it has no mappings xRx, it is anti-reflexive.

R = {(1,1), (1,2), (2,1)} 
Note: This subset R has a mapping (1,1), and so it is not anti-reflexive

#### Symmetric

For all elements in the domain, xRy if and only if yRx

Example A = {1,2,3} ... A x A = {(1,1)(1,2)(1,3)(2,1,)(2,2)(2,3)(3,1)(3,2)(3,3)}

R = {(1,2),(2,1)}
Note: This subset has mappings (1,2) and (2,1), which means that xRy and yRx. 

R = {(1,2)(2,1)(1,3)}
Note: Even though this subset has mappings (1,2) and (2,1) which are symmetric by themselves, we also include (1,3), but not (3,1), so it is not symmetric.

#### Anti-symmetric

Can't be symmetric. Everything else is allowed.

#### Transitive

If a maps to b, and b maps to c, then a maps to c.

Note: This isn't saying that a graph must be transitive, just that it is transitive if we have mappings from x to y, then y to z, and x to z.

### Digraphs

is a pair of Vertices and their Edges (V,E). V is a set of vertices, E is a set of directed edges that is a subset of V x V. 

#### Head / Tail
In a directed graph, v -> u, v is the head, u is the tail.

#### In/Out Degree

How many edges point to or away from a vertex

#### Walk
Can be reprsented by notation

<v0, v1, ... vi>

Length = number of edges in a walk

Open Walk is where first and last vertices are not the same
Closed walk is when the first and last vertices are the same

**Types of Walks**
- Trail: Unique Edges
- Path: Unique Vertices
- Circuit: A closed trail. Or a closed walk with unique edges
- Cycle: A circuit greater than or equal to 1, where all vertices are unique except for the start and end. In other words, A Circuit Path.

### Composition of Relations

All relations have been represented using a digraph so far.

The composition of relations basically takes a mapping aXb and mapping bYc, and we end up with the relation aZc if we composite the relations together.

#### Graph Powers and Transitive Closure

#### Matrices

#### Partial Order

Relation R on set A is a partial order if it is reflexive, transitive, and anti-symmetric. 

#### Strict Order

Irreflexive, assymetric, and transitive

#### Equivalence Relations
Reflexive, symmetric, and transitive

### Directed Acyclic Graphs