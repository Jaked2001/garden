---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/sustainable-mobility/notes/01-basic-of-traffic-flow-and-management-sm/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"SM","Tipo":"T","Stato":"🟠 Studiare","Slide":["[1 - Basic of traffic flow and management - SM.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/1%20-%20Basic%20of%20traffic%20flow%20and%20management%20-%20SM.pdf)","[1.2 - Basic of traffic flow and management - Slides - SM.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/1.2%20-%20Basic%20of%20traffic%20flow%20and%20management%20-%20Slides%20-%20SM.pdf)"],"PDF":null,"Parents":["[[🚲 Sustainable Mobility|🚲 SM]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Magistrale/1° Anno/2° Semestre/Sustainable Mobility/Notes/01 - Basic of traffic flow and management - SM\|01 - Basic of traffic flow and management - SM]]

```table-of-contents
```

## Traffic engineering story

1886: Benz's patent for first motor car

## Traffic flow variables

### Spacing

```ad-Definizione
title: Spacing ($s$)

Spacing is the distance between the front of 2 cars.

```

### Headway

Headway ($h$)
**Headway** is the time between two vehicles (front to front).


### Speed

### Flow

Flow ($Q$) is the number of vehicles observed at a certain point in unit of time.

It's measured in $\rm\left[ \dfrac{veh}{h} \right]$.

### Density

Density is the number of vehicle observed at a certain time per unit of length.

### Time mean Speed

```ad-Definizione
title: Time mean Speed ($TMS$ or $v_{t}$)

The **Time mean Speed** is the average velocity based on time.

$
v_{t} = \frac{\sum\limits_{i=1}^{N}v_{i}}{N}
$

```


- Determine each car speed in one point
- Average them out

### Space mean speed


```ad-Definizione
title: Space mean speed ($SMS$ or $v_{s}$)

The **Space mean speed** is the average velocity based on distance travelled



```

$$
v_{s} = \frac{L}{\sum\limits_{i=1}^{N} \frac{t_{i}}{N}} = \frac{N}{\sum\limits_{i=1}^{N}\frac{1}{v_{i}}} = \frac{\sum\limits_{i=1}^{N}v_{i}}{N}
$$

- Select a road section of knonw length
- Measure the time it takes each veh to go through the section
- Calculate using the formula

### Time space diagram

See:
- [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Trajectories of a traffic stream on a time-space diagram\|01 - Introduction to trajectories Analysis - OMT#Trajectories of a traffic stream on a time-space diagram]]
- [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Traffic stream properties\|01 - Introduction to trajectories Analysis - OMT#Traffic stream properties]]

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ 
❗❗❗❗❗❗❗❗❗❗❗❗
 
I stopped paying attention for a while, since we already did all of this in [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/🚦 Operation & Management of Transport Systems\|🚦 OMT]].


#### Fundamental relationship of traffic

[[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/01 - Introduction to trajectories Analysis - OMT#Fundamental equation of traffic\|01 - Introduction to trajectories Analysis - OMT#Fundamental equation of traffic]]

- $k:$ density
- $q:$ flow

$$
k = \frac{N}{T} = \frac{1}{s} \qquad q = \frac{N}{T} = \frac{1}{h}
$$
$$
u = {\rm \frac{space}{time} } = \frac{s}{h} = \frac{\frac{1}{k}}{\frac{1}{q}} = \frac{q}{k}
$$
therefore:
$$
q=ku
$$

### Traffic flow diagrams

![Schermata 2025-02-27 alle 15.40.11.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/Schermata%202025-02-27%20alle%2015.40.11.png)

![Schermata 2025-02-27 alle 15.40.26.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/Allegati/Schermata%202025-02-27%20alle%2015.40.26.png)

### Importance of traffic variables in sustainability

They directly influence pollution levels by affecting fuel consumption and emissions.

When traffic is heavy, cars move slowly or stop often, increasing emissions per trip.

#### Emission factor

They are values that show how much pollklution a specific source releases into the air, for example grams of CO2 per kilometre.

![01 - Basic of traffic flow and management - SM 2025-02-27 15.46.00.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Sustainable%20Mobility/Notes/Allegati/01%20-%20Basic%20of%20traffic%20flow%20and%20management%20-%20SM%202025-02-27%2015.46.00.excalidraw.png)



## Traffic dynamics



## Traffic distribution in networks

## Traffic control and management

### Software for traffic simulation

- [[AIMSUM\|AIMSUM]]
- [[VISUM\|VISUM]]
- [[VISSIM\|VISSIM]]

See video:

<iframe width="560" height="315" src="https://www.youtube.com/embed/EmYEmTi43sk?si=7oeCsS-p3l7m_XP8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

and:

<iframe width="560" height="315" src="https://www.youtube.com/embed/dvCi38B1WEI?si=BWaquMQQCWquWG6w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


We can model several strategies:

TC and MS (traffic control and management strategies) are methods used to regulate and optimise the flow of vehicles to reduce congestion.
- Dynamic management of speed limits
- Dynamic lane assignment
	- Reversible lanes
	- Dynamic use of hard shoulder
	- High occupancy veh lanes
- Incident management
- Autonomous driving
- Freeway access management
	- Ramp metering

## Macroscopic control and analysis


