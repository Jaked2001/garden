---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/decision-making-and-economy-in-urban-mobility/notes/01-production-and-cost-functions-in-transport-dme/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME\|01 - Production and cost functions in transport - DME]]

```table-of-contents
```

## Production function

![01 - Production and cost functions in transport - DME 2024-11-04 19.24.54.excalidraw.png](/img/user/Excalidraw-2/01%20-%20Production%20and%20cost%20functions%20in%20transport%20-%20DME%202024-11-04%2019.24.54.excalidraw.png)
%%[[01 - Production and cost functions in transport - DME 2024-11-04 19.24.54.excalidraw.md|🖋 Edit in Excalidraw]]%%

```ad-Definizione
title: Production function ($x$)

The **production function** is the relation between the output (*products*, $x$) and the *Capital* ($K$) and *Labor* ($L$) involved in making that product.

$
x = f(K,L)
$

```

It works under the assumption of **efficient process**: given $K$ and $L$, we have the best output possible.

### Indicators
#### Average Productivity

```ad-Definizione
title: Average productivity

$
P_{av,L} = \frac{x}{L} \qquad P_{av, K} = \frac{x}{K}
$

```

#### Marginal Productivity

```ad-Definizione
title: Marginal Productivity ($P_{ma,L}$,$P_{ma,K}$ )

Marginal productivity is a measure of how many units of input are necessary to increase the output of 1 unit.

$
P_{ma,L} = \frac{\partial x}{\partial L} \qquad P_{ma, K} = \frac{\partial x}{\partial K}
$

```

### Characteristics

Usually, a [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Production function\|#Production function]] tends to have the following characteristics:
- [[#Monotony of a production function|Monotony]]
- [[#Convexity of a production function|Convexity]]

#### Monotony of a production function

```ad-Teo
title: Monotony of the Production function

The [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Production function\|#Production function]] increases when the labor or the capital increases, or, at the very least, it stays constant. It NEVER decreases.
$
\frac{\partial x}{\partial L} \ge 0 \qquad \frac{\partial x}{\partial K} \ge 0 
$
```

#### Convexity of a production function

```ad-Teo
title: Convexity of the [[#Production function]]

The product $X$ grows *slower and slower* as the Labor or the Capital keep increasing.

$
\frac{\partial^{2} x}{\partial^{2} L} = \frac{\partial P_{ma,L}}{\partial L} \le 0 \qquad \frac{\partial^{2} x}{\partial^{2} K} = \frac{\partial P_{ma,K}}{\partial K} \le 0
$

```

### Iso-production curves

They show what are the admissible combinations of labor and capital for a given value of the [[#Production function]].

![Iso-production curves - 01 - Production and cost functions in transport - DME 2024-11-04 19.45.12.excalidraw.png](/img/user/Excalidraw-2/Iso-production%20curves%20-%2001%20-%20Production%20and%20cost%20functions%20in%20transport%20-%20DME%202024-11-04%2019.45.12.excalidraw.png)
%%[[Iso-production curves - 01 - Production and cost functions in transport - DME 2024-11-04 19.45.12.excalidraw|🖋 Edit in Excalidraw]]%%

### Diminishing return law

Assuming a production function $x=f(K,L)$, if $ΔL$ (or $Δk$) and $K$ is constant (or $L$), then productivity increases proportionally more than the productive factor until at a level upon which the productivity diminishes.

![Schermata 2024-11-04 alle 20.55.51.png](/img/user/Schermata%202024-11-04%20alle%2020.55.51.png)

### Return to scale

Return to scale is the concept of relating how fast the [[#Production function]] increases with the increase of the inputs:
- [[#Increasing return to scale]]
- [[#Constant return to scale]]
- [[#Reducing return to scale]]


#### Increasing return to scale

We have an **increasing return to scale** when the [[#Production function]] increases *more than proportionally* with the inputs.

- [x] Does that means that $x$ increases more than linearly? How can a function grow more than linearly and still be convex? ✅ 2024-11-29
	- [ ] Yes, but not indefinitly. For example, $\ln(x)$ grows quicker than $x$ up to a point.

Keeping in mind that the production function is [[Homogenous Function]] (like the cost function), we have in creasing return to scale if:
$$
x = f(\lambda K, \lambda L) = \lambda ^{s} f(K,L) \qquad s>1
$$

#### Constant return to scale

We have a **constant return to scale** when the [[#Production function]] increases *proportionally* with the inputs.

#### Reducing return to scale

We have a **reducing return to scale** when the [[#Production function]] increases *less than proportionally* with the inputs.

### Types of production function

There are a few [[#Iso-production curves]] that are often used in the field:
- [[#Cobb-Douglas]]
- [[#Leontief]]

#### Cobb-Douglas

![Cobb-Douglas - 01 - Production and cost functions in transport - DME 2024-11-04 21.04.33.excalidraw.png](/img/user/Excalidraw-2/Cobb-Douglas%20-%2001%20-%20Production%20and%20cost%20functions%20in%20transport%20-%20DME%202024-11-04%2021.04.33.excalidraw.png)
%%[[Cobb-Douglas - 01 - Production and cost functions in transport - DME 2024-11-04 21.04.33.excalidraw|🖋 Edit in Excalidraw]]%%

The **Cobb-Douglas** [[#Iso-production curves]] has the following equation for the [[#Production function]]
$$
f(K,L) = x = K^{a}L^{b}
$$
where:
- $a,b:$ are 2 parameters

The Cobb-Douglas function can be written linearly:
$$
\begin{align}
x &= K^{a}L^{b} =  \\
\underbrace{\ln(x)}_{\hat{x}} &= a\underbrace{\ln(K)}_{\hat{K}} + b\underbrace{\ln(L)}_{\hat{L}} = \\
\hat{x} &= a \hat{K} + b \hat{L}
\end{align}
$$
In the Cobb-Douglas function, the [[#Return to scale]] is:
$$
RTS = - \frac{a}{b} \frac{L}{K}
$$

#### Leontief

![Leontief - 01 - Production and cost functions in transport - DME 2024-11-04 21.04.56.excalidraw.png](/img/user/Excalidraw-2/Leontief%20-%2001%20-%20Production%20and%20cost%20functions%20in%20transport%20-%20DME%202024-11-04%2021.04.56.excalidraw.png)
%%[[Leontief - 01 - Production and cost functions in transport - DME 2024-11-04 21.04.56.excalidraw|🖋 Edit in Excalidraw]]%%

The **Leontief** [[#Production function]] is often used for its simplicity:
$$
f(K,L) = x = \min{(aL,bK)}
$$

### Technical Substitution Relation (TSR)

- [?] I don't understand what Technical substitution relation is? 

The [[#Iso-production curves|iso-production curve]] below is given:

![Schermata 2024-11-04 alle 21.09.53.png](/img/user/Schermata%202024-11-04%20alle%2021.09.53.png)

By definition, along the curve, $x$ is constant, meaning its differential, ${\rm d} x =0$.
The differential of $x$ is defined as follows:
$$
{\rm d}x = \frac{\partial x}{\partial K}{\rm d}K + \frac{\partial x}{\partial L}{\rm d}L = 0
$$
meaning we can write:
$$
-\frac{{\rm d}K}{{\rm d}L} = \frac{ \frac{\partial x}{\partial L} }{ \frac{\partial x}{\partial K} }
$$
where, at the second member, we recognise the [[#Marginal Productivity|marginal productivities]]:
$$
-\frac{{\rm d}K}{{\rm d}L} = \frac{ P_{ma,L} }{ P_{ma, K} }
$$
This last quantity is defined as **Technical Substitution Relation**

```ad-Definizione
title: Technical Substitution Relation ($TSR$)

**Technical Substitution Relation** ($TSR$) is defined as the ratio of the marginal costs of the production factors (Labor and Kapital).
$
TSR = -\frac{{\rm d}K}{{\rm d}L} = \frac{ P_{ma,L} }{ P_{ma, K} }
$

```


## Cost Function

[[01 - Production and cost functions in transport - DME]]

```ad-Definizione
title: Cost function ($CT$)

The **Cost Function**, or Total cost ($CT$) is the relation
$
CT(x,w,r) = wL+rK
$
where:
- $L,K:$ number of productive factors
- $r,w:$ unitary cost of the productive factors

```

We work under the assumption that we have the **minimum** cost for producing $x$.

### Indicators

#### Average cost

```ad-Definizione
title: Average Cost ($C_{av}$)
$
C_{av} = \frac{CT}{x}
$

```

#### Marginal cost

```ad-Definizione
title: Marginal Cost ($C_{ma}$)
$
C_{ma} = \frac{\partial CT}{\partial x}
$

```

### Properties of the cost function

#### ???

```ad-Teo
title: Teorema

There is **no** diminishing with unitary cost of the productive factors

```

- [x] What does this mean? ✅ 2024-11-29
	- [ ] It's a positive function...

#### Homogeneity of the cost function

```ad-Teo
title: Homogeneity

The [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Cost Function\|#Cost Function]] is [[Homogenous Function\|homogeneous]] of first grade in $r$ and $w$.

```

#### Convexity of the cost function

```ad-Teo
title: Convexity

The [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Cost Function\|#Cost Function]] is **convex** in $w$.
```

#### Continuity of the cost function

```ad-Teo
title: Continuity

The [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Cost Function\|#Cost Function]] is **continous** in $w$ for $w\ge 0$.

```

### Fixed and variable costs

The total cost can be divided into the following sum:
$$
CT = CF + CV
$$
where
- $CF:$ [[#Fixed cost]]
- $CV:$ [[#Variable cost]]

#### Fixed cost

```ad-Definizione
title: Fixed cost

**Fixed costs** ($CF$) are costs that do not change in a given system. They can only be defined in the [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Short term cost function\|#Short term cost function]].

```

#### Variable cost

```ad-Definizione
title: 

**Variable costs** ($CV$) are costs dependent on the [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Production function\|production]] of a system.

They exist both in the [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Short term cost function\|#Short term cost function]] and the [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Long term cost function\|#Long term cost function]].
```
 
### Short term and long term

#### Short term cost function

In the short term, the [[#Cost Function]] is given by the sum of the [[#Variable cost]] and the [[#Fixed cost]]:

![Short term cost function - 01 - Production and cost functions in transport - DME 2024-11-05 12.10.50.excalidraw.png](/img/user/Excalidraw-2/Short%20term%20cost%20function%20-%2001%20-%20Production%20and%20cost%20functions%20in%20transport%20-%20DME%202024-11-05%2012.10.50.excalidraw.png)
%%[[Short term cost function - 01 - Production and cost functions in transport - DME 2024-11-05 12.10.50.excalidraw|🖋 Edit in Excalidraw]]%%

The graph specifically shows the sum of the <mark style="background: #BBFABBA6;">Average Fixed cost</mark> and the <mark style="background: #FF5582A6;">Average Variable cost</mark> to give, in <mark style="background: #ADCCFFA6;">blue</mark>, the [[#Average cost]].

#### Long term cost function

In the long term, even the [[#Fixed cost]] can change. Therefore, there are not [[#Fixed cost]] in the Long term cost function, only [[#Variable cost]].

The long term cost function can be obtained overlapping all the [[#Short term cost function]] at different sizes of the system:

![Long term cost function - 01 - Production and cost functions in transport - DME 2024-11-05 12.25.46.excalidraw.png](/img/user/Excalidraw-2/Long%20term%20cost%20function%20-%2001%20-%20Production%20and%20cost%20functions%20in%20transport%20-%20DME%202024-11-05%2012.25.46.excalidraw.png)
%%[[Long term cost function - 01 - Production and cost functions in transport - DME 2024-11-05 12.25.46.excalidraw|🖋 Edit in Excalidraw]]%%

Each $x_{i}^{*}$ is the optimal production in the [[#Short term cost function|short term]], at the given system size. All the $x_{i}^{*}$ give the long term cost function. For a business, the optimal size is that that minimizes the long term cost function.


## Efficiency

```ad-Definizione
title: Efficiency

**Efficiency** is the condition where we get the maximum output for a fixed numer of *productive factors*.

```

#### Types of efficiency

We can define efficiency based on different things:
- [[#Technical efficiency]]
- [[#Efficiency of market assignation]]
- [[#Social efficiency]]
- [[#Efficiency of scale]]
- [[#Structural Efficiency]]

##### Technical efficiency

```ad-Definizione
title: Techincal efficiency

**Technical efficiency** is reached when the [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Cost Function\|cost]] is minimized.

```

##### Efficiency of market assignation

```ad-Definizione
title: Efficiency of market assignation

When efficient market decisions are made.

```

##### Social efficiency

```ad-Definizione
title: Social efficiency

Social efficiency is the [[Università/Magistrale/1° Anno/1° Semestre/Decision Making & Economy in Urban Mobility/Notes/01 - Production and cost functions in transport - DME#Efficiency\|#Efficiency]] condition when **Externalities** are included.

```

##### Efficiency of scale

Current capacity vs ideal capacity
- Ideal: combination of inputs and outputs inside the constant returns to scale
- Long-term competitive equilibrium, where production has constant returns to scale

##### Structural Efficiency

Structural efficiency is reached when production is located in the non-congested region of possibile inputs combinations.

#### How to measure efficiency

![Schermata 2024-11-05 alle 12.38.39.png](/img/user/Schermata%202024-11-05%20alle%2012.38.39.png)

### Economy of scale

[[#Average cost]] $\searrow \iff \nearrow$ scale  

If the nature of a business is to take advantage of economy of scale, that business will try to grow. There will then be just a few big businesses in that sector.

### Economy of density

Economy of density is the concept in which a business sees its cost decreasing when the density of the business increases.

```ad-example
The total cost to transport passengers decreases by increasing utilisation of existing vehicle fleet and infrastructure capacity within a market area of given size.
```

### Mohring effect

```ad-Definizione
title: Mohring effect

The Mohring effect is a scenario where, adding users to a transportation network actually decreases the average cost incurred by the user.

```

Let's try to understand this through an example:

```ad-example

Imagine we have a road. Every time another car enters the road, the road becomes more conjested and travel time increases for every one. This is a normal behavior.

Let's consider now a bus line. An increase in users will make the ride more unconfortable for everyone, since the bus will be more crowded. At a certain point though, if there are enough users, the bus company might decide to add more buses increasing the ferquency. This will shorten travel time for everyone and increase everyone's comfort. In this case, an increase in users has reduced the average cost incurred by each user. This last one, was an example of the **Mohring effect**.

```


