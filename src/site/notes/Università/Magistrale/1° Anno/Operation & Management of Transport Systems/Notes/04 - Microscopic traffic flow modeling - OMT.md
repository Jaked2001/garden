---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/operation-and-management-of-transport-systems/notes/04-microscopic-traffic-flow-modeling-omt/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/04 - Microscopic traffic flow modeling - OMT\|04 - Microscopic traffic flow modeling - OMT]]

```table-of-contents
```

## Introduction

Microscopic traffic flow modeling falls under the scope of **[[Car following theory]]**.

This kind of theories work well only for [[03 - Fundamentals of traffic flow modeling - OMT#Heavy traffic|heavy traffic]] conditions.


## Definitions

![04 - Microscopic traffic flow modeling - OMT 2024-12-12 16.12.22.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-12%2016.12.22.excalidraw.png)
%%[[04 - Microscopic traffic flow modeling - OMT 2024-12-12 16.12.22.excalidraw.md|🖋 Edit in Excalidraw]]%%

2 vehicles follow each-other.

The vehicle in front is referred to as **Leader** and is vehicle $n$ of all the vehicles on the road. The following vehicle is referred to as **Follower** and is vehicle $n+1$.

Some parameters:
- $l_{n},l_{n+1}:$ length of the vehicles
- $g_{n+1}:$ The gap between the follower and the leader
- $s_{n+1} = l_{n+1}+g_{n+1}:$ The [[01 - Introduction to trajectories Analysis - OMT#Spacing|spacing]] of the follower vehicle

## Introduction

The objective of microscopic traffic flow modeling is trying to predict the trajectories of individual vehicles on space and time. The movement has 2 components:
- Longitudinal - Moving along the axis of the road
- Lateral - ie Lane changes

In this chapter we will only look at longitudinal models.

Spacing in central for 2 concepts:
- Traffic safety
- Infrastructure capacity

### Safety vs flow

Spacing needs to ensure that drivers can react and adapt to new speeds of vehicles in front without colliding. In terms of safety, the larger the spacing, the safer. In contrast, a large spacing, at equivalent speed, causes a reduction in capacity of the infrastructure:
$$
q = \frac{v}{s}
$$
In terms of capacity, it would be ideal to have high speed and small spacing.

On the road, spacing is left to the driver perception of risk. It's the drivers that evaluates and decides what is the appropriate trade-off for each situation to guarantee safety. In other kind of transportations, like trains, it's the infrastructure that tells the driver the spacing, or better, it forces the appropriate spacing.

![04 - Microscopic traffic flow modeling - OMT 2024-12-12 16.47.17.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-12%2016.47.17.excalidraw.png)
%%[[04 - Microscopic traffic flow modeling - OMT 2024-12-12 16.47.17.excalidraw.md|🖋 Edit in Excalidraw]]%%
#### Automated driving

Automated driving promises to brake the trade-off [[#Safety vs flow]].

Autonomous vehicles can achieve very short reaction times. If we assume that all vehicles are able to communicate with each other, then the reaction time is barely the time it takes the information to travel from one veh to the other. The order of magnitude is $1 \,\rm ms$. Also, because of communication, all veh are able to react together even without line of sight.

Therefore, Autonomous vehicles should be able to travel with very little spacing.

The diagram shown in [[#Safety vs flow]], with autonomous vehicles, could become more similar to the following:

![04 - Microscopic traffic flow modeling - OMT 2024-12-15 12.39.20.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-15%2012.39.20.excalidraw.png)
%%[[04 - Microscopic traffic flow modeling - OMT 2024-12-15 12.39.20.excalidraw.md|🖋 Edit in Excalidraw]]%%

Notice how the spacing will be fairly constant, despite the speed, in heavy traffic, to a point where spacing is not dependent on speed anymore in light traffic.

##### Platooning

What [[#Automated driving]] is supposed to achieve is known as platooning.

Platooning is a condition where many vehicles travel as if they were one, connected as a train.

## Car following models

Several [[#04 - Microscopic traffic flow modeling - OMT|microscopic models]] were proposed during the years. Here we will see some of them. In order to study them, it's important to first understand the following graph:

![04 - Microscopic traffic flow modeling - OMT 2024-12-15 16.32.28.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-15%2016.32.28.excalidraw.png)
%%[[04 - Microscopic traffic flow modeling - OMT 2024-12-15 16.32.28.excalidraw.md|🖋 Edit in Excalidraw]]%%

From now on we will have to account for the vehicles length, hence, each vehicle is represented by a pair of trajectories (one for the front and one for the tail of each vehicle). All the main parameters are shown in the graph:
- ${\color{purple} h_{n+1}}:$ headway
- ${\color{red} g_{n+1}}:$ gap
- ${\color{green} l_{n+1}}:$ vehicle length
- ${\color{blue} s_{n+1}}:$ spacing
- ${\color{orange} \dot{x}_{n} {\color{black},}\dot{x}_{n+1}}:$ vehicles speed

The following relations can be deduced:
$$
\begin{align}
s_{n+1}(t) &= l_{n+1} + g_{n+1}(t) \\
s_{n+1}(t) &= h_{n+1}(t) \cdot \dot{x}_{n+1} (t)
\end{align}
$$

Now we are ready to see several models. Specifically, we will see:
- [[#Pipes car-following model (1953)]]
- [[#Forbes car-following model (1958)]]
- [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/04 - Microscopic traffic flow modeling - OMT#General motors car-following models (1958-1961)\|#General motors car-following models (1958-1961)]]

### Pipes car-following model (1953)

Pipes' was one of the first [[#Car following models]] ever proposed.

It comes from the [[California Driving Code]]. The code stated: "*Drivers should leave a gap of one vehicle length for every $10\,\rm mph$ of traveling speed."*

This translates to:

```ad-Teo
title: Pipes model (1953)

![04 - Microscopic traffic flow modeling - OMT 2024-12-15 17.06.10.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-15%2017.06.10.excalidraw.png)



According to the Pipes model, *Drivers should leave a gap of one vehicle length for every $10\,\rm mph$ of traveling speed*:
$
s_{n+1}(t) = l_{n+1} + \frac{\dot{x}_{n+1}(t)}{10\,\rm mph}l_{n+1}
$

```

This model works quite well although:
- For low speeds, it yields spacing considerably lower than the measured one
- It only works for heavy traffic (this is true for any car following model)

This model is incredibly simple: in fact it has only 1 parameter: the follower length $l_{n+1}$.

### Forbes car-following model (1958)

In 1958, Forbes introduced [[Reaction time (traffic)]] $(\Delta t)$ into the model.

It was proposed that, in order to avoid collisions, the time gap between 2 vehicles should be at least equal to the reaction time.

Therefore, the headway should be the reaction time $\Delta t$ *plus* the time it takes the vehicle to cover one vehicle length $\dfrac{l_{n+1}}{\dot x_{n+1}(t)}$.
$$
h_{n+1}(t) = \Delta t + \frac{l_{n+1}}{\dot x_{n+1}(t)}
$$

Since the spacing is given by
$$
s_{n+1}(t) = h_{n+1}(t) \cdot \dot{x}_{n+1} (t)
$$
Forbes model, formulated in terms of spacing, then becomes:
$$
\begin{align}
s_{n+1}(t) &= \left( \Delta t + \frac{l_{n+1}}{\dot x_{n+1}(t)} \right) \dot{x}_{n+1}(t) = \\
&= l_{n+1} + \Delta t \cdot \dot{x}_{n+1}
\end{align}
$$

```ad-Teo
title: Forbes model (1958)
$
s_{n+1}(t)= l_{n+1} + \Delta t \cdot \dot{x}_{n+1}
$
```

Like [[#Pipes car-following model (1953)|pipes' model]], this is also linear. This time though, it is dependent on a parameter that is not fixed, meaning the model can be calibrated to better describe the specific traffic observed.


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

In the 1st generation of the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/04 - Microscopic traffic flow modeling - OMT#General motors car-following models (1958-1961)\|#General motors car-following models (1958-1961)]] the sensitivity $\alpha$ is considered constant:
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

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.30.23.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.30.23.excalidraw.png)


GM observed that $\alpha$ had too much variation. So, they decided to use 2 different values of $\alpha$

#### 3rd generation - GM model

Since they didn't know at what point you would get a new value of $\alpha$, GM decided to use a linear function to describe $\alpha$:

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.32.57.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.32.57.excalidraw.png)


$$
\ddot{x}_{n+1}(t+\Delta t) = \frac{\alpha_{0}}{[x_{n}(t)-x_{n+1}(t)]} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ]
$$
where $\alpha_{0}$ is the sensitivity coefficient and is measured in $\rm\left[  \dfrac{m}{s}  \right]$.

So, $\alpha_{0}$ is a speed. It gives the linkage between [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/04 - Microscopic traffic flow modeling - OMT\|microscopic]] and [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Problems/Es 3 - LWR traffic flow theory - OMT\|macroscopic]] traffic flow models.

##### Relation between 3rd gen micro model and Greenberg macro model

Integrating the 3rd generation model in time, we get (notice that the relative speed is the derivative of the spacing):
$$
\dot{x}_{n+1}(t+\Delta t) = \alpha_{0} \ln{(x_{n}(t)-x_{n+1}(t))} + C
$$
In terms of speed:
$$
V = \alpha_{0} \ln\left( \frac{C}{k} \right)
$$
We can try to find the constant of integration $C$ by the following initial conditions:
$$
V = 0 \quad k= k_{j}
$$
then:
$$
0 = \alpha_{0}\ln{\left( \frac{C}{k_{j}} \right)} \quad \Longrightarrow \quad C = k_{j}
$$
and we get:
$$
V = \alpha_{0}\ln\left( \frac{k_{j}}{k} \right)
$$
which looks exactly like the [[Università/Magistrale/1° Anno/Operation & Management of Transport Systems/Notes/03 - Fundamentals of traffic flow modeling - OMT#Greenberg k-v model (1959)\|03 - Fundamentals of traffic flow modeling - OMT#Greenberg k-v model (1959)]] with $\alpha_{0} = v_{0}$, which is the optimal speed.

#### 4th generation - GM model

In the 4th generation, they proposed that $\alpha_{0}$ is not constant but dependent on the speed of the follower:
$$
\alpha_{0} = \alpha' \dot{x}_{n+1}(t)
$$
the model is then
$$
\ddot{x}_{n+1}(t+\Delta t) = \frac{\alpha'\dot{x}_{n+1}(t)}{[x_{n}(t)-x_{n+1}(t)]} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ]
$$
where
- $\alpha'$ is a-dimensional

This means that how attentive you are,  not only depends on the spacing, but also on the traveling speed (more attentive the faster you go)

! We still have 2 parameters.

#### 5th generation - GM model

2 parameters are added, $n$ and $l$. They have no known physical meaning, but they're useful to hav more flexibility in calibrating the model.

$$
\ddot{x}_{n+1}(t+\Delta t) = \frac{\alpha'[\dot{x}_{n+1}(t)]^{n}}{[x_{n}(t)-x_{n+1}(t)]^{l}} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ]
$$

All the [[#General motors car-following models (1958-1961)]] are a particular case of the 5th gen model.

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.49.33.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.49.33.excalidraw.png)


## Traffic stability

The kind of equations we setup in the [[#General motors car-following models (1958-1961)]] define an oscillatory movement.

![04 - Microscopic traffic flow modeling - OMT 2024-12-16 16.55.53.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/04%20-%20Microscopic%20traffic%20flow%20modeling%20-%20OMT%202024-12-16%2016.55.53.excalidraw.png)


We can look at an **instability parameter**, found from the models:
$$
C = \alpha \cdot \Delta t
$$
Notice that $C$ is a-dimensional.

It can be shown that traffic is stable if:
$$
C \le 0.5
$$
If $C> 0.5$ you get unstable traffic: overreaction.

This condition is valid for **asymptotic stability**: it's not only a pair of veh, it's a long queue of vehicles.

