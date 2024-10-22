---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/topografia-e-positioning/appunti/05-problemi-di-positioning-tp/","tags":["UNI"]}
---

# [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/05 - Problemi di Positioning - TP\|05 - Problemi di Positioning - TP]]

Al fine di impostare un problema di positioning è importante rispettare due principi base, i quali non dipendono dal tipo di strumento e sono valide in generale:
- Comprendere come suddividere il rilievo (dal generale al particolare)
- La ridondanza - serve a tenere sotto controllo gli inevitabili errori e quantificare la loro entità media

In generale, nella risoluzione di un problema, si avranno un certo numero di incognite e un certo numero di equazioni (le [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP\|Equazione di osservazione]]). Il problema può essere in linea teorica risolto già quando $n = m$ ma ci si trova in una condizione di **minima informazione necessaria**: non si sta rispettando il principio di [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/05 - Problemi di Positioning - TP#Ridondanza\|#Ridondanza]].

Aggiungere informazioni ridondanti (e quindi equazioni non indipendenti) però porta a non poter risolvere il problema in forma algebrica. Andrà risolto per via statistica. In questo modo si assolvono i seguenti obiettivi:
- Arrivare ad una soluzione quale che sia la ridondanza
- Quantificare l'effetto degli errori di misura su ciò a cui si è interessati

È necessario pertanto introdurre il concetto di [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/05 - Problemi di Positioning - TP#Principio di stima\|#Principio di stima]]

## Principio di stima

Risolvendo un generico [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/05 - Problemi di Positioning - TP\|Problema di positioning]] nel quale sia contemplata un qualche livello di [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/05 - Problemi di Positioning - TP#Ridondanza\|#Ridondanza]] implica l'impossibilità di giungere a una soluzione algebrica. Occorrerà pertanto stimare la soluzione.

Per comprendere meglio questo problema partiremo da un caso applicativo: una **battuta di livellazione** - [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP\|Livellazione geometrica]]

![05 - Problemi di Positioning - TP 2024-05-26 12.52.37.excalidraw.png](/img/user/Excalidraw/05%20-%20Problemi%20di%20Positioning%20-%20TP%202024-05-26%2012.52.37.excalidraw.png)


La situazione è quella descritta in figura:
- 3 punti: $A,B$ e $C$
- Del punto $A$ si suppone di conoscere la quota esatta

Si procede nel seguente modo.
1. Stabilire un [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|sistema di riferimento]]
	1. Ci troviamo in 1 dimensione: basta fissare un'origine (scelgo il punto $A$)
2. Essendo $O \equiv A$
	1. $H_{A}$ è considerata nota
	2. $H_{B},H_{C}$ sono le incognite del problema
3. $\Delta H_{AB}, \Delta H_{BC}$ sono le **osservabili**
4. $\Delta H_{AB_{O}}, \Delta H_{BC_{O}}$ sono le misurazioni (le **osservazioni**)

In linea teorica si potrebbero misurare i dislivelli $\Delta H_{AB}, \Delta H_{BC}$ e ottenere le quote di $B$ e $C$ come segue:
$$
\begin{cases}
H_{B} &= H_{A} + \Delta H_{AB_{O}} \\
H_{C} &= H_{A} + \Delta H_{AC_{O}}
\end{cases}
$$


