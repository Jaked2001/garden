---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/mobility-modeling/assgm-mm/assgm-0-introductory-excercise-mm/"}
---


# [[Università/Magistrale/1° Anno/1° Semestre/Mobility Modeling/Assgm - MM/Assgm 0 - Introductory Excercise - MM\|Assgm 0 - Introductory Excercise - MM]]



Name (*Name surname*): Matteo Meloni $\qquad\qquad$ID: CA41844HP
# Assgm 0

For the following multi-commodity network:
- 1--> 2 is required to transport g1 =400 flow units of commodity 1
- 3 --> 4 is required to transport g2= 400 flow units of commodity 2

$t_{0}$ = transportation cost per unit

![Schermata 2024-11-03 alle 10.58.30.png|450](/img/user/Schermata%202024-11-03%20alle%2010.58.30.png)

## Problem a

*Using the corresponding AMPL model solve the problem (it is necessary first to edit the parameters file)*

### Problem a.1

a.1 - *No joint capacity limits at links.*

This is a multi-commodity problem.

We use the `MinCM2.mod` model file in AMPL to solve it. The figure below shows the solution:

The solution has a total cost of **1232**.

![Assgm 0.a.1 - Introductory Excercise - MM 2024-11-03 10.59.57.excalidraw.png|450](/img/user/Excalidraw/Excalidraw-2/Assgm%200.a.1%20-%20Introductory%20Excercise%20-%20MM%202024-11-03%2010.59.57.excalidraw.png)


### Problem a.2

*Modify the AMPL model so that joint capacity constraints enter into play. Define the value of these joint capacities so that the solution found in [[#Problem a.1]] is no longer feasible at one or more links.*

The following constraints were added:
$$
u_{59} = 300 \qquad u_{56} = 600
$$
The new solution has a total cost of **1292** and is represented in the following figure:

![Assgm 0.a.2 - Introductory Excercise - MM 2024-11-03 11.25.03.excalidraw.png|450](/img/user/Excalidraw/Excalidraw-2/Assgm%200.a.2%20-%20Introductory%20Excercise%20-%20MM%202024-11-03%2011.25.03.excalidraw.png)



Notice how the constraint $u_{56}$ doesn't affect the solution, given that the upper bound is greater than the optimal amount of units through that same link.

We can see that the new upper bounds limited the amount of goods that could go through link 5-9. Therefore, some good units are rerouted along other links.

## Problem b

*Assume now that there is only a single commodity in the network and that it is necessary to transport 400 & 400 from 1,3 to 2,4 (no capacity limits). Solve the problem using AMPL and compare the solutions with those obtained in a.1). (Hint: adapt and use Mincost.mod, Mincost.dat)*

For this problem, the `MinCost.mod` model was used.

The solution in this case is given by the graph below. The total cost is now equal to **1152**.

![Assgm 0.b - Introductory Excercise - MM 2024-11-03 11.37.15.excalidraw.png|450](/img/user/Excalidraw/Excalidraw-2/Assgm%200.b%20-%20Introductory%20Excercise%20-%20MM%202024-11-03%2011.37.15.excalidraw.png)


In this case the total cost is lower than the one in [[#Problem a]]. This is expected. In the single commodity problem, we don't put constraints on where the units go as a function of where they are from. For example, in a), units from node 1 **had** to exit at node 2. Now this is not necessary, and in fact, the optimal solution has them exiting at node 4.