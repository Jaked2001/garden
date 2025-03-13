---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/public-transport/notes/01-network-design-pt/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/2° Semestre/Public Transport/Notes/01 - Network Design - PT\|01 - Network Design - PT]]

```table-of-contents
```


## Management and planning

```ad-Definizione
title: Planning

**Planning** is to optimise the different elements of a system in order to achieve the optimum output.

```

Quantify the potential effect of deploying a system.

Planning is a rational process from the system's analysis anbd understanding its behaviour, allocates resources effectively in order to reach a target in a future scenario.

## Mobility mutations

- Infrastructure --> services
	- I don't care what infrastructure you need, I care about what service you want to provide, then we pick what infrastructure is best
- Objects --> processes
- Static --> dynamic
	- For example distinguish between pick hour and other times
- Recurrence (pendular trip, commuter) --> singularity
- Infrastructures for people
- Re-engineering mobility
- Information on-line, positioning and tracking


## Urban Planning and economic territory

Usually more **density** results in higher service.

Population density is one of the most important parameter that rules PT planning.

## Transportation system

Core elements:
- **Engine** - power drain
- **Container** - provide protection and carriage
- **Control**
- **Infrastructure way**
But there are many other parts in a transportation system:
- Stakeholders
- Society
- Technology
- Culture
- Business
- Environment
- Energy

```ad-example
title: DRT gone wrong example - Kutsuplus

**Kutsuplus**: One of the first attempt to provide DRT in a big city (Helsinki). It was very well planned, people liked... In the end, the average cost per trip for the bus operator was 18 €/trip (= €/pax). In Barcelona, a bus trip is 2.65 €/pax (we're basically talking of the ticket). For a taxi is 12 €/trip. A taxi in Barcelona is cheaper than a trip with DRT in Helsinki.
```

## Public transport decalogue

1. Minimal demand treshold (Bus is efficient if demand is lower than 6000 pax/h. Tram - 6000-20000 pax/h)
2. Investment + operation + maintenance cost
	 - We need to take into account all costs
3. Minimal frequency and service time period
4. Adequate stations
5. Door-to-door chain
	- All the means of transportation needed to move from the initial starting point to the final destination
6. Information, readability
7. Time competitive

![01 - Network Design - PT 2025-02-18 15.53.59.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Public%20Transport/Notes/Allegati/01%20-%20Network%20Design%20-%20PT%202025-02-18%2015.53.59.excalidraw.png)
%%[[01 - Network Design - PT 2025-02-18 15.53.59.excalidraw.md|🖋 Edit in Excalidraw]]%%

For bus, since you can leverage existing infrastructure, you start from a lower budget.


$\tau$ is the fare

| Demand  | Cost    | Freq    | Income      |
| ------- | ------- | ------- | ----------- |
| $D_{0}$ | $C_{0}$ | $F_{0}$ | $D_0\tau_0$ |
| $D_1$   | $C_1$   | $F_1$   | $D_1\tau_1$ |
If I want to reduce cost I can take different routes:
- Subsidies
- Tolls
- Reduce frequency

Reducing frequency will reduce service and therefore reduce demand. Also cost will probably be reduces:
- $D_{1}<D_{0}$
- $C_{1}<C_{0}$
- $F_{1}< F_{0}$
- $D_1\tau_{1}< D_0\tau_{0}$

If demand for bus reduces even more in favour of private cars, then we create even more problems:
- More congestion
- Travel time on bus will go up
- Operation cost of the bus will also go up

This process is known as the **vicious cycle** of PT. To avoid this, every PT service has to be operated over a minimum service threshold.

## Time perception

It's easy to capture the door to door travel time. But what counts is the perceived travel time

- Access and waiting time are perceived 2/3 times more than travel times
- Transfers are perceived 3 to 4 times more than travel times


## Modal competition

Main advantages of rail transit are right of way and capacity. In urban environment, the less friction is not really relevant since there are many stops.

## Smart ICT in mobility

It's important to keep in mind cause-effect relationship. 


## Transport microeconomics

Let the total cost be
$$
TC = \sum\limits_{i}I_{i}
$$
sum of all the investemnts.
Let $x$ be the *demand*.

Then we define average cost


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/magistrale/1-anno/1-semestre/decision-making-and-economy-in-urban-mobility/notes/01-production-and-cost-functions-in-transport-dme/#average-cost" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



#### Average cost

```ad-Definizione
title: Average Cost ($C_{av}$)
$
C_{av} = \frac{CT}{x}
$

```


</div></div>



and Marginal Cost


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/magistrale/1-anno/1-semestre/decision-making-and-economy-in-urban-mobility/notes/01-production-and-cost-functions-in-transport-dme/#marginal-cost" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



#### Marginal cost

```ad-Definizione
title: Marginal Cost ($C_{ma}$)
$
C_{ma} = \frac{\partial CT}{\partial x}
$

```


</div></div>


Marginal cost in road network is higher than the average cost. In PT is lower.
- **Moggridge paradox**







