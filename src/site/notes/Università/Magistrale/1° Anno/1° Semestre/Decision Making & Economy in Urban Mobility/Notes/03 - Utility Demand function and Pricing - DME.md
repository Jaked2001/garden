---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/decision-making-and-economy-in-urban-mobility/notes/03-utility-demand-function-and-pricing-dme/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/03 - Utility Demand function and Pricing - DME\|03 - Utility Demand function and Pricing - DME]]
```table-of-contents
```

%%
[[2024-11-08]]
%%

```ad-tip
title: Assumption - Consumer economically rational

In the following discussion, we will assume the costumer to be **economically rational**:

The costumer will always try to *maximize*:
- Consumption
- Utililazation

```

## Utility function

Let $\mathbf{X}$ be the set of goods that an economy can produce:
$$
\mathbf{X} = \{ x_{1}, x_{2}, ..., x_{n} \}
$$
For simplicity, in this chapter we will work with only 2 goods:
$$
\mathbf{X} = \{ x_{1},x_{2} \}
$$
We can visualize this in the following graph:

![03 - Utility Demand function and Pricing - DME 2024-12-01 12.04.09.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2012.04.09.excalidraw.png)
%%[[03 - Utility Demand function and Pricing - DME 2024-12-01 12.04.09.excalidraw|🖋 Edit in Excalidraw]]%%

The area under the graph is the set of all possible combination of $x_{1}$ and $x_{2}$.

The utility function is defined as follows:

```ad-Definizione
title: Utility function ($u$)

The **utility function**, is a function $u$:
$
u: \mathbb{R}^{2} \to \mathbb{R}
$
such that $\forall (x_{1},x_{2}), (y_{1},y_{2}) \in \mathbf{X}$, if $(x_{1},x_{2})$ is chosen over $(y_{1},y_{2})$, then $u(x1,x_{2}) > u(y_{1},y_{2})$.

```

It's a particular function. We are not as much interested in the absolute value of the function as much as we are in the relative value. We don't really care how much $u(x_{1},x_{2})$ or $u(y_{1},y_{2})$ are, but more if  $u(x_{1},x_{2}) >u(y_{1},y_{2})$.

### Properties of the utility function

The [[#Utility function]] is **continuous**

The [[#Utility function]] is **monotonically increasing** on every single variable:
$$
\frac{\partial u}{\partial x_{i}} \ge 0 \qquad \forall i
$$

The second derivative exists and is always negative or equal to 0 (the function is **cuasi-convex**):
$$
\frac{\partial^{2} u}{\partial x_{i}^{2}} \le 0 \qquad \forall i
$$

The [[#Utility function]], calculated in the empty set (in $(0,0)$) is equal to 0:
$$
u(0,0) = 0
$$
### Types of utility function

#### Cobb-Douglas utility function

![Cobb-Douglas utility function - 03 - Utility Demand function and Pricing - DME 2024-12-01 12.14.18.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Cobb-Douglas%20utility%20function%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2012.14.18.excalidraw.png)
%%[[Cobb-Douglas utility function - 03 - Utility Demand function and Pricing - DME 2024-12-01 12.14.18.excalidraw|🖋 Edit in Excalidraw]]%%

The Cobb-Douglas utility function has the following value:
$$
u(x_{1},x_{2}) = x_{1}^{a}x_{2}^{b}
$$
where
- $a,b:$ are positive coefficients that measure the consumer preferences.

#### Quasilinear utility function

![Quasilinear Utility Function - 03 - Utility Demand function and Pricing - DME 2024-12-01 12.16.27.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Quasilinear%20Utility%20Function%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2012.16.27.excalidraw.png)
%%[[Quasilinear Utility Function - 03 - Utility Demand function and Pricing - DME 2024-12-01 12.16.27.excalidraw|🖋 Edit in Excalidraw]]%%

The **Quasilinear** utility function has the following expression:
$$
u(x_{1},x_{2}) = \nu(x_{1}) + x_{2}
$$
where:
- $\nu(x_{1}) = \sqrt{x_{1}}$ or $\nu(x_{1}) = \ln{(x_{2})}$

#### Linear utility function

The **linear** [[#Utility function]] is works well for [[#Perfectly substitutive goods]]:
$$
u(x_{1},x_{2}) = ax_{1} + bx_{2}
$$
where:
- $a,b > 0$

#### Other utility function

The **other** [[#Utility function]] works well for [[#Perfectly complementary goods]].
$$
u(x_{1},x_{2}) = \min\{ax_{1}, bx_{2}\}
$$
where:
- $a,b > 0$

### Indifference curve

```ad-Definizione
title: Indifference curve

The **indifference curve** is the locus of points $(x_{1},x_{2})$ where the [[#Utility function]] remains equal

```

### Budget constrain

Let
- $m:$ the total budget available
- $p_{1},p_{2}:$ Respectively the unit prices of goods 1 and 2
Then
$$
p_{1}x_{1}+p_{2}x_{2}\le m
$$

%%
[[2024-11-13]]
%%
### Theory of election
,
What combination $(x_{1},x_{2})$ will the consumer choose?

Reminding that the consumer is rational, we have an optimization problem:
$$
\max_{(x_{1},x_{2})} u(x_{1},x_{2})
$$
subject to:
$$
p_{1}x_{1}+p_{2}x_{2} \le m
$$

![03 - Utility Demand function and Pricing - DME 2024-12-01 12.29.47.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2012.29.47.excalidraw.png)
%%[[03 - Utility Demand function and Pricing - DME 2024-12-01 12.29.47.excalidraw|🖋 Edit in Excalidraw]]%%

The solution to the problem is given by the utility such that the iso-utility curve is tangent to the constraint, in the tangent point:
$$
(x_{1}^{*},x_{2}^{*})
$$

#### Relation of Marginal Substitution

![03 - Utility Demand function and Pricing - DME 2024-12-01 12.47.59.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2012.47.59.excalidraw.png)
%%[[03 - Utility Demand function and Pricing - DME 2024-12-01 12.47.59.excalidraw|🖋 Edit in Excalidraw]]%%

```ad-Teo
title: Teorema

In order to maintain the [[#Utility function]] constant, the ratio between the production of good 1 and good 2 needs to be equal to the **Relation of Marginal Substitution**:
$
RMS = - \frac{p_{1}}{p_{2}}
$
___
**Proof:**
Keeping $u(x_{1},x_{2})$ constant can be written as forcing its [[Differential\|Differential]] equal to 0:
$
\begin{align}
{\rm d}u &\stackrel{!}{=}0 \\
{\rm d}u &= \frac{\partial u}{\partial x_{1}}{\rm d}x_{1} + \frac{\partial u}{\partial x_{2}} {\rm d}x_{2} \stackrel{!}{=} 0
\end{align}
$
From this we can write:
$
\frac{{\rm d}x_{1}}{{\rm d}x_{2}} =- \frac{ \frac{\partial u}{\partial x_{2}} }{ \frac{\partial u}{\partial x_{1}} } \stackrel{\triangle}{=} RMS
$
Notice that, in the optimum point, the ratio $\dfrac{{\rm d}x_{1}}{{\rm d}x_{2}}$ must be equal to the slope of the budget $-\dfrac{p_{1}}{p_{2}}$
*q.e.d.*
```

#### Particular cases

##### Perfectly substitutive goods

```ad-Definizione
title: Perfectly substitutive goods

Two goods are **perfectly substitutive** when the consumer is willing to substitute one goods for an other with no change with a 1:1 ratio:

![Perfectly substitutive goods - 03 - Utility Demand function and Pricing - DME 2024-12-01 13.00.14.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Perfectly%20substitutive%20goods%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2013.00.14.excalidraw.png)


The arrow represents the direction in which the [[#Utility function]] increases

```

In this case, the utility function is well represented by a [[#Linear utility function]]

##### Perfectly complementary goods


```ad-Definizione
title: Perfectly complementary goods

Two goods are **perfectly complementary** if both are always consumed using fixed proportions.

![Perfectly complementary goods - 03 - Utility Demand function and Pricing - DME 2024-12-01 13.09.32.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Perfectly%20complementary%20goods%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2013.09.32.excalidraw.png)


The arrow represents the direction in which the [[#Utility function]] increases

```

In this case the [[#Utility function]] is well represented by the [[#Other utility function]].

##### Undesirable goods
 
```ad-Definizione
title: Undesirable good

A good is considered undesirable when the consumer does not accept it.

If $x_{2}$ is the undesirable goods, the [[#Utility function]] grows in the direction of decreasing $x_{2}$ and increasing $x_{1}$.

![Undesirable good - 03 - Utility Demand function and Pricing - DME 2024-12-01 13.12.39.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Undesirable%20good%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2013.12.39.excalidraw.png)


The arrow represents the direction in which the [[#Utility function]] increases

```

## Demand function

```ad-Definizione
title: Demand Function

A **demand function** ($x_{i}$) is a function that tells how much of a good the customers want:
$
x_{i} = f(p_{i}, p_{j}, m)
$
where:
- $x_{i}:$ Demand of good $i$
- $p_{i}:$ Price of good $i$
- $p_{j}:$ Price of good different than $i$
- $m:$ Budget of the buyer (can be seen as costumer's income)


```

The demand has different patterns depending on the type of good:

![Types of demand functions - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.07.30.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Types%20of%20demand%20functions%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.07.30.excalidraw.png)
%%[[Types of demand functions - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.07.30.excalidraw|🖋 Edit in Excalidraw]]%%

As a function of prices, usually demand decreases as price increases

![03 - Utility Demand function and Pricing - DME 2024-12-01 16.12.21.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.12.21.excalidraw.png)
%%[[03 - Utility Demand function and Pricing - DME 2024-12-01 16.12.21.excalidraw|🖋 Edit in Excalidraw]]%%


### Griffen goods

**Giffen goods** are goods that, for some reason, have a demand that increases as price increases. This happens for example with some items during emergencies, when there is scarcity (remember face masks during covid).

![Giffen goods - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.14.28.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Giffen%20goods%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.14.28.excalidraw.png)
%%[[Giffen goods - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.14.28.excalidraw|🖋 Edit in Excalidraw]]%%


### Elasticity

In general, finding the [[#Demand function]] is quite difficult. Often times though, we are not really interested in knowing the full demand, but we can work at the local level. We maybe just need to know how the demand varies when changing the several factors. This introduces the concept of elasticity.

```ad-Definizione
title: Demand elasticity ($\varepsilon_{p}$)

Let a demand be $q = f(p)$.
Elasticity is defined as:
$
\varepsilon_{p} = \lim_{\Delta p \to 0} \frac{\frac{\Delta q}{q}}{\frac{\Delta p}{p}} = \frac{p}{q} \frac{\partial q}{\partial p}
$
Elasticity is the ratio between percentage change of demand and price. It tells us how much the demand varies, for a given variation in price (see also [[Università/Triennale/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/06. Teoria Elementare della domanda e dell'offerta#Elasticità della domanda\|Elasticità della domadna]]).


```

#### Types of elasticity

##### Perfectly elastic demand

```ad-Definizione
title: Perfectly elastic demand

![Perfectly elastic demand - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.25.48.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Perfectly%20elastic%20demand%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.25.48.excalidraw.png)


A perfectly elastic demand is one where [[#Elasticity]] is infinite:
$
\varepsilon_{p} = \infty
$
This means that, even the slightest change in price will make the demand completely different. Really, what it means is that, even keeping the price constant, makes the demand change freely.

```


##### Elastic demand

```ad-Definizione
title: Elastic demand

![Elastic demand - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.28.16.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Elastic%20demand%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.28.16.excalidraw.png)


An **elastic demand** is one where the demand is sensitive to the price. Changing the price strongly affects the demand
$
1<\varepsilon_{p} < \infty 
$


```

##### Perfectly inelastic demand


```ad-Definizione
title: Perfectly inelastic demand


![Perfectly inelastic demand - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.29.48.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Perfectly%20inelastic%20demand%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.29.48.excalidraw.png)


A **perfectly inelastic demand** is one where for any change in price, the demand stays constant
$
\varepsilon_{p} = 0
$

```

##### Inelastic demand


```ad-Definizione
title: Inelastic demand

![Inelastic demand - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.32.36.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Inelastic%20demand%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.32.36.excalidraw.png)


An **inelastic demand** is one where even big change in prices, only cause small changes in demand.
$
0 <\varepsilon_{p} < 1
$

```

##### Unitary elasticity

```ad-Definizione
title: Unitary elasticity

![Unitary elasticity - 03 - Utility Demand function and Pricing - DME 2024-12-01 16.34.19.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/Unitary%20elasticity%20-%2003%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2016.34.19.excalidraw.png)


A demand with **unitary elasticity** is one where for any percentage change in price, the demand changes of the same percentage.
$
\varepsilon_{p} = 1
$

```

# Theory of pricing


## Social Welfare

Social Welfare is defined as the sum of [[#Consumer surplus]] and [[#Producer surplus]]

Let's imagine we have the following situation:
- A demand ($q$) that increases with the reducing in price
- A supply ($s$) that increases with increase in price
The intersection of the 2 is an equilibrium point, called **equilibrium price**.

![03 - Utility Demand function and Pricing - DME 2024-12-01 17.04.35.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2017.04.35.excalidraw.png)


The equilibrium point is how much the costumer/consumer is pays in the current state of the market (with demand $q$ and supply $s$).

Notice that, if the producer were to increase the supply, the price would increase. Same if the demand increased. This means that, in reality, the consumer is willing to pay more than $p_{E}$. The consumer would pay any price indicated by the demand curve $q$. 

### Consumer surplus

The consumer surplus is the cumulative amount that all the consumers are still willing to pay given the current market conditions. It's what they're willing to pay **on top** of what they're paying currently.

In the graph, the consumer suprlus can be seen as the area indicated in orange:

![03 - Utility Demand function and Pricing - DME 2024-12-01 17.10.37.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2017.10.37.excalidraw.png)


### Producer surplus

The producer surplus is the amount of supply that the producer is still willing to provide.

In the graph, is the area in green

![03 - Utility Demand function and Pricing - DME 2024-12-01 17.14.21.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2017.14.21.excalidraw.png)



### Cost, value, price

Let $g$ be the **generalized social cost** (assuming no externalities):
$$
g = p + c_{u}
$$
where:
- $p:$ price
- $c_{u}:$ cost (time) of user

From the user prospective we have:

![03 - Utility Demand function and Pricing - DME 2024-12-01 19.40.37.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2019.40.37.excalidraw.png)


Then, the price costumers are willing to pay at $q_{1}$ is the area in blue:
$$
\int_{0}^{q_{1}} g(z) \, dz
$$
We can then define:

[[#Consumer surplus]]:
$$
{\color{red} CS } = {\color{blue} \int_{0}^{q_{1}} \left(g(z) \, dz \right)} - ({\color{green} p_{1}}+ {\color{orange}c_{u}})q_{1}
$$
CS = Willing to pay - cash - trip time


While, from the producer prospective:

![03 - Utility Demand function and Pricing - DME 2024-12-01 19.50.22.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Decision%20Making%20&%20Economy%20in%20Urban%20Mobility/Notes/Allegati/03%20-%20Utility%20Demand%20function%20and%20Pricing%20-%20DME%202024-12-01%2019.50.22.excalidraw.png)


In the graph we have:
The curve $q$ is the demand for a transportation service. Let's imagine we're working with $q_{1}$ users.

The <mark style="background: #ADCCFFA6;">blue area</mark> is how much the costumers are cumulatively willing to pay.

The generalized cost for the user will be $g_{1}$
$$
{\color{red} g_{1}} = p_{1} + {\color{orange} c_{u}}
$$
The generalized cost for the user is the sum of the price ($p_{1}$) and all the other external costs (specifically time, $c_{u}$).

If it costs the producer $\color{green} c$ to provide the service, $p_{1} - \color{green} c$ will be the producer's revenue and the corresponding <mark style="background: #FF5582A6;">red area</mark> the [[#Producer surplus]].

The **total social** cost will be the sum of the <mark style="background: #FFB86CA6;">orange</mark> and <mark style="background: #BBFABBA6;">green</mark> areas.
While the **net social benefit** will be the <mark style="background: #ADCCFFA6;">willing to pay</mark> - social cost.

### Pricing principles in transportation

Remember that the [[#Social Welfare]] is:
$$
SW = CS + PS
$$
The Consumer Surplus is an average cost that mainly depends on the number of users ($q$) and the size of the infrastructure ($k$):
$$
c_{u}(q,k)
$$

The Producer Surplus will depend on:
- $r(k):$ Annual fix cost of the infrastructure
- $C'(q):$ Operating and maintenance costs
- $C^{0}(q):$ Operative cost of vehicles
For simplicity:
$$
C'(q) = c'q \qquad C^{0}(q) = c^{0}q
$$
Then, the [[#Producer surplus]] is the sum:
$$
\begin{align}
PS &=  C^{0}(q) + C'(q) + r(k)k= \\
&= \underbrace{pq}_{\text{income}} \underbrace{- c^{0}q - c'q -  r(k)k}_{\text{TOT annual costs}}
\end{align}
$$
#### Maximizing the social welfare

In general, with transportation, we're interested in maximising the [[#Social Welfare]]:
$$
\max_{q,k} SW(q,x)
$$
Where the SW:
$$
SW(q,x) = CS(q,k) + PS(q,k)
$$
This, according to what has been said before, can be written as:
$$
\begin{align}
SW(q,x) &= CS(q,k) + PS(q,k) =  \\
&=  \int_{0}^{q_{1}} \left(g(z) \, dz \right) - c_{u}(q,k)q - c^{0}q - c'q -  r(k)k
\end{align}
$$
where notice that, the term $-pq$ for the PS is already in the CS. We don't have to count this twice (this is clearer looking at the graph)
$$
SW(q,x) =  \int_{0}^{q_{1}} \left(g(z) \, dz \right) - c_{u}(q,k)q - c^{0}q - c'q -  r(k)k
$$
To maximize this function, we calculate the first derivatives (in $q$ and $k$) and impose it equal to 0:
$$
\begin{align}
\frac{\partial}{\partial q} SW(q,x) = g(q)  - c_{u}(q,k) - \frac{\partial c_{u}(q,k)}{\partial q}q - c^{0} - c' &\stackrel{!}{=} 0  \quad \longrightarrow \quad q^{*} \qquad [1]\\
\frac{\partial}{\partial k} SW(q,x) = - q \frac{\partial c_{u}(q,k)}{\partial k} - r(k) - \frac{\partial r(k)}{\partial k}k &\stackrel{!}{=} 0 \quad \longrightarrow \quad k^{*} \qquad [2]
\end{align}
$$
Now, $[1]$ can be written as:
$$
g(q^{*}) = c_{u}(q^{*},k) + \left.\frac{\partial c_{u}(q,k)}{\partial q}\right|_{q^{*}} q^{*} + c^{0} + c' 
$$
And, remembering the definition of generalized cost:
$$
g = p + c_{u}(q,k)
$$
we can write:
$$
 \cancel{c_{u}(q,k)} + \underbrace{\frac{\partial c_{u}(q,k)}{\partial q}}_{\text{Social Marginal cost}} q + c^{0} + c'  = p + \cancel{c_{u}(q,k)}
$$
So:
$$
p = c^{0} + c' + q^{*} \left.\frac{\partial c_{u}}{\partial q} \right|_{q^{*},k^{*}}
$$

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

### Pricing without congestion

