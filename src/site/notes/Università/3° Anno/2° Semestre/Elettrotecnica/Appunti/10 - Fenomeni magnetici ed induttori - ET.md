---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/10-fenomeni-magnetici-ed-induttori-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/10 - Fenomeni magnetici ed induttori - ET\|10 - Fenomeni magnetici ed induttori - ET]]


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/induttore/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Induttore\|Induttore]]

![Induttore sinusoidale.excalidraw.png](/img/user/Excalidraw/Induttore%20sinusoidale.excalidraw.png)


L'**induttore** è descritto dalla seguente legge:
$
\phi(t) = Li(t)
$
dove:
- $\phi(t):$ Flusso nel solenoide
- $L:$ [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/10 - Fenomeni magnetici ed induttori - ET#Induttanza\|#Induttanza]]

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
$
e(t) = - \frac{d\phi(t)}{dt} = - L \frac{di(t)}{dt}
$

```ad-Teo
title: Legge costitutiva dell'induttore

La **Legge costitutiva dell'[[Induttore]]** lega la tensione alla corrente ([[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Caratteristica esterna\|caratteristica esterna]]):
$
v(t)= L \frac{di(t)}{dt}
$

```

## Regime sinusoidale


![Induttore sinusoidale.excalidraw.png](/img/user/Excalidraw/Induttore%20sinusoidale.excalidraw.png)


L'[[Induttore]], [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore\|convenzionato da utilizzatore]], dotato di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/10 - Fenomeni magnetici ed induttori - ET#Induttanza\|#Induttanza]] costante $L$, rispetta sempre la relazione:
$
v(t) = L \frac{di(t)}{dt}
$
dove
- $i(t) = I_{M}\sin(\omega t+\beta) = \sqrt{2} I\sin(\omega t+\beta)$

da cui si ricava la legge della tensione:
$
v(t) = \omega L I_{M}\sin\left( \omega t + \beta + \frac{\pi}{2} \right)
$
Valgono pertanto le seguenti relazioni:

```ad-Teo
title:
$
\frac{V_{M}}{I_{M}} = \frac{V}{I} = \omega L \qquad \alpha-\beta = \varphi=\frac{\pi}{2}
$

```

Quindi la tensione, in un induttore a regime sinusoidale, si trova in *[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in anticipo]]* sulla corrente

![Induttore 2024-06-20 14.18.01.excalidraw.png](/img/user/Excalidraw/Induttore%202024-06-20%2014.18.01.excalidraw.png)


Si osservi che la tensione e la corrente sono legate dal prodotto
$
X_{L} = \omega L
$
che è definita [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/10 - Fenomeni magnetici ed induttori - ET#reattanza induttiva\|#reattanza induttiva]].

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza istantanea]] ha ampiezza $VI$ e dà luogo a lavoro assorbito in forma di energia induttiva pari a $w_{L}(t) = \frac{1}{2}Li^{2}$.

Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|fattore di potenza]] è nullo: $\cos(\varphi) = 0$ (essendo corrente e tensione in quadratura). Pertanto anche la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] assorbita è nulla. Inoltre, [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|potenza apparente]] e [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|reattiva]] coincidono.
$
P = 0 \qquad Q = A = VI = X_{L}I^{2}
$

___

L'induttore in regime sinusoidale può essere descritto anche facendo riferimento alle grandezze [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriali]].
$
\begin{align}
i(t) &\Longrightarrow \overline{I} = Ie^{j\beta} \\
v(t) &\Longrightarrow \overline{V} = Ve^{j\alpha}
\end{align}
$
Il rapporto tra i fasori vale:
$
\frac{\overline{V}}{\overline{I}} = \frac{V}{I}e^{j\varphi} = \frac{V}{I}e^{j \frac{\pi}{2}} = j\omega L = j X_{L}
$

Pertanto, in termini fasoriali, è vera la relazione:
$
\overline{V} = jX_{L}\overline{I}
$
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


## Mutuo accoppiamento

Si considerino 2 induttori (immaginiamo per semplicità 2 spire) qualsiasi tali che nel primo non scorra corrente $i_{1} \equiv 0$ e nel secondo scorra corrente alternata $i_{2}$. Nella seconda spira sarà indotto un campo magnetico $\boldsymbol{B_{2}}$ dovuto solo ad $i_{2}$. È possibile che alcune linee di campo di $\boldsymbol{B_{2}}$ siano concatenate con la prima spira. 

Allo stesso modo, è possibile la situazione duale in cui $i_{2}\equiv0$ e nella prima spira scorra $i_{1}$, inducendo $\boldsymbol{B_{1}}$ con alcune linee di campo concatenate con spira 2.

Nella situazione descritta si dice che gli induttori sono **mutualmente accoppiati**.

Per via del mutuo accoppiamento si può scrivere, nel primo caso, la relazione
$
M_{12} = \frac{\varphi_{c12}(t)}{i_{2}(t)}
$
dove:
- $\varphi_{c12}:$ flusso del campo $\boldsymbol{B_{2}}$ concatenato dall'induttore 1
- $i_{2}(t):$ Corrente che scorre nell'induttore 2
- $M_{12}:$ **Mutua induttanza** o **coefficiente di mutua induzione** tra l'induttore 1 e l'induttore 2

In modo del tutto analogo si definisce $M_{21}$

Si può definire il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/10 - Fenomeni magnetici ed induttori - ET#Coefficiente di mutuo accoppiamento\|#Coefficiente di mutuo accoppiamento]]
$
M_{12} = M_{21} = M
$


![Induttore 2024-06-22 11.42.03.excalidraw.png](/img/user/Excalidraw/Induttore%202024-06-22%2011.42.03.excalidraw.png)


Gli induttori in figura sono mutualmente accoppiati con [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/10 - Fenomeni magnetici ed induttori - ET#Coefficiente di mutuo accoppiamento\|#Coefficiente di mutuo accoppiamento]] pari a $M$. Si possono pertanto scrivere le equazioni:
$
\begin{cases}
\overline{V}_{1} = j\omega L_{1} \overline{I}_{1} + j\omega M \overline{I}_{2} \\
\overline{V}_{2} = j\omega L_{2} \overline{I}_{2} + j\omega M \overline{I}_{1}
\end{cases}
$
Il segno della caduta di tensione dovuta alla mutua induzione si sceglie a seconda della posizione del pallino rispetto alle correnti:
- Se entrambe le correnti incontrano prima il pallino o prima l'induttore si prende concorde alla caduta di tensione sull'induttore
- Se una delle correnti incontra prima il pallino e l'altra prima l'induttore si prende segno discorde alla caduta di tensione sull'induttore

### Coefficiente di mutuo accoppiamento

```ad-Definizione
title: Coefficiente di mutuo accoppiamento ($M$)

Il **coefficiente di mutua induttanza** caratterizza il [[#Mutuo accoppiamento]] tra 2 induttori:
$
M = \frac{\varphi_{c12}(t)}{i_{2}(t)} = \frac{\varphi_{c21}(t)}{i_{1}(t)} \qquad \rm [H]
$

```




</div></div>


## Circuito RL

```ad-Definizione
title: Circuito RL

Un **circuito RL** è una [[03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica|rete elettrica]] costituita esclusivamente da [[Resistore|resistori]] e [[Induttore|Induttori]].

```

![10 - Fenomeni magnetici ed induttori - ET 2024-06-18 17.26.09.excalidraw.png](/img/user/Excalidraw/10%20-%20Fenomeni%20magnetici%20ed%20induttori%20-%20ET%202024-06-18%2017.26.09.excalidraw.png)


Percorrendo la maglia in senso orario, si scrive la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]]:
$$
e_{s}(t) -v_{R}(t)-v_{L}(t)
$$
da cui, tenendo a mente le [[06 - Bipoli e potenza elettrica - ET#Caratteristica esterna|caratteristica esterna]] del [[Resistore#Caratteristica esterna\|resistore]] e la [[Induttore#Legge costitutiva dell'induttore\|legge costitutiva dell'induttore]] si può riscrivere:
$$
e_{s}(t) = Ri(t) +L \frac{di(t)}{dt}
$$

```ad-note
title: Osservazione
In [[DC]] (Direct Current) $i(t) = \rm cost.$ e quindi $\dfrac{di(t)}{dt}=0$. In DC quindi, in un circuito LR, l'induttore svolge il ruolo di [[06 - Bipoli e potenza elettrica - ET#Cortocircuito|cortocircuito]].

```

