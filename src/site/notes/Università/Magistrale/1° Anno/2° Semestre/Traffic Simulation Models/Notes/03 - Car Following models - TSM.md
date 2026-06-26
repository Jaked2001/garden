---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/traffic-simulation-models/notes/03-car-following-models-tsm/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"TSM","Tipo":"T","Stato":"🪶🟡 Scrivere","Slide":null,"PDF":["[Car Following Models Review - M. Paz Linares.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Traffic%20Simulation%20Models/Notes/Allegati/Car%20Following%20Models%20Review%20-%20M.%20Paz%20Linares.pdf)"],"Parents":["[[🖥 Traffic Simulation Models|🖥 TSM]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Notes/03 - Car Following models - TSM\|03 - Car Following models - TSM]]

```table-of-contents
```

Models for exam:
- [x] [[Hidas]] ✅ 2025-04-10
- [x] [[#General Motors]] ✅ 2025-04-10
- [x] [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Notes/03 - Car Following models - TSM#Gipps model (1981)\|#Gipps model (1981)]] ✅ 2025-04-10
- [ ] [[#Mahut]]
- [x] [[#Intelligent Driver Model]] ✅ 2025-04-10
- [x] [[#Newell]] ✅ 2025-04-10
- [x] [[#Krauss]] ✅ 2025-04-10


## Car following model

```ad-Definizione
title: Car following model

A **car following model** describes how a pair of vehicles interacts one with each other.

```

In each CFM we always have a **leader** and a **follower**.

See also: [[04 - Microscopic traffic flow modeling - OMT#Car following models]]

```ad-note
title: Observation

This is not usually stated explicitly (eccepts in Gipps' paper) but, when a leader is not available (very low traffic density), we simply assume the vehicles try to follow free-flow behaviour.
```

There are some aspects to take into account. If we start to allow lane changing, then we need to consider that the leader/follower pairs also change.

We will look into several CFM:

### General Motors

(In this class, we only looked at generations 1, 3 and 5)

Differently from [[🚦 Operation & Management of Transport Systems|🚦 OMT]], we use this notation:
- $\lambda:$ sensitivity
- $T:$ Reaction time


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/04-microscopic-traffic-flow-modeling-omt/#general-motors-car-following-models-1958-1961" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### General motors car-following models (1958-1961)

In the late 50's, American company [[General Motors]] started developing some [[#Car following models]]
They developed several generations of a model. The models were calibrated using real world data.

General Motors car-following models fall under the spectrum of [[stimulus-response model]].

#### GM car following models

```ad-Definizione
title: Stimulus-response models

**Stimulus-response models**, in car-following theory, describe the acceleration of the *follower* as a function of the speed relative to the leader. 
$$
\rm Response = f(stimuli, sensitivity)
$$
```


#### Response

In longitudinal movement, the follower can only react in 2 ways to what the vehicle in front does:
- Accelerate
- Decelerate

The response is therefore measured in terms of follower acceleration:
$$
\ddot{x}_{n+1}(t+\Delta t)
$$


#### Stimulus

#### Sensitivity

measures how attentive you are to traffic.



___

- **Response:** follower acceleration - $\ddot{x}_{n+1}(t+\Delta t)$ - measured at a time $t+\Delta t$ (a reaction time after $t$) - If the stimulus happens at $t$, the response always happens $\Delta t$ after the stimulus
- **Stimulus:** Relative speed - $\dot{x}_{n}(t)-\dot{x}_{n+1}(t)$
- **Sensitivity:** a proportionality factor (or function) - $\alpha$

The general model is always in the form:
$$
\ddot{x}_{n+1}(t+\Delta t) = \alpha(...) \cdot \left[  \dot{x}_{n}(t) - \dot{x}_{n+1}(t)  \right]
$$
Depending on the model generation then, $\alpha$ is expressed as different functions.




#### GM model Generations
#### 1st generation - GM model

In the 1st generation of the [[#General motors car-following models (1958-1961)]] the sensitivity $\alpha$ is considered constant:
$$
\begin{align}
\ddot{x}_{n+1}(t+\Delta t) &= \alpha \cdot \left[  \dot{x}_{n}(t) - \dot{x}_{n+1}(t)  \right] \\
\left[  \mathrm{\frac{m}{s^{2}}}\right] &=  \left[\frac{1}{s}\right] \cdot \left[\frac{m}{s} \right]
\end{align}
$$
The acceleration of the follower is directly proportional to the relative speed between the leader and the follower.

$\alpha$ and $\Delta t$ are considered constant parameters to calibrate.

```ad-note

When [[General Motors\|DM]] tried to calibrate the model, they realized that they weren't able to find a constant falue for $\alpha$. This was instead possible for $\Delta t$.

The sensitivity parameter showed large variability depending on the driving conditions, suggesting that maybe this parameter was not a constant.

```


#### 2nd generation - GM model

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.30.23.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.30.23.excalidraw.png)
[[04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.32.57.excalidraw|🖋 Edit in Excalidraw]][[04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.49.33.excalidraw|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/04 - Microscopic traffic flow modeling - OMT 2024-12-15 17.06.10.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Notes/Allegati/03 - Car Following models - TSM 2025-04-10 19.16.30.excalidraw\|🖋 Edit in Excalidraw]]%%

Type I:
- Big jams
- **Stable** output jam flow
- Phase separation, metastability, capacity drop

Type II:
- Some jamming
- **Unstable** output jam flow
- Phase separation not clear, jams don't scale

Type III:
- No structural jamming
- Homogeneous traffic

