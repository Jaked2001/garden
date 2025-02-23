---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/02-fundamentals-fo-queuing-theory-omt/","tags":["UNI"]}
---


# [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT\|02 - Fundamentals fo Queuing Theory - OMT]]

```table-of-contents
```


Queues appear when a flow of vehicles, persons or objects wants to receive a service that implies a restriction. Typically, services have a **limited capacity** or are offered only with some **frequency**, which may lead to queues, delays and waits.

The subject that studies queues is referred to Queuing Theory (see also [[03. Variabili Aleatorie#Teoria delle code]], [[05. Teoria del Deflusso#Teoria delle code]]).

Most of the complexities of queuing theory come from the stochastic nature of the processes involved. 


## Components of a queuing system


Server: the restriction
Storage: where the costumer waits
Arrivals: the ones that feed the queue
Departures: the yield after service

![Queuing system diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.01.37.excalidraw.png](/img/user/Excalidraw-2/Queuing%20system%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.01.37.excalidraw.png)
%%[[Queuing system diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.01.37.excalidraw|🖋 Edit in Excalidraw]]%%

### Server

```ad-Definizione
title: Server

In a [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Components of a queuing system\|queuing system]], the **server** represents the restriction of the system. The server is able to provide the service at a certain rate, $\mu$.


![Server symbol - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.17.04.excalidraw.png](/img/user/Excalidraw-2/Server%20symbol%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.17.04.excalidraw.png)


```

#### Server disposition

In any system, there can be more than 1 server. The $n$ servers, can be
- [[#Servers in parallel]]
- [[#Servers in series]]

##### Servers in parallel

When the servers are localised in parallel, they can work at the same time. These are differentiated  based on how the queue works:
- [[#Decentralised system]]
- [[#Centralised queue]]

One problem that might arise with parallel service, is that the servers are not positioned in space in an efficient way. It may happen that the queue of one server blocks some other server. This could happen, for example, at a petrol station where two pumps are one after the other and there is not enough space for cars to overtake each other.

![Schermata 2024-10-26 alle 12.33.58.png](/img/user/Schermata%202024-10-26%20alle%2012.33.58.png)

###### Decentralised system

In a decentralised system, each server has its own queue.

![Decentralized queues diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.20.34.excalidraw.png](/img/user/Excalidraw-2/Decentralized%20queues%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.20.34.excalidraw.png)
%%[[Decentralized queues diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.20.34.excalidraw|🖋 Edit in Excalidraw]]%%

###### Centralised queue

In a centralized queue, there are multiple [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Server\|servers]] but only 1 queue.

![Centralized queue diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.22.01.excalidraw.png](/img/user/Excalidraw-2/Centralized%20queue%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.22.01.excalidraw.png)
%%[[Centralized queue diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.22.01.excalidraw|🖋 Edit in Excalidraw]]%%

The centralised queue, if well managed, can maximize the capacity and efficiency of the system. In fact, in this case, no server will ever be idle, while there are other servers working. 

It also guarantees the [[#First Come First Serves - FCFS]] functioning.

In these kind of systems, it is important to implement adequate information system that assigns customers to servers at due time. This needs to ensure that there is no idle server at any time.

This can be challenging, especially when it takes a long time for the costumer to get to the server from the end of the queue (think of container ships waiting outside a port).

##### Servers in series

###### Tandem queues

![Tandem Queues diagram02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.27.24.excalidraw.png](/img/user/Excalidraw-2/Tandem%20Queues%20diagram02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.27.24.excalidraw.png)
%%[[Tandem Queues diagram02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.27.24.excalidraw|🖋 Edit in Excalidraw]]%%

In this kind of systems costumers need to undertake several steps to receive a complete service.

For example, in an airport, a passenger has first to check-in, thank go through security, and finally queue to board the plane. Seen as a whole, this is a tandem queue. 

In this scenario, the departure from the previous server, is the arrival of the subsequent one.

A better explanation of this kind of systems is provided in the section [[#Tandem queueing system]]
### Storage

### Arrivals

### Departures

## Queuing disciplines

Queuing discipline is a non-physical component of a queuing system. It refers to the rules which determine **in which order the costumers are served**.

The most common ones are:
- [[#First Come First Serves - FCFS]]
- [[#Last Come Last Serves - LCLS]]
- [[#Service in Random Order - SIRO]]
- [[#Round Robin - RR]]

Sometimes, there can be priorities assigned to some kind of costumers, leading to a new type of discipline:
- [[#Early Due Date First - EDDF]]
- [[#Shortest Service Time First - SSTF]]

### First Come First Serves - FCFS

This is the most common discipline when dealing with human costumers.

```ad-Definizione
title: First Come First Serves (FCFS)

In **FCFS discipline**, service is provided in the same order of arrivals.

```

This doesn't mean that the first costumer to enter will also be the first one to exit as, with [[#Servers in parallel]], some server may be faster than another allowing for overtakes in the system.

### Last Come First Serves - LCFS

```ad-Definizione
title: Last Come First Serves (LCFS)

In **LCLS discipline**, costumers are served in the reversed order of arrival. 

```

This happens when the [[#Storage]] is in a closed space and the entrance and exit are the same "door". 

For example an airport shuttle bus will unload first the passengers that boarded the bus at last and viceversa.


### Service in Random Order - SIRO

```ad-Definizione
title: Service in Random Order (SIRO)

In **SIRO discipline** there is no preset order and the costumer is selected randomly from the queue.

```

This system is mostly applied to industrial processes where the costumer are different items in a production line.

### Round Robin - RR

```ad-Definizione
title: Round Robin - RR

In RR discipline, each costumer is assigned the same amount of service time. If the service is not completed in said time, the costumer returns back into the queue.

```

This discipline applies in the communication networks.

### Early Due Date First - EDDF

### Shortest Service Time First - SSTF


## Cumulative plot


```ad-Definizione
title: Cumulative plot

A cumulative plot - $(N,t)$ diagram - plots the cumulative number of customers $N$, to cross a specific location as a function of time $t$.

![Cumulative plot generic - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 15.09.12.excalidraw.png](/img/user/Excalidraw-2/Cumulative%20plot%20generic%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2015.09.12.excalidraw.png)


```

Properties of the cumulative plot:
- It's a discrete function
- It's always increasing or, at most, constant

The [[01 - Introduction to trajectories Analysis - OMT#Flow|flow]] of vehicles or passengers $q$ can be calculated starting from the cumulative plot as:
$$
q_{(T)} = \frac{N(t_{j}) - N(t_{i})}{t_{j}-t_{i}}
$$
where
- $T= t_{j}-t_{i}$ the period of observation

The plot can be obtained in 2 ways:
- Every time a customer enters the system, the time and the cumulative number of customer is recorded
- Every a predefined $\Delta t$, the cumulative number of customer that entered the system in that time interval is recored

When a large number of customer is recorded, the jumps of the $N(t)$ function become meaningfulness. So, the function is usually replaced by a continuous interpolation.

![Cumulative plot interpolation - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 15.24.01.excalidraw.png](/img/user/Excalidraw-2/Cumulative%20plot%20interpolation%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2015.24.01.excalidraw.png)
%%[[Cumulative plot interpolation - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 15.24.01.excalidraw|🖋 Edit in Excalidraw]]%%

In this situation, we can calculate the instantaneous flow $q_{(t)}$ as:
$$
q_{(t)} = \frac{\partial N}{\partial t} 
$$

## Input-output diagram

An input-output diagram is the overlay of 2 [[#Cumulative plot]]:
- $A(t) = N(t,x_{0}):$ cumulative plot measured at location $x_{0}$, before the system being measured. In other words, the [[#Arrivals]]
- $D(t) = N(t,x_{1}):$ cumulative plot measured at location $x_{1}$, after the system being measured. In other words, the [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Departures\|#Departures]]

- [x] If the $A(t)$ curve is not measured exactly at the entrance of the system of interest, don't we overestimate the delay time in the system? ✅ 2024-10-29

![Input-Output Diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 16.04.28.excalidraw.png](/img/user/Excalidraw-2/Input-Output%20Diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2016.04.28.excalidraw.png)
%%[[Input-Output Diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 16.04.28.excalidraw|🖋 Edit in Excalidraw]]%%

The diagram above is an input-output diagram.

Notice that the horizontal distance between the 2 curves at a given number of cumulative costumers, $n_{1}$, is the time spent by that costumer in the system. This time includes:
- Potential delays
- Free flow service time

Instead, the vertical distance between the 2 curves at a given instant $t_{1}$, is the customer **accumulation** in the system. This includes:
- The customer being served at the moment
- The customers waiting to be served

```ad-note
title: Observation

The $D(t)$ curve can **never** go above the $A(t)$ curve since, in order to exit, a customer has to have enter first.

It the 2 curves match, it means that the system is **empty** of customers.

```

In the diagram above, other than the input-output diagram, the amount of customers in service and in queue at any given time is also shown:

![input-output plus service plus queue diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 16.30.06.excalidraw.png](/img/user/Excalidraw-2/input-output%20plus%20service%20plus%20queue%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2016.30.06.excalidraw.png)
%%[[input-output plus service plus queue diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 16.30.06.excalidraw|🖋 Edit in Excalidraw]]%%

### A logistic curve

We will now consider an [[#Input-output diagram]] with a large number of customers, so that the curves can be seen as continuous functions.

![Input-output diagram - continuous - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.05.26.excalidraw.png](/img/user/Excalidraw-2/Input-output%20diagram%20-%20continuous%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2017.05.26.excalidraw.png)
%%[[Input-output diagram - continuous - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.05.26.excalidraw|🖋 Edit in Excalidraw]]%%

In the input-output diagram, the Arrival curve $A(t)$ usually takes the shape of a logistic curve.

The arrival rate is always relatively small at the two extremes while it picks in the middle (the arrival rate, $\lambda$, is given by the slope of the arrival curve). This is because, as humans, we tend to want the same service at about the same time. This pick rate is theoretically **unbounded**.

The departure curve instead, has a fixed maximum rate, $\mu$, equal to the Capacity of the system. So, this slope is always **bounded**.

From a normal [[#Input-output diagram]] we can easily read the sum of the service time and delay, and the total accumulation (number of customer being served + customers queuing).

It is useful to be able to read directly the delay and the excess accumulation. This can be done through the [[#Virtual Arrivals Curve]]


## 3D representation of input-output diagram

If we want to visualize both vehicles [[01 - Introduction to trajectories Analysis - OMT#Trajectories of a traffic stream on a time-space diagram|trajectories]] and input-output diagram on the same chart, we can do so in a 3D diagram:

![Schermata 2024-10-26 alle 16.57.30.png](/img/user/Schermata%202024-10-26%20alle%2016.57.30.png)

The projection of this diagram on the ($x,t$) plane gives the trajectories, while the projection onto the $(N,t)$ plane gives the input-output diagram.

We can also look at the two projection one under the other to visualize everything on a single plane:

![Schermata 2024-10-26 alle 16.59.03.png](/img/user/Schermata%202024-10-26%20alle%2016.59.03.png)

- [x] If at one point there is queuing (accumulation), shouldn't the $x,t$ diagram show the trajectory going horizontal for a bit? ✅ 2024-10-28
	- [ ] Not necessarily: if more veh are being served and they don't need to stop, than this is correct

## Virtual Arrivals Curve


```ad-Definizione
title: Virtual Arrivals Curve (V(t))

The **Virtual Arrivals Curve** is a curve obtained by moving the arrival curve ($A(t)$) forward in time of an amount equal to the free flow travel time.

It can also be defined as the [[#Departures]] curve that would be measured in the absence of delay.

![Virtual Arrivals curve - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.14.37.excalidraw.png](/img/user/Excalidraw-2/Virtual%20Arrivals%20curve%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2017.14.37.excalidraw.png)


```

What we obtain:
- [[#Excess accumulation]]
	- [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Average excess accumulation\|#Average excess accumulation]]
- [[#Delay]]
	- [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Average delay per costumer\|#Average delay per costumer]]

### Excess accumulation

```ad-Definizione
title: Excess Accumulation ($Q$)

**Excess accumulation** is the number of extra costumer that we have in the system due to the fact that there is a queue forming.

```

The Excess accumulation can be obtained as the vertical distance in the $N-t$ diagram between the [[#Virtual Arrivals Curve]] and the [[#Departures]] curve.

![Excess accumulation N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.14.50.excalidraw.png](/img/user/Excalidraw-2/Excess%20accumulation%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.14.50.excalidraw.png)
%%[[Excess accumulation N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.14.50.excalidraw|🖋 Edit in Excalidraw]]%%

#### Average excess accumulation

![Average excess accumulation on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.19.33.excalidraw.png](/img/user/Excalidraw-2/Average%20excess%20accumulation%20on%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.19.33.excalidraw.png)
%%[[Average excess accumulation on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.19.33.excalidraw|🖋 Edit in Excalidraw]]%%

We define the area
$$
W_{1} \quad \rm [customers \cdot time]
$$
as the total aggregated delay in the period $t_{i}, t_{j}$

```ad-Teo
title: Average excess accumulation ($\overline{Q}$)

We can calculate **Average excess accumulation** ($\overline{Q}$) in the period $t_{i},t_{j}$:
$
\overline{Q} = \frac{W_{1}}{t_{j}-t_{i}}
$

```

Take some time to think on the meaning of the average excess accumulation:

```ad-attention

The average excess accumulation $\overline{Q}$ is always less or equal to the number of costumers that we see in the physical queue. Watch the example below to better understand this concept.

The diagram shows a stretch of road in 2 scenarios:
1. No queue: cars move freely at the same speed
	- We count 2 veh in the area of interest (the one in the orange dashed box)
2. Queue: Some cars are queueing in the area of interest
	- We count 5 cars

![02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.27.37.excalidraw.png](/img/user/Excalidraw-2/02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.27.37.excalidraw.png)


Notice that, of the 5 cars in the boxed area, even without queue, there would be 2. Meaning, the excess accumulation is NOT 5, but just 3.
```


### Delay

```ad-Definizione
title: Delay ($w$)

The **Delay** ($w$) is the extra time a costumer has to spend in the system due to queuing.

```

Delay can be obtained as the horizontal distance in the $N-t$ diagram between the [[#Virtual Arrivals Curve]] and the [[#Departures]] curve.

![02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.17.21.excalidraw.png](/img/user/Excalidraw-2/02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.17.21.excalidraw.png)
%%[[02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.17.21.excalidraw.md|🖋 Edit in Excalidraw]]%%

#### Average delay per costumer

![Average delay per costumer on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.23.15.excalidraw.png](/img/user/Excalidraw-2/Average%20delay%20per%20costumer%20on%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.23.15.excalidraw.png)
%%[[Average delay per costumer on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.23.15.excalidraw|🖋 Edit in Excalidraw]]%%

We define the area:$$
W_{2} \quad \rm[costumers]
$$as the total delay collectively incurred by customers between $n_{i}$ and $n_{j}$.

```ad-Teo
title: Average delay per costumer ($\overline{w}$)

We calculate the **Average delay per costumer** ($\overline{w}$) in the group between $n_{i}$ and $n_{j}$:
$
\overline{w} = \frac{W_{2}}{n_{j}-n_{i}}
$

```

## Little's Formula

![Little's Formula diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.36.38.excalidraw.png](/img/user/Excalidraw-2/Little's%20Formula%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.36.38.excalidraw.png)
%%[[Little's Formula diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.36.38.excalidraw.md|🖋 Edit in Excalidraw]]%%

```ad-Teo
title: Little's Formula

$
\overline{\lambda} = \frac{\overline{Q}}{\overline{w}}
$

**Proof:**

According to the definition, we can write for the [[#Average excess accumulation]]:
$
\overline{Q} = \frac{W}{t_{2}-t_{1}} \quad \Longrightarrow \quad W =  \overline{Q}(t_{2}-t_{1})
$
and for the [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Average delay per costumer\|#Average delay per costumer]]:
$
\overline{w} = \frac{W}{n_{2}-n_{1}} \quad \Longrightarrow \quad W =  \overline{w}(n_{2}-n_{1})
$
Meaning that:
$
\overline{Q}(t_{2}-t_{1}) = \overline{w}(n_{2}-n_{1})
$
Therefore:
$
\frac{\overline{Q}}{\overline{w}} = \frac{n_{2}-n_{1}}{t_{2}-t_{1}}
$
where the ratio on the right-hand side is the ratio of arrival of costumer, $\lambda$.
$
\frac{\overline{Q}}{\overline{w}} = \lambda 
$
*q.e.d.*
```

## Typical scenario

In a typical scenario we only have part of the data:
$$
\begin{align}
\text{Knowns: }&
\begin{cases}
V(t): \text{Measured when there are few people} \\
\mu : \text{Max service flow (it's a property of the facility)}
\end{cases} \\ \\

\text{Unknowns: }&
\begin{cases}
\overline{w}\\
\overline{Q}
\end{cases} \quad \Longrightarrow\text{We need the }D(t)
\end{align}
$$
We will describe how we can construct the [[#Departures|departure's]] curve.

First, keep in mind these 2 properties:
- $\dot{D}(t) = \mu \quad$ if there is queue
- $\dot{D}(t) = \min(\dot{V}(t), \mu)\quad$ if there is NO queue

Also, the following rules must be followed:
$$
\begin{cases}
D(t) < V(t) \quad \forall t \\
\dot{D}(t) < \mu \quad \forall t 
\end{cases}
$$

![Constructing a departures curve on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 19.24.26.excalidraw.png](/img/user/Excalidraw-2/Constructing%20a%20departures%20curve%20on%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2019.24.26.excalidraw.png)
%%[[Constructing a departures curve on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 19.24.26.excalidraw.md|🖋 Edit in Excalidraw]]%%

Notice how the $D(t)$ curve follows exactly the $V(t)$ curve until the rate of arrival, $\dot{V}(t)$ is greater than the rate of service, $\mu$. From this instance, the $D(t)$ has a constant slope equal to $\mu$, until it meets back the $V(t)$, at which point it goes back to following it.


❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ How to take average
❗❗❗❗❗❗❗❗❗❗❗❗

## On-off queueing system

```ad-Definizione
title: On-off queueing system

**On-off queueing systems** are systems where the service rate has 2 values, depending on wether the system is on or off:
$
\text{Service rate} = 
\begin{cases}
\mu \quad \text{when on}\\
0 \quad \text{when off}
\end{cases}
$
```

A typical example of on-off queuing system is the **traffic light**.

For simplicity, the following paragraph will assume the system is a traffic light with 2 states: <mark style="background: #BBFABBA6;">Geen</mark> and <mark style="background: #FF5582A6;">Red</mark>.

The traffic light alternates between an on state, green, for a time $G$ and an off-state, red, for a time $R$. The green and red phases together make a *cycle*, lasting $C$.

The system has a steady demand, $\lambda$, and a maximum constant on-state rate of service equal to $\mu$. 

A traffic signal defined as such, can work in 3 different conditions:
- [[#Unsaturated system]]
- [[#Exactly Saturated system]]
- [[#Overly Saturated system]]

### Unsaturated system

In an **undersaturated** system, all customers that arrive at the traffic light while it's red are served AND there remain time for people arriving later to pass without stopping. At the end of this paragraph you can find the condition so that a traffic signal is undesaturated.

![Undersaturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-14 15.56.17.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Undersaturated%20system%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-14%2015.56.17.excalidraw.png)
%%[[Undersaturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-14 15.56.17.excalidraw|🖋 Edit in Excalidraw]]%%

We can get the total cumulated [[#Delay]] as the area in purple, $W$.
Let $t^{*}$ be the time at which the queue completely dissipates, the total amount of customers that were in a queue and that were completely served in the time $t^{*}$ is equal to:
$$
n = \begin{cases}
\lambda t^{*} \\
\mu (t^{*}-R)
\end{cases}
$$
This tells us that:
$$
\lambda t^{*} = \mu (t^{*} -R)
$$
therefore
$$
\begin{align}
\lambda t^{*} &= \mu (t^{*} -R) \\
\lambda t^{*} &= \mu t^{*} - \mu R \\
(\lambda -\mu )t^{*} &= -\mu R \\
(\mu - \lambda )t^{*} &= \mu R \\
t^{*} &= \frac{\mu R}{\mu -\lambda }
\end{align}
$$
We can now calculate $n$:
$$
n = \lambda t^{*} = \frac{\mu \lambda R}{\mu -\lambda }
$$
Finally, the total cumulated delay is the area of the triangle of base $R$ and height $n$:
$$
W = \frac{1}{2} Rn = \frac{1}{2} \frac{\mu \lambda R^{2}}{\mu -\lambda }
$$
The [[#Average delay per costumer]] is the total delay dived by the total amount of customers served during 1 cycle, $n'$, where $n' = \lambda(R+G)$.
$$
\overline{w} = \frac{W}{n'} = \frac{\frac{1}{2} \frac{\mu \lambda R^{2}}{\mu -\lambda }}{\lambda (R+G)} = \frac{1}{2} \frac{\mu R^{2}}{(\mu -\lambda)(R+G) }
$$
```ad-Teo
title: Condition of undesaturation

A traffic light is undersaturated if all the customers arriving in one cycle are served  in the same cycle and still there remains some time for other customers to arrive.

```

Given that we can write:
- $\lambda (R+G):$ the total amount of customers that can arrive in one cycle
- $\mu G:$ the maximum amount of customers that can be served in one cycle
we want the condition:
$$
\lambda (R+G) < \mu G
$$
that can be written as
$$
\frac{\lambda}{\mu} < \frac{G}{R+G}
$$
In the particular case that $\frac{\lambda}{\mu} = \frac{G}{R+G}$, we have an [[#Exactly Saturated system]].

### Exactly Saturated system

In **exactly saturated** systems, *all and only* the costumers that arrive at the traffic light when it's red are served.

![Exactly saturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.02.44.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Exactly%20saturated%20system%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2016.02.44.excalidraw.png)
%%[[Exactly saturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.02.44.excalidraw|🖋 Edit in Excalidraw]]%%

Now the [[#Average delay per costumer]] can be obtained as:
$$
\overline{w} = \frac{W}{n'}
$$

### Overly Saturated system

In **Overly saturated** systems, *NOT all* the costumers that arrive at the traffic light when it's red are served. Some will have to wait for the next cycle.

In this scenario, the queue keeps growing.

![Overly saturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.09.14.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Overly%20saturated%20system%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2016.09.14.excalidraw.png)
%%[[Overly saturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.09.14.excalidraw|🖋 Edit in Excalidraw]]%%

In this case it's not possible to define a unique [[#Average delay per costumer]]. It can only be done if we set a number of cycles to take into consideration.

## Tandem queueing system


```ad-Definizione
title: Tandem queueing system


![Tandem queuing system diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.15.08.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Tandem%20queuing%20system%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2016.15.08.excalidraw.png)



Tandem queuing systems are systems in which a customer has to undergo several [[#Server|servers]] before exiting the system.

We call $n$ the number of servers.

```

For simplicity, we now consider a system of 3 servers:

![02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.20.39.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2016.20.39.excalidraw.png)
%%[[02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.20.39.excalidraw|🖋 Edit in Excalidraw]]%%

In the specific case shown in the figure above, the arrival and departure rates are related as follows:
$$
\lambda > \mu_{2} > \mu_{3}
$$
Let's get to a more realistic case, where the arrival curve is actually [[#A logistic curve]].

![02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.25.35.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2016.25.35.excalidraw.png)
%%[[02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.25.35.excalidraw|🖋 Edit in Excalidraw]]%%

Also in this case, the following condition is true:
$$
\mu_{1} > \mu_{2} > \mu_{3}
$$
The purple area, is the total cumulated delay for service 3. That is, the delay of all passengers between service 2 and service 3.

The total delay in the system would be the total area included between $\color{red} V(t)$ and $\color{orange} D(t)$.

```ad-note
title: What's the best way to improve the system

In general, it's to improve the service rate of the slowest server. In this case, $\mu_{3}$ is the smallest rate. The first course of action should be to improve this one. 

This can only be improved to the point $\mu_{3} = \mu_{2}$. After that, both need to be improved at the same time, otherwise the faster server doesn't actually allow for less queueing.

___

It is **NOT** recommended to design a system so that $\mu_{1}=\mu_{2} = \cdots = mu_{n}$. Designing like this would mean assuming there will not be queues. If, for whatever reason, one server happened to be slower than the others (or one is faster), the system wouldn't be able to accomodate these people.

```

### Diverging systems

A particular case of a [[#Tandem queueing system]] is one where a portion of customers leave the system before going through ALL the [[#Server|servers]].



## Stochastic queuing

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

### Relaxation time


## Centralisation

A queuing system with $n$ [[#Servers in parallel]] is given. The system can be operated in two ways:
- with $n$ independent queues ([[#Decentralised system]]), so that each server receives demand $a$
- with 1 single [[#Centralised queue]], whose demand is equal to $A = \sum\limits_{i=1}^{n}a_{i}$
We assume that the system has enough capacity to work without significant delays; only the [[#Stochastic delays]] apply.

![Centralization is better diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.09.22.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Centralization%20is%20better%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2019.09.22.excalidraw.png)
%%[[Centralization is better diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.09.22.excalidraw|🖋 Edit in Excalidraw]]%%

```ad-Teo
title: Centralisation is better than decentralised
A centralised system require less resources to offer the same level of service (or equivalently, with the same resources centralised systems provide better level of service).
___
*Proof*
The resources ($R_{C}, R_{D}$) needed to serve the system at a given level of service will be proportional to the fluctuations experienced by the demand. We can characterize these fluctuations with the [[Standard Deviation\|Standard Deviation]] of the arrival rates ($\sigma_{A}$). The 2 statement are therefore true:
$
R_{C} \propto \sigma_{A}; \qquad R_{D} \propto \sum\limits_{i=1}^{n}\sigma_{a} = n \sigma_{a}
$
We can relate the standard deviation of the single decentralized queues ($\sigma_{a}$) to that of the centralized one ($\sigma_{A}$).
Remember that, by definition
$
\sigma_{i} = \sqrt{\text{Var}{(i)}}
$
Remember also that the [[Variance\|Variance]] is a linear operator:
$
\text{Var}(nA+B) = n\text{Var}(A) + \text{Var}(B)
$
In our case:
$
\text{Var}(A) = \text{Var}\left(\sum\limits_{i=1}^{n}a \right) = n \text{Var}(a)
$
Applying the square root at both members of the equation:
$
\begin{align}
\sqrt{\text{Var}(A)} &= \sqrt{n \text{Var}(a)} \\
\sigma_{A} &= \sqrt{n}\sigma_{a}
\end{align}
$
Therefore, if the resources are proportional to the variances:
$
R_{D} \propto n \sigma_{a} = n \frac{\sigma_{A}}{\sqrt{n}} = \sqrt{n}\sigma_{A} \propto \sqrt{n} R_{C}
$
The conclusion is:
$
R_{D} \propto \sqrt{n}R_{C}
$
Given that $\sqrt{n} \ge 1$, this means that the resources for a decentralized system are always greater than those for a centralized one.

*q.e.d.*

```



## Optimisation

In a transportation system, there are always at least the two following costs to keep in mind:
- $Z_A:$ **Operator or Agency cost:** costs undergone by the operator of the transportation system (investments, operation, ...)
- $Z_{u}:$ **User cost:** costs undergone by the users using the system (tickets, time, delays,...)
The optimal level of service is obtained when the total cost is minimized.

![Optimization introduction diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.16.46.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Optimization%20introduction%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2019.16.46.excalidraw.png)
%%[[Optimization introduction diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.16.46.excalidraw|🖋 Edit in Excalidraw]]%%

We have an optimisation problem, where the objective function is:
$$
Z_{tot} = Z_{A} + Z_{u}
$$
The **decision variable** is the rate of service (measure of the level of service), $\mu$:
$$
\min_\mu Z = \min_\mu (Z_{A}+ Z_{u})
$$
We can do this analytically imposing the first derivative equal to 0:
$$
\frac{\partial Z}{\partial \mu} \stackrel{!}{=}0
$$
and solving for $\mu$.

```ad-example

Optimization example

Imagine we have a bus service that we want to optimize. It means we want to define what is the best [[Università/Triennale/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/05. Teoria del Deflusso#Distanziamento Temporale\|headway]], $h$. The headway is the *decision variable*.

To solve the problem, we need to define the agency and the user costs. 

**Agency costs:**
- $\beta:$ Cost of operating 1 bus for 1 day (includes everything)
- $\frac{C}{h}:$ Number of buses in use ($C=$ cycle time)
The total agency cost is:
$
Z_{A} = \frac{\beta C}{h}
$
**User costs:**
- $\overline{w}:$ [[#Average delay per costumer]]
- $\alpha:$ Value of time $\left[ \frac{\text{EURO}}{h}  \right]$ ($\sim 15$ €/h in Barcelona)
- $\lambda:$ Demand rate (daily demand)
$
Z_{u} = \lambda \overline{w} \alpha = \lambda \frac{h}{2 }\alpha 
$
The graphs below show both the shape of the 2 cost function, and why the average delay is equal to $\frac{h}{2}$.

![02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.29.05.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-17%2019.29.05.excalidraw.png)


The objective function is therefore:
$
\min_{h} \left( \beta C\frac{1}{h} + \frac{1}{2}\lambda\alpha  h \right)
$
We calculate the first derivative:
$
\frac{\partial Z}{\partial h} = -\beta C \frac{1}{h^{2}} + \frac{1}{2} \lambda \alpha \stackrel{!}{=}0
$
from which we get:
$
\begin{align}
-\beta C \frac{1}{h^{2}} + \frac{1}{2} \lambda \alpha &\stackrel{!}{=}0 \\
\frac{1}{2} \lambda \alpha &= \beta C \frac{1}{h^{2}} \\
\frac{1}{2} \lambda \alpha h^{2} &= \beta C \\
h^{2} = \frac{\beta C}{\frac{1}{2}\lambda \alpha}
\end{align}
$
which ultimately becomes:
$
h = \sqrt{\frac{2\beta C}{\lambda \alpha }}
$
```


## Psychology

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗