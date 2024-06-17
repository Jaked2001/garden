---
{"dg-publish":true,"permalink":"/generatore-di-tensione/"}
---

# # [[Generatore di tensione\|Generatore di tensione]]


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/generatore-ideale-di-tensione/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Generatore ideale di tensione\|Generatore ideale di tensione]]


```ad-Definizione
title: Generatore ideale di corrente

Il generatore ideale di corrente è un [[00 - Introduzione elettrotecnica#Dipolo|dipolo]] attivo che verifica la relazione:
$
E = E_{s} \quad \forall I
$

```

Si indica con il simbolo:

![Generatore ideale di tensione 2024-03-03 18.09.15.excalidraw.png](/img/user/Excalidraw/Generatore%20ideale%20di%20tensione%202024-03-03%2018.09.15.excalidraw.png)


### Caratteristica esterna

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del [[Generatore di tensione#Generatore ideale di tensione\|#Generatore ideale di tensione]] è
$
V = E_{s} \quad \forall I
$

Sul piano $V-I$ si ha una retta parallela a $I$ passante per la quota $E_{s}$:

![Generatore ideale di tensione 2024-03-03 18.12.01.excalidraw.png](/img/user/Excalidraw/Generatore%20ideale%20di%20tensione%202024-03-03%2018.12.01.excalidraw.png)


Essendo la [[Potenza\|Potenza]] data da
$
P = VI = E_{s}I
$
è evidente che il **generatore ideale di tensione** può avere potenza negativa (nel 2° quadrante).

$I < 0$ vuol dire che la corrente ha verso opposto a quello che avevo indicato. Il dipolo sta lavorando da *utilizzatore* e non da *generatore*.
Quest'ultima proprietà lo rende un dipolo attivo.



</div></div>



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

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del [[Generatore di tensione#Generatore reale di tensione\|#Generatore reale di tensione]] è
$
V = E - RI_{s}
$
Sul piano $V-I$

![Generatore reale di tensione 2024-06-16 16.01.53.excalidraw.png](/img/user/Excalidraw/Generatore%20reale%20di%20tensione%202024-06-16%2016.01.53.excalidraw.png)


</div></div>

