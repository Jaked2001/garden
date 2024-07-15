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
- **Parte reale** della potenza complessa = [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|#Potenza attiva - reale]]
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
| [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|#Potenza reattiva]] - $Q$                                                    | $$0$$                                     | $$X_LI^2$$                                | $$X_CI^2$$                                   |
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
Essendo $\varphi=0$ poiché tensione e corrente risultano in fase.



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

Quindi la tensione, in un induttore a regime sinusoidale, si trova in *[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in anticipo]]* sulla corrente

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

Data una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] fatta di [[Generatore di corrente\|Generatore di corrente]] e [[Generatore di tensione\|Generatore di tensione]] e [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Bipoli passivi ideali in regime sinusoidale\|#Bipoli passivi ideali in regime sinusoidale]], se a tutti i bipoli si sostituiscono le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenze]] equivalenti, si applicano tutte le leggi viste per le reti in regime stazionario ([[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]], [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]], Metodi di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|risoluzione]]), trattando le impedenze come resistenze. 

Ammesso di sostituire a ogni bipolo l'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|#Impedenza]] equivalente e di usare il valore dell'impedenza come fosse una resistenza, valgono le regole di:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Resistori in serie\|Resistori in serie]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Resistori in parallelo\|Resistori in parallelo]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Trasformazione triangolo-stella\|Trasformazione triangolo-stella]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Trasformazione stella-triangolo\|Trasformazione stella-triangolo]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Metodo di analisi delle reti lineari\|Metodi di analisi delle reti lineari]]

## Serie RL

![14 - Serie RL - ET 2024-06-26 11.58.35.excalidraw.png](/img/user/Excalidraw/14%20-%20Serie%20RL%20-%20ET%202024-06-26%2011.58.35.excalidraw.png)


Si considerino un [[Resistore\|Resistore]] e un [[Induttore\|Induttore]] in serie. Le cadute di tensione di ognuno dei due bipoli si trovano come:
$$
\overline{V}_{R} = R \overline{I} \qquad \overline{V}_{L} = j\omega L \overline{I} 
$$
Ai morsetti si misura una ddp:
$$
v(t) = \sqrt{2}V\sin(\omega t) = Ri(t) + L \frac{di(t)}{t}
$$
che in notazione [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriale]] diventa:
$$
\overline{V} = R\overline{I} + j\omega L \overline{I} = (R + j\omega L) \overline{I}
$$

![14 - Reti in regime sinusoidale - ET 2024-06-26 12.06.53.excalidraw.png](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-26%2012.06.53.excalidraw.png)


In particolare lo [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|sfasamento]] tra $\overline{V}$ e $\overline{I}$ è
$$
\varphi = \varphi_{v} - \varphi_{i}
$$
Pertanto, l'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|#Impedenza]] equivalente diventa:
$$
\dot{Z} = R+i\omega L = \frac{\overline{V}}{\overline{I}} = \frac{Ve^{j\varphi_{v}}}{Ie^{j\varphi_{i}}} = \frac{V}{I} e^{j(\varphi_{v}-\varphi_{i})} = \frac{V}{I} e^{j\varphi} = Ze^{j\varphi}
$$
- $\overline{V}$ è in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|anticipo]] rispetto a $\overline{I}$
- $\overline{I}$ è in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|ritardo]] rispetto a $\overline{V}$



## Serie RC

## Serie RLC

#UNI/ET/Domanda 

![14 - Serie RLC.excalidraw.png](/img/user/Excalidraw/14%20-%20Serie%20RLC.excalidraw.png)


Di ogni bipolo si scrive l'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|#Impedenza]] corrispondente:
$$
\begin{align}
Z_{R} &= R \\
Z_{L} &= j\omega L = jX_{L} \\
Z_{C} &= -j \frac{1}{\omega C} = jX_{C}
\end{align}
$$
A questo punto, la serie si può sostituire con un bipolo equivalente la cui impedenza valga:
$$
\dot Z_{s} = \dot Z_{R} + \dot Z_{L} + \dot Z_{C}
$$
Vale ancora la formula del [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Partitore di tensione\|partitore di tensione]] applicato usando l'impedenza al posto della resistenza.


### Risonanza in serie

È dato un circuito alimentato da un [[Generatore ideale di tensione sinusoidale\|Generatore ideale di tensione sinusoidale]] e 3 bipoli in serie:
- Un [[Resistore\|resistore]]
- Un [[Induttore\|induttore]]
- Un [[Condensatore\|Condensatore]]

![14 - Reti in regime sinusoidale - ET 2024-06-21 18.40.54.excalidraw.png](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-21%2018.40.54.excalidraw.png)


Si scrive la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]]:
$$
\begin{align}
\overline{E}_{s} &= \overline{V}_{R} + \overline{V}_{L} + \overline{V}_{C} \\
&= \left(  R + j\omega L - \frac{j}{\omega C} \right) \overline{I} = \\
&= \left[  R + j \left(X_{L}-X_{C} \right) \right] \overline{I} \\
&= (R+jX)\overline{I}
\end{align}
$$
essendo $X=X_{L}-X_{C}$


Si ha pertanto l'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|#Impedenza]] equivalente data dalla [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RLC\|#Serie RLC]]:
$$
\begin{align}
\dot Z &= \dot Z_{R} + \dot Z_{L} + \dot Z_{C} =  \\
&= R + j \left( \omega L - \frac{1}{\omega C} \right)
\end{align}
$$
$\dot Z$ ha modulo e argomento rispettivamente pari a:
$$
Z(\omega) = \sqrt{R^{2} + \left( \omega L - \frac{1}{\omega C} \right)^{2}}
\qquad;\qquad
\varphi(\omega) = \arctan\left(  \frac{\omega L - \frac{1}{\omega C}}{R}  \right)
$$
La corrente sarà data da:
$$
\overline{I} = \frac{\overline{V}}{\dot{Z}} = \frac{V}{Z}e^{-j\varphi} = Ie^{-j\varphi}
$$
essendo quindi $\varphi$ lo [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|sfasamento]] tra tensione e corrente

#### Condizione di risonanza

La condizione di risonanza si ha quando $X=0$, ovvero per la pulsazione $\omega$ tale che le reattanze [[Induttore#Reattanza induttiva\|induttiva]] e [[Condensatore#Reattanza capacitiva\|capacitiva]] siano uguali in modulo:
$$
\omega_{0} \quad \text{ t.c. } \quad j\omega L = j \frac{1}{\omega C}
$$
In particolare si ottiene che
$$
\omega_{0} = \frac{1}{\sqrt{LC}}
$$



#### Comportamento Ohmico-Induttivo - Serie RLC

$$
\boldsymbol{\omega>\omega_{0} \quad - \quad X_{L}>X_{C} \quad - \quad \omega L> \frac{1}{\omega C} }
$$
In questo caso
$$
\varphi>0
$$
In questa condizione la [[Induttore#Reattanza induttiva\|reattanza induttiva]] prevale sulla [[Induttore#Reattanza induttiva\|reattanza induttiva]][[Condensatore#Reattanza capacitiva\|reattanza capacitiva ]] e la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RLC\|#Serie RLC]] si comporta come una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RL\|#Serie RL]].

Il circuito assume comportamento **Ohmico-Induttivo**. Mi aspetto:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|Fasore]] di corrente in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|ritardo]] rispetto a $\overline{V}$


In questa condizione,
$$
\overline{V}_{L} > \overline{V}_{C}
$$

Se si prende in considerazione la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]]:
$$
\overline{E}_{s} = \overline{V}_{R} + \overline{V}_{L} + \overline{V}_{C}
$$
e la si rappresenta su un diagramma fasoriale si ottiene infatti

![14 - Serie RLC comportamento Ohmico-Induttivo - ET 2024-06-27 12.05.08.excalidraw.png](/img/user/Excalidraw/14%20-%20Serie%20RLC%20comportamento%20Ohmico-Induttivo%20-%20ET%202024-06-27%2012.05.08.excalidraw.png)


Il diagramma è stato così ottenuto:
1. Traccio fasore $\color{green}\overline{I}$
2. Traccio fasore ${\color{red}\overline{V}_{R}} = R{\color{green}\overline{I}}$ in linea (in fase) con ${\color{green}\overline{I}}$
3. Sommo a $\color{red}\overline{V}_R$ il fasore ${\color{blue}\overline{V}_{L}}= j \omega L{\color{green}\overline{I}}$ a 90° rispetto a ${\color{red}\overline{V}_{R}}$ (si ricordi che la tensione, nell'[[Induttore\|induttore]] si trova in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in anticipo]] rispetto alla corrente)
4. Sommo a ${\color{blue}\overline{V}_{L}}$ il fasore ${\color{pink}\overline{V}_{C}} = -j \dfrac{1}{\omega C}{\color{green}\overline{I}}$ allineato con ${\color{blue}\overline{V}_{L}}$ ma diretto nel verso opposto (ricordo che ${\color{pink}\overline{V}_{C}}<{\color{blue}\overline{V}_{L}}$)
Si ottiene così il fasore di ${\color{orange}\overline{V}}$ come somma di tutte le cadute di tensione e si osserva, come previsto, che ${\color{green}\overline{I}}$ appare in ritardo rispetto a ${\color{orange}\overline{V}}$.

#### Comportamento Ohmico-Capacitivo - Serie RLC

$$
\boldsymbol{\omega<\omega_{0} \quad - \quad X_{L}<X_{C} \quad - \quad \omega L<\frac{1}{\omega C} }
$$
In questo caso
$$
\varphi<0
$$

In questa condizione la [[Condensatore#Reattanza capacitiva\|reattanza capacitiva ]] prevale sulla [[Induttore#Reattanza induttiva\|reattanza induttiva]] e la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RLC\|#Serie RLC]] si comporta come una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RC\|#Serie RC]].

Il circuito assume comportamento **Ohmico-Capacitivo**. Mi aspetto:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|Fasore]] di corrente in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|anticipo]] rispetto a $\overline{V}$


In questa condizione,
$$
\overline{V}_{L} < \overline{V}_{C}
$$

Se si prende in considerazione la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]]:
$$
\overline{E}_{s} = \overline{V}_{R} + \overline{V}_{L} + \overline{V}_{C}
$$
e la si rappresenta su un diagramma fasoriale si ottiene infatti

![14 - Serie RLC comportamento Ohmico-Capacitivo - ET 2024-06-27 12.22.03.excalidraw.png](/img/user/Excalidraw/14%20-%20Serie%20RLC%20comportamento%20Ohmico-Capacitivo%20-%20ET%202024-06-27%2012.22.03.excalidraw.png)


Il diagramma è stato così ottenuto:
1. Traccio fasore $\color{green}\overline{I}$
2. Traccio fasore ${\color{red}\overline{V}_{R}} = R{\color{green}\overline{I}}$ in linea (in fase) con ${\color{green}\overline{I}}$
3. Sommo a $\color{red}\overline{V}_R$ il fasore ${\color{pink}\overline{V}_{C}}= -j \dfrac{1}{\omega C}{\color{green}\overline{I}}$ a 90° rispetto a ${\color{red}\overline{V}_{R}}$
4. Sommo a ${\color{pink}\overline{V}_{C}}$ il fasore ${\color{blue}\overline{V}_{C}} = -j \omega L{\color{green}\overline{I}}$ allineato con ${\color{pink}\overline{V}_{C}}$ ma diretto nel verso opposto (ricordo che ${\color{pink}\overline{V}_{C}}>{\color{blue}\overline{V}_{L}}$)
Si ottiene così il fasore di ${\color{orange}\overline{V}}$ come somma di tutte le cadute di tensione e si osserva, come previsto, che ${\color{green}\overline{I}}$ appare in anticipo rispetto a ${\color{orange}\overline{V}}$.

#### Comportamento in risonanza - Serie RLC

$$
\boldsymbol{\omega=\omega_{0} \quad - \quad X_{L}=X_{C} \quad - \quad \omega L=\frac{1}{\omega C} }
$$
In questo caso
$$
\varphi=0
$$

In questa condizione la [[Condensatore#Reattanza capacitiva\|reattanza capacitiva ]] eguaglia la [[Induttore#Reattanza induttiva\|reattanza induttiva]] e la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RLC\|#Serie RLC]] si comporta come una rete puramente resistiva.

Il circuito assume comportamento puramente **Ohmico**. Mi aspetto:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|Fasore]] di corrente in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|fase]] con $\overline{V}$

In questa condizione,
$$
\overline{V}_{L} = \overline{V}_{C}
$$

Se si prende in considerazione la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]]:
$$
\overline{E}_{s} = \overline{V}_{R} + \overline{V}_{L} + \overline{V}_{C}
$$
e la si rappresenta su un diagramma fasoriale si ottiene infatti

Scrivo $\overline{V}_L$:
$$
\overline{V}_{L} = j \sqrt{\frac{L}{C}} \overline{I} 
$$
Scrivo $\overline{V}_{C}$
$$
\begin{align}
\overline{V}_{C} &= -j \frac{1}{\omega_{0} C} = \\
&= -j \frac{\sqrt{LC}}{1} \frac{1}{C} = -j \sqrt{\frac{L}{C}} \overline{I}
\end{align}
$$

![14 - Serie RLC Comportamento in risonanza - ET 2024-06-27 12.28.00.excalidraw.png](/img/user/Excalidraw/14%20-%20Serie%20RLC%20Comportamento%20in%20risonanza%20-%20ET%202024-06-27%2012.28.00.excalidraw.png)


Si noti quindi come, dall'esterno, gli effetti dei bipoli della [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RLC\|#Serie RLC]] in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Condizione di risonanza\|#Condizione di risonanza]], siano equivalenti a quelli di un circuito costituito esclusivamente da un [[Generatore ideale di tensione sinusoidale\|Generatore ideale di tensione - AC]] e un [[Resistore\|resistore]].

Si può quindi ricavare $\overline{I}$ come
$$
\overline{I} = \frac{\overline{E}_{s}}{R}
$$
che sostituiamo nelle espressioni delle cadute di tensione di induttore e condensatore:
$$
\begin{align}
\overline{V}_{L} &= j \sqrt{\frac{L}{C}} \frac{\overline{E_{s}}}{R} \\
\overline{V}_{C} &= -j \sqrt{\frac{L}{C}} \frac{\overline{E_{s}}}{R}
\end{align}
$$
si definisce il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di merito\|#Fattore di merito]]:

##### Fattore di merito

```ad-Definizione
title: Fattore di merito o fattore di qualità ($Q_{0}$)

Si definisce **fattore di merito** la quantità
$
Q_{0} = \sqrt{\frac{L}{C}} \frac{1}{R}
$
e rappresenta il rapporto tra la caduta di tensione di un [[Induttore\|Induttore]] o un [[Condensatore\|Condensatore]] e la tensione impressa in un circuito [[#Serie RLC]] in [[#Comportamento in risonanza - Serie RLC|risonanza]].
$
Q_{0} = \frac{V_{L}}{E_{s}} = \frac{V_{C}}{E_{S}}
$


```

Il fattore di merito può essere:
- $Q_{0}<1:$ condizione normale, in cui le cadute di tensione sono minori della tensione impressa
- $Q_{0}>1:$ Condizione in cui la tensione sull'induttore o sul condensatore sono in valore efficace maggiore dalla tensione erogata dal generatore
- $Q_{0}\to \infty$ se ho un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Cortocircuito\|cortocircuito]] sul resistore
	- Pericoloso perché tensione va a infinito e rischio di 
	- Utile per leggere tensioni molto molto piccole



## Parallelo RLC

#UNI/ET/Domanda 

![14 - Reti in regime sinusoidale - ET 2024-06-21 18.28.02.excalidraw.png](/img/user/Excalidraw/14%20-%20Reti%20in%20regime%20sinusoidale%20-%20ET%202024-06-21%2018.28.02.excalidraw.png)


Di ogni bipolo si scrive l'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Ammettenza\|#Ammettenza]] corrispondente:
$$
\begin{align}
\dot Y_{R} &= \frac{1}{R} \\
\dot Y_{L} &= -j\frac{1}{\omega L} = - j \frac{1}{X_{L}} \\
\dot Y_{C} &= j{\omega C} = - j \frac{1}{X_{L}} \\
\end{align}
$$
A questo punto, il parallelo si può sostituire con un bipolo equivalente la cui ammettenza valga:
$$
\dot Y_{p} = \dot Y_{R} + \dot Y_{L} + \dot Y_{C}
$$


### Risonanza in parallelo - antirisonanza

Antirisonanza

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

## Rifasamento monofase

#UNI/ET/Domanda 

È dato un circuito [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Serie RL\|#Serie RL]]:

![14 - Rifasamento - rete RL - ET 2024-06-27 17.48.52.excalidraw.png](/img/user/Excalidraw/14%20-%20Rifasamento%20-%20rete%20RL%20-%20ET%202024-06-27%2017.48.52.excalidraw.png)


Si può ridisegnare il circuito tenendo conto dell'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|#Impedenza]] equivalente della sere.
$$
\dot{Z} = R + j\omega L
$$
A questo tipo di carico sono associati:
- [[#Potenza attiva - reale]] positiva
- [[#Potenza reattiva]] positiva

Infatti, per il [[Resistore\|Resistore]]:
$$
P = VI \cos\varphi|_{\varphi_{R}=0}\ge 0  \qquad Q = 0
$$
Mentre per l'[[Induttore]]
$$
P = 0 \qquad Q = VI\sin\varphi|_{\varphi_{L}=90°} = VI = j\omega L I^{2} \ge 0
$$

Il carico pertanto sta assorbendo sia potenza attiva che potenza reattiva.

Si rappresentano sul diagramma fasoriale la tensione $\overline{V} = \overline{E}_{s}$ e la corrente $\overline{I}$ del circuito:

![14 - Rifasamento - Serie RL - Diagramma fasoriale - ET 2024-06-27 18.01.37.excalidraw.png](/img/user/Excalidraw/14%20-%20Rifasamento%20-%20Serie%20RL%20-%20Diagramma%20fasoriale%20-%20ET%202024-06-27%2018.01.37.excalidraw.png)


La corrente è in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|ritardo]] rispetto alla tensione di un angolo $\varphi$. Si osservi come la corrente possa essere scomposta in 2 componenti una in fase e una in quadratura con la tensione:
- $\overline{I}_{f}:$ Componente della corrente in **fase**
- $\overline{I}_{q}:$ Componente della corrente in **quadratura**

La potenza $P$ associata alle perdite di tipo Ohmico (dissipazioni), si può esprimere come [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule\|potenza dissipata per effetto Joule]]:
$$
P = RI^{2}
$$
dove questa $I$ corrisponde alla *componente corrente in fase* con la tensione:
$$
P = RI^{2}_{f}
$$
Su un impianto elettrico, la corrente che viene effettivamente usata (in termini di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valore efficace]]) è effettivamente $I$. L'erogatore della corrente (tipo [[eni\|eni]]) però, dal contatore, è capace di registrare solamente la corrente in fase che viene "consumata". Pertanto esso ha interesse a far si che la quota parte più grande possibile di $I$ sia in $I_{f}$, ovvero che $\cos\varphi\sim 1$: questo corrisponde a massimizzare il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|#Fattore di potenza]].

Di solito, per utenze civili, si cerca portare il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|#Fattore di potenza]] a:
$$
\cos\varphi\ge 0.95
$$
L'operazione che permette di ottenere ciò è detta rifasamento.
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Rifasamento con condensatore\|#Rifasamento con condensatore]]

È chiaramente fondamentale che il comportamento della rete, per l'utenza, rimanga totalmente invariato dal punto di vista di correnti e tensioni.

### Rifasamento con condensatore

Generalmente il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Rifasamento monofase\|#Rifasamento monofase]] si effettua con il [[Condensatore]]. Infatti, se vado ad aggiungere al circuito una potenza reattiva addizionale, che porti a una diminuzione della componente di corrente in quadratura.

Vediamo cosa succede se al circuito [[14 - Rifasamento - rete RL - ET 2024-06-27 17.48.52.excalidraw.png]] aggiungo un condensatore in parallelo.

![14 - Rifasamento con condensatore - ET 2024-06-27 18.14.42.excalidraw.png](/img/user/Excalidraw/14%20-%20Rifasamento%20con%20condensatore%20-%20ET%202024-06-27%2018.14.42.excalidraw.png)


A questo punto, si ha, per la [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]]:
$$
\overline{I}' = \overline{I}_{C}+\overline{I}
$$
Vediamo quindi il diagramma fasoriale (si pone sempre la tensione adagiata sull'asse reale):

![14 - Rifasamento con condensatore - Diagramma fasoriale - ET 2024-06-27 18.19.51.excalidraw.png](/img/user/Excalidraw/14%20-%20Rifasamento%20con%20condensatore%20-%20Diagramma%20fasoriale%20-%20ET%202024-06-27%2018.19.51.excalidraw.png)


Quando si aggiunge la corrente $\overline{I}_{C}$, essendo questa in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in anticipo]] rispetto alla tensione, si andrà a sottrarre alla componente in quadratura della corrente. Si ottiene così un nuovo fasore di corrente $\overline{I}'$ molto più simile alla componente in fase della corrente.

Rimane ora da **dimensionare** il condensatore in modo da ottenere il giusto rifasamento.

Si ricorda essere
$$
\overline{V} = -j \frac{1}{\omega C} \overline{I} \qquad\Longrightarrow\qquad I_{C} = \omega C V 
$$
In termini di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valori efficaci]] si impone:
$$
\begin{align}
I_{q} &= I_{q}' + I_{C} = \\
\underbrace{VI\sin(\varphi)}_{Q} &= \underbrace{VI'\sin(\varphi')}_{Q'} + \omega CV^{2} 
\end{align}
$$
dove:
- $Q =VI\sin(\varphi):$ Potenza reattiva prima del rifasamento
- $Q =VI'\sin(\varphi'):$ Potenza reattiva dopo il rifasamento
L'espressione sopra diventa quindi:
$$
Q = Q' + \omega C V^{2}
$$
dove $\varphi'$ si può ricavare dal [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|#Fattore di potenza]] obiettivo del rifasamento:
$$
\cos(\varphi')= 0.95
$$
```ad-Teo
title: Capacità per rifasamento monofase

Pertanto, la [[Condensatore#Capacità|capacità]] del condensatore necessario al rifasamento sarà:
$
C = \frac{Q-Q'}{\omega V^{2}} \qquad\rm [F]
$

```

Solitamente si considerano le potenze attive. Conoscendo il rapporto tra $P$ e $Q$ si può comunque calcolare la capacità:
$$
\frac{P}{Q} = \frac{VI\cos(\varphi)}{VI\sin(\varphi)} = \frac{1}{\tan(\varphi)}
$$
inoltre
$$
I_{f} = I\cos(\varphi) = I_{f}' = I'\cos(\varphi')
$$
quindi, ricordando che la potenza attiva si è conservata: $P=P'$
$$
C = \frac{Q-Q'}{\omega V^{2}} = \frac{P\tan(\varphi)-P'\tan(\varphi')}{\omega V^{2}} = P\frac{\tan(\varphi)-\tan(\varphi')}{\omega V^{2}} \qquad\rm [F]
$$


### Rifasamento con resistore


❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

## Mutuo accoppiamento


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/induttore/#mutuo-accoppiamento" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



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

Si può definire il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Coefficiente di mutuo accoppiamento\|#Coefficiente di mutuo accoppiamento]]
$
M_{12} = M_{21} = M
$


![Induttore 2024-06-22 11.42.03.excalidraw.png](/img/user/Excalidraw/Induttore%202024-06-22%2011.42.03.excalidraw.png)


Gli induttori in figura sono mutualmente accoppiati con [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Coefficiente di mutuo accoppiamento\|#Coefficiente di mutuo accoppiamento]] pari a $M$. Si possono pertanto scrivere le equazioni:
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


