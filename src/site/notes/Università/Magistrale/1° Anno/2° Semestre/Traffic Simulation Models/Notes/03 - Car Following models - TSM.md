---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/traffic-simulation-models/notes/03-car-following-models-tsm/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Notes/03 - Car Following models - TSM\|03 - Car Following models - TSM]]

```table-of-contents
```


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

There are some aspects to take into account. We we start to allow lane changing, then we need to consider that the leader/follower pairs also change.

We will look into several CFM:

### General Motors

(In this class, we only looked at generations 1, 3 and 5.

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
$
\rm Response = f(stimuli, sensitivity)
$
```


#### Response

In longitudinal movement, the follower can only react in 2 ways to what the vehicle in front does:
- Accelerate
- Decelerate

The response is therefore measured in terms of follower acceleration:
$
\ddot{x}_{n+1}(t+\Delta t)
$


#### Stimulus

#### Sensitivity

measures how attentive you are to traffic.



___

- **Response:** follower acceleration - $\ddot{x}_{n+1}(t+\Delta t)$ - measured at a time $t+\Delta t$ (a reaction time after $t$) - If the stimulus happens at $t$, the response always happens $\Delta t$ after the stimulus
- **Stimulus:** Relative speed - $\dot{x}_{n}(t)-\dot{x}_{n+1}(t)$
- **Sensitivity:** a proportionality factor (or function) - $\alpha$

The general model is always in the form:
$
\ddot{x}_{n+1}(t+\Delta t) = \alpha(...) \cdot \left[  \dot{x}_{n}(t) - \dot{x}_{n+1}(t)  \right]
$
Depending on the model generation then, $\alpha$ is expressed as different functions.




#### GM model Generations
#### 1st generation - GM model

In the 1st generation of the [[#General motors car-following models (1958-1961)]] the sensitivity $\alpha$ is considered constant:
$
\begin{align}
\ddot{x}_{n+1}(t+\Delta t) &= \alpha \cdot \left[  \dot{x}_{n}(t) - \dot{x}_{n+1}(t)  \right] \\
\left[  \mathrm{\frac{m}{s^{2}}}\right] &=  \left[\frac{1}{s}\right] \cdot \left[\frac{m}{s} \right]
\end{align}
$
The acceleration of the follower is directly proportional to the relative speed between the leader and the follower.

$\alpha$ and $\Delta t$ are considered constant parameters to calibrate.

```ad-note

When [[General Motors\|DM]] tried to calibrate the model, they realized that they weren't able to find a constant falue for $\alpha$. This was instead possible for $\Delta t$.

The sensitivity parameter showed large variability depending on the driving conditions, suggesting that maybe this parameter was not a constant.

```


#### 2nd generation - GM model

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.30.23.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.30.23.excalidraw.png)
%%[[04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.30.23.excalidraw|🖋 Edit in Excalidraw]]%%

GM observed that $\alpha$ had too much variation. So, they decided to use 2 different values of $\alpha$

#### 3rd generation - GM model

Since they didn't know at what point you would get a new value of $\alpha$, GM decided to use a linear function to describe $\alpha$:

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.32.57.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.32.57.excalidraw.png)
%%[[04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.32.57.excalidraw|🖋 Edit in Excalidraw]]%%

$
\ddot{x}_{n+1}(t+\Delta t) = \frac{\alpha_{0}}{[x_{n}(t)-x_{n+1}(t)]} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ]
$
where $\alpha_{0}$ is the sensitivity coefficient and is measured in $\rm\left[  \dfrac{m}{s}  \right]$.

So, $\alpha_{0}$ is a speed. It gives the linkage between [[04 - Microscopic traffic flow modeling - OMT|microscopic]] and [[Es 3 - LWR traffic flow theory - OMT|macroscopic]] traffic flow models.

##### Relation between 3rd gen micro model and Greenberg macro model

Integrating the 3rd generation model in time, we get (notice that the relative speed is the derivative of the spacing):
$
\dot{x}_{n+1}(t+\Delta t) = \alpha_{0} \ln{(x_{n}(t)-x_{n+1}(t))} + C
$
In terms of speed:
$
V = \alpha_{0} \ln\left( \frac{C}{k} \right)
$
We can try to find the constant of integration $C$ by the following initial conditions:
$
V = 0 \quad k= k_{j}
$
then:
$
0 = \alpha_{0}\ln{\left( \frac{C}{k_{j}} \right)} \quad \Longrightarrow \quad C = k_{j}
$
and we get:
$
V = \alpha_{0}\ln\left( \frac{k_{j}}{k} \right)
$
which looks exactly like the [[03 - Fundamentals of traffic flow modeling - OMT#Greenberg k-v model (1959)]] with $\alpha_{0} = v_{0}$, which is the optimal speed.

#### 4th generation - GM model

In the 4th generation, they proposed that $\alpha_{0}$ is not constant but dependent on the speed of the follower:
$
\alpha_{0} = \alpha' \dot{x}_{n+1}(t)
$
the model is then
$
\ddot{x}_{n+1}(t+\Delta t) = \frac{\alpha'\dot{x}_{n+1}(t)}{[x_{n}(t)-x_{n+1}(t)]} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ]
$
where
- $\alpha'$ is a-dimensional

This means that how attentive you are,  not only depends on the spacing, but also on the traveling speed (more attentive the faster you go)

! We still have 2 parameters.

#### 5th generation - GM model

2 parameters are added, $n$ and $l$. They have no known physical meaning, but they're useful to hav more flexibility in calibrating the model.

$
\ddot{x}_{n+1}(t+\Delta t) = \frac{\alpha'[\dot{x}_{n+1}(t)]^{n}}{[x_{n}(t)-x_{n+1}(t)]^{l}} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ]
$

All the [[#General motors car-following models (1958-1961)]] are a particular case of the 5th gen model.

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.49.33.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.49.33.excalidraw.png)
%%[[04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.49.33.excalidraw|🖋 Edit in Excalidraw]]%%


</div></div>


### 3 car following model

This is an extension of the [[#General Motors]] models, proposed by Fox-Lemann in 1967. They account for 3 cars at the same time, where the follower is affected both by the leader and the leader's leader stimuli:

$$
\ddot{x}_{n+2}(t+T) = \alpha \dot{x}_{n+2}(t+T) \left[ \omega_{1} \frac{\dot{x}_{n+1}(t)-\dot{x}_{n+2}(t)}{x_{n+1}(t) - x_{n+2}(t)} + \omega_{2} \frac{\dot{x}_{n}(t)-\dot{x}_{n+1}(t)}{x_{n}(t) - x_{n+1}(t)} \right] 
$$

### Collision avoidance models

```ad-Definizione
title: Collision avoidance models

The main principle behind **collision avoidance models** is that a driver will place themselves at a certain distance from the leading vehicle, such that in the event of an emergency stop by the leader, the follower will come to rest without striking the leading vehicle

```

Models that fall under this category are:
- Pipes (1953)
- Gipps (1981)
- Mehut (1999-2001) - improvement over Gipps' model

#### Pipes model (1953)


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/04-microscopic-traffic-flow-modeling-omt/#pipes-car-following-model-1953" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Pipes car-following model (1953)

Pipes' was one of the first [[#Car following models]] ever proposed.

It comes from the [[California Driving Code]]. The code stated: "*Drivers should leave a gap of one vehicle length for every $10\,\rm mph$ of traveling speed."*

This translates to:

```ad-Teo
title: Pipes model (1953)

![04 - Microscopic traffic flow modeling - OMT 2024-12-15 17.06.10.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-15%2017.06.10.excalidraw.png)



According to the Pipes model, *Drivers should leave a gap of one vehicle length for every $10\,\rm mph$ of traveling speed*:
$
s_{n+1}(t) = l_{n+1} + \frac{\dot{x}_{n+1}(t)}{10\,\rm mph}l_{n+1}
$

```

This model works quite well although:
- For low speeds, it yields spacing considerably lower than the measured one
- It only works for heavy traffic (this is true for any car following model)

This model is incredibly simple: in fact it has only 1 parameter: the follower length $l_{n+1}$.


</div></div>


#### Gipps model (1981)

The principle is to keep a safe distance from the leading vehicle to avoid crashing.

It's a **time discrete** model, meaning it needs time steps.

```ad-info
title: Properties
According to Gipps, the model should have the following properties:
- Model should mimic behaviour of real traffic
- Parameters should have physical meaning on driver and vehicle (easy calibration)
- Time step = reaction time
```

This model basically works as an optimization problem where the user wants to maximize their speed according to 2 constrains:
- **Acceleration constraint**: each vehicle has a maximum acceleration it can be subject to
- **Safety constraint**: the trajectory of each vehicle is affected by that of the vehicle in front

Gipps uses the following notation:
- $\tau:$ reaction time
- $V_{n}:$ derived speed of vehicle $n$
- $a_{n}:$ maximum acceleration with the driver of vehicle $n$ wishes to undertake
- $b_{n}:$ most severe braking for vehicle $n$
- $s_{n-1}:$ effective length of vehicle $n-1$
- $\hat{b}_{n-1}:$ estimated most severe braking for vehicle $n-1$ (empirically)

**ACCELERATION:**
$$
v_{n}(t+\tau) = v_{n}(t) + 2.5 a_{n}\tau \left( 1- \frac{v_{n}(t)}{V_{n}} \right)\left( \sqrt{0.025 + \frac{v_{n}(t)}{V_{n}}} \right)
$$
**SAFETY:**
$$
v_{n}(t+\tau) = b_{n}\tau + \sqrt{b_{n}^{2}\tau ^{2} - b_{n}[2(x_{n-1}(t))-s_{n-1}-x_{n}(t)]} \cdot \sqrt{-v_{n}(t)\tau - \frac{v_{n-1}(t)^{2}}{\hat{b}_{n-1}}}
$$
After estimating both quantities, Gipps selects the minimum value of speed between the two, and assigns that to the vehicle.