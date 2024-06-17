---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/04-fenomeni-di-conduzione-e-resistori-et/"}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET\|04 - Fenomeni di conduzione e resistori - ET]]

## Resistenza elettrica

Dato un conduttore cilindrico omogeneo di una certa sezione $S$ collegato ad un generatore, questo sarà attraversato da una certa corrente $I$.
Tra i due capi del conduttore si può misurare una differenza di potenziale (d.d.p.) $V$.

```ad-Definizione
title: Resistena Elettrica

In condizioni stazionarie, si osserva proporzionalità diretta tra i valori di $I$ e $V$. Pertanto, il loro rapporto è costante:
$
R = \frac{V}{I}
$
Il parametro di proporzionalità $R$ è detto **resistenza elettrica** e ha le dimensioni fisiche di ohm:
$
[\Omega] = \rm \left[  \frac{V}{A}  \right]
$

```

Quella appena enunciata è la [[I Legge di Ohm\|I Legge di Ohm]]

##### Potenza dissipata per Effetto Joule

L'esperienza di Joule dimostra che un conduttore attraversato da corrente si riscalda. Dissipa pertanto energia.

```ad-Teo
title: Potenza dissipata per Effetto Joule ($P_{d}$)

La potenza dissipata per effetto Joule è
$
P_{d} = RI^{2} \qquad \rm [W]
$

```

La potenza elettrica dissipata per Effetto Joule coincide con la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza assorbita\|potenza assorbita]] dal tratto di conduttore preso in considerazione:
$$
P_{a} = VI = P_{d}
$$

### Legge di Ohm


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


### Conduttanza

È possibile definire anche un altro parametro come inverso della [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica\|#Resistenza elettrica]]:

```ad-Definizione
title: Conduttanza ($G$)

La **conduttanza** è l'inverso della [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica\|#Resistenza elettrica]]:
$
G = \frac{1}{R} \qquad [S]
$
e si misura in *siemens* ($S$).

```

## Resistività e conducibilità dei materiali

La [[#Resistenza elettrica]] dipende dalla geometria del conduttore. In particolare, si può definire la [[II Legge di Ohm\|II Legge di Ohm]]:


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






