---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/mobility-modeling/lab-ampl/lab-1-introduction-to-ampl/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Mobility Modeling/LAB - AMPL/Lab 1 - Introduction to AMPL\|Lab 1 - Introduction to AMPL]]

AMPL IDE is an environment to run the AMPL system

AMPL is a language to run mathematical optimization programs.

It solves them by means of solvers. They are the ones that do the work. AMPL just manages them giving them a language.

- They are oriented to the development of models commonly used in OR
- The formulations are: understandable to other users and can be easily modified and extended.
- For solving the models, general purpose SOLVERS are used
- Usually there are environments suited for developement/debugging.
- AMPL language is very well suited and featured for complex data structures in large/specialized models
- Other languages: GAMS, CAMPS, L INGO.

AMPL is thought to shorten the time of developing mathematical problems.

## Knapsack problem

In the knapsack problem, **you need to pack a set of items, with given values and sizes (such as weights or volumes), into a container with a maximum capacity** . If the total size of the items exceeds the capacity, you can't pack them all.

Let
- $x_{i} =$ # of pieces of type $i$
- $c_{i}=$ unit value of piece of type $i$
- $b =$ volume of the knapsack
- $a_{i} =$ volume of unit of piece $i$
- $u_{i}=$ max number of units of type $i$ available

![Schermata 2024-10-10 alle 17.20.15.png](/img/user/Schermata%202024-10-10%20alle%2017.20.15.png)

We want to maximaze the value we steal.
$$
\max_{x}\sum\limits_{i=1}^{n} c_{i}x_{i}
$$
There are constrains (s.a):
$$
\begin{align}
\sum\limits_{i=1}^{n} a_{i}x_{i} &\le b \\
0 \le x_{i} &\le u_{i}, \quad i = 1,2,...,n
\end{align}
$$

The more valuable pieces are the ones with higher ratio: $\dfrac{c_{i}}{a_{i}}$.

I can fill the pack of volume $b$ completely if I accept item can be taken in pieces.

If I define what $i$ is in a set called $P$, I can reformulate the problem as:
$$
\max_{x}\sum\limits_{i=1}^{n} c_{i}x_{i}
$$
with constrains
$$
\begin{align}
\sum\limits_{i=1}^{n} a_{i}x_{i} &\le b \\
0 \le x_{i} &\le u_{i}, \quad i \in P
\end{align}
$$

The problem can also be written in matrix form:
$$
\max_{x} c^{T}x
$$
with constrains
$$
\begin{align}
a^{T}x \le b \\
0\le x\le u
\end{align}
$$


### The .mod file

The mod file defines the structure of the problem. It defines what everything is: like P is a set, a is a parameter... It doesn't assign values.

![Schermata 2024-10-10 alle 17.26.34.png](/img/user/Schermata%202024-10-10%20alle%2017.26.34.png)

- .mod files - contain description. Everything we write

I define the parameters:

```AMPL
set P;
param a {j in P};
param b;
param c {j in P};
param u {j in P};

# I define a variable x
var X {j in P}

# I define the objective function
maxiaze beneficio: sum {j in P} c[j] * X[j]

# I define the constrains
subject to tiempo: sum {j in P} a[j] * X[j]<=b;
subject to Limites {j in P}: 0 <= X[j] <= u[j];

```

```ad-note

Capital letters matter. Names are case sensitive.

```



### The .dat file

.dat files - contain the data that has to be compatible with the .mod file

It has to be consistent with what is in the .mod file.

![Schermata 2024-10-10 alle 17.42.07.png](/img/user/Schermata%202024-10-10%20alle%2017.42.07.png)

the aboves are two possible formats.

we define the set P with indexes "bandas" and "bobinas".

Then we assign values to the parameters.

a ha value 200 for "bandas" and 140 for "bobinas".


### Execute

MsDoJ

open AMPL

AMPLE > get mod with command - `ampl: model <fileName>.mod`
AMPLE > get data with dat command - `ampl: data <fileName>.dat`
AMPLE > solve

We can work in 2 ways:
- IDE system - Amplide
- Terminal
- sw.exe to create a command window

There are 4 solvers in our systems:
- [[gurobi\|gurobi]] - Integer and linear programming
- [[cplex\|cplex]] - Integer and linear programming
- [[minos\|minos]] - Non linear programming
- ??? - Non linear programming


### Understanding a model we don't know

If we're given a model of which we don't know the content, there are some commands that can help:
- `show` - shows the parameters
- `display <what To display>` - shows value of variables
- `expand` - Tells me what is loaded in memory


## minCost example

### minCost.mod

Translates a graph. $G = (N,A)$ 
- N: Ciudades (cities)
- A: Arcos (arcs)

$$
A \in N\times N
$$
This is said as: `set ARCOS within (CIUDADES cross CIUDADES);`
- This "within" tells that the arcs are included in the set of all possible arcs between all possible cities.

For network flow problems we don't use `var` and `subject to` for the flow variables and constrains.
We use 2 new commands:
- `arc` (equivalent to `var`)
- `node` (equivalent to `subject to`)

$$
x_{ij}, \quad (i,j) \in A
$$
is written as: `node Nodo {k in CIUDADES}: net_in = domanda[k]-oferta[k]`
The part in the write tells that $i \in N$.

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗
