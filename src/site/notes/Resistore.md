---
{"dg-publish":true,"permalink":"/resistore/"}
---

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

$$
P = RI^{2} \qquad \rm [W] = [\Omega][A^{2}]
$$


### Caratteristica esterna

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]] del resistore è
$$
V = RI
$$
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
$$
i(t) = \sqrt{2}I\sin(\omega t+\beta)
$$
pertanto la tensione sarà:
$$
v(t) = \sqrt{2} RI\sin(\omega t+\beta) = \sqrt{2}V\sin(\omega t+\alpha)
$$
Valgono pertanto le relazioni:
- $\dfrac{V}{I} = R$ tra [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valori efficaci]]
- $\alpha=\beta$ e quindi [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|sfasamento]] $\varphi=0$

Nel [[Resistore#Regime sinusoidale\|resistore in regime sinusoidale]] tensione e corrente sono in fase quindi massimi, minimi e zeri sono negli stessi punti.

![Resistore 2024-06-20 12.10.16.excalidraw.png](/img/user/Excalidraw/Resistore%202024-06-20%2012.10.16.excalidraw.png)


La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] del resistore è
$$
P = VI \ge 0
$$
ed è sempre **NON** negativa (il resistore non può erogare potenza). La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza istantanea]] ha valore massimo $V_{M}I_{M} = 2VI$.

Essendo $\varphi=0$ il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|fattore di potenza]] $\cos(\varphi)=1$. Quindi, tutta la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza assorbita\|potenza assorbita]] coincide con la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|potenza apparente]] $A$. La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|potenza reattiva]] $Q = 0$.
$$
A = \sqrt{P^{2}+Q^{2}} = P
$$
quindi
$$
P = A = VI = RI^{2} \qquad Q = 0
$$

___

Il resistore in regime sinusoidale può essere descritto anche facendo riferimento alle grandezze [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriali]].
$$
\begin{align}
i(t) &\Longrightarrow \overline{I} = Ie^{j\beta} \\
v(t) &\Longrightarrow \overline{V} = Ve^{j\alpha}
\end{align}
$$
Il rapporto tra i fasori vale:
$$
\frac{\overline{V}}{\overline{I}} = \frac{V}{I}e^{j\varphi} = R
$$

