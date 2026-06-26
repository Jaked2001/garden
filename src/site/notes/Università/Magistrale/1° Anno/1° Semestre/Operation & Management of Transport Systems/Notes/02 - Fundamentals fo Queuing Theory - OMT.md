---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/operation-and-management-of-transport-systems/notes/02-fundamentals-fo-queuing-theory-omt/","tags":["UNI"],"dg-note-properties":{"aliases":["Fundamentals fo Queuing Theory","Queuing Theory"],"Materia":"OMT","Tipo":"T","Stato":"🟢 Fatto","Slide":null,"PDF":["[2 - Fundamentals of queuing theory - OMT.pdf](/img/user/2%20-%20Fundamentals%20of%20queuing%20theory%20-%20OMT.pdf)"],"Parents":["[[🚦 Operation & Management of Transport Systems|🚦 OMT]]"],"Children":null,"Siblings":["[[03. Variabili Aleatorie#Teoria delle code]]","[[05. Teoria del Deflusso#Teoria delle code]]"],"tags":["UNI"]}}
---


# [[Università/Magistrale/1° Anno/1° Semestre/Operation & Management of Transport Systems/Notes/02 - Fundamentals fo Queuing Theory - OMT\|02 - Fundamentals fo Queuing Theory - OMT]]

```table-of-contents
```


Queues appear when a flow of vehicles, persons or objects wants to receive a service that implies a restriction. Typically, services have a **limited capacity** or are offered only with some **frequency**, which may lead to queues, delays and waits.

The subject that studies queues is referred to Queuing Theory (see also [[03. Variabili Aleatorie#Teoria delle code]], [[05. Teoria del Deflusso#Teoria delle code]]).

Most of the complexities of queuing theory come from the stochastic nature of the processes involved. 


## Components of a queuing system


Server: the restriction
Storage: where the costumer waits
Arrivals: the ones that feed the queue
Departures: the yield after service

![Queuing system diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.01.37.excalidraw.png](/img/user/Excalidraw/Excalidraw-2/Queuing%20system%20diagram%20-%2002%20-%20Fundamentals%20fo%20Queuing%20Theory%20-%20OMT%202024-10-26%2012.01.37.excalidraw.png)
[[Server symbol - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.17.04.excalidraw|🖋 Edit in Excalidraw]][[Decentralized queues diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.20.34.excalidraw|🖋 Edit in Excalidraw]][[Centralized queue diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.22.01.excalidraw|🖋 Edit in Excalidraw]][[Tandem Queues diagram02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 12.27.24.excalidraw|🖋 Edit in Excalidraw]][[Cumulative plot generic - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 15.09.12.excalidraw|🖋 Edit in Excalidraw]][[Cumulative plot interpolation - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 15.24.01.excalidraw|🖋 Edit in Excalidraw]][[Input-Output Diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 16.04.28.excalidraw|🖋 Edit in Excalidraw]][[input-output plus service plus queue diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 16.30.06.excalidraw|🖋 Edit in Excalidraw]][[Input-output diagram - continuous - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.05.26.excalidraw|🖋 Edit in Excalidraw]][[Virtual Arrivals curve - 02 - Fundamentals fo Queuing Theory - OMT 2024-10-26 17.14.37.excalidraw|🖋 Edit in Excalidraw]][[Excess accumulation N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.14.50.excalidraw|🖋 Edit in Excalidraw]][[Average excess accumulation on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.19.33.excalidraw|🖋 Edit in Excalidraw]][[02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.27.37.excalidraw.md|🖋 Edit in Excalidraw]][[02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.17.21.excalidraw|🖋 Edit in Excalidraw]][[Average delay per costumer on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.23.15.excalidraw|🖋 Edit in Excalidraw]][[Little's Formula diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 18.36.38.excalidraw|🖋 Edit in Excalidraw]][[Constructing a departures curve on N-t diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-03 19.24.26.excalidraw|🖋 Edit in Excalidraw]][[Undersaturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-14 15.56.17.excalidraw|🖋 Edit in Excalidraw]][[Exactly saturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.02.44.excalidraw|🖋 Edit in Excalidraw]][[Overly saturated system - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.09.14.excalidraw|🖋 Edit in Excalidraw]][[Tandem queuing system diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.15.08.excalidraw.md|🖋 Edit in Excalidraw]][[02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.20.39.excalidraw|🖋 Edit in Excalidraw]][[02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 16.25.35.excalidraw|🖋 Edit in Excalidraw]][[Centralization is better diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.09.22.excalidraw|🖋 Edit in Excalidraw]][[Optimization introduction diagram - 02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.16.46.excalidraw|🖋 Edit in Excalidraw]][[02 - Fundamentals fo Queuing Theory - OMT 2024-11-17 19.29.05.excalidraw.md|🖋 Edit in Excalidraw]]%%

The objective function is therefore:
$$
\min_{h} \left( \beta C\frac{1}{h} + \frac{1}{2}\lambda\alpha  h \right)
$$
We calculate the first derivative:
$$
\frac{\partial Z}{\partial h} = -\beta C \frac{1}{h^{2}} + \frac{1}{2} \lambda \alpha \stackrel{!}{=}0
$$
from which we get:
$$
\begin{align}
-\beta C \frac{1}{h^{2}} + \frac{1}{2} \lambda \alpha &\stackrel{!}{=}0 \\
\frac{1}{2} \lambda \alpha &= \beta C \frac{1}{h^{2}} \\
\frac{1}{2} \lambda \alpha h^{2} &= \beta C \\
h^{2} = \frac{\beta C}{\frac{1}{2}\lambda \alpha}
\end{align}
$$
which ultimately becomes:
$$
h = \sqrt{\frac{2\beta C}{\lambda \alpha }}
$$
```


## Psychology

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗