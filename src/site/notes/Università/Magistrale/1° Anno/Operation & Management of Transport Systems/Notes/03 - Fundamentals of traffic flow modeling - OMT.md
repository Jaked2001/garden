---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/operation-and-management-of-transport-systems/notes/03-fundamentals-of-traffic-flow-modeling-omt/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT\|03 - Fundamentals of traffic flow modeling - OMT]]

```table-of-contents
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/Fn3HMAaEfcQ?si=2lf72dOCaHH4Tdjp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

In traffic flow modeling, we can distinguish between
- Macroscopic models
- Microscopic models

![Schermata 2024-11-30 alle 18.57.20.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Allegati/Schermata%202024-11-30%20alle%2018.57.20.png)


In this chapter we will focus on [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#LWR Traffic flow theory\|#LWR Traffic flow theory]].

## Macroscopic models

```ad-Definizione
title: Macroscopic models

**Macroscopic models** predict the evolution in time of the macroscopic variables:
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Flow\|Flow]] - $q$
- Density - $k$
- Average Speed - $v$

They are very **robust**: it's difficult for things to go wrong in calculation. They only use a few parameters (3).

```


They are known with many different names:
- Lightwill, Witham, Rehand (LWR) model
- Continuous Traffic Flow Model
- Shock-Wave theory
- Cinematic Wave Theory

And are solved by some simulators - Calculation can be done by hand
- Cell Transmission Model



## Microscopic models

```ad-Definizione
title: Microscopic models

**Microscopic models** try to predict how one vehicle, the *follower*, follows another vehicle, the *leader*

Given the trajectory of the leader, we are interested in obtaining the trajectory of the follower.

```

They are very detailed, but use many many parameters (in the order of $10^{1}$).

In microscopic models, we work with microscopic variables:
- Headway - $h$
- [[01 - Introduction to trajectories Analysis - OMT#Spacing|Spacing]] - $s$
- Instantaneous speed - $v_{i}$

Microscopic models are known as:
- Car following theories

And are solve by computer simulators:
- [[AIMSUM]]
- [[VISSIM]]
- [[PARAMICS]]
- [[SUMO]] - which is [[Open Source]]

# LWR Traffic flow theory

## LWR theory postulates

LWR theory is based on 2 postulates:

```ad-tip
title: Postulates of LWR theory
1. [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Conservation of vehicles\|#Conservation of vehicles]]
2. [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Equation of state\|#Equation of state]]
```

### Conservation of vehicles

Given a control volume (space x time), the number of vehicles that enter the volume and that exit the volume must be equal.

Look at the trajectories in the following diagram:

![Conservation of veh principle graph - 03 - Fundamentals of traffic flow modeling - OMT 2024-11-30 19.13.03.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Conservation%20of%20veh%20principle%20graph%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-11-30%2019.13.03.excalidraw.png)
%%[[Conservation of veh principle graph - 03 - Fundamentals of traffic flow modeling - OMT 2024-11-30 19.13.03.excalidraw|🖋 Edit in Excalidraw]]%%

!!! The control volume is just a mathematical object. From now on we will refer to control area. The control area is the **physical** space that we are observing (for example, a stretch of road).

Let
- $m_{i}:$ Number of veh entering/exiting the control area
- $n_{i}:$ Number of veh already in the control area
Then
$$
m_{1} + n_{3} = m_{2} + n_{4}
$$
The members can be rearrange to write:
$$
m_{2}-m_{1} = n_{3}-n_{4}
$$
We can express the conservation of vehicles principle as follows:

*The difference between vehicles entering and exiting the control volume must be equal to the variation in storage in the control volume.*

The last equation can be divided by the area of the control region in the graph:
$$
\begin{align}
\frac{m_{2}-m_{1}}{(t_{2}-t_{1})(x_{2}-x_{1})} &= \frac{n_{3}-n_{4}}{(t_{2}-t_{1})(x_{2}-x_{1})} \\
\frac{m_{2}-m_{1}}{T} \frac{1}{x_{2}-x_{1}} &= \frac{n_{3}-n_{4}}{L} \frac{1}{t_{2}-t_{1}} \\
(q_{2}-q_{1}) \frac{1}{x_{2}-x_{1}} &= (k_{3}-k_{4}) \frac{1}{t_{2}-t_{1}} \\
\frac{q_{2}-q_{1}}{x_{2}-x_{1}} &= \frac{k_{3}-k_{4}}{t_{2}-t_{1}} \\
\frac{\Delta q}{\Delta x} &= -\frac{\Delta k}{\Delta t}
\end{align}
$$
where at one point we have substituted the definitions of flow and density. Finally, at limit, the equation can be written as:
$$
\frac{\partial q}{\partial x} = -\frac{\partial k}{\partial t}
$$

```ad-Teo
title: Conservation of Vehciles principle
The difference between vehicles entering and exiting the *control volume* must be equal to the variation in storage in the control volume.
$
\frac{\partial q}{\partial x} = -\frac{\partial k}{\partial t}
$
```

#### Relative flow

Let's consider the following time-space diagram:

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 16.49.23.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2016.49.23.excalidraw.png)
%%[[03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 16.49.23.excalidraw.md|🖋 Edit in Excalidraw]]%%

There are several vehicles traveling at speed $v$ and 1 <mark style="background: #FF5582A6;">observer</mark> traveling at speed $v_{0}$.

The [[#Conservation of vehicles]] applies for any control volume we consider. Therefore, it applies for the one indicated in orange in the graph.

Given that:
- $k:$ density of the vehicles traveling at speed $v$
- $T:$ Time span considered
- $L:$ Space considered

then, we have that:
$$
\begin{cases}
kL = \text{Number of vehicles entering from the left} \\
qT = \text{Number of vehicles exiting from the top} \\
q_{0}T = \text{Number of vehicles enetring from the bottom}
\end{cases}
$$
where $q_{0}$ is known as the **relative flow**. This is the flow seen by the observer. According to the [[#Conservation of vehicles]]:
$$
kL + q_{0}T = qT
$$
So:
$$
\begin{align}
q_{0}T &= qT - kL \\
q_{0} &= q - k \frac{L}{T} \\
q_{0} &= q - k v_{0}
\end{align}
$$
according to the [[01 - Introduction to trajectories Analysis - OMT#Fundamental equation of traffic|fundamental equation of trafic]] ($q = kv$):
$$
q_{0} = k (\underbrace{v-v_{0}}_{v_{re}})
$$
where $v_{re}$ is the relative speed between the observer and the the other vehicles.

```ad-Definizione
title: Relative flow
The **relative flow**, defined as
$
q_{0} = k(v-v_{0})
$
describes the amount of overtakes an observer experiences.
```

$$
\begin{cases}
v_{re} = 0 \quad\Longrightarrow\quad \text{No overtakes} \\
v_{re} > 0 \quad\Longrightarrow\quad \text{Traffic moves faster than the observer} \\
v_{re} < 0 \quad\Longrightarrow\quad \text{Traffic moves slower than. theobserver}
\end{cases}
$$
In case $v_{0}<0$, then $q_{0}>q$.


### Equation of state

The second postulate of the [[#LWR Traffic flow theory]] is the existence of an equation of state. This means that the state of the system can be univocally determined applying one equation to a state variable.

In [[#LWR Traffic flow theory]] there are 3 variables: $q,k,\overline{v}$. So, according to [[01 - Introduction to trajectories Analysis - OMT#Fundamental equation of traffic|the fundamental equation of traffic]], we can write one state variable as a function of the other 2. To get to the required equation of state, we need to go down to 1 degree of freedom. We need 1 extra equation.

This relation will be obtained empirically, meaning it is a regression of some measurement.

Let's imagine taking data points of speed against spacing:

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.04.39.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2018.04.39.excalidraw.png)
%%[[03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.04.39.excalidraw.md|🖋 Edit in Excalidraw]]%%

The graph shows the empirical relation between average speed and spacing. Notice that as spacing increases, also velocity increases until speed starts to approach a constant value, $v_{f}$, known as **free-flow speed**.

Remembering the [[01 - Introduction to trajectories Analysis - OMT#Fundamental equation of traffic|fundamental equation of traffic flow]], $q = kv = \frac{v}{s}$, we can see that, for each point on the curve, the slope of the line passing through that point and the origin gives the flow in that state. 

From this it's fairly easy to find the maximum flow, known as capacity of the infrastructure, as the <mark style="background: #BBFABBA6;">tangent line</mark>.

From the state diagram, we can also define some new concepts:
- [[#Congestion regime]]
- [[#Traffic regime]]

#### Congestion regime

![Congestion regime diagram - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.16.49.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Congestion%20regime%20diagram%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2018.16.49.excalidraw.png)
%%[[Congestion regime diagram - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.16.49.excalidraw|🖋 Edit in Excalidraw]]%%

##### Free-flow regime

```ad-Definizione
title: Free flow traffic

We have **free flow traffic** when we work on spacings (*density*) grater (*less*) than those relative to the capacity. 

```


##### Congestion

```ad-Definizione
title: Congestion

We have **congestion** when we work on spacings (*density*) less (*greater*) than those relative to the capacity. 

```

#### Traffic regime

##### Light traffic

```ad-Definizione
title: Light traffic

We have **light traffic** when the speed is **not** dependent on the spacing or density

```


##### Heavy traffic

```ad-Definizione
title: Heavy traffic

We have **heavy traffic** when the speed is dependent on the spacing or density

```


#### Density speed models

The first model was proposed by [[Bruce Greenshield]]. It's known as [[#Greenshield k-v model]]. We will see the following models:
- [[#Greenshield k-v model]]
- [[#Greenberg k-v model (1959)]]
- [[#Underwood k-v model (1961)]]
- [[#Edie k-v model]]


##### Greenshield k-v model

![Schermata 2024-12-06 alle 17.14.15.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Schermata%202024-12-06%20alle%2017.14.15.png)

The figure above shows the original Greenshield k-v model. He described the average speed as a function of density, requaring 2 calibration parameters



```ad-Definizione
title: The Greenshield $k-v$ model

![Greenshield k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.18.32.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Greenshield%20k-v%20model%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.18.32.excalidraw.png)


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

$v_{0}$ and $k_{0}$ can be obtained as follows. According to the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Fundamental equation of traffic\|fundamental equation of traffic]] and to the Greenshield model
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

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.31.49.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.31.49.excalidraw.png)

```


##### Greenberg k-v model (1959)

Greenberg, in 1959, proposed a model that works very well in the congested part of the diagram, but not so much in the free flow.

```ad-Definizione
title: Greenberg $k-v$ model

![Greenberg k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.35.46.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Greenberg%20k-v%20model%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.35.46.excalidraw.png)


$
v = v_{0} \ln{ \left(  \frac{k_{j}}{k}  \right) }
$

```

Since, mathematically, this model has velocity appriximating infinity for very low values of $k$, the model is usually cut at the free flow speed, $v_{f}$.

##### Underwood k-v model (1961)

Underwood, in 1961, proposed a model calibrated for free flow condition, but that doesn't work well in congestion

```ad-Definizione
title: Underwood $k-v$ model

![Underwood k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.41.25.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Underwood%20k-v%20model%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.41.25.excalidraw.png)


$
v = v_f e^{- \left( \frac{k}{k_0} \right)}
$

```

##### Edie k-v model

Edie, in 1961, decided to merge the [[#Greenberg k-v model (1959)]] and [[#Underwood k-v model (1961)]] in order to obtain one unique model that would work well for both free flow traffic and for congestion. This is simply the merging of the 2 functions cutoff at the capacity point $k_{0}$.

```ad-Definizione
title: Edie $k-v$ model


![Edie k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.45.41.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Edie%20k-v%20model%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.45.41.excalidraw.png)



```

## Traffic shock-wave


<iframe width="560" height="315" src="https://www.youtube.com/embed/Fn3HMAaEfcQ?si=2lf72dOCaHH4Tdjp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


```ad-Definizione
title: Traffic shock-wave
Whenever there is a change in the state of traffic, such as an acceleration or deceleration, the information of such change travels in traffic. The travel of information is referred to as a traffic **shock-wave**. This means that in different points in space and time, the change in traffic state happens only once the shock-wave reaches that point.

```

### Traffic shockwave speed

Look at the trajectory diagram below. There are several vehicles travelling at speed $v_{1}$ that then start to move at speed $v_{2} < v_{1}$.

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.25.33.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2018.25.33.excalidraw.png)
%%[[03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.25.33.excalidraw.md|🖋 Edit in Excalidraw]]%%

Let's apply the [[#Conservation of vehicles]] to the red square:
$$
\begin{align}
m_{1}+n_{3} &= m_{2}+ n_{4} \\
\underbrace{m_{1}-n_{4}}_{\text{State }U} &= \underbrace{m_{2}- n_{3}}_{\text{State } D}
\end{align}
$$
Let $q_{U}$ and $q_{D}$ be the flows for states $U$ and $D$ respectively. Similarly for $k_{U}$ and $k_{D}$ for densities. Then, the following relations stand:
$$
\begin{align}
m_{1} &= q_{U}T & n_{4} &= k_{U}L \\
m_{2} &= q_{D}T & n_{3} &= k_{D}L
\end{align}
$$
So we get:
$$
q_{U}T - k_{U}L = q_{D}T - k_{D}L
$$
Dividing both members by $T$, defining $\frac{L}{T} = u$:
$$
q_{U} - k_{U} u = q_{D} - k_{U} u
$$
from which we find:
$$
u = \frac{q_{U}-q_{D}}{k_{U} - k_{D}} = \frac{\Delta q}{\Delta k}
$$
that is defined as the **shockwave speed**.

```ad-Definizione
title: Traffic Shockwave speed

The **speed of a traffic shock-wave** between 2 stationary traffic states is determined by the increase in flow over the increase in density:
$
u = \frac{\Delta q}{\Delta k}
$
If:
- $u>0:$ wave travles in same direction of traffic
- $u<0:$ wave travles in opposite direction of traffic
```

## Fundamental diagram of traffic

The fundamental diagram of traffic is a density-flow diagram ($k-q$). It's vastly used because a lot of information can be derived from it by simple inspection.

The typical shape of a fundamental diagram of traffic is the following:

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 12.59.15.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2012.59.15.excalidraw.png)


Traffic will be on any point of that curve and each point resembles a different traffic state. 

**A TRAFFIC STATE ON THE GRAPH**

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 13.02.39.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2013.02.39.excalidraw.png)


Look at traffic state A.
- $k_{A}$ is the density in state $A$
- $q_{A}$ is the flow in state $A$
By definition, the speed can be found as $\frac{q}{k}$. So:
$$
v_{A} = \frac{q_{A}}{k_{A}}
$$
This can be represented graphically by a line going through the origin and intersecting the diagram in point $A$.

**RELATIVE FLOW**

From the same graph we can also obtain the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Relative flow\|#Relative flow]] 
between an observer traveling at speed $v_{A}$ and any other traffic state. Here we can see the relative flow with A1, $q_{0}^{A1} > 0$ and with A2, $q_{0}^{A2} < 0$.



**FREE FLOW AND CAPACITY**

Let's look at some specific states on the fundamental diagram (FD):

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 13.07.45.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2013.07.45.excalidraw.png)


In the graph above 2 states are represented:
- <mark style="background: #FFB86CA6;">Maximum flow</mark> - State M
- <mark style="background: #BBFABBA6;">Free flow</mark> - State F

From the graph it's easy to gain the free-flow speed, $\color{green} v_{F}$ and the optimal speed, $\color{orange}v_{opt}$.

**SHOCK-WAVE SPEED**

Let's now imagine traffic moves from state A to state B. It would be, in this case, an acceleration.

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 13.17.03.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2013.17.03.excalidraw.png)


By definition, $u = \dfrac{\Delta q}{\Delta k}$ is the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Traffic shockwave speed\|#Traffic shockwave speed]] between state A and state B. In the graph this can be read as the slope of the line going through A and B:
$$
u_{AB} = \frac{q_{A}-q_{B}}{k_{A}-k_{B}}
$$

## Shocks and waves

The concept behind [[#LWR Traffic flow theory]] is that every change in traffic state causes a wave to be generated. If we're able to track the waves in space and time, we are then able to predict traffic evolution.

Just 2 situations are possible with traffic:
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Acceleration - LWR\|#Acceleration - LWR]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Deceleration - LWR\|#Deceleration - LWR]]

### Acceleration - LWR

To study the acceleration transition, we will suppose a 1 lane road in which some vehicles are piled up behind a slow moving truck until time $t_{1}$. At $t_{1}$, the truck exits the road and vehicles behind it start accelerating. During the acceleration, the vehicles will travel at all the intermidiate speeds between the truck speed, $v_{B}$ and the free-flow speed, $v_{H}$.

At every *differential* speed change a [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Traffic shock-wave\|#Traffic shock-wave]] is generated.

![Acceleration - LWR theory - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 19.02.12.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Acceleration%20-%20LWR%20theory%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2019.02.12.excalidraw.png)


Each <mark style="background: #D2B3FFA6;">wave</mark> on the $t-x$ graph, with slope $u_{ij}$, describes the threshold between traffic state $i$ and traffic state $j$. Meaning we can predict the trajectory knowing the supposed slope from the $k-q$ [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Fundamental diagram of traffic\|#Fundamental diagram of traffic]].

Notice that since each step is theoretically differential, there are infinitely many shockwaves every time we go from one state to another.


### Deceleration - LWR

Now we just suppose that, on a stretch of road, vehicles are decelerating from speed $v_{A}$ to a lower speed $v_{F}$, therefore moving from state A to state F. Differently from the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Acceleration - LWR\|#Acceleration - LWR]], here waves do not tend to fan out. Instead, they tend to collide with one another.

When 2 waves collide, it means that 2 very different traffic states are colliding without any smooth transition. This generates yet an other wave, known as **shock**.

We will observe that initially there will be a smooth transition between state A and state F. Eventually though, only a single shockwave will remain changing abruptly from state A to state F. 

Thinking of this in real life, when traffic slows down on a road, initially, the first cars have time to slow down gradually as the very first cause of the slowdown. As more cars arrive, the new ones will have less and less time to react until a point where one car is moving at free-flow speed until it finds the end of the queue that just formed.

![Deceleration - LWR - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 19.35.04.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Deceleration%20-%20LWR%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2019.35.04.excalidraw.png)


## LWR simplifications

From the explanation of [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Shocks and waves\|#Shocks and waves]] it's clear that applying the model is not easy due to the infinitely many waves that generate between 2 states.

There are some simplifications that we can introduce to make things a lot easier. Specifically, we will add 2 assumptions:

### Instantaneous accelerations/decelerations - LWR

We will consider every change in speed instantaneous. This means that, for each state change, only one [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Traffic shock-wave\|#Traffic shock-wave]] is generated. This is particularly useful in [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Deceleration - LWR\|#Deceleration - LWR]], where infinitely many waves otherwise collide generating infinitely many shocks.

This assumption is actually quite justified when thinking that usually speed transition happen on a short time-span compared to the whole trajectory of a vehicle.

With this simplification, the graphs shown in [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Deceleration - LWR\|#Deceleration - LWR]] will appear as the following:

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 19.57.32.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2019.57.32.excalidraw.png)


This simplification still doesn't help much in accelerations, for which we need a new assumption: [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Triangular fundamental diagram\|#Triangular fundamental diagram]].

### Triangular fundamental diagram

In the 1990 it was proposed to adopt a **triangular** [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Fundamental diagram of traffic\|#Fundamental diagram of traffic]]. This served 2 porpuses:
- It was shown to actually be more accurate in describing present traffic, except for the area near capacity where the real data showed a smother transition
- It made every state change in the two areas ([[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Congestion\|#Congestion]] and [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Free-flow regime\|#Free-flow regime]]) have the same [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Traffic shockwave speed\|#Traffic shockwave speed]].

Now, the new state change, for [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Acceleration - LWR\|#Acceleration - LWR]], would look more like this

![03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 20.05.36.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/03%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-07%2020.05.36.excalidraw.png)


Now, in terms of waves, the state change $B\to H$ and $B\to C$ are equivalent. Therefore, the wave speed between for state change $B\to H$ is $w$.

## LWR Theory example


## LWR theory limitations

- All vehicles are considered equal
	- Avg behavior (no overtakes, all at same speed)
- Doesn't work well for light traffic
- Can't give much precision - all results should be approximated
	- $q-k$ graph comes from regression
	- We are considering changes from happening instantaneously --> waves should be considered to be thick lines
- Theory is not always stable
	- In congested traffic speeds often fluctuate (stop and go), which is not predicted by this model


