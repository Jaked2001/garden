---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/traffic-simulation-models/assgm/nonlinear-follow-the-leader-models-of-traffic-flow/","tags":["UNI"]}
---



# [[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Assgm/Nonlinear follow-the-leader models of traffic flow\|Nonlinear follow-the-leader models of traffic flow]]

```table-of-contents
```
Follow the leader theory of traffic

Single-lane dense traffic with no passing.

each driver reacts in some specific fashion to a stimulus from the car ahed of and/or behind them.

The theory applies mainly to **dense** traffic.

Basic idea:

$$
\text{response} = \text{sensitivity} \cdot \text{stimulus}
$$

- response is taken as the acceleration of the vehicle as the driver has direct control over this parameter.
- The stimulus is a function fo the position of cars and their time derivatives (speed)

It has been established that there is correlation between driver response and relative speed of their car and the one ahead. **The stimulus is than taken as the relative speed**.

## Equations

$$
\ddot{x}_{n+1} (t+T) = \lambda [\dot{x}_{n}(t) - \dot{x}_{n+1}(t)]
$$
- $x_{n}:$ position of the $n^{tn}$ car
- $T:$ reaction time
- $\lambda:$ sensitivity 

Possible sensitivity functions:
$$
\begin{cases}
1. \,\text{constant} &\lambda = a \\
2. \,\text{step function} &\lambda = \begin{cases}
a,\quad s \le s^{*} \\
b,\quad s > s^{*}
\end{cases} \\
3. \,\text{reciprocal spacing} &\lambda = \dfrac{c}{s}
\end{cases}
$$
where:
- $s = x_{n}- x_{n+1}$ (the spacing)
- $a,b,c$ are constants

General equation:
$$
\lambda = a\frac{\left[\dot{x}_{n+1}(t)\right]^{m}}{[x_{n}(t)-x_{n+1}(t)]^{l}} 
$$
This can lead to some specific forms for the sensitivity:
$$
\begin{cases}
\text{Edie:} \quad &\lambda = c \dfrac{\dot{x}_{n+1}}{s^{2}} \\
\text{Leading to Greenshield:} \quad &\lambda  = \dfrac{c}{s^{2}}
\end{cases}
$$
For the validity of each model, we have to look at 2 things:
- Stability - Only for the linear form (otherwise, too difficult)
	- Same bounds are applied for the non linear cases
		- This is possible as long the nonlinear system only has small perturbations (?piccole oscillazioni?)
- Steady-state flow characteristics

### Steady flow characteristics

For steady-state flow characteristics is possible to obtain a fairly complete description corresponding to any sensitivity given by an equation such as the one used in the following:
$$
\ddot{x}_{n+1}(t+\Delta t) = a\frac{[\dot{x}_{n+1}(t)]^{m}}{[x_{n}(t)-x_{n+1}(t)]^{l}} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ]
$$

- [?] Pag. 547/548. Why does integrating the equation yields the steady-state flow equation?

