---
{"dg-publish":true,"permalink":"/condensatore/","tags":["UNI"]}
---

# [[Condensatore\|Condensatore]]

![Condensatore 2024-06-18 16.47.59.excalidraw.png](/img/user/Excalidraw/Condensatore%202024-06-18%2016.47.59.excalidraw.png)


Il condensatore è descritto dalla seguente legge che mette in relazione la ddp e la carica accumulata:
$$
Q(t) = Cv(t)
$$
dove:
- $C:$ [[Condensatore#Capacità\|#Capacità]]

## Capacità

```ad-Definizione
title: Capacità (C)

La capacità del condensatore è
$
C = \frac{\varepsilon_{0}\varepsilon_{r}S}d{} \qquad \rm \left[ \frac{C}{V} \right] = [F]
$
dove:
- $\varepsilon_{0}:$ [[Costante dielettrica nel vuoto]]
- $\varepsilon_{r}:$ Costante dielettrica tra le piastre del condensatore
- $d:$ Distanza tra le piastre
- $S:$ Area della superficie delle piastre
e si misura in Farad $[F]$.

```

## Corrente di spostamento

La corrente $i$ è detta **corrente di spostamento**:
$$
i = \frac{dQ}{dt} = C \frac{dv(t)}{dt}
$$
da cui
$$
v(t) = \frac{1}{C} \int_{0}^{t} i(t)\, dt
$$

## Regime sinusoidale

![Condensatore sinusoidale.excalidraw.png](/img/user/Excalidraw/Condensatore%20sinusoidale.excalidraw.png)


Il [[Condensatore\|Condensatore]], [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Convenzione dell'utilizzatore\|convenzionato da utilizzatore]], dotato di [[Condensatore#Capacità\|#Capacità]] costante $C$, rispetta sempre la relazione:
$$
i(t) = C \frac{dv(t)}{dt}
$$
dove
- $v(t) = V_{M}\sin(\omega t+\alpha) = \sqrt{2} V\sin(\omega t+\alpha)$

da cui si ricava la legge della corrente:
$$
i(t) = \omega C V_{M}\sin\left( \omega t + \beta + \frac{\pi}{2} \right) = I_{M}\sin\left( \omega t + \beta + \frac{\pi}{2} \right)
$$
Valgono quindi le seguenti relazioni:

```ad-Teo
title:
$
\frac{V_{M}}{I_{M}} = \frac{V}{I} = \frac{1}{\omega C}  \qquad \varphi=\alpha-\beta= - \frac{\pi}{2}
$
```


quindi la tensione, in un induttore a regime sinusoidale, si trova in *[[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|quadratura in ritardo]]* sulla corrente.

![Condensatore 2024-06-20 14.29.31.excalidraw.png](/img/user/Excalidraw/Condensatore%202024-06-20%2014.29.31.excalidraw.png)


Si osservi che la tensione e la corrente sono legate dal prodotto
$$
X_{C} =- \frac{1}{\omega C}
$$
che viene definito [[Condensatore#Reattanza capacitiva\|#Reattanza capacitiva]]

La [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza istantanea]] assorbita è sinusoidale di ampiezza $VI$. In un quarto di periodo è positiva e da luogo a lavoro assorbito immagazzinato in forma di energia capacitiva: $w_{C}(t) = C \frac{v^{2}}{2}$ che viene poi restituita nel quarto di periodo successivo.

Il [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|fattore di potenza]] $\cos(\varphi) = 0$ è nullo e quindi [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] assorbita $P=0$
$$
P= 0 \qquad Q=-A = -VI = X_{C}I^{2}
$$

___

Il condensatore in regime sinusoidale può essere descritto anche facendo riferimento alle grandezze [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriali]].
$$
\begin{align}
i(t) &\Longrightarrow \overline{I} = Ie^{j\beta} \\
v(t) &\Longrightarrow \overline{V} = Ve^{j\alpha}
\end{align}
$$
Il rapporto tra i fasori vale:
$$
\frac{\overline{V}}{\overline{I}} = \frac{V}{I}e^{j\varphi} = \frac{V}{I}e^{-j \frac{\pi}{2}} = -j \frac{1}{\omega C} = j X_{C}
$$

Pertanto, in termini fasoriali, è vera la relazione:
$$
\overline{V} = jX_{C}\overline{I}
$$
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


