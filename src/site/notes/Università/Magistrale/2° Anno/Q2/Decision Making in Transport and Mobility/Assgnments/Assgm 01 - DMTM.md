---
{"dg-publish":true,"permalink":"/universita/magistrale/2-anno/q2/decision-making-in-transport-and-mobility/assgnments/assgm-01-dmtm/"}
---


# [[Università/Magistrale/2° Anno/Q2/Decision Making in Transport and Mobility/Assgnments/Assgm 01 - DMTM\|Assgm 01 - DMTM]]

## Formulating and solving the basic routing problem

### TSP Formulations

#### Miller-Tucker-Zemlin (MTZ)

[[Università/Magistrale/1° Anno/1° Semestre/Mobility Modeling/Notes/Traveling Salesman Problem\|Traveling Salesman Problem]]

$$
\min \sum\limits_{i\in N} \sum\limits_{j \in N} c_{ij}x_{ij}
$$
such that:
- Degree constraints
$$
\begin{align}
\sum\limits_{j \in N} x_{ij} = 1 \quad \forall i \in N \\
\sum\limits_{i \in N} x_{ij} = 1 \quad \forall j \in N
\end{align}
$$
- Subtour breaking constraints:
$$
\begin{align}
u_{i}-u_{j}+nx_{ij} \le n-1 &\quad \forall i,j \in N, i\ne j, \\
2 \le u_{i}\le n &\quad \forall i \in N \setminus \{1\}, \\
u_{1} = 1
\end{align}
$$

$$
x_{ij} \in \{0,1\} \quad \forall i,j \in N
$$
#### Dantzig-Fulkerson-Johnson (DFJ)

$$
\min \sum\limits_{i\in N} \sum\limits_{j \in N} c_{ij}x_{ij}
$$
such that:
- Degree constraints
$$
\begin{align}
\sum\limits_{j \in N} x_{ij} = 1 \quad \forall i \in N \\
\sum\limits_{i \in N} x_{ij} = 1 \quad \forall j \in N
\end{align}
$$
- Subtour breaking constraints:
$$
\sum\limits_{i\in S}\sum\limits_{j\in S} x_{ij} \le |S|-1 \quad \forall S \subset N, |S| \ge 2
$$
$$
x_{ij} \in \{0,1\} \quad \forall i,j \in N
$$


## 2.1 Practical Constraints

### 2.1.a - Add capacity and Time Windows


Decision variables:
- $x_{ij}:$ Binary. 0 = do not use edge, 1 = use edge $(i,j)$
- $u_{i}:$ Amount of goods delivered to node $i$
- $T_{i}:$ Time at which node $i$ is visited
$$
\min \sum\limits_{i\in N} \sum\limits_{j \in N} c_{ij}x_{ij}
$$
such that:
- Degree constraints
$$
\begin{align}
\sum\limits_{j \in N} x_{ij} = 1 \quad \forall i \in N \setminus \{0\} \\
\sum\limits_{i \in N} x_{ij} = 1 \quad \forall j \in N \setminus \{0\}
\end{align}
$$
- Capacity constraints:
$$
\begin{align}
u_{i}-u_{j} + Qx_{ij} \le Q - q_{j}, &\quad \forall i \in N,\, \forall j \in N \setminus \{0\}, i\ne j, \\
q_{j} \le u_{i}\le Q, &\quad \forall i \in N \setminus \{0\}, \\
u_{0} = 0,
\end{align}
$$
- TimeWindows constraints:
$$
\begin{align}
T_{i} + s_{i}+ t_{ij} - T_{j} \le M (1-x_{ij}), &\quad \forall i,j \in N, i\ne j \\
a_{i}\le T_{i}\le b_{i}, &\quad \forall i \in N\\
T_{0} = 0,
\end{align}
$$
$$
x_{ij} \in \{0,1\} \quad \forall i,j \in N
$$

### 2.1.b - Compare to 1.1

### 2.1.c - Minimise number of vehicles

Parameters:
- $c_{ij}:$ Cost of edge $(i,j)$
- $t_{ij} \equiv c_{ij}:$ Time travel on edge $(i,j)$ (We just use $c_{ij}$ in the constraints, because speed is $60 \,\rm{\frac{km}{h}}$)
- $Q:$ Capacity of a vehicle
- $q_{i}:$ Demand of node $i$
- $C:$ Cost of activating a route
Decision variables:
- $x_{ijk}:$ *Binary*. 0 = do not use edge, 1 = use edge $(i,j)$ with vehicle $k$
- $u_{ik}:$ *Continuous*. Amount of goods delivered to node $i$ by vehicle $k$
- $T_{ik}:$ *Continuous*. Time at which node $i$ is visited by vehicle $k$

$$
\min \sum\limits_{k \in K}\sum\limits_{i\in N} \sum\limits_{j \in N} c_{ijk}x_{ijk} + \sum\limits_{k \in K} \left( \left( \sum\limits_{i \in N} \sum\limits_{j \in N} x_{ijk} \right) -1 \right)
$$
such that:
- Degree constraints
$$
\begin{align}
\sum\limits_{j \in N} x_{ijk} = 1 &\quad \forall i \in N \setminus \{0\},\, \forall k \in K \\
\sum\limits_{i \in N} x_{ijk} = 1 &\quad \forall j \in N \setminus \{0\},\, \forall k \in K \\
\sum\limits_{k \in K} x_{ijk} \le 1 &\quad \forall i,j \in N \setminus \{0\}
\end{align}
$$
- Capacity constraints:
$$
\begin{align}
u_{ik}-u_{jk} + Qx_{ijk} \le Q - q_{j}, &\quad \forall i \in N,\, \forall j \in N \setminus \{0\},\, i\ne j,\, \forall k \in K \\
q_{j} \le u_{ik}\le Q, &\quad \forall i \in N \setminus \{0\},\, \forall k \in K \\
u_{0k} = 0, &\quad\forall k \in K
\end{align}
$$
- TimeWindows constraints:
$$
\begin{align}
T_{ik} + s_{i}+ t_{ij} - T_{jk} \le M (1-x_{ijk}), &\quad \forall i,j \in N, i\ne j, \forall k \in K \\
a_{i}\le T_{ik}\le b_{i}, &\quad \forall i \in N, \forall k \in K \\
T_{0k} = 0, &\quad \forall k \in K
\end{align}
$$

$$
x_{ijk} \in \{0,1\} \quad \forall i,j \in N,\, \forall k \in K
$$

