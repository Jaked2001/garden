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

Un **generatore reale di tensione** è dato dalla serie di un [[Generatore ideale di tensione]] e un [[Resistore\|Resistore]]. Esso genera una tensione $E_{s}$:
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


### Rendimento e adattamento del carico


Si consideri un [[Generatore reale di tensione\|Generatore reale di tensione]] $E$ con resistenza interna $R_{i}$ collegati a un carico (utilizzatore) rappresentabile da un [[Resistore\|Resistore]] $R_{u}$.

![08 - Reti in regime stazionario - ET 2024-06-18 13.28.54.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2013.28.54.excalidraw.png)


La corrente $I$ è data dalla relazione:
$
I = \frac{E}{R_{i}+R_{u}}
$
mentre la tensione $V$ ai capi del carico è:
$
V = IR_{u} = \frac{R_{u}}{R_{i}+R_{u}}E
$

Si vanno ora a calcolare le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza\|potenze]] in gioco.

La potenza [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] dal generatore **reale**, uguale alla potenza entrante al carico è
$
P = VI = \frac{R_{u}E^{2}}{(R_{i}+R_{u})^{2}}E
$

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule\|potenza dissipata per Effetto Joule]] dalla resistenza interna al generatore è:
$
P_{d} = R_{i}I^{2} = \frac{R_{i}E^{2}}{(R_{i}+R_{u})^{2}}
$
mentre la potenza generata dal generatore **ideale** è:
$
P_{g} = EI = I = \frac{E^{2}}{R_{i}+R_{u}}
$

Inoltre, per il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/05 - Generatori elettrici - ET#Bilancio di potenza di un generatore\|bilancio di potenza di un generatore]], la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] è scrivibile come:
$
P = P_{g}-P_{d}
$

#### Rendimento

```ad-Definizione
title: Rendimento del generatore reale di tensione

Si definisce **rendimento del [[Generatore reale di tensione\|Generatore reale di tensione]]** il rapporto tra [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] e potenza generata.
$
\eta = \frac{P}{P_{g}} = \frac{P_{g}-P_{d}}{P_{g}} = \frac{R_{u}}{R_{i}+R_{u}}
$

```

![Generatore reale di tensione 2024-06-18 13.46.13.excalidraw.png](/img/user/Excalidraw/Generatore%20reale%20di%20tensione%202024-06-18%2013.46.13.excalidraw.png)


#### Condizione di adattamento del carico

La condizione di adattamento del carico è la condizione in cui la Potenza trasferita al carico è massima (e quindi lo è anche il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Rendimento\|#Rendimento]]).

Calcolando la derivata della [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] e ponendola uguale a zero si può ricavare il suo massimo.
$
P = VI = \frac{R_{u}E^{2}}{(R_{i}+R_{u})^{2}}
$
Si deriva rispetto a $R_{u}$:
$
\begin{align}
\frac{dP}{dR_{u}} &= \frac{E^{2}}{(R_{i}+R_{u})^{2}} - \frac{2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} = \\
&= \frac{E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} \stackrel{!}{=} 0 
\end{align}
$
che quindi corrisponde a trovare:
$
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} = 0
$
che diventa
$
\begin{align}
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} &= 0 \\
R_{i}+R_{u}-2R_{u} &= 0 \\
R_{u} = R_{i}
\end{align}
$
```ad-Teo
title: Condizione di adattamento del carico

La condizione di adattamento del carico si ha quando la resistenza del carico è uguale alla resistenza interna al generatore
$
R_{u}= R_{i}
$
In tale condizione valgono:
$
\begin{align}
V &= \frac{V_{0}}{2} \\
I &= \frac{I_{cc}}{2} \\
\eta &= 0.5
\end{align}
$
```


La stessa relazione vale quando il carico $R_{u}$ è alimentato da una generica [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] lineare ai nodi A e B. Rappresentando la rete con il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Teorema di Thévenin\|teorema di Thévenin]] con $E_{eq} = E_{0}$ e $R_{eq} = R_{i}$, la condizione di adattamento è ancora $R_{u}= R_{i} =(R_{eq})$.

La potenza trasferita vale $P = \frac{V_{0}^{2}}{4R_{i}}$. Sul rendimento però non si può dire nulla in quanto il generatore equivalente non è significativo della rete reale dal punto di vista energetico.

</div></div>





### Partitore di tensione

```ad-Teo
title: Formula del partitore di tensione

Data una [[#Resistori in serie|serie di resistori]] agli estremi dei quali è presente una tensione $V_{s}$, la tensione si ripartisce su ognuno dei resistori in modo proporzionale.
$
V_{k} = R_{k}I_{k} = R_{k}I_{s} = R_{k} \frac{V_{s}}{R_{s}} = V_{s} \frac{R_{k}}{\sum R}
$

```


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

![08 - Reti in regime stazionario - ET 2024-06-18 14.30.32.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2014.30.32.excalidraw.png)


Per il $k$-esimo resistore si ha
$$
I_{k} = V_{k}G_{k}
$$
Per quanto detto sui [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Bipoli in parallelo\|#Bipoli in parallelo]], $V_{k}= V_{p}$ mentre applicando la [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]] al nodo A o al nodo B:
$$
I_{p} = \sum_{k=1}^{l}I_{k}
$$
Si può quindi scrivere:
$$
\begin{align}
I_{p} &= \sum_{k=1}^{l}I_{k} = \\
&= \sum_{k=1}^{l}V_{k}G_{k} = \\
&= V_{p}\sum_{k=1}^{l}G_{k} = V_{p} \sum_{k=1}^{l} \frac{1}{R_{k}}
\end{align}
$$
Per $l$ resistori in parallelo la resistenza equivalente è:
$$
R_{p} = \left(  \sum_{k=1}^{l} \frac{1}{R_{k}}  \right)^{-1}
$$

### Generatore reale di Corrente

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗
[[Generatore reale di corrente\|Generatore reale di corrente]]

### Partitore di corrente

```ad-Teo
title: Formula del partitore di corrente

Data un [[#Resistori in parallelo|parallelo di resistori]] agli estremi del quale scorre una corrente $I_{p}$, questa corrente ripartisce su ognuno dei resistori in modo proporzionale alla sua [[04 - Fenomeni di conduzione e resistori - ET#Conduttanza|conduttanza]].
$
I_{k} = G_{k}V_{k} = G_{k}V_{p} = G_{k} \frac{I_{p}}{G_{p}} = I_{p} \frac{G_{k}}{\sum G}
$

```


## Reti di resistori

![08 - Reti in regime stazionario - ET 2024-06-18 15.17.19.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2015.17.19.excalidraw.png)


Ci consideri una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] generica di soli [[Resistore\|resistori]] di cui sono accessibili solamente i terminali A e B. Si vuole determinare la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] della rete. Si osservi che la rete può essere vista a tutti gli effetti come un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Bipolo\|bipolo]].
Essendo la rete passiva (solo resistori), la caratteristica esterna è sempre del tipo:
$$
V = R_{i}I \qquad I = G_{i}V
$$
dove
- $R_{i}:$ **Resistenza interna** della rete alla porta AB
- $G_{i}:$ **Conduttanza interna** della rete alla porta AB

La rete, tra A e B, ha comportamento equivalente a quello di un bipolo resistore di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica\|resistenza]] equivalente (o conduttanza equivalente):
$$
R_{eq} = R_{i} \qquad G_{eq} = G_{i}
$$

### Configurazioni stella e triangolo

![08 - Reti in regime stazionario - ET 2024-06-18 15.26.13.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2015.26.13.excalidraw.png)


#### Configurazione a triangolo

![08 - Reti in regime stazionario - ET 2024-06-18 15.32.59.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2015.32.59.excalidraw.png)



#### Configurazione a stella

![08 - Reti in regime stazionario - ET 2024-06-18 15.33.22.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2015.33.22.excalidraw.png)



#### Trasformazione triangolo-stella

Si dimostra che una tripletta di [[Resistore\|resistori]] disposti in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a triangolo\|#Configurazione a triangolo]] può essere sostituita da una tripletta di resistori in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|#Configurazione a stella]] rispettando le relazioni:
$$
\begin{cases}
R_{A} &= \dfrac{R_{AB}R_{AC}}{R_{AB}+R_{BC}+R_{CA}} \\
R_{B} &= \dfrac{R_{AB}R_{BC}}{R_{AB}+R_{BC}+R_{CA}} \\
R_{C} &= \dfrac{R_{BC}R_{AC}}{R_{AB}+R_{BC}+R_{CA}}
\end{cases}
$$

```ad-Teo
title: Conversione triangolo-stella

Una tripletta di [[Resistore\|resistori]] uguali (di resistenza $R_{\triangle}$ disposti in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a triangolo\|#Configurazione a triangolo]] può essere sostituita da una tripletta di resistori in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|#Configurazione a stella]] (di resistenza $R_\star$) tale che:
$
R_{\star}= \frac{1}{3} R_{\triangle}
$

```



#### Trasformazione stella-triangolo

Si dimostra che una tripletta di [[Resistore\|resistori]] disposti in [[#Configurazione a stella]] può essere sostituita da una tripletta di resistori in [[#Configurazione a triangolo]] rispettando le relazioni:
$$
\begin{cases}
R_{AB} &= \dfrac{R_{A}R_{B}+R_{B}R_{C}+R_{C}R_{A}}{R_{C}} \\
R_{BC} &= \dfrac{R_{A}R_{B}+R_{B}R_{C}+R_{C}R_{A}}{R_{A}} \\
R_{CA} &= \dfrac{R_{A}R_{B}+R_{B}R_{C}+R_{C}R_{A}}{R_{B}}
\end{cases}
$$

```ad-Teo
title: Conversione stella-triangolo

Una tripletta di [[Resistore|resistori]] uguali (di resistenza $R_{\star}$ disposti in [[#Configurazione a stella]] può essere sostituita da una tripletta di resistori in [[#Configurazione a triangolo]] (di resistenza $R_\trinagle$) tale che:
$
R_{\triangle} = 3 R_{\star}
$


```


## Metodo di analisi delle reti lineari

[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|Risolvere una rete]] di $l$ [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipoli]] significa determinare tensioni e correnti su ciascuno dei bipoli e quindi $2l$ grandezze incognite. Saranno pertanto necessarie $2l$ equazioni indipendenti.

A partire dalle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Sistemi di equazioni topologiche\|equazioni topologiche]], è possibile ricavare $l$ equazioni in tutto:
- $p := n-1:$ LKC indipendenti
- $m := l-p:$ LKT indipendenti (maglie indipendenti)

Le mancanti $l$ equazioni sono costituite dalle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristiche esterne]] dei bipoli. In caso di generatori ideali di [[Generatore ideale di tensione\|tensione]] e [[Generatore ideale di corrente\|corrente]] e di [[Resistore|resistori]]:
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



```ad-example
title: Esempio

È dato il circuito in figura

![08 - Reti in regime stazionario - ET 2024-06-16 16.59.56.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-16%2016.59.56.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-16 16.59.56.excalidraw.md|🖋 Edit in Excalidraw]]%%

Sono presenti due generatori: $J$ e $E$ e due resistori: $R_{1}$ e $R_{2}$.

Si vogliono calcolare:
- $V_{2}$
- $I_{2}$
- [[03 - Introduzione allo studio delle reti elettriche - ET#Potenza assorbita|potenza assorbita]] da $R_{2}$: $P_{2}$

___

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

#UNI/ET/Domanda 

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

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ Correggere tutti i versi delle tensioni.
❗❗❗❗❗❗❗❗❗❗❗❗

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

### Teorema di Thévenin

#UNI/ET/Domanda 

Generatore di tensione equivalente.

```ad-Teo
title: Teorema di Thévenin

![08 - Reti in regime stazionario - ET 2024-06-17 19.46.01.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-17%2019.46.01.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-17 19.46.01.excalidraw.md|🖋 Edit in Excalidraw]]%%


Il comportamento di una qualunque [[03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica|rete]] di [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipoli]] lineari in termini di tensione $V$ e corrente $I$ ai terminali A e B è **equivalente** a quello di un bipolo costituito da un [[Generatore ideale di tensione]] $E_{eq}$ in serie con un [[Resistore]] di [[04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica|resistenza]] $R_{eq}$ aventi i seguenti valori
$
\begin{align}
E_{eq} &= V_{0} = \text{Tensione a vuoto tra A e B} \\
R_{eq} &= \frac{V_{0}}{I_{cc}} = \text{Resistenza equivalente}
\end{align}
$
dove:
- $I_{cc}:$ Corrente di [[06 - Bipoli e potenza elettrica - ET#Cortocircuito|cortocircuito]] ai terminali AB

La resistenza $R_{eq}$ coincide con la resistenza equivalente tra i nodi A e B quando tutti i generatori sono **spenti**.


___
**DIMOSTRAZIONE**
Pongo tra i nodi A e B un [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipolo]] qualsiasi C. In questa configurazione si avranno, tra i nodi, una tensione $V$ e una corrente $I$.

![08 - Reti in regime stazionario - ET 2024-06-18 10.52.30.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2010.52.30.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-18 10.52.30.excalidraw.md|🖋 Edit in Excalidraw]]%%

In base alle proprietà di sostituzione, il bipolo C può essere sostituito da un [[Generatore ideale di corrente]] avente corrente impressa $J = I$, senza modificare tensioni e correnti nel circuito.

Ora, la tensione $V$ può essere determinata, secondo il **principio di sovrapposizione degli effetti** come:
$
V = V'+V''
$
dove:
- $V' :$ Tensione tra A e B con $J=0$ e generatori interni accesi
- $V'':$ Tensione tra A e B con $J=I$ e generatori interni spenti
Nei due casi, risultano i circuiti nella figura sottostante:

![08 - Reti in regime stazionario - ET 2024-06-18 10.59.21.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2010.59.21.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-18 10.59.21.excalidraw.md|🖋 Edit in Excalidraw]]%%

$V'$ coincide con la tensione a vuoto tra i nodi A e B: $V_{0}$
$
V' \equiv V_{0}
$
Nel secondo caso invece, applicando la [[Legge di Kirchhoff delle Tensioni (LKT)|LKT]] in senso *orario* si ottiene:
$
V'' + R_{eq}I = V''+R_{eq}J = 0
$
Per cui
$
V'' = -R_{eq}J
$


In definitiva si ha che $V = V'+V''$ diventa:
$
V = V_{0}-R_{eq}I
$
che è proprio la [[Generatore reale di tensione#Caratteristica esterna|caratteristica esterna]] di un [[Generatore reale di tensione]], costituito da un [[Generatore ideale di tensione]] $E_{eq} = V_{0}$ e di un [[Resistore]] di resistenza $R_{eq}$ che è proprio l'enunciato del teorema.
*q.e.d.*

```

### Teorema di Norton

Generatore di corrente equivalente

```ad-Teo
title: Teorema di Norton

![08 - Reti in regime stazionario - ET 2024-06-18 11.33.07.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2011.33.07.excalidraw.png)
%%[[08 - Reti in regime stazionario - ET 2024-06-18 11.33.07.excalidraw.md|🖋 Edit in Excalidraw]]%%

Il comportamento di una qualunque [[03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica|rete]] di [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipoli]] lineari in termini di rtensione $V$ e corrente $I$ ai terminali A e B è equivalente a quello di un bipolo costituito da un [[Generatore ideale di corrente]] $J_{eq}$ in [[#Bipoli in parallelo|parallelo]] con una [[04 - Fenomeni di conduzione e resistori - ET#Conduttanza|conduttanza]] $G_{eq}$ aventi i seguenti valori:
$
\begin{align}
J_{eq} &= J_{cc} = \text{Corrente di cortocircuito tra A e B} \\
G_{eq} &= \frac{I_{cc}}{V_{0}} = \text{Conduttanza equivalente}
\end{align}
$
dove:
- $I_{cc}:$ Corrente ai terminali A e B quando sono collegati in [[06 - Bipoli e potenza elettrica - ET#Cortocircuito|cortocircuito]]
- $G_{eq}:$ Conduttanza equivalente della rete quando tutti i generatori sono spenti

```

## Rendimento ed adattamento del carico


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/generatore-reale-di-tensione/#rendimento-e-adattamento-del-carico" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Rendimento e adattamento del carico


Si consideri un [[Generatore reale di tensione]] $E$ con resistenza interna $R_{i}$ collegati a un carico (utilizzatore) rappresentabile da un [[Resistore]] $R_{u}$.

![08 - Reti in regime stazionario - ET 2024-06-18 13.28.54.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2013.28.54.excalidraw.png)


La corrente $I$ è data dalla relazione:
$
I = \frac{E}{R_{i}+R_{u}}
$
mentre la tensione $V$ ai capi del carico è:
$
V = IR_{u} = \frac{R_{u}}{R_{i}+R_{u}}E
$

Si vanno ora a calcolare le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza\|potenze]] in gioco.

La potenza [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] dal generatore **reale**, uguale alla potenza entrante al carico è
$
P = VI = \frac{R_{u}E^{2}}{(R_{i}+R_{u})^{2}}E
$

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule\|potenza dissipata per Effetto Joule]] dalla resistenza interna al generatore è:
$
P_{d} = R_{i}I^{2} = \frac{R_{i}E^{2}}{(R_{i}+R_{u})^{2}}
$
mentre la potenza generata dal generatore **ideale** è:
$
P_{g} = EI = I = \frac{E^{2}}{R_{i}+R_{u}}
$

Inoltre, per il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/05 - Generatori elettrici - ET#Bilancio di potenza di un generatore\|bilancio di potenza di un generatore]], la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] è scrivibile come:
$
P = P_{g}-P_{d}
$

#### Rendimento

```ad-Definizione
title: Rendimento del generatore reale di tensione

Si definisce **rendimento del [[Generatore reale di tensione]]** il rapporto tra [[03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata|potenza erogata]] e potenza generata.
$
\eta = \frac{P}{P_{g}} = \frac{P_{g}-P_{d}}{P_{g}} = \frac{R_{u}}{R_{i}+R_{u}}
$

```

![Generatore reale di tensione 2024-06-18 13.46.13.excalidraw.png](/img/user/Excalidraw/Generatore%20reale%20di%20tensione%202024-06-18%2013.46.13.excalidraw.png)


#### Condizione di adattamento del carico

La condizione di adattamento del carico è la condizione in cui la Potenza trasferita al carico è massima (e quindi lo è anche il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Rendimento\|#Rendimento]]).

Calcolando la derivata della [[03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata|potenza erogata]] e ponendola uguale a zero si può ricavare il suo massimo.
$
P = VI = \frac{R_{u}E^{2}}{(R_{i}+R_{u})^{2}}
$
Si deriva rispetto a $R_{u}$:
$
\begin{align}
\frac{dP}{dR_{u}} &= \frac{E^{2}}{(R_{i}+R_{u})^{2}} - \frac{2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} = \\
&= \frac{E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} \stackrel{!}{=} 0 
\end{align}
$
che quindi corrisponde a trovare:
$
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} = 0
$
che diventa
$
\begin{align}
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} &= 0 \\
R_{i}+R_{u}-2R_{u} &= 0 \\
R_{u} = R_{i}
\end{align}
$
```ad-Teo
title: Condizione di adattamento del carico

La condizione di adattamento del carico si ha quando la resistenza del carico è uguale alla resistenza interna al generatore
$
R_{u}= R_{i}
$
In tale condizione valgono:
$
\begin{align}
V &= \frac{V_{0}}{2} \\
I &= \frac{I_{cc}}{2} \\
\eta &= 0.5
\end{align}
$
```


La stessa relazione vale quando il carico $R_{u}$ è alimentato da una generica [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] lineare ai nodi A e B. Rappresentando la rete con il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Teorema di Thévenin\|teorema di Thévenin]] con $E_{eq} = E_{0}$ e $R_{eq} = R_{i}$, la condizione di adattamento è ancora $R_{u}= R_{i} =(R_{eq})$.

La potenza trasferita vale $P = \frac{V_{0}^{2}}{4R_{i}}$. Sul rendimento però non si può dire nulla in quanto il generatore equivalente non è significativo della rete reale dal punto di vista energetico.

</div></div>







