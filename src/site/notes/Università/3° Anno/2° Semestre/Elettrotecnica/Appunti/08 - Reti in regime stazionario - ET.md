---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/08-reti-in-regime-stazionario-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET\|08 - Reti in regime stazionario - ET]]

## Bipoli in serie

![08 - Reti in regime stazionario - ET 2024-06-15 17.54.36.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-15%2017.54.36.excalidraw.png)


```ad-Definizione
title: Bipoli in serie

2 [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Bipolo\|bipoli]] si dicono **in serie** quando si trovano su uno stesso [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Lato\|lato]].

```
 
 Essi sono attraversati dalla stessa corrente, infatti, immaginando la situazione nel diagramma, e applicando la [[Legge di Kirchhoff delle Correnti (LKT)\|Legge di Kirchhoff delle Correnti (LKT)]] al punto P si ottiene che:
$$
I_{s} = I_{1} = I_{2}
$$
Inoltre, applicando la [[Legge di Kirchhoff delle Tensioni (LKT)\|Legge di Kirchhoff delle Tensioni (LKT)]] nel verso indicato:
$$
V_{s}= V_{1}+ V_{2}
$$

### Resistori in serie

![08 - Reti in regime stazionario - ET 2024-06-15 18.16.25.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-15%2018.16.25.excalidraw.png)


La caratteristica del $k$-esimo [[Resistore\|Resistore]] è $V_{k}= R_{k}I_{k}$.

Applicando le [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]] e [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]]:
$$
\begin{align}
I_{s} &= I_{k} \\
V_{s} &= \sum\limits_{k=1}^{l}V_{k}
\end{align}
$$
Inserendo la caratteristica del resistore generico nella seconda:
$$
\begin{align}
V_{s} &= \sum\limits_{k=1}^{l} V_{k} = \\
&= \sum\limits_{k=1}^{l} R_{k}I_{k} =  \\
&= \left( \sum\limits_{k=1}^{l} R_{k} \right) I_{s}
\end{align}
$$

Da cui è evidente che
$$
R_{s} = \sum\limits_{k=1}^{l} R_{k}
$$
Pertanto, la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica\|resistenza]] equivalente di resistori in serie è data dalla somma delle singole resistenze.

### Generatore reale di Tensione


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/generatore-reale-di-tensione/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Generatore reale di tensione\|Generatore reale di tensione]]


```ad-Definizione
title: Generatore reale di tensione

Un **generatore reale di tensione** è dato dalla serie di un [[Generatore ideale di tensione]] e un [[Resistore]]. Esso genera una tensione $E_{s}$:
$
E_{s} = E - RI_{s}
$
```

![Generatore reale di tensione 2024-06-16 15.48.08.excalidraw.png](/img/user/Excalidraw/Generatore%20reale%20di%20tensione%202024-06-16%2015.48.08.excalidraw.png)


Applicando la [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]] in un qualsiasi punto del circuito mostrato si deve avere che:
$
I_{s} = I_{1} = - I_{2}
$
Pertanto, esprimendo anche la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] si ottiene:
$
\begin{align}
V_{s} &= V_{1} + V_{2} =  \\
&= E + V_{2} =  \\
&= E - RI_{s}
\end{align}
$

### Caratteristica esterna

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Generatore reale di tensione\|#Generatore reale di tensione]] è
$
V = E - RI_{s}
$
Sul piano $V-I$

![Generatore reale di tensione 2024-06-16 16.01.53.excalidraw.png](/img/user/Excalidraw/Generatore%20reale%20di%20tensione%202024-06-16%2016.01.53.excalidraw.png)


</div></div>




## Bipoli in parallelo

![08 - Reti in regime stazionario - ET 2024-06-16 16.14.50.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-16%2016.14.50.excalidraw.png)


```ad-Definizione
title: Bipoli in parallelo

Due [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipoli]] si dicono in **parallelo** se le coppie di terminali di entrambi i bipoli sono collegati alla stessa coppia di [[07 - Proprietà generali delle reti elettriche - ET#Nodo|nodi]] A e B.

```

Essendo i bipoli posti tra gli stessi nodi, e dovendo essere la ddp tra A e B unica e pari a $V_{p}$, si ha che:
$$
V_{p} = V_{1} = V_{2}
$$
Invece, applicando la [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]] si ottiene per le correnti:
$$
I_{p} = I_{1} + I_{2}
$$

```ad-attention
title: Attenzione
Non tutti i bipoli possono essere collegati in parallelo. Ad esempio, due [[Generatore ideale di tensione\|generatori ideali di tensione]] con f.e.m. $E_{1}$ e $E_{2}$ diverse tra loro non verificherebero la relazione vista sopra.

```


### Resistori in parallelo

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

$$
R_{p} = \frac{1}{\sum\limits_{k_{1}}^{l} \frac{1}{R_{k}}}
$$

### Generatore reale di Corrente

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗



## Reti di resistori

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗
### Configurazione a stella

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

### Configurazione a triangolo

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

## Metodo di analisi delle reti lineari

[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|Risolvere una rete]] di $l$ [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipoli]] significa determinare tensioni e correnti su ciascuno dei bipoli e quindi $2l$ grandezze incognite. Saranno pertanto necessarie $2l$ equazioni indipendenti.

A partire dalle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Sistemi di equazioni topologiche\|equazioni topologiche]], è possibile ricavare $l$ equazioni in tutto:
- $p := n-1:$ LKC indipendenti
- $m := l-p:$ LKT indipendenti (maglie indipendenti)

Le mancanti $l$ equazioni sono costituite dalle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristiche esterne]] dei bipoli. In caso di generatori ideali di [[Generatore ideale di tensione\|tensione]] e [[Generatore ideale di corrente\|corrente]] e di [[Resistore\|resistori]]:
$$
\begin{cases}
V = E & \text{Gen. ideale di tensione} \\
I = J & \text{Gen. ideale di corrente} \\
V - RI = 0 \qquad &\text{Resistori}
\end{cases}
$$
Pertanto, in una rete costituita esclusivamente da questi elementi (che per tale motivo è detta **rete lineare**), si può impostare un sistema della seguente forma:
$$
[A]
\begin{bmatrix}
V \\ I
\end{bmatrix}
=
\begin{bmatrix}
E \\ J
\end{bmatrix}
$$
Il quale può essere risolto invertendo la matrice $A$:
$$
\begin{bmatrix}
V \\ I
\end{bmatrix}
=
[A]^{-1}
\begin{bmatrix}
E \\ J
\end{bmatrix}
$$
Questo metodo consiste di fatto nell'invertire matrici molto grandi e risulta quindi poco pratico per circuiti poco più complessi di circuiti elementari. Esistono comunque dei metodi più efficienti che fanno comunque riferimento ai passaggi appena descritti:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Metodo di sovrapposizione degli effetti\|#Metodo di sovrapposizione degli effetti]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Metodo delle maglie\|#Metodo delle maglie]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Metodo dei nodi\|#Metodo dei nodi]]

### Metodo di analisi generale

### Metodo di sovrapposizione degli effetti

A partire dalle equazioni enunciate prima
$$
\begin{bmatrix}
V \\ I
\end{bmatrix}
=
[A]^{-1}
\begin{bmatrix}
E \\ J
\end{bmatrix}
$$
si può affermare che la tensione $V$ o la corrente $I$ su ciascuno dei lati è esprimibile come combinazione lineare delle tensioni dei [[Generatore ideale di tensione\|generatori ideali]] $E$ e delle correnti dei [[Generatore ideale di corrente\|generatori ideali]] $J$.

Pertanto, si può scrivere che, in presenza di
- $r$ [[Generatore ideale di tensione|generatori ideali di tensione]] - $(E_{1}, E_{2},..., E_{r})$
- $s$ [[Generatore ideale di corrente\|generatori ideali di corrente]] - $(J_{1}, J_{2},..., J_{s})$
per il lato $h$-esimo:
$$
\begin{cases}
V_{h} = \sum\limits_{k=1}^{r} \alpha_{hk}E_{k} + \sum\limits_{k=1}^{s} R_{hk}J_{k} \\
I_{h} = \sum\limits_{k=1}^{r} G_{hk}E_{k}  + \sum\limits_{k=1}^{s} \beta_{hk}J_{k}
\end{cases}
$$
Essendo il tutto un insieme di relazioni lineari, è evidente che si può applicare il principio di sovrapposizione degli effetti.

Il sistema completo può quindi essere risolto nel seguente modo:
1. Calcolare la tensione (o la corrente) sul lato considerato, ottenuta attivando **un solo** generatore ($E$ o $J$), con tutti gli altri generatori spenti ($E = 0, J=0$)
2. Ripetere il calcolo per tutti i generatori, attivandone uno per volta
3. Sommare gli effetti

```ad-note
title: Osservazione
- [[Generatore ideale di tensione]] **spento**: $V = E = 0$ coincide con [[06 - Bipoli e potenza elettrica - ET#Cortocircuito|cortocircuito]]
- [[Generatore ideale di corrente]] **spento**: $I = J = 0$ coincide con [[06 - Bipoli e potenza elettrica - ET#Circuito aperto|circuito aperto]]

```


**ESEMPIO**

È dato il circuito in figura

![08 - Reti in regime stazionario - ET 2024-06-16 16.59.56.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-16%2016.59.56.excalidraw.png)


Sono presenti due generatori: $J$ e $E$ e due resistori: $R_{1}$ e $R_{2}$.

Si vogliono calcolare:
- $V_{2}$
- $I_{2}$
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza assorbita\|potenza assorbita]] da $R_{2}$: $P_{2}$

___

```ad-example
title: Esempio

Per applicare il [[#Metodo di sovrapposizione degli effetti]] dobbiamo spegnere alternativamente i due generatori. Dovremo pertanto risolvere i seguenti due circuiti:

![08 - Reti in regime stazionario - ET 2024-06-16 17.22.00.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-16%2017.22.00.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-16 17.22.00.excalidraw.md|🖋 Edit in Excalidraw]]%%

**a)**
Spento il generatore di corrente, si nota che rimane una sola maglia costituita da 2 resistori in serie e il generatore di tensione.
$
R_{s} = R_{1} + R_{2}
$
A questo punto, la corrente che attraversa $R_{2}$, $I_{2E}$, può essere calcolata con la [[I Legge di Ohm]]:
$
I_{2E} = \frac{E}{R_{s}}
$
La tensione ai capi di $R_{2}$ invece sarà:
$
V_{2E} = I_{2E} R_{2} = \frac{R_{2}}{R_{s}} E
$

**b)**
Spento il generatore di tensione, rimane la configurazione b) con i 2 resistori in parallelo. La resistenza equivalente è data da:
$
R_{p} = \frac{R_{1} R_{2}}{R_{1} + R_{2}}
$
Per via del [[#Partitore di corrente]]
$
I_{2J} = \frac{R_{1}}{R_{1}+R_{2}}J
$
Inoltre, la tensione ai capi di $R_{2}$ si può ottenere applicando la [[I Legge di Ohm]]
$
V_{2J} = R_{p}J
$

**Applicazione del principio di sovrapposizione degli effetti**
Sommando gli effetti si può dire che:
$
\begin{align}
I_{2} &= I_{2E} + I_{2J} = \\
&= \frac{E}{R_{1} + R_{2}} + \frac{R_{1}}{R_{1}+R_{2}}J = \\
&= \frac{E + R_{1}J}{R_{1}+R_{2}}
\end{align}
$
e, per quanto riguarda la tensione $V_{2}$
$
\begin{align}
V_{2} &= V_{2E} + V_{2J} = \\
&= \frac{R_{2}}{R_{1} + R_{2}} E + \frac{R_{1} R_{2}}{R_{1} + R_{2}} J = \\
&= \frac{R_{2} (E+ R_{1}J)}{R_{1} + R_{2}}
\end{align}
$
Infine si può calcolare la [[03 - Introduzione allo studio delle reti elettriche - ET#Potenza assorbita|potenza assorbita]] dal resistore:
$
P_{2} = V_{2}I_{2} = \frac{R_{2} (E+ R_{1}J)}{R_{1} + R_{2}} \cdot\frac{E + R_{1}J}{R_{1}+R_{2}}
$
Si ricorda che la potenza assorbita da un resistore, in [[03 - Introduzione allo studio delle reti elettriche - ET#Convenzione del generatore]] è pari alla [[04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule|potenza dissipata per effetto Joule]]:
$
P_{2} = R_{2} I_{2}^{2} = R_{2} \left(\frac{E + R_{1}J}{R_{1}+R_{2}}\right)^{2}
$
```


### Metodo delle maglie

Il metodo delle maglie consente di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|risolvere la rete]] riducendo il numero di equazioni necessarie. Fa uso delle cosiddette **correnti di maglia**.

Scelto un sistema di $m = l-p$ maglie, ad ogni maglia si associa una *corrente virtuale*, $I_{m}$, che percorre tutti i lati della maglia.

Solitamente, è conveniente scegliere le correnti di maglia tutte nello stesso verso (ad esempio percorrendo le maglie in senso orario).

A questo punto, la corrente di ogni lato sarà:
- La corrente di maglia, per i lati esterni della rete
- La differenza delle correnti di maglia che incidono sullo stesso lato, se questo è comune a due maglie
	- Se ad esempio il lato $h$-esimo appartiene alle maglie $M_{r}$ e $M_{s}$ e la sua corrente di lato $I_{h}$ ha verso concorde con $I_{r}$ si avrà $I_{h} = I_{m_r}-I_{m_s}$

Qualora ciascuno dei bipoli sia un [[Generatore di tensione\|Generatore di tensione]] descritto da una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del tipo
$$
V_{h} = E_{h} - R_{h}I_{h}
$$
allora, tenendo conto delle trasformazioni con correnti di lato, si può scrivere:
$$
V_{h} = E_{h} - R_{h}(I_{m_r}-I_{m_s})
$$
Se si va a scrivere la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] per ognuna delle $m$ maglie scelte, si ottengono $m$ equazioni della forma:
$$
\begin{align}
\sum_{h} V_{h} &= \sum_{h} E_{h} - \sum_{h} R_{h}I_{h} = 0\\
&= \sum_{h} E_{h} - \sum_{h} R_{h}(I_{m_{r}} - I_{m_{s}}) = 0
\end{align}
$$
Prendendo ognuna delle maglie, si definiscono:
- $E_{m_{h}}:$ somma algebrica di tutte le tensioni dei [[Generatore di tensione\|generatori di tensione]] della maglia $h$
- $I_{m_{h}}:$ Corrente di maglia, della maglia $h$
- $R_{m_{hh}}:$ Somma di tutte le resistenze della maglia $h$ - **autoresistenze di maglia**
- $R_{m_{hr}}:$ Resistenza del lato comune alla maglia $h$ e alla maglia $r$ - **mutue resistenze**

Con questi parametri, si può impostare il sistema:
$$
\begin{cases}
E_{m_{1}} &= R_{m_{1}}I_{m_{1}} - \sum\limits_{r=1, r\ne1}^{m} R_{m_{1}} I_{m_{r}} \\
E_{m_{2}} &= R_{m_{2}}I_{m_{2}} - \sum\limits_{r=1,r\ne2}^{m} R_{m_{2}} I_{m_{r}} \\ &\vdots \\
E_{m_{m}} &= R_{m_{m}}I_{m_{m}} - \sum\limits_{r=1,r\ne m}^{m} R_{m_{m}} I_{m_{r}} 
\end{cases}
$$

Questo sistema si traduce in un sistema matriciale $m\times m$ nella seguente forma:
$$
\boldsymbol{[E]} = \boldsymbol{[A]}\boldsymbol{[I_{m}]}
$$



```ad-example
title: Esempio


![08 - Reti in regime stazionario - ET 2024-06-17 12.57.17.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-17%2012.57.17.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-17 12.57.17.excalidraw.md|🖋 Edit in Excalidraw]]%%

Si vuole risolvere la rete nel diagramma, considerando note le fem dei generatori e i valori delle resistenze.

Impostando il sistema mostrato sopra si ottiene:
$
\begin{cases}
E_{1} - E_{6} &= (R_{1}+R_{2})I_{m_{1}} - R_{2}I_{m_{2}} \\
E_{3} - E_{4} &= - R_{2}I_{m_{1}} + (R_{2}+R_{3}+R_{4})I_{m_{2}} - R_{4}I_{m_{3}} \\
E_{4}+E_{5} &= -R_{4}I_{m_{2}} + R_{4}I_{m_{3}}
\end{cases}
$
Il sistema può essere scritto in forma matriciale come:
$
\begin{bmatrix}
E_{1}-E_{6} \\ E_{3}-E_{4} \\ E_{4}+E_{5}
\end{bmatrix}
=
\begin{bmatrix}
(R_{1} + R_{2}) & -R_{2} & 0 \\
-R_{2} & (R_{2}+R_{3}+R_{4}) & -R_{4} \\
0 & -R_{4} & R_{4}
\end{bmatrix}
\begin{bmatrix}
I_{m_{1}} \\ I_{m_{2}} \\ I_{m_{3}}
\end{bmatrix}
$
Si osservi che si sono usate le correnti di maglia, che si legano alle correnti di lato secondo le seguenti relazioni:
$
\begin{align}
I_{1} &= I_{m_{1}} & I_{4} &= -I_{m_{2}} + I_{m_{3}}\\
I_{2} &= -I_{m_{1}} + I_{m_{2}} &\qquad I_{5} &= I_{m_{3}}\\
I_{3} &= I_{m_{2}} & I_{6} &= -I_{m_{1}}\\
\end{align}
$
Invertendo la matrice delle resistenze, si possono ricavare le correnti di maglia e da queste risalire alle correnti di lato.
```


### Metodo dei nodi

#UNI/ET/Domanda 

Il **metodo dei nodi**, o metodo dei potenziali nodali, consente di ridurre il numero di equazioni necessarie a [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|risolvere la rete]] a $p = n-1$.

Come primo step, si sceglie - arbitrariamente - un nodo cui associare potenziale nullo. Sia questo il nodo $n$, si avrà $U_{n} =0$. Rispetto a questo nodo si considerano i potenziali di tutti gli altri nodi della rete.

Le tensioni di ciascun lato risulteranno pertanto esprimibili come differenze di potenziale. Ad esempio, la tensione del [[07 - Proprietà generali delle reti elettriche - ET#Lato|lato]] $h$-esimo, tra i nodi a potenziale $U_{r}$ e $U_{s}$ sarà
$$
V_{h} = V_{rs} = U_{r} - U_{s}
$$
Qualora ciascuno dei bipoli sia un [[Generatore di corrente\|Generatore di corrente]] descritto da una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del tipo
$$
\begin{align}
I_{h} &= J_{h} - G_{h}V_{h} = \\
&= J_{h} - G_{h}(U_{r} - U_{s})
\end{align}
$$
Si avrà quindi, per ognuno degli $n-1$ nodi, che la [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]] si presenta nella forma:
$$
\sum_{h} I_{h} = \sum_{h} J_{h} - \sum_{h} G_{h}(U_{r}-U_{s}) = 0
$$
Quindi, si può scrivere un sistema di $n-1$ equazioni come segue:
$$
\begin{cases}
J_{1} &= G_{11}U_{1} - \sum\limits_{r = 1, r\ne 1}^{p} G_{1r}U_{r} \\
J_{2} &= G_{22}U_{2} - \sum\limits_{r = 1, r\ne 2}^{p} G_{2r}U_{r} \\
&\vdots \\
J_{p} &= G_{pp}U_{p} - \sum\limits_{r = 1, r\ne p}^{p} G_{pr}U_{r}
\end{cases}
$$
dove:
- $G_{ss}:$ Somma delle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Conduttanza\|conduttanze]] dei lati che toccano il nodo $s$ - **autoconduttanze**
- $G_{sr}:$ Somma delle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Conduttanza\|conduttanze]] dei lati compresi tra il nodo $s$ e il nodo $r$ - **mutue conduttanze**
- $J_{s}:$ Somma algebrica delle correnti dei [[Generatore di corrente\|generatori di corrente]] collegati al nodo $s$

- [!] Le correnti sono prese con segno **positivo** se dirette **dentro** il nodo


```ad-example
title: Esempio

![08 - Reti in regime stazionario - ET 2024-06-17 18.41.44.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-17%2018.41.44.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-17 18.41.44.excalidraw.md|🖋 Edit in Excalidraw]]%%

Dato il circuito in figura, [[07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete|risolvere la rete]] supponendo di conoscere tutte le $J$ e le $R$.

Seguendo le indicazioni sopra, si costruisce il sistema di $p = n-1$ equazioni, supponendo di assegnare potenziale nullo al nodo D ($U_{D} = 0$):
$
\begin{align}
A: \\ B: \\ C:
\end{align}
\quad
\begin{cases}
J_{1} + J_{5} + J_{6} = (G_{1} + G_{5})U_{D} - G_{1}U_{B} - G_{5}U_{C} \\
-J_{1}+J_{3} = -G_{1}U_{A} + (G_{1}+G_{2}+G_{3})U_{B} - G_{3}U_{C} \\
-J_{3}-J_{4}-J_{5} = -G_{5}U_{A} - G_{3}U_{B} + (G_{3}+G_{4}+G_{5})
\end{cases}
$
Il sistema può essere riscritto in forma matriciale come:
$
\begin{bmatrix}
J_{1} \\ J_{2} \\ J_{3}
\end{bmatrix}
=
\begin{bmatrix}
(G_{1}+G_{5}) & -G_{1} & - G_{5} \\
-G_{1} & (G_{1}+G_{2}+G_{3}) & -G_{3} \\
-G_{5} & -G_{3} & (G_{3}+G_{4}+G_{5})
\end{bmatrix}
\begin{bmatrix}
U_{A} \\ U_{B} \\ U_{C}
\end{bmatrix}
$
Invertendo la matrice delle conduttanze è possibile risolvere il sistema e trovare i potenziali nodali. Da questi, sfruttando le seguenti relazioni, è possibile ricavare le tensioni dei vari bipoli del sistema:
$
\begin{align}
V_{1} &= U_{A}-U_{B} &\quad V_{4} &= -U_{C} \\
V_{2} &= -U_{B} & V_{5} &= U_{C}-U_{A} \\
V_{3} &= V_{B}-V_{C} & V_{6} &= U_{A}
\end{align}
$

```


## Proprietà delle reti lineari

