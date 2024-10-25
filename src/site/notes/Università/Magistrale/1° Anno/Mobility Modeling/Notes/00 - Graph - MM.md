---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/mobility-modeling/notes/00-graph-mm/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/00 - Graph - MM\|00 - Graph - MM]]

Graphs are useful mathematical models for representing urban and transportation networks.

![Schermata 2024-10-10 alle 16.09.44.png](/img/user/Schermata%202024-10-10%20alle%2016.09.44.png)


## Directed graph

```ad-Definizione
title: Directed Graph

A **directed graph** is a set of $N$ nodes and a set of $A$ arcs or links whose elements are ordered pairs of distinct nodes.

It is represented as

$
G = (N, A)
$

```

- Nodes are usually numbered with integers.
- Arcs are either named with integers, or with the pair of nodes they connect

![00 - Graph 2024-10-10 16.12.25.excalidraw.png](/img/user/Excalidraw-2/00%20-%20Graph%202024-10-10%2016.12.25.excalidraw.png)


For the example graoh above we would have:
$$
\begin{align}
N &= {1,2,3,4,5,6,7} \\
A &= \left\{ (1,2), (1,3), (2,3), (2,4), (3,6), (4,5), (4,7), (5,2), (5,3), (5,7), (6,7)  \right\}
\end{align}
$$

## Graph representation

### Incidence matrix

[[Università/Triennale/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/07. Schematizzazione dell'offerta di trasporto#Matrice di incidenza\|07. Schematizzazione dell'offerta di trasporto#Matrice di incidenza]]

A graph is a just a diagram. We need to make calculations. We have to define a way to translate the graph into a mathematical instrument we can use. 

Each graph can be written as a matrix, called **incidence matrix**.

![00 - Graph 2024-10-10 16.18.33.excalidraw.png](/img/user/Excalidraw-2/00%20-%20Graph%202024-10-10%2016.18.33.excalidraw.png)


- Each row represents a node
- Each column represents an arc or link

We can represent a graph through a matrix in which every row represents a node, and each column represents a link (links are also numbered).

The graph above gives the following **incidence matrix**:
$$
\begin{bmatrix}
1 & 0 & 0 & 0 & 0 & 0 & 0 & -1 & 0 & 0  \\
-1 & 1 & 0 & 1 & 1 & 0 & 1 & 0 & 0 & 0  \\
0 & -1 & 1 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & -1 & -1 & -1 & 0 & 0 & 0 & 1 & -1 \\
0 & 0 & 0 & 0 & -1 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & -1 & 1 & -1 & 1
\end{bmatrix}
$$

## Elements in a graph

### Adjacency and Incidency

#### Forward star or Adjacency

```ad-Definizione
title: Forward star or Adjacency of node $i$ ($E[i]$)

A **forward star**, or **Adjacency** of a node $i$, is the set of head nodes of links emanating from node $i$. It is designated by $E[i]$.

```

For example, given the graph below:

![00 - Graph 2024-10-10 16.12.25.excalidraw.png](/img/user/Excalidraw-2/00%20-%20Graph%202024-10-10%2016.12.25.excalidraw.png)


the forward star of node $5$ is
$$
E[5] = {2,3,7}
$$

![Forward star - 00 - Graph 2024-10-24 12.48.02.excalidraw.png](/img/user/Excalidraw-2/Forward%20star%20-%2000%20-%20Graph%202024-10-24%2012.48.02.excalidraw.png)


By gathering the adjacency of all nodes, the number of links in A can be obtained:

$$
|A| = \left| E[1] \cup E[2] \cup \cdots \cup E[n] \right| 
$$


#### Incidency

```ad-Definizione
title: Incidency of node $i$

The incidency of node $i$ is the set of tail nodes of links *incoming* to node $i$.

```

### Out-degree and In-degree

```ad-Definizione
title: Outdegree of node $i$

The **out-degree** of node $i$ is the number of elements in the [[#Forward star or Adjacency]] of that same node $i$.

$
|E[i]| 
$
```

### Path

A **path** is a chain of links, starting at node $p$ and ending at a different node $q$.

#### Directed path

```ad-Definizione
title: Directed path

A **directed path** on a graph is a sequence of arcs 
$
a_{1} = (i_{1},j_{1}), a_{2} = (i_{2},j_{2}), ..., a_{n} = (i_{n},j_{n})
$
so that
$
j_{1} = i_{2}, j_{2} = i_{3}, ..., j_{n-1} = i_{n}
$

```

Given the following graph

![00 - Graph 2024-10-10 16.12.25.excalidraw.png](/img/user/Excalidraw-2/00%20-%20Graph%202024-10-10%2016.12.25.excalidraw.png)


a possible directed path si:

![Directed path - 00 - Graph 2024-10-24 13.00.21.excalidraw.png](/img/user/Excalidraw-2/Directed%20path%20-%2000%20-%20Graph%202024-10-24%2013.00.21.excalidraw.png)


$$
\text{path} = (1,2)(2,3)(3,6)(6,7)
$$

#### Undirected path


```ad-Definizione
title: Undirected path

An **undirected path** on a graph is a sequence of arcs 
$
a_{1} = (i_{1},j_{1}), a_{2} = (i_{2},j_{2}), ..., a_{n} = (i_{n},j_{n})
$
so that


```


$$
\begin{align}
j_{1} = i_{2} \quad \lor \quad  j_{1} &= j_{2} \quad \lor \quad i_{1} = i_{2} \\
j_{2} = i_{3} \quad \lor \quad j_{2} &= j_{3} \quad \lor \quad i_{2} = i_{3} \\
&\vdots \\
j_{n-1} = i_{n} \quad \lor \quad j_{n-1} &= j_{n} \quad \lor \quad i_{n-1} = i_{n}
\end{align}
$$
Given the graph


![00 - Graph 2024-10-10 16.12.25.excalidraw.png](/img/user/Excalidraw-2/00%20-%20Graph%202024-10-10%2016.12.25.excalidraw.png)


An undirected path can be:

![Undirected path - 00 - Graph 2024-10-24 13.08.17.excalidraw.png](/img/user/Excalidraw-2/Undirected%20path%20-%2000%20-%20Graph%202024-10-24%2013.08.17.excalidraw.png)


$$
\text{Undirected path} = (1,2)(2,3)(5,3)(5,7)
$$

#### Cycle

```ad-Definizione
title: Cycle

A **cycle** or **directed cycle** is a [[#Directed path]] with the additional condition
$
j_{n} = i_{1}
$

```

From the graph

![00 - Graph 2024-10-10 16.12.25.excalidraw.png](/img/user/Excalidraw-2/00%20-%20Graph%202024-10-10%2016.12.25.excalidraw.png)


a cycle is
$$
\text{cycle} = (2,4)(4,5)(5,2)
$$
There can also be undirected cycles, where the direction of links doesn't matter.

### Connected nodes

```ad-Definizione
title: Connected nodes

Node-$i$ is **connected** to node-$j$ if there exits a [[#Directed path]] starting at $i$ and ending at $j$.


```

### Tree

```ad-Definizione
title: Tree

A **tree** is a special type of graph that contains *no* [[#Cycle|cycles]].

It can be **directed** or **undirected**.

```

```ad-note
title: Observation

A [[#Path]] is always a tree. More specifically, a [[#Directed path]] is always a directed tree.

**BUT**

A tree is not necesseraly a [[#Path]]

```

#### Spanning tree

```ad-Definizione
title: Spanning tree

A **spanning tree** is a part of graph $G$, or subgraph, that contains all the same nodes of $G$ but with only a subset of links, so that they forma an *undirected* [[#Tree]].

```

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

Do slides 11 to 13 (finish pdf).

See iPad.

