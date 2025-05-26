---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/traffic-simulation-models/assgm/nonlinear-follow-the-leader-models-of-traffic-flow/","tags":["UNI"]}
---



# [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Assgm/Nonlinear follow-the-leader models of traffic flow\|Nonlinear follow-the-leader models of traffic flow]]

```table-of-contents
```
Follow the leader theory of traffic

Single-lane dense traffic with no passing.

each driver reacts in some specific fashion to a stimulus from the car ahed of and/or behind them.

The theory applies mainly to **dense** traffic.

Basic idea:

$$
\text{response} = \text{sensitivity} \cdot \text{stimulus}
$$

- response is taken as the acceleration of the vehicle as the driver has direct control over this parameter.
- The stimulus is a function fo the position of cars and their time derivatives (speed)

It has been established that there is correlation between driver response and relative speed of their car and the one ahead. **The stimulus is than taken as the relative speed**.

## Equations

$$
\ddot{x}_{n+1} (t+T) = \lambda [\dot{x}_{n}(t) - \dot{x}_{n+1}(t)] \qquad (2)
$$
- $x_{n}:$ position of the $n^{tn}$ car
- $T:$ reaction time
- $\lambda:$ sensitivity 

Possible sensitivity functions:
$$
\begin{cases}
1. \,\text{constant} &\lambda = a \\
2. \,\text{step function} &\lambda = \begin{cases}
a,\quad s \le s^{*} \\
b,\quad s > s^{*}
\end{cases} \\
3. \,\text{reciprocal spacing} &\lambda = \dfrac{c}{s}
\end{cases}
$$
where:
- $s = x_{n}- x_{n+1}$ (the spacing)
- $a,b,c$ are constants

General equation:
$$
\lambda = a\frac{\left[\dot{x}_{n+1}(t)\right]^{m}}{[x_{n}(t)-x_{n+1}(t)]^{l}} 
$$
This can lead to some specific forms for the sensitivity:
$$
\begin{cases}
\text{Edie:} \quad &\lambda = c \dfrac{\dot{x}_{n+1}}{s^{2}} \qquad (6)\\
\text{Leading to Greenshield:} \quad &\lambda  = \dfrac{c}{s^{2}} \qquad (7)
\end{cases}
$$
For the validity of each model, we have to look at 2 things:
- Stability - Only for the linear form (otherwise, too difficult)
	- Same bounds are applied for the non linear cases
		- This is possible as long the nonlinear system only has small perturbations (?piccole oscillazioni?)
- Steady-state flow characteristics

### Steady flow characteristics

For steady-state flow characteristics is possible to obtain a fairly complete description corresponding to any sensitivity given by an equation such as the one used in the following:
$$
\ddot{x}_{n+1}(t+\Delta t) = a\frac{[\dot{x}_{n+1}(t)]^{m}}{[x_{n}(t)-x_{n+1}(t)]^{l}} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ] \qquad (9)
$$

- [x] Pag. 547/548. Why does integrating the equation yields the steady-state flow equation? ✅ 2025-04-18


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/03-fundamentals-of-traffic-flow-modeling-omt/#greenshield-k-v-model" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



##### Greenshield k-v model

![Schermata 2024-12-06 alle 17.14.15.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Schermata%202024-12-06%20alle%2017.14.15.png)

The figure above shows the original Greenshield k-v model. He described the average speed as a function of density, requaring 2 calibration parameters



```ad-Definizione
title: The Greenshield $k-v$ model

![Greenshield k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.18.32.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Greenshield%20k-v%20model%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.18.32.excalidraw.png)


$
v = v_{f} \left(  1 - \frac{k}{k_{j}}  \right)
$
where:
- $v_{f}:$ Free flow speed - Speed at which vehicles travel when density is very low
- $k_{j}:$ Jam density - Maximum density at the infrastructure when vehicles are in a gridlock jam, completely stopped

```

Given $q_{max}$ is the **maximum flow** of the infrastructure, the **capacity**, this is given by the area of the rectangle of sides $v_{0}$ and $k_{0}$.

The capacity point also distinguishes between two states:
- Congestion
- Free flowing

```ad-note
title: Finding $q_{max}$

$v_{0}$ and $k_{0}$ can be obtained as follows. According to the [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Fundamental equation of traffic\|fundamental equation of traffic]] and to the Greenshield model
$
\begin{cases}
q = vk \\
v = v_{f} \left(  1 - \frac{k}{k_{j}}  \right)
\end{cases}
$
Combining the 2 equations:
$
\begin{align}
q &= v_{f} \left(  1 - \frac{k}{k_{j}}  \right)k = \\
&= v_{f}k - \frac{v_{f}}{k_{j}}k^{2}
\end{align}
$
To find the maximum of this funciton, we can derive and impose equal to 0:
$
\begin{align}
\frac{\partial q}{\partial k} = \frac{\partial}{\partial k} \left( v_{f}k - \frac{v_{f}}{k_{j}}k^{2} \right) &\stackrel{!}{=} 0 \\
v_{f} - 2 \frac{v_{f}}{k_{j}} k &= 0 \\
k = \frac{1}{2} k_{j}
\end{align}
$
So, 
$
k_{0} = \frac{1}{2} k_{j} \qquad v_{0} = \frac{1}{2} v_{f}
$

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.31.49.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.31.49.excalidraw.png)

```



</div></div>

# Experimental and observational data

 2 types of data:
 - Phenomenological flow & Density measurements
	 - Tunnels of New York City area by the Port of New York Authority
		 - No passing allowed
		 - Fairly congested for long periods every day
 - Records of follow-the-leader experiments
	 - General Motors Technical Center test track
		 - Used to obtain stimulus-response laws with constant sensitivity
	- More tests in General Motors Technical Center test track
	- Tunnels of New York
		- To compare macroscopic phenomenological measurements with microscopic results of follow-the-leader theory

## Phenomenological flow & Density measurements

- Tunnels of New York City area by the Port of New York Authority
		 - No passing allowed
		 - Fairly congested for long periods every day

## Records of follow-the-leader experiments

- General Motors Technical Center test track
	 - Used to obtain stimulus-response laws with constant sensitivity
- More tests in General Motors Technical Center test track
- Tunnels of New York
	- To compare macroscopic phenomenological measurements with microscopic results of follow-the-leader theory

The data was used in 2 ways:
- Phenomenological study of the **time averages** of **space** and **speed**
- **Timewise correlation study** of the **response** of the following car with various functionals assumed for the product of *stimulus times sensitivity*


Experiment conducted with 2 cars.
Assumptions:
- Headway and speed of the 2 cars are the same of the time and space averages of the whole stream of traffic
First equation (11)

$$
y_{i} \stackrel{\triangle}{=} f_{m}(\overline{u}_{i}) =
\begin{cases}
\overline{u}_{i}^{1-m} \qquad &m\ne 1 \\
\ln(\overline{u}_{i}) \qquad &m = 1
\end{cases}
\qquad\qquad
x_{i} \stackrel{\triangle}{=} f_{l}(\overline{s}_{i}) =
\begin{cases}
\overline{s}_{i}^{1-l} \qquad &l\ne 1 \\
\ln(\overline{s}_{i}) \qquad &l = 1
\end{cases}
$$
Linear correlation between $y_{i}$ and $x_{i}$ was evaluated. They computed the **correlation coefficient** for different values of $m$ and $l$.

Also, they calculated the standard deviation for the coefficient $c$ of eq (11).

Difficulties:
- Limited number of runs $i$. Only 18
- Drivers do not necessarily have the same coefficients $c$ and $c'$

The objective was not to find non-integer values of $m$ and $l$ to maximize correlation. Rather to discover trends, like, are $m$ and $l$ likely to be positive or negative?


[[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Edie k-v model\|03 - Fundamentals of traffic flow modeling - OMT#Edie k-v model]]


___

### Follow the leader experiments

Used data of 18 experiments in the Lincoln Tunnel of New York.

2 approaches:
- Phenomenological aspects
- Timewise correlation study



# Report

Gazis, Herman and  Rottery propose a car fallowing model of the "stimulus-response" type. Two vehicles are involved, a *leader* and a *follower*. According to stimulus-response models, the follower reacts to the behaviour of the leader. The intensity of the response is governed by a factor called *sensitivity*. These models have the following form:
$$
\begin{equation}
\text{Response} = \text{Sensitivity} \times \text{Stimulus}
\end{equation}
$$
A driver can mainly control one aspect of the vehicle: the acceleration (or deceleration) \footnote{They can also control steering but that is beyond the scope of this study}. Therefore, it makes sense for the response to be the follower's (vehicle $n+1)$ acceleration:
$$\ddot{x}_{n+1}(t+T)$$
Notice how the quantity is evaluated at time $t+T$; $T$ is the reaction time. The stimulus is taken to be the difference in speed between the two vehicles: 
$$
\dot{x}_{n}(t) - \dot{x}_{n+1}(t)
$$
The sensitivity, $\lambda$, is some generic function of the follower's speed ($x_{n+1}(t+T)$) and the current spacing between the two cars ($x_{n}(t)-x_{n+1}(t)$).

In short, the model under study is explained by the equation:
$$
\begin{equation}
\ddot{x}_{n+1}(t+T) = \underbrace{a\frac{\left[\dot{x}_{n+1}(t)\right]^{m}}{[x_{n}(t)-x_{n+1}(t)]^{l}}}_{=\lambda} \times \left[ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) \right]
\label{eq: GM 5th gen}
\end{equation}
$$
where:
- $a:$ is a constant
- $m,l:$ are two parameters that need calibration

The sensitivity depends on 2 parameters, $m$ and $l$. These have no physical meaning. The authors idea is that these values can be tweaked to better fit real life data.

This approach is quite useful since it allows to study several models at once. In fact, this is the 5th iteration of the General Motors (GM) models, each described assigning specific values to the exponents $m$ and $l$. On top of these, also some more functionals proposed by other authors (ie: Edie) can be studied starting from the same equation.

A summary of some models described by the Equation (\ref{eq: GM 5th gen}) is portrayed in Table (\ref{tab: Some models}) 45


![Nonlinear follow-the-leader models of traffic flow 2025-04-12 18.57.22.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Traffic%20Simulation%20Models/Assgm/Allegati/Nonlinear%20follow-the-leader%20models%20of%20traffic%20flow%202025-04-12%2018.57.22.excalidraw.png)
