---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/traffic-simulation-models/notes/01-introduction-to-the-traffic-simulation-models-tsm/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"TSM","Tipo":"T","Stato":"🟢 Fatto","Slide":["[1 - Introduction to the traffic simulation models - TSM.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Traffic%20Simulation%20Models/Notes/Allegati/1%20-%20Introduction%20to%20the%20traffic%20simulation%20models%20-%20TSM.pdf)"],"PDF":null,"Parents":["[[🖥 Traffic Simulation Models|🖥 TSM]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
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

A **simulation** is an imitation of the operation and dynamics of a real world (or proposed) process or system *over time*.

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
[[DTA structure - 01 - Introduction to the traffic simulation models - TSM 2025-02-28 18.08.30.excalidraw|🖋 Edit in Excalidraw]]%%

[[#Dynamic Network Loading]]

This is an iterative process. If the result does not match the reality, then we must reiterate changing some variables. Every time we are running a new simulation (the [[#Dynamic Network Loading]]).

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