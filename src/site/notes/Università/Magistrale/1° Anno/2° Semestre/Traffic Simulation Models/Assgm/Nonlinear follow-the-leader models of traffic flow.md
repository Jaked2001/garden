---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/traffic-simulation-models/assgm/nonlinear-follow-the-leader-models-of-traffic-flow/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"TSM","Tipo":"Es","Stato":"🟢 Fatto","Slide":null,"PDF":["[Nonlinear follow the leader models of traffic flow - Gazis, Herman, Rothery - 1961.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Traffic%20Simulation%20Models/Assgm/Allegati/Nonlinear%20follow%20the%20leader%20models%20of%20traffic%20flow%20-%20Gazis,%20Herman,%20Rothery%20-%201961.pdf)"],"Parents":["[[🖥 Traffic Simulation Models|🖥 TSM]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
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
\ddot{x}_{n+1} (t+T) = \lambda [\dot{x}_{n}(t) - \dot{x}_{n+1}(t)] \qquad (2)
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
\text{Edie:} \quad &\lambda = c \dfrac{\dot{x}_{n+1}}{s^{2}} \qquad (6)\\
\text{Leading to Greenshield:} \quad &\lambda  = \dfrac{c}{s^{2}} \qquad (7)
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
\ddot{x}_{n+1}(t+\Delta t) = a\frac{[\dot{x}_{n+1}(t)]^{m}}{[x_{n}(t)-x_{n+1}(t)]^{l}} [ \dot{x}_{n}(t) - \dot{x}_{n+1}(t) ] \qquad (9)
$$

- [x] Pag. 547/548. Why does integrating the equation yields the steady-state flow equation? ✅ 2025-04-18


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/03-fundamentals-of-traffic-flow-modeling-omt/#greenshield-k-v-model" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



##### Greenshield k-v model

![Schermata 2024-12-06 alle 17.14.15.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Schermata%202024-12-06%20alle%2017.14.15.png)

The figure above shows the original Greenshield k-v model. He described the average speed as a function of density, requaring 2 calibration parameters



```ad-Definizione
title: The Greenshield $k-v$ model

![Greenshield k-v model - 03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.18.32.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Operation%20&%20Management%20of%20Transport%20Systems/Notes/Allegati/Greenshield%20k-v%20model%20-%2003%20-%20Fundamentals%20of%20traffic%20flow%20modeling%20-%20OMT%202024-12-06%2017.18.32.excalidraw.png)
[[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/Allegati/03 - Fundamentals of traffic flow modeling - OMT 2024-12-06 17.31.49.excalidraw\|🖋 Edit in Excalidraw]][[Università/Magistrale/1° Anno/2° Semestre/Traffic Simulation Models/Assgm/Allegati/Nonlinear follow-the-leader models of traffic flow 2025-04-12 18.57.22.excalidraw\|🖋 Edit in Excalidraw]]%%