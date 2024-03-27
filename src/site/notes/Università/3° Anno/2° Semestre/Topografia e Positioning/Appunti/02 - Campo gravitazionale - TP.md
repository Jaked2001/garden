---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/02-campo-gravitazionale-tp/"}
---

!
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
Il campo di gravità terrestre è la somma del [[#Campo gravitazionale]] e del [[#Campo della forza centrifuga]]

$$
\vec{g} = \vec{f} + \vec{c}
$$
```

#### Campo gravitazionale

Sappiamo, dalla fisica, che il campo gravitazionale è
$$
\vec{f} = -G \frac{Mm}{r^{3}} \vec{r}
$$
D'ora in poi, per semplicità, supporrò $m=1$. Guardo quindi al campo gravitazionale della Terra di massa $M$ che interagisce con una massa unitaria.
$$
\vec{f} = -G \frac{M}{r^{3}}\vec{r}
$$
Consideriamo la situazione sottostante:

![02 - Campo gravitazionale - TP 2024-03-21 17.32.51.excalidraw.png|450](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.32.51.excalidraw.png)


Prendo un punto $P$ fermo rispetto alla superficie terrestre. Questo punto subisce l'attrazione di ogni elementino della Terra, $dM$ situato nel punto $Q$.
pertanto, la forza di attrazione gravitazionale sarà data da:
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

```ad-note
title: Osservazione
La forza centrifuga, dipendendo da $|\vec{l_{P}}|$, è massima all'Equatore e nulla ai Poli.
Quindi la gravità varia lungo la superficie terrestre
- per direzione
- per modulo

```

![02 - Campo gravitazionale - TP 2024-03-21 17.32.51.excalidraw.png|450](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.32.51.excalidraw.png)


Anche il campo di forza centrifuga ammette un potenziale, detto **potenziale centrifugo**, per cui
$$
\vec{c} = \vec{\rm grad}C
$$
Si può dimostrare che il potenziale Newtoniano è pari a 
$$
V = G \int _{\text{Vol. Terra}} \frac{dM}{r_{PQ}} 
$$

##### Potenziale centrifugo

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

L'ellissoide usato oggi maggiormente e preso come riferimento è il [[WGS84\|WGS84]]. Quando parlo di $(a,b)$ o di $(a,e^{2})$ sto implicitamente facendo riferimento all'ellissoide [[WGS84\|WGS84]].

Nei nostri telefoni è in uso una descrizione semplificata del geoide: il [[EGM2008\|EGM2008]].








