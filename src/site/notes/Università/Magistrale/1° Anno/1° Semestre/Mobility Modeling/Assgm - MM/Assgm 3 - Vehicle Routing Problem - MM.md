---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/mobility-modeling/assgm-mm/assgm-3-vehicle-routing-problem-mm/"}
---


# [[Università/Magistrale/1° Anno/1° Semestre/Mobility Modeling/Assgm - MM/Assgm 3 - Vehicle Routing Problem - MM\|Assgm 3 - Vehicle Routing Problem - MM]]

Given link $(i,j)$, cost on the link is given by:
$$
c_{ij} = 95 + (x_{i}-x_{j})^{2} + (y_{i}-y_{j})^{2} \qquad \forall (i,j) \in A \cup \hat{A}
$$
where $x_{i}, y_{i}$ are the coordinates of node $i$.

___

**DEPOT:**
Since I have an even ID number (CA41844HP), I will use node A as a depot. This is node with coordinates:
$$
A = (1,4) = 11
$$
also known as node 11.

## Poin 3 - Fisher & Jaikumar's Heuristic

See slide 79 (page 70 in my iPad) for problem definition

.mod file

```
y {CLD cross {1..K}} binary;
subject to cc{k in {1..K}}: sum{j in CLD} a[j]*y{j,k} <= C;

```

.run file

```
let {p in Depot} a[p] := 0;
# Constraint d_iik = \min(...)
```

## Deleted from ample

.dat file
```{AMPL}
param a :=

1 0

2 0

3 0

4 0

5 10

6 0

7 0

8 10

9 0

10 0

11 0

12 10

13 10

14 10

15 0

16 0

17 10

18 10

19 10

20 0

21 10

22 0

23 10

24 0 ;
```


## Ricapitolo i problemi risolti

MTZVRP:
- Vars:
	- x
	- u
- Constrains:
	- nulx
	- degree_in
	- degree_out
	- Degree_con_depot_ent
	- Degree_con_depot_exit
	- u0
	- subtour_breaking
	- lowerBound
	- upperBound
- Objective func:
	- fobj;

```{AMPL}
problem MTZVRP: x, u, nulx, degree_in, degree_out, Degree_con_depot_ent, Degree_con_depot_exit, u0, subtour_breaking, lowerBound, upperBound, fobj;
```


FJ:
- Vars:
	- y
- Constrains:
	- FJcap
	- FJdegree_client
	- FJdegree_depot
- Objective function:
	- FJ_obj;

```{AMPL}
problem FJ: y, FJcap, FJdegree_client, FJdegree_depot, FJ_obj;
```


TSP:
- Vars:
	- x_TSP
	- s
- Constrains
	- TSP_nulx
	- TSP_degree_in
	- TSP_degree_out
	- s0
	- subtour_breaking_TSP
	- TSP_lowerBound
	- TSP_upperBound
- Objective func
	- TSP_obj;


```{AMPL}
problem TSP: x_TSP, s, TSP_nulx, TSP_degree_in, TSP_degree_out, s0, subtour_breaking_TSP, TSP_lowerBound, TSP_upperBound, TSP_obj;
```