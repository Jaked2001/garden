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




# [[Resistività]]

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



</div></div>
