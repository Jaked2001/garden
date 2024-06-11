---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/sistemi-di-coordinate-fondamentali/","tags":["UNI"]}
---


# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali\|Sistemi di coordinate fondamentali]]

[[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di coordinate\|Sistema di coordinate]]

Possiamo definire diversi [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Sistema di coordinate\|sistemi di coordinate]]. In particolare vedremo:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate cartesiane geocentriche (G)\|#Coordinate cartesiane geocentriche (G)]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate ellissoidiche (E)\|#Coordinate ellissoidiche (E)]]
	- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate geografiche\|#Coordinate geografiche]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate cartografiche\|#Coordinate cartografiche]]


### DATUM

```ad-Definizione
title: DATUM

Il **DATUM** è il [[01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento|sistema di riferimento]] al quale è associato un certo ellissoide nella sua forma geometrica e come questo ellissoide è posizionato rispetto al geoide e quindi al corpo fisico della Terra

```


```ad-example
title: Esempio

Ad esempio il datum $\rm WGS84$ rappresenta l'ellissoide di rotazione definito osservando l'asse di rotazione terrestre nel 1984, con dimensioni ($a,e^{2}$).
```


## Coordinate cartesiane Geocentriche (G)

Le Coordinate Cartesiane Geocentriche sono definite a partire dal seguente [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Sistema di riferimento\|#Sistema di riferimento]]
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
- $\lambda:$ L'angolo tra il piano $xz$ e il piano $xr$ - lo chiameremo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#longitudine\|#longitudine]]
- $\varphi:$ L'angolo tra la normale $\vec{n}$ e l'asse $r$ - lo chiameremo [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#latitudine\|#latitudine]]

Ogni punto sulla superficie terrestre sarà quindi individuato da coordinate:
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Quota\|#Quota]] $h$
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Latitudine\|#Latitudine]] $\varphi$
- La [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Longitudine\|#Longitudine]] $\lambda$

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
$$
\begin{align}
0\degree \le &\lambda \le 360\degree \\
-180\degree \le &\lambda \le 180\degree \\
180\degree \,\rm Ovest\le &\lambda <\le180\degree \,\rm Est
\end{align}
$$
A seconda di come si decide di far variare l'angolo (le tre scrittura sopra sono perfettamente equivalenti).


#### Latitudine

```ad-Definizione
title: Latitudine ($\varphi$)

La **latitudine** (ellissoidica) è l'angolo $\varphi$ compreso tra il piano equatoriale e la normale all'ellissoide passante per il punto P.

```

![Sistemi di coordinate fondamentali 2024-06-07 16.13.57.excalidraw.png](/img/user/Excalidraw/Sistemi%20di%20coordinate%20fondamentali%202024-06-07%2016.13.57.excalidraw.png)


La latitudine assume valori
$$
\begin{cases}
\varphi_{P}>0 \quad \text{Emisfero Boreale} \\
\varphi_{P}=0 \quad \text{Piano Equatoriale} \\
\varphi_{P}<0 \quad \text{Emisfero Australe}
\end{cases}
$$
In particolare:
$$
\begin{align}
-90\degree &\le \varphi \le 90\degree \\
&\text{oppure} \\
90 \degree \,\rm Sud &\le\varphi \le90\degree \rm Nord
\end{align}
$$
### Coordinate geografiche

Le coordinate geografiche sono definite a partire dalle [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate ellissoidiche (E)\|#Coordinate ellissoidiche (E)]].

Se le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate ellissoidiche (E)\|#Coordinate ellissoidiche (E)]] sono
$$
(\varphi, \lambda, h)
$$
Le coordinate geografiche sono semplicemente:
$$
(\varphi,\lambda)
$$

Quindi, per ogni punto appartenente alla stessa normale, le coordinate geografiche sono identiche.

### Ellissoide orientato

![Schermata 2024-06-07 alle 18.07.29.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Topografia%20e%20Positioning/Appunti/allegati/Schermata%202024-06-07%20alle%2018.07.29.png)

Quando si ha necessità di lavorare su parti limitate del geoide, è possibile usare un ellissoide locale, in modo da meglio approssimare il geoide rispetto a quanto fa quello geocentrico.

Questo ellissoide è detto **ellissoide orientato**.

Quando si adopera l'ellissoide orientato, anche le coordinate cambiano.

![Schermata 2024-06-07 alle 18.08.26.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Topografia%20e%20Positioning/Appunti/allegati/Schermata%202024-06-07%20alle%2018.08.26.png)

Gli ellissoidi orientati usati in ambito nazionale sono 5:
- 2 attinenti a UTM e Gauss-Boaga
- 3 storici - utilizzati nella cartografia catastale

#### DATUM Roma 1940

Il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#DATUM\|#DATUM]] **Roma 1940** è quello che fa riferimento all'ellissoide cosiddetto **internazionale** oppure **Heyford-1924**.

In ambito nazionale, si è preso l'ellissoide internazionale e si è imposta la condizione che, all'Osservatorio di Roma Monte Mario la verticale fisica (filo a piombo) e la normale all'ellissoide coincidano.

L'ellissoide si dice **orientato ad un punto**.

In realtà un punto non basta a definire l'ellissoide. Ne serve un altro. Si è scelto Genova, dove è presente il **mareografo fondamentale nazionale** --> oggetto che misura continuamente il livello del mare e permette di definire dove passa il geoide.

A Genova, si è imposto che geoide ed ellissoide passino per lo stesso punto.

Le condizioni sono pertanto:
1. $\vec{n_{MM}} = \vec{\nu_{MM}}$ - Normale all'ellissoide e verticale fisica coincidenti a Monte Mario
2. $N_{G} = 0$ - [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Ondulazione del geoide\|Ondulazione del geoide]] nulla a Genova

![Sistemi di coordinate fondamentali 2024-06-08 10.37.05.excalidraw.png](/img/user/Excalidraw/Sistemi%20di%20coordinate%20fondamentali%202024-06-08%2010.37.05.excalidraw.png)


Con le condizioni imposte, l'ellissoide in realtà non è ancora definito in maniera **univoca**. Infatti, entrambe le configurazioni sottostanti rispettano le condizioni 1. e 2.:

![Sistemi di coordinate fondamentali 2024-06-08 10.43.19.excalidraw.png](/img/user/Excalidraw/Sistemi%20di%20coordinate%20fondamentali%202024-06-08%2010.43.19.excalidraw.png)


È pertanto necessario introdurre un'altra condizione sull'asse di rotazione dell'ellissoide.
- Si considera solo l'ellissoide il cui asse di rotazione sia parallelo all'asse di rotazione terrestre

```ad-Teo
title: DATUM Roma 1940

In definitiva, le condizioni del DATU Roma 1940 sono:
1. $\vec{n_{MM}} = \vec{\nu_{MM}}$ - Normale all'ellissoide e verticale fisica coincidenti a Monte Mario
2. $N_{G} = 0$ - [[02 - Campo gravitazionale - TP#Ondulazione del geoide|Ondulazione del geoide]] nulla a Genova
3. Si considera solo l'ellissoide il cui asse di rotazione sia parallelo all'asse di rotazione terrestre


```



#### DATUM Roma 1950

![Schermata 2024-06-08 alle 11.17.22.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Topografia%20e%20Positioning/Appunti/allegati/Schermata%202024-06-08%20alle%2011.17.22.png)





## Coordinate Cartesiane locali (L)

Talvolta si considera un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento\|SR]] locale, centrato in un punto di interesse $P_{l}$ dell'ellissoide.

Le **Coordinate Cartesiane Locali** sono coordinate definite localmente. È necessario pertanto introdurre un origine locale.

```ad-Definizione
title: Sistema di coordinate cartesiane locali (L)

Un **sistema di coordinate cartesiane locali** (L) è un sistema che ha origine in $P_{l}$, un punto dell'ellissoide. È caratterizzato da 3 assi $(x,y,z)$. Di conseguenza $P_{l}(0,0,0)$.

```

Considero un solo ottante, come quando abbiamo definito le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate ellissoidiche\|#Coordinate ellissoidiche]].

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

Considero un generico punto $P$ sull'asse $z$ (ossia $\vec{n}$). La distanza da $P$ a $P_{l}$ è la [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Quota ellissoidica\|#Quota ellissoidica]] $h$ ed in questo caso coincide con la coordinata $z$ di $P$

Considerando un altro punto $Q$ che non si trova su $z$, la coordinata $z_{Q}$ e l'altezza ellissoidica $h_{Q}$ non coincideranno più.

Questi sistemi di coordinate sono semplici da definire ma complicati dal punto di vista applicativo. 
Vengono in nostro soccorso le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]]

## Coordinate cartesiane di livello locale (LL)

Nelle [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]] l'asse-$z$ ( e di conseguenza gli altri assi) è definito a partire dalla normale all'ellissoide passante per il punto $P$. È utile però definire un sistema di coordinate il cui asse-$z$ sia definito a partire dalla direzione del [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP#Campo di gravità terrestre\|campo di gravità terrestre]]. Si va così a definire un sistema di **Coordinate cartesiane del Livello Locale**

Considero, a partire dal punto $P$ il versore che indica la forza di gravità ($\vec{\nu}$).

![01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.16.15.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-04-04%2010.16.15.excalidraw.png)


L'asse $z$ è individuato dal versore $\vec{\nu}$. Pertanto:
$$
\begin{align}
z_{u} &\parallel \vec{\nu} \\
x_{u}, y_{u} &\perp \vec{\nu}
\end{align}
$$
```ad-attention
Nel caso di [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]], il piano $\Pi$ era quello **tangente** all'ellissoide. Ossia era **perpendicolare** alla normale all'ellissoide ($\vec{n}$).

In questo caso, il piano $\Pi$ è **perpendicolare** alla **gravità** ($\vec{\nu}$).


![01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.39.13.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-04-04%2010.39.13.excalidraw.png)
%%[[01 - Sistemi di riferimento e di coordinate - TP 2024-04-04 10.39.13.excalidraw.md|🖋 Edit in Excalidraw]]%%

$\vec{n}$ e $\vec{\nu}$ sono deviate di un angolo $\varepsilon$.

Localmente $\varepsilon$ è molto piccolo e quindi **trascurabile** ma MAI NULLO.

Facciamo l'ipotesi che $\vec{n} \equiv \vec{\nu}$.
```

$x_{u}, y_{u}$ giacciono sul piano orizzontale locale, quello identificato come perpendicolare al vettore $\vec{n}$.

Questo modello è più semplice perché l'asse $x_{u}$ è individuato dalla direzione della gravità.

Come si passa da questo sistema alle [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate Cartesiane locali (L)\|#Coordinate Cartesiane locali (L)]]?

Se si trascura l'angolo $\varepsilon$ tra $\vec{n}$ e $\vec{\nu}$, tra le [[#Coordinate Cartesiane locali (L)]] e le [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Coordinate cartesiane di livello locale (LL)\|#Coordinate cartesiane di livello locale (LL)]], l'unica differenza è che gli assi $x$ e $y$ sono disposti come più fa comodo (e non allineati con le direzioni cardinali). Pertanto, passare da un sistema all'altro significa compiere una rotazione di un certo angolo $k$ attorno all'asse-$z$.

$$
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
$$

## Coordinate cartografiche

Le **coordinate cartografiche** sono delle coordinate che si definiscono su una rappresentazione cartografica. Quando si proietta l'ellissoide terrestre sul piano si vanno a definire delle nuove coordinate dette appunto coordinate cartografiche

vd. [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP\|06 - Cartografia - TP]].


# Conversioni tra sistemi di coordinate


❗❗❗❗❗❗❗❗❗❗❗
❗❗❗COMPLETARE❗❗❗
❗❗❗❗❗❗❗❗❗❗❗





