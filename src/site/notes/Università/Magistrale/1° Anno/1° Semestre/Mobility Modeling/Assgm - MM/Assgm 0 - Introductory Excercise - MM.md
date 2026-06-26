---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/mobility-modeling/assgm-mm/assgm-0-introductory-excercise-mm/","dg-note-properties":{"aliases":null,"Materia":"MM","Tipo":"Es","Stato":"🟢 Fatto","PDF":["[0 - Introductory Ex - MM 1.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Mobility%20Modeling/Assgm%20-%20MM/Allegati/0%20-%20Introductory%20Ex%20-%20MM%201.pdf)"],"Data":"2024-11-01","Parents":["[[📐 Mobility Modeling|📐 MM]]"],"Children":null,"Siblings":null,"tags":null}}
---


# [[Università/Magistrale/1° Anno/1° Semestre/Mobility Modeling/Assgm - MM/Assgm 0 - Introductory Excercise - MM\|Assgm 0 - Introductory Excercise - MM]]



Name (*Name surname*): Matteo Meloni $\qquad\qquad$ID: CA41844HP
# Assgm 0

For the following multi-commodity network:
- 1--> 2 is required to transport g1 =400 flow units of commodity 1
- 3 --> 4 is required to transport g2= 400 flow units of commodity 2

$t_{0}$ = transportation cost per unit

![Schermata 2024-11-03 alle 10.58.30.png\|450](/img/user/Schermata%202024-11-03%20alle%2010.58.30.png)

## Problem a

*Using the corresponding AMPL model solve the problem (it is necessary first to edit the parameters file)*

### Problem a.1

a.1 - *No joint capacity limits at links.*

This is a multi-commodity problem.

We use the `MinCM2.mod` model file in AMPL to solve it. The figure below shows the solution:

The solution has a total cost of **1232**.

![Assgm 0.a.1 - Introductory Excercise - MM 2024-11-03 10.59.57.excalidraw.png\|450](/img/user/Excalidraw/Excalidraw-2/Assgm%200.a.1%20-%20Introductory%20Excercise%20-%20MM%202024-11-03%2010.59.57.excalidraw.png)
[[Excalidraw/Excalidraw-2/Assgm 0.a.2 - Introductory Excercise - MM 2024-11-03 11.25.03.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/Assgm 0.b - Introductory Excercise - MM 2024-11-03 11.37.15.excalidraw\|🖋 Edit in Excalidraw]]%%

In this case the total cost is lower than the one in [[Università/Magistrale/1° Anno/1° Semestre/Mobility Modeling/Assgm - MM/Assgm 0 - Introductory Excercise - MM#Problem a\|#Problem a]]. This is expected. In the single commodity problem, we don't put constraints on where the units go as a function of where they are from. For example, in a), units from node 1 **had** to exit at node 2. Now this is not necessary, and in fact, the optimal solution has them exiting at node 4.