---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/00-introduzione-elettrotecnica/"}
---


# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica\|00 - Introduzione elettrotecnica]]

## Dipolo

I dipoli sono lineari

Un dipolo è ad esempio un [[Resistore\|Resistore]]


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/resistore/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Resistore\|Resistore]]

![Resistore 2024-02-26 18.37.25.excalidraw.png](/img/user/Excalidraw/Resistore%202024-02-26%2018.37.25.excalidraw.png)


Un resistore è un **dipolo passivo**

Esso ostacola la corrente e dissipa potenza per [[Effetto Joule\|Effetto Joule]]

La potenza dissipata è

$
P = RI^{2} \qquad \rm [W] = [\Omega][A^{2}]
$


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

```ad-example
title: Esempi

**SISTEMA ELETTRICO in un AULA**
Consideriamo il sistema elettrico di un'aula universitaria. La corrente nell'aula è di tipo alternata con frequenza $f = 50 \, \rm Hz$. Inoltre, un'aula ha una dimensione caratteristica di circa $20 \, \rm m$.
La lunghezza d'onda sarà:
$
\lambda = \frac{c}{f} = \frac{3\times 10^{8} \frac{m}{s}}{50 \,\rm Hz} \sim = 6 \times 10^{6} \,\rm m
$
La lunghezza d'onda è quindi di circa $6000 \,\rm km$ mentre un'aula ha una dimensione di circa $20\,\rm m$. È evidente che tra due punti di un'aula gli effetti elettromagnetici saranno praticamente identici.
Si può pertanto studiare questo sistema con un sistema a **parametri concentrati**

___

**TELEFONO in un AULA**
Consideriamo ora un telefono cellulare all'interno di un'aula. Questo lavora su frequenze anche intorno a $f = 1 \,\rm GHz$. In questo caso, la lunghezza d'onda è
$
\lambda = \frac{c}{f} = \frac{3\times 10^{8} \frac{m}{s}}{10^{9} \,\rm Hz} \sim 0.3\,\rm m = 30 \,\rm cm
$
Questo sistema **NON** può essere chiaramente studiato a parametri concentrati in quanto un'onda elettromagnetica all'interno di una stanza entra più di 20 volte.

```


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

Supponiamo di avere un segnale elettrocomagnetico fatto come in figura sotto:

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

