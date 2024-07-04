---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/00-introduzione-elettrotecnica/"}
---


# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica\|00 - Introduzione elettrotecnica]]

## Dipolo

Il dipolo è un componente accessibile da due poli
I dipoli sono lineari

Un esempio di dipolo è il [[Resistore\|Resistore]].


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/resistore/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Resistore\|Resistore]]

![Resistore 2024-02-26 18.37.25.excalidraw.png](/img/user/Excalidraw/Resistore%202024-02-26%2018.37.25.excalidraw.png)


```ad-Definizione
title: Resistore

Un resistore è un **dipolo passivo**. È un componente elettrico dotato di due morsetti costruito di materiali conduttori e privo di f.e.m.

È caratterizzato dalle seguenti relazioni.
$
V = RI \qquad I = GV
$
dove:
- $V:$ Tensione ai capi del resistore
- $R:$ [[04 - Fenomeni di conduzione e resistori#Resistenza elettrica|Resistenza elettrica]] del resistore
- $I:$ Corrente che transita per il resistore
- $G:$ [[04 - Fenomeni di conduzione e resistori#Conduttanza|Conduttanza]] del resistore

```

Se $R$ e $G$ sono costanti al variare di tensione e corrente allora si dice che il resistore è **ideale** o **lineare**.

Esso ostacola la corrente e dissipa potenza per [[Effetto Joule\|Effetto Joule]]

La potenza dissipata è

$
P = RI^{2} \qquad \rm [W] = [\Omega][A^{2}]
$


### Caratteristica esterna

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del resistore è
$
V = RI
$
rappresentata graficamente nella figura sottostante:

![Resistore 2024-06-14 17.26.23.excalidraw.png](/img/user/Excalidraw/Resistore%202024-06-14%2017.26.23.excalidraw.png)


## Regime sinusoidale

![Resistore sinusoidale.excalidraw.png](/img/user/Excalidraw/Resistore%20sinusoidale.excalidraw.png)


```ad-Definizione
title: 

In regime sinusoidale il [[#Resistore]] di [[04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica|resistenza]] $R$ ([[03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore|convenzionato da utilizzatore]]) rispetta, in qualunque istante, la seguente relazione:
$
v(t) = Ri(t)
$

```

In regime sinusoidale significa che la corrente è descritta da una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|funzione sinusoidale]] della forma:
$
i(t) = \sqrt{2}I\sin(\omega t+\beta)
$
pertanto la tensione sarà:
$
v(t) = \sqrt{2} RI\sin(\omega t+\beta) = \sqrt{2}V\sin(\omega t+\alpha)
$
Valgono pertanto le relazioni:
- $\dfrac{V}{I} = R$ tra [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valori efficaci]]
- $\alpha=\beta$ e quindi [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|sfasamento]] $\varphi=0$

Nel [[Resistore#Regime sinusoidale\|resistore in regime sinusoidale]] tensione e corrente sono in fase quindi massimi, minimi e zeri sono negli stessi punti.

![Resistore 2024-06-20 12.10.16.excalidraw.png](/img/user/Excalidraw/Resistore%202024-06-20%2012.10.16.excalidraw.png)


La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] del resistore è
$
P = VI \ge 0
$
ed è sempre **NON** negativa (il resistore non può erogare potenza). La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza istantanea]] ha valore massimo $V_{M}I_{M} = 2VI$.

Essendo $\varphi=0$ il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|fattore di potenza]] $\cos(\varphi)=1$. Quindi, tutta la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza assorbita\|potenza assorbita]] coincide con la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|potenza apparente]] $A$. La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|potenza reattiva]] $Q = 0$.
$
A = \sqrt{P^{2}+Q^{2}} = P
$
quindi
$
P = A = VI = RI^{2} \qquad Q = 0
$

___

Il resistore in regime sinusoidale può essere descritto anche facendo riferimento alle grandezze [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriali]].
$
\begin{align}
i(t) &\Longrightarrow \overline{I} = Ie^{j\beta} \\
v(t) &\Longrightarrow \overline{V} = Ve^{j\alpha}
\end{align}
$
Il rapporto tra i fasori vale:
$
\frac{\overline{V}}{\overline{I}} = \frac{V}{I}e^{j\varphi} = R
$
Essendo $\varphi=0$ poiché tensione e corrente risultano in fase.



</div></div>


## Leggi di Ohm


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/i-legge-di-ohm/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[I Legge di Ohm\|I Legge di Ohm]]

```ad-Teo
title: I Legge di Ohm

La **legge di Ohm** è una formula matematica che descrive la relazione di proporzionalità diretta tra la tensione elettrica $V$ (misurata in [[Volt]]) applicata ai capi di un conduttore elettrico, e la [[Corrente elettrica]] $I$ (espressa in [[Ampere]] che scorre nel conduttore stesso; essa deriva da evidenze empiriche ed è valida per molti materiali conduttori
$
V = RI \qquad \rm [\Omega]
$

```

Si tratta di fatto di una relazione **lineare** ammesso di supporre che la resistenza $R$ sia **costante**. Questa è un'ipotesi che si basa sul considerare la [[Resistività\|Resistività]] introdotta nella [[II Legge di Ohm\|II Legge di Ohm]] anch'essa costante

La I Legge di Ohm può anche essere scritta nella forma:
$
I = \frac{1}{R}V = GV
$
dove G prende il nome di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Conduttanza\|conduttanza]].

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/ii-legge-di-ohm/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[II Legge di Ohm\|II Legge di Ohm]]

```ad-Teo
title: Teorema

La **seconda legge di Ohm** lega la resistenza alle dimensioni del conduttore (sezione $S$ e lunghezza $l$).
$
R = \rho \frac{l}{S}
$
dove:
- $\rho = \rm [\Omega\cdot m]$ - [[Resistività\|Resistività]]
- $l$ - Lunghezza del conduttore
- $S$ - Sezione del conduttore

```

Tendiamo a supporre la [[Resistività\|Resistività]] costante. Questo permette di affermare che anche la [[Resistenza\|Resistenza]] è costante.

In realtà la resistività dipende anche dalla temperatura:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/resistivita/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Resistività\|Resistività]]

```ad-Definizione
title: Resistività ($\rho$)

La resistività è una caratteristica dei materiali conduttori elettrici che misura la loro capacità di condurre, o meglio, di ostacolare il passaggio di corrente.

```

## Dipendenza della resistività dalla temperatura

```ad-Teo
title: Dipendenza di $\rho$ dalla temperatura
La [[resistività]] di un conduttore $\rho$ è funzione della temperatura del conduttore stesso. In prima approssimazione si può considerare la relazione come lineare:
$
\rho(T) = \rho_{0}[1+\alpha(T-T_{0})]
$
```





</div></div>


</div></div>


## Circuito elettrico


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/circuito-elettrico/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Circuito Elettrico\|Circuito Elettrico]]

```ad-Definizione
title: Circuito Elettrico

Un **circuito elettrico** è un modello di un sistema elettrico reale

```



</div></div>



## Sistema a parametri concentrati

```ad-Definizione
title: Sistema a parametri concentrati

Nelle **applicazioni pratiche** si tende a supporre che il [[#Dipolo]] sia concentrato in un unico punto

```

Supponiamo di avere un segnale elettromagnetico fatto come in figura sotto:

![00 - Introduzione elettrotecnica 2024-02-26 19.02.19.excalidraw.png](/img/user/Excalidraw/00%20-%20Introduzione%20elettrotecnica%202024-02-26%2019.02.19.excalidraw.png)


Sia $c$ la [[Velocità della luce\|Velocità della luce]], $\lambda$ la [[Lunghezza d'onda\|Lunghezza d'onda]], $T$ il periodo e $f$ la frequenza, si può scrivere:
$$
c = \frac{\lambda}{T} = \lambda f
$$
essendo
$$
f = \frac{1}{T}
$$
A questo punto si può dire che, se la lunghezza d'onda è molto maggiore della **dimensione caratteristica** del sistema che si sta considerando, si può effettivamente affermare di avere a che fare con un sistema a parametri concentrati.

Il potenziale, verificata questa ipotesi, varierà di una quantità impercettibile all'interno del sistema considerato.

```ad-example
title: Esempi

**SISTEMA ELETTRICO in un AULA**
Consideriamo il sistema elettrico di un'aula universitaria. La corrente nell'aula è di tipo alternata con frequenza $f = 50 \, \rm Hz$. Inoltre, un'aula ha una dimensione caratteristica di circa $20 \, \rm m$.
La lunghezza d'onda sarà:
$
\lambda = \frac{c}{f} = \frac{3 \times 10^{8} \,\rm \frac{m}{s}}{50 \,\rm Hz} \sim 3 \times 10^{8} \,\rm m = 6000\,\rm km  \gg L = 20 \,\rm m
$
La lunghezza d'onda è quindi di circa $6000 \,\rm km$ mentre un'aula ha una dimensione di circa $20\,\rm m$. È evidente che tra due punti di un'aula gli effetti elettromagnetici saranno praticamente identici.
Si può pertanto studiare questo sistema con un sistema a **parametri concentrati**

___

**TELEFONO in un AULA**
Consideriamo ora un telefono cellulare all'interno di un'aula. Questo lavora su frequenze anche intorno a $f = 1 \,\rm GHz$. In questo caso, la lunghezza d'onda è
$
\lambda = \frac{c}{f} = \frac{3 \times 10^{8} \,\rm \frac{m}{s}}{10^{9} \,\rm Hz} \sim 0.3 \,\rm m = 30\,\rm cm  < L = 20 \,\rm m
$
Questo sistema **NON** può essere chiaramente studiato a parametri concentrati in quanto un'onda elettromagnetica all'interno di una stanza entra più di 20 volte.

```

## Trasformatore


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/trasformatore/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





# [[Trasformatore\|Trasformatore]]

![Trasformatore 2024-06-28 17.51.48.excalidraw.png](/img/user/Excalidraw/Trasformatore%202024-06-28%2017.51.48.excalidraw.png)



```ad-Definizione
title: Trasformatore

Un **trasformatore** è una macchina elettrica statica che trasforma una potenza in ingresso in una (a volte diversa) potenza in uscita. Lo stesso fa per la tensione e la corrente

$
\begin{align}
P_{in} &\to P_{out} \\
V_{in}, I_{in} &\to V_{out}, I_{out}
\end{align}
$

Viene usato per variare i livelli di tensione e corrente.
```

.

```ad-example
title: Perché non produciamo e distribuiamo la corrente direttamente a $V_m$?

La corrente che usiamo quotidianamente è a tensione:
$
V_{m} \simeq 230\,\rm V \quad \text{A.C.}
$
A Roma si può contare un numero di utenze elettriche (abitazioni) nell'ordine di $10^{6}$. Ognuna di queste utenze ha solitamente a disposizione, da contratto, una potenza assorbita $P = 3 \,\rm kW = 3\times 10^{3}\,\rm kW$.

Si ha così che la potenza totale ($10^{6}\cdot 3\times 10^{3}\,\rm kW = 3\times10^{9}\,\rm kW$) data anche da $P = VI$, al fine di essere trasportata, richiederebbe una corrente di:
$
I = \frac{P}{V} = \frac{3\times10^{9}\,\rm kW}{230\,\rm V} \sim 13\times 10^{6}\,\rm A
$
I conduttori generalmente non sono garantiti per una densità di corrente infinita. Il limite è in genere di $J_{MAX} = 4\,\rm \frac{A}{mm^{2}}$. Per una corrente nell'ordine di $10^{6}\,\rm A$ servirebbe un conduttore di circa $3\,\rm m^{2}$ di sezione, il che risulta alquanto sconveniente.
```

# Trasformatore ideale

#UNI/ET/Domanda 

![Trasformatore 2024-06-28 17.55.16.excalidraw.png](/img/user/Excalidraw/Trasformatore%202024-06-28%2017.55.16.excalidraw.png)


Per via della [[Legge di Faraday-Neumann Lentz\|Legge di Faraday-Neumann Lentz]], nella seconda spira si genera una fem indotta:
$
e = \frac{\mathrm{d}\Phi }{\mathrm{d}t} 
$

### Riluttanza

```ad-Definizione
title: Riluttanza ($\mathcal{R}$)

$
\mathcal{R} = \frac{l}{\mu_{0}\mu_{r}S} \quad\rm [H^{-1}]
$
dove:
- $l:$ lunghezza del tratto mediano che definisce
- $\mu_{0} = 4 \pi \times10^{-7}\,\rm \frac{H}{m}:$
- $\mu_{r}:$ Permeabilità relativa ($\mu=\mu_{0}\mu_{r}$)


```

## Funzionamento del trasformatore

![Trasformatore 2024-06-28 18.07.33.excalidraw.png](/img/user/Excalidraw/Trasformatore%202024-06-28%2018.07.33.excalidraw.png)


Lo studio del [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore ideale\|#Trasformatore ideale]] prevede un'ipotesi di base di **idealità**: Permettono di dire che le perdite di potenza sono nulle

### Ipotesi di idealità

#### Ip 1 - Resistività del rame nulla

```ad-tip
title: Resistività del rame nulla

$
\rho_{\rm Cu} = 0:
$
La [[Resistività]] del [[Rame\|Rame]] è nulla. Questo implica che le [[04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule|perdite per effetto Joule]] siano nulle
$
P_{J_{1}},P_{J_{2}} = 0
$
```


#### Ip 2- Tubo di flusso ideale


```ad-tip
title: 2- Permeabilità magnetica del [[Ferro]] infinita

$
\mu_{\rm Fe} = \infty 
$
Non c'è neanche una minima quota parte di flusso che si richiude in aria. Tutto il flusso si richiude nel ferro del trasformatore. Quindi il **nucleo** agisce da **TUBO DI FLUSSO**.

Il flusso disperso è nullo: $\phi_{d} = 0$.

Questo implica che tra i due avvolgimenti vi sia [[Induttore#Mutuo accoppiamento|accoppiamento]] perfetto:
$
M = k \sqrt{L_{1}L_{2}} \quad \text{con } k = 1
$

```

Dalla definizione di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Riluttanza\|#Riluttanza]] si ottiene inoltre che, nel [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore ideale\|#Trasformatore ideale]]
$
\mathcal{R} = \frac{l}{\mu_{0}\mu_{r}S} \stackrel{\mu_{\rm Fe} = \infty}{=} 0
$

#### Ip 3 - Perdite per correnti parassite nulle

$
P_{cp} = 0
$
La potenza dissipata a causa delle correnti parassite o di [[Faucoult\|Faucoult]] è nulla.

Nella sezione infatti si genera una fem: $e(r) = j\omega\phi(r)$ (dove $r$ è la distanza dal centro della sezione) dovuta alla variazione del campo $\vec{B}$. Questo porta alla generazione di correnti vorticose che dissipano energia. La potenza dissipata da queste correnti è:
$
P_{cp} = Kf^{2}S^{2}B_{H}^{2}\sigma_{\rm Fe}
$
L'ipotesi è verificata sess $\sigma_{\rm Fe} = 0$ (conducibilità del nucleo ferromagnetico nulla)

#### Ip 4 - Perdite per isteresi nulle

Se guardassimo il nucleo ferromagnetico al microscopio noteremmo tanti domini magnetici orientati in maniera diversa --> tanti bipoli ognuno in direzione diversa.

Legge di Ampere:
$
\int \vec{H}\cdot \vec{dl} = N
$
dove
- $\vec{H}:$ Campo di intensità definito dal Teorema di circuitazione di Ampere (riferito alla corrente)

Si associa ad esso un campo $\vec{B}$ magnetico:
$
\vec{B} = \mu \vec{H}
$
La corrente aumenta proporzionalmente ad $\vec{H}$. $\vec{B}$, poiché $\mu$ non è costante, non aumenta proporzionalmente con $\vec{H}$ se non per un piccolissimo tratto.

![Trasformatore 2024-06-28 19.15.02.excalidraw.png](/img/user/Excalidraw/Trasformatore%202024-06-28%2019.15.02.excalidraw.png)


0-1
All'aumentare di $\vec{H}$, i domini cominciano ad orientarsi nella stessa direzione lungo la **curva di prima magnetizzazione** (0-1). 

1-2
Successivamente, quando tutti i domini si sono isorientati, $\vec{B}$ non aumenta più e si raggiunge il **campo di saturazione** - $\vec{B}_{s}$

2-3
Quando tolgo la corrente, si nota che la curva di ritorno non ripercorre quella di andata ma, quando la corrente è nulla, c'è una **magnetizzazione residua** non nulla - $\vec{B}_{r}$

3-4
La magnetizzazione va a zero solamente per una corrente imposta negativa. Si parla pertanto di **campo coercitivo**.

4-5
Raggiungo nuovamente un valore di saturazione della magnetizzazione - $-B_{s}$

5-7
Aumentando di nuovo la corrente torno a raggiungere **magnetizzazioen residua nulla** al valore positivo di campo coercitivo - $\vec{H}_{c}$

A questo punto, aumentando e diminuendo la corrente si continuerà a percorrere questo percorso detto **ciclo di isteresi**

Si dimostra che l'area del ciclo di isteresi è proporzionale alla potenza dissipata - $P_{is}$. Inoltre il ciclo non è lineare.

```ad-tip
title: Dissipazione per isteresi nulla


Si **ipotizza** che il ciclo di isteresi sia
- Lineare
- $P_{is} =0$
```


##### Legge di Hopkinson

$
\mathcal{R} \phi = \sum\limits_{i} \pm N_{i}I_{i} \stackrel{\triangle}{=} \mathcal{F} \qquad\rm [A] = [\text{Ampere Spire}] 
$
La legge di Hopkinson correla gli effetti delle grandezze elettriche (correnti) con gli effetti magnetici.


### Rapporto di trasformazione

```ad-Definizione
title: Rapporto di trasformazione

$
n = \frac{N_{1}}{N_{2}}
$


```

### Circuito equivalente ideale

![Trasformatore - Circuito equivalente ideale 2024-06-28 19.44.51.excalidraw.png](/img/user/Excalidraw/Trasformatore%20-%20Circuito%20equivalente%20ideale%202024-06-28%2019.44.51.excalidraw.png)


Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore ideale\|#Trasformatore ideale]] può essere rappresentato in una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] dal circuito equivalente disegnato sopra.

Sia
$
n = \frac{N_{1}}{N_{2}}
$
il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Rapporto di trasformazione\|#Rapporto di trasformazione]], sono vere le seguenti relazioni:
$
n = \frac{V_{1}}{V_{2}} \qquad n = \frac{I_{2}}{I_{1}}
$
Inoltre si deve avere che:
$
\overline{V}_{1} = \overline{E}_{1} \qquad \overline{V}_{2} = \overline{E}_{2}
$

Essendo per la [[Legge di Faraday-Neumann Lentz\|Legge di Faraday-Neumann Lentz]]
$
e = - \frac{\mathrm{d} \phi (t)}{\mathrm{d}t} 
$
allora:
$
\begin{align}
\overline{E}_{1} &= j\omega  N_{1}\overline\phi_{t} \qquad\longrightarrow\qquad \phi_{1c} = N_{1}\phi _{t}\\
\overline{E}_{2} &= j\omega  N_{2}\overline\phi_{t} \qquad\longrightarrow\qquad \phi_{2c} = -N_{2}\phi _{t}
\end{align}
$

Si richiama la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Legge di Hopkinson\|#Legge di Hopkinson]]

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/trasformatore/#legge-di-hopkinson" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



##### Legge di Hopkinson

$
\mathcal{R} \phi = \sum\limits_{i} \pm N_{i}I_{i} \stackrel{\triangle}{=} \mathcal{F} \qquad\rm [A] = [\text{Ampere Spire}] 
$
La legge di Hopkinson correla gli effetti delle grandezze elettriche (correnti) con gli effetti magnetici.



</div></div>


e la si applica al trasformatore. Ricordando l'ipotesi [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Ip 2- Tubo di flusso ideale\|#Ip 2- Tubo di flusso ideale]] per cui la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Riluttanza\|#Riluttanza]] è nulla si ha che:
$
\mathcal{F} = \mathcal{R}\phi = N_{1}\overline{I}_{1} - N_{1}\overline{I}_{2} \stackrel{\mathcal{R = 0}}{=} 0
$
e quindi si ricava la relazione:
$
\frac{\overline{I}_{1}}{\overline{I}_{2}} = \frac{N_{2}}{N_{1}}
$

Si ottengono così le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Equazioni di trasferimento del trasformatore ideale\|#Equazioni di trasferimento del trasformatore ideale]]

#### Equazioni di trasferimento del trasformatore ideale

$
\begin{cases}
\dfrac{V_{1}}{V_{2}} = \dfrac{E_{1}}{E_{2}} = \dfrac{N_{1}}{N_{2}} = n \\
\dfrac{I_{1}}{I_{2}} =  \dfrac{1}{n}
\end{cases}
$
#### Tipi di trasformatore ideale

- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore elevatore o innalzatore\|#Trasformatore elevatore o innalzatore]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore riduttore o abbassatore\|#Trasformatore riduttore o abbassatore]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore di isolamento\|#Trasformatore di isolamento]]

##### Trasformatore elevatore o innalzatore

Il **trasformatore elevatore o innalzatore** è quello per cui la tensione in uscita risulta *superiore* alla tensione in ingresso (a discapito della corrente)
$
\begin{align}
V_{1} &< V_{2} \\
N_{1} &< N_{2} \\
I_{1} &> I_{2}
\end{align}
$
Quindi
$
n < 1
$


##### Trasformatore riduttore o abbassatore


Il **trasformatore riduttore o abbassatore** è quello per cui la tensione in uscita risulta *inferiore* alla tensione in ingresso (a discapito della corrente)
$
\begin{align}
V_{1} &> V_{2} \\
N_{1} &> N_{2} \\
I_{1} &< I_{2}
\end{align}
$
Quindi
$
n>1
$

##### Trasformatore di isolamento

Il trasformatore di isolamento lascia invariate tensione e corrente tra ingresso e uscita. Serve come misura di sicurezza per disaccoppiare galvanicamente due parti dell'impianto.

$
\begin{align}
V_{1} &= V_{2} \\
N_{1} &= N_{2} \\
I_{1} &= I_{2}
\end{align}
$
Quindi
$
n=1
$

#### Trasparenza delle potenze - trasformatore ideale

Nel [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore ideale\|#Trasformatore ideale]] deve essere risultare che la somma delle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza complessa\|potenze complesse]] in ingresso e in uscita sia pari a 0:
$
\dot{P} = \dot{P}_{1}+\dot{P}_{2} = 0
$
Ricordando la definizione di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza complessa\|potenza complessa]] infatti:
$
\begin{align}
\dot{P}_{1}+\dot{P}_{2} &= \overline{V}_{1}\overline{I}_{1}^{*} - \overline{V}_{2}\overline{I}_{2}^{*} = \\
&= \cancel{n}\overline{V}_{2} \frac{\overline{I}_{2}^{*}}{\cancel{n}} - \overline{V}_{2}\overline{I}_{2}^{*}  =  \\
&= \overline{V}_{2} \overline{I}_{2}^{*} - \overline{V}_{2}\overline{I}_{2}^{*} = 0
\end{align}
$
Tanta potenza entra tanta ne esce.

Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore ideale\|#Trasformatore ideale]] ha **rendimento** unitario:
$
\eta  = \frac{P_{2}}{P_{1}} = 1
$

# Trasformatore reale

Lo studio del **trasformatore reale** si effettua a partire dal [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore ideale\|#Trasformatore ideale]] andando via via a rimuovere le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Ipotesi di idealità\|#Ipotesi di idealità]].

### Ipotesi trasformatore reale

#### Ip 1 - Resistività del rame

La [[Resistività]] del [[Rame]] è pari a
$
\begin{align}
\rho_{\rm Cu} &= 1.68\times10^{-8} \,\rm \Omega m \\
\sigma_{\rm Cu} &= 5.8\times10^{7} \,\rm \frac{S}{m}
\end{align}
$
Pertanto la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule\|potenza dissipata per Effetto Joule]] NON è nulla:
$
P_{J} \neq 0
$

Questo è rappresentabile nel circuito equivalente da una coppia di [[Resistore\|resistori]] (uno per avvolgimento):

![Trasformatore - Circuito eq con resistori - 2024-06-29 19.36.56.excalidraw.png](/img/user/Excalidraw/Trasformatore%20-%20Circuito%20eq%20con%20resistori%20-%202024-06-29%2019.36.56.excalidraw.png)



#### Ip 2 - Accoppiamento imperfetto

L'accoppiamento tra gli avvolgimenti del [[Trasformatore\|Trasformatore]] non è perfetto:
$
M = k \sqrt{L_{1}L_{2}} \qquad \text{con } k < 1
$
Questo è dovuto al fatto che la permeabilità magnetica del ferro $\mu_{\rm Fe} \neq 0$ e quindi il nucleo NON costituisce un Tubo di flusso ideale. Pertanto, alcune linee di flusso del campo magnetico si richiuderanno all'esterno del nucleo. Questo è rappresentabile sul circuito equivalente per mezzo di 2 [[Induttore\|induttori]]: **impedenze di dispersione** - $L_{1d}, L_{2d}$

![Trasformatore reale 2024-06-29 19.40.19.excalidraw.png](/img/user/Excalidraw/Trasformatore%20reale%202024-06-29%2019.40.19.excalidraw.png)


Le impedenze di dispersione sono tali da rispettare l'espressione:
$
L = \frac{N\phi_{d}}{\overline{I}}
$
dove:
- $N:$ Numero di avvolgimenti/spire
- $\phi_{d}:$ Flusso disperso
- $\overline{I}:$ Corrente

#### Altre ipotesi

Togliendo le altre ipotesi si ha che
$
\mathcal{R} \ne 0 \qquad\Longrightarrow\qquad \mathcal{F} = \mathcal{R}\phi \neq 0
$
che implica che bisogna spendere energia per magnetizzare il nucleo.
$
N_{1}\overline{I}_{1} \neq N_{2}\overline{I}_{2}
$
### Circuito equivalente reale'


![Trasformatore reale 2024-06-29 19.40.19.excalidraw.png](/img/user/Excalidraw/Trasformatore%20reale%202024-06-29%2019.40.19.excalidraw.png)


Nel trasformatore reale non è più vero che
$
\overline{V}_{1} = \overline{E}_{1} \qquad \overline{V}_{2} = \overline{E}_{2}
$
Infatti si ha:
$
\begin{cases}
\overline{V}_{1} &= \overline{E}_{1} + (R_{1}+j\omega L_{1d}) \overline{I}_{1} \\
\overline{V}_{2} &= \overline{E}_{2} - (R_{2}+j\omega L_{2d}) \overline{I}_{2}
\end{cases}
$
### Funzionamento a vuoto

Per valutare l'energia spesa dal [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Trasformatore reale\|#Trasformatore reale]] lo si studia in una configurazione a vuoto. Nel secondario viene lasciato il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Circuito aperto\|circuito aperto]] e quindi $\overline{I}_{2}=0$. 

![Trasformatore a vuoto 2024-06-30 12.13.57.excalidraw.png](/img/user/Excalidraw/Trasformatore%20a%20vuoto%202024-06-30%2012.13.57.excalidraw.png)


Il primario è ancora alimentato a una tensione $\overline{V}_{1}$, il secondario è aperto.

Vi saranno delle perdite di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] nel nucleo.

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Legge di Hopkinson\|#Legge di Hopkinson]] diventa:
$
\mathcal{R}\phi = N_{1}\overline{I}_{1} - N_{2}\cancel{\overline{I}_{2}} = N_{1}\overline{I}_{1\mu}
$
dove:
- $\overline{I}_{1\mu}:$ Corrente di magnetizzazione del primario

Si avranno pertanto le seguenti relazioni:
$
\begin{cases}
\overline{V}_{1} &= j\omega N_{1}\overline{\phi}_{t} \\
\overline{\phi}_{t} &= \dfrac{N_{1}\overline{I}_{1\mu }}{\mathcal{R}}
\end{cases}
$
che unite permettono di esprimere la tensione $\overline{V}_{1}$ come
$
\overline{V}_{1} = j\omega  \frac{N_{1}^{2}}{\mathcal{R}} \overline{I}_{1\mu }
$
Questo effetto è rappresentabile da un [[Induttore\|Induttore]] in parallelo con l'avvolgimento del trasformatore come in figura. In parallelo ad esso si aggiunge poi un [[Resistore\|Resistore]] per tenere conto della componente in fase della corrente.

Si avranno pertanto:
- 1 induttore - $\overline{I}_{1\mu}$ - tiene conto della potenza persa per magnetizzare il nucleo ferromagnetico
- 1 resistore - $\overline{I}_{1f}$ - tiene conto delle perdite di potenza attiva nel nucleo

![Trasformatore reale - circuito 2024-06-30 16.05.42.excalidraw.png](/img/user/Excalidraw/Trasformatore%20reale%20-%20circuito%202024-06-30%2016.05.42.excalidraw.png)


### Circuito equivalente reale


![Trasformatore reale - circuito 2024-06-30 16.05.42.excalidraw.png](/img/user/Excalidraw/Trasformatore%20reale%20-%20circuito%202024-06-30%2016.05.42.excalidraw.png)


Per la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] alle due maglie (del primario e del secondario):
$
\begin{cases}
\overline{V}_{1} &= \overline{E}_{1} + (R_{1}+j\omega L_{1d})\overline{I}_{1} \\
\overline{V}_{2} &= \overline{E}_{2} - (R_{2}+j\omega L_{2d})\overline{I}_{2}
\end{cases}
$
Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Rapporto di trasformazione\|#Rapporto di trasformazione]]
$
n = \frac{\overline{E}_{1}}{\overline{E}_{2}} = \frac{N_{1}}{N_{2}}
$
che permette di riscrivere le equazioni sopra:
$
\begin{cases}
\overline{V}_{1} &= \overline{E}_{1} + (R_{1}+j\omega L_{1d})\overline{I}_{1} = n\overline{E}_{2} + (R_{1}+j\omega L_{1d})\overline{I}_{1} \\
\overline{V}_{2} &= \overline{E}_{2} - (R_{2}+j\omega L_{2d})\overline{I}_{2} \qquad\Longrightarrow\qquad \overline{E}_{2} = \overline{V}_{2} + (R_{2}+j\omega L_{2d})\overline{I}_{2}
\end{cases}
$
E quindi scrivo $\overline{V}_{1}$ come
$
\overline{V}_{1} = (R_{1}+j\omega L_{1d})\overline{I}_{1} + n \left( \overline{V}_{2} + (R_{2}+j\omega L_{2d})\overline{I}_{2} \right) 
$
Si osservi come **NON** c'è proporzionalità diretta tra $V_{1}$ e $V_{2}$.

Le correnti presenti nel circuito equivalente sono legate dalle seguenti relazioni:
$
\begin{align}
\overline{I}_{10} &= \overline{I}_{1\mu} + \overline{I}_{1f} \\
\overline{I}_{1} &= \overline{I}_{10} + \overline{I}_{12}
\end{align}
$
Mentre le correnti tra primario e secondario sono legate dalla:
$
\overline{I}_{12} = \frac{1}{n} \overline{I}_{2}
$
Si ottengono così le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Equazioni di trasferimento del trasformatore reale\|#Equazioni di trasferimento del trasformatore reale]]

#### Equazioni di trasferimento del trasformatore reale

$
\begin{cases}
\overline{V}_{1} &= (R_{1}+j\omega L_{1d})\overline{I}_{1} + n \left( \overline{V}_{2} + (R_{2}+j\omega L_{2d})\overline{I}_{2} \right) \\
\overline{I}_{12} &= \cfrac{1}{n} \overline{I}_{2}
\end{cases}
$

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗


</div></div>
