---
{"dg-publish":true,"permalink":"/time-to-collision-ttc/"}
---

# [[Time-To-Collision (TTC)\|Time-To-Collision (TTC)]]

```ad-Definizione
title: Time To Collision (TTC)

The time that remains until a collision between two vehicles would have occured if the collision course and speed difference are maintained (https://resolver.tudelft.nl/uuid:8fb40be7-fae1-4481-bc37-12a7411b85c7: a time-based analysis of read user behaviour in normal and critical encounters)

**TTC** is the time until a colllision between the vehicles would occur if they kept their present course at their present rates ([[Università/Magistrale/Master Thesis/Literature/Intersection Safety Assessment Using Video-Based Traffic Conflict Analysis - The Case Study of Thailand\|Intersection Safety Assessment Using Video-Based Traffic Conflict Analysis - The Case Study of Thailand]])
```

Source: 
- 

$$
TTC_{i}(t) = \frac{X_{i-1}(t)-X_i(t)-l_{i}}{V_{i}(t)-V_{i-1}(t)}
$$
where:
- $X_{i}(t):$ Position of vehicle $i$
- $X_{i-1}(t)-X_{i}(t):$ Relative distance
- $V_{i}(t):$ Speed of vehicle $i$
- $V_{i}(t)-V_{i-1}(t):$ Relative speed
- $l_{i}:$ Length of vehicle $i$

If I understand correctly, this is defined at any point in space-time (even if the objects are not on collision course, but are tracing conflicting trajectories). The minumum value of $TTC$ calculated is $TTC_{min}$. 
If the vehicles are on a collision course, the last value of $TTC$ calculated before an evasive action is the $TA$ ([[Time To Accident (TA)\|Time To Accident (TA)]]).
- [?] Can TTC decrease and increase in an event before an evasive action is taken?

([[Università/Magistrale/Master Thesis/Literature/Intersection Safety Assessment Using Video-Based Traffic Conflict Analysis - The Case Study of Thailand\|Intersection Safety Assessment Using Video-Based Traffic Conflict Analysis - The Case Study of Thailand]]) defines TTC as:
$$
TTC = \frac{S}{CS}
$$
where:
- $S:$ conflict distance - relative distance from the position of vehicle taking the evasive action to the potential conflict point
- $CS:$ conflict speed - speed of the relevant vehicle while taking the evasive action


## Critical TTC values

Generally, TTC lower than the perception and reaction time should be considered unsafe ([[Università/Magistrale/Master Thesis/Literature/Application of proximal surrogate indicators for safety evaluation - A review of recent developments and research needs\|Application of proximal surrogate indicators for safety evaluation - A review of recent developments and research needs]])

![Screenshot 2026-02-11 at 12.25.29.png](/img/user/allegati/Screenshot%202026-02-11%20at%2012.25.29.png)

Thresholds values according to [[Intersection Safety Assessment Using Video-Based Traffic Conflict Analysis - The Case Study of Thailand]]

![Screenshot 2026-02-12 at 11.35.31.png](/img/user/allegati/Screenshot%202026-02-12%20at%2011.35.31.png)

