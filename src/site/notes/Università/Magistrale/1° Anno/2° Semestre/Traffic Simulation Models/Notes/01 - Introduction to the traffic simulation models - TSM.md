---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/traffic-simulation-models/notes/01-introduction-to-the-traffic-simulation-models-tsm/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Notes/01 - Introduction to the traffic simulation models - TSM\|01 - Introduction to the traffic simulation models - TSM]]


```table-of-contents
```

Often times, we are asked to run 3D simulation of traffic. The only function of a 3D simulation is to look pretty. They take much longer to run and provide no additional information from a 2D simulation.

![Schermata 2025-02-23 alle 17.02.34.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Traffic%20Simulation%20Models/Notes/Allegati/Schermata%202025-02-23%20alle%2017.02.34.png)


## Simulation

As already stated in [[00 - Course introduction - TSM]] I provide again the definition of a simulation:

```ad-Definizione
title: Simulation

A **simulation** is an imitation of the operation and dynamics of a real world (or proposed) process or system over time.

```

### Why do we simulate

An alternative approach to simulation is direct experimentation: trying variating the system in the real world. Simulation has several advantages against real experimentation:
- It's **cheaper** to implement and doesn't disrupt the real system
- It's **faster** to implement
- It can be **replicated** multiple times (needed for statistic porpuses)
- It's **safe** since no real person is actually involved
- It's **ethical** and **legal** since it can also implement changes in policies that would be illegal in the real life


"Another alternative is to use a mathematical model representing the system. However, it is often infeasible, if not impossible, to come up with an exact mathematical model which can faithfully represent the system under study."

- [x] What is the difference between a simulation and a mathematical model. Doesn't the simulation itself come from a mathematical model? ✅ 2025-02-28
	- [ ] The model refers to the translation of the system into a mathematical form. The simulation refers to reproducing the development of the system over time


## What is needed in a simulation

![01 - Introduction to the traffic simulation models - TSM 2025-02-23 17.10.38.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Traffic%20Simulation%20Models/Notes/Allegati/01%20-%20Introduction%20to%20the%20traffic%20simulation%20models%20-%20TSM%202025-02-23%2017.10.38.excalidraw.png)
%%[[01 - Introduction to the traffic simulation models - TSM 2025-02-23 17.10.38.excalidraw.md|🖋 Edit in Excalidraw]]%%

There are mainly 3 elements needed to construct a [[00 - Course introduction - TSM#Traffic simulation models|traffic simulation model]]:
- **[[#The Network]]**
- [[#The Management Schemes]]
- **[[#The demand model (OD matrixes)]]**

### The Network

The network is the easiest thing to obtain. It includes the map (and digital translation) of the system we are interested in. It can be obtained, for example, from [[Open Street Map]].

### The Management Schemes

Management schemes are very hard to obtain. Furthermore, they are often also really hard to implement in the simulation softwares themselves.

They include, for example, the workings of traffic lights in the system. 

### The demand model (OD matrixes)

```ad-note

We could theoretically consider every single door step as a domand generator and attractor, but it would be impractical to run the simulation.

```


Demand models are very well studied but are still quite hard to generate.

We rely mainly on Origin Destination matrixes.

Very good O/D matrix would be every 15 min.
#### Zoning

The first step in studying the demand is **zoning**. We need to divide the system of interest into homogeneous zones. Each zone should have a single land use and all zones should share approximately the same number of trips.

##### Centroids

[[#Zoning|Zones]] are identified by centroids.

```ad-Definizione
title: Centroid

A **centroid** is the point in a zone where we concentrate all the demand (either starting or arriving) of the zone.

```

They leave us with a challenge. They are generally distinct entities from the links and nodes of the network. Therefore, we need [[#Connectors]]

##### Connectors

```ad-Definizione
title: Connectors

**Connectors** are the elemetns that connect centroids to the network itself.

```

 Deciding the connectors introduces a lot of errors into the simulation. In fact, we only use a handful of connectors per zone (to limit computation complexity). This isnt's such an issue in small zones, but becomes quite relevan for big zones since we mind end up assigning demand in very different and far apart parts of the zone.

## Micro- vs Meso- vs Macro- scopic models

There's a difference between:
- [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Notes/01 - Introduction to the traffic simulation models - TSM#Macroscopic models\|#Macroscopic models]]
- [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Notes/01 - Introduction to the traffic simulation models - TSM#Microscopic models\|#Microscopic models]]
- [[#Mesoscopic models]]
They all differ in the level of granularity that represents the studied system (space, time, demand)

### Macroscopic models

See [[03 - Fundamentals of traffic flow modeling - OMT#Macroscopic models|Macroscopic models]]


```ad-Definizione
title: Macroscopic models

**Macroscopic models** are also known as *traffic flow models*, as they focus on macroscopic variables like *traffic flow*.

```


- [p] Short running time
- [p] Very few calibration parameters
- [c] Not able to reproduce some specific traffic behaviour like traffic lights or lane changes

### Microscopic models

See [[03 - Fundamentals of traffic flow modeling - OMT#Microscopic models|Microscopic models]]

```ad-Definizione
title: Microscopic models

**Microscopic models** try to predict how one vehicle follows another vehicle. They fall under the scope of car following theory. They are realistic, very detailed models.

```

- [p] Realistic models
- [p] Very detailed emulation of the system
- [c] High computational costs
- [c] Expensive calibration

```ad-note

If we aggregate the results of a microscopic model, we should be able to obtain the same results of the corresponding macroscopic model.

This is a good validation step to apply every time we run simulations.
```


### Mesoscopic models

```ad-Definizione
title: Mesoscopic

**Mesoscopic models** are models that fall in between [[#Microscopic models]] and [[#Macroscopic models]]. They have some characteristics of both.

For example, they could model micro demand (veh by veh) but not take lane changes into account, or viceversa, model lane changes but rely on macro demand.

```

- [p] Reasonable computational times
- [p] Model only the details of interest
- [p] Few calibration parameters

## Dynamic Traffic Assignment

### Traffic Assignment

```ad-Definizione
title: Traffic Assignment

**Traffic assigmnent** is used to determine how the demand is loaded into the road network providing a way to calculate different traffic variables on network sections.

```

We need to determine the set of routes that people choose from A to B.

What we need:
- Set of routes
- Route cost (time) to find the shortest path


### Dynamic Traffic Assignment (DTA)

```ad-Definizione
title: Dynamic Traffic Assignment (DTA)

**Dynamic Traffic Assignment (DTA)** is an extension of the traffic assignment problem that is able to describe the time and spatial evolution of the traffic patterns into the network.

```

The diagram below shows a general process for DTA:

![DTA structure - 01 - Introduction to the traffic simulation models - TSM 2025-02-28 18.08.30.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Traffic%20Simulation%20Models/Notes/Allegati/DTA%20structure%20-%2001%20-%20Introduction%20to%20the%20traffic%20simulation%20models%20-%20TSM%202025-02-28%2018.08.30.excalidraw.png)
%%[[DTA structure - 01 - Introduction to the traffic simulation models - TSM 2025-02-28 18.08.30.excalidraw|🖋 Edit in Excalidraw]]%%

[[#Dynamic Network Loading]]

This is an iterative process. If The result does not match the reality, then we must reiterate changing some variables. Every time we are running a new simulation (the [[#Dynamic Network Loading]]).

## Dynamic Network Loading

```ad-Definizione
title: Dynamic Network Loading

**Dynamic Network Loading** is the process to efficiently reproduce how network flow propagates along the corresponding paths taking into account the time and a variable traffic demand on each path.

```

DNL models the **propagation of traffic** once vehicles have been assigned to specific routes, considering realistic traffic flow dynamics.

## Traffic simulation softwares

- [[AIMSUN\|AIMSUN]]
- [[SUMO\|SUMO]]
- [[VISUM\|VISUM]]
- [[VISSIM\|VISSIM]]

- [[Dynamit\|Dynamit]]
- [[Dynameq\|Dynameq]]



## Real Projects

- Detection Layout problem
	- Where is best to locate traffic detectors (they can go in traffic lights)
	- Limited amount of detectors that we can install
- ValenciaPort
- In4Mo
- Ride-sharing system

# Important

Demand \ne OD matrix

Demand is made by many OD matrixes.