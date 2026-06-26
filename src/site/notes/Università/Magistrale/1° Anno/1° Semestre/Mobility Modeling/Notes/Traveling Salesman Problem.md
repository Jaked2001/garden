---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/mobility-modeling/notes/traveling-salesman-problem/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"MM","Tipo":"T","Stato":"🟡 Finire","Slide":null,"PDF":null,"Parents":["[[📐 Mobility Modeling|📐 MM]]","[[Introduzione Ricerca Operativa]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Magistrale/1° Anno/1° Semestre/Mobility Modeling/Notes/Traveling Salesman Problem\|Traveling Salesman Problem]]

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
- **Objective:** find an [[Hamiltonian circuit]] of minimum cost when the cost of a circuit is the sum of the costs of the links defining the circuit

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

![Schermata 2024-12-27 alle 17.25.03.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Mobility%20Modeling/Notes/Allegati/Allegati/Schermata%202024-12-27%20alle%2017.25.03.png)

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

Remember:
- $A^{+}(i)= \{j | (i,j) \in A\}:$ set of all links *entering* node $i$
- $A^{-}(i)= \{j | (j,i) \in A\}:$ set of all links *exiting* node $i$

**SUBTOUR BREAKING COSTRAINT:**
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

Remember:
- $A^{+}(i)= \{j | (i,j) \in A\}:$ set of all links *entering* node $i$
- $A^{-}(i)= \{j | (j,i) \in A\}:$ set of all links *exiting* node $i$

Explanation of the **WEAK SUBTOUR BREAKING CONSTRAINT**
$u_{i}$ is a variable that allows to avoid subtours in the solution. Notice how $u_{j}$ must be greater than a certain quantity, specifically $u_{j} \ge u_{i}+1$ for links in the solution, **except** for when $i=1$. $i=1$ is the depot. This means that, the only occasion where $u_{j}$ can be lower than $u_{i}+1$ is when we go back to the depot. It is therefore impossible for the problem to generate subtours. In fact, that would mean that a cycle is created but in order for that to happen, $u_{j}$ would be greater than $u_{i}+1$ when $i$ is not 1. Here is an attempt of a visual representation of how this constraint works:

![Traveling Salesman Problem 2024-12-27 19.37.16.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Mobility%20Modeling/Notes/Allegati/Traveling%20Salesman%20Problem%202024-12-27%2019.37.16.excalidraw.png)
[[Traveling Salesman Problem 2024-12-28 15.41.04.excalidraw|🖋 Edit in Excalidraw]][[Traveling Salesman Problem 2024-12-28 15.54.03.excalidraw|🖋 Edit in Excalidraw]]%%

In the example we compare the cost of having the green links in place of the red ones. Since the cost is lower for the green pair, then we exchange them. Notice how we also need to switch the direction of the dashed links in order to keep the directed hamiltonian cycle.

```ad-note
title: Asymmetric graphs

In case of asymmetric graphs, we also need to check and compare the costs of the links we do not intend to exchange but that we need to reverse. It would become:
$
c_{p,p+1} + c_{q,q+1} + {\color{orange} c_{p+1, q}} > c_{p,q} + c_{p+1,q+1} + {\color{orange} c_{q, p+1}}
$
where the orange costs are the total costs to go from node $p+1$ to node $q$ (with all the intermediate links taken into account) and viceversa.

```

