---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/04-equazione-di-osservazione-tp/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP\|04 - Equazione di osservazione - TP]]

# Equazione di osservazione

L'equazione di osservazione è lo strumento analitico che lega tra di loro ciò che osservo (osservazione = misure) con ciò che mi interessa determinare. 

Tendenzialmente quando si eseguono delle misurazioni non si è interessati alle misurazioni stesse, ma quest'ultime si utilizzano per calcolare le grandezze di cui effettivamente si ha bisogno.


```ad-Definizione
title: Equazione di osservazione

L'**equazione di osservazione** è una funzione che mette in relazione la quantità osservabile (quella che viene misurata) con le incognite che si è interessati a calcolare. È generalmente una relazione non lineare della forma:
$
y = f(x,a,c)
$
dove:
- $y:$ Osservabile
- $x:$ Vettore dei **parametri incogniti**
- $a:$ Vettore dei **parametri di disturbo**
- $c:$ Vettore dei **parametri noti**

```

## Equazione di osservazione alla distanza

![04 - Equazione di osservazione - TP 2024-05-22 16.12.14.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-22%2016.12.14.excalidraw.png)


Si vuole determinare la distanza 2D del punto $j$ dal punto $i$. Non è una grandezza che siamo capaci di misurare direttamente ma dobbiamo ottenerla proiettando la distanza 3D tra $i$ e $j$.
- $i:$ Centro dello strumento
- $j:$ Centro del prisma retroriflettore (o un punto naturale)

Introduciamo un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|sistema di riferimento]] e un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di coordinate\|sistema di coordinate]].

![04 - Equazione di osservazione - TP 2024-05-22 16.14.54.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-22%2016.14.54.excalidraw.png)


Scriviamo ora l'[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#Equazione di osservazione\|#Equazione di osservazione]] che lega la distanza $d_{ij}$ (che è quella che osserviamo) alle coordinate dei punti $i$ e $j$ rispetto al SR con origine in $O_{L}$:

```ad-Teo
title: Equazione di osservazione alla distanza 3D

$
d_{ij} = \sqrt{(x_{jL}-x_{iL})^{2} + (y_{jL}-y_{iL})^{2} + (z_{jL}-z_{iL})^{2}}
$

```

(abbiamo semplicemente applicato Pitagora)

```ad-note
title: Osservazione

La distanza 3D **non** dipende dal campo gravitazionale $\vec{g}$.

La distanza 2D dipende dal SR e dal campo gravitazionale

```

La distanza 2D dipende da $\vec{g}$ in quanto questa è la distanza misurata sul piano-$x_{L}y_{L}$ il quale è ortogonale all'asse $z_{L}$ il quale è parallelo con la direzione della gravità nel punto $O_{L}$.

È importante osservare che, spostando il punto $O_{L}$ la distanza 3D tra $i$ e $j$ non cambia, ma cambia la direzione della gravità. Cambia anche la giacitura del piano-$x_{L}y_{L}$ e quindi la proiezione di $i$ e $j$ su di essa 

Si ottiene così l'[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#Equazione di osservazione\|#Equazione di osservazione]] della distanza 2D $d_{ij}\,\rm 2D$
$$
{\rm 2D} \, d_{ij} = \sqrt{(x_{jL}-x_{iL})^{2} + (y_{jL}-y_{iL})^{2}}
$$
ed è detta **distanza orizzontale**.


## Equazione di osservazione all'angolo zenitale

L'[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Angolo zenitale\|angolo zenitale]] **dipende** dalla direzione della gravità!

Si parla di *angolo* e non di *direzione* perché l'angolo zenitale è misurato rispetto a un riferimento fisico esterno: direzione della gravità nel punto $i$ (non è definito quindi internamente allo strumento).

![04 - Equazione di osservazione - TP 2024-05-22 17.05.03.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-22%2017.05.03.excalidraw.png)


Nella configurazione sopra, siamo interessati a trovare gli angoli zenitali $\color{blue} Z_{ij}$ e $\color{red} Z_{ji}$.

Si noti che, in generale, gli angoli zenitali $\color{blue} Z_{ij}$ e $\color{red} Z_{ji}$ sono diversi e completamente **indipendenti** l'una dall'altra essendo fisicamente dipendente esclusivamente dal campo della gravità.

Per semplicità, e supponendo di non fare mai misure di punti troppo lontani tra loro, facciamo **l'ipotesi di campo di gravità parallelo**.

Sotto questa ipotesi (e introducendo un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|SR]] e un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di coordinate\|SC]]) lo schema del problema diventa il seguente:

![04 - Equazione di osservazione - TP 2024-05-22 17.16.32.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-22%2017.16.32.excalidraw.png)


Notiamo che se $i$ e $j$ avessero la stessa quota si avrebbe 
$$Z_{ij}=Z_{ji} = \frac{\pi}{2}$$
Sotto l'ipotesi di campo parallelo, vale la relazione:
$$
Z_{ij} + Z_{ji} = \pi
$$

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

- [?] Non ho capito qual è l'equazione di osservazione per l'angolo zenitale





## Equazione di osservazione alla direzione azimutale

L'[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#\|##azimut]] è una grandezza che dipende dal campo di gravità.

Facciamo l'ipotesi di campo $\vec{g}$ parallelo.

![04 - Equazione di osservazione - TP 2024-05-22 18.18.00.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-22%2018.18.00.excalidraw.png)


- $\vec{\nu_{i}}:$ Asse verticale

Nel diagramma sopra si hanno 3 piani:
- $\Pi_{j}:$ Piano generato da $\vec{\nu_{i}}$ che contiene il punto $j$
- ${\color{red} \Pi_{O}}:$ Piano individuato dalla direzione dello **zero** del cerchio verticale del [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08.1 - Teodolite - TP\|Teodolite]]
- ${\color{blue} \Pi_{OR_{i}}}:$ Il piano perpendicolare ai due piani precedenti

La grandezza [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08 - Strumenti di misura - TP#Direzione azimutale\|direzione azimutale]] è riferita allo zero del cerchio, che p un riferimento interno allo strumento. Nell'operazione di [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/08.1 - Teodolite - TP#Messa in stazione\|messa in stazione]], non sappiamo dove vada a finire lo zero del cerchio. La posizione dello zero non ha nessuna attinenza con l'ambiente circostante.

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ considerazioni sul piano orizzontale
❗❗❗❗❗❗❗❗❗❗❗❗

Considerato il campo di gravità parallelo, conviene considerare il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#\|##Sistema di riferimento cartesiano]]. A questo punto l'asse z risulta parallelo alla verticale $\vec{\nu}$.

Si lavora quindi nel piano-$x_{L}y_{L}$ proiettando i punti $i$ e $j$ in questo piano.

![04 - Equazione di osservazione - TP 2024-05-25 17.48.24.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-25%2017.48.24.excalidraw.png)


L'obiettivo è legare $\alpha_{ij}$ a $x_{L}$ e $y_{L}$. Ossia, siamo interessati a determinare la posizione di $i$ e $j$ ($i_{xy}$ e $j_{xy}$) ma possiamo misurare solo $\alpha_{ij}$.

Bisogna ragionare in termini trigonometrici:
- Si considera il triangolo rettangolo tratteggiato
- Si introduce un ulteriore angolo: $\Delta_{i}$ - l'angolo individuato dalla direzione dello zero del cerchio rispetto alla parallela all'asse delle $y$
	- N.B.: questo angolo non viene mai misurato

A questo punto possiamo affermare che:
$$
\tan(\Delta_{i}+\alpha_{ij}) = \dfrac{x_{Lj}-x_{Li}}{y_{Lj}-y_{Li}}
$$
Da questa relazione si può ricavare l'[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#Equazione di osservazione\|#Equazione di osservazione]]:
$$
\Delta_{i} + \alpha_{ij} = \arctan2\left( \dfrac{x_{Lj}-x_{Li}}{y_{Lj}-y_{Li}} \right)
$$
In definitiva

- [?] Perché calcoliamo l'angolo in senso orario e non in senso antiorario dovendo calcolare quindi l'$\arctan2$ di x/y invece che con la formula convenzionale y/x?


```ad-Teo
title: Equazione di osservazione alla direzione azimutale
Nell'ipotesi di campo parallelo, l'equazione di osservazione alla direzione azimutale è
$
\alpha_{ij} = \arctan2\left( \dfrac{x_{Lj}-x_{Li}}{y_{Lj}-y_{Li}} \right) - \Delta_{i}
$

```


| **Parametri incogniti**   | $x_{i}, x_{j}, y_{i}, y_{j}$ |
| ------------------------- | ---------------------------- |
| **Parametri di disturbo** | $\Delta_i$                   |
| **Parametri noti**        |                              |



❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

# Equazione di osservazione in forma generale

## Equazione di osservazione in forma vettoriale


Si introducono:
- 2 vettori che rappresentano le posizioni di due punti qualsiasi rispetto ad un certo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|sistema di riferimento]]
- Vettore differenza di posizione dei due vettori

![04 - Equazione di osservazione - TP 2024-05-26 11.16.47.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-26%2011.16.47.excalidraw.png)


Si hanno così:
- $\color{black} \vec{r_{i}}:$ Vettore posizione del punto $i$
- ${\color{purple} \vec{r_{j}}} :$ Vettore posizione del punto $j$
- ${\color{green} \vec{r_{ij}}} = {\color{purple} \vec{r_{j}}} - {\color{black} \vec{r_{i}}}:$ Vettore differenza tra i due vettori posizione


Si possono ora scrivere le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#Equazione di osservazione\|equazioni di osservazione]]:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#Equazione di osservazione alla distanza - vettoriale\|#Equazione di osservazione alla distanza - vettoriale]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#Equazione di osservazione all'angolo zenitale - vettoriale\|#Equazione di osservazione all'angolo zenitale - vettoriale]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/04 - Equazione di osservazione - TP#Equazione di osservazione alla direzione azimutale - vettoriale\|#Equazione di osservazione alla direzione azimutale - vettoriale]]

### Equazione di osservazione alla distanza - vettoriale

Si può pertanto definire la distanza tra $i$ e $j$ in termini vettoriali:
$$
d_{ij} = \sqrt{\vec{r_{ij}} \cdot \vec{r_{ij}} }
$$

### Equazione di osservazione all'angolo zenitale - vettoriale

![04 - Equazione di osservazione - TP 2024-05-26 11.46.47.excalidraw.png](/img/user/Excalidraw/04%20-%20Equazione%20di%20osservazione%20-%20TP%202024-05-26%2011.46.47.excalidraw.png)


Si vuole trovare l'angolo $\color{green} Z_{ij}$. Si può usare il prodotto scalare tra il versore verticale $\vec{\nu}_{i}$ e il vettore $\vec{r}_{ij}$. Infatti:
$$
\vec{\nu}_{i} \cdot \frac{\vec{r_{ij}}}{d_{ij}} = \left| \vec{\nu_{i}} \right| \left| \frac{\vec{r_{ij}}}{d_{ij}} \right| \cos \left(Z_{ij}\right)
$$
Da cui si ricava

```ad-Teo
title: Eq. di Oss. all'angolo zenitale - vettoriale

$
Z_{ij} = \arccos\left(  \frac{\vec{\nu}_{i}\cdot \vec{r_{ij}} }{d_{ij}}  \right)
$

```


### Equazione di osservazione alla direzione azimutale - vettoriale

$$
\alpha_{ij} = 
$$
