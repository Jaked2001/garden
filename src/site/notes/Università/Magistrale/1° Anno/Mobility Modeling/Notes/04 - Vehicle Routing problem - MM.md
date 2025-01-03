---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/mobility-modeling/notes/04-vehicle-routing-problem-mm/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/04 - Vehicle Routing problem - MM\|04 - Vehicle Routing problem - MM]]

```table-of-contents
```

# The Capacitated Vehicle Routing Problem - CVRP

In a system, we identify 1 **depot** and many **clients**. Given $k$ trucks (or delivery vehicle in general), we want to assign every client to a track and then define a cycle route from and to the depot, that the truck has to follow in order to deliver to every client, minimizing the total cost.

![04 - Vehicle Routing problem - MM 2024-12-23 17.27.34.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/04%20-%20Vehicle%20Routing%20problem%20-%20MM%202024-12-23%2017.27.34.excalidraw.png)
%%[[04 - Vehicle Routing problem - MM 2024-12-23 17.27.34.excalidraw.md|🖋 Edit in Excalidraw]]%%

for example, given the situation above (imaiginig that all points are nods of a [[07. Schematizzazione dell'offerta di trasporto#Completezza di un grafo|complete graph]]), we wnat to get a solution like:

![04 - Vehicle Routing problem - MM 2024-12-23 17.29.01.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/04%20-%20Vehicle%20Routing%20problem%20-%20MM%202024-12-23%2017.29.01.excalidraw.png)
%%[[04 - Vehicle Routing problem - MM 2024-12-23 17.29.01.excalidraw.md|🖋 Edit in Excalidraw]]%%

In the graph above, each color represent a transportation unit.

What we want to achieve in the Capacitated Vehicle Routing Problem, is to:
- Assign each client to one transportation unit
- Create the best route for each transportation unit

## Overview of CVRP

As we will see, the problem is formulated as a **binary linear programming problem**.

Since the CVRP is a quite difficult problem to both formulate and solve, the common approach is to first work on an simpler problem, known as the [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/Traveling Salesman Problem\|Traveling Salesman Problem]]

```ad-danger

Before continuining reading this note, it is higly suggested to read the [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/Traveling Salesman Problem\|Traveling Salesman Problem]], if you're not yet familiar with it and with the methods to solve it.

```


### Characteristics of CVRP

- Each costumer is visited **exactly once** by **one** vehicle
- The route of each vehicle starts and ends at the depot
- The sum of demands of costumers on a route must not exceed vehicle's capacity


## CVRP formulations

We will give several formulations of the [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/04 - Vehicle Routing problem - MM\|Capacitated Vehicle Routing Problem]].

Conceptually we could define the problem in 2 parts:
- Assigning clients to trucks - [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/04 - Vehicle Routing problem - MM#CVRP formulation in terms of linear generalised assignment problem\|#CVRP formulation in terms of linear generalised assignment problem]]
- Optimizing routes

### CVRP formulation in terms of linear generalised assignment problem

We first give a formulation of a problem that would allow to assign clients to a route efficiently.

Let's first define the variables and parameters needed in this formulation.

**Paramters:**
- Suppose we have $n$ clients. Each client will be named $i = 1,...,n$. 
- There is one depot, at $i=0$
- There are $K$ delivery vehicles (trucks) available. Each one is called $k = 1,...,K$
- $C_{k}$ is the capacity of vehicle $k$
- $a_{i}$ is the amount of goods that client $i$ requires

**Decision Variable:**
$y_{ik}$ is the decision variable. It's a binary variable:
$$
y_{ik} =
\begin{cases}
1, \quad \text{if client } i \text{ is visited by truck } k \\
0, \quad \text{otherwise}
\end{cases}
$$
**Objective function:**
$$
\sum\limits_{k} f(y_{k})
$$
where $f(y_{k})$ is the cost of an optimal [[Traveling Salesman Problem]] tour for all clients served by truck $k$. We are not able to provide an explicit formulation of the objective function without solving the problem first, since it requires the clients to be assigned already and tours to have been made.

The formulation of the problem would therefore become:
$$
\min_{y_{k}} \sum\limits_{k}f(y_{k})
$$
subject to:
$$
\begin{align}
\text{Capacity constraint: } &\sum\limits_{i}a_{i}y_{ik} \le C_{k}, \qquad \forall k = 1,...,n \\
\text{Degree constraint: } &\sum\limits_{k} y_{ik}
\begin{cases}
K, \quad i = 0 \qquad &\text{Depot} \\
1, \quad\forall i = 1,...,n \qquad &\text{Clients}
\end{cases} \\
& y_{ik} = \{0,1\}, \quad i= 0,...n,\,\, k = 1,...,K
\end{align}
$$
#### Fisher & Jaikumar's Heuristic

To solve the problem in [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/04 - Vehicle Routing problem - MM#CVRP formulation in terms of linear generalised assignment problem\|#CVRP formulation in terms of linear generalised assignment problem]] that we don't know how to write the objective function explicitly, we can try to brute force it to be a linear function, making the problem the following:
$$
\min_{y_{k}} \sum\limits_{k} d_{ik} y_{ik}
$$
subject to:
$$
\begin{align}
\text{Capacity constraint: } &\sum\limits_{i}a_{i}y_{ik} \le C_{k}, \qquad \forall k = 1,...,n \\
\text{Degree constraint: } &\sum\limits_{k} y_{ik}
\begin{cases}
K, \quad i = 0 \qquad &\text{Depot} \\
1, \quad\forall i = 1,...,n \qquad &\text{Clients}
\end{cases} \\
& y_{ik} = \{0,1\}, \quad i= 0,...n,\,\, k = 1,...,K
\end{align}
$$

where the $d_{ik}$ coefficient are estimated as
❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ I don't get how they are estimated
❗❗❗❗❗❗❗❗❗❗❗❗

### CVRP Basic formulation

A basic formulation of the [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/04 - Vehicle Routing problem - MM\|CVRP]] is the following:
$$
\min \sum\limits_{i \in V} \sum\limits_{j\in V} c_{ij}x_{ij}
$$
Subject to:
$$
\begin{align}
\text{Clients degree constraints: } 
&\begin{cases}
\sum\limits_{i\in V} x_{ij} = 1 \qquad \forall j \in V \setminus \{0\} \quad\text{entering node } i\\
\sum\limits_{j\in V} x_{ij}= 1 \qquad \forall i \in V \setminus \{0\} \quad\text{exiting node } i
\end{cases} \\\\
\text{Depot degree constraints: } 
&\begin{cases}
\sum\limits_{i\in V} x_{i0} = K &\quad\text{enterint depot }\\
\sum\limits_{j\in V} x_{0j}= 0  &\quad\text{exiting depot}
\end{cases}
\\
\end{align}
$$

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗ The problem formulation is missing some conditions


