---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/01-introduction-to-trajectories-analysis-omt/","tags":["UNI"]}
---



# [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT\|01 - Introduction to trajectories Analysis - OMT]]

🕒 17:30: Problem solved in class (see iPad)


```ad-example

Imagine three friends who want to take a long trip using a tandem bicycle for two persons. Because the bike riders travel at 20 km/h, independent of the number of riders, and all three persons walk at 4 km/h, they proceed as follows:
- To start the journey, friends “A” and “B” ride the bicycle and friend “C” walks.
- After a while, friend “A” drops off friend “B” who starts walking and “A” rides the bicycle alone in reverse direction.
- When “A” and “C” meet, they turn the bicycle and ride forward until they catch up with “B”.
At that moment, the 3 friends have completed a basic cycle of their strategy, which they then repeat a number of times until they reach their destination. Could you determine their average travel speed?


Solution: $v_{m} = 10 \,\rm \frac{km}{h}$


![Introduction to trajectories Analysis 2024-10-01 18.15.47.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-01%2018.15.47.excalidraw.png)
%%[[Introduction to trajectories Analysis 2024-10-01 18.15.47.excalidraw.md|🖋 Edit in Excalidraw]]%%


```

## Trajectories of a traffic stream on a time-space diagram

When we work with time and space we use coordinated axis, with time ($t$) on the horizontal axis and space ($x)$ on the vertical axis.

![Introduction to trajectories Analysis 2024-10-01 17.52.02.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-01%2017.52.02.excalidraw.png)


This visualisation allows to have all the main parameters readily available:
- Position
- Speed/velocity
- Acceleration
- Time

Velocity:
$$
v = \frac{\partial x}{\partial t} = \dot{x}
$$

Acceleration:
$$
a = \frac{\partial^{2}x}{\partial t^{2}} = \ddot{x}
$$

![Introduction to trajectories Analysis 2024-10-01 17.59.18.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-01%2017.59.18.excalidraw.png)


The graph shows a possible trajectory of an elevator that stops at floor 3 and 5.


## Scheduling

We want to figure out the capacity of a rail line (single rail)

We have a train traveling from A to B at constant speed $V_{tech}$. We neglect accelerations.

Capacity is a flow: $q_{max} \quad \rm \left[ \frac{veh}{h} \right]$

```ad-Definizione
title: Flow
**Flow** it's the number of passengers or vehicles or expeditions per hour
$
q
$
```

![Introduction to trajectories Analysis 2024-10-01 18.20.11.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-01%2018.20.11.excalidraw.png)


**Dwell time** is the time taken for passengers to board and un-board.
**Headway:** ($h$)


$$
\underline{q} = \frac{1}{\overline{h}}
$$
then:
$$
\underline{q}_{max} = \frac{1}{h_{min}}
$$
We can increase capacity of the diagram above in different ways:
- Add a way for trains to pass each other in the middle: side track
- We could add more sidetracks but it becomes a problem of controlling the switches. If any train is delayed, then every train gets delayed
- Faster trains would allow for shorter headways
- Have more tracks at the ends so we can have train ready to leave as soon as one arrives

![Introduction to trajectories Analysis 2024-10-01 18.40.19.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-01%2018.40.19.excalidraw.png)




## Constructing trajectories

![Introduction to trajectories Analysis 2024-10-07 17.03.13.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-07%2017.03.13.excalidraw.png)



# Traffic stream properties

- $q, k, \overline{V}$ - macro
- $h, s,V_{i}$ - micro
- time vs space average

![Introduction to trajectories Analysis 2024-10-07 17.09.52.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-07%2017.09.52.excalidraw.png)


### Flow

We can define the flow - MACROscopic variable:
$$
q = \frac{m}{T}
$$
where:
- $m$: # of vehicles
- $T$: time

Can be written as:
$$
q = \frac{m}{\sum\limits_{i=1}^{m}h_{i}}
$$
also
$$
q = \frac{1}{\frac{1}{m}\sum\limits_{i=1}^{m}h_{i}} = \frac{1}{h}
$$
Flow is equal to the inverse of the **average headway**:

The headway is considered a *microscopic* variable.

### Spacing

$$
s \quad \rm[m]
$$
If we count the number ($n$) of vehicles in a stretch of length $L$, we obtain the DENSITY:
$$
k = \frac{n}{L} \quad \rm \left[ \frac{veh}{spac} \right], \left[ \frac{veh}{km} \right]
$$
And can also write:
$$
k = \frac{1}{\frac{1}{n} \sum\limits_{j=1}^{n} s_{j}} = \frac{1}{s}
$$
### Speed

![Introduction to trajectories Analysis 2024-10-07 17.19.26.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-07%2017.19.26.excalidraw.png)


![Introduction to trajectories Analysis 2024-10-07 17.27.14.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-07%2017.27.14.excalidraw.png)


The difference is that in one case we're measuring 
$$
\overline{V}_{t} \ge \overline{V}_{s}
$$
Let $i$ be a family of vehicle (ie traveling at the same speed)
$$
\overline{V}_{t} = \frac{\sum\limits_{i}m_{i}V_{i}}{\sum\limits_{i} m_{i}}
$$
If I multiply everything by $\frac{1}{T}$:
$$
\overline{V}_{t} = \frac{ \frac{1}{T}\sum\limits_{i}m_{i}V_{i}}{ \frac{1}{T} \sum\limits_{i} m_{i}} = \frac{\sum\limits_{i} q_{i}V_{i}}{q_{tot}}
$$

For spatial:

$$
\overline{V}_{s} = \frac{ \frac{1}{L}\sum\limits_{j}n_{j}V_{j}}{ \frac{1}{L} \sum\limits_{j} n_{j}} = \frac{\sum\limits_{i} k_{j}V_{j}}{k_{tot}}
$$


# Fundamental equation of traffic

## Stationary traffic

You can measure any value anywhere and it's always the same.

The only way is to have parallel trajectories that are equidistant.

![Introduction to trajectories Analysis 2024-10-07 17.38.34.excalidraw.png](/img/user/Excalidraw-2/Introduction%20to%20trajectories%20Analysis%202024-10-07%2017.38.34.excalidraw.png)


$$
q = \frac{m}{T} \qquad k = \frac{n}{L}
$$

$$
\frac{q}{k} = \frac{L}{T} = V
$$
then
$$
q = k\overline{V}
$$
This is true for stationary traffic.
Also:
$$
\overline{V}_{s} = \overline{V}_{t}
$$

It's also true for any kind of traffic:

$$
q = k\overline{V}_{s}
$$


❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗

$$
q = \sum_{i} q_{. }= \sum_{i}k_{i}V_{i}\cdot \frac{k}{k}
$$

$$
q = k \left[  \frac{\sum\limits k_{i}V_{i}}{k} \right]
$$