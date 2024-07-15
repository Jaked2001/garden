---
{"dg-publish":true,"permalink":"/generatore-reale-di-tensione/"}
---

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
$$
I_{s} = I_{1} = - I_{2}
$$
Pertanto, esprimendo anche la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] si ottiene:
$$
\begin{align}
V_{s} &= V_{1} + V_{2} =  \\
&= E + V_{2} =  \\
&= E - RI_{s}
\end{align}
$$

### Caratteristica esterna

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del [[Generatore reale di tensione#Generatore reale di tensione\|#Generatore reale di tensione]] è
$$
V = E - RI_{s}
$$
Sul piano $V-I$

![Generatore reale di tensione 2024-06-16 16.01.53.excalidraw.png](/img/user/Excalidraw/Generatore%20reale%20di%20tensione%202024-06-16%2016.01.53.excalidraw.png)


### Rendimento e adattamento del carico

#UNI/ET/Domanda 

Si consideri un [[Generatore reale di tensione\|Generatore reale di tensione]] $E$ con resistenza interna $R_{i}$ collegati a un carico (utilizzatore) rappresentabile da un [[Resistore]] $R_{u}$.

![08 - Reti in regime stazionario - ET 2024-06-18 13.28.54.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-18%2013.28.54.excalidraw.png)


La corrente $I$ è data dalla relazione:
$$
I = \frac{E}{R_{i}+R_{u}}
$$
mentre la tensione $V$ ai capi del carico è:
$$
V = IR_{u} = \frac{R_{u}}{R_{i}+R_{u}}E
$$

Si vanno ora a calcolare le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza\|potenze]] in gioco.

La potenza [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] dal generatore **reale**, uguale alla potenza entrante al carico è
$$
P = VI = \frac{R_{u}E^{2}}{(R_{i}+R_{u})^{2}}
$$

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule\|potenza dissipata per Effetto Joule]] dalla resistenza interna al generatore è:
$$
P_{d} = R_{i}I^{2} = \frac{R_{i}E^{2}}{(R_{i}+R_{u})^{2}}
$$
mentre la potenza generata dal generatore **ideale** è:
$$
P_{g} = EI = I = \frac{E^{2}}{R_{i}+R_{u}}
$$

Inoltre, per il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/05 - Generatori elettrici - ET#Bilancio di potenza di un generatore\|bilancio di potenza di un generatore]], la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] è scrivibile come:
$$
P = P_{g}-P_{d}
$$

#### Rendimento

```ad-Definizione
title: Rendimento del generatore reale di tensione

Si definisce **rendimento del [[Generatore reale di tensione]]** il rapporto tra [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata\|potenza erogata]] e potenza generata.
$
\eta = \frac{P}{P_{g}} = \frac{P_{g}-P_{d}}{P_{g}} = \frac{R_{u}}{R_{i}+R_{u}}
$

```

![Generatore reale di tensione 2024-06-18 13.46.13.excalidraw.png](/img/user/Excalidraw/Generatore%20reale%20di%20tensione%202024-06-18%2013.46.13.excalidraw.png)


#### Condizione di adattamento del carico

La condizione di adattamento del carico è la condizione in cui la Potenza trasferita al carico è massima (e quindi lo è anche il [[Generatore reale di tensione#Rendimento\|#Rendimento]]).

Calcolando la derivata della [[03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata|potenza erogata]] e ponendola uguale a zero si può ricavare il suo massimo.
$$
P = VI = \frac{R_{u}E^{2}}{(R_{i}+R_{u})^{2}}
$$
Si deriva rispetto a $R_{u}$:
$$
\begin{align}
\frac{dP}{dR_{u}} &= \frac{E^{2}}{(R_{i}+R_{u})^{2}} - \frac{2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} = \\
&= \frac{E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} \stackrel{!}{=} 0 
\end{align}
$$
che quindi corrisponde a trovare:
$$
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} = 0
$$
che diventa
$$
\begin{align}
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} &= 0 \\
R_{i}+R_{u}-2R_{u} &= 0 \\
R_{u} = R_{i}
\end{align}
$$
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

