---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/02-campo-gravitazionale-tp/"}
---


# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP\|02 - Campo gravitazionale - TP]]



## Geoide

```ad-Definizione
title: Geoide
Il **geoide** è una particolare superficie equipotenziale della gravità terrestre
```

La conoscenza del geoide ci permette di conoscere, ad esempio, come viaggiano le correnti oceaniche.

## Campo di gravità terrestre

- [?] È giusto dire che il campo gravitazionale è $\vec{f}$ e quindi dovuto solo alla forza di gravità, mentre il campo di gravità terrestre è quello che tenga conto anche dell'azione della forza centrifuga dovuta alla rotazione della Terra?

```ad-Definizione
title: Campo di gravità terrestre
Il **Campo di gravità terrestre** è la *somma* del [[#Campo di attrazione Newtoniana]] e del [[#Campo della forza centrifuga]]
$$
\vec{g} = \vec{f} + \vec{c}
$$
```

#### Campo di attrazione Newtoniana

Sappiamo, dalla fisica, che la **forza di attrazione Newtoniana** è
$$
\vec{f} = -G \frac{Mm}{r^{3}} \vec{r}
$$
D'ora in poi, per semplicità, si supporrà $m=1$. Guardo quindi al campo gravitazionale della Terra di massa $M$ che interagisce con una massa unitaria.
$$
\vec{f} = -G \frac{M}{r^{3}}\vec{r}
$$
Consideriamo la situazione sottostante:

![02 - Campo gravitazionale - TP 2024-03-21 17.32.51.excalidraw.png|450](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.32.51.excalidraw.png)


Prendo un punto $P$ fermo rispetto alla superficie terrestre. Questo punto subisce l'attrazione di ogni elementino della Terra, $dM$ situato nel punto $Q$.
Pertanto, la forza di attrazione gravitazionale sarà data da:
$$
\vec{f} = -G \int_{\text{vol. Terra}} \dfrac{dM}{r_{PQ}}\vec{r}_{PQ}
$$
##### Potenziale Newtoniano

```ad-Definizione
title: Potenziale newtoniano

Posso definire la forza attrattiva per mezzo di una funzione, detta [[Potenziale Newtoniano]] e dire che
$$
\vec{f} = \vec{\rm grad} V
$$

```

Si dimostra pertanto

```ad-Teo
title: Potenziale Newtoniano

$$
V = G \int_{\text{Vol. Terra}} \frac{dM}{r_{PQ}}
$$

```



#### Campo della forza centrifuga

Se introduco la rotazione della Terra a velocità angolare $\vec{\omega}$ attorno a un certo asse di rotazione, devo considerare anche la forza centrifuga generata come effetto di tale rotazione:
$$
\vec{c} = \omega^{2}\vec{l_{P}}
$$
dove:
- $\omega:$ velocità angolare di rotazione della Terra
- $\vec{l_{P}}:$ Vettore distanza del punto P dall'asse di rotazione terrestre

```ad-note
title: Osservazione
La forza centrifuga, dipendendo da $|\vec{l_{P}}|$, è massima all'Equatore e nulla ai Poli.
Quindi la gravità varia lungo la superficie terrestre
- per direzione
- per modulo

```

![02 - Campo gravitazionale - TP 2024-03-21 17.32.51.excalidraw.png|450](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.32.51.excalidraw.png)




##### Potenziale centrifugo

Anche il campo di forza centrifuga ammette un potenziale, detto **potenziale centrifugo**, tale che
$$
\vec{c} = \vec{\rm grad}C
$$

```ad-Teo
title: Potenziale Centrifugo

Si può dimostrare che il potenziale centrifugo è pari a
$$
C = \frac{1}{2} \omega^{2} l_{P}^{2}
$$

```



### Potenziale del campo di gravità terrestre

![02 - Campo gravitazionale - TP 2024-03-21 17.55.14.excalidraw.png|550](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.55.14.excalidraw.png)


Posso esplicitare $r_{PQ}$ e $l_{P}$ introducendo un sistema di coordinate centrato nel baricentro della Terra.
A questo punto avremmo
$$
\begin{align}
r_{PQ} &= \sqrt{(x_{P}-x_{Q})^{2} + (y_{P}-y_{Q})^{2} + (z_{P}-z_{Q})^{2}} \\
l_{P} &= \sqrt{x_{P}^{2} + y_{P}^{2}}
\end{align}
$$
Essendo
$$
\vec{g} = \vec{f} + \vec{c}
$$
posso definire una funzione potenziale $W$ anche per il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Campo di gravità terrestre\|#Campo di gravità terrestre]] scrivendo quindi
$$
\vec{g} = {\rm \vec{grad}}V + {\rm \vec{grad}}C = {\rm \vec{grad}}W
$$
e quindi:
$$
W = V + C = G \int_{\text{Vol. Terra}} \frac{dM}{r_{PQ}}  \ + \frac{1}{2}\omega^{2}l_{P}^{2}
$$
Posso inoltre, introducendo la densità terrestre, riscrivere $dM$ in coordinate cartesiane:
$$
dM = \rho_Q(x,y,z) dxdydz
$$
e quindi, il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Potenziale Newtoniano\|#Potenziale Newtoniano]] diventa:
$$
V = G \int_{z}\int_{y}\int_{x} \frac{\rho_{Q}(x,y,z)}{r_{PQ}} \underbrace{dxdydz}_{= dV}
$$

```ad-note
title: Osservazione
Si noti che
- $\overline{\rho}_{\text{Superficie Terra}} \approx 2.67 \,\rm \frac{g}{cm^{3}}$
- $\overline{\rho}_{\text{Vol. Terra}} \approx 5.5 \,\rm \frac{g}{cm^{3}}$

Conosco solo i valori medi di densità. So molto poco sui valori puntuali. Vedremo che questo problema può essere aggirato facendo ricorso all'[[#Equazione di Laplace]]
```

#### Equazione di Laplace

```ad-Teo
title: Equazione di Laplace
L'**eqiazione di Laplace** afferma che
$$
\Delta^{2}V = 0
$$
al di fuori della Terra
```


### Approssimazione del potenziale V

La funzione potenziale del [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Campo di gravità terrestre\|#Campo di gravità terrestre]] è una funzione armonica al di fuori della Terra. Questo ci permette di riscriverla come serie di funzioni armoniche:
$$
V = \sum\limits_{n=0}^{+\infty}\sum\limits_{m=-n}^{+n} A_{nm} \frac{Y_{nm}}{r_{P}^{n+1}}
$$
dove:
- $Y_{nm}:$ Funzioni sferiche
- $A_{nm}:$ Coefficienti delle funzioni sferiche
- $n:$ Grado
- $m:$ Ordine

Le conoscenze odierne ci permettono di conoscere i valori di poco meno di 5 milioni di termini di questa serie. 
Sfortunatamente però la serie converge molto lentamente, quindi i termini più piccoli comunque non sono trascurabili e per aumentare la precisione del risultato occorre usare moltissimi termini della serie.
I più importanti però sono i primi temrini e in particolare, guardando ai *coefficienti delle funzioni sferiche*:
- $A_{00}:$ Il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Termine di campo centrale\|#Termine di campo centrale]]
- $A_{20}:$


#### Termine di campo centrale

Per $n=0$ $m$ è per forza $m=0$ e
$$
\begin{align}
Y_{00} &= 1 \\
A_{00} &= GM
\end{align}
$$
e quindi
$$
V_{00} = \frac{GM}{r}
$$
dove:
- $M:$ Massa della Terra
Ossia il potenziale di un punto esterno alla terra se concentrassi tutta la massa della Terra in un unico punto nel baricentro.


#### Termini del primo grado

I termini del primo grado sono quelli con $n=1$. Per questi valori, $m$ assume valori $m=-1,0,1$.
$$
\begin{align}
A_{1,-1} &= k \int_{z}\int_{y}\int_{x} x \rho_{Q}(x,y,z dxdydx) \\
A_{1,0} &= k \int_{z}\int_{y}\int_{x} y \rho_{Q}(x,y,z dxdydx) \\
A_{1, 1} &= k \int_{z}\int_{y}\int_{x} z \rho_{Q}(x,y,z dxdydx)
\end{align}
$$
Che risultano essere, rispettivamente,
- $A_{1,-1}:$ Coordinata $x$ del baricentro
- $A_{1,0}:$ Coordinata $y$ del baricentro
- $A_{1,1}:$ Coordinata $z$ del baricentro
Essendo il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|Sistema di Riferimento]] in questo caso centrato proprio nel baricentro, le coordinate del baricentro verrebbero $(0,0,0)$.

#### Termini del secondo grado

Al secondo grado ottengo termini nella forma di momenti e prodotti di inerzia.
Per $n=2$, l'ordine assume valori $m = -2,-1,0,1,2$.

Noi siamo interessati solo al termine $A_{2,0}$ che è quello prevalente. Questo termine tiene conto dell'effetto dello schiacciamento ai poli.

```ad-info
Si ricordano gli ordini di grandezza che riguardano le dimensioni della Terra. Se guardiamo alla Terra come un ellissoide infatti, per i semiassi $a$ e $b$ valgono le seguenti relazioni:
$$
\begin{align}
a &\simeq 6370 \,\rm km \\
a-b &\simeq 21 \,\rm km
\end{align}
$$

```

Paragoniamo a queste dimensioni gli ordini di grandezza dei termini della serie:

| ODG       | $\boldsymbol{ODG(V_{nm})}$ |
| --------- | -------------------------- |
| $n=0$     | 1                          |
| $n=1$     | 0                          |
| $n=2$     | $10^{-3}$                  |
| $n \ge 2$ | $10^{-6}\div 10^{-7}$      |

Se considero soltanto i termini con maggior peso, ossia $A_{00}$ e $A_{20}$ si ottiene che la superficie equipotenziale è un **ellissoide di rotazione**
$$
\frac{x^{2}+y^{2}}{a^{2}} + \frac{z^{2}}{b_{2}} = 1
$$
con:
- $a:$ Semi-asse maggiore (equatoriale)
- $b:$ Semi-asse minore (polare)
Seppure di pochi chilometri, vale la relazione $a>b$ essendo
$$
\begin{align}
a \simeq 6378 \,\rm km \\
b \simeq 6357 \,\rm km
\end{align}
$$
```ad-note
title: Osservazione
Il geoide si discosta dall'ellissoide di valori compresi entro i $100 \,\rm m$.

```

I parametri $(a,b)$ dipendono da vari fattori:
$$
(a,b) = f(W_{0}, A_{00}, A_{20}, \omega)
$$
Il geoide è di fatto la superficie del mare (là dove c'è il mare).

#### Potenziale del campo normale

```ad-Definizione
title: Potenziale del campo normale ($U$)

Il [[#Potenziale del campo di gravità terrestre]] rappresentato esclusivamente dall'ellissoide di rotazione e quindi con i termini $A_{00}$ e $A_{20}$ della serie costituisce il **potenziale del campo normale**
$$
\tilde{W} = U = \frac{GM}{r_{P}} + A_{20} \frac{Y_{20}}{r_{P}^{3}} + \frac{1}{2}\omega^{2}l_{P}^{2}
$$

```

![02 - Campo gravitazionale - TP 2024-03-21 17.55.14.excalidraw.png|550](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.55.14.excalidraw.png)


```ad-info
title: Curiosità
Allo stato attuale, il campo ha un'accuratezza, con tutti i coefficienti noti, non migliore di qualche $\rm cm$.

```

Ad oggi la descrizione del geoide è fatta in termini **perturbativi**: si prende la misura di quanto si discosta dall'ellissoide.

Quale ellissoide?


## Descrizione pratica del geoide

Allo stato attuale, la descrizione del geoide è fatta in termini **perturbativi**. Si rappresenta il geoide sotto forma di quanto questo si discosta dall'ellissoide.

L'ellissoide usato oggi maggiormente e preso come riferimento è il [[WGS84\|WGS84]]. Quando parlo di $(a,b)$ o di $(a,e^{2})$ sto implicitamente facendo riferimento all'ellissoide [[WGS84\|WGS84]].

Nei nostri telefoni è in uso una descrizione semplificata del geoide: il [[EGM2008\|EGM2008]].

```ad-example
title: Esempio

Le correnti del mare dipendono dalla superficie oceanica stazionaria ($\ne$ dal geoide). Ad esempio la [[Corrente del Golfo]] eiste perché c'è un piccolo dislivello ($\sim 2 \,\rm m$) tra l'America e l'Europa.
```


## Quota

Definito il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Geoide\|#Geoide]] si può iniziare a parlare di quota. In particolare vedremo:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Quota ellissoidica\|#Quota ellissoidica]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Quota Ortometrica\|#Quota Ortometrica]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Ondulazione del geoide\|#Ondulazione del geoide]]
Le grandezze elencate sopra fanno tutte riferimento al seguente diagramma:

![02 - Campo gravitazionale - TP 2024-03-27 14.37.08.excalidraw.png](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-27%2014.37.08.excalidraw.png)



### Quota ellissoidica

```ad-Definizione
title: Quota/Altezza ellissoidica ($h$)

La **quota ellissoidica** è la distanza del punto $P$ dall'ellissoide. 

```

La si ottiene proiettando il punto $P$ sull'ellissoide, ottenendo così $P_{e}$. È quindi uguale alla lunghezza del segmento $\overline{PP_{e}}$


### Quota Ortometrica

```ad-Definizione
title: Quota/Altezza ortometrica ($H$)

La **quota ortometrica** è la distanza del punto $P$ dal geoide, calcolata seguendo la linea di forza del campo di gravità (che arriverà poi perpendicolare al geoide)

```

Questa è di fatto quella che noi comunemente chiamiamo quota sul livello del mare.

### Ondulazione del geoide

```ad-Definizione
title: Ondulazione del geoide ($N$)

L'**ondulazione del geoide** è la distanza di ogni punto del geoide dall'ellissoide ($\overset{\frown}{P_{g}P_{eg}}$)

```


## Discostamento tra geoide ed ellissoide

Abbiamo detto che l'ellissoide di rotazione che prendiamo in considerazione ha i seguenti semi-assi:
$$
\begin{align}
a = 6371 \,\rm km \\
b = 6357 \,\rm km
\end{align}
$$
L'ellissoide e il geoide si discostano al massimo di $\pm 100\,\rm m$.

È chiaro che questa distanza è trascurabile nella maggior parte delle applicazioni pratiche. 

Questo significa inoltre che l'angolo tra i versori $\vec{n}$ e $\vec{\nu}$ è molto piccolo. Infatti questo misura al massimo 1 primo sessagesimale (1').

In generale vale la relazione
$$
N \simeq h-H
$$
Per quanto ci riguarda possiamo dire che
$$
N = h-H
$$

## Sistemi di coordinate fondamentali


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/2-semestre/topografia-e-positioning/appunti/sistemi-di-coordinate-fondamentali/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali\|Sistemi di coordinate fondamentali]]

[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di coordinate\|Sistema di coordinate]]

Possiamo definire diversi [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Sistema di coordinate\|sistemi di coordinate]]. In particolare vedremo:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate cartesiane geocentriche (G)\|#Coordinate cartesiane geocentriche (G)]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate ellissoidiche (E)\|#Coordinate ellissoidiche (E)]]
	- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate geografiche\|#Coordinate geografiche]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate cartografiche\|#Coordinate cartografiche]]


### Datum

Il datum è il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|sistema di riferimento]] in cui si sta lavorando.

```ad-example
title: Esempio

Ad esempio il datum $\rm WGS84$ rappresenta l'ellissoide di rotazione definito osservando l'asse di rotazione terrestre nel 1984, con dimensioni ($a,e^{2}$).
```


## Coordinate cartesiane Geocentriche (G)

Le Coordinate Cartesiane Geocentriche sono definite a partire dal seguente [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Sistema di riferimento\|#Sistema di riferimento]]
- $O:$ Baricentro terrestre
- $Z:$ Asse di rotazione terrestre
- $XZ:$ Piano meridiano di riferimento
- $Y:$ Asse ortogonale a completare terna destrorsa

![01 - Sistemi di riferimento e di coordinate - TP 2024-06-07 15.42.27.excalidraw.png|350](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-06-07%2015.42.27.excalidraw.png)


## Coordinate ellissoidiche (E)

Si può parlare di coordinate ellissoidiche solo dopo aver introdotto un ellissoide di riferimento. Faremo uso del [[WGS84\|WGS84]].

![02 - Campo gravitazionale - TP 2024-03-28 19.31.58.excalidraw.png](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-28%2019.31.58.excalidraw.png)


Nel diagramma è raffigurato un ellissoide di rotazione (ad esempio il [[WGS84\|WGS84]]) rispetto ai 3 assi cartesiani $x,y,z$. In particolare è raffigurato solo un ottavo dell'ellissoide, quello corrispondente ai semiassi positivi.

Si prende un punto $P$ qualunque sulla superficie terrestre e si vuole definire la sua posizione rispetto all'origine con un qualche sistema di coordinate.

Tracciamo quindi la <mark style="background: #FF5582A6;">normale</mark> all'ellissoide passante per il punto $P$, $\vec{n}$. Questa intersecherà l'ellissoide in un punto $P_{c}$. Tracciamo corrispondentemente l'arco dal polo all'equatore che passa per questo punto (<mark style="background: #ADCCFFA6;">tratto blu</mark>). Si traccia quindi un asse di riferimento, l'asse $r$, come in figura.

```ad-note
title: Osservazione

In generale, la normale in un punto all'ellissoide non passa per il centro dello stesso.

```


Andiamo ad individuare così 2 angoli:
- $\lambda:$ L'angolo tra il piano $xz$ e il piano $xr$ - lo chiameremo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#longitudine\|#longitudine]]
- $\varphi:$ L'angolo tra la normale $\vec{n}$ e l'asse $r$ - lo chiameremo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#latitudine\|#latitudine]]

Ogni punto sulla superficie terrestre sarà quindi individuato da coordinate:
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Quota\|#Quota]] $h$
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Latitudine\|#Latitudine]] $\varphi$
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Longitudine\|#Longitudine]] $\lambda$

```ad-example
title: Esempio
Vediamo alcuni punti e le rispettive coordinate.

- Punto al polo nord: LAT $\varphi= 90\degree$
- Punto sul piano $xz$: LON $\lambda = 0\degree$
- Punto sul piano $yz$: LON $\lambda = 90\degree$
```

### Datum

### Latitudine e Longitudine

Latitudine e longitudine sono due angoli e possono essere espressi in:
- Gradi sessagesimali: $aa\degree \,\,bb'\,\,cc.dd''$
- Gradi sessadecimali: $aa.bbbbbb \degree$

#### Longitudine

```ad-Definizione
title: Longitudine ($\lambda$)

La **Longitudine** (ellissoidica) è l'angolo diedro compreso tra il piano-$xz$ e il piano-$zr$

```

![Sistemi di coordinate fondamentali 2024-06-07 16.14.50.excalidraw.png](/img/user/Excalidraw/Sistemi%20di%20coordinate%20fondamentali%202024-06-07%2016.14.50.excalidraw.png)


La longitudine assume valori
$
\begin{align}
0\degree \le &\lambda \le 360\degree \\
-180\degree \le &\lambda \le 180\degree \\
180\degree \,\rm Ovest\le &\lambda <\le180\degree \,\rm Est
\end{align}
$
A seconda di come si decide di far variare l'angolo (le tre scrittura sopra sono perfettamente equivalenti).


#### Latitudine

```ad-Definizione
title: Latitudine ($\varphi$)

La **latitudine** (ellissoidica) è l'angolo $\varphi$ compreso tra il piano equatoriale e la normale all'ellissoide passante per il punto P.

```

![Sistemi di coordinate fondamentali 2024-06-07 16.13.57.excalidraw.png](/img/user/Excalidraw/Sistemi%20di%20coordinate%20fondamentali%202024-06-07%2016.13.57.excalidraw.png)


La latitudine assume valori
$
\begin{cases}
\varphi_{P}>0 \quad \text{Emisfero Boreale} \\
\varphi_{P}=0 \quad \text{Piano Equatoriale} \\
\varphi_{P}<0 \quad \text{Emisfero Australe}
\end{cases}
$
In particolare:
$
\begin{align}
-90\degree &\le \varphi \le 90\degree \\
&\text{oppure} \\
90 \degree \,\rm Sud &\le\varphi \le90\degree \rm Nord
\end{align}
$
### Coordinate geografiche

Le coordinate geografiche sono definite a partire dalle [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate ellissoidiche (E)\|#Coordinate ellissoidiche (E)]].

Se le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate ellissoidiche (E)\|#Coordinate ellissoidiche (E)]] sono
$
(\varphi, \lambda, h)
$
Le coordinate geografiche sono semplicemente:
$
(\varphi,\lambda)
$

Quindi, per ogni punto appartenente alla stessa normale, le coordinate geografiche sono identiche.

### Ellissoide orientato

![Schermata 2024-06-07 alle 18.07.29.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Topografia%20e%20Positioning/Appunti/allegati/Schermata%202024-06-07%20alle%2018.07.29.png)

Quando si ha necessità di lavorare su parti limitate del geoide, è possibile usare un ellissoide locale, in modo da meglio approssimare il geoide rispetto a quanto fa quello geocentrico.

Questo ellissoide è detto **ellissoide orientato**.

Quando si adopera l'ellissoide orientato, anche le coordinate cambiano.

![Schermata 2024-06-07 alle 18.08.26.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Topografia%20e%20Positioning/Appunti/allegati/Schermata%202024-06-07%20alle%2018.08.26.png)




## Coordinate Cartesiane locali (L)

Talvolta si considera un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|SR]] locale, centrato in un punto di interesse $P_{l}$ dell'ellissoide.

Le **Coordinate Cartesiane Locali** sono coordinate definite localmente. È necessario pertanto introdurre un origine locale.

```ad-Definizione
title: Sistema di coordinate cartesiane locali (L)

Un **sistema di coordinate cartesiane locali** (L) è un sistema che ha origine in $P_{l}$, un punto dell'ellissoide. È caratterizzato da 3 assi $(x,y,z)$. Di conseguenza $P_{l}(0,0,0)$.

```

Considero un solo ottante, come quando abbiamo definito le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate ellissoidiche\|#Coordinate ellissoidiche]].

![02 - Campo gravitazionale - TP 2024-04-03 19.20.58.excalidraw.png](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-04-03%2019.20.58.excalidraw.png)


Si osservi alla figura sopra. 
Il punto $P_{l}$, intersezione dell'ellissoide con la normale $\vec{n}$ è considerato come **origine locale**.

$\vec{n}$ è il versore perpendicolare e uscente dal piano tangente in $P_{l}$. Lo chiamiamo **"piano ($\Pi$) tg nel punto $P_{l}$"**.

Essendo $P_{l}$ la nuova origine, l'asse individuato da $\vec{n}$ è il nuovo asse $z$

Abbiamo così definito un nuovo sistema di coordinate, detto *sistema di coordinate cartesiane locali*.

In alto a destra nella figura è raffigurata la proiezione dell'ellissoide nel piano $zr$.

Gli assi del [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|SR]] locale sono pertanto:
- $z:$ Coincidente con la normale $\vec{n}$ - *uscente* dall'ellissoide
- $x:$ Diretto verso sud
- $y:$ Diretto verso est

L'asse $x$ è tangente al ramo dell'ellisse, l'asse $y$ invece è entrante nel foglio.

Considero un generico punto $P$ sull'asse $z$ (ossia $\vec{n}$). La distanza da $P$ a $P_{l}$ è la [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Quota ellissoidica\|#Quota ellissoidica]] $h$ ed in questo caso coincide con la coordinata $z$ di $P$

Considerando un altro punto $Q$ che non si trova su $z$, la coordinata $z_{Q}$ e l'altezza ellissoidica $h_{Q}$ non coincideranno più.

Questi sistemi di coordinate sono semplici da definire ma complicati dal punto di vista applicativo. 
Vengono in nostro soccorso le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]]

## Coordinate cartesiane di livello locale (LL)

Nelle [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]] l'asse-$z$ ( e di conseguenza gli altri assi) è definito a partire dalla normale all'ellissoide passante per il punto $P$. È utile però definire un sistema di coordinate il cui asse-$z$ sia definito a partire dalla direzione del [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Campo di gravità terrestre\|campo di gravità terrestre]]. Si va così a definire un sistema di **Coordinate cartesiane del Livello Locale**

Considero, a partire dal punto $P$ il versore che indica la forza di gravità ($\vec{\nu}$).

![01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.16.15.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-04-04%2010.16.15.excalidraw.png)


L'asse $z$ è individuato dal versore $\vec{\nu}$. Pertanto:
$
\begin{align}
z_{u} &\parallel \vec{\nu} \\
x_{u}, y_{u} &\perp \vec{\nu}
\end{align}
$
```ad-attention
Nel caso di [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]], il piano $\Pi$ era quello **tangente** all'ellissoide. Ossia era **perpendicolare** alla normale all'ellissoide ($\vec{n}$).

In questo caso, il piano $\Pi$ è **perpendicolare** alla **gravità** ($\vec{\nu}$).


![01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.39.13.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-04-04%2010.39.13.excalidraw.png)
%%[[01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.39.13.excalidraw.md|🖋 Edit in Excalidraw]]%%

$\vec{n}$ e $\vec{\nu}$ sono deviate di un angolo $\varepsilon$.

Localmente $\varepsilon$ è molto piccolo e quindi **trascurabile** ma MAI NULLO.

Facciamo l'ipotesi che $\vec{n} \equiv \vec{\nu}$.
```

$x_{u}, y_{u}$ giacciono sul piano orizzontale locale, quello identificato come perpendicolare al vettore $\vec{n}$.

Questo modello è più semplice perché l'asse $x_{u}$ è individuato dalla direzione della gravità.

Come si passa da questo sistema alle [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]]?

Se si trascura l'angolo $\varepsilon$ tra $\vec{n}$ e $\vec{\nu}$, tra le [[#Coordinate Cartesiane locali (L)]] e le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]], l'unica differenza è che gli assi $x$ e $y$ sono disposti come più fa comodo (e non allineati con le direzioni cardinali). Pertanto, passare da un sistema all'altro significa compiere una rotazione di un certo angolo $k$ attorno all'asse-$z$.

$
\begin{bmatrix}
x_{L} \\ y_{L} \\ z_{L}
\end{bmatrix}
=
\begin{bmatrix}
\cos(k) & \sin(k) & 0 \\
-\sin(k) & \cos(k) & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
x \\ y \\ z
\end{bmatrix}
$

## Coordinate cartografiche

Le **coordinate cartografiche** sono delle coordinate che si definiscono su una rappresentazione cartografica. Quando si proietta l'ellissoide terrestre sul piano si vanno a definire delle nuove coordinate dette appunto coordinate cartografiche

vd. [[06 - Cartografia - TP\|06 - Cartografia - TP]].


# Conversioni tra sistemi di coordinate


❗❗❗❗❗❗❗❗❗❗❗
❗❗❗COMPLETARE❗❗❗
❗❗❗❗❗❗❗❗❗❗❗







</div></div>
