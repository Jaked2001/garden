---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/13-funzioni-sinusoidali-e-fasori-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET\|13 - Funzioni sinusoidali e fasori - ET]]

## Funzione sinusoidale

```ad-Definizione
title: Funzione sinusoidale

![13 - Funzioni sinusoidali e fasori - ET 2024-06-18 18.05.01.excalidraw.png](/img/user/Excalidraw/13%20-%20Funzioni%20sinusoidali%20e%20fasori%20-%20ET%202024-06-18%2018.05.01.excalidraw.png)
%%[[13 - Funzioni sinusoidali e fasori - ET 2024-06-18 18.05.01.excalidraw.md|🖋 Edit in Excalidraw]]%%

Una **funzione sinusoidale** nel tempo è esprimibile come
$
a(t) = A_{M}\sin(\omega t+\alpha)
$
dove:
- $A_{M}:$ **Ampiezza**
- $\omega:$ **Pulsazione** $\rm \left[\frac{rad}{s}\right]$
- $\alpha:$ **Fase iniziale** $\rm[rad]$
- $T = \frac{1}{f}:$ Periodo
- $f:$ frequenza $[\rm Hz]$

```

In una funzione sinusoidale vale sempre la relazione:
$$
\omega T = 2\pi
$$
Si possono quindi scrivere delle relazioni che legano frequenza, periodo e pulsazione:
$$
T = \frac{1}{f} = \frac{2\pi}{\omega}
\qquad
f = \frac{1}{T} = \frac{\omega}{2\pi}
\qquad
\omega=2\pi f = \frac{2\pi}{T}
$$
La funzione sinusoidale è un caso particolare di [[Funzione periodica\|Funzione periodica]], ossia una funzione $a(t)$ tale che
$$
a(t) = a(t+nT) \quad \forall n\in \mathbb{Z}
$$
### Valore efficace

Il **valore efficace** di una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|#Funzione sinusoidale]] è la media quadratica in un periodo:
$$
A \stackrel{\triangle}{=} \sqrt{\frac{1}{T}\int_{T} a^{2}(t) \, dt} = \frac{A_{M}}{\sqrt{2}}
$$
## Funzioni sinusoidali isofrequenziali

```ad-Definizione
title: Funzioni sinusoidali isofrequenziali

Le funzioni sinusoidali si dicono **isofrequenziali** quando sono dotate di uguale frequenza.

```

Siano
$$
\begin{align}
a(t) &= A_{M}\sin(\omega_{a} t+\alpha) \\
b(t) &= B_{M}\sin(\omega_{b} t+\beta)
\end{align}
$$
sono isofrequenziali se e solo se.
$$
\omega_{a} = \omega_{b}
$$

### Sfasamento

Lo **sfasamento** è la differenza di fase tra 2 [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzioni sinusoidali isofrequenziali\|#Funzioni sinusoidali isofrequenziali]].

Siano
$$
\begin{align}
a(t) &= A_{M}\sin(\omega t+\alpha) \\
b(t) &= B_{M}\sin(\omega t+\beta)
\end{align}
$$
due [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzioni sinusoidali isofrequenziali\|#Funzioni sinusoidali isofrequenziali]], lo **sfasamento** è
$$
\varphi = \alpha-\beta
$$
Sono possibili diverse situazioni:
- $\varphi=0:$ $a(t)$ e $b(t)$ sono dette **in fase**
- $\varphi>0:$ $a(t)$ **in anticipo** rispetto a $b(t)$
- $\varphi<0:$ $a(t)$ **in ritardo** rispetto a $b(t)$

Inoltre, ci sono alcuni casi particolari:
- $\varphi = \pm \pi:$ le funzioni sono dette in **opposizione di fase**
- $\varphi = + \frac{\pi}{2}:$ $a(t)$ è **in quadratura in anticipo** rispetto a $b(t)$
- $\varphi = - \frac{\pi}{2}:$ $a(t)$ è **in quadratura in ritardo** rispetto a $b(t)$

## Metodo simbolico

Detto anche **"Trasformazione di Steinmetz-Kennedy"**.

In [[Università/3° Anno/2° Semestre/Elettrotecnica/🔌 Elettrotecnica\|🔌 Elettrotecnica]] è spesso necessario eseguire numerose operazioni tra tensioni e correnti. Quando queste sono descritte da [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|funzioni sinusoidali]] le operazioni (somma algebrica, moltiplicazione per uno scalare, derivazione temporale), seppure concettualmente semplici, possono diventare onerose da eseguire. È possibile, sotto alcune ipotesi, creare una corrispondenza biunivoca tra funzioni sinusoidali e numeri complessi che permette di semplificare i conti.

```ad-tip
title: Ipotesi

- Tutte le grandezze devono essere [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzioni sinusoidali isofrequenziali\|#Funzioni sinusoidali isofrequenziali]]
- Tutti i [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipoli]] sono lineari


```

### Fasore

```ad-Definizione
title: Fasore ($\overline{A}$)

Un **fasore** è un numero complesso associato a una [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|#Funzione sinusoidale]] secondo la trasformazione del [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Metodo simbolico\|#Metodo simbolico]].

Data la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|#Funzione sinusoidale]]
$
a(t) = A_{M}\sin(\omega t + \alpha) = \sqrt{2} A \sin(\omega t + \alpha)
$
le associo un numero complesso che abbia:
- Modulo pari al [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|#Valore efficace]] $A$
- Argomento pari alla fase iniziale $\alpha$
Si ottiene quindi:
$
\overline{A} \stackrel{\triangle}{=} Ae^{j\alpha}
$
che è stato espresso con la notazione esponenziale.

```

Quando si mettono a confronto fasori diversi, è chiaro che le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|funzioni sinusoidali]] da cui hanno origine devono essere necessariamente [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzioni sinusoidali isofrequenziali\|isofrequenziali]] (come specificato anche nelle ipotesi del [[#Metodo simbolico]]). Altrimenti queste avrebbero pulsazioni diverse. Si noti infatti che, in ogni caso, nell'espressione del fasore non compare la pulsazione.

#### Espressioni dei fasori

##### Notazione trigonometrica

```ad-Definizione
title: Notazione trigonometrica

Dato un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|#Fasore]] $\overline{A} = Ae^{j\alpha}$, questo, mediante la [[Formula di Eulero]], può essere espresso in **notazione trigonometrica**:
$
\overline{A} = Ae^{j\alpha} = A(\cos(\alpha) + j\sin(\alpha))
$

```


##### Notazione cartesiana

```ad-Definizione
title: Notazione cartesiana

Dato un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|#Fasore]] $\overline{A} = Ae^{j\alpha}$, questo, a partire dalla [[#Notazione trigonometrica]], può essere espresso in **notazione cartesiana**:
$
\begin{align}
\overline{A} = Ae^{j\alpha} &= A\cos(\alpha) + jA\sin(\alpha) = \\
&=\mathcal{Re}_{A} + j \mathcal{Im}_{A} 
\end{align}
$

```

Valgono le seguenti relazioni
$$
\begin{cases}
\mathcal{Re}_{A} &= A\cos(\alpha) \\
\mathcal{Im}_{A} &= A\sin(\alpha)
\end{cases}
\quad\iff\quad
\begin{cases}
A &= \sqrt{\mathcal{Re}^{2}_{A} + \mathcal{Im}_{A}^{2}} \\
\alpha &=   \arctan2\left(\dfrac{\mathcal{Re}_{A}}{\mathcal{Im}_{A}} \right)
\end{cases}
$$
dove per ricavare la fase si è usata l'[[Università/3° Anno/2° Semestre/Topografia e Positioning/allegati/arcotangente2\|arcotangente2]].

#### Rappresentazione grafica dei fasori

![13 - Funzioni sinusoidali e fasori - ET 2024-06-19 11.04.55.excalidraw.png](/img/user/Excalidraw/13%20-%20Funzioni%20sinusoidali%20e%20fasori%20-%20ET%202024-06-19%2011.04.55.excalidraw.png)


Un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|#Fasore]], in quanto rappresentato da un numero immaginario, può essere rappresentato sul [[Piano di Gauss\|Piano di Gauss]] dove:
- La **parte reale** si trova sulle ascisse
- La **parte immaginaria** si trova sulle ordinate

I fasori, sul piano di Gauss, sono rappresentati come vettori, aventi
- **Origine** nell'origine degli assi
- **Lunghezza** pari al [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|#Valore efficace]] $A$
- **Angolo con le ascisse** pari alla fase iniziale $\varphi$

Sullo stesso piano sono raffigurabili anche più fasori, ammesso che questi rappresentino [[#Funzioni sinusoidali isofrequenziali]].

![13 - Funzioni sinusoidali e fasori - ET 2024-06-19 11.12.07.excalidraw.png](/img/user/Excalidraw/13%20-%20Funzioni%20sinusoidali%20e%20fasori%20-%20ET%202024-06-19%2011.12.07.excalidraw.png)


La rappresentazione grafica permette di visualizzare immediatamente le relazioni tra i fasori, soprattutto per quanto riguarda lo [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|#Sfasamento]].

Nel diagramma sopra, essendo $\beta-\alpha=\varphi>0$, si può affermare che il fasore $\overline{B}$ è in **anticipo** rispetto al fasore $\overline{A}$.
- Ruotato in senso **antiorario** = [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|#Sfasamento]] in anticipo
- Ruotato in senso **orario** = [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|#Sfasamento]] in ritardo

#### Operazioni tra fasori

##### Somma

Sono date due [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|sinusoidi]]:
$$
\begin{align}
a(t) &= \sqrt{2}A\sin{(\omega t+\alpha)} \\
b(t) &= \sqrt{2}B\sin{(\omega t+\beta)}
\end{align}
$$
e si vuole trovare la sinusoide
$$
c(t) = a(t) + b(t)
$$
in termini fasoriali.

Le due sinusoidi corrispondono rispettivamente ai fasori
$$
\begin{align}
\overline{A} &= Ae^{j\alpha} = A\cos(\alpha) + jA\sin(\alpha) = \mathcal{Re}_{A} + i\mathcal{Im}_{A} \\
\overline{B} &= Be^{j\alpha} = B\cos(\alpha) + jB\sin(\alpha) = \mathcal{Re}_{B} + i\mathcal{Im}_{B}
\end{align}
$$
Si vuole trovare il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|#Fasore]] somma:
$$
\overline{C} = \overline{A} +\overline{B} 
$$
Sostituendo:
$$
\begin{align}
\overline{C} &= \overline{A} +\overline{B} = \\
&= (\mathcal{Re}_{A} + i\mathcal{Im}_{A}) + (\mathcal{Re}_{B} + i\mathcal{Im}_{B})= \\
&= (\mathcal{Re}_{A} + \mathcal{Re}_{B}) + i(\mathcal{Im}_{A} + \mathcal{Im}_{B}) =\\
&= \mathcal{Re}_{C} + i\mathcal{Im}_{C}
\end{align}
$$
Da cui si ottiene
$$
\begin{align}
\mathcal{Re}_{C} &= C\cos(\gamma) = A\cos(\alpha) + B\cos(\beta) \\
\mathcal{Re}_{C} &= C\sin(\gamma) = A\sin(\alpha) + B\sin(\beta)
\end{align}
$$

Graficamente, la somma di due fasori corrisponde alla somma vettoriale di essi sul [[Piano di Gauss\|Piano di Gauss]]:

![13 - Funzioni sinusoidali e fasori - ET 2024-06-19 12.15.16.excalidraw.png](/img/user/Excalidraw/13%20-%20Funzioni%20sinusoidali%20e%20fasori%20-%20ET%202024-06-19%2012.15.16.excalidraw.png)


##### Prodotto per uno scalare

È data una [[#Funzione sinusoidale]]
$$
a(t) = \sqrt{2}A \sin(\omega t+\alpha)
$$
e si vuole trovare
$$
c(t) = ka(t)
$$
in termini fasoriali:

La sinusoide corrisponde al [[#Fasore]]:
$$
\overline{A} = Ae^{j\alpha} = A\cos(\alpha) + jA\sin(\alpha) = \mathcal{Re}_{A} + i\mathcal{Im}_{A}
$$
Dalla formula di $c(t)$ è evidente che:
$$
\overline{C} = k\overline{A}
$$

##### Rapporto

Sono date due [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|sinusoidi]]:
$$
\begin{align}
a(t) &= \sqrt{2}A\sin{(\omega t+\alpha)} \\
b(t) &= \sqrt{2}B\sin{(\omega t+\beta)}
\end{align}
$$
e si vuole trovare la sinusoide
$$
c(t) = \frac{a(t)}{b(t)}
$$
Le due sinusoidi corrispondono rispettivamente ai [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasori]]
$$
\begin{align}
\overline{A} &= Ae^{j\alpha} = A\cos(\alpha) + jA\sin(\alpha) = \mathcal{Re}_{A} + i\mathcal{Im}_{A} \\
\overline{B} &= Be^{j\beta} = B\cos(\beta) + jB\sin(\beta) = \mathcal{Re}_{B} + i\mathcal{Im}_{B}
\end{align}
$$
Sostituendo nell'equazione di $c(t)$ le rispettive quantità fasoriali
$$
\begin{align}
\overline{C} &= \frac{\overline{A}}{\overline{B}} = \\
&= \frac{Ae^{j\alpha}}{Be^{j\beta}} = \\
&= \frac{A}{B}e^{j(\alpha-\beta)} = \\
&= Ce^{j(\alpha-\beta)}
\end{align}
$$
##### Prodotto

Sono date due [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Funzione sinusoidale\|sinusoidi]]:
$$
\begin{align}
a(t) &= \sqrt{2}A\sin{(\omega t+\alpha)} \\
b(t) &= \sqrt{2}B\sin{(\omega t+\beta)}
\end{align}
$$
e si vuole trovare la sinusoide
$$
c(t) = a(t)b(t)
$$
Le due sinusoidi corrispondono rispettivamente ai [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasori]]
$$
\begin{align}
\overline{A} &= Ae^{j\alpha} = A\cos(\alpha) + jA\sin(\alpha) = \mathcal{Re}_{A} + i\mathcal{Im}_{A} \\
\overline{B} &= Be^{j\beta} = B\cos(\beta) + jB\sin(\beta) = \mathcal{Re}_{B} + i\mathcal{Im}_{B}
\end{align}
$$
Sostituendo nell'equazione di $c(t)$ le rispettive quantità fasoriali
$$
\begin{align}
\overline{C} &= \overline{A}\cdot\overline{B} = \\
&= Ae^{j\alpha}\cdot Be^{j\beta} = \\
&= ABe^{j(\alpha+\beta)} = \\
&= Ce^{j(\alpha+\beta)}
\end{align}
$$

Il prodotto di 2 fasori è dato da un [[#Fasore]] che ha per [[#Valore efficace]] il prodotto dei valori efficaci dei due fasori iniziali e per fase la somma delle fasi:
$$
\overline{A}\cdot\overline{B} = ABe^{j(\alpha+\beta)}
$$
##### Derivazione

È data una [[#Funzione sinusoidale]]
$$
a(t) = \sqrt{2}A \sin(\omega t+\alpha)
$$
e si vuole trovare
$$
c(t) =  \frac{d}{dt}a(t)
$$
Derivando l'espressione di $a(t)$
$$
\begin{align}
c(t) &= \frac{d}{dt}a(t) = \\
&= \sqrt{2}A\omega \cos(\omega t+\alpha) = \\
&= \sqrt{2}A\omega \sin\left( \omega t+\alpha + \frac{\pi}{2} \right)
\end{align}
$$
che, ricordando l'espressione [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriale]] di $a(t)$:
$$
\overline{A} = Ae^{j\alpha}
$$
si può riscrivere:
$$
\overline{C} = \omega  Ae^{j\left( \alpha+ \frac{\pi}{2} \right)}
$$
che, facendo alcuni semplici passaggi:
$$
\begin{align}
\overline{C} &= \omega  Ae^{j\left( \alpha+ \frac{\pi}{2} \right)} = \\
&= \omega A e^{j\alpha}e^\frac{j\pi}{2}= \\
&= \omega A e^{j\alpha}j= \\
&= j\omega \overline{A}
\end{align}
$$
```ad-Teo
title: Derivazione di un fasore

Derivare un [[#Fasore]] corrisponde quindi a moltiplicarlo per la quantità $j\omega$.
$
\frac{d}{dt}\overline{A} = j\omega\overline{A}
$


```

##### Integrazione

```ad-Teo
title: Ingegrazione di un fasore

Analogamente a quanto visto per la [[#Derivazione]], l'integrazione di un [[#Fasore]] si può ottenere semplicemente dividendolo per la quantità $j\omega$:
$
\int \overline{A} \, dt  = \frac{\overline{A}}{j\omega}
$

```
