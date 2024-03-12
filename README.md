[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/QM7QGF1q)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

# Graph Isomorphism Proof:

## Definitions

**Graph Isomorphism**: Two graphs $G_1=(V_1, E_1)$ and $G_2=(V_2, E_2)$ are isomorphic if there exists a bijection $f: V_1 \rightarrow V_2$ such that for any pair of vertices $(u, v) \in V_1$, $(u, v) \in E_1$  $\Longleftrightarrow$ $(f(u), f(v)) \in E_2$. This definition ensures the preservation of adjacency relationships between vertices through a bijection.

**Complete Connectivity**: A graph is completely connected, or a complete graph, if there is an edge between every pair of distinct vertices. The notation for a complete graph with $n$ vertices is $K_n$.

## Proof by Contradiction

To prove that two graphs being isomorphic does not require them to be completely connected, we assume the contrary and derive a contradiction.

### Assumption

Assume that for two graphs $A$ and $B$ to be isomorphic, they must be completely connected.

### Contradictory Example

- Let $G_1=(V_1, E_1)$ be a simple path graph $P_3$ with vertices $V_1 = \{a, b, c\}$ and edges $E_1 = \{(a, b), (b, c)\}$.
- Let $G_2=(V_2, E_2)$ also be a simple path graph $P_3$ with vertices $V_2 = \{x, y, z\}$ and edges $E_2 = \{(x, y), (y, z)\}$.

Under the assumption, $G_1$ and $G_2$ cannot be isomorphic since they are not completely connected, contradicting the requirement for a $K_n$ structure.

### Isomorphism Verification

A bijection $f: V_1 \rightarrow V_2$ can be defined by $f(a) = x$, $f(b) = y$, and $f(c) = z$, which satisfies the isomorphism condition by preserving the adjacency relationship, therefore contradicting the initial assumption.

## Conclusion

The contradiction clearly shows that our initial assumption is incorrect. The example of simple path graphs, which are not completely connected but satisfy the formal definition of graph isomorphism, denies the requirement of complete connectivity for isomorphism. Therefore, it is proved that two graphs can be isomorphic without being completely connected, as the essential requirement is the preservation of adjacency relationships through a bijection, as per the formal definition of graph isomorphism.
