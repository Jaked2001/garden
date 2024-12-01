---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/operation-and-management-of-transport-systems/notes/03-fundamentals-of-traffic-flow-modeling-omt/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT\|03 - Fundamentals of traffic flow modeling - OMT]]

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
- [[01 - Introduction to trajectories Analysis - OMT#Flow|Flow]] - $q$
- Density - $k$
- Average Speed - $v$
They are very **robust**: it's difficult for things to go wrong in calculation. They only use a few parameters (3).

```


They are known with many different names:
- Lightwill, Witham, Rehand (LWR) model
- Continuous theories
- KW (Kinematic Wave) - shock wave theory

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
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Spacing\|Spacing]] - $s$
- Instantaneous speed - $v_{i}$
Microscopic models are known as:
- Car following theories
And are solve by computer simulators:
- [[AIMSUM\|AIMSUM]]
- [[VISSIM\|VISSIM]]
- [[PARAMICS\|PARAMICS]]
- [[SUMO\|SUMO]] - which is [[Open Source\|Open Source]]

# LWR Traffic flow theory

## LWR theory postulates

LWR theory is based on 2 postulates:

```ad-tip
title: Postulates of LWR theory
1. [[#Conservation of vehicles]]
2. [[#Equation of state]]
```

### Conservation of vehicles

Given a control volume (space x time), the number of vehicles that enter the volume and that exit the volume must be equal.

Look at the trajectories in the following diagram:

![Conservation of veh principle graph - 03 - Fundamentals of traffic flow modeling - OMT 2024-11-30 19.13.03.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Conservation%20of%20veh%20principle%20graph%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-11-30%2019.13.03.excalidraw.png)


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

