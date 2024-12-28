---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/mobility-modeling/notes/traveling-salesman-problem/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/Traveling Salesman Problem\|Traveling Salesman Problem]]

```table-of-contents
```

```ad-Definizione
title: Traveling Salesman Problem

The **Traveling Salesman Problem** consists in solving the following:

Given a complete graph, with $n$ nodes, and the cost of traveling between each and every pair of nodes, what is the shortest possible route that visit each node only once and returns to the initial node?

```

The following elements come into play:
- $K_{n}:$ the complete graph with $n$ nodes, where $V$ is the set of nodes and $|V| = n$
- $c_{ij}:$ cost associated with link $(i,j)$
- $x_{ij}:$ **decision variable** - equals 1 if link $(i,j)$ is used in the solution, 0 otherwise
- **Objective:** find an [[Hamiltonian circuit\|Hamiltonian circuit]] of minimum cost when the cost of a circuit is the sum of the costs of the links defining the circuit

## Formulation of the TSP

There exist several formulations for the TSP.

### Basic TSP formulation

A basic formulation of the [[#Traveling Salesman Problem]] is the following:

```ad-Teo
title: Basic Traveling Salesman Problem formulation

$
\min_{x_{ij}} \sum\limits_{(i,j) \in A} c_{ij}x_{ij}
$
subject to:
$
\text{Degree constraints:}\begin{cases}
\sum\limits_{j \in A^{+}(i)} x_{ij} = 1, \qquad \forall i \in V \\
\sum\limits_{j \in A^{-}(i)} x_{ij} = 1, \qquad \forall i \in V
\end{cases}
$
where:
- $x_{ij}\in \{0,1\}, \quad \forall (i,j) \in A$
	- $x_{ij}= 1$ if link $(i,j)$ is used in the solution, 0 otherwise

```

**DEGREE CONSTRAINTS:**
The **degree constraints** are needed to ensure that every node has only one link entering it and one exiting it.

More specifically:
- $A^{+}(i)= \{j | (i,j) \in A\}:$ set of all links *entering* node $i$
- $A^{-}(i)= \{j | (j,i) \in A\}:$ set of all links *exiting* node $i$

```ad-attention

This formulation is not sufficient to define the problem. In fact, a possible solution with this formulation could give something like this:

![Schermata 2024-12-27 alle 17.25.03.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/Allegati/Schermata%202024-12-27%20alle%2017.25.03.png)

In the solution shown above, we can see that every link is only visited once, and the cost was minimized. We can easily see thoug that many **subtours** were made in place of a single tour.
```

### TSP formulation with subtours breaking constraints

In order to avoid subtours like the one originating from the [[#Basic TSP formulation]], a new constraint is added to the formulation:


```ad-Teo
title: Traveling Salesman Problem formulation with subtours breaking constraints

$
\min_{x_{ij}} \sum\limits_{(i,j) \in A} c_{ij}x_{ij}
$
subject to:
$
\begin{align}
\text{Degree constraints:} &\begin{cases}
\sum\limits_{j \in A^{+}(i)} x_{ij} = 1, \qquad \forall i \in V \\
\sum\limits_{j \in A^{-}(i)} x_{ij} = 1, \qquad \forall i \in V \\
x_{ij} \in \{0,1\}, \qquad \forall (i,j) \in V
\end{cases} \\ \\

\text{Subtour breaking constraint:} &\sum\limits_{i\in S, j \in S} x_{ij} \le |S| - 1, \qquad \forall S \ne 0, \quad S\subset V
\end{align}
$
where:
- $x_{ij}\in \{0,1\}, \quad \forall (i,j) \in A$
	- $x_{ij}= 1$ if link $(i,j)$ is used in the solution, 0 otherwise
- $S:$ is a subset of all the nodes ($V$)

```

**SUBSETS BREAKING COSTRAINT:**
The **subset breaking constraint** does the following: for any subset of nodes, the number of links connecting these nodes has to be lower or equal the number of nodes in the subset minus 1. With this constraint, if $S \equiv V$, than a tour connecting all nodes will necessarily have $|V|-1$ links. If, for example, I was to take a subset, $S$, with only 3 nodes, and these 3 nodes where connected to each other in a cycle, the cycle would contain 3 links, but this would break the constraint. So, if we check this condition for every possible subset of $V$, we will be sure that no subtour is created.

```ad-attention

Despite this constraint being theoretically acturate, and it would allow to come to the right solution to the problem, given a network with $n$ nodes, the constraints needed would amount to
$
2^{n-1}
$
conditions. These, is way too many for any computer when $n$ approaches values of any significance.
```


### TSP formulation with weak subtour breaking constraints

Since, as we've seen in [[#TSP formulation with subtours breaking constraints]], the formulation of the breaking constrains is highly impractical when it comes to solving the problem with a computer, we hereby propose an alternative formulation. 

```ad-Teo
title: Traveling Salesman Problem formulation with weak subtours breaking constraints

$
\min_{x_{ij}} \sum\limits_{(i,j) \in A} c_{ij}x_{ij}
$
subject to:
$
\begin{align}
\text{Degree constraints:} &\begin{cases}
\sum\limits_{j \in A^{+}(i)} x_{ij} = 1, \qquad \forall i \in V \\
\sum\limits_{j \in A^{-}(i)} x_{ij} = 1, \qquad \forall i \in V \\
x_{ij} \in \{0,1\}, \qquad \forall (i,j) \in V
\end{cases} \\ \\
\text{Weak Subtour breaking constraint:}
&\begin{cases}
u_{j} \ge u_{i} - n(1-x_{ij}) + 1, \qquad i\ne j, \quad i \ne 1 \\
u_{1} = 1 \\
1 \le u_{i} \le n, \qquad \forall i \in V
\end{cases}
\end{align}
$
where:
- $x_{ij}= 1$ if link $(i,j)$ is used in the solution, 0 otherwise

```

Explanation of the **WEAK SUBTOUR BREAKING CONSTRAINT**
$u_{i}$ is a variable that allows to avoid subtours in the solution. Notice how $u_{j}$ must be greater than a certain quantity, specifically $u_{j} \ge u_{i}+1$ for links in the solution, **except** for when $i=1$. $i=1$ is the depot. This means that, the only occasion where $u_{j}$ can be lower than $u_{i}+1$ is when we go back to the depot. It is therefore impossible for the problem to generate subtours. In fact, that would mean that a cycle is created but in order for that to happen, $u_{j}$ would be greater than $u_{i}+1$ when $i$ is not 1. Here is an attempt of a visual representation of how this constraint works:

![Traveling Salesman Problem 2024-12-27 19.37.16.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/Traveling%20Salesman%20Problem%202024-12-27%2019.37.16.excalidraw.png)
%%[[Traveling Salesman Problem 2024-12-27 19.37.16.excalidraw|Edit in excalidraw]]%%

The figure above shoes the same network with 2 different solutions to the TSP. Keep in mind only the links in the solution are shown, the network is supposed to be complete.

On the left, the solution breaks the the *weak subtour breaking constraints*. In fact, $u_{1}'\ge 4$ and $u_{1}=1$ is suppsed to be a contraddiction: in fact a number cannot be greater than 4 and equal to 1 at the same time (the prime notation is just to show that it is obtained following the cycle). This is allowed since for $i = 1$ the constraint is not valid. Notice though how the same happens in the green cycle at node 4. This time though this disrepancy is not allowed, therefore, this solution is not permitted. 

On the write, a unique cycle where the only occasion where the constraint is broken is when it is actually allowed, at $i = 1$.


## Solving the TSP

Solving the [[Traveling Salesman Problem]] is no easy task. That is why the problem is most often approached through [[Heuristic]] methods.

These are methods that are not proven to be mathematically optimised (as a matter of fact, they are not), but rather use an intuitive approach to reach a solution that is, at the very least, good enough. They won't guarantee to approach the exact solution, but should be able to provide a solution that is not far from it.

We will see the following:
- [[#Nearest neighbour heuristic]]
- [[#Nearest neighbour insertion heuristic]]
- [[#Spanning tree heuristic]]
- [[#Christofides heuristic]]
- [[#Improvement heuristics]]

For any of the following method, a cost matrix is going to be needed. This is a matrix that, for each link, gives the cost of traveling on that link.

### Nearest neighbour heuristic

The **nearest neighbour heuristic** is considered a [[greedy heuristic]].

```ad-Teo
title: Nearest neighbour heuristic

To approach a solution this is how we proceed:
1. Select a node $i \in N$ in the network. Label this node as to remember that has already been visited;
2. Look at all the links leaving node $i$ and select the one with the lowest cost;
3. Follow the selected link to $j$ and label it too;
4. Keep going like this until all nodes have been labeled.

We can think of labelling a node as to add it to a set $T$. Whenever we look for a new link, we will only check links the go to a node that is not yet in $T$.

When all nodes are in $T$, we stop as we will have obtained a [[Hamiltonian circuit]].

```


### Nearest neighbour insertion heuristic

The **nearest neighbour insertion heuristic** is considered a [[greedy heuristic]].

```ad-Teo
title: Nearest neighbour insertion heuristic

1. Select any initial subtour. The nodes in the subtour will go into a set $C$
2. For every $i^{\rm th}$ node not in the subtour, create a set, $d(i,C)$ containing all costs from and to that node $i$ to every node in the subtour ($C$)
	- we will have something like: $d(i,C) = \{c_{i1}, c_{i2}, ...,c_{in}\}$ for each node $i \not\in C$
3. Select the minimum cost of each set $d(i,C)$: $\min\limits_{j\in C} (d(i,C))$
4. Select the minimum of all the costs found in step 3
5. Add the selected link to the subtour and repeat the steps


```


### Spanning tree heuristic

To apply the spanning tree heuristic, a [[07. Schematizzazione dell'offerta di trasporto#Completezza di un grafo|complete graph]] is needed: $K_{n} = (V,A)$ (where: $V$-set of links and $A$-set of nodes).

```ad-Teo
title: Spanning tree heuristic

1. Find a [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/Traveling Salesman Problem#Finding a Minimum Spanning Tree - Prim's Algorithm\|minimum spanning tree]] of $K$ --> $ST$
2. **Double** all arcs in $ST$, generating an auxiliary graph: $(V,ST)$
3. Since each node has [[Eulerian cycle#Even degree\|even degree]], an [[Eulerian cycle\|Eulerian cycle]] exists
	1. Determine an [[Eulerian cycle\|Eulerian cycle]]: $C$
	2. Assign an orientation to $C$
	3. Select a starting node $i$
4. Make a [[Hamiltonian circuit\|Hamiltonian cycle]] following the nodes in the order of the [[Eulerian cycle\|Eulerian cycle]]. whenever a node already visited should be selected, jump to the first available node in the [[Eulerian cycle\|Eulerian cycle]]
5. Stop when the [[Hamiltonian circuit\|Hamiltonian cycle]] is complete

```

#### Finding a Minimum Spanning Tree - Prim's Algorithm

```ad-Teo
title: Prim's Algorithm

1. Select an arbitrary node in the network
2. Select the arc with the minimum cost among those that connect any node already in the ST to any node not yet in the spanning tree
3. Repeat until the Spanning Tree contains all nodes in the network

```

### Christofides heuristic

```ad-Teo
title: Christofides heuristic

1. Determine a [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/Traveling Salesman Problem#Finding a Minimum Spanning Tree - Prim's Algorithm\|Minimum Spanning Tree]] $ST$ of $K_{n}$
2. Find all nodes with [[Eulerian cycle#Even degree\|odd degree]] and find a [[Minimum Perfect Matching\|Minimum Perfect Matching]], $M$
3. Make a new graph, $H$, out of all the edges in $ST$ and $M$
4. Form an [[Eulerian cycle\|Eulerian cycle]] in $H$ and orient it arbitrarily
5. Make a [[Hamiltonian circuit\|Hamiltonian cycle]] following the nodes in the order of the [[Eulerian cycle\|Eulerian cycle]]. whenever a node already visited should be selected, jump to the first available node in the [[Eulerian cycle\|Eulerian cycle]] 
Stop when all nodes are part of the [[Hamiltonian circuit\|Hamiltonian cycle]].


```


### Improvement heuristics

In the heuristics described above, it is rare to find an optimal solution. They are, in general, of moderate quality. Therefore, we pose the question of how we can improve a [[Hamiltonian circuit|Hamiltonian cycle]] found in one of the previous heuristic.

We will see the [[#Exchange Heuristic]]. This is quite intuitive to understand if we're looking at an Euclidean problems. In a Euclidean problem, the distance between 2 nodes is given simply by the Euclidean distance between the nodes (basically, the real distance in any geometric space).

In this case, whenever a [[Hamiltonian circuit|Hamiltonian cycle]] crosses itself, there must exist a better path, without crossings. What we will do is to unfold the path where it crosses itself in order to have a lower cost.

In a general problem (not euclidean), we can't really think in terms of unfolding a crossing, but the concept stays the same. We'll try to exchange some links in order to bring the cost between 2 nodes down. This is what we do in the [[#Exchange Heuristic]]

#### Exchange Heuristic

Suppose we have a [[Hamiltonian circuit|Hamiltonian cycle]] like the following:

![Traveling Salesman Problem 2024-12-28 15.41.04.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/Traveling%20Salesman%20Problem%202024-12-28%2015.41.04.excalidraw.png)
%%[[Traveling Salesman Problem 2024-12-28 15.41.04.excalidraw.md|🖋 Edit in Excalidraw]]%%

We are interested in links: $(i_{p}, i_{p+1})$ and $(i_{1}, i_{q+1})$.

The heuristic goes as follow:
1. Choose any vertex $i$
2. Pick a pair of links such that they fall into the set $Z$:
$$
Z := \left\{ (i_{p}, i_{p+1}), (i_{q}, i_{q+1})  \quad|\quad  p+1 \ne q,\, p \ne q,\, q+1 \ne p,\, 1 \le p,\, q \le n   \right\}
$$
which means any pair of links such that they have at least one other link in between them.
3. For each pair in $Z$ check if
$$
c_{p,p+1} + c_{q,q+1} > c_{p,q} + c_{p+1,q+1}
$$
then remove links $(i_{p}, i_{p+1})$ and $(i_{1}, i_{q+1})$ from the solution and add $(i_{p}, i_{q})$ and $(i_{p+1}, i_{q+1})$.
Repeat for every node in the network.

![Traveling Salesman Problem 2024-12-28 15.54.03.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/Traveling%20Salesman%20Problem%202024-12-28%2015.54.03.excalidraw.png)
%%[[Traveling Salesman Problem 2024-12-28 15.54.03.excalidraw.md|🖋 Edit in Excalidraw]]%%

In the example we confront the cost of having the green links in place of the red ones. Since the cost is lower for the green pair, then we exchange them. Notice how we also need to switch the direction of the dashed links in order to keep the directed hamiltonian cycle.

```ad-note
title: Asymmetric graphs

In case of asymmetric graphs, we also need to check and compare the costs of the links we do not intend to exchange but that we need to reverse. It would become:
$
c_{p,p+1} + c_{q,q+1} + {\color{orange} c_{p+1, q}} > c_{p,q} + c_{p+1,q+1} + {\color{orange} c_{q, p+1}}
$
where the orange costs are the total costs to go from node $p+1$ to node $q$ (with all the intermediate links taken into account) and viceversa.

```

