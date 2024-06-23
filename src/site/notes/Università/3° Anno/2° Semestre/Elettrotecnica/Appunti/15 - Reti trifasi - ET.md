---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/15-reti-trifasi-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET\|15 - Reti trifasi - ET]]

# Sistema trifase simmetrico

```ad-Definizione
title: Sistema trifase simmetrico 

Si definisce **sistema trifase simmetrico** un insieme di 3 grandezze [[13 - Funzioni sinusoidali e fasori - ET#Funzioni sinusoidali isofrequenziali|sinusoidali isofrequenziali]] di uguale ampiezza, sfasate reciprocamente di $\frac{2\pi}{3}$ ($120°$).
$
\begin{cases}
e_{1}(t) &= \sqrt{2} E\sin(\omega t) \\
e_{2}(t) &= \sqrt{2} E\sin\left( \omega t \mp \frac{2\pi}{3} \right) \\
e_{3}(t) &= \sqrt{2} E\sin\left( \omega t \mp \frac{4\pi}{3} \right) \\
\end{cases}
$

```


Si può dimostrare che:


```ad-Teo
title: Teorema

$
\sum\limits e_{i}() = 0
$
che riscritta in termini [[13 - Funzioni sinusoidali e fasori - ET#Fasore|fasoriali]]:
$
\begin{align}
\sum\limits \overline{E} &= 0 \\
\overline{E}_{1}+ \overline{E}_{2}+ \overline{E}_{3}&= 0
\end{align}
$

```



### Sistema trifase simmetrico diretto

![15 - Reti trifasi - ET 2024-06-22 18.26.29.excalidraw.png|450](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-22%2018.26.29.excalidraw.png)


```ad-Definizione
title: Sistema trifase simmetrico diretto

Un [[#Sistema trifase simmetrico]] si dice **diretto** se ciascuna grandezza risulta in [[13 - Funzioni sinusoidali e fasori - ET#Sfasamento|ritardo]] di 120° ($\left(-\frac{2\pi}{3}\right)$ rispetto alla precedente


```

### Sistema trifase simmetrico inverso

![15 - Reti trifasi - ET 2024-06-22 18.37.17.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-22%2018.37.17.excalidraw.png)


```ad-Definizione
title: Sistema trifase simmetrico inverso

Un [[#Sistema trifase simmetrico]] si dice **inverso** se ciascuna grandezza risulta in [[13 - Funzioni sinusoidali e fasori - ET#Sfasamento|ritardo]] di 120° ($\left(+\frac{2\pi}{3}\right)$ rispetto alla precedente.

```

## Collegamenti generatori-utilizzatori

Si considerino le 3 [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|reti]] *monofase* in figura ognuna caratterizzata da un [[Generatore ideale di tensione sinusoidale\|Generatore ideale di tensione sinusoidale]] $\overline{E}_{i}$ e un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Bipolo in regime sinusoidale e potenza\|bipolo]] di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenza]] $\dot Z_{i}$.

![15 - Reti trifasi - ET 2024-06-23 12.50.33.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2012.50.33.excalidraw.png)


Le 3 correnti sono rispettivamente:
$$
I_{1} = \frac{\overline{E}_{1}}{\dot Z_{1}}
\qquad\qquad
I_{2} = \frac{\overline{E}_{2}}{\dot Z_{2}}
\qquad\qquad
I_{3} = \frac{\overline{E}_{3}}{\dot Z_{3}}
$$












