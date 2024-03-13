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

## Trasformazioni SR 2D

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-13 11.42.30.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-13%2011.42.30.excalidraw.png)


La rappresentazione del punto $P$ la faccio in coordinate cartesiane Ortogonali
$\vec{P}$ e $\vec{P'}$ sono i VETTORI POSIZIONE del punto $P$


❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ lezione del [[_Giornaliera/2024-03-06\|2024-03-06]]
❗❗❗❗❗❗❗❗❗❗❗❗❗






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
- Essendo interessato a conoscere le direzioni, posso anche lavorare con i **versori** invece che con i vettori.
- Le informazioni strettamente necessarie a calcolare i parametri sono effettivamente 6

Il calcolo della trasformazione tra SR è possibile solo conoscendo i punti doppi, punti le cui coordinate sono note nei due SR tra i quali si vuole calcolare la trasformazione.

Ogni punto doppio genera una equazione vettoriale di rototraslazione equivalente a tre equazioni scalari del tipo:
$$
\begin{bmatrix}
x' \\
y' \\
z'
\end{bmatrix}
= R
\left[
\begin{bmatrix}

\end{bmatrix}
\right]
$$









