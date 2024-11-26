---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/mobility-modeling/notes/02-traffic-assignment-problem-mm/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/02 - Traffic Assignment Problem - MM\|02 - Traffic Assignment Problem - MM]]

## Wardrop's equilibrium principle

We work under the following assumptions:
- Users are **rational** and **selfish** individuals. They try to maximize their individual utilities
- Users have **perfect information** on network conditions
- Operational conditions on the network are stable during the period of time under analysis

```ad-Teo
title: Wardrop's equilibrium principle
In a transportation network, to go from origin $p$ to destination $q$, travelers choose their routes unilaterally and flows split between different available routes $p \to q$, in a way such that, if a traveller would commute to another route, its own O-D trip time would be worse, while other users, also from $p \to q$, would benefit from this decision.
```

Consequently, travelers choose their routes such that all the chosen options result in a unique and minimum travel cost $c_{pq}$. Non-used routes from $p \to q$ all have a travel cost $c \ge c_{pq}$.

This means that each user decides what route has the lowest cost for themselves. In the end, the total cost of the network will not be the minimum possible, but each user will have chosen their routes to minimize their own cost at the moment they chose the route.

### Wardrop's equilibrium principle example

It is considered useful to visualize the problem through an example.

The simple network below is given:

![02 - Traffic Assignment Problem - MM 2024-11-24 11.50.51.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/02%20-%20Traffic%20Assignment%20Problem%20-%20MM%202024-11-24%2011.50.51.excalidraw.png)


There is a demand $T$ to go from node $A$ to node $B$. There are 2 possible paths. The flows of the 2 paths are $v_{1}$ and $v_{2}$.

The flows have to follow the condition:
$$
v_{1}+v_{2} = T \qquad v_{1},v_{2}\ge 0
$$
The [[Volume delay function\|Volume delay functions]] are:
$$
\begin{cases}
s_{1}(v_{1}) = 1+v_{1}^{2} \\
s_{2}(v_{2}) = 2+v_{2}^{2}
\end{cases}
$$
We can try an intuitive visualization of the problem:

![02 - Traffic Assignment Problem - MM 2024-11-24 12.08.01.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Mobility%20Modeling/Notes/Allegati/02%20-%20Traffic%20Assignment%20Problem%20-%20MM%202024-11-24%2012.08.01.excalidraw.png)


The [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/02 - Traffic Assignment Problem - MM#Wardrop's equilibrium principle\|#Wardrop's equilibrium principle]] is reached when both delay function are equal. At that point in fact, the last user could choose link indifferently, as its cost would be the same.
$$
s_{1}(v_{1}^{*}) = s_{2}(v_{2}^{*})
$$
In this case, the condition is met for 
$$
v_{1}^{*} = \frac{17}{8} \qquad v_{2}^{*}= \frac{15}{8}
$$
And
$$
s_{1}(v_{1}^{*}) = s_{2}(v_{2}^{*}) = 5.51
$$
Keep in mind that if this was a [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/01.2 - The minimum cost flow problem - From book - MM\|min-cost flow problem]], the total cost would be lower. but there would be some users with a much higher cost and some with a much lower cost, going against the [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/02 - Traffic Assignment Problem - MM#Wardrop's equilibrium principle\|#Wardrop's equilibrium principle]].

## The traffic assignment problem

The Traffic Assignment Problem (TAP) can be written as follow:

Minimize the total cumulative cost in the network subject to the usual network constraints (those that define the links and the demand). In maths terms:

```ad-Teo
title: Traffic Assignment problem

$
\min_{\mathbf{x}} f(\mathbf{x})
$
subjet to
$
\mathbf{A} \mathbf{x} = \mathbf{b}, \quad \mathbf{x} \ge 0
$
from which we get the solution $\mathbf{\hat{x}}$.

```

The TAP can be solved through the [[Frank-Wolfe Method\|Frank-Wolfe Method]].


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/frank-wolfe-method/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Frank-Wolfe Method\|Frank-Wolfe Method]]

The following problem is given:
$
\min_{\mathbf{x}} f(\mathbf{x})
$
subjet to
$
\mathbf{A} \mathbf{x} = \mathbf{b}, \quad \mathbf{x} \ge 0
$
from which we get the solution $\mathbf{\hat{x}}$.

where:
- $f(\mathbf{x}): \mathbb{R}^{n}\to \mathbb{R}$
- $\mathbf{A}\in \mathbb{R}^{n}\times \mathbb{R}^{n}$
- $\mathbf{x}\in \mathbb{R}^{n}$
- $\mathbf{b}\in \mathbb{R}^{n}$

The Frank-Wolfe is an iterative method to solve the problem with the following steps

## 0. Find a feasible solution

The first step is to find any feasible solution $\mathbf{x}^{(k)}$. In the first iteration, $k=0$.

This solution has to meet the condition $\mathbf{A} \mathbf{x} = \mathbf{b}, \quad \mathbf{x} \ge 0$

## 1. Define the subproblem

The Frank-Wolfe method works generating a new problem, called a subproblem. This is still an optimization problem but is allegedly easier to solve.

In order to define the new problem, we first need to find the [[Gradient\|Gradient]] of $f(\mathbf{x})$. Then, the subproblem is:
$
\min_{\mathbf{y}} \boldsymbol{\nabla f}\left(\mathbf{x}^{(k)} \right)^T \cdot \mathbf{y}
$
subj to:
$
\mathbf{A} \mathbf{y} = \mathbf{b}, \quad \mathbf{y} \ge 0
$
from which we get the value $\mathbf{\hat{y}}$.

### Calculate the descent direction

The, we need to calculate a new vector, called the direction, that will allow us to get the solution for the next step of the algorithm.

$
\mathbf{d}^{(k)} = \mathbf{\hat{y}} - \mathbf{x}^{(k)}
$
## 2. Stopping criteria

We need some sort of stopping criteria to know if the solution $\mathbf{x}^{(k)}$ is close enough to the actual solution $\mathbf{\hat{x}}$ of the original problem.

We calculate a relative gap, $r$ as
$
r = - \frac{\mathbf{\nabla f} \left(\mathbf{x}^{(k)} \right)^{T} \cdot \mathbf{d}^{(k)} }{\mathbf{\nabla f} \left(\mathbf{x}^{(k)} \right)^{T} \cdot \mathbf{x}^{(k)}}
$

We define a relative gap that we find suitable. This is going to be a very small value, $\varepsilon$ ($= 10^{-2}, 10^{-4},...$)

If $r < \varepsilon$ than we stop and accept $\mathbf{x}^{(k)}$ as a solution ($\mathbf{x}^{(k)} \approx \mathbf{\hat{x}}$). Otherwise, we go the next step

## 3. Line search

The new solution will be given by
$
\mathbf{x}^{(k+1)} = \mathbf{x}^{(k)} + \alpha^* \mathbf{d}^{(k)}
$
where $\alpha^{*}$ is the solution to the problem:
$
\min_{0\le\alpha\le 1} h(\alpha ) = \min_{0\le\alpha\le 1} f\left( \mathbf{x}^{(k)} + \alpha \mathbf{d}^{(k)} \right)
$
This can be solved finding the first derivative of $h(\alpha)$, imposing it equal to 0 and then solving for $\alpha$. This last step is often impossible to do analitically, so we rely on numeric methods to find $\alpha^{*}$ (like: [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.2 Il metodo delle Tangenti\|Metodo di Newton]] o [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.2 Il metodo delle Tangenti\|Il metodo delle Tangenti]], [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.1 Metodo di Bisezione\|Metodo di Bisezione]], [[Università/Triennale/2° anno/2° Semestre/Analisi Numerica/Appunti/03.3 Il metodo delle Secanti\|Il metodo delle Secanti]]).

```ad-note

In the particular case that all elements of $\boldsymbol{\nabla} \mathbf{f} \left( \mathbf{x}^{(k)} \right) \stackrel{\triangle}{=} \mathbf{s}(\mathbf{x}^{(k)})$ are in the form $a+bx$, then $\alpha^{*}$ can be taken equal to
$
\min\{1, \tilde{\alpha } \}
$
where:
$
\tilde{\alpha} = \frac{\sum\limits_{i} s_{i}(x_{i}) \cdot d_{i}^{(k)}}{\sum\limits_{i} b_{i}\cdot \left(d_{i}^{(k)}\right)^{2}}
$


```


## 4. Update

After having found $\alpha^{*}$ is time to update the solution to the next step: $\mathbf{x}^{(k)}$ and repeat the method from step [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/02 - Traffic Assignment Problem - MM#0. Find a feasible solution\|#0. Find a feasible solution]]


</div></div>



