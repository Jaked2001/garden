---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/14-reti-in-regime-sinusoidale-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET\|14 - Reti in regime sinusoidale - ET]]

## Regime sinusoidale

Una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] si dice che lavora in regime sinusoidale quando *tutte* le tensioni e *tutte* le correnti variano nel tempo come [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzioni sinusoidali isofrequenziali\|sinusoidi isofrequenziali]].

Possono essere analizzate con metodi molto simili a quelli usati per le reti in regime stazionario. Ammesso che tutte le equazioni descrittive siano equazioni differenziali lineari alle derivate parziali valgono il principio di sovrapposizione degli effetti e i metodi che ne derivano.

## Bipolo in regime sinusoidale e potenza

#UNI/ET/Domanda 

### Tensione, corrente e sfasamento

Si consideri un generico [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Bipolo\|bipolo]] in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Regime sinusoidale\|#Regime sinusoidale]] applicando una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzioni per tensione e corrente su un bipolo\|convenzione a scelta]].

![14 - Reti in regime sinusoidale - ET 2024-06-19 17.53.51.excalidraw.png|450](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-19%2017.53.51.excalidraw.png)


Sopra è mostrato un generico bipolo in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore\|convenzione utilizzatori]]. Tensione e corrente sono descritte da [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|funzioni sinusoidali]]:
$$
\begin{cases}
v(t) &= V_{M}\sin(\omega t+\alpha) = \sqrt{2}V\sin(\omega t+\alpha)\\
i(t) &= I_{M}\sin(\omega t+\beta) = \sqrt{2}I\sin(\omega t+\beta)
\end{cases}
$$
dove:
- $V,I:$ [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|Valori efficaci]] di tensione e corrente

Lo [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|sfasamento]] tra tensione e corrente è $\varphi$:
$$
\varphi=\alpha-\beta
$$

![14 - Reti in regime sinusoidale - ET 2024-06-19 17.59.46.excalidraw.png](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-19%2017.59.46.excalidraw.png)


Si associano a $v(t)$ e $i(t)$ i seguenti [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasori]]:
$$
\begin{cases}
\overline{V} &= Ve^{j\alpha} \\
\overline{I} &= Ie^{j\beta}
\end{cases}
$$

![14 - Reti in regime sinusoidale - ET 2024-06-19 18.08.25.excalidraw.png](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-19%2018.08.25.excalidraw.png)



### Potenza istantanea

```ad-Definizione
title: Potenza istantanea

La **potenza istantanea** - in maniera analoga alla [[03 - Introduzione allo studio delle reti elettriche - ET#Potenza|potenza in regime stazionario]] - è data da prodotto di tensione e corrente:
$
p(t) = v(t)i(t) \qquad \rm [W]
$

```

La potenza istantanea diventa, in accordo con la definizione:
$$
p(t) = v(t)i(t) = V_{M}\sin(\omega t + \alpha)I_{M}\sin(\omega t + \beta)
$$
Sfruttando una delle [[Formule di Werner\|Formule di Werner]] l'equazione sopra può essere riscritta come:
$$
\begin{align}
p(t) &= \frac{V_{M}I_{M}}{2} \cos(\alpha-\beta) - \frac{V_{M}I_{M}}{2} \cos(2\omega t+\alpha+\beta) = \\
&= VI\cos(\varphi)- VI\cos (2\omega t+\alpha+\beta)
\end{align}
$$
dove:
- $\varphi:$ [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|sfasamento]]
- $V,I:$ [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valori efficaci]]

Nella formula si osserva la somma di 2 quantità. Una costante:
$$
P_{cost} = VI \cos(\varphi)
$$
e una sinusoidale con pulsazione angolare $2\omega$ detta **potenza fluttuante**:
$$
p_{f}(t) = -VI\cos (2\omega t+\alpha+\beta)
$$
Quindi:
$$
p(t) = P_{cost} + p_{f}(t)
$$



### Potenza attiva - reale

```ad-Definizione
title: Potenza attiva ($P$)

Si definisce **potenza attiva** o **reale** il valore medio sul periodo di una potenza periodica:
$
P = \frac{1}{T} \int_{T}p(t) \, dt = VI\cos(\varphi) \qquad \rm [W]
$

```

Si osservi che la potenza attiva corrisponde alla parte costante della [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|#Potenza istantanea]].

- È **massima** e pari a $VI$ se tensione e corrente sono in *fase*.
- È **minima** e pari a $-VI$ se tensione e corrente sono in *opposizione di fase*.
- È **nulla** se tensione e corrente sono in *quadratura*

La potenza attiva è proporzionale a:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|Valore efficace]] di tensione
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|Valore efficace]] di corrente
- Coseno dello sfasamento ([[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|#Fattore di potenza]])

Il **lavoro** $\Delta\mathcal{L}$ assorbito in un intervallo di tempo multiplo del periodo ($\Delta t = nT$) è ottenibile come:
$$
\Delta\mathcal{L} = P\Delta t
$$
La formula vale per un qualunque intervallo di tempo (anche non multiplo del periodo) purché esso sia molto maggiore del periodo ($\Delta t >>T$). In questo caso infatti, seppur toccherebbe contare il contributo della [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza fluttuante]], questa sarebbe trascurabile.

### Potenza apparente e reattiva

[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|#Potenza apparente]] e [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|#Potenza reattiva]] (definite in seguito) sono rapportate dalla seguente relazione alla [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|#Potenza attiva - reale]]:
$$
A = \sqrt{P^{2}+Q^{2}}
$$
Inoltre si può dire
$$
P = A\cos \varphi \qquad Q = A\sin \varphi
$$
La quantità $\cos\varphi$ è detto [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|#Fattore di potenza]]

#### Potenza apparente

```ad-Definizione
title: Potenza apparente ($A$)

La potenza apparente è definita come la quantità
$
A = VI \qquad \rm [VA]
$
e si misura in voltampere. 
```

La potenza apparente non è associata al lavoro scambiato pertanto non si misura in Watt ma in Voltampere (le due unità sono comunque omogenee).

La potenza apparente è **sempre positiva**
$$
A > 0 \quad \text{sempre}
$$

#### Potenza reattiva

```ad-Definizione
title: Potenza reattiva ($Q$)

La **potenza reattiva** è definita come
$
Q = VI \sin(\varphi) \qquad \rm [VAR]
$
e si misura in Voltampere reattivi.

```

$$
Q =A\sin\varphi
$$

La potenza reattiva è entrante se il bipolo è [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore\|convenzionato da utilizzatore]], è uscente se è [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione del generatore\|convenzionato da generatore]].

La potenza reattiva non è associata al lavoro scambiato pertanto non si misura in Watt ma in Voltampere reattivi (le due unità sono comunque omogenee).

La potenza reattiva dipende da:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|Valore efficace]] di tensione
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|Valore efficace]] di corrente
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|Sfasamento]] tra tensione e corrente


- È **massima** e pari a $VI$ se la tensione è in *quadratura in anticipo* rispetto alla corrente
- È **minima** e pari a $-VI$ se la tensione è in *quadratura in ritardo* rispetto alla corrente
- È **nulla** se tensione e corrente sono in *fase* o in *opposizione di fase*

#### Fattore di potenza

```ad-Definizione
title: Fattore di potenza ($\cos\varphi$)

Si dice **fattore di potenza** la quantità
$
\cos\varphi= \frac{P}{A}
$
ed esprime la quota parte di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|#Potenza apparente]] che dà luogo a [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|#Potenza attiva - reale]] (ossia a scambi di lavoro)

```

### Potenza complessa

```ad-Definizione
title: Potenza complessa ($\dot{P}$)

Si definisce **potenza complessa** il prodotto tra il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasore]] di tensione $\overline{V}$ e il coniugato del fasore di corrente $\overline{I}^{*}$
$
\dot{P} = \overline{V}\overline{I}^{*}= VIe^{j\varphi}
$

```

Ricordando inoltre la definizione di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|#Potenza apparente]] $A = VI$
$$
\dot{P} = Ae^{j\varphi} = A\cos{\varphi} + jA\sin\varphi= P+jQ
$$
Pertanto, si può dire che
- **Parte reale** della potenza complessa = [[#Potenza attiva - reale]]
- **Parte immaginaria** della potenza complessa = [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|#Potenza reattiva]]
$$
\dot{P} = \mathcal{Re}_{\dot P} + j \mathcal{Im}_{\dot P}
$$
dove:
- $\mathcal{Re}_{\dot P} = P$
- $\mathcal{Im}_{\dot P} = Q$

```ad-note
title: Osservazione

Si noti che conoscere la potenza complessa significa avere ben 4 informazioni:
- [[#Potenza apparente]] - $A$
- [[13 - Funzioni sinusoidali e fasori - ET#Sfasamento|Sfasamento]] tra tensione e corrente - $\varphi$
- [[#Potenza attiva - reale]] - $P$
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|#Potenza reattiva]] - $Q$

```

## Bipoli ideali in regime sinusoidale

### Generatori ideali in regime sinusoidale


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/generatore-ideale-di-tensione-sinusoidale/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# Generatore ideale di tensione - AC

</div>



# [[Generatore ideale di tensione sinusoidale\|Generatore ideale di tensione sinusoidale]]

```ad-Definizione
title: Generatore ideale di tensione sinusoidale

![Generatore ideale di tensione - AC 2024-06-20 10.57.28.excalidraw.png](/img/user/Excalidraw/Generatore%20ideale%20di%20tensione%20-%20AC%202024-06-20%2010.57.28.excalidraw.png)
%%[[Generatore ideale di tensione - AC 2024-06-20 10.57.28.excalidraw.md|🖋 Edit in Excalidraw]]%%

Un **generatore ideale di tensione** è un [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipolo]] attivo che impone ai morsetti una tensione [[13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale|sinusoidale]]:
$
v(t) = e(t) = E_{M}\sin(\omega t+\alpha) = \sqrt{2} E \sin(\omega t+\alpha) \qquad\forall i(t)
$
- $e(t)$ è detta **tensione sinusoidale impressa**

```

Più comunemente la tensione impressa si esprime con il rispettivo [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasore]]:
$
\overline{E_{s}} = Ee^{j\alpha}
$


</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/generatore-ideale-di-corrente-sinusoidale/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# Generatore ideale di corrente - AC

</div>



# [[Generatore ideale di corrente sinusoidale\|Generatore ideale di corrente sinusoidale]]

```ad-Definizione
title: Generatore ideale di corrente sinusoidale

![Generatore ideale di corrente sinusoidale 2024-06-20 11.57.14.excalidraw.png](/img/user/Excalidraw/Generatore%20ideale%20di%20corrente%20sinusoidale%202024-06-20%2011.57.14.excalidraw.png)
%%[[Generatore ideale di corrente sinusoidale 2024-06-20 11.57.14.excalidraw.md|🖋 Edit in Excalidraw]]%%

Un **generatore ideale di corrente** è un [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipolo]] attivo che impone ai morsetti una corrente [[13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale|sinusoidale]]:
$
i(t) = j(t) = I_{M}\sin(\omega t+\beta) = \sqrt{2} I \sin(\omega t+\beta) \qquad\forall i(t)
$
- $j(t)$ è detta **corrente sinusoidale impressa**

```

Più comunemente la tensione impressa si esprime con il rispettivo [[13 - Funzioni sinusoidali e fasori - ET#Fasore|fasore]]:
$
\overline{I_{s}} = Ie^{j\beta}
$




</div></div>

### Bipoli passivi ideali in regime sinusoidale

| Proprietà                                                                      | [[Resistore\|Resistore]] $R$                         | [[Induttore\|Induttore]] $L$                         | [[Condensatore\|Condensatore]] $C$                         |
| ------------------------------------------------------------------------------ | ----------------------------------------- | ----------------------------------------- | -------------------------------------------- |
|                                                                                | ![Resistore sinusoidale.excalidraw.png](/img/user/Excalidraw/Resistore%20sinusoidale.excalidraw.png) | ![Induttore sinusoidale.excalidraw.png](/img/user/Excalidraw/Induttore%20sinusoidale.excalidraw.png) | ![Condensatore sinusoidale.excalidraw.png](/img/user/Excalidraw/Condensatore%20sinusoidale.excalidraw.png) |
| Caratteristica esterna                                                         | $$v(t) = Ri(t)$$                          | $$v(t) = L\frac{di(t)}{dt}$$              | $$i(t) = C\frac{dv(t)}{dt}$$                 |
| Reattanza                                                                      | $$-$$                                     | $$X_{L}= \omega L$$                       | $$X_{C}= - \frac{1}{\omega C}$$              |
| $$\frac{V_{M}}{I_{M}} = \frac{V}{I}$$                                          | $$R$$                                     | $$X_L$$                                   | $$X_C$$                                      |
| [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|Sfasamento]] - $\varphi$ | $$0$$                                     | $$\frac{\pi}{2}$$                         | $$-\frac{\pi}{2}$$                           |
| [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|Potenza attiva]] - $P$                              | $$RI^2$$                                  | $$0$$                                     | $$0$$                                        |
| [[#Potenza reattiva]] - $Q$                                                    | $$0$$                                     | $$X_LI^2$$                                | $$X_CI^2$$                                   |
| [[#Potenza apparente]] - $S$                                                   | $$RI^2$$                                  | $$\|X_L\|I^2$$                            | $$\|X_C\|I^2$$                               |
| $$\dot{Z} =\frac{\overline{V}}{\overline{I}}$$                                 | $$R$$                                     | $$jX_L= j\omega L$$                       | $$jX_{C} = - \frac{j}{\omega C}$$            |



#### Resistore ideale passivo


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/resistore/#regime-sinusoidale" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Regime sinusoidale

![Resistore sinusoidale.excalidraw.png](/img/user/Excalidraw/Resistore%20sinusoidale.excalidraw.png)


```ad-Definizione
title: 

In regime sinusoidale il [[#Resistore]] di [[04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica|resistenza]] $R$ ([[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore\|convenzionato da utilizzatore]]) rispetta, in qualunque istante, la seguente relazione:
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



</div></div>


#### Induttore ideale


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/induttore/#regime-sinusoidale" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Regime sinusoidale


![Induttore sinusoidale.excalidraw.png](/img/user/Excalidraw/Induttore%20sinusoidale.excalidraw.png)


L'[[Induttore\|Induttore]], [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore\|convenzionato da utilizzatore]], dotato di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Induttanza\|#Induttanza]] costante $L$, rispetta sempre la relazione:
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

quindi la tensione, in un induttore a regime sinusoidale, si trova in *[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in anticipo]]* sulla corrente

![Induttore 2024-06-20 14.18.01.excalidraw.png](/img/user/Excalidraw/Induttore%202024-06-20%2014.18.01.excalidraw.png)


Si osservi che la tensione e la corrente sono legate dal prodotto
$
X_{L} = \omega L
$
che è definita [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#reattanza induttiva\|#reattanza induttiva]].

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




</div></div>


#### Condensatore ideale


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/condensatore/#regime-sinusoidale" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Regime sinusoidale

![Condensatore sinusoidale.excalidraw.png](/img/user/Excalidraw/Condensatore%20sinusoidale.excalidraw.png)


Il [[Condensatore\|Condensatore]], [[03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore|convenzionato da utilizzatore]], dotato di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Capacità\|#Capacità]] costante $C$, rispetta sempre la relazione:
$
i(t) = C \frac{dv(t)}{dt}
$
dove
- $v(t) = V_{M}\sin(\omega t+\alpha) = \sqrt{2} V\sin(\omega t+\alpha)$

da cui si ricava la legge della corrente:
$
i(t) = \omega C V_{M}\sin\left( \omega t + \beta + \frac{\pi}{2} \right) = I_{M}\sin\left( \omega t + \beta + \frac{\pi}{2} \right)
$
Valgono quindi le seguenti relazioni:

```ad-Teo
title:
$
\frac{V_{M}}{I_{M}} = \frac{V}{I} = \frac{1}{\omega C}  \qquad \varphi=\alpha-\beta= - \frac{\pi}{2}
$
```


quindi la tensione, in un induttore a regime sinusoidale, si trova in *[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in ritardo]]* sulla corrente.

![Condensatore 2024-06-20 14.29.31.excalidraw.png](/img/user/Excalidraw/Condensatore%202024-06-20%2014.29.31.excalidraw.png)


Si osservi che la tensione e la corrente sono legate dal prodotto
$
X_{C} =- \frac{1}{\omega C}
$
che viene definito [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Reattanza capacitiva\|#Reattanza capacitiva]]

La [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza istantanea]] assorbita è sinusoidale di ampiezza $VI$. In un quarto di periodo è positiva e da luogo a lavoro assorbito immagazzinato in forma di energia capacitiva: $w_{C}(t) = C \frac{v^{2}}{2}$ che viene poi restituita nel quarto di periodo successivo.

Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|fattore di potenza]] $\cos(\varphi) = 0$ è nullo e quindi [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] assorbita $P=0$
$
P= 0 \qquad Q=-A = -VI = X_{C}I^{2}
$

___

Il condensatore in regime sinusoidale può essere descritto anche facendo riferimento alle grandezze [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriali]].
$
\begin{align}
i(t) &\Longrightarrow \overline{I} = Ie^{j\beta} \\
v(t) &\Longrightarrow \overline{V} = Ve^{j\alpha}
\end{align}
$
Il rapporto tra i fasori vale:
$
\frac{\overline{V}}{\overline{I}} = \frac{V}{I}e^{j\varphi} = \frac{V}{I}e^{-j \frac{\pi}{2}} = -j \frac{1}{\omega C} = j X_{C}
$

Pertanto, in termini fasoriali, è vera la relazione:
$
\overline{V} = jX_{C}\overline{I}
$
immaginario puro

### Reattanza capacitiva

```ad-Definizione
title: Reattanza capacitiva ($X_{C}$)

La reattanza induttiva è definita come il prodotto
$
X_{C} = - \frac{1}{\omega C} \qquad \rm [F^{-1}s] = [\Omega]
$
e ha unità di misura omogenee con quella della [[04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica|resistenza]].

```




</div></div>


## Impedenza e Ammettenza


| Bipolo           |                                              |          Impedenza - $\dot Z$          | Ammettenza - $\dot Y$                  |
| ---------------- | -------------------------------------------- | :------------------------------------: | -------------------------------------- |
| [[Resistore\|Resistore]]    | ![Resistore sinusoidale.excalidraw.png](/img/user/Excalidraw/Resistore%20sinusoidale.excalidraw.png)    |          $$\dot{Z}_{R} = R$$           | $$\dot{Z}_{R} = \frac{1}{R}$$          |
| [[Induttore\|Induttore]]    | ![Induttore sinusoidale.excalidraw.png](/img/user/Excalidraw/Induttore%20sinusoidale.excalidraw.png)    |      $$\dot{Z}_{L} = j\omega L$$       | $$\dot{Z}_{L} = -j\frac{1}{\omega L}$$ |
| [[Condensatore\|Condensatore]] | ![Condensatore sinusoidale.excalidraw.png](/img/user/Excalidraw/Condensatore%20sinusoidale.excalidraw.png) | $$\dot{Z}_{C} = -j\frac{1}{\omega C}$$ | $$\dot{Z}_{C} = j\omega C$$            |


### Impedenza

```ad-Definizione
title: Impedenza

![14 - Reti in regime sinusoidale - ET 2024-06-20 15.18.32.excalidraw.png](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-20%2015.18.32.excalidraw.png)
%%[[14 - Reti in regime sinusoidale - ET 2024-06-20 15.18.32.excalidraw.md|🖋 Edit in Excalidraw]]%%

Preso un [[#Bipoli ideali in regime sinusoidale|bipolo lineare e passivo]] il quale sia [[03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore|convenzionato da utilizzatore]] si definisce **impedenza** il rapporto tra il [[13 - Funzioni sinusoidali e fasori - ET#Fasore|fasore]] di tensione e quello di corrente:
$
\dot Z = \frac{\overline{V}}{\overline{I}} = Ze^{j\varphi} \qquad \rm [\Omega]
$
dove
- $Z = \frac{V}{I}:$ [[13 - Funzioni sinusoidali e fasori - ET#Valore efficace|Valore efficace]] dato dal rapporto dei valori efficaci di tensione e corrente
- $\varphi:$ [[13 - Funzioni sinusoidali e fasori - ET#Sfasamento|Sfasamento]] tra tensione e corrente

Si misura in [[ohm]] - $\rm[\Omega]$.
```

Si ha chiaramente che:
$$
Z = \sqrt{\mathcal{Re}_{\dot Z}^{2}+ \mathcal{Im}_{\dot Z}^{2}} \qquad \varphi=\arctan\left( \frac{\mathcal{Im}_{\dot Z}}{\mathcal{Re}_{\dot Z}} \right)
$$

```ad-Teo
title: I Legge di Ohm Complessa

L'**impedenza** permette di generalizzare la [[I Legge di Ohm]]. Infatti, dati fasori di tensione ($\overline{V}$) e corrente ($\overline{I}$), e preso un bipolo qualunque di impedenza $\dot Z$, vale la relazione:
$
\overline{V} = \dot Z \overline{I}
$

```

#### Potenza assorbita dall'impedenza

Dato un bipolo di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|#Impedenza]] $\dot Z$, la sua [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza complessa\|#Potenza complessa]] è:
$$
\dot P = \overline{V} \, \overline{I}^{*} = \dot{Z}\overline{I}\,\overline{I}^{*} = (\mathcal{Re}_{\dot Z} + j\mathcal{Im}_{\dot Z})I^{2}
$$

da cui si ricava che:
$$
\begin{cases}
A &= ZI^{2} \quad &\text{Potenza apparente} \\
P &= \mathcal{Re}_{\dot Z}I^{2} \quad &\text{Potenza attiva} \\
Q &= \mathcal{Im}_{\dot Z}I^{2} \quad &\text{Potenza reattiva}
\end{cases}
$$



### Ammettenza


```ad-Definizione
title: Impedenza

![14 - Reti in regime sinusoidale - ET 2024-06-20 15.18.32.excalidraw.png](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-20%2015.18.32.excalidraw.png)
%%[[14 - Reti in regime sinusoidale - ET 2024-06-20 15.18.32.excalidraw.md|🖋 Edit in Excalidraw]]%%

Preso un [[#Bipoli ideali in regime sinusoidale|bipolo lineare e passivo]] il quale sia [[03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore|convenzionato da utilizzatore]] si definisce **impedenza** il rapporto tra il [[13 - Funzioni sinusoidali e fasori - ET#Fasore|fasore]] di corrente e quello di tensione:
$
\dot Y = \frac{\overline{I}}{\overline{V}} = Ye^{-j\varphi} \qquad \rm [S]
$
dove
- $Y = \frac{V}{I}:$ [[13 - Funzioni sinusoidali e fasori - ET#Valore efficace|Valore efficace]] dato dal rapporto dei valori efficaci di corrente e tensione
- $\varphi:$ [[13 - Funzioni sinusoidali e fasori - ET#Sfasamento|Sfasamento]] tra tensione e corrente

Si misura in [[siemens]] - $\rm[S]$.

```

L'ammettenza è il reciproco dell'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|#Impedenza]]
$$
\dot{Y} = \frac{1}{\dot Z}
$$



# Reti di bipoli passivi

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

Data una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] fatta di [[Generatore di corrente\|Generatore di corrente]] e [[Generatore di tensione\|Generatore di tensione]] e [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Bipoli passivi ideali in regime sinusoidale\|#Bipoli passivi ideali in regime sinusoidale]], se a tutti i bipoli si sostituiscono le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenze]] equivalenti, si applicano tutte le leggi viste per le reti in regime stazionario ([[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]], [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]], Metodi di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|risoluzione]]), trattando le impedenze come resistenze.