---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/sustainable-mobility/notes/02-public-transport-sm/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/2° Semestre/Sustainable Mobility/Notes/02 - Public Transport - SM\|02 - Public Transport - SM]]
!
```table-of-contents
```

## Definitions

### Public transport

The definition of **public transport** (PT) is not unanimous. Differente people categorise as PT different modes of transportation.

```ad-Definizione
title: Public transport

**Public transport** (or public transportation, or pablic transit or mass transit) is a system of transport for passengers *available for use by the general public*, typically *managed on a schedule*, *operated on established routes* and that charge a *posted fee for each trip*

```

Examples of PT are:
- Buses
- Trolleybuses
- Trams (or light rail) and passenger trains
- Rapid Transit (metro/subway/underground)
- Ferries

Public transport between cities is dominated by airlines, coaches and intercity rail (or high speed rail).

```ad-attention

The definition provided has some limitations:
- "managed on a schedule" and "operated on established routes": this is not always true, especially in the case of [[Demand Responsive Transit\|Demand Responsive Transit]];
- "charge a posted fee for each trip": we now have examples of cities or countries where public transport is free

```

Most PT systems run along fixed routes on a prefixed timetable. More frequent services run to a headway.

In basically every case, using public transport includes using at least one other mean of transportation (walking, driving...).

Public transport can then be [[#Public transport classification|classified]] following different criteria.

### Public transport classification

2 possible classifications of public transport are:
- Based on [[#Operation classification|operation]]
- Based on spatial [[#Coverage classification|coverage]]

#### Operation classification

- Schedule based service
- Frequency based service
- Flexible on-demand

#### Coverage classification

- Urban
- Suburban/metropolitan
- Regional/intercity
- Long-Distance

### Public transport route types

- Radial routes
- Circular routes
- Grid routes
- Linear routes
- Feeder routes
- Express routes
- On-demand/flexible routes


### Public transport characteristics

#### PT - Public vs private

Public transport refers to shared transportation services that are **available to the general public**, typically operated and regulated by the government or public agencies.

On the other end, private transport refers to modes that are **owned and used by individuals or specific groups**, rather than being open to the general public.


#### PT - Collective vs individual

Collective transport is a mode where multiple passengers **share** a vehicle or service, typically following a fixed route and schedule.

Individual transport is a mode where the **user has full control** over route and schedule, often using a private or exclusive vehicle.

#### PT - Urban vs Suburban

![Schermata 2025-03-12 alle 17.12.54.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/Schermata%202025-03-12%20alle%2017.12.54.png)

- Urban transport focuses on high-frequency, short-distance trips within cities
- Non-urban transport connects suburban, regional and intercity areas with longer distance services and lower frequencies

#### PT - Fixed routes vs flexible on-demand routes

Fixed routes PT operate on predefined routes and schedules, stopping at designated point regardless of passenger demand.

Flexible or on-demand PT adjusts its routes, stops or schedule based on real-time passenger requests.

#### PT - Dedicated vs shared infrastructure

**Dedicated infrastructure** is fully reserved for one kind of transport mode: **exclusive lanes, tracks or spaces**. They prevent interference with private vehicles

Shared infrastructure can be used by both PT and private vehicles.

#### PT - Frequency, scheduled and on-demand

![Schermata 2025-03-12 alle 17.26.05.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/Schermata%202025-03-12%20alle%2017.26.05.png)

- **Frequency** based transport is best for high-demand urban areas offering short waiting times and reliability
- **Scheduled** transport is convenient for long distance services and for commuters, requiring **planning**
- **On-demand** transport provides **flexibility** for *low-density* areas

#### PT - Access vs Affordability

**Access** in PT refers to how easily people can reach and use the transport system. It includes physical, geographic and social factors that determine whether transport is **available to all users.**

```ad-example
title: Examples of accessible transport
- A dense metro network that covers an entire city
- Bus stops within walking distance of most residencies
- Wheelchair-accassible buses and stations
- Real-time apps and wayfinding for better passenger navigation

```

**Affordability** refers to how much passengers **have to pay** for using transport **relative to their 
income**.

```ad-example
title: Examples of affordable transit
- Subsidized metro fares in major cities
- Discounted transport for students, seniors and disabled people
- Free public transport policies
```

#### PT - Types of fares

![Schermata 2025-03-12 alle 17.32.26.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/Schermata%202025-03-12%20alle%2017.32.26.png)


### Public transport generalised cost

PT operations make up for a big part of the cost for a PT system. There are mainly 2 players in terms of cost:
- Operator costs:
	- Infrastructure
	- Vehicles and associated costs
	- Workforce and fleet
- User costs:
	- Time consumption
	- Access
	- Fee

In respect to PT design, both components have to be accounted for and be part of the design process.

One of the most common approaches to network design is the [[Parsimonious models for Public transport network design|Parsimonious models]].


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/parsimonious-models-for-public-transport-network-design/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Parsimonious models for Public transport network design]]


Parsimonious models carry various advantages:
- [p] They have few assumptions and analytically tractable --> they provide a close solution
- [p] Low data requirements
- [p] Low computational complexity
- [p] Better system representation
- [p] Greater transparency
- [p] Higher sharpness or insight

for these reasons they are often used to analyse large transportation systems and can be physically realistic and accurate

They rely on a [[#Continuous approximation method]]:

## Continuous approximation method

This method allows for the development of [[#Parsimonious models]].

It consists in solving an optimisation problem in which we try to minimise the total cost defined as:
$
{\rm Cost_{tot}}= \int_{0}^{L} {\rm cost_{local}}(x) \, dx  
$
where:
- $L$ is the length of the line

Finding the minimum means to derivate the function and set it equal to zero:
$
	\frac{\partial {\rm Cost_{local}}}{\partial s} \stackrel{!}{=} 0 
$

### 1D line

We will start by considering a 1 dimensional system with the following characteristics:
- $2L:$ line length
- $l:$ distance travelled by a generic user
- $\Lambda \,\rm\left[ \frac{pax}{h} \right]:$ demand, *uniformly* distributed along the line length
- $v:$ vehicle cruising speed
- $a:$ vehicle constant acceleration/deceleration
- $\tau':$ boarding and alighting time per passenger
- $v_{w}:$ walking speed

**Decision variables:**
- $s:$ stop spacing (distance between stops)
- $H:$ vehicles headway (time distance between 2 consecutive vehicles)

We need to find the total cost of travelling along the line. We have to distinguish:
- [[#User cost]]
- [[#Operator cost]]

#### User cost

The user cost can be decomposed in 3 components, relating to time:
- $A$ - [[#Access time]]
- $W$ - [[#Waiting time]]
- $IVTT$ - [[#In Vehicle Travel Time]]

From that we will calculate the [[#User Generalised Cost]], as:
$
GC = \beta [A + W + IVTT] + \theta
$
where:
- $\beta:$ value of time $\rm\left[ \dfrac{EUR}{pax \cdot h} \right]$
- $\theta:$ trip fare $\rm\left[ \dfrac{EUR}{pax} \right]$

##### User travel time

###### Access time

The **Access time** is the time it take the passenger to get from their origin to the closest bus stop (or from the stop to the destination).

Imagine we have a stretch of line like in the diagram:

![Parsimonious models for Public transport network design 2025-03-12 18.04.16.excalidraw.png](/img/user/allegati/Parsimonious%20models%20for%20Public%20transport%20network%20design%202025-03-12%2018.04.16.excalidraw.png)
%%[[Parsimonious models for Public transport network design 2025-03-12 18.04.16.excalidraw.md|🖋 Edit in Excalidraw]]%%

Ignoring the transversal distance between the start of the jurney and the closest stop (which cannot be influenced by changing the decision variable), we are interested in the distance that a passenger has to travel to reach the closest stop.

This distance could have any value between $0$ and $\dfrac{s}{2}$. 

Considering the worst case, in which every user has to walk at least $\frac{s}{2}$, the Access time is:

```ad-Teo
title: Access Time (A)

$
A = \frac{s}{2v_{w}}
$

```


###### Waiting time

The **waiting time** is the time a generic passenger has to wait at a bus stop before the bus arrives. 

The extreme cases are:
- The bus arrives exactly at the same time as the user, then the waiting time is $W =0$
- The bus leaves exactly as the user arrives, than they have to wait for the next bus: $W = H$

The average waiting time is:
```ad-Teo
title: Waiting time (W)

$
W = \frac{H}{2}
$

```



###### In Vehicle Travel time

The in vehicle travel time is the time that the generic passenger spends in the vehicle for their trip. It accounts for dwell times and acceleration. It can be divided in 3 components:
1. Time spent travelling at constant speed
2. Time spent accelerating and decelerating
3. Time spent for passengers boarding and alighting

To evaluate these, it's useful to keep in mind a generic trajectory for a bus stopping at a bus stop:

![Parsimonious models for Public transport network design 2025-03-12 18.21.30.excalidraw.png](/img/user/allegati/Parsimonious%20models%20for%20Public%20transport%20network%20design%202025-03-12%2018.21.30.excalidraw.png)
%%[[Parsimonious models for Public transport network design 2025-03-12 18.21.30.excalidraw.md|🖋 Edit in Excalidraw]]%%

**1 - Time spent travelling at constant speed**

If the user travels for a distance $l$ and, at costant speed the vehicle moves with a speed $v$, then, the time spent is:
$
t^{R}(l) = \frac{l}{v}
$
```ad-attention
This slightly overestimates the actual time. This way in fact we are also considering the space where the vehicle is not travelling at constant speed.

```

- [?] This slightly overestimates the actual time. This way in fact we are also considering the space where the vehicle is not travelling at constant speed

**2 - Time spent accelerating and decelerating**

Along the distance travelled, we have $\dfrac{l}{s}$ stops.

At each stop, the time spent accelerating is $\frac{1}{2}\frac{v}{a}$
At each stop, the time spent decelerating is $\frac{1}{2}\frac{v}{a}$

- [?] Shouldn't the acceleration time, according to uniformly accelerated motion, be $\frac{v}{a}$. Why are we using $\frac{1}{2} \frac{v}{a}$? ⏫ 

Then, the time spent not travelling at constant speed at each stop is $2\frac{1}{2}\frac{v}{a}$, and, the total along the passenger journey is:
$
t^{A}(l) = \frac{l}{s} \frac{v}{a}
$


**3 - Time spent for passengers boarding and alighting**

Lastly, we need to account for the dwell time.

In order to calculate this, we need to know how many passengers will board at each bus stop.

- If the general demand per hour is $\Lambda$, then, along the whole corridor, the number of passengers boarding each vehicle will be $\Lambda H$;
- We only have to account for the proportion of travellers along the stretch of length $l$. Therefore, we will need to multiply the demand per bus by $\frac{l}{2L}$;
- For one pax, the dwell time is $\tau'$
 Then, for the whole trip, the time spent stopping for boarding operations is:
 $
 t^{B}(l) = \Lambda H \frac{l}{2L}\tau'
$

**IVTT**:
We can now write the In Vehicle Travel Time as the sum of the aforementioned components:

```ad-Teo
title: In Vehicle Travel Time (IVTT)

$
IVTT(l) = \frac{l}{v} + \frac{l}{s} \frac{v}{a} + \Lambda H \frac{l}{2L \tau'}
$

```


##### User Generalised Cost

The user generalised cost is given by:
$
GC = \beta [A + W + IVTT] + \theta
$
where:
- $\beta:$ value of time $\rm\left[ \dfrac{EUR}{pax \cdot h} \right]$
- $\theta:$ trip fare $\rm\left[ \dfrac{EUR}{pax} \right]$

that we can write explicitly as:
$
GC_{us} = \left[  \frac{s}{2v_{w}} + \frac{H}{2} + \frac{l}{v} + \frac{l}{s} \frac{v}{a} + \Lambda H \frac{l}{2L \tau'}   \right] + \theta
$

###### Time perception

The calculations done in the previous sections does not account for the fact that users perceive time differently depending on what they're doing. Therefore, when calculating the [[#User Generalised Cost]] we should account for this factor. The following table shows average and ranges values for time perception at different phases of the trip:

![Schermata 2025-03-12 alle 18.49.30.png](/img/user/allegati/Schermata%202025-03-12%20alle%2018.49.30.png)


#### Operator costs

The operator costs include mainly these components:
- $L$ - [[#Corridor length]]
- V - Distance travelled by the fleet per hour ([[#Operation]])
- M - [[#Fleet size]] (number of vehicles) and Work force per hour

After having calculated every one of the mentioned components, we can calculate the generalised operator cost:
$
Z_{A}= \text{€}_{L}L + \text{€}_{V}V + \text{€}_{M}M
$
where:
- $\text{€}_{L} \,\,\rm \left[ \dfrac{\text{€}}{km\cdot h} \right]:$ unitary cost of infrastructure per km and hour
- $\text{€}_{V} \,\,\rm \left[ \dfrac{\text{€}}{veh\cdot km} \right]:$ unitary cost based on distance travelled by fleet per hour
- $\text{€}_{M} \,\,\rm \left[ \dfrac{\text{€}}{veh\cdot h} \right]:$ unitary cost for fleet acquisition and crew operation

##### Corridor length

The corridor length is simply a constant:
$
L
$

We do not consider 2L as we are assuming a circular line. Then, the same infrastructure is used in both directions

##### Operation

The operation is caused by the distance travelled by the whole fleet per hour.

If the total length of the line is $2L$, and vehicles travel with a headway of $H$, then:
$
V = \frac{2L}{H}
$

##### Fleet size

The fleet size is given by the total amount of vehicles. In order to get this, we need the time spent by one vehicle to travel the whole corridor and divide it by the headway. The time spent by one vehicle is given by the corridor length over the [[#Commercial speed]].
$
M = \frac{\frac{2L}{v_{c}}}{H} = \frac{V}{v_{c}}
$


###### Commercial speed

The commercial speed is the average speed of a vehicle in a transportation line, accounting for each slow down.

It's given by the total distance in the corridor over the time spent in the corridor (the [[#In Vehicle Travel time]] calculated for a trip length of $l =2L$).

$
v_{c} = \frac{2L}{IVTT(l=2L)} = \frac{2L}{\dfrac{2L}{v} + \dfrac{2L}{s} \tau + \Lambda H \tau'}
$
where $\tau= \frac{v}{a}$.

#### 1D line optimisation problem

The problem to solve is then:
$
\min_{s,H} Z = \min_{s,H} \left[ \text{€}_{L}L + \text{€}_{V}V + \text{€}_{M}M + \Lambda \beta (A + W + IVTT + T_{TR}) \right]
$
subject to:
- $O \le C$
- $s,H \ge 0$

where
- $T_{TR}$ is the transfer time
- $O \,\,\rm[\dfrac{pax}{veh}]:$ Maximum vehicle occupancy during peak hour
- $C:$ vehicle capacity

#### 2D line

A similar problem to the [[#1D line]] can be defined for a 2D line, where transfers between lines are possible.

The easiest example is a grid system:

![Schermata 2025-03-12 alle 19.26.17.png](/img/user/allegati/Schermata%202025-03-12%20alle%2019.26.17.png)



</div></div>



## Network design approaches

When designing a PT network, different approaches can be followed.

One of the biggest difference is in having either a door-to-door line for every use case, or, on the contrary, basing the system on line transfers. They both have they're own advantages and disadvantages.

![Schermata 2025-03-12 alle 19.29.02.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/Schermata%202025-03-12%20alle%2019.29.02.png)

## PT operations

### Bus bunching

```ad-Definizione
title: Bus bunching

Bus **bunching** is a phenomenon in bus systems where 2 vehicles start running one right after the other, leaving a great gap somewhere else in the line.

```

The reason is the random passenger arrivals at the bus stops, since their individual boarding maneuvers delay the buses: if on arriving at a bus stop a bus finds more than the average number of passengers waiting, this bus will likely be delayed relative to the bus that precedes it. As a result the delayed bus may encounter more passengers on succeeding stops, and be delayed further. Further delays imply more passengers, which in turn imply more delay. This positive feedback mechanism is the reason[1]. But things are even worse... because as our bus falls behind schedule, it picks up passengers that should have been collected by the following bus. Thus, the following bus experiences less stopping delay so that it tends to catch up until the two buses eventually pair up and travel as a single unit. As time goes by pairs become bunches, until in the end there is a single moving unit. This is the bunching effect.

Read more about it at: http://faculty.ce.berkeley.edu/daganzo/Research/BusSim/index.html

Transit agencies often attempt to mitigate it by including extra time (slack) into their schedules, and then asking drivers to be punctual at selected control points along the route-even if this means delaying some buses. This method is of limited effectiveness because the slack has to be calculated by assuming a worst case scenario for the bus travel time between consecutive control points along the line, so that buses can stay on schedule despite disruptions. Worst case slack means slow travel times, which is not good for on board passengers-the medicine can be worse than the cure!

Today, as we can know the position of each bus real time, we can adopt real time strategies to avoid bus bunching.

## More

Read more from slides