---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/08-strumenti-di-misura-tp/"}
---

# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP\|08 - Strumenti di misura - TP]]



Nella topografia ci sono 3 grandezze di particolare interesse. Queste sono:
- Angoli
- Distanze
- Dislivelli
Tutte e 3 sono grandezze **osservabili**.

## Livellazione geometrica

La **livellazione geometrica** misura il dislivello ortometrico

Dislivello: Il dislivello ortonormale tra $A$ e $B$ è la differenza tra la [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Quota Ortometrica\|quota ortometrica]] di A e quella di B. La quota ortometrica si intende valutata rispetto al geoide e misurata lungo le linee di forza del campo di gravità.

Per quanto riguarda questa parte, si considererà come quota di un punto, $H$, quella ottenuta proiettando il punto sul geoide geometricamente.

Quota: Distanza di un punto da una superficie (il geoide)
$$
\Delta = qA - qB
$$

```ad-note
title: Osservazione
Nella topografia si misurano **dilsivelli** e non **quote assolute**. Quest'ultime si ottengono a partire da un punto a una quota nota.

```

```ad-attention
D'ora in poi si approssimerà il geoide come una sfera. Questa cosa è vera se i punti di interesse sono abbastanza vicini tra loro ($D<100 \,\rm m$).

```


### Livellazione Idrostatica

```ad-Definizione
title: Livellazione idrostatica

La **livellazione idrostatica** è un metodo di misura dell'altezza relativa di un punto rispetto ad un altro che sfrutta il [[Principio dei vasi comunicanti]].

```

![Livellazione Geometrica 2024-03-22 16.13.59.excalidraw.png](/img/user/Excalidraw/Livellazione%20Geometrica%202024-03-22%2016.13.59.excalidraw.png)


Sono necessari, per effettuare la misurazione:
- Un $\color{green}\text{tubo}$ in cui far passare acqua
- Delle $\color{orange} \rm stadie$: Sono delle aste graduate necessarie a misurare i livelli dell'acqua

Avremo che l'acqua alle estremità dei due punti si andrà a posizionare alla stessa superficie di livello (superficie piezometrica). Questa disterà $d$ dal geoide. Potremo quindi scrivere
$$
L_{A} + H_{A} = L_{B} + H_{B}
$$
È evidente quindi che, il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Dislivello\|#Dislivello]] tra i due punti possa essere espresso come
$$
\Delta H_{AB} = H_{B}-H_{A} = L_{A}-L_{B}
$$

### Livellazione geometrica con cannocchiale

Tra i metodi più comuni di misurazione del [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#dislivello\|#dislivello]] tra due punti vi è quello che fa uso di un cannocchiale.

Gli strumenti necessari sono:
- Un cannocchiale ad asse orizzontale (è pertanto dotato di una livella)
- 2 stadie verticali (dotate di livella)
- Capisaldi: dispositivi che materializzano i punti

Le stadie sono solitamente rinforzate con [[Inuar\|Inuar]]. Questo è un materiale estremamente resistente alle deformazioni termiche e permette di assicurarsi che le misure che si leggono sulle stadie non siano falsate da eventuali deformazioni delle stadie stesse.

La livellazione con cannocchiale può avvenire essenzialmente in due modi:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Livellazione dal mezzo\|#Livellazione dal mezzo]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Livellazione reciproca\|#Livellazione reciproca]]


#### Livellazione dal mezzo

La **livellazione dal mezzo** è un metodo di [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Livellazione geometrica con cannocchiale\|#Livellazione geometrica con cannocchiale]] che consiste nel posizionare il cannocchiale sull'asse che separa i due punti di cui si vuole conoscere il dislivello. Idealmente si posiziona esattamente sul punto medio.

![03 - Livellazione Geometrica - TP 2024-03-29 11.44.45.excalidraw.png](/img/user/Excalidraw/03%20-%20Livellazione%20Geometrica%20-%20TP%202024-03-29%2011.44.45.excalidraw.png)


La livellazione dal mezzo fa uso della seguente strumentazione
- 2 stadie *verticali* - dotate di livella
- Cannocchiale con asse *orizzontale* - dotato di livella
- Capisaldi - permettono la materializzazione dei punti

La livellazione dal mezzo consiste nel leggere l'altezza sulle stadie guardando attraverso il cannocchiale. 

Nel diagramma si è tracciata con una linea tratteggiata grigia la <mark style="background: #CACFD9A6;">superficie equipotenziale</mark> passante per il cannocchiale. In rosso invece, si è tracciata la linea <mark style="background: #FF5582A6;">orizzontale di vista dal cannocchiale</mark>. Sulle stadie si leggerà pertanto la quota in corrispondenza della linea rossa, quando siamo interessati a quella sulla grigia.

Lo zero delle stadie è posizionato sulla superficie terrestre. Da cannocchiale si leggerà pertanto la <mark style="background: #BBFABBA6;">quota</mark> $L_{A}$ ed $L_{B}$ rispettivamente per i punti $A$ e $B$. 

Siamo interessati a calcolare il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#dislivello\|#dislivello]] $\Delta H_{AB} = H_{B}-H_{A}$.

Essendo la linea tratteggiata in grigio una superficie equipotenziale, la sua distanza dal geoide è costante e pari a $d$.
$$
d = H_{A}+l_{A} = H_{B}+l_{B}
$$
Posso pertanto misurare $\Delta H_{AB}$ come
$$
\Delta H_{AB} = H_{B}-H_{A} = l_{A}-l_{B}
$$
Notiamo che le $l_{A}$ ed $l_{B}$ sono rispettivamente uguali a:
$$
\begin{align}
l_{A} = L_{A}-\delta L_{A} \\
l_{B} = L_{B}-\delta L_{B}
\end{align}
$$
dove, ammesso che il cannocchiale sia posizionato nel punto medio tra i punti $A$ e $B$, vale
$$
\delta L_{A} = \delta L_{B} = \delta L
$$
Pertanto:
$$
\begin{align}
\Delta H_{AB} &= H_{B}-H_{A} = \\
&= l_{A}-l_{B} = \\
&= L_{A} - \delta L_{A} - L_{B} + \delta L_{B} = \\
&= L_{A} - \cancel{\delta L} - L_{B} + \cancel{\delta L} = \\
&= L_{A}-L_{B} 
\end{align}
$$

##### Errori - livellazione dal mezzo

###### Non orizzontalità del cannocchiale

Ogni cannocchiale presenta, per costruzione, un angolo tra l'orizzontale reale e quello indicato dalla livella. In ogni caso, anche quando la livella dovesse segnare che il cannocchiale è perfettamente orizzontale, la linea di vista non lo sarà esattamente.

![03 - Livellazione Geometrica - TP 2024-03-29 19.13.52.excalidraw.png](/img/user/Excalidraw/03%20-%20Livellazione%20Geometrica%20-%20TP%202024-03-29%2019.13.52.excalidraw.png)


Per via di questo ulteriore errore, l'altezza reale, $l$ sarà:
$$
\begin{align}
l_{A} = L_{A} - \delta L_{A} - \frac{D}{2} \varepsilon \\
l_{B} = L_{B} - \delta L_{B} - \frac{D}{2} \varepsilon
\end{align}
$$
Essendo l'errore per la non orizzontalità del cannocchiale lo stesso da entrambi i lati, questo termine di errore si cancella quando si va a calcolare il dislivello $\Delta H_{AB}$ e può pertanto non essere valutato.


###### Non verticalità della stadia

❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗

###### Rifrazione atmosferica

A causa della temperatura variabile lungo il percorso tra il cannocchiale e le stadie si possono generare fenomeni di rifrazione per cui la lettura può avere degli errori.

Questa differenza di temperatura dipende dalla copertura del suolo. Posso, per limitare questo errore, cercare di effettuare misure in modo che il suolo sia lo stesso.


#### Livellazione reciproca

La **livellazione dal reciproca** è un metodo di [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Livellazione geometrica con cannocchiale\|#Livellazione geometrica con cannocchiale]] che consiste nell'effettuare due misure speculari.

Si vuole misurare il dislivello tra i punti $i$ e $j$. Si eseguono le misure dai punti $A$ e $B$.

![03 - Livellazione Geometrica - TP 2024-03-29 19.25.23.excalidraw.png](/img/user/Excalidraw/03%20-%20Livellazione%20Geometrica%20-%20TP%202024-03-29%2019.25.23.excalidraw.png)


<mark style="background: #ADCCFFA6;">Cannocchiale in A</mark>
Dal cannocchiale in A si misura il seguente dislivello:
$$
\begin{align}
\Delta H_{ijA} &= L_{iA} - L_{jA} = \\
&= l_{iA} - l_{jA} = \\
&= L_{iA} - \delta L_{iA} - L_{jA} + \delta L_{jA}
\end{align}
$$

<mark style="background: #FF5582A6;">Cannocchiale in B</mark>
Dal cannocchiale in B si misura il seguente dislivello:
$$
\begin{align}
\Delta H_{ijB} &= L_{iB} - L_{jB} = \\
&= l_{iB} - l_{jB} = \\
&= L_{iB} - \delta L_{iB} - L_{jB} + \delta L_{jB}
\end{align}
$$
I dislivelli $\Delta_{ijA}$ e $\Delta_{ijB}$ devono necessariamente essere uguali:
$$
\Delta H_{ijA} = \Delta H_{ijB} = \Delta H_{ij}
$$
Li sommo:
$$
\begin{align}
2 \Delta H_{ij} = L_{iA} - L_{jA} + L_{iB} - L_{jB} - \delta L_{iA} + \delta L_{jA} - \delta L_{iB} + \delta L_{jB}
\end{align}
$$
Ricordando le considerazioni fatte prima e quelle fatte nello studio della [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Livellazione dal mezzo\|#Livellazione dal mezzo]], posso fare delle semplificazioni:
$$
\begin{align}
2 \Delta H_{ij} = L_{iA} - L_{jA} + L_{iB} - L_{jB} - \cancel{\delta L_{i}} + \cancel{\delta L_{j}} - \cancel{\delta L_{i}} + \cancel{\delta L_{j}}
\end{align}
$$
ottenendo:
$$
\begin{align}
\Delta H_{ij} &= \frac{L_{iA} - L_{jA} + L_{iB} - L_{jB}}{2}= \\
&= \frac{\Delta H_{ijA} + \Delta H_{ijB}}{2}
\end{align}
$$
Ossia, la media tra le 2 misurazioni che faccio

Ci sono anche qui alcuni [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Errori - Livellazione reciproca\|errori]] che vengono commessi

##### Errori - Livellazione reciproca

###### Errore di srettifica

L'errore di srettifica è quello dovuto al fatto che il cannocchiale non vede perfettamente in orizzontale.


❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗






