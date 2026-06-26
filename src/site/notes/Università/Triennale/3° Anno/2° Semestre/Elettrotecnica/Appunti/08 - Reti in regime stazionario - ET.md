---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/08-reti-in-regime-stazionario-et/","tags":["UNI"],"dg-note-properties":{"aliases":["8 - Reti in regime stazionario - ET"],"Materia":"ET","Tipo":"T","Stato":"🟢 Fatto","Slide":null,"PDF":null,"Parents":["[[🔌 Elettrotecnica]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET\|08 - Reti in regime stazionario - ET]]

## Bipoli in serie

![08 - Reti in regime stazionario - ET 2024-06-15 17.54.36.excalidraw.png](/img/user/Excalidraw/08%20-%20Reti%20in%20regime%20stazionario%20-%20ET%202024-06-15%2017.54.36.excalidraw.png)
[[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-15 18.16.25.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-16 16.14.50.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 14.30.32.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 15.17.19.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 15.26.13.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 15.32.59.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 15.33.22.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-16 16.59.56.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-16 17.22.00.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-17 12.57.17.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-17 18.41.44.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-17 19.46.01.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 10.52.30.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 10.59.21.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/08 - Reti in regime stazionario - ET 2024-06-18 11.33.07.excalidraw\|🖋 Edit in Excalidraw]]

#### Condizione di adattamento del carico

La condizione di adattamento del carico è la condizione in cui la Potenza trasferita al carico è massima (e quindi lo è anche il [[#Rendimento]]).

Calcolando la derivata della [[03 - Introduzione allo studio delle reti elettriche - ET#Potenza erogata|potenza erogata]] e ponendola uguale a zero si può ricavare il suo massimo.
$$
P = VI = \frac{R_{u}E^{2}}{(R_{i}+R_{u})^{2}}
$$
Si deriva rispetto a $R_{u}$:
$$
\begin{align}
\frac{dP}{dR_{u}} &= \frac{E^{2}}{(R_{i}+R_{u})^{2}} - \frac{2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} = \\
&= \frac{E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2}}{(R_{i}+R_{u})^{3}} \stackrel{!}{=} 0 
\end{align}
$$
che quindi corrisponde a trovare:
$$
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} = 0
$$
che diventa
$$
\begin{align}
E^{2}(R_{i}+R_{u}) - 2R_{u}E^{2} &= 0 \\
R_{i}+R_{u}-2R_{u} &= 0 \\
R_{u} = R_{i}
\end{align}
$$
```ad-Teo
title: Condizione di adattamento del carico

La condizione di adattamento del carico si ha quando la resistenza del carico è uguale alla resistenza interna al generatore
$$
R_{u}= R_{i}
$$
In tale condizione valgono:
$$
\begin{align}
V &= \frac{V_{0}}{2} \\
I &= \frac{I_{cc}}{2} \\
\eta &= 0.5
\end{align}
$$
```


La stessa relazione vale quando il carico $R_{u}$ è alimentato da una generica [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|rete elettrica]] lineare ai nodi A e B. Rappresentando la rete con il [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Teorema di Thévenin\|teorema di Thévenin]] con $E_{eq} = E_{0}$ e $R_{eq} = R_{i}$, la condizione di adattamento è ancora $R_{u}= R_{i} =(R_{eq})$.

La potenza trasferita vale $P = \frac{V_{0}^{2}}{4R_{i}}$. Sul rendimento però non si può dire nulla in quanto il generatore equivalente non è significativo della rete reale dal punto di vista energetico.



</div></div>







