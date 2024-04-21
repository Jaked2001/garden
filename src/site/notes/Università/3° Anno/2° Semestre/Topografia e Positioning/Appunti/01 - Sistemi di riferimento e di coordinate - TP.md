---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/01-sistemi-di-riferimento-e-di-coordinate-tp/"}
---


# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP\|01 - Sistemi di riferimento e di coordinate - TP]]

# Sistema di riferimento

Un sistema di riferimento può essere definito (almeno per ciò che è di nostro interesse) in 1, 2 o 3 dimensioni:

```ad-Definizione
title: Sistema di riferimento

Un **sistema di riferimento** è un insieme di scelte e regole che individuano univocamente la posizione di un punto in un prefissato ambito dimensionale.

Le *scelte*, sono quelle che bloccano **tutti e soli** i [[02. Cinematica dei corpi rigidi#Gradi di Libertà|gradi di libertà (g.d.l.)]] di un corpo rigido in quell'ambito dimensionale

```

Potremo parlare di:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento 2D\|#Sistema di riferimento 2D]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento 3D\|#Sistema di riferimento 3D]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento 1D\|#Sistema di riferimento 1D]]

| Ambito dimensionale | g.d.l. T | g.d.l. R   |
| ------------------- | -------- | ---------- |
| 1D                  | 1        | 0          |
| 2D                  | 2        | 1          |
| 3D                  | 3        | 3          |
|                     | Origine  | Assi/piani |




## Sistema di riferimento 2D

Immaginiamo di trovarci sul piano.
Un corpo rigido sul piano ha 3 gradi di libertà: 2 alla Traslazione e 1 alla Rotazione.

Vogliamo definire la posizione di un generico punto $P$.

Possiamo, per prima cosa, eliminare i gradi di libertà alla Traslazione, fissando un origine di un sistema di riferimento, $O$.

Successivamente, andremo a tracciare un asse $x$ il quale permette di bloccare il rimanente grado di libertà alla Rotazione.

Se si è fatta l'ipotesi di scegliere gli assi come ortonormali, basterà tracciare un unico asse. L'altro sarà infatti identicamente determinato, dovendo passare per $O$ e dovendo essere perpendicolare all'asse-$x$.

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-01 12.03.56.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-01%2012.03.56.excalidraw.png)


Per definire la posizione di un punto in uno spazio a 2 dimensioni, è **necessario** e **sufficiente** fissare:
- Un'origine
- Un asse passante per l'origine

## Sistema di riferimento 3D

Un Corpo Rigido in 3 Dimensioni ha 6 [[Università/2° anno/1° Semestre/Scienza delle costruzioni/Appunti/02. Cinematica dei corpi rigidi#Gradi di Libertà\|g.d.l.]]: 3T + 3R

- Fisso un'Origine O
- Fisso un asse $z$ (tolgo 2 gradi di libertà)
	- L'asse obbliga la giacitura del piano $x-y$
- Fisso un generico piano appartenente al **fascio proprio** di piani passante per l'asse $z$
Quest'ultimo piano identifica una retta nel piano $x-y$ che identifica l'asse $x$.

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-01 18.26.13.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-01%2018.26.13.excalidraw.png)



## Sistema di riferimento 1D

In uno spazio mono-dimensionale, un Corpo Rigido possiede 1 [[Università/2° anno/1° Semestre/Scienza delle costruzioni/Appunti/02. Cinematica dei corpi rigidi#Gradi di Libertà\|g.d.l.]]: 1T 

Per definire la posizione di un punto è sufficiente:
- Fissare un'origine O


# Sistema di coordinate

```ad-Definizione
title: Sistema di coordinate



```

## Sistema di coordinate 2D

In due dimensioni si possono individuare almeno 3 modi per rappresentare la posizione di un punto rispetto ad un certo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|#Sistema di riferimento]].

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-12 21.39.32.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-12%2021.39.32.excalidraw.png)


Il modo che si sceglie per rappresentare la posizione è una scelta **arbitraria** guidata solo dal voler scegliere il metodo che più si adatta al contesto (che renda più semplici i calcoli).

Devo però essere capace di passare da un sistema ad un altro.

### Trasformazioni di coordinate

Si vuole passare dalla rappresentazione del punto $P$ in coordinate cartesiane $\color{pink} (x,y)$ alla rappresentazione in coordinate polari $\color{green} (d,\alpha)$.

La trasformazione ${\color{green} (d,\alpha)} \to {\color{pink} (x,y)}$ è abbastanza semplice e diretta:
$$
\begin{cases}
x = d \sin(\alpha) \\
y = d \cos(\alpha)
\end{cases}
$$
Occorre però fare attenzione nella trasformazione inversa. Verrebbe infatti naturale scrivere
$$
\begin{cases}
d = \sqrt{x^{2}+y^{2}} \\
\alpha = \arctan\left( \dfrac{x}{y} \right)
\end{cases}
$$

```ad-error
title: Sbagliato
$$
\begin{cases}
d = \sqrt{x^{2}+y^{2}} \\
\alpha = \arctan\left( \dfrac{x}{y} \right)
\end{cases}
$$
La trasformazione scritta sopra è sbagliata in quanto la funzione $\arctan$ è in grado di rappresentare esclusivamente angoli compresi in $\left(  -\dfrac{\pi}{2}, \dfrac{\pi}{2} \right)$, mentre noi abbiamo bisogno di rappresentare $\alpha\in (0,2\pi)$.

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-12 21.50.56.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-12%2021.50.56.excalidraw.png)
%%[[01 - Sistemi di riferimento e di coordinate - TP 2024-03-12 21.50.56.excalidraw.md|🖋 Edit in Excalidraw]]%%
```

Per ovviare a ciò si introduce una nuova funzione, chiamata $\arctan2$ e si scrive $\alpha$ come
$$
\alpha = \arctan2\left( \frac{x}{2} \right)
$$

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-13 11.25.28.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-13%2011.25.28.excalidraw.png)


Rispetto allo schema sopra, possiamo dire:
$$
\begin{align}
&\color{green} \alpha' \\
&\color{green} \alpha = \alpha' +\pi \\
&\color{red} \alpha' \\
&\color{red} \alpha = \alpha' +\pi
\end{align}
$$
In base al quadrante in cui ci troviamo, l'$\arctan2$ può assumere i seguenti valori:

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-13 11.34.53.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-13%2011.34.53.excalidraw.png)


| CASI | $\boldsymbol\arctan2$ |
| ---- | --------------------- |
| 1    | $\arctan$             |
| 2    | $\arctan$             |
| 3    | $\arctan$             |
| 4    | $\arctan+\pi$         |
| 5    | $\arctan+\pi$         |
| 6    | $\arctan+\pi$         |
| 7    | $\arctan+2\pi$        |
| 8    | $\arctan+2\pi$        |
| 9    | $\arctan+2\pi$        |

Dove si noti che i primi tre casi sono tali che il codominio è comunque incluso in quello della funzione $\arctan$ che quindi non va variata affatto.





# Trasformazioni sistemi di riferimento


## Trasformazioni SR 1D


## Trasformazioni SR 2D

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-13 11.42.30.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-13%2011.42.30.excalidraw.png)


La rappresentazione del punto $P$ la faccio in coordinate cartesiane Ortogonali
- $\vec{P}$ e $\vec{P'}$ sono i VETTORI POSIZIONE del punto $P$
- $\vec{T}$ è la traslazione tra le due origini $O$ e $O'$

Si ha che:
$$
\vec{T}+\vec{P'} = \vec{P}
$$
e quindi
$$
\vec{P'} = \vec{P} - \vec{T}
$$

Le coordinate di $P$ in $S$ e $S'$ sono rispettivamente:
$$
\vec{P} =
\begin{bmatrix}
x \\
y
\end{bmatrix}_{S}
\qquad
\vec{P'} =
\begin{bmatrix}
x' \\
y'
\end{bmatrix}_{S'}
$$
Il vettore traslazione invece è
$$
\vec{T} =
\begin{bmatrix}
t_{x} \\ t_{y}
\end{bmatrix}_{S} 
=
\begin{bmatrix}
t'_{x} \\ t'_{y}
\end{bmatrix}_{S'}
$$

```ad-attention
title: Attenzione

Potrei pensare di scrivere la seguente relazione:
$$
\begin{bmatrix}
x' \\
y'
\end{bmatrix}_{S'}
=
\begin{bmatrix}
x \\
y
\end{bmatrix}_{S}
-
\begin{bmatrix}
t_{x} \\ t_{y}
\end{bmatrix}_{S} 
$$
In questo modo però non sto tenendo conto della rotazione tra i due Sistemi di Riferimento

```

Bisogna quindi introdurre una rotazione.

La relazione corretta è (traslazione + rotazione):
$$
\begin{bmatrix}
x' \\
y'
\end{bmatrix}_{S'}
=
R
\left(
\begin{bmatrix}
x \\
y
\end{bmatrix}_{S}
-
\begin{bmatrix}
t_{x} \\ t_{y}
\end{bmatrix}_{S}
\right)
$$
oppure, in modo del tutto equivalente (rotazione + traslazione):
$$
\begin{bmatrix}
x' \\ y'
\end{bmatrix}_{S'}
=
R
\begin{bmatrix}
x \\ y
\end{bmatrix}_{S}
-
\begin{bmatrix}
t'_{x} \\ t'_{y}
\end{bmatrix}_{S'}
$$



### Matrice di rotazione




❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ lezione del [[_Giornaliera/2024-03-06\|2024-03-06]]
❗❗❗❗❗❗❗❗❗❗❗❗❗






Immaginiamo di trovarci in una dimensione e di avere a disposizione 2 sistemi di riferimento. Saranno valide le seguenti relazioni:
$$
\begin{cases}
z' = z - t_{z} \\
z' = z + t_{z'}
\end{cases}
\Longrightarrow
z' = z-t
$$
Siamo interessati a passare dall'uno all'altro sistema di riferimento. In ogni caso devo chiaramente conoscere il parametro $t = z-z'$.

Al fine di trovare questo parametro è richiesta la conoscenza di almeno un punto e delle sue coordinate in **entrambi** i sistemi di riferimento.
Questo punto è detto [[punto doppio\|punto doppio]].

Noto il punto doppio posso ricavare il parametro $t$ che posso successivamente utilizzare per trasformare tutti gli altri punti.
















Nella realtà il passaggio da un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|#Sistema di riferimento]] a un altro non viene compiuto prima individuando i due SR e poi matematicamente studiando i punti. Questo perché i punti su cui operiamo sono già definiti, ma in SR che non sono noti e ai quali noi dobbiamo pervenire.

- Per capire come è messo $\mathcal{S}'$ rispetto a $\mathcal{S}$ (o viceversa) devo partire dai vettori posizione
- Devo ricavare tutti i parametri che regolano il modo in cui $\mathcal{S'}$ è messo rispetto ad $\mathcal{S}$
- Devono essere note le coordinate del punto da studiare nei due sistemi
- Devo determinare: $T_{x}, T_{y}, T_{z}, \omega, \varphi, k$

```ad-note
title: Osservazione 1

La trasformazione:
$$
\begin{bmatrix}
x' \\
y' \\
z'
\end{bmatrix}
=
R_{z}(k)
\left[
R_{y}(\varphi)
\left[
R_{x}(\omega)
\left[
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
-
\begin{bmatrix}
T_{x} \\
T_{y} \\
T_{z}
\end{bmatrix}
\right]
\right]
\right]
$$
Risulta essere una relazione **altamente non lineare**.
```

Un punto fornisce:
- 3 equazioni
- 6 incognite
Questo ovviamente non basta a risolvere il problema
Posso pensare di aggiungere un secondo punto, in modo da aggiungere 3 equazioni scalari

A questo punto avrei 6 equazioni in 6 incognite ma ancora non basterebbe a risolvere il problema

- [?] Qual è il problema da risolvere?🔼 

Infatti si tratta di un **problema singolare**.
Infatti, nello spazio, 2 punti definiscono una retta, ma non bastano a definire una rotazione attorno a questa retta. Non riesco pertanto a bloccare un SR rispetto all'altro perché il secondo può ancora ruotare attorno a questa retta di angoli qualunque.

Per individuare la rotazione avrò necessità di prendere un terzo punto non appartenente alla retta: mi serve una terna di punti non allineati. Trovo così:
- 9 equazioni
- 6 incognite

- [?] che vuol dire che il problema è singolare? Perché anche se ho 6eq e 6inc. non basta a risolvere il sistema? Capito concettualmente ma algebricamente non torna...

Di questi 3 punti prendo le informazioni necessarie a risolvere il problema.
Prendo i cosiddetti **PUNTI DOPPI** in quanto sono noti in entrambi i sistemi di riferimento.
$$
\begin{cases}
P(x_{p}, y_{p}, y_{p}) \\
P(x'_{p}, y'_{p}, y'_{p})
\end{cases}
\qquad
\begin{cases}
Q(x_{q}, y_{q}, y_{q}) \\
Q(x'_{q}, y'_{q}, y'_{q})
\end{cases}
\qquad
\begin{cases}
R(x_{q}, y_{q}, y_{q}) \\
R(x'_{q}, y'_{q}, y'_{q})
\end{cases}
$$
Dei 3 punti prendo in considerazione i primi 2, dei quali calcolo la differenza tra le coordinate.
$$
\begin{align}
SR(\mathcal{S}): \left\{ \Delta x_{PQ}, \Delta y_{PQ}, \Delta z_{PQ} \right\} \\
SR(\mathcal{S'}): \left\{ \Delta x'_{PQ}, \Delta y'_{PQ}, \Delta z'_{PQ} \right\}
\end{align}
$$

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-13 21.47.12.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-13%2021.47.12.excalidraw.png)


- Essendo interessato a conoscere le direzioni, posso anche lavorare con i **versori** invece che con i vettori.
- Le informazioni strettamente necessarie a calcolare i parametri sono effettivamente 6

Il calcolo della trasformazione tra SR è possibile solo conoscendo i punti doppi, punti le cui coordinate sono note nei due SR tra i quali si vuole calcolare la trasformazione.

Ogni punto doppio genera una equazione vettoriale di rototraslazione equivalente a tre equazioni scalari del tipo:
$$
(1)\begin{bmatrix}
x' \\
y' \\
z'
\end{bmatrix}
= R
\left[
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
-
\begin{bmatrix}
T_{x} \\
T_{y} \\
T_{z}
\end{bmatrix}
\right]
\quad \text{oppure} \quad 
(2)
\begin{bmatrix}
x' \\
y' \\
z'
\end{bmatrix}
= R
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
-
\begin{bmatrix}
T'_{x} \\
T'_{y} \\
T'_{z}
\end{bmatrix}
$$
Che, riscritte in forma vettoriale compatta diventano:
$$
(1) \quad \vec{P'} = \boldsymbol{R} \left[\vec{P} - \vec{T}\right] \qquad (2) \quad \vec{P'} = \boldsymbol{R}\vec{P} - \vec{T}
$$
dalle quali devono essere calcolate 6 incognite ($\boldsymbol{R}$ e $\vec{T}$)
1 punto doppio è insufficiente. Considero pertanto 2 punti doppi nella forma $(2)$.

Considero quindi 2 punti, $P_{1}$ e $P_{2}$ e le loro coordinate nei due sistemi di riferimento. Potremo scrivere:
$$
\begin{align}
(2.1) \quad \vec{P'_{1}} = R \vec{P_{1}} - \vec{T} \\
(2.2) \quad \vec{P'_{2}} = R \vec{P_{2}} - \vec{T}
\end{align}
\quad \Longrightarrow \quad
\left(\vec{P'_{2}}-\vec{P'_{1}} \right) = R \left(\vec{P_{2}}-\vec{P_{1}} \right) \qquad(2.3)
$$
dove le due differenze sono il vettore $\overrightarrow{P_{1}P_{2}}$. Si avrà che
$$
\left| \vec{P'_{2}}-\vec{P'_{1}} \right| = \left| \vec{P_{2}}-\vec{P_{1}} \right| = \Delta P_{12}
$$
Possiamo dire che il modulo di questo vettore da $P_{1}$ a $P_{2}$ è indipendente dal sistema di riferimento in cui lo si guarda.
Quindi
$$
\frac{\left(\vec{P'_{2}}-\vec{P'_{1}} \right)}{\Delta P_{12} } = R \frac{\left(\vec{P_{2}}-\vec{P_{1}} \right)}{\Delta P_{12} }
$$
Introduciamo ora i versori corrispondenti:
$$
\hat{e}_{12}' = R \hat{e}_{1} \qquad (2.4)
$$
Queste 3 equazioni scalari NON sono indipendenti poiché sussiste la condizione tra le componenti dei versori: 
$$
\left| \hat{e}_{12}' \right| = \left| \hat{e}_{12} \right| = 1
$$
Le equazioni trovate fino ad ora, $(2.1), (2.2), (2.3), (2.4)$ equivalgono solo a 2 equazioni scalari indipendenti in 3 incognite.
- Non sono sufficienti 2 punti doppi per calcolare $R$ e quindi per calcolare la rototraslazione ($R,\vec{T}$) tra $\mathcal{S}$ e $\mathcal{S'}$
- È necessario un terzo punto doppio non allineato con $P_{1}$ e $P_{2}$ altrimenti l'equazione vettoriale competente a $P_{3}$ risulterebbe identica alla $(2.4)$



❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗






## Materializzazione di un Sistema di Riferimento

- [?] Cosa significa materializzare un sistema di riferimento?

Al fine di Materializzare un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|#Sistema di riferimento]] occorre fornire opportune coordinate per opportuni punti
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Materializzazione di un Sistema di Riferimento 2D\|#Materializzazione di un Sistema di Riferimento 2D]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Materializzazione di un Sistema di Riferimento 1D\|#Materializzazione di un Sistema di Riferimento 1D]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Materializzazione di un Sistema di Riferimento 3D\|#Materializzazione di un Sistema di Riferimento 3D]]

### Materializzazione di un Sistema di Riferimento 2D

Cominciamo con il bloccare un'origine $O$:
$$
O(0,0)
$$
Per l'origine scelgo convenzionalmente le coordinate $(0,0)$. Questa è una scelta arbitraria, dettata dalla convenienza del caso specifico in esame.

Notiamo che per avere un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento 2D\|#Sistema di riferimento 2D]], abbiamo bisogno anche di un asse in modo da bloccare la rotazione del sistema di riferimento. Grazie all'origine infatti abbiamo bloccato solo le due traslazioni.

Posso farlo andando a definire un secondo punto, $P$, con l'unica condizione che sia diverso da $O$. Di questo punto fisso una delle due coordinate, ad esempio $y$, e la impongo $y=0$. Lascio l'altra coordinata libera:
$$
P(x_{P},0) \ne O
$$
$x_{P}$ può assumere qualsiasi valore purché sia diversa dalla $x_{O}$ (che in questo caso è 0).

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-14 21.35.40.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-14%2021.35.40.excalidraw.png)


Nel caso 2D occorrono:
- Opportuni punti: 2 punti distinti
- Opportune coordinate:
	- Per uno dei due punti entrambe le coordinate
	- Per l'altro solo una delle due coordinate
In questo modo vengono bloccati **tutti e soli** i gradi di libertà che mi interessa bloccare.



### Materializzazione di un Sistema di Riferimento 1D


Nel caso monodimensionale è sufficiente definire l'origine con una coordinata:
$$
O(0)
$$
- 1 punto
- 1 coordinata bloccata

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-14 21.40.34.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-14%2021.40.34.excalidraw.png)




### Materializzazione di un Sistema di Riferimento 3D


Nel caso tridimensionale, per la [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Materializzazione di un Sistema di Riferimento\|#Materializzazione di un Sistema di Riferimento]], occorre bloccare 6 gradi di libertà: 3T+3R.

Comincio fissando un'origine:
$$
O(0,0,0)
$$
Blocco così i 3 g.d.l. alla traslazione.

❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗

# Sistemi di coordinate fondamentali

[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di coordinate\|Sistema di coordinate]]

Possiamo definire diversi [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di coordinate\|sistemi di coordinate]]. In particolare vedremo:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Coordinate ellissoidiche\|#Coordinate ellissoidiche]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]]


## Coordinate ellissoidiche


Si può parlare di coordinate ellissoidiche solo dopo aver introdotto un ellissoide di riferimento. Faremo uso del [[WGS84\|WGS84]]

![02 - Campo gravitazionale - TP 2024-03-28 19.31.58.excalidraw.png](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-28%2019.31.58.excalidraw.png)


Nel diagramma è raffigurato un ellissoide di rotazione (ad esempio il [[WGS84\|WGS84]]) rispetto ai 3 assi cartesiani $x,y,z$. In particolare è raffigurato solo un ottavo dell'ellissoide, quello corrispondente ai semiassi positivi.

Si prende un punto $P$ qualunque sulla superficie terrestre e si vuole definire la sua posizione rispetto all'origine con un qualche sistema di coordinate.

Tracciamo quindi la <mark style="background: #FF5582A6;">normale</mark> all'ellissoide passante per il punto $P$, $\vec{n}$. Questa intersecherà l'ellissoide in un punto $P_{c}$. Tracciamo corrispondentemente l'arco dal polo all'equatore che passa per questo punto (<mark style="background: #ADCCFFA6;">tratto blu</mark>). Si traccia quindi un asse di riferimento, l'asse $r$, come in figura.

Andiamo ad individuare così 2 angoli:
- $\lambda:$ L'angolo tra il piano $xz$ e il piano $xr$ - lo chiameremo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#longitudine\|#longitudine]]
- $\varphi:$ L'angolo tra la normale $\vec{n}$ e l'asse $r$ - lo chiameremo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#latitudine\|#latitudine]]

Ogni punto sulla superficie terrestre sarà quindi individuato da coordinate:
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Quota\|#Quota]] $h$
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Latitudine\|#Latitudine]] $\varphi$
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Longitudine\|#Longitudine]] $\lambda$

```ad-example
title: Esempio
Vediamo alcuni punti e le rispettive coordinate.

- Punto al polo nord: LAT $\varphi= 90\degree$
- Punto sul piano $xz$: LON $\lambda = 0\degree$
- Punto sul piano $yz$: LON $\lambda = 90\degree$
```


### Longitudine

❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗

### Latitudine

❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗

- $\lambda:$ Angolo diedro


❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ ORIENTAZIONE dell'ellissoide
❗❗❗❗❗❗❗❗❗❗❗❗❗





## Coordinate Cartesiane locali (L)

Sono coordinate definite localmente. È necessario pertanto introdurre un origine locale

Considero un solo ottante, come quando abbiamo definito le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Coordinate ellissoidiche\|#Coordinate ellissoidiche]].


![02 - Campo gravitazionale - TP 2024-04-03 19.20.58.excalidraw.png](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-04-03%2019.20.58.excalidraw.png)


Si osservi alla figura sopra. 
Il punto $P_{l}$, intersezione dell'ellissoide con la normale $\vec{n}$ è considerato come **origine locale**

$\vec{n}$ è il versore perpendicolare e uscente dal piano tangente in $P_{l}$. Lo chiamiamo "piano ($\Pi$) tg nel punto $P_{l}$".

Essendo $P_{l}$ la nuova origine, l'asse individuato da $\vec{n}$ è il nuovo asse $z$

Abbiamo così definito un nuovo sistema di coordinate, detto *sistema di coordinate cartesiane locali*.

In alto a destra nella figura è raffigurata la proiezione dell'ellissoide nel piano $zr$.

L'asse $x$ è tangente al ramo dell'ellisse, l'asse $y$ invece è entrante nel foglio.

Considero un generico punto $P$ sull'asse $z$ (ossia $\vec{n}$). La distanza da $P$ a $P_{l}$ è la [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Quota ellissoidica\|#Quota ellissoidica]] $h$ ed in questo caso coincide con la coordinata $z$ di $P$

Considerando un altro punto $Q$ che non si trova su $z$, la coordinata $z_{Q}$ e l'altezza ellissoidica $h_{Q}$ non coincideranno più.

```ad-Definizione
title: Sistema di coordinate cartesiane locali (L)

Un **sistema di coordinate cartesiane locali** (L) è un sistema che ha origine in $P_{l}$, un punto dell'ellissoide. È caratterizzato da 3 assi $(x,y,z)$. Di conseguenza $P_{l}(0,0,0)$.

```

Questi sistemi di coordinate sono semplici da definire ma complicati dal punto di vista applicativo. 
Vengono in nostro soccorso le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]]

## Coordinate cartesiane di livello locale (LL)


Considero, a partire dal punto $P$ il versore che indica la forza di gravità ($\vec{\nu}$).

![01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.16.15.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-04-04%2010.16.15.excalidraw.png)


L'asse $z$ è individuato dal versore $\vec{\nu}$. Pertanto:
$$
\begin{align}
z_{u} &\parallel \vec{\nu} \\
x_{u}, y_{u} &\parallel \vec{\nu}
\end{align}
$$
```ad-attention
Nel caso di [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]], il piano $\Pi$ era quello **tangente** all'ellissoide. Ossia era **perpendicolare** alla normale all'ellissoide ($\vec{n}$).

In questo caso, il piano $\Pi$ è **perpendicolare** alla **gravità** ($\vec{\nu}$).


![01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.39.13.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-04-04%2010.39.13.excalidraw.png)
%%[[01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.39.13.excalidraw.md|🖋 Edit in Excalidraw]]%%

$\vec{n}$ e $\vec{\nu}$ sono deviate di un angolo $\varepsilon$.

Localmente $\varepsilon$ è molto piccolo e quindi **trascurabile** ma MAI NULLO.

Facciamo l'ipotesi che $\vec{n} \equiv \vec{\nu}$.
```

$x_{u}, y_{u}$ giacciono sul piano orizzontale locale, quello identificato con la ???

Questo modello è più semplice perché l'asse $x_{u}$ è individuato dalla direzione della gravità.

Come si passa da questo sistema alle [[#Coordinate Cartesiane locali (L)]]?











❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ Lezione da recuperare, ero assente!!!
❗❗❗❗❗❗❗❗❗❗❗❗❗






