---
{"dg-publish":true,"permalink":"/induttore/"}
---

# [[Induttore\|Induttore]]

![Induttore sinusoidale.excalidraw.png](/img/user/Excalidraw/Induttore%20sinusoidale.excalidraw.png)


L'**induttore** è descritto dalla seguente legge:
$$
\phi(t) = Li(t)
$$
dove:
- $\phi(t):$ Flusso nel solenoide
- $L:$ [[Induttore#Induttanza\|#Induttanza]]

## Induttanza

```ad-Definizione
title: Induttanza

L'**induttanza** dell'[[Induttore\|Induttore]] è
$
L = \frac{\phi(t)}{i(t)} \qquad [H]
$
Si misura in Henry $[H]$.


```

## Legge costitutiva dell'induttore

Per la [[Legge di Faraday-Neumann Lentz\|Legge di Faraday-Neumann Lentz]]
$$
e(t) = - \frac{d\phi(t)}{dt} = - L \frac{di(t)}{dt}
$$

```ad-Teo
title: Legge costitutiva dell'induttore

La **Legge costitutiva dell'[[Induttore]]** lega la tensione alla corrente ([[06 - Bipoli e potenza elettrica - ET#Caratteristica esterna|caratteristica esterna]]):
$
v(t)= L \frac{di(t)}{dt}
$

```

## Regime sinusoidale


![Induttore sinusoidale.excalidraw.png](/img/user/Excalidraw/Induttore%20sinusoidale.excalidraw.png)


L'[[Induttore]], [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore\|convenzionato da utilizzatore]], dotato di [[Induttore#Induttanza\|#Induttanza]] costante $L$, rispetta sempre la relazione:
$$
v(t) = L \frac{di(t)}{dt}
$$
dove
- $i(t) = I_{M}\sin(\omega t+\beta) = \sqrt{2} I\sin(\omega t+\beta)$

da cui si ricava la legge della tensione:
$$
v(t) = \omega L I_{M}\sin\left( \omega t + \beta + \frac{\pi}{2} \right)
$$
Valgono pertanto le seguenti relazioni:

```ad-Teo
title:
$
\frac{V_{M}}{I_{M}} = \frac{V}{I} = \omega L \qquad \alpha-\beta = \varphi=\frac{\pi}{2}
$

```

quindi la tensione, in un induttore a regime sinusoidale, si trova in *[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in anticipo]]* sulla corrente

![Induttore 2024-06-20 14.18.01.excalidraw.png](/img/user/Excalidraw/Induttore%202024-06-20%2014.18.01.excalidraw.png)


Si osservi che la tensione e la corrente sono legate dal prodotto
$$
X_{L} = \omega L
$$
che è definita [[Induttore#reattanza induttiva\|#reattanza induttiva]].

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza istantanea]] ha ampiezza $VI$ e dà luogo a lavoro assorbito in forma di energia induttiva pari a $w_{L}(t) = \frac{1}{2}Li^{2}$.

Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|fattore di potenza]] è nullo: $\cos(\varphi) = 0$ (essendo corrente e tensione in quadratura). Pertanto anche la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] assorbita è nulla. Inoltre, [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|potenza apparente]] e [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|reattiva]] coincidono.
$$
P = 0 \qquad Q = A = VI = X_{L}I^{2}
$$

___

L'induttore in regime sinusoidale può essere descritto anche facendo riferimento alle grandezze [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriali]].
$$
\begin{align}
i(t) &\Longrightarrow \overline{I} = Ie^{j\beta} \\
v(t) &\Longrightarrow \overline{V} = Ve^{j\alpha}
\end{align}
$$
Il rapporto tra i fasori vale:
$$
\frac{\overline{V}}{\overline{I}} = \frac{V}{I}e^{j\varphi} = \frac{V}{I}e^{j \frac{\pi}{2}} = j\omega L = j X_{L}
$$

Pertanto, in termini fasoriali, è vera la relazione:
$$
\overline{V} = jX_{L}\overline{I}
$$
immaginario puro
### Reattanza induttiva

```ad-Definizione
title: Reattanza induttiva ($X_{L}$)

La reattanza induttiva è definita come il prodotto
$
X_{L} = \omega L \qquad \rm [Hs^{-1}] = [\Omega]
$
e ha unità di misura omogenee con quella della [[04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica|resistenza]].

```


