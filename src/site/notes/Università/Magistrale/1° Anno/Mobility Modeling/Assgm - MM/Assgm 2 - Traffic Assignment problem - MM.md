---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/mobility-modeling/assgm-mm/assgm-2-traffic-assignment-problem-mm/"}
---


# [[Università/Magistrale/1° Anno/Mobility Modeling/Assgm - MM/Assgm 2 - Traffic Assignment problem - MM\|Assgm 2 - Traffic Assignment problem - MM]]


My parameters: [[Assgm 2 - Parameters - MM.pdf]]

| Name          | ID        | File_XX.jpg | $c_{ij}$ | $d_{ij}$ | O-D Flow | Aug. factor for $c_{ij}$ at red links |
| ------------- | --------- | ----------- | -------- | -------- | -------- | ------------------------------------- |
| Matteo Meloni | ca41844hp | 18          | 2        | 0,1863   | 30       | 2.9430                                |

You are assigned the following network

![Assgm 2 - Traffic Assignment problem - MM 2024-12-08 11.36.44.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Assgm%20-%20MM/Allegati/Assgm%202%20-%20Traffic%20Assignment%20problem%20-%20MM%202024-12-08%2011.36.44.excalidraw.png)


The [[Volume delay function\|Volume delay function]] is the same for each link, and it's equal to:
$$
s_{ij}(x) = c_{ij} + d_{ij}x_{ij}^{2}
$$
where:
- $x:$ is the flow for the given link

According to the assigned parameters, the values are as follows:
- $c_{ij} = 2$
- $d_{ij} = 0,1863$

❗❗ Keep in mind, parameters have different names in the AMPL code...

## What we have to do

Solve a [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/02 - Traffic Assignment Problem - MM\|02 - Traffic Assignment Problem - MM]] using AMPL. 
- Solve the whole problem (Beckmann's problem) minimizing the objective function in the MinCM2.mod file
- Solve implementing the [[Frank-Wolfe Method\|Frank-Wolfe Method]] in the .run file and using solvers only to solve the subproblem

### Beckmann's problem - Assgm 2

Given the volume delay function:
$$
t0_{ij}(v_{ij}) = c_{ij} + {\rm cap}_{ij}v_{ij}^{2}
$$
the Beckmann's problem is
$$
\min_{x_{ij}} \sum\limits_{ij \in A} \int_{0}^{x_{ij}} t0_{ij}(x) \, dx
$$
Subject to
$$
\mathbf{A}\mathbf{v} = \mathbf{b}
$$
where $A$ is the set containing **all** the links in the network

The objective function can be written explicitly:
$$
\begin{align}
\int_{0}^{v_{ij}}  t0_{ij}(x) \, dx &= \int_{0}^{v_{ij}} (c_{ij} + {\rm cap}_{ij}x_{ij}^{2})\, dx \\
&= c_{ij}v_{ij} + \frac{1}{3} {\rm cap}_{ij}v_{ij}^{3}
\end{align}
$$

In AMPL, the Beckmann's problem is problem $Q$:

```AMPL
problem Q: v_k, v, N, flux_total, Vnl; # Traffic Assignment (Equilibrium problem) Definition
```

Which uses:
- $v:$ the link flow vector (what we called $\mathbf{x}$ in problem definition before)
- $N:$ node vector
- $v_{k}:$ flow of commodity $k$ (we have 2 commodities in our case)
- $Vnl:$ Beckmann's problem objective function

The objective function in the .mod file appears as

```AMPL
minimize Vnl: sum { (i,j) in links} (gamma * c[i,j] + cap[i,j] * (1/3) * v[i,j]^3);
```

which corresponds to
$$
\min_{v} {\rm Vnl} = \min_{v} \left(  \gamma  c_{ij} + {\rm cap}_{ij} \frac{1}{3} v_{ij}^{3}  \right)
$$
where:
- $\gamma:$ Augmenting factor for $c_{ij}$ in red links
- $c_{ij}:$ the old $c_{ij}$ parameter
- ${\rm cap}_{ij}:$ the old $d_{ij}$ parameter


### Last question

Pick 4 OD pairs.
For each OD pair, pick 3 paths.

Picked OD pairs and paths:
- (11, 17)
	- (11, 12) (12, 15) (15, 16) (16, 17)
	- (11, 12) (12,13) (13, 17)
	- (11, 12) (12, 15) (15, 13) (13, 17)
- (11, 14)
- (3,)


## The problems in AMPL

![Assgm 2 - Traffic Assignment problem - MM 2024-12-09 15.43.53.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Assgm%20-%20MM/Allegati/Assgm%202%20-%20Traffic%20Assignment%20problem%20-%20MM%202024-12-09%2015.43.53.excalidraw.png)


![Assgm 2 - Traffic Assignment problem - MM 2024-12-11 09.37.19.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Assgm%20-%20MM/Allegati/Assgm%202%20-%20Traffic%20Assignment%20problem%20-%20MM%202024-12-11%2009.37.19.excalidraw.png)


