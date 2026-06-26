---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/03-fundamentals-of-traffic-flow-modeling-omt/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"OMT","Tipo":"T","Stato":"🟢 Fatto","Slide":null,"PDF":["[3 - Fundamentals fo traffic flow modeling - OMT.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/3%20-%20Fundamentals%20fo%20traffic%20flow%20modeling%20-%20OMT.pdf)"],"Parents":["[[🚦 Operation & Management of Transport Systems|🚦 OMT]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT\|03 - Fundamentals of traffic flow modeling - OMT]]

```table-of-contents
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/Fn3HMAaEfcQ?si=2lf72dOCaHH4Tdjp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

In traffic flow modeling, we can distinguish between
- Macroscopic models
- Microscopic models

![Schermata 2024-11-30 alle 18.57.20.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Allegati/Schermata%202024-11-30%20alle%2018.57.20.png)


In this chapter we will focus on [[#LWR Traffic flow theory]].

## Macroscopic models

```ad-Definizione
title: Macroscopic models

**Macroscopic models** predict the evolution in time of the macroscopic variables:
- [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Flow\|Flow]] - $q$
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
1. [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Conservation of vehicles\|#Conservation of vehicles]]
2. [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Equation of state\|#Equation of state]]
```

### Conservation of vehicles

Given a control volume (space x time), the number of vehicles that enter the volume and that exit the volume must be equal.

Look at the trajectories in the following diagram:

![Conservation of veh principle graph - 03 - Fundamentals of traffic flow modeling - OMT 2024-11-30 19.13.03.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Conservation%20of%20veh%20principle%20graph%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-11-30%2019.13.03.excalidraw.png)
[[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 16.49.23.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.04.39.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/Congestion regime diagram - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.16.49.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/Greenshield k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.18.32.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.31.49.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/Greenberg k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.35.46.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/Underwood k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.41.25.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/Edie k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.45.41.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 18.25.33.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 12.59.15.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 13.02.39.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 13.07.45.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 13.17.03.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/Acceleration - LWR theory - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 19.02.12.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/Deceleration - LWR - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 19.35.04.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 19.57.32.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-07 20.05.36.excalidraw\|🖋 Edit in Excalidraw]]%%

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


