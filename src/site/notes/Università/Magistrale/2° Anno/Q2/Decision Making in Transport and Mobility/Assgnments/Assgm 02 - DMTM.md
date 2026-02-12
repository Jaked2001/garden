---
{"dg-publish":true,"permalink":"/universita/magistrale/2-anno/q2/decision-making-in-transport-and-mobility/assgnments/assgm-02-dmtm/"}
---

# [[Università/Magistrale/2° Anno/Q2/Decision Making in Transport and Mobility/Assgnments/Assgm 02 - DMTM\|Assgm 02 - DMTM]]

Timetabling and Rolling Stock scheduling.


<iframe src="/img/user/Universit%C3%A0/Magistrale/2%C2%B0%20Anno/Q2/Decision%20Making%20in%20Transport%20and%20Mobility/Assgnments/Allegati/1CM110_Assignment2.pdf" width="100%" height="900px" title="1CM110_Assignment2.pdf" style="border:1px solid #ccc;"></iframe>


## Timetabling

![Assgm 02 - DMTM 2025-12-05 18.22.38.excalidraw.png](/img/user/Excalidraw/Assgm%2002%20-%20DMTM%202025-12-05%2018.22.38.excalidraw.png)



- [x] For the headway at arrival, do we do the same considerations that we do at departure? ✅ 2025-12-13
	- [ ] No need. headway at arrival is already gartanteed
- [x] In Std (Sittard), there are 3 tracks leaving the station. There are 2 lines: to Mt and to Hrl. One of the 3 tracks is shared between the 2 lines. How should we treat it? Are the line contrasting? Do they always need headways? ✅ 2025-12-13
	- [ ] Pretend it's not a problem
- [x] [[Screenshot 2025-12-10 at 18.34.42.png]]: should we keep both transfer opportunities? How would we select only the best? ✅ 2025-12-13
	- [ ] Think about it. If you do, it makes it infeasible

## Rolling stock scheduling

Abbink 2004:
- train **classes**: power-driven, diesel-drive, locomotive-driven, locomotive-hauled carriages
	- Train **types**: Koplopers (intercity), Mat'64 (regional)
		- Train **subtypes**: Koplopers 3 cars; Koplopers 4 cars... Mat'64 2 cars and MAt'64 4 cars...
		- Train units of same type can be combined. Train units of different types cannot.
- Train unit: certain number of carriages that cannot be split during operation


In our case, we have
- 1 class
- 1 type: **PLx**.
- 2 subtypes: PL3 and PL4

### The model

We can minimise shortages or cost

$S:$ shortages = number of paxs without a seat

Variables:
- $N_{u,t}:$ Number of trains of type $u$ for cross-section train $t$

constraints:
$$
S_{t} \ge P_{t} - \sum\limits_{u} C_{u} \cdot N_{u,t} \qquad \forall t \in T
$$
$$
\begin{align}
\sum\limits_{u} N_{u,t} &\ge 1 \qquad \forall t \in T \\
\sum\limits_{u} \lambda_{u}N_{u,t} &\le L_{t} \qquad \forall t \in T \\
\sum\limits_{t}N_{1,t} &\le 1.25 \cdot \sum\limits_{t}N_{2,t} \\
\sum\limits_{t}N_{2,t} &\le 1.25 \cdot \sum\limits_{t}N_{1,t}
\end{align}
$$

$$
\begin{align}
S &\ge P - \sum\limits CN \\
S &\ge 0  \\
\end{align}
$$



![Assgm 02 - DMTM 2025-12-14 21.47.45.excalidraw.png](/img/user/Excalidraw/Assgm%2002%20-%20DMTM%202025-12-14%2021.47.45.excalidraw.png)
