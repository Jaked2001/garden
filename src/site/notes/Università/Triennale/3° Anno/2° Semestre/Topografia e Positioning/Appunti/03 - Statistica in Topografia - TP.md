---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/topografia-e-positioning/appunti/03-statistica-in-topografia-tp/"}
---

# [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP\|03 - Statistica in Topografia - TP]]




Ogni volta che facciamo una misura compiamo un errore. Ci sono diverse cause di errore:
- Strumento
- Operatore
- Ambiente

Gli errori di misura possono essere categorizzate in 3 tipologie:
- Noise
- Bias
- Outlier


Siamo interessati a definire un [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#centro\|#centro]] di misura.

### Robustezza

La robustezza è la proprietà di un indice statistico di resistere alla presenza di un [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Outlier\|#Outlier]].

```ad-Definizione
title: Robustezza

La robustezza di una grandezza è la sua capacità di resistere alla presenza di [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Outlier\|#Outlier]].

```


## Centro

```ad-Definizione
title: Centro

Quando si esegue una misura, il **centro** è il valore che decido essere rappresentativo del fenomeno stocastico che ho davanti.

```

Quando misuro una grandezza, intervengono molteplici cause di errore che generano una fluttuazione dei risultati di misura. A fronte di questi devo scegliere comunque un valore rappresentativo della misura, che è proprio il **centro**.

### Indici di centro

Il centro può essere scelto in vari modi, ognuno dei quali, vedremo, ha dei pro e dei contro. Iniziamo a vedere alcuni indici statistici che possiamo pensare di usare come [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]] di una misura:
- [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Media aritmetica\|#Media aritmetica]]
- [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Mediana\|#Mediana]]

#### Media aritmetica

```ad-Definizione
title: Media Aritmetica

$
\mu = \frac{1}{N} \sum\limits_{i=1}^{N} x_{i}
$
dove:
- $x_{i}:$ sono i valori di cui calcolo la media
- $N:$ la numerosità del campione
```

La media, per quanto semplice da calcolare, non è un buon parametro da prendere come [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]] di una serie di misure. La media infatti è molto [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Robustezza\|poco robusta]].

```ad-example
title: Esempio

Immaginiamo di avere il seguente set di dati:
$
\begin{align}
3.4721 \\
3.4718 \\
3.4719 \\
3.4723 \\
{\color{red} 4.4722}
\end{align}
$
Se calcoliamo la media solo dei primi 4 valori otteniamo $\mu = 3.4720$. Se invece includo anche il quinto valore (quello in rosso), ottengo $\mu = 3.6721$. È evidente che, con una singola misura molto diversa dalle altre, si ottenga una media molto diversa. 

In particolare si dice che 4.4722 è un [[#Outlier]] (= che sta fuori). Non è quindi rappresentativo del fenomeno rispetto agli altri 4 valori. 

Attenzione! Questo non vuol dire che sia sbagliato e gli altri giusti. Potrebbe essere l'unico esatto.
```



### Mediana

```ad-Definizione
title: Mediana
La **mediana** ($\rm Me$) è il valore tale che la [[#frequenza relativa]] dei valori minori di $\rm Me$ e dei valori maggiori di $\rm Me$ è la stessa e pari a 0.5.
$
\sum\limits_{i=1}^{N_{\rm Me}} f_{i} = \sum\limits_{i = N_{\rm Me}+1}^{N} f_{i} = 0.5
$
dove 
- $f_{i}:$ [[#Frequenza relativa]]

```

Qualora la variabile di cui si calcola la mediana fosse discreta (come avviene sempre nel caso si parli di grandezze derivanti da misurazioni), a seconda che il campione abbia numerosità $n$ pari o dispari, si sceglie il valore mediano come segue:
- $n$ pari: $\rm Me$ è la **media** $\mu$ dei valori centrali del campione
- $n$ dispari: $\rm Me$ è il **valore centrale** del campione

La mediana è una grandezza [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Robustezza di una grandezza\|robusta]].

```ad-note
title: Osservazione
Confrontando [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Media aritmetica\|#Media aritmetica]] e mediana posso accorgermi della presenza di [[#Outlier]]. Se media e mediana sono sostanzialmente vicini, è possibile che non ce ne siano. Al contrario, se differiscono di molto, è probabile che siano presenti degli outlier.

```

### Moda



## Dispersione

Gli errori a cui sono soggette le misure generano variabilità dei risultati di rappresentazione.

```ad-Definizione
title: Dispersione

La dispersione è il valore rappresentativo della variabilità della misura o della grandezza.

```

È possibile che due serie di misure abbiano la stessa media ma che in una le misure siano tutte molto vicine al valor medio, nell'altra molto lontane. Gli indici di dispersione permettono di quantificare questo fatto.

Stiamo implicitamente valutando la dispersione intorno al [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]].

Esistono vari indicatori di dispersione, tra cui:
- [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Varianza\|#Varianza]]
	- [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Deviazione Standard\|#Deviazione Standard]]
- [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#MAD (Median Absolute Deviation)\|#MAD (Median Absolute Deviation)]]
- ...

### Varianza

```ad-Definizione
title: Varianza ($\sigma^{2}$)

$
\sigma^{2} = \frac{1}{N} \sum\limits_{i=1}^{n} (x_{i}-\mu)^{2}
$

```

```ad-note
title: Osservazione
La varianza è un indice quadratico. Se ad esempio misuro lunghezze, queste sono misurate in metri. Se di una serie di misure calcolo la varianza, questa verrà restituita in metri quadri. Questa discrepanza di unità di misura fà si che più spesso si usi come indicatore la [[#Deviazione Standard]] (o *scarto quadratico medio*).

```

La varianza è [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Robustezza\|poco robusta]] essendo definita rispetto la [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Media aritmetica\|#Media aritmetica]] che è, come detto, a sua volta poco robusta.
#### Deviazione Standard

```ad-Definizione
title: Deviazione Standard o Scarto Quadratico Medio ($\sigma$)

La **deviazione standard** è ottenuta calcolando la radice quadrata della [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Varianza\|#Varianza]]

$
\sigma= \sqrt{\sigma^{2}}
$
```

La Deviazione standard è [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Robustezza\|poco robusta]]


### MAD (Median Absolute Deviation)

```ad-Definizione
title: Median Absolute Deviation ($MAD$)
La Median Absolute Deviation è un surrogato della [[#Varianza]] che usa la [[#Mediana]] al posto della [[#Mediana]] nel suo calcolo.
$
MAD = \rm Me (|x_{1}-\rm Me|)
$
```

Prendo il valore mediano degli scarti così che, dovesse ancora esserci un valore anomalo, questo verrebbe minimizzato.

È chiaro che, per come è definita, la MAD sia molto più robusta della [[#Varianza]].


#### NMAD (Normalized MAD)

La N.MAD è definita semplicemente come
$$
N.MAD = 1.48 MAD
$$
Qualora $N.MAD = \sigma$ possiamo affermare che la distribuzione di probabilità dei miei valori è assimilabile a una [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/03. Variabili Aleatorie#Variabile Aleatoria Normale o Gaussiana\|distribuzione normale (o Gaussiana)]].

Se $N.MAD \ne MAD$
- O ci sono [[#Outlier]]
- O la distribuzione di probabilità non è una normale

#### Min-Max

Il minimo e il massimo di una distribuzione rappresentano la [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Dispersione\|#Dispersione]] come l'intervallo nel quale sono contenuti tutti i valori.
$$
{\rm MinMax} = x_{MAX} - x_{min}
$$
Non è affatto un indice [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Robustezza\|robusto]].

Questo indicatore è utile per ricordare il [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Teorema di Cebicev\|#Teorema di Cebicev]]

##### Teorema di Cebicev

```ad-Teo
title: Teo di Cevicev

Dato un intervallo:
$
I_{\lambda}= (\mu-\lambda\sigma, \mu+\lambda\sigma) \quad \lambda \ge 1
$
indipendentemente dalla distribuzione di probabilità, la probabilità che una variabile $x$ appartenga all'intervallo $I_\lambda$ è maggiore o uguale a $1-\dfrac{1}{\lambda^{2}}$.
$
\mathcal{P}(I_{\lambda}) \ge 1 - \frac{1}{\lambda^{2}}
$

```

Quindi:
- $\lambda = 1 \quad\Longrightarrow\quad \mathcal{P}(I_{\lambda}) \ge 0$
- $\lambda = 2 \quad\Longrightarrow\quad \mathcal{P}(I_{\lambda}) \ge 0.75$
- $\lambda = 3 \quad\Longrightarrow\quad \mathcal{P}(I_{\lambda}) \ge 0.91$

### Covarianza

```ad-Definizione
title: Covarianza

La **covarianza** è una misura della dipendenza aleatoria o stocastica tra due componenti della variabile casuale, che non sia una dipendenza funzionale.
$
\sigma_{x_{i},x_{j}} = \frac{1}{N} \sum\limits_{k=1}^{N}(x_{ik}-\mu_{i})(x_{jk}-\mu_{j})
$
Si noti che nel caso in cui $i=j$ la covarianza coincide con la [[#Varianza]].
```

Supponiamo di avere una variabile bidimensionale $(i,j)$. Ogni volta che eseguo una misurazione ottengo entrambe le componenti. Ripeto tante volte la misurazione e si ottiene (riportando i dati su un piano cartesiano) una distribuzione di punti come in figura.

![03 - Statistica in Topografia - TP 2024-05-22 11.59.06.excalidraw.png](/img/user/Excalidraw/03%20-%20Statistica%20in%20Topografia%20-%20TP%202024-05-22%2011.59.06.excalidraw.png)


Notiamo che i punti si addensano in una certa regione del piano e questo fa pensare che il modo di variare di una delle due componenti condizioni il modo di variare dell'altra.

![03 - Statistica in Topografia - TP 2024-05-22 13.30.25.excalidraw.png](/img/user/Excalidraw/03%20-%20Statistica%20in%20Topografia%20-%20TP%202024-05-22%2013.30.25.excalidraw.png)


Si guardi ai due grafici sopra. In quello a sinistro la covarianza esiste ed è diversa da zero: $\sigma_{ij}$. Si può quindi definire una retta di regressione lineare. Nel secondo caso, la covarianza è uguale a zero: $\sigma_{ij}=0$. Quindi, in questo caso:
- Non c'è dipendenza lineare
- Il problema ha infinite dimensioni
In pratica in quest'ultimo caso qualsiasi retta di regressione è corretta.

La covarianza si rappresenta in forma matriciale:

#### Matrice di covarianza

È data una [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/01. Osservazione e probabilità#Variabili aleatorie\|variabile aleatoria]] $X$ di $n$-dimensioni

Definiamo una matrice $C_{XX}$ che sia:
- Quadrata di ordine $n$
- Simmetrica
- Definita positiva: $a^{T}C_{XX} \ge 0 \forall a \in \mathbb{R}^{n}$

$$
\underset{(n,n)}{C_{XX}} =
\begin{bmatrix}
\sigma_{X_{1}}^{2} & \sigma_{X_{1},X_{2}} & \dots & \sigma_{X_{1},X_{n}} \\
\sigma_{X_{2},X_{2}} & \sigma_{X_{2}}^{2} & \dots & \sigma_{X_{2},X_{n}} \\
\vdots & \vdots & \ddots & \vdots \\
\sigma_{X_{n},X_{n}} & \sigma_{X_{n},X_{2}} & \dots & \sigma_{X_{n}}^{2}
\end{bmatrix}
\in \rm Sym
$$


### Coefficiente di correlazione lineare

### Dipendenza e Indipendenza stocastica


## Teorema della media

Usiamo il teorema della media per passare da ciò che misuriamo a ciò che calcoliamo. Il Teo. della Media può essere usato solamente se scegliamo la [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Media aritmetica\|#Media aritmetica]] come [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]] della misura.

Rappresento la variabile di misura con una [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/01. Osservazione e probabilità#Variabili aleatorie\|variabile aleatoria]] (v.a.)

- $x:$ Misura - Variabile della quale conosco il [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]]
- $y:$ Risultato - Variabile della quale voglio determinare il [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]] - Variabile **obiettivo**
So che posso definire $y$ come una qualche funzione $g$ di $x$:
$$
y = g(x)
$$

Siamo interessati a un [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Corollario al Teo della Media\|#Corollario al Teo della Media]]:

### Corollario al Teo della Media

```ad-Teo
title: Corollario al Teo della Media

Date le [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/01. Osservazione e probabilità#Variabili aleatorie\|variabili aleatorie]]:
- $X$ - $n$-dimensioni
- $Y$ - $m$-dimensioni

Siano rispettivamente
- $\mu_{X}:$ la [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Media aritmetica\|#Media aritmetica]] di $X$
- $\mu_{y}:$ la [[#Media aritmetica]] di $Y$

Si ha che:
$
\underbrace{\mu_{X}}_{(n,1)} =
\begin{bmatrix}
\mu_{X_{1}} \\
\mu_{X_{2}} \\
\vdots \\
\mu_{X_{n}}
\end{bmatrix}
\qquad
\underbrace{\mu_{Y}}_{(m,1)} =
\begin{bmatrix}
\mu_{Y_{1}} \\
\mu_{Y_{2}} \\
\vdots \\
\mu_{Y_{m}}
\end{bmatrix}
$
Sia inoltre $Y = G(X)$: $Y$ è una funzione di $X$ nota.

Se sono rispettate le seguenti ipotesi:
- Buona concentrazione ([[#Deviazione Standard]] piccola)
- Regolarità funzionale quasi ovunque

**Allora**
$
\mu_{Y} \approx G(\mu_{X})
$


```

In pratica il teorema dice che le medie di 2 variabili aleatorie sono legate (con buona approssimazione) dalla stessa funzione che lega le variabili stesse ammesso che la deviazione standard sia piccola e che la funzione sia sufficientemente regolare.

```ad-note
title: Osservazione
Il Corollario al Teo della media risulta esatto ($\mu_{Y} = G(\mu_{X})$) se la funzione che lega le due variabili aleatorie è **lineare**, ossia se:
$
Y = AX+b
$

```


```ad-example
title: Esempio

![03 - Statistica in Topografia - TP 2024-05-22 13.56.11.excalidraw.png](/img/user/Excalidraw/03%20-%20Statistica%20in%20Topografia%20-%20TP%202024-05-22%2013.56.11.excalidraw.png)
%%[[03 - Statistica in Topografia - TP 2024-05-22 13.56.11.excalidraw.md|🖋 Edit in Excalidraw]]%%
(ndr. ignora $\sigma^{2}$ nel diagramma)

Consideriamo un rettangolo di base $b$ e altezza $h$.
- Misuro $b$ e $h$ più volte
- Rappresento il [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]] di $b$ e $h$ usando la [[#Media aritmetica]]
	- Conosco: $\mu_{b}$ e $\mu_{h}$

Vogliamo ricavare perimetro $p$, area $A$ e diagonale $d$.

___

- Perimetro: $p=2(b+h)$
- Area: $A=b\cdot h$
- Diagonale: $d=\sqrt{b^{2}+h^{2}}$

La variabile aleatoria $X$ in questo caso è: $X = \begin{bmatrix} b \\ h \end{bmatrix}$

La variabile aleatoria $Y$ è a 3 dimensioni: $Y = \begin{bmatrix} p \\ A \\ d \end{bmatrix}$

Il funzionale $G(X)$ è l'insieme delle funzioni che legano $X$ a $Y$:
$
G(X) =
\begin{bmatrix}
2(b+h) \\
b\cdot h \\
\sqrt{b^{2}+h^{2}}
\end{bmatrix}
$
Si noti che, a parte per il perimetro, il legame è **NON** lineare. Devo applicare il teorema della media in forma approssimata. Posso quindi dire
$
\mu_{Y} =
\begin{bmatrix}
\mu_{p} \\
\mu_{A} \\
\mu_{d}
\end{bmatrix}
=
\begin{bmatrix}
2(\mu_{b}+\mu_{h}) \\
\mu_{b}\cdot \mu_{h} \\
\sqrt{\mu_{b}^{2}+\mu_{h}^{2}}
\end{bmatrix}
$

```


### Legge di propagazione della covarianza

Date le [[01. Osservazione e probabilità#Variabili aleatorie|variabili aleatorie]]:
- $X$ - $n$-dimensioni
- $Y$ - $m$-dimensioni

Siano rispettivamente
- $\mu_{X}:$ la [[#Media aritmetica]] di $X$
- $\mu_{y}:$ la [[#Media aritmetica]] di $Y$

Si ha che:
$$
\underbrace{\mu_{X}}_{(n,1)} =
\begin{bmatrix}
\mu_{X_{1}} \\
\mu_{X_{2}} \\
\vdots \\
\mu_{X_{n}}
\end{bmatrix}
\qquad
\underbrace{\mu_{Y}}_{(m,1)} =
\begin{bmatrix}
\mu_{Y_{1}} \\
\mu_{Y_{2}} \\
\vdots \\
\mu_{Y_{m}}
\end{bmatrix}
$$
Sia inoltre $Y = G(X)$: $Y$ è una funzione di $X$ nota.

Considerata la [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Matrice di covarianza\|#Matrice di covarianza]] $C_{XX}$:
$$
\underset{(n,n)}{C_{XX}} =
\begin{bmatrix}
\sigma_{x_{1}}^{2} & \sigma_{x_{1},x_{2}} & \dots & \sigma_{x_{1},x_{n}} \\
\sigma_{x_{2},x_{2}} & \sigma_{x_{2}}^{2} & \dots & \sigma_{x_{2},x_{n}} \\
\vdots & \vdots & \ddots & \vdots \\
\sigma_{x_{n},x_{n}} & \sigma_{x_{n},x_{2}} & \dots & \sigma_{x_{n}}^{2}
\end{bmatrix}
\in \rm Sym
$$
$C_{XX}$ è una matrice **definita positiva** (tutti autovalori nulli o positivi).

Per la **legge di propagazione della covarianza**, se sono rispettate le stesse ipotesi del [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Corollario al Teo della Media\|#Corollario al Teo della Media]], si ha che:
$$
C_{YY} = J_{\mu_{X}} C_{XX} J_{\mu_{X}}^{T}
$$
Dove:
- $J_{\mu_{X}}:$ Matrice Jacobiana (Matrice delle derivate prime) del funzionale $G(X)$

Come è fatta $J$:
- $J$ ha tante righe quante sono le dimensioni del funzionale --> $m$
- $J$ ha tante colonne quante sono le dimensioni del vettore $X$ --> $n$

In definitiva $J$ è:
$$
\underset{(m,n)}{J} =
\begin{bmatrix}
\dfrac{\partial g_{1}}{\partial x_{1}} & \dfrac{\partial g_{1}}{\partial x_{2}} & \cdots &  \dfrac{\partial g_{1}}{\partial x_{n}} \\
\dfrac{\partial g_{2}}{\partial x_{2}} & \dfrac{\partial g_{1}}{\partial x_{2}} & \cdots &  \dfrac{\partial g_{2}}{\partial x_{n}} \\
\vdots & \vdots & \ddots & \vdots \\
\dfrac{\partial g_{m}}{\partial x_{1}} & \dfrac{\partial g_{m}}{\partial x_{2}} & \cdots &  \dfrac{\partial g_{m}}{\partial x_{n}}
\end{bmatrix}
$$
Devo valutare la matrice in $\mu_{X}$
$$
\underset{(m,n)}{J}(\mu_{X}) =
\begin{bmatrix}
\dfrac{\partial g_{1}}{\partial x_{1}} & \dfrac{\partial g_{1}}{\partial x_{2}} & \cdots &  \dfrac{\partial g_{1}}{\partial x_{n}} \\
\dfrac{\partial g_{2}}{\partial x_{2}} & \dfrac{\partial g_{1}}{\partial x_{2}} & \cdots &  \dfrac{\partial g_{2}}{\partial x_{n}} \\
\vdots & \vdots & \ddots & \vdots \\
\dfrac{\partial g_{m}}{\partial x_{1}} & \dfrac{\partial g_{m}}{\partial x_{2}} & \cdots &  \dfrac{\partial g_{m}}{\partial x_{n}}
\end{bmatrix}_{\mu_{X}}
$$

```ad-example
title: Esempio

![03 - Statistica in Topografia - TP 2024-05-22 13.56.11.excalidraw.png](/img/user/Excalidraw/03%20-%20Statistica%20in%20Topografia%20-%20TP%202024-05-22%2013.56.11.excalidraw.png)
%%[[03 - Statistica in Topografia - TP 2024-05-22 13.56.11.excalidraw.md|🖋 Edit in Excalidraw]]%%

Consideriamo un rettangolo di base $b$ e altezza $h$.
- Misuro $b$ e $h$ più volte
- Rappresento il [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]] di $b$ e $h$ usando la [[#Media aritmetica]]
- Rappresento la dispersione di $b$ e di $h$ usando i rispettivi [[#Deviazione Standard|scarti quadratici medi]]

Vogliamo valutare la [[#Covarianza]] di $b$ e $h$

Voglio valutare la dipendenza stocastica perché le nostre cause di incertezza sono classificabili in 3 grandi classi:
- strumento
- operatore
- ambiente

Anche se mi aspetto che base e altezza siano due misure tra loro stocasticamente indipendenti, è raro che questo avvenga proprio perché sono misure "prese" con lo stesso strumento e magari dallo stesso operatore e quindi sottoposte allo tesso errore che influenza la misura

Sappiamo che
$
Y = 
\begin{bmatrix}
P \\
A \\
d
\end{bmatrix}
=
\begin{bmatrix}
2(b+h) \\
b\cdot h \\
\sqrt{b^{2}+h^{2}}
\end{bmatrix}
=G(X)
$
Al fine di calcolare la $C_{YY}$ devo come prima cosa calcolare $C_{XX}$
$
\underset{(2,2)}{C_{XX}} =
\begin{bmatrix}
\sigma^{2}_{b} & \sigma_{bh} \\
\sigma_{bh} & \sigma^{2}_{h}
\end{bmatrix}
$
A questo punto devo calcolare la Jacobiana:
$
\underset{(3,2)}{J} =
\begin{bmatrix}
\dfrac{\partial p}{\partial b} & \dfrac{\partial p}{\partial h} \\
\dfrac{\partial A}{\partial b} & \dfrac{\partial A}{\partial h} \\
\dfrac{\partial d}{\partial b} & \dfrac{\partial d}{\partial h}
\end{bmatrix}
=
\begin{bmatrix}
2 & 2 \\
h & b \\
\dfrac{b}{\sqrt{b^{2}+h^{2}}} & \dfrac{h}{\sqrt{b^{2}+h^{2}}}
\end{bmatrix}_{\mu_{X}}
$
Ricordo:
$
\mu_{X} =
\begin{bmatrix}
\mu_{b} \\
\mu_{h}
\end{bmatrix}
$
e quindi:
$
J(\mu_{X}) =
\begin{bmatrix}
2 & 2 \\
\mu_{h} & \mu_{b} \\
\dfrac{\mu_{b}}{\sqrt{\mu_{b}^{2}+\mu_{h}^{2}}} & \dfrac{\mu_{h}}{\sqrt{\mu_{b}^{2}+\mu_{h}^{2}}}
\end{bmatrix}
$
A questo punto si può calcolare $C_{YY}$  come 
$
C_{YY} = J(\mu_{X})C_{XX}J(\mu_{X})^{T}
$
Le cui componenti saranno:
$
\underset{(3,3)}{C_{YY}} =
\begin{bmatrix}
\sigma^{2}_{p} & \sigma_{pA} & \sigma_{pd} \\
\sigma_{Ap} & \sigma_{A}^{2} & \sigma_{Ad} \\
\sigma_{dp} & \sigma_{dA} & \sigma^{2}_{d}
\end{bmatrix}
$

```

## Applicazione al cambio di coordinate

![03 - Statistica in Topografia - TP 2024-05-22 14.37.05.excalidraw.png](/img/user/Excalidraw/03%20-%20Statistica%20in%20Topografia%20-%20TP%202024-05-22%2014.37.05.excalidraw.png)


Si immagini di avere le seguenti quantità con le rispettive [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Media aritmetica\|medie]]:
- $\alpha:$ [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#\|##direzione azimutale]] $\longrightarrow \mu_\alpha$
- $z:$ [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#\|##angolo zenitale]] $\longrightarrow \mu_{z}$
- $d:$ distanza $\longrightarrow \mu_{d}$

A queste misure corrisponde una [[Università/Triennale/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Matrice di covarianza\|#Matrice di covarianza]] $C_{\alpha z d,\alpha z d}$
Si avrà quindi
$$
X =
\begin{bmatrix}
\alpha \\
z \\
d
\end{bmatrix}
\qquad
\mu_{X} =
\begin{bmatrix}
\mu_{\alpha} \\
\mu_{z} \\
\mu_{d}
\end{bmatrix}
\qquad
C=
\begin{bmatrix}
\sigma_{\alpha}^{2} & \sigma_{\alpha z} & \sigma_{\alpha d} \\
\sigma_{z \alpha} & \sigma_{z}^{2} & \sigma_{z d} \\
\sigma_{d \alpha} & \sigma_{dz} & \sigma_{d}^{2}
\end{bmatrix}
$$
Nonché
$$
Y =
\begin{bmatrix}
x_{LP} \\
y_{LP} \\
z_{LP}
\end{bmatrix}
\qquad
\mu_{Y} =
\begin{bmatrix}
\mu_{x_{LP}} \\
\mu_{y_{LP}} \\
\mu_{z_{LP}}
\end{bmatrix}
\qquad
C =
\begin{bmatrix}
\sigma_{x_{LP}}^{2} & \sigma_{xy} & \sigma_{xz} \\
\sigma_{yx} & \sigma_{y_{LP}}^{2} & \sigma_{yz} \\
\sigma_{zx} & \sigma_{zy} & \sigma_{z_{LP}}^{2}
\end{bmatrix}
$$

Possiamo scrivere che $Y = G(X)$. Abbiamo quindi bisogno di definire $G$
Vediamo che:
$$
\underset{Y}
{
\begin{bmatrix}
x_{LP} \\
y_{LP} \\
z_{LP}
\end{bmatrix}
}
=
\underset{X}
{\begin{bmatrix}
d\sin z \sin \alpha \\
d \sin z \cos \alpha \\
d \cos z
\end{bmatrix}}
$$

...


# Misure

## Precisione vs Accuratezza

![03 - Statistica in Topografia - TP 2024-05-22 15.13.34.excalidraw.png](/img/user/Excalidraw/03%20-%20Statistica%20in%20Topografia%20-%20TP%202024-05-22%2015.13.34.excalidraw.png)


### Precisione

```ad-Definizione
title: Precisione

La **Precisione** fa riferimento alla [[#Dispersione]] attorno al [[#Centro]] della misura.

```

Se ad esempio consideriamo un tiratore al bersaglio, questo sarà **preciso** se tutti i suoi colpi cadono molto vicini tra loro, sempre più o meno nello stesso punto, al di là che questi siano o meno vicino al centro del bersaglio.

In questo caso il [[#Centro]] non si avvicina al risultato esatto ma tutti i dati sono abbastanza vicini al centro.

### Accuratezza

```ad-Definizione
title: Accuratezza

L'**accuratezza** fa riferimento alla [[#Dispersione]] attorno a un riferimento esterno

```

Se ad esempio consideriamo un tiratore al bersaglio, questo sarà **accurato** se tutti i suoi colpi cadono in un qualche intorno del centro del bersaglio anche se sono molto lontani tra loro.

In questo caso il [[#Centro]] si avvicina molto al risultato esatto ma i dati sono tutti lontani dal centro

