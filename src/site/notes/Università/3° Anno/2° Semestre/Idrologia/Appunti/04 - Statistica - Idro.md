---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/idrologia/appunti/04-statistica-idro/"}
---

# [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro\|04 - Statistica - Idro]]

## Esperimento casuale




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/2-semestre/probabilita-e-statistica/appunti/02-misura-e-probabilita/#spazio-di-probabilita" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Spazio di probabilità


```ad-Definizione
title: Spazio di probabilità
Uno spazio di probabilità è l'insieme $\Omega$ di tutti i possibili risultati, esaustivi e mutualmente esclusivi, di un dato esperimento casuale.

$
(\Omega, \mathcal{A}, P)
$
Dove
- $\Omega =$ Insieme eventi elementari
- $\mathcal{A} =$ "$\sigma$-Algebra indotta da $\Omega$" --> Insieme di tutti gli eventi ai quali possiamo essere interessati
- $P=$ Probabilità: $P: \mathcal{A} \to [0,1]$


```

$\sigma$-algebra è indotta da Omega. Si ottiene per chiusura di $\Omega$.

```ad-summary
title: Esempio: dado regolare

Nell'esempio del dado regolare abbiamo:
$\Omega = \{ 1,2,3,4,5,6 \}$  l'insieme degli eventi elementari

Se volessimo calcolare la probabilità che esca un numero $k$ otterremmo:

$
P(D=k) = 
\begin{cases}
\frac{1}{6} &\, k \in \Omega \\
0 &\, k \in \Omega^{c}
\end{cases}
\,\,\,\, k \in \mathbb{Z}
$

La probabilità che esca un numero pari è invece:
$
P(D \in \{ 2,4,6 \}) = P(\{2,4,6\}) = \frac{3}{6} = \frac{1}{2} = \frac{|\{ 2,4,6 \}|}{|\Omega|}
$

L'insieme di tutti gli eventi ai quali possiamo essere interessati è invece $\mathcal{A}$:
$
\mathcal{A} = \{ \Omega, \emptyset, \{1,2\},..., \{ 1,2,3\}, ... \}
$
Si ha poi che:
$P(\Omega) = 1$
$P(\Omega^{c}) = 0$


```


___
[[_Giornaliera/2023-03-03\|2023-03-03]]
___

$\mathcal{A}$: $\sigma$-algebra indotta da $\Omega$ si ottiene per chiusura rispetto a:
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Unione\|#Unione]]: Dati $E_{1}, E_{2} \Rightarrow E_{1} \cup E_{2}$
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Intersezione\|#Intersezione]]: Dati Dati $E_{1}, E_{2} \Rightarrow E_{1} \cap E_{2}$
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Passaggio a complementare\|#Passaggio a complementare]]: Dato $E \Rightarrow E^{c}$ oppure $\overline E$

```ad-question

Un insieme chiuso è un insieme che contiene tutti i suoi punti di accumulazione. La chiusura di un insieme X è il più piccolo insieme chiuso che contiene X.
Un insieme chiuso può avere un numero finito di elementi? $\mathcal{A}$ ha sempre un numero infinito di elementi?

```

Chiusura rispetto a un'operazione e non rispetto a un altro insieme.

```ad-summary
title: Esempio: Dado

$
\mathcal{A} = \left\{ \Omega, \Omega^{c} = \emptyset, \{1\}, \{1\}^{c}, \{1,2\} = \{1\} \cup \{2\}, \{1\} = \Omega \smallsetminus \{2,3,4,5,6, ...\}  \right\}
$


```

### Assiomi

```ad-Teo
title: Assiomi probabilità

**A.1**: Gli eventi sono sottoinsiemi di $\Omega$ e formano $\mathcal{A}$

**A.2**: $\forall A \in \mathcal{A}$ è associato un numero $P(A) \in [0,1]$

**A.3**: $\mathcal{P}(\Omega) = 1$

**A.4**: Se $A \cap B = \emptyset \Rightarrow \mathcal{P}(A \cup B) = \mathcal{P}(A) + \mathcal{P}(B)$

**A.5**: Se $\{ A_{n}\}_{n \in \mathbb{N}}$ è decrescente e $\lim\limits_{n \to \infty} A_{n} = \emptyset \Rightarrow \lim\limits_{n \to \infty} \mathcal{P}(A_{n}) = 0$

```

#Dubbio


</div></div>


## Evento

```ad-Definizione
title: Evento

Dato uno [[02. Misura e Probabilità#Spazio di probabilità|Spazio di probabilità]] $\Omega$ relativo ad un [[#Esperimento casuale]], un **evento** è sempre un sottoinsieme di $\Omega$.

Tuttavia:
- Se $\Omega$ è costituito da un numero finito o da un'infinità numerabile di punti campionari, è evento ogni sottoinsieme $A$ di $\Omega$
- Se invece $\Omega$ è costituito da un'infinità non numerabile di punti non tutti i possibili sottoinsiemi di $\Omega$ ma soltanto i cosiddetti *sottoinsiemi ammissibili* di $\Omega$.
```

## Variabile casuale

```ad-Definizione
title: Variabili casuali o aleatoria

Si definisce **variabile casuale o aleatoria** una variabile $X$ associata ad una partizione di [[#Evento|eventi]] $E$ sulla quale è associata una distribuzione di probabilità $P$.

```

### Funzione di ripartizione

[[Università/2° anno/2° Semestre/Probabilità e statistica/Appunti/03. Variabili Aleatorie#Funzione di Ripartizione\|03. Variabili Aleatorie#Funzione di Ripartizione]]

```ad-Definizione
title: Funzione di ripartizione

La **funzione di ripartizione** o **Funzione delle Probabilità Comulate** (Cumulative Distribuction Function - CDF) è la funzione
$
P(x) = \text{prob}(X \le x)
$
verifica la seguente:
$
0 \le P(x) \le 1
$


```

### Funzione di densità probabilità

```ad-Definizione
title: Funzione di densità di probabilità
La **Funzione di densità di probabilità** o pdf (progability density function) è la funzione
$
p(x) = \frac{dP(x)}{dx}
$

```



## Statistica della popolazione

È utile definire degli indici prefissati per la grandezza che si sta osservando. 
Ci sono in generale 3 tipi di indici:
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Indice di posizione\|#Indice di posizione]]
	- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Valore atteso o media\|#Valore atteso o media]]
	- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Mediana\|#Mediana]]
	- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Moda\|#Moda]]
	- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Quantili\|#Quantili]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Indice di dispersione\|#Indice di dispersione]]
	- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Coefficiente di variazione\|#Coefficiente di variazione]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Indice di forma\|#Indice di forma]]
	- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Coefficiente di asimmetria\|#Coefficiente di asimmetria]]
	- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Coefficiente di Curtosi\|#Coefficiente di Curtosi]]

### Indice di posizione

Valutano la tendenza ad assumere certi valori

Gli indici di posizione si dividono in:
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Valore atteso o media\|#Valore atteso o media]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Mediana\|#Mediana]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Moda\|#Moda]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Quantili\|#Quantili]]

#### Valore atteso o media

```ad-Definizione
title: Media ($\mu$)
La media di una [[#Variabile casuale]] discreta è
$
\mu = E[z(x)] = \sum\limits_{k=-\infty}^{\infty} z(x_{k})p(x_{k})
$

```

#### Mediana

```ad-Definizione
title: Mediana ($x_{M}$)

La **mediana** è il valore $x_{M}$ di $X$ cui corrisponde i lvalore 0.5 della funzione di ripartizione. Quello ciè tale per cui:
$
P(x_{M}) = 0.5
$

```

La mediana divide la popolazione in due parti.

#### Moda

```ad-Definizione
title: Moda ($x_m$)

La **moda** è il valore $x_{m}$ di $X$ cui corrisponde il massimo valore della probabilità (se la variabile è discreta)
```

La moda è il valore della popolazione che ha più probabilità di "uscire".


#### Quantili

```ad-Definizione
title: Quantile

Il **quantile** di ordine $\alpha$ rappresenta il valore che divide il campione *ordinato* in due parti di ampiezza $\alpha$ e $(1-\alpha)$

```

Alcuni dei quantili più utilizzati sono
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Mediana\|#Mediana]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Quartile\|#Quartile]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Percentile\|#Percentile]]

##### Quartile

```ad-Definizione
title: Quartili

I **quartili** sono i [[#Quantili]] di ordine:
- $\alpha = \dfrac{1}{4}$
- $\alpha = \dfrac{2}{4}$ ([[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Mediana\|#Mediana]])
- $\alpha = \dfrac{3}{4}$


```

##### Percentile

```ad-Definizione
title: Percentili o centili

I **percentili** sono i [[#Quantili]] di ordine $\dfrac{m}{100}$ e dividono la popolazione in 100 parti uguali. Vengono anche detti centili

```


### Indice di dispersione

- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Coefficiente di variazione\|#Coefficiente di variazione]]

Per definirlo, occorre prima definire la [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Varianza\|#Varianza]] e la [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Deviazione Standard\|#Deviazione Standard]]
#### Varianza

```ad-Definizione
title: Varianza ($\sigma^{2}$)

La **varianza** di una [[#Variabile casuale]] discreta è
$
\sigma^{2} = V(X) = \sum\limits_{k=-\infty}^{\infty} (x_{k}-\mu)^{2}p(x_{k})
$
```

##### Deviazione Standard

```ad-Definizione
title: Deviazione standard ($\sigma$)

La deviazione standard è la radice quadrata della [[#Varianza]], $\sigma$

```


#### Coefficiente di variazione

```ad-Definizione
title: Coefficiente di variazione ($CV$)

Il **Coefficiente di variazione** fornisce una misura del grado di dispersione della [[#Variabile casuale]]:

$
VC = \frac{\sigma(x)}{\mu(x)}
$
essendo:
- $\sigma(x):$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Deviazione Standard\|#Deviazione Standard]]
- $\mu(x):$ [[#Valore atteso o media]]
```


### Indice di forma

Gli **indici di forma** sono 2:
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Coefficiente di asimmetria\|#Coefficiente di asimmetria]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Coefficiente di Curtosi\|#Coefficiente di Curtosi]]

#### Coefficiente di asimmetria

```ad-Definizione
title: Coefficiente di asimmetria ($\gamma(x)$)
Il **Coefficiente di asimmetria** o **skewness** fornisce l'asimmetria della distribuzione di probabilità rispetto alla distribuzione normale.
$
\gamma(x) = \frac{\mu_{3}(x)}{\sigma^{3}(x)}
$
dove:
- $\mu_{3}:$ [[03. Variabili Aleatorie#Moment|momento di ordine 3]]
- $\sigma(x):$ [[#Deviazione Standard]]
```

#### Coefficiente di Curtosi

```ad-Definizione
title: Coefficiente di curtosi ($CK$)

Il **coefficiente di curtosi** è il grado di appiattimento della [[#Funzione di densità probabilità]] rispetto alla [[#Distribuzione normale]].
$
CK = \frac{\mu_{4}(x)}{\mu_{2}^{2}(x)}
$
dove:
- $\mu_{4}:$ [[03. Variabili Aleatorie#Moment|momento di ordine 4]]
- $\mu_{2}^{2}(x)=\sigma^{4}(x):$ Quadrato della [[#Varianza]]
```


## Distribuzioni di probabilità

### Distribuzione normale o di Gauss


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/2-semestre/probabilita-e-statistica/appunti/03-variabili-aleatorie/#variabile-aleatoria-normale-o-gaussiana" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Variabile Aleatoria Normale o Gaussiana

> La Variabile Normale si ritrova in moltissime applicazioni pratiche. È stata introdotta inizialmente come approssimazione di una [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Variabile Aleatoria Binomiale\|#Variabile Aleatoria Binomiale]] per grandi valori del parametro $n$.
   È usata, ad esempio, come distribuzione:
> - Dell'altezza di una persona
> - Dell'errore nella misura di una quantità fisica



```ad-Definizione
title: VA Normale o Gaussiana (Continua): $X \sim N(\mu, \sigma^{2})$

$X \sim N(\mu, \sigma^{2})$ con $\mu \in \mathbb{R}, \sigma^{2} > 0$ 

La [[#Densità continua]] è
$
f_{X}(x) = \frac{1}{\sqrt{2 \pi \sigma^{2}}}e^{\frac{(x-\mu)^{2}}{2 \sigma^{2}}}
$
con $x \in \mathbb{R}$.

Il [[#Supporto]]:

$
\mathrm{Supp}(f_{X}) = \mathrm{Supp}(X) = \mathbb{R}
$

___

Per $\mu = 0$ e $\sigma^{2}=1$ si parla di **Normale Standard**: $X \sim N(0, 1)$

![GraficoDistribuzioneNormale 2.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/Probabilit%C3%A0%20e%20statistica/Appunti/allegati/GraficoDistribuzioneNormale%202.png)

```

Verifichiamo che $\mathcal{P}(X \in \mathbb{R}) = 1$

$
\begin{align}
\mathcal{P}(X \in \mathbb{R}) = \int_{\mathbb{R}} f_{X}(x)\, dx &= \int_{\mathbb{R}}  \frac{e^{- \frac{(x-\mu)^{2}}{2 \sigma^{2} }}}{\sqrt{2 \pi \sigma^{2}}} \, dx  =  \\
&= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \int_{- \infty}^{\infty} e^{- \frac{(x-\mu)^{2}}{2 \sigma^{2} }} \, dx  = \begin{bmatrix}
y = x-\mu \\
x = y+\mu \\
dx = dy
\end{bmatrix} =  \\
&= \frac{2}{\sqrt{2 \pi \sigma^{2}}} \int_{0}^{\infty} e^{- \frac{y^{2}}{2 \sigma^{2} }} \, dy  = \begin{bmatrix}
\omega = y^{2} \\
y = \omega^{\frac{1}{2}} \\
dy = \frac{1}{2}\omega^{- \frac{1}{2}}
\end{bmatrix} =   \\
&= \frac{\cancel{2}}{\sqrt{2 \pi \sigma^{2}}} \int_{0}^{\infty} e^{- \frac{\omega}{2 \sigma^{2} }} \frac{1}{\cancel{2}} \omega^{\frac{1}{2}-1}\, d \omega
\end{align}
$
Moltiplico e divido per la quantità
$
\frac{\Gamma\left( \frac{1}{2} \right)}{\left( \frac{1}{2 \sigma^{2}} \right)^{\frac{1}{2}}}
$
ottengo

$
\begin{align}
\mathcal{P}(X \in \mathbb{R}) &= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \frac{\Gamma\left( \frac{1}{2} \right)}{\left( \frac{1}{2 \sigma^{2}} \right)^{\frac{1}{2}}}\int_{0}^{\infty} \frac{\Gamma\left( \frac{1}{2} \right)}{\left( \frac{1}{2 \sigma^{2}} \right)^{\frac{1}{2}}} e^{- \frac{\omega}{2 \sigma^{2} }}  \omega^{\frac{1}{2}-1}\, d \omega
\end{align}
$
Noto che l'integrale è diventato quello per la probabilità $\mathcal{P}(X \in \mathbb{R})$ per $X \sim \mathrm{Gamma}\left( \frac{1}{2 \sigma^{2}}, \frac{1}{2} \right)$ che abbiamo già dimostrato essere uguale a 1 in [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Variabile Aleatoria Gamma\|#Variabile Aleatoria Gamma]].
Per cui rimane
$
\begin{align}
\mathcal{P}(X \in \mathbb{R}) &= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \frac{\Gamma\left( \frac{1}{2} \right)}{\left( \frac{1}{2 \sigma^{2}} \right)^{\frac{1}{2}}}
\end{align}
$
dove $\Gamma\left( \frac{1}{2} \right) = \sqrt(\pi)$ per le **proprietà** della [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Funzione Gamma\|#Funzione Gamma]]. Per cui
$
\begin{align}
\mathcal{P}(X \in \mathbb{R}) &= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \frac{\sqrt{\pi}}{\sqrt{\frac{1}{2 \sigma^{2}}}} =  \\
&= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \sqrt{2 \pi \sigma^{2}} = 1
\end{align}
$


#### Media VA Normale

```ad-Teo
title: Media VA Normale

$
E(X) = \mu 
$


```

#### Varianza VA Normale

```ad-Teo
title: Varianza VA Normale



$
\mathrm{Var}(X) = \sigma^{2}
$
___
**Dimostrazione**

$
\begin{align}

\mathrm{Var}(X) &= E(X-\mu)^{2} = \\

&= \int_\mathbb{R} (x-\mu)^{2}f_{X}(x) \, dx = \\

&= \int_\mathbb{R} (x-\mu)^{2}\frac{e^{\frac{(x-\mu)^{2}}{2 \sigma^{2}}}}{\sqrt{2 \pi \sigma^{2}}} \, dx = 
\begin{bmatrix} x-\mu = y \\ x = y+\mu \\ dx = dy \end{bmatrix} =\\

&= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \int_\mathbb{R}y^{2} e^{-\frac{y^{2}}{2\sigma^{2}}} \, dy = \begin{bmatrix} y^{2} = t \\ y = t^{\frac{1}{2}} \\ dy = \frac{1}{2}t^{\frac{1}{2}-1} dt \end{bmatrix} =\\

&= \frac{\not 2}{\sqrt{2 \pi \sigma^{2}}} \int_\mathbb{R}t e^{-\frac{t}{2\sigma^{2}}} \frac{1}{\not 2}t^{\frac{1}{2}-1}\, dt = \\

&= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \int_\mathbb{R}t^{\frac{1}{2}} e^{-\frac{t}{2\sigma^{2}}} \, dt = \begin{bmatrix} \frac{t}{2 \sigma^{2}} = l \\ t = 2 \sigma^{2}l \\ dt = 2 \sigma^{2} dl \end{bmatrix} = \\

&= \frac{1}{\sqrt{\not 2 \pi \not \sigma^{2}}} \int_\mathbb{R}(\not 2 \not \sigma^{2}l)^{\frac{1}{2}} e^{-l} 2 \sigma^{2}\, dl = \\

&= \frac{2 \sigma^{2}}{\sqrt{\pi}} \int_{0}^{\infty} l^{\frac{1}{2}}e^{-l} \, dl = \\

&= \frac{2 \sigma^{2}}{\sqrt{\pi}} \int_{0}^{\infty} l^{\frac{3}{2}-1} e^{-l} \, dl = \\

&= \frac{2 \sigma^{2}}{\sqrt{\pi}} \Gamma \left(\frac{3}{2} \right) = \frac{2 \sigma^{2}}{\sqrt{\pi}} \frac{1}{2} \sqrt{\pi} = \sigma^{2}
\end{align}
$
*c.v.d.*

```



</div></div>



| Simbolo       | Significato                |
| ------------- | -------------------------- |
| $\mu(x)$      | Media della popolazione    |
| $m(x)$        | Media campionaria          |
| $\sigma^2(x)$ | Varianza della popolazione |
| $s^2(x)$      | Varianza campionaria       |
Parametri della distribuzione:
- $\mu = m$
- $\sigma^{2} = s^{2}$

Notare che:
- La $p(x)$ è una curva simmetrica rispetto alla media $\mu(x)$
- La [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Mediana\|#Mediana]] coincide con la [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Valore atteso o media\|media]]
- La [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Moda\|#Moda]] coincide con [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Valore atteso o media\|media]] e [[#Mediana]]
- Cambiando la [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Valore atteso o media\|media]] $\mu(x)$ il grafico trasla ma non si deforma; cambiando la [[#Deviazione Standard]] $\sigma(x)$ il grafico si deforma ma non trasla

![Schermata 2024-05-02 alle 16.51.05.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Esercitazioni/allegati/allegati/Schermata%202024-05-02%20alle%2016.51.05.png)


### Distribuzione LogNormale (o di Galton)

```ad-Definizione
title: Distribuzione LogNormale o di Galton
$
p(x) = \frac{1}{x \sqrt{2 \pi} \sigma(y)} e^{\dfrac{(\ln(x) - \mu(y))^{2}}{2 \sigma(y)^{2}}} \quad 0 \le x \le \infty
$

![Schermata 2024-05-02 alle 16.58.52.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Esercitazioni/allegati/allegati/Schermata%202024-05-02%20alle%2016.58.52.png)

```

Funzione di ripartizione:

$$
P(x) = \frac{1}{\sqrt{2 \pi} \sigma(y)} \int_{-\infty}^{x} e^{\dfrac{(\ln(x) - \mu(y))^{2}}{2 \sigma(y)^{2}}}  \, dx 
$$

Siano:

| Simbolo       | Significato                |
| ------------- | -------------------------- |
| $\mu(x)$      | Media della popolazione    |
| $m(x)$        | Media campionaria          |
| $\sigma^2(x)$ | Varianza della popolazione |
| $s^2(x)$      | Varianza campionaria       |


Parametri della distribuzione:
- $y = \ln(x)$
- $\mu = m(y)$
- $\sigma^{2} = s^{2}(y)$

Notare che:
- La $p(x)$ è una curva *asimmetrica*, con asimmetria che cresce al crescere di $\sigma(x)$.





### Teoria dei valori estremi

### Distribuzione di Gumbel

### Distribuzione di Fréchet

### Distribuzione Gamma





