---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/18-campo-magnetico-rotante-et/","tags":["UNI"]}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/18 - Campo magnetico rotante - ET\|18 - Campo magnetico rotante - ET]]

#UNI/ET/Domanda 

È data una [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET\|macchina per la conversione elettromeccanica dell'energia]] a 3 coppie polari, alimentata da un [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico\|Sistema trifase di correnti sinusoidali]].
- Stesso [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valore efficace]]
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|Sfasamento]] di 120°
- Somma dei fasori nulla

![18 - Macchina elettrica - trifase 2024-07-02 18.45.36.excalidraw.png](/img/user/Excalidraw/18%20-%20Macchina%20elettrica%20-%20trifase%202024-07-02%2018.45.36.excalidraw.png)


Le 3 correnti saranno pertanto sfasate di 120° sia nello spazio (l'angolo tra le spire) che nel tempo:
$$
\begin{cases}
i_{1}(t) &= \sqrt{2}I\sin(\omega t) \\
i_{2}(t) &= \sqrt{2}I\sin\left( \omega t- \frac{2}{3}\pi \right) \\
i_{3}(t) &= \sqrt{2}I\sin\left( \omega t - \frac{4}{3}\pi \right)
\end{cases}
$$
Presa una direzione qualunque come riferimento, dalla quale misuriamo un angolo $\theta$ (uno per ogni spira: $\theta_{1}, \theta_{2}, \theta_{3}$), il campo magnetico di induzione nel traferro si esprime in funzione di $\theta$ e di $t$.
Posto
$$
K \stackrel{\triangle}{=} \frac{4\sqrt{2}\mu_{0}NI}{2\pi \delta }
$$
i campi magnetici sono:
$$
\begin{cases}
B_{1}(\theta_{1},t) &= - K \sin(\omega t)\cos(\theta_{1}) \\
B_{2}(\theta_{2},t) &= - K \sin\left( \omega t - \frac{2}{3}\pi  \right)\cos(\theta_{2}) \\
B_{3}(\theta_{3},t) &= - K \sin(\omega t - \frac{4}{3}\pi )\cos(\theta_{3})
\end{cases}
$$
Al fine di sommare i contributi però, bisogna adottare lo stesso riferimento. Gli angoli $\theta$ saranno:
$$
\begin{cases}
\theta_{1} &= \theta \\
\theta_{2} &= \theta - 120° \\
\theta_{3} &= \theta - 240°
\end{cases}
$$
Sommando ora i 3 contributi si ottiene che, il **campo magnetico di induzione al traferro risultante** è:
$$
B_{tot}(\theta,t) = - \frac{3K}{2} \sin(\omega t-\theta )
$$
Che si osservi essere un campo **rotante**, di ampiezza massima pari a $\frac{3}{2}$ quella dei singoli campi

![Schermata 2024-07-02 alle 19.28.53.png](/img/user/Schermata%202024-07-02%20alle%2019.28.53.png)

Il cui andamento sulla macchina è:

![18 - Campo magnetico rotante 2024-07-02 19.29.16.excalidraw.png](/img/user/Excalidraw/18%20-%20Campo%20magnetico%20rotante%202024-07-02%2019.29.16.excalidraw.png)


Il campo statorico $B_{s}$ ruota a velocità angolare
$$
\omega_{s} = \frac{\omega}{p}
$$

