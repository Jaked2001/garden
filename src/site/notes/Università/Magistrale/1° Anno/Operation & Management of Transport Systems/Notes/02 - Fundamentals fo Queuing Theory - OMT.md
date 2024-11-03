---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/operation-and-management-of-transport-systems/notes/02-fundamentals-fo-queuing-theory-omt/","tags":["UNI"]}
---


# [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT\|02 - Fundamentals fo Queuing Theory - OMT]]

Queues appear when a flow of vehicles, persons or objects wants to receive a service that implies a restriction. Typically, services have a **limited capacity** or are offered only with some **frequency**, which may lead to queues, delays and waits.

The subject that studies queues is referred to Queuing Theory (see also [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/03. Variabili Aleatorie#Teoria delle code\|03. Variabili Aleatorie#Teoria delle code]], [[Università/Triennale/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/05. Teoria del Deflusso#Teoria delle code\|05. Teoria del Deflusso#Teoria delle code]]).

Most of the complexities of queuing theory come from the stochastic nature of the processes involved. 


## Components of a queuing system


Server: the restriction
Storage: where the costumer waits
Arrivals: the ones that feed the queue
Departures: the yield after service

![Queuing system diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.01.37.excalidraw.png](/img/user/Excalidraw-2/Queuing%20system%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.01.37.excalidraw.png)


### Server

```ad-Definizione
title: Server

In a [[#Components of a queuing system|queuing system]], the **server** represents the restriction of the system. The server is able to provide the service at a certain rate, $\mu$.


![Server symbol - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.17.04.excalidraw.png](/img/user/Excalidraw-2/Server%20symbol%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.17.04.excalidraw.png)
%%[[Server symbol - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.17.04.excalidraw|🖋 Edit in Excalidraw]]%%

```

#### Server disposition

In any system, there can be more than 1 server. The $n$ servers, can be
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Servers in parallel\|#Servers in parallel]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Servers in series\|#Servers in series]]

##### Servers in parallel

When the servers are localized in parallel, they can work at the same time. These are differentiated  based on how the queue works:
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Decentralized system\|#Decentralized system]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Centralized queue\|#Centralized queue]]

One problem that might arise with parallel service, is that the servers are not positioned in space in an efficient way. It may happen that the queue blocks some other server. This could happen, for example, at a petrol station where two pumps are one after the other and there is not enought space for cars to overtake each other.

![Schermata 2024-10-26 alle 12.33.58.png](/img/user/Schermata%202024-10-26%20alle%2012.33.58.png)

###### Decentralized system

In a decentralized system, each server has its own queue.

![Decentralized queues diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.20.34.excalidraw.png](/img/user/Excalidraw-2/Decentralized%20queues%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.20.34.excalidraw.png)


###### Centralized queue

In a centralized queue, there are multiple [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Server\|servers]] but only 1 queue.

![Centralized queue diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.22.01.excalidraw.png](/img/user/Excalidraw-2/Centralized%20queue%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.22.01.excalidraw.png)


The centralized queue, if well managed, can maximize the capacity and efficiency of the system. In fact, in this case, no server will ever be idle, while there are other servers working. 

It also guarantees the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#First Come First Serves - FCFS\|#First Come First Serves - FCFS]] functioning.

In these kind of systems, it is important to implement adequate information system that assigns customers to servers at due time. This needs to ensure that there is no idle server at any time.

This can be challenging, especially when it takes a long time for the costumer to get to the server from the end of the queue (think of container ships waiting outside a port).

##### Servers in series

###### Tandem queues

![Tandem Queues diagram02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.27.24.excalidraw.png](/img/user/Excalidraw-2/Tandem%20Queues%20diagram02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.27.24.excalidraw.png)


In this kind of systems costumers need to undertake several steps to receive a complete service.

For example, in an airport, a passenger has first to check-in, thank go through security, and finally queue to board the plane. Seen as a whole, this is a tandem queue. 

In this scenario, the departure from the previous server, is the arrival of the subsequent one.

### Storage

### Arrivals

### Departures

## Queuing disciplines

Queuing discipline is a non-physical component of a queuing system. It refers to the rules which determine **in which order the costumers are served**.

The most common ones are:
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#First Come First Serves - FCFS\|#First Come First Serves - FCFS]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Last Come Last Serves - LCLS\|#Last Come Last Serves - LCLS]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Service in Random Order - SIRO\|#Service in Random Order - SIRO]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Round Robin - RR\|#Round Robin - RR]]

Sometimes, there can be priorities assigned to some kind of costumers, leading to a new type of discipline:
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Early Due Date First - EDDF\|#Early Due Date First - EDDF]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Shortest Service Time First - SSTF\|#Shortest Service Time First - SSTF]]

### First Come First Serves - FCFS

This is the most common discipline when dealing with human costumers.

```ad-Definizione
title: First Come First Serves (FCFS)

In **FCFS discipline**, service is provided in the same order of arrivals.

```

This doesn't mean that the first costumer to enter will also be the first one to exit as, with [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Servers in parallel\|#Servers in parallel]], some server may be faster than another allowing for overtakes in the system.

### Last Come Last Serves - LCLS

```ad-Definizione
title: Last Come Last Serves (LCLS)

In **LCLS discipline**, costumers are served in the reversed order of arrival. 

```

This happens when the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Storage\|#Storage]] is in a closed space and the entrance and exit are the same "door". 

For example an airport shuttle bus will unload first the passengers that boarded the bus at last and viceversa.


### Service in Random Order - SIRO

```ad-Definizione
title: Service in Random Order (SIRO)

In **SIRO discipline** there is no preset order and the costumer is selected randomly from the queu.

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
%%[[Cumulative plot generic - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 15.09.12.excalidraw|🖋 Edit in Excalidraw]]%%

```

Properties of the cumulative plot:
- It's a discrete function
- It's always increasing or, at most, constant

The [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Flow\|flow]] of vehicles or passengers $q$ can be calculated starting from the cumulative plot as:
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


In this situation, we can calculate the instantaneous flow $q_{(t)}$ as:
$$
q_{(t)} = \frac{\partial N}{\partial t} 
$$

## Input-output diagram

An input-output diagram is the overlay of 2 [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Cumulative plot\|#Cumulative plot]]:
- $A(t) = N(t,x_{0}):$ cumulative plot measured at location $x_{0}$, before the system being measured. In other words, the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Arrivals\|#Arrivals]]
- $D(t) = N(t,x_{1}):$ cumulative plot measured at location $x_{1}$, after the system being measured. In other words, the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Departures\|#Departures]]

- [x] If the $A(t)$ curve is not measured exactly at the entrance of the system of interest, don't we overestimate the delay time in the system? ✅ 2024-10-29

![Input-Output Diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 16.04.28.excalidraw.png](/img/user/Excalidraw-2/Input-Output%20Diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2016.04.28.excalidraw.png)


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


### A logistic curve

We will now consider an [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Input-output diagram\|#Input-output diagram]] with a large number of customers, so that the curves can be seen as continuous functions.

![Input-output diagram - continuous - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.05.26.excalidraw.png](/img/user/Excalidraw-2/Input-output%20diagram%20-%20continuous%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2017.05.26.excalidraw.png)



In the input-output diagram, the Arrival curve $A(t)$ usually takes the shape of a logistic curve.

The arrival rate is always relatively small at the two extremes while it picks in the middle (the arrival rate, $\lambda$, is given by the slope of the arrival curve). This is because, as humans, we tend to want the same service at about the same time. This pick rate is theoretically **unbounded**.

The departure curve instead, has a fixed maximum rate, $\mu$, equal to the Capacity of the system. So, this slope is always **bounded**.

From a normal [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Input-output diagram\|#Input-output diagram]] we can easily read the sum of the service time and delay, and the total accumulation (number of customer being served + customers queuing).

It is useful to be able to read directly the delay and the excess accumulation. This can be done through the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Virtual Arrivals Curve\|#Virtual Arrivals Curve]]


## 3D representation of input-output diagram

If we want to visualize both vehicles [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Trajectories of a traffic stream on a time-space diagram\|trajectories]] and input-output diagram on the same chart, we can do so in a 3D diagram:

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

It can also be defined as the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Departures\|#Departures]] curve that would be measured in the absence of delay.

![Virtual Arrivals curve - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.14.37.excalidraw.png](/img/user/Excalidraw-2/Virtual%20Arrivals%20curve%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2017.14.37.excalidraw.png)
%%[[Virtual Arrivals curve - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.14.37.excalidraw|🖋 Edit in Excalidraw]]%%

```

What we obtain:
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Excess accumulation\|#Excess accumulation]]
	- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Average excess accumulation\|#Average excess accumulation]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Delay\|#Delay]]
	- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Average delay per costumer\|#Average delay per costumer]]

### Excess accumulation

```ad-Definizione
title: Excess Accumulation ($Q$)

**Excess accumulation** is the number of extra costumer that we have in the system due to the fact that there is a queue forming.

```

The Excess accumulation can be obtained as the vertical distance in the $N-t$ diagram between the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Virtual Arrivals Curve\|#Virtual Arrivals Curve]] and the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Departures\|#Departures]] curve.

![Excess accumulation N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.14.50.excalidraw.png](/img/user/Excalidraw-2/Excess%20accumulation%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.14.50.excalidraw.png)


#### Average excess accumulation

![Average excess accumulation on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.19.33.excalidraw.png](/img/user/Excalidraw-2/Average%20excess%20accumulation%20on%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.19.33.excalidraw.png)


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
%%[[02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.27.37.excalidraw.md|🖋 Edit in Excalidraw]]%%

Notice that, of the 5 cars in the boxed area, even without queue, there would be 2. Meaning, the excess accumulation is NOT 5, but just 3.
```


### Delay

```ad-Definizione
title: Delay ($w$)

The **Delay** ($w$) is the extra time a costumer has to spend in the system due to queuing.

```

Delay can be obtained as the horizontal distance in the $N-t$ diagram between the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Virtual Arrivals Curve\|#Virtual Arrivals Curve]] and the [[#Departures]] curve.

![02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.17.21.excalidraw.png](/img/user/Excalidraw-2/02%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.17.21.excalidraw.png)


#### Average delay per costumer

![Average delay per costumer on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.23.15.excalidraw.png](/img/user/Excalidraw-2/Average%20delay%20per%20costumer%20on%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2018.23.15.excalidraw.png)


We define the area:
$$
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
and for the [[#Average delay per costumer]]:
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
We will describe how we can construct the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT#Departures\|departure's]] curve.

First, keep in mind these 2 properties:
- $\dot{D}(t) = \mu \quad$ ff there is queue
- $\dot{D}(t) = \min(\dot{V}(t), \mu)\quad$ if there is NO queue

Also, the following rules must be followed:
$$
\begin{cases}
D(t) < V(t) \quad \forall t \\
\dot{D}(t) < \mu \quad \forall t 
\end{cases}
$$

![Constructing a departures curve on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 19.24.26.excalidraw.png](/img/user/Excalidraw-2/Constructing%20a%20departures%20curve%20on%20N-t%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-11-03%2019.24.26.excalidraw.png)


Notice how the $D(t)$ curve follows exactly the $V(t)$ curve untile the rate of arrival, $\dot{V}(t)$ is greater than the rate of service, $\mu$. From this instance, the $D(t)$ has a constant slope equal to $\mu$, until it meets back the $V(t)$, at which point it goes back to following it.



## On-off queueing system

### Unsaturated system

### Exactly Saturated system

### Overly Saturated system

## Tandem queueing system

### Diverging systems


